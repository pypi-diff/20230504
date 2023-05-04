# Comparing `tmp/inductor-0.2.8.tar.gz` & `tmp/inductor-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/workspaces/inductor/dist/.tmp-oe8ppd00/inductor-0.2.8.tar", last modified: Mon Apr 17 10:13:58 2023, max compression
+gzip compressed data, was "/workspaces/inductor/dist/.tmp-yhav9rrz/inductor-0.2.9.tar", last modified: Thu May  4 21:40:45 2023, max compression
```

## Comparing `inductor-0.2.8.tar` & `inductor-0.2.9.tar`

### file list

```diff
@@ -1,610 +1,612 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:58.000000 inductor-0.2.8/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3130 2023-01-26 14:41:07.000000 inductor-0.2.8/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      153 2022-12-18 07:02:56.000000 inductor-0.2.8/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)      276 2023-04-17 10:13:58.000000 inductor-0.2.8/PKG-INFO
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    32836 2023-03-08 16:33:31.000000 inductor-0.2.8/inductor/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6459 2023-03-08 16:33:31.000000 inductor-0.2.8/inductor/cli.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/compute/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      169 2022-12-18 07:02:56.000000 inductor-0.2.8/inductor/compute/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1675 2023-03-08 16:33:31.000000 inductor-0.2.8/inductor/compute/common.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1747 2022-12-18 07:02:56.000000 inductor-0.2.8/inductor/compute/local.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10427 2023-03-23 19:54:50.000000 inductor-0.2.8/inductor/conftest.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/data/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      101 2022-12-18 07:02:56.000000 inductor-0.2.8/inductor/data/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/data/table/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      113 2022-12-18 07:02:56.000000 inductor-0.2.8/inductor/data/table/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    24069 2023-03-10 17:04:19.000000 inductor-0.2.8/inductor/data/table/dynamodb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    28123 2023-02-23 06:08:55.000000 inductor-0.2.8/inductor/data/table/mysql.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    30169 2023-02-23 06:08:55.000000 inductor-0.2.8/inductor/data/table/postgresql.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17688 2023-02-23 06:08:55.000000 inductor-0.2.8/inductor/data/table/snowflake.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22985 2023-02-23 06:08:55.000000 inductor-0.2.8/inductor/data/table/sqlite.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13842 2023-04-14 16:23:19.000000 inductor-0.2.8/inductor/data/table/table.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    36687 2023-04-14 16:23:19.000000 inductor-0.2.8/inductor/data/table/table_catalog.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4829 2023-03-08 16:33:31.000000 inductor-0.2.8/inductor/data/table/table_util.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3640 2023-04-14 16:23:19.000000 inductor-0.2.8/inductor/environment.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/ml/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      109 2022-12-18 07:02:56.000000 inductor-0.2.8/inductor/ml/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22685 2023-03-02 05:05:13.000000 inductor-0.2.8/inductor/ml/model_store.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/ui/
--rw-r--r--   0 vscode    (1000) vscode    (1000)   108271 2023-04-14 16:23:19.000000 inductor-0.2.8/inductor/ui/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/ui/frontend/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/ui/frontend/build/
--rw-r--r--   0 vscode    (1000) vscode    (1000)   102942 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/asset-manifest.json
--rw-r--r--   0 vscode    (1000) vscode    (1000)      153 2023-04-17 10:09:38.000000 inductor-0.2.8/inductor/ui/frontend/build/favicon.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)      751 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/index.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5347 2023-04-17 10:09:38.000000 inductor-0.2.8/inductor/ui/frontend/build/logo192.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9664 2023-04-17 10:09:38.000000 inductor-0.2.8/inductor/ui/frontend/build/logo512.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)      489 2023-04-17 10:09:38.000000 inductor-0.2.8/inductor/ui/frontend/build/manifest.json
--rw-r--r--   0 vscode    (1000) vscode    (1000)       67 2023-04-17 10:09:38.000000 inductor-0.2.8/inductor/ui/frontend/build/robots.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/ui/frontend/build/static/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4597 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10592 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)  1360865 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/main.742afa3c.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3257 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/main.742afa3c.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)  5214586 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/main.742afa3c.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8169 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9826 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1150 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2696 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1091 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1970 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1132 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1820 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1005 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1793 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2868 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3794 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1460 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3292 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8448 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9738 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5704 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8969 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1275 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1938 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2061 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2703 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1305 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2617 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8874 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15381 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      447 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arff.c5d78406.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      928 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arff.c5d78406.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4822 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11751 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1126 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1946 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1993 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3062 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7785 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25599 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9397 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10636 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1089 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2209 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5571 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10479 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1252 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2565 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6229 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12983 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2088 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2750 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1931 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4683 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      713 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1643 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1539 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3685 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      828 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1629 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2793 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6635 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      555 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1250 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      491 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brainfuck.373a8f58.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1157 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brainfuck.373a8f58.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1347 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2745 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1364 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2268 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2827 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3931 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2105 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4566 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1477 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2844 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6130 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13815 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2363 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3181 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      964 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1934 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3306 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4325 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10896 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11926 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5348 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6717 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1699 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4190 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2145 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3932 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3293 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5068 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4839 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10843 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5246 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11994 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6621 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22720 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9262 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    32789 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1483 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3553 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1468 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3657 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3511 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7049 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      329 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csv.3eb58e61.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      688 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csv.3eb58e61.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1292 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2502 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2477 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5019 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1843 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4336 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1113 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2398 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3687 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4618 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1498 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4000 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      860 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2874 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2595 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10400 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1089 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2155 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1836 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5561 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1464 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3762 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      631 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1360 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      619 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1561 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1204 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2303 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1904 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8613 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2097 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5052 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1267 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3252 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5609 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17469 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2267 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2534 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9993 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1245 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3378 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10315 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    29173 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      633 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1642 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1052 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2350 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1158 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2337 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1524 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2638 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2356 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4306 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3261 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12510 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1272 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2740 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      479 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gcode.d23c9ac3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1105 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gcode.d23c9ac3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1180 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2266 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      779 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1689 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15972 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12391 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      490 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_git.8814e653.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2604 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_git.8814e653.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3309 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6138 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8413 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8989 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1302 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2922 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1209 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2156 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      677 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1487 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2777 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9777 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1917 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4290 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6162 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15753 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2314 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9503 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3232 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5553 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1810 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3897 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1645 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3459 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3864 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7426 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      722 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1322 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      438 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hpkp.74d3b1ac.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      971 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hpkp.74d3b1ac.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      399 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hsts.f4e5dec7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      923 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hsts.f4e5dec7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2183 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7370 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1022 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1750 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1185 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1938 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2354 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7506 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3988 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7058 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1577 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2582 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      633 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3596 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5362 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      860 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2050 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1965 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2784 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1067 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1989 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2378 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5271 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4876 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14014 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1130 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4441 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4717 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9050 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1817 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6690 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      853 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1457 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1715 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2984 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1434 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3531 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2717 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6836 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2878 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    16647 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4057 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12093 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      708 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1624 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1222 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2972 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1023 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2428 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1030 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2247 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2688 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9233 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1297 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2961 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5913 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7403 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1229 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2426 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2190 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4788 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2666 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5293 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1794 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2970 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1295 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3325 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8946 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25523 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      931 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2525 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5616 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12658 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3526 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11416 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2910 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9236 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2219 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5171 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      804 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1584 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2768 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5680 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1428 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2736 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      851 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1662 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1385 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2413 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1202 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2159 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5490 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    19283 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3033 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8872 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1345 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6982 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      689 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1345 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1925 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4273 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17044 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    18305 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2341 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5232 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1302 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1860 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3680 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8613 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1134 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2044 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2304 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4030 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2053 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3050 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      823 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1568 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      534 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1078 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2049 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7158 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      954 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1736 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1259 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2425 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2224 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4993 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      984 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2577 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1393 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3093 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1523 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2748 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3968 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4996 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2905 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5972 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1428 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2926 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12128 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17309 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1908 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1075 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1975 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1107 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2686 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1691 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3919 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2168 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3951 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1620 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4108 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1061 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2603 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1513 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2837 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2488 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6656 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7750 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22085 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8201 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23130 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9480 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    28299 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6357 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8308 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2204 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3739 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2408 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4611 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      759 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1483 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      606 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1520 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1491 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4463 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      539 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1040 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1243 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2560 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3432 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4534 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3085 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8744 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2795 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6887 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3700 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6709 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2707 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4863 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5647 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9609 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2360 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4307 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1962 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4038 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1698 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4006 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1254 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2090 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2230 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7205 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      775 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1552 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4667 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10058 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1066 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2112 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1546 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4508 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      837 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1798 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4544 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5371 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3808 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8379 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1024 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2037 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      713 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1564 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1761 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4835 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3822 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8980 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2743 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6512 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7790 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17100 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1340 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3558 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3729 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8105 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4282 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8817 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1567 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4106 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7321 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    16385 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1617 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3717 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      907 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1991 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3431 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13007 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1795 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4250 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1325 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2139 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      960 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2458 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3037 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11612 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2224 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4321 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1964 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2913 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    33625 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    34751 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3514 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4573 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1340 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2627 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1782 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3922 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3990 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7867 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3272 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7429 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1012 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3428 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7557 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25986 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      900 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2806 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4843 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8564 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2700 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7260 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1761 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2946 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3785 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14076 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1218 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2896 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1853 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4129 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4518 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14101 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2620 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10005 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1164 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2589 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2319 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9303 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1565 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3551 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1654 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4076 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2065 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3463 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2652 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3930 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1486 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3810 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2127 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4495 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2236 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4464 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3921 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5335 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1496 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3628 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2357 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3453 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1587 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2520 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14461 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14997 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2183 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3191 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      887 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1883 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1462 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2361 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2484 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5515 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1408 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3490 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1128 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2249 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1602 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4465 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2158 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5043 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1922 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1376 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2063 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4182 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10979 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2213 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5936 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1343 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2565 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6304 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2927 2022-12-18 07:02:56.000000 inductor-0.2.8/inductor/util.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      276 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)    61729 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       46 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      454 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      341 2023-03-08 16:33:31.000000 inductor-0.2.8/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      902 2023-04-17 10:13:58.000000 inductor-0.2.8/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-04 21:40:45.000000 inductor-0.2.9/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3130 2023-01-26 14:41:07.000000 inductor-0.2.9/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      153 2022-12-18 07:02:56.000000 inductor-0.2.9/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      301 2023-05-04 21:40:45.000000 inductor-0.2.9/PKG-INFO
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-04 21:40:41.000000 inductor-0.2.9/inductor/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    33831 2023-05-04 13:47:10.000000 inductor-0.2.9/inductor/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6459 2023-03-08 16:33:31.000000 inductor-0.2.9/inductor/cli.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-04 21:40:41.000000 inductor-0.2.9/inductor/compute/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      169 2022-12-18 07:02:56.000000 inductor-0.2.9/inductor/compute/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1675 2023-03-08 16:33:31.000000 inductor-0.2.9/inductor/compute/common.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1747 2022-12-18 07:02:56.000000 inductor-0.2.9/inductor/compute/local.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10427 2023-03-23 19:54:50.000000 inductor-0.2.9/inductor/conftest.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-04 21:40:41.000000 inductor-0.2.9/inductor/data/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      101 2022-12-18 07:02:56.000000 inductor-0.2.9/inductor/data/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-04 21:40:42.000000 inductor-0.2.9/inductor/data/table/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      113 2022-12-18 07:02:56.000000 inductor-0.2.9/inductor/data/table/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    16558 2023-05-03 16:16:15.000000 inductor-0.2.9/inductor/data/table/bigquery.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    24069 2023-03-10 17:04:19.000000 inductor-0.2.9/inductor/data/table/dynamodb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6622 2023-05-01 07:26:52.000000 inductor-0.2.9/inductor/data/table/mysql.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    30169 2023-04-27 17:13:52.000000 inductor-0.2.9/inductor/data/table/postgresql.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17688 2023-02-23 06:08:55.000000 inductor-0.2.9/inductor/data/table/snowflake.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    33977 2023-05-01 06:29:51.000000 inductor-0.2.9/inductor/data/table/sqlalchemy.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22985 2023-02-23 06:08:55.000000 inductor-0.2.9/inductor/data/table/sqlite.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14388 2023-04-27 13:07:41.000000 inductor-0.2.9/inductor/data/table/table.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    39479 2023-05-03 16:16:15.000000 inductor-0.2.9/inductor/data/table/table_catalog.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4829 2023-03-08 16:33:31.000000 inductor-0.2.9/inductor/data/table/table_util.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4272 2023-05-04 13:47:10.000000 inductor-0.2.9/inductor/environment.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-04 21:40:42.000000 inductor-0.2.9/inductor/ml/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      109 2022-12-18 07:02:56.000000 inductor-0.2.9/inductor/ml/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    26592 2023-04-26 23:04:53.000000 inductor-0.2.9/inductor/ml/model_store.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-04 21:40:42.000000 inductor-0.2.9/inductor/ui/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   108263 2023-04-26 23:04:53.000000 inductor-0.2.9/inductor/ui/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-04 21:40:41.000000 inductor-0.2.9/inductor/ui/frontend/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-04 21:40:42.000000 inductor-0.2.9/inductor/ui/frontend/build/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   102942 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/asset-manifest.json
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      153 2023-05-04 21:38:12.000000 inductor-0.2.9/inductor/ui/frontend/build/favicon.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      751 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/index.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5347 2023-05-04 21:38:12.000000 inductor-0.2.9/inductor/ui/frontend/build/logo192.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9664 2023-05-04 21:38:12.000000 inductor-0.2.9/inductor/ui/frontend/build/logo512.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      489 2023-05-04 21:38:12.000000 inductor-0.2.9/inductor/ui/frontend/build/manifest.json
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       67 2023-05-04 21:38:12.000000 inductor-0.2.9/inductor/ui/frontend/build/robots.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-04 21:40:41.000000 inductor-0.2.9/inductor/ui/frontend/build/static/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-04 21:40:45.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4597 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10592 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)  1360865 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/main.742afa3c.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3257 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/main.742afa3c.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)  5214586 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/main.742afa3c.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8169 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9826 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1150 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2696 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1091 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1970 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1132 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1820 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1005 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1793 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2868 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3794 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1460 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3292 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8448 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9738 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5704 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8969 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1275 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1938 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2061 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2703 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1305 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2617 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8874 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15381 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      447 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arff.c5d78406.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      928 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arff.c5d78406.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4822 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11751 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1126 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1946 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1993 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3062 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7785 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    25599 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9397 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10636 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1089 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2209 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5571 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10479 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1252 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2565 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6229 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12983 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2088 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2750 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1931 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4683 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      713 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1643 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1539 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3685 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      828 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1629 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2793 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6635 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      555 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1250 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      491 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brainfuck.373a8f58.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1157 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brainfuck.373a8f58.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1347 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2745 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1364 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2268 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2827 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3931 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2105 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4566 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1477 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2844 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6130 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13815 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2363 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3181 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      964 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1934 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3306 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4325 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10896 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11926 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5348 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6717 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1699 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4190 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2145 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3932 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3293 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5068 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4839 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10843 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5246 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11994 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6621 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22720 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9262 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    32789 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1483 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3553 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1468 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3657 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3511 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7049 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      329 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csv.3eb58e61.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      688 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csv.3eb58e61.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1292 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2502 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2477 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5019 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1843 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4336 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1113 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2398 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3687 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4618 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1498 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4000 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      860 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2874 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2595 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10400 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1089 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2155 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1836 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5561 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1464 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3762 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      631 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1360 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      619 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1561 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1204 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2303 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1904 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8613 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2097 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5052 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1267 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3252 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5609 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17469 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2267 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2534 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9993 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1245 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3378 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10315 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    29173 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      633 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1642 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1052 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2350 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1158 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2337 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1524 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2638 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2356 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4306 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3261 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12510 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1272 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2740 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      479 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gcode.d23c9ac3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1105 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gcode.d23c9ac3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1180 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2266 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      779 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1689 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15972 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12391 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      490 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_git.8814e653.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2604 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_git.8814e653.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3309 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6138 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8413 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8989 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1302 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2922 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1209 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2156 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      677 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1487 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2777 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9777 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1917 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4290 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6162 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15753 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2314 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9503 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3232 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5553 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1810 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3897 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1645 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3459 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3864 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7426 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      722 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1322 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      438 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hpkp.74d3b1ac.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      971 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hpkp.74d3b1ac.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      399 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hsts.f4e5dec7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      923 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hsts.f4e5dec7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2183 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7370 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1022 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1750 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1185 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1938 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2354 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7506 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3988 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7058 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1577 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2582 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      633 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3596 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5362 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      860 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2050 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1965 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2784 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1067 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1989 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2378 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5271 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4876 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14014 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1130 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4441 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4717 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9050 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1817 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6690 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      853 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1457 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1715 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2984 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1434 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3531 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2717 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6836 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2878 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    16647 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4057 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12093 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      708 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1624 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1222 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2972 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1023 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2428 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1030 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2247 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2688 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9233 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1297 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2961 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5913 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7403 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1229 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2426 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2190 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4788 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2666 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5293 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1794 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2970 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1295 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3325 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8946 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    25523 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      931 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2525 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5616 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12658 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3526 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11416 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2910 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9236 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2219 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5171 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      804 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1584 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2768 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5680 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1428 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2736 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      851 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1662 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1385 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2413 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1202 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2159 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5490 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    19283 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3033 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8872 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1345 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6982 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      689 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1345 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1925 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4273 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17044 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    18305 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2341 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5232 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1302 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1860 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3680 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8613 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1134 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2044 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2304 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4030 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2053 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3050 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      823 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1568 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      534 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1078 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2049 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7158 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      954 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1736 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1259 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2425 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2224 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4993 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      984 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2577 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1393 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3093 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1523 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2748 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3968 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4996 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2905 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5972 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1428 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2926 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12128 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17309 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1908 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1075 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1975 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1107 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2686 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1691 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3919 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2168 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3951 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1620 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4108 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1061 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2603 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1513 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2837 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2488 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6656 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7750 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22085 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8201 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    23130 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9480 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    28299 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6357 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8308 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2204 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3739 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2408 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4611 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      759 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1483 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      606 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1520 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1491 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4463 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      539 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1040 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1243 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2560 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3432 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4534 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3085 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8744 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2795 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6887 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3700 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6709 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2707 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4863 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5647 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9609 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2360 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4307 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1962 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4038 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1698 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4006 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1254 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2090 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2230 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7205 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      775 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1552 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4667 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10058 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1066 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2112 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1546 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4508 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      837 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1798 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4544 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5371 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3808 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8379 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1024 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2037 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      713 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1564 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1761 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4835 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3822 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8980 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2743 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6512 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7790 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17100 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1340 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3558 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3729 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8105 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4282 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8817 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1567 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4106 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7321 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    16385 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1617 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3717 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      907 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1991 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3431 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13007 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1795 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4250 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1325 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2139 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      960 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2458 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3037 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11612 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2224 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4321 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1964 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2913 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    33625 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    34751 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3514 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4573 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1340 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2627 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1782 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3922 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3990 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7867 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3272 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7429 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1012 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3428 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7557 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    25986 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      900 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2806 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4843 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8564 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2700 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7260 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1761 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2946 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3785 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14076 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1218 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2896 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1853 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4129 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4518 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14101 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2620 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10005 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1164 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2589 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2319 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9303 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1565 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3551 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1654 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4076 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2065 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3463 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2652 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3930 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1486 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3810 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2127 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4495 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2236 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4464 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3921 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5335 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1496 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3628 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2357 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3453 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1587 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2520 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14461 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14997 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2183 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3191 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      887 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1883 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1462 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2361 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2484 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5515 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1408 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3490 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1128 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2249 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1602 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4465 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2158 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5043 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1922 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1376 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2063 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4182 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10979 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2213 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5936 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1343 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2565 2023-05-04 21:38:29.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6304 2023-05-04 21:38:30.000000 inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2927 2022-12-18 07:02:56.000000 inductor-0.2.9/inductor/util.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-04 21:40:41.000000 inductor-0.2.9/inductor.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      301 2023-05-04 21:40:41.000000 inductor-0.2.9/inductor.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    61795 2023-05-04 21:40:41.000000 inductor-0.2.9/inductor.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-04 21:40:41.000000 inductor-0.2.9/inductor.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       46 2023-05-04 21:40:41.000000 inductor-0.2.9/inductor.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      590 2023-05-04 21:40:41.000000 inductor-0.2.9/inductor.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-04 21:40:41.000000 inductor-0.2.9/inductor.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      341 2023-03-08 16:33:31.000000 inductor-0.2.9/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1043 2023-05-04 21:40:45.000000 inductor-0.2.9/setup.cfg
```

### Comparing `inductor-0.2.8/LICENSE` & `inductor-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/__init__.py` & `inductor-0.2.9/inductor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """The entrypoint for creating Inductor apps."""
 
 from dataclasses import dataclass
 import functools
 import inspect
 import json
 import os
+import posixpath
 import threading
 import traceback
 from typing import Any, Callable, Coroutine, Dict, Iterable, List, Optional, Tuple, Union
 from urllib import parse
 
 from apscheduler.schedulers import asyncio as apscheduler_asyncio
 from apscheduler.triggers import cron as apscheduler_cron
@@ -278,14 +279,25 @@
                 else:
                     count = apps_table.select(
                         "COUNT(*)", "WHERE app_id = {app_id}").value()
                     if count != 1:
                         del apps_table[self._env.app_name]
             # Retrieve app ID
             self._app_id = apps_table[self._env.app_name]["app_id"]
+            # Construct object store URL for this app
+            if self._env.object_store_url.startswith("file://"):
+                self._object_store_url = os.path.join(
+                    self._env.object_store_url, self._app_id)
+            elif self._env.object_store_url.startswith(("s3://", "gs://")):
+                self._object_store_url = posixpath.join(
+                    self._env.object_store_url, self._app_id)
+            else:
+                raise ValueError(
+                    "Unrecognized environment object_store_url prefix: " +
+                    self._env.object_store_url)
             # Initialize table storing state for unique id generation
             unique_id_state_table = table_util.table_from_url(
                 database_url=self._env.database_url,
                 table_name=f"inductor_app_{self._app_id}_uid",
                 primary_key_column="universe_id")
             unique_id_state_table.set(0, {"value": 0}, skip_if_exists=True)
         else:
@@ -543,32 +555,40 @@
         """Returns this app's ModelStore."""
         if isinstance(self._env, environment.Local):
             return model_store.LocalModelStore(
                 self._model_storage_dir,
                 self._internal_tables["ml_model_metadata"],
                 self._unique_id_gen)
         elif isinstance(self._env, environment.Server):
-            if self._env.object_store_url.startswith("file://"):
+            if self._object_store_url.startswith("file://"):
                 return model_store.LocalModelStore(
                     os.path.join(
-                        self._env.object_store_url[len("file://"):],
+                        self._object_store_url[len("file://"):],
                         "ml",
                         "models"),
                     self._internal_tables["ml_model_metadata"],
                     self._unique_id_gen)
-            elif self._env.object_store_url.startswith("s3://"):
-                s3_url = self._env.object_store_url
+            elif self._object_store_url.startswith("s3://"):
+                s3_url = self._object_store_url
                 if not s3_url.endswith("/"):
                     s3_url += "/"
                 return model_store.S3ModelStore(
                     s3_url + "ml/models/",
                     self._internal_tables["ml_model_metadata"],
                     self._unique_id_gen)
+            elif self._object_store_url.startswith("gs://"):
+                gcs_url = self._object_store_url
+                if not gcs_url.endswith("/"):
+                    gcs_url += "/"
+                return model_store.GCSModelStore(
+                    gcs_url + "ml/models/",
+                    self._internal_tables["ml_model_metadata"],
+                    self._unique_id_gen)
             else:
-                raise RuntimeError(
+                raise ValueError(
                     "Unrecognized environment object_store_url prefix: " +
                     self._env.object_store_url)
         else:
             raise TypeError(f"Unsupported env type ({type(self._env)})")
 
     def __call__(
         self,
```

### Comparing `inductor-0.2.8/inductor/cli.py` & `inductor-0.2.9/inductor/cli.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/compute/common.py` & `inductor-0.2.9/inductor/compute/common.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/compute/local.py` & `inductor-0.2.9/inductor/compute/local.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/conftest.py` & `inductor-0.2.9/inductor/conftest.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/data/table/dynamodb.py` & `inductor-0.2.9/inductor/data/table/dynamodb.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/data/table/mysql.py` & `inductor-0.2.9/inductor/data/table/postgresql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,108 @@
 # Copyright 2022 Inductor, Inc.
 
-"""Abstractions for MySQL tables."""
+"""Abstractions for PostgreSQL tables."""
 
 import datetime
 import re
 import sys  # pylint: disable=unused-import
 from typing import Any, Dict, Iterable, Optional, Tuple, Union
 
-import pymysql
+import psycopg2
+from psycopg2 import errorcodes
+from psycopg2 import extras
 
 from inductor.data.table import table
 
-# Name of empty placeholder column used to ensure that MySQL tables never
+# Name of empty placeholder column used to ensure that PostgreSQL tables never
 # contain no columns
 _PLACEHOLDER_COLUMN = "inductor_placeholder_column"
 
 # Suffix appended to names of columns that thus far contain only null values.
 _ALL_NULL_COLUMN_SUFFIX = "__allnull__"
 
 
 def _clean_row_dict(row_dict: table.Row) -> table.Row:
-    """Cleans a raw row dictionary returned by a pymysql.cursors.DictCursor.
+    """Returns a copy of row_dict with modifications.
 
     Args:
-        row: A raw row dictionary returned by a pymysql.cursors.DictCursor.
+        row: A raw row dictionary returned by a psycopg2.cursors.DictCursor.
 
     Returns:
-        A new dictionary containing the cleaned contents of row_dict.
+        A new dictionary containing the same contents as row_dict, but with
+        the following modifications:
+            - The placeholder column, _PLACEHOLDER_COLUMN, is removed.
+            - Columns with names ending in _ALL_NULL_COLUMN_SUFFIX are renamed
+                to remove the suffix.
     """
     clean_row_dict = {}
     for key in row_dict.keys():
         if key != _PLACEHOLDER_COLUMN:
             if key.endswith(_ALL_NULL_COLUMN_SUFFIX):
                 clean_row_dict[
                     key[:-len(_ALL_NULL_COLUMN_SUFFIX)]] = row_dict[key]
             else:
                 clean_row_dict[key] = row_dict[key]
     return clean_row_dict
 
 
+def _standardize_output(value: Any) -> Any:
+    """Converts values from PostgreSQL to their original Python data types.
+
+    Converts memoryview objects to bytes objects.
+
+    Args:
+        value: The value to convert.
+
+    Returns:
+        The converted value.
+    """
+    if isinstance(value, memoryview):
+        return bytes(value)
+    elif isinstance(value, dict):
+        return {
+            k: _standardize_output(v)
+            for k, v in value.items()}
+    elif isinstance(value, set):
+        return set(
+            _standardize_output(item)
+            for item in value)
+    elif isinstance(value, list):
+        return [
+            _standardize_output(item)
+            for item in value]
+    else:
+        return value
+
+
 def _format_metadata(metadata: Dict[str, Any]) -> Dict[str, Any]:
-    """Formats metadata to have the right params for MysqlTable.
+    """Formats metadata to have the right params for PostgresqlTable.
 
     Args:
-        metadata: Metadata representing a MysqlTable.
+        metadata: Metadata representing a PostgresqlTable.
     """
     table_metadata = metadata.copy()
-    if "mysql_password" in table_metadata:
-        table_metadata["password"] = table_metadata["mysql_password"]
-        del table_metadata["mysql_password"]
+    if "postgresql_password" in table_metadata:
+        table_metadata["password"] = table_metadata["postgresql_password"]
+        del table_metadata["postgresql_password"]
     return table_metadata
 
 
-class MysqlView(table.Table):
-    """A view of a MySQL table."""
+class PostgresqlView(table.Table):
+    """A view of a PostgreSQL table."""
 
     def __init__(
         self,
-        parent: "MysqlTable",
+        parent: "PostgresqlTable",
         query: table.SqlSelectQuery):
-        """Constructs a new MysqlView instance.
+        """Constructs a new PostgresqlView instance.
 
         Args:
-            parent: The underlying MysqlTable of which this instance is a view.
+            parent: The underlying PostgresqlTable of which
+                this instance is a view.
             query: The query (over parent) defining this view.
         """
         self._parent = parent
         self._query = query
 
     def _query_string(self) -> Tuple[str, Tuple[Any]]:
         """Returns the SQL query string and values underlying this view."""
@@ -74,58 +110,61 @@
         return self._query.to_sql_query_string(self._parent._table_name)
 
     def __iter__(self) -> Iterable[table.Row]:
         """See base class."""
         query_string, query_values = self._query_string()
         rows = []
         try:
-            with self._parent._connection.cursor() as cursor:
+            with self._parent._connection.cursor() as cursor:  # pylint: disable=protected-access
                 cursor.execute(query_string, query_values)
                 row_dict = cursor.fetchone()
                 while row_dict is not None:
                     if self._parent._auto_ddl:  # pylint: disable=protected-access
                         row_dict = _clean_row_dict(row_dict)
+                    row_dict = _standardize_output(row_dict)
                     rows.append(row_dict)
                     row_dict = cursor.fetchone()
             self._parent._connection.commit()  # pylint: disable=protected-access
-        except pymysql.MySQLError as error:
+        except psycopg2.Error as error:
             self._parent._connection.rollback()  # pylint: disable=protected-access
             with self._parent._connection.cursor() as cursor:  # pylint: disable=protected-access
                 cursor.execute(
                     f"SELECT COUNT(*) AS c FROM {self._parent._table_name}")  # pylint: disable=protected-access
                 total_num_rows = cursor.fetchone()["c"]
             self._parent._connection.commit()  # pylint: disable=protected-access
             if total_num_rows == 0:
                 rows = []
             else:
                 raise error
         return rows.__iter__()
 
     def first_row(self) -> Optional[table.Row]:
         """See base class."""
+        query_string, query_values = self._query_string()
         try:
             with self._parent._connection.cursor() as cursor:  # pylint: disable=protected-access
-                query_string, query_values = self._query_string()
                 cursor.execute(
                     f"SELECT * FROM ({query_string}) AS subquery LIMIT 1",
                     query_values)
                 row_dict = cursor.fetchone()
             self._parent._connection.commit()  # pylint: disable=protected-access
-        except pymysql.MySQLError as error:
+        except psycopg2.Error as error:
             self._parent._connection.rollback()  # pylint: disable=protected-access
             with self._parent._connection.cursor() as cursor:  # pylint: disable=protected-access
                 cursor.execute(
                     f"SELECT COUNT(*) AS c FROM {self._parent._table_name}")  # pylint: disable=protected-access
                 total_num_rows = cursor.fetchone()["c"]
             self._parent._connection.commit()  # pylint: disable=protected-access
             if total_num_rows == 0:
                 return None
             raise error
-        if row_dict is not None and self._parent._auto_ddl:  # pylint: disable=protected-access
-            row_dict = _clean_row_dict(row_dict)
+        if row_dict is not None:
+            if self._parent._auto_ddl:  # pylint: disable=protected-access
+                row_dict = _clean_row_dict(row_dict)
+            row_dict = _standardize_output(row_dict)
         return row_dict
 
     @property
     def columns(self) -> Iterable[str]:
         """See base class."""
         row = self.first_row()
         return list(row.keys()) if row is not None else []
@@ -135,33 +174,33 @@
         return NotImplementedError()
 
     @staticmethod
     def from_metadata(metadata: Dict[str, Any]) -> table.Table:
         return NotImplementedError()
 
 
-class MysqlTable(table.SqlQueryable, table.Appendable):
-    """A Table backed by a MySQL table."""
+class PostgresqlTable(table.SqlQueryable, table.Appendable):
+    """A Table backed by a PostgreSQL table."""
 
     def __init__(
         self,
         host: str,
         user: str,
         password: str,
         database: str,
         table_name: str,
         indexed_columns: Iterable[str] = tuple(),
         port: Optional[int] = None,
         auto_ddl: bool = True):
-        """Constructs a new MysqlTable instance.
+        """Constructs a new PostgresqlTable instance.
 
         Args:
-            host: Name of database server host hosting the MySQL database
+            host: Name of database server host hosting the PostgreSQL database
                 containing this table.
-            user: MySQL database server username.
+            user: PostgreSQL database server username.
             password: Password for user.
             database: Name of database containing table.
             table_name: Name of table in database given by preceding arguments.
             indexed_columns: Names of columns that should be indexed for faster
                 queries.
             port: Optionally, the port on which to connect to the database
                 server.
@@ -169,75 +208,75 @@
                 execute DDL commands to create the table and add and modify
                 columns.  If False, then no processing of retrieved rows to
                 account for prior automatic DDL is performed.
         """
         self._connection_params = {
             "host": host, "user": user,
             "password": password, "database": database,
-            "cursorclass": pymysql.cursors.DictCursor
+            "cursor_factory": extras.RealDictCursor
         }
-        if port:
+        if port is not None:
             self._connection_params["port"] = port
         self._table_name = table_name
         self._indexed_columns = list(indexed_columns)
         self._auto_ddl = auto_ddl
-        self._connection = pymysql.connect(**self._connection_params)
+        self._connection = psycopg2.connect(**self._connection_params)
         if self._auto_ddl:
             with self._connection.cursor() as cursor:
                 cursor.execute(
                     f"CREATE TABLE IF NOT EXISTS {self._table_name} "
                     f"({_PLACEHOLDER_COLUMN} INTEGER)")
             self._connection.commit()
 
     def __del__(self):
         """Closes self._connection as necessary on object destruction."""
-        if (self._connection.open and
+        if (not self._connection.closed and
             # To ensure that the Python interpreter is not currently exiting
-            # (self._connection.close() here raises an exception if called while
-            # interpreter is exiting).
+            # (self._connection.close() here may raise an exception if called
+            # while interpreter is exiting).
             "sys" in globals() and
             hasattr("sys", "modules")):
             self._connection.close()
 
     def __iter__(self) -> Iterable[table.Row]:
         """See base class."""
-        return MysqlView(self, table.SqlSelectQuery("*")).__iter__()
+        return PostgresqlView(self, table.SqlSelectQuery("*")).__iter__()
 
     def first_row(self) -> Optional[table.Row]:
         """See base class."""
-        return MysqlView(self, table.SqlSelectQuery("*")).first_row()
+        return PostgresqlView(self, table.SqlSelectQuery("*")).first_row()
 
     @property
     def columns(self) -> Iterable[str]:
         """See base class."""
         row = self.first_row()
         return list(row.keys()) if row is not None else []
 
     def to_metadata(self) -> Dict[str, Any]:
         """See base class."""
         metadata = self._connection_params.copy()
-        del metadata["cursorclass"]
+        del metadata["cursor_factory"]
         del metadata["password"]
         metadata["table_name"] = self._table_name
         metadata["indexed_columns"] = self._indexed_columns
         metadata["auto_ddl"] = self._auto_ddl
         return metadata
 
     @staticmethod
-    def from_metadata(metadata: Dict[str, Any]) -> "MysqlTable":
+    def from_metadata(metadata: Dict[str, Any]) -> "PostgresqlTable":
         """See base class."""
-        return MysqlTable(**_format_metadata(metadata))
+        return PostgresqlTable(**_format_metadata(metadata))
 
     def indexed_columns(self) -> Iterable[str]:
         """See base class."""
         return self._indexed_columns.copy()
 
-    def select(self, expression: str, after_from: str = "") -> MysqlView:
+    def select(self, expression: str, after_from: str = "") -> PostgresqlView:
         """See base class."""
-        return MysqlView(
+        return PostgresqlView(
             self,
             table.SqlSelectQuery(
                 expression=expression, after_from=after_from, placeholder="%s"))
 
     def _add_table_columns(self, rows: Iterable[table.Row]):
         """Adds columns to underlying table for any new columns in rows.
 
@@ -245,19 +284,19 @@
             rows: New rows based upon which to update table columns.
         """
         if not self._auto_ddl:
             return
         # Determine set of existing column names
         existing_col_names = set()
         with self._connection.cursor() as cursor:
-            cursor.execute(f"SHOW COLUMNS FROM {self._table_name}")
-            for row in cursor.fetchall():
-                col_name = row["Field"]
-                if col_name != _PLACEHOLDER_COLUMN:
-                    existing_col_names.add(col_name)
+            cursor.execute(f"SELECT * FROM {self._table_name} LIMIT 0")
+            for col in cursor.description:
+                if col.name != _PLACEHOLDER_COLUMN:
+                    existing_col_names.add(col.name)
+        self._connection.commit()
         # Add table columns as necessary
         for row in rows:
             for col_name in row.keys():
                 if (col_name not in existing_col_names
                     or (row[col_name] is not None and
                     col_name + _ALL_NULL_COLUMN_SUFFIX
                     in existing_col_names)):
@@ -285,124 +324,115 @@
                                 f"{col_name} TEXT DEFAULT NULL")
                             cursor.execute(
                                 f"ALTER TABLE {self._table_name} ADD COLUMN "
                                 f"{col_name_all_null} TEXT DEFAULT NULL")
                         existing_col_names.add(col_name)
                         existing_col_names.add(col_name_all_null)
                     else:
-                        index_prefix_clause = ""
                         if isinstance(value, bool):
-                            mysql_type = "BOOLEAN"
+                            postgresql_type = "BOOLEAN"
                         elif isinstance(value, int):
-                            mysql_type = "INTEGER"
+                            postgresql_type = "INTEGER"
                         elif isinstance(value, float):
-                            mysql_type = "DOUBLE"
+                            postgresql_type = "DOUBLE PRECISION"
                         elif isinstance(value, str):
-                            mysql_type = "TEXT"
-                            index_prefix_clause = "(300)"
-                            if (isinstance(self, MysqlKeyedTable) and
-                                # pylint: disable-next=no-member
-                                col_name == self.primary_key_column()):
-                                mysql_type = "VARCHAR(255)"
-                                index_prefix_clause = "(255)"
+                            postgresql_type = "TEXT"
                         elif isinstance(value, bytes):
-                            mysql_type = "BLOB"
-                            index_prefix_clause = "(600)"
+                            postgresql_type = "BYTEA"
                         elif isinstance(value, datetime.datetime):
-                            mysql_type = "DATETIME"
+                            postgresql_type = "TIMESTAMP"
                         elif isinstance(value, datetime.date):
-                            mysql_type = "DATE"
+                            postgresql_type = "DATE"
                         else:
                             raise TypeError(
                                 f"Unsupported value type: {type(value)}")
                         with self._connection.cursor() as cursor:
                             if col_name in existing_col_names:
                                 cursor.execute(
                                     f"ALTER TABLE {self._table_name} "
                                     f"DROP COLUMN "
                                     f"{col_name + _ALL_NULL_COLUMN_SUFFIX}")
                                 existing_col_names.remove(
                                     col_name + _ALL_NULL_COLUMN_SUFFIX)
                                 cursor.execute(
                                     f"ALTER TABLE {self._table_name} "
-                                    f"CHANGE COLUMN {col_name} "
-                                    f"{col_name} {mysql_type} "
-                                    "DEFAULT NULL")
+                                    f"ALTER COLUMN {col_name} "
+                                    f"TYPE {postgresql_type} "
+                                    f"USING {col_name}::{postgresql_type}")
                             else:
-                                if (isinstance(self, MysqlKeyedTable) and
-                                    # pylint: disable-next=no-member
-                                    col_name == self.primary_key_column()):
-                                    cursor.execute(
-                                        f"ALTER TABLE {self._table_name} "
-                                        f"ADD COLUMN {col_name} {mysql_type}")
-                                else:
-                                    cursor.execute(
-                                        f"ALTER TABLE {self._table_name} "
-                                        f"ADD COLUMN {col_name} {mysql_type} "
-                                        "DEFAULT NULL")
+                                cursor.execute(
+                                    f"ALTER TABLE {self._table_name} "
+                                    f"ADD COLUMN {col_name} {postgresql_type} "
+                                    "DEFAULT NULL")
                                 existing_col_names.add(col_name)
                                 if (col_name + _ALL_NULL_COLUMN_SUFFIX in
                                     existing_col_names):
                                     cursor.execute(
                                         f"ALTER TABLE {self._table_name} "
                                         "DROP COLUMN "
                                         f"{col_name + _ALL_NULL_COLUMN_SUFFIX}")
                                     existing_col_names.remove(
                                         col_name + _ALL_NULL_COLUMN_SUFFIX)
                             if col_name in self._indexed_columns:
                                 cursor.execute(
                                     "CREATE INDEX "
                                     f"{self._table_name}__{col_name}_index "
                                     f"ON {self._table_name} "
-                                    f"({col_name}{index_prefix_clause})")
-                            if (isinstance(self, MysqlKeyedTable) and
+                                    f"({col_name})")
+                            if (isinstance(self, PostgresqlKeyedTable) and
                                 # pylint: disable=no-member
                                 col_name == self.primary_key_column()):
                                 # pylint: enable=no-member
                                 cursor.execute(
                                     f"ALTER TABLE {self._table_name} "
                                     f"ADD PRIMARY KEY ({col_name})")
                         self._connection.commit()
 
     def extend(self, rows: Iterable[table.Row]):
         """See base class."""
         self._add_table_columns(rows)
         with self._connection.cursor() as cursor:
             for row in rows:
-                col_names = [k for k, v in row.items() if v is not None]
-                col_names_clause = ",".join(col_names)
-                values_clause = ",".join(["%s" for _ in col_names])
-                cursor.execute(
-                    f"REPLACE INTO {self._table_name} "
-                    f"({col_names_clause}) "
-                    f"VALUES({values_clause})",
-                    tuple(row[c] for c in col_names))
+                all_values_none = all(value is None for value in row.values())
+                if all_values_none:
+                    cursor.execute(
+                        f"INSERT INTO {self._table_name} "
+                        f"DEFAULT VALUES")
+                else:
+                    col_names = [k for k, v in row.items() if v is not None]
+                    col_names_clause = ",".join(col_names)
+                    values_clause = ",".join(["%s" for _ in col_names])
+                    cursor.execute(
+                        f"INSERT INTO {self._table_name} "
+                        f"({col_names_clause}) "
+                        f"VALUES({values_clause})",
+                        tuple(row[c] for c in col_names))
         self._connection.commit()
 
 
-class MysqlKeyedTable(MysqlTable, table.WithPrimaryKey):
-    """A MysqlTable having a primary key."""
+class PostgresqlKeyedTable(PostgresqlTable, table.WithPrimaryKey):
+    """A PostgresqlTable having a primary key."""
 
     def __init__(
         self,
         host: str,
         user: str,
         password: str,
         database: str,
         table_name: str,
         primary_key_column: str,
         indexed_columns: Iterable[str] = tuple(),
         port: Optional[int] = None,
         auto_ddl: bool = True):
-        """Constructs a new MysqlKeyedTable instance.
+        """Constructs a new PostgresqlKeyedTable instance.
 
         Args:
-            host: Name of database server host hosting the MySQL database
+            host: Name of database server host hosting the PostgreSQL database
                 containing this table.
-            user: MySQL database server username.
+            user: PostgreSQL database server username.
             password: Password for user.
             database: Name of database containing table.
             table_name: Name of table in database given by preceding arguments.
             primary_key_column: Name of column containing primary key.
             indexed_columns: Names of columns that should be indexed for faster
                 queries.
             port: Optionally, the port on which to connect to the database
@@ -424,33 +454,66 @@
         if "primary_key_column" in super_metadata:
             raise RuntimeError(
                 "super_metadata already contains key \"primary_key_column\".")
         super_metadata["primary_key_column"] = self._primary_key_column
         return super_metadata
 
     @staticmethod
-    def from_metadata(metadata: Dict[str, Any]) -> "MysqlKeyedTable":
+    def from_metadata(metadata: Dict[str, Any]) -> "PostgresqlKeyedTable":
         """See base class."""
-        return MysqlKeyedTable(**_format_metadata(metadata))
+        return PostgresqlKeyedTable(**_format_metadata(metadata))
 
     def extend(self, rows: Iterable[table.Row]):
         """See base class.
 
         All rows in rows must contain a primary key in the column named
         self.primary_key_column().
         """
         for row in rows:
             if (self._primary_key_column not in row
                 or row[self._primary_key_column] is None):
                 raise ValueError(
                     f"All rows in rows must contain a primary key in the "
                     f"column named {self._primary_key_column}.")
-        # Note that super().extend() creates the primary key column in the
-        # underlying table if it does not already exist.
-        super().extend(rows)
+
+        self._add_table_columns(rows)
+
+        # Extend the table using the `INSERT INTO... ON CONFLICT DO UPDATE SET`
+        # statement in order to avoid duplicate primary keys. This will have
+        # the same effect as `REPLACE INTO` in MySQL or SQLite, but requires
+        # including all columns in the `INSERT` statement, even if they are
+        # not being updated.
+        columns_in_rows = set()
+        for row in rows:
+            for col in row.keys():
+                columns_in_rows.add(col)
+        all_columns = list(set(self.columns).union(columns_in_rows))
+        with self._connection.cursor() as cursor:
+            for row in rows:
+                col_names_clause = ",".join(all_columns)
+                values_clause = ""
+                parameters = []
+                for col in all_columns:
+                    if col in row:
+                        values_clause += "%s,"
+                        parameters.append(row[col])
+                    else:
+                        values_clause += "DEFAULT,"
+                values_clause = values_clause[:-1]
+
+                set_clause = ",".join(f"{c}=EXCLUDED.{c}" for c in all_columns)
+
+                cursor.execute(
+                    f"INSERT INTO {self._table_name} "
+                    f"({col_names_clause}) "
+                    f"VALUES({values_clause}) "
+                    f"ON CONFLICT ({self._primary_key_column}) "
+                    f"DO UPDATE SET {set_clause}",
+                    parameters)
+        self._connection.commit()
 
     def primary_key_column(self) -> str:
         """See base class."""
         return self._primary_key_column
 
     def get(
         self,
@@ -460,41 +523,42 @@
         with self._connection.cursor() as cursor:
             try:
                 cursor.execute(
                     f"SELECT * FROM {self._table_name} "
                     f"WHERE {self._primary_key_column}=%s", (key,))
                 table_rows = cursor.fetchall()
                 self._connection.commit()
-            except pymysql.MySQLError as error:
+            except psycopg2.Error as error:
                 self._connection.rollback()
-                if (error.args[0] == pymysql.constants.ER.BAD_FIELD_ERROR
-                        and "Unknown column" in error.args[1]):
+                if error.pgcode == errorcodes.UNDEFINED_COLUMN:
                     table_rows = None
                 else:
                     raise error
         if not table_rows:
             return default
         if len(table_rows) > 1:
             raise RuntimeError("Found multiple rows having same primary key.")
         table_row = table_rows[0]
         if self._auto_ddl:
             table_row = _clean_row_dict(table_row)
+        table_row = _standardize_output(table_row)
         return table_row
 
     def __contains__(self, key: Any) -> bool:
         """See base class."""
         try:
             with self._connection.cursor() as cursor:
                 cursor.execute(
                     f"SELECT COUNT(*) AS c FROM {self._table_name} "
                     f"WHERE {self._primary_key_column}=%s", (key,))
                 c = cursor.fetchone()["c"]
             self._connection.commit()
             return c > 0
-        except pymysql.MySQLError as error:
+        except psycopg2.Error as error:
+            self._connection.rollback()
             with self._connection.cursor() as cursor:
                 cursor.execute(f"SELECT COUNT(*) AS c FROM {self._table_name}")
                 total_num_rows = cursor.fetchone()["c"]
             self._connection.commit()
             if total_num_rows == 0:
                 return False
             else:
@@ -525,26 +589,24 @@
                 cursor.execute(
                     f"DELETE FROM {self._table_name} "
                     f"WHERE {self._primary_key_column}=%s", (key,))
             col_names = [k for k, v in row.items() if v is not None]
             col_names_clause = ",".join(col_names)
             values_clause = ",".join(["%s" for _ in col_names])
             if skip_if_exists:
-                on_duplicate_key_clause = (
-                    "ON DUPLICATE KEY UPDATE "
-                    f"{self._primary_key_column}={self._primary_key_column}")
+                on_conflict_key_clause = "ON CONFLICT DO NOTHING"
             else:
-                on_duplicate_key_clause = ""
+                on_conflict_key_clause = ""
             cursor.execute(
                 (f"INSERT INTO {self._table_name} ({col_names_clause}) " +
-                f"VALUES({values_clause}) {on_duplicate_key_clause}"),
+                f"VALUES({values_clause}) {on_conflict_key_clause}"),
                 tuple(row[c] for c in col_names))
             if skip_if_exists:
-                cursor.execute("SELECT ROW_COUNT() AS rc")
-                return_value = cursor.fetchone()["rc"] > 0
+                rc = cursor.rowcount
+                return_value = rc is not None and rc > 0
             else:
                 return_value = True
         self._connection.commit()
         return return_value
 
     def update(self, key: Any, values: table.Row):
         """See base class.
@@ -568,23 +630,24 @@
         # (Note: We only insert or update values for columns that explicitly
         # exist in the table, as, by virtue of the preceding call to
         # self._add_table_columns(), all other values must be None in the values
         # argument and are already null in the table.)
         with self._connection.cursor() as cursor:
             cursor.execute(
                 f"INSERT INTO {self._table_name} ({self._primary_key_column}) "
-                f"VALUES(%s) ON DUPLICATE KEY UPDATE "
-                f"{self._primary_key_column}={self._primary_key_column}",
-                (key,))
+                f"VALUES(%s) ON CONFLICT DO NOTHING", (key,))
+            # We do not update a column that is null/None in the values
+            #   argument and all null/None in the table. Therefore we
+            #   use the raw columns (that contain _ALL_NULL_COLUMN_SUFFIX
+            #   suffixes) to determine which columns to update.
             existing_col_names = set()
-            cursor.execute(f"SELECT * FROM {self._table_name} LIMIT 1")
-            for row in cursor.fetchall():
-                for col_name in row.keys():
-                    if not self._auto_ddl or col_name != _PLACEHOLDER_COLUMN:
-                        existing_col_names.add(col_name)
+            cursor.execute(f"SELECT * FROM {self._table_name} LIMIT 0")
+            for col in cursor.description:
+                if not self._auto_ddl or col.name != _PLACEHOLDER_COLUMN:
+                    existing_col_names.add(col.name)
             update_col_names = [
                 k for k in values.keys() if k in existing_col_names]
             set_clause = ",".join([f"{c}=%s" for c in update_col_names])
             cursor.execute(
                 f"UPDATE {self._table_name} SET {set_clause} "
                 f"WHERE {self._primary_key_column}=%s",
                 tuple([values[c] for c in update_col_names] + [key]))
@@ -593,18 +656,17 @@
     def __delitem__(self, key: Any):
         """See base class."""
         with self._connection.cursor() as cursor:
             try:
                 cursor.execute(
                     f"DELETE FROM {self._table_name} "
                     f"WHERE {self._primary_key_column}=%s", (key,))
-            except pymysql.MySQLError as error:
+            except psycopg2.Error as error:
                 self._connection.rollback()
-                if (error.args[0] == pymysql.constants.ER.BAD_FIELD_ERROR
-                    and "Unknown column" in error.args[1]):
+                if error.pgcode == errorcodes.UNDEFINED_COLUMN:
                     pass
                 else:
                     raise error
         self._connection.commit()
 
     def increment(
         self,
@@ -613,36 +675,34 @@
         increment_by: int) -> Union[int, float]:
         """See base class."""
         # Ensure that key is not None.
         if key is None:
             raise ValueError("Primary key value cannot be None.")
         # Ensure that the column_name is not the primary key column.
         if column_name == self._primary_key_column:
-            raise ValueError(
-                "Cannot increment primary key column.")
+            raise ValueError("Cannot increment primary key column.")
         # Increment column.
         try:
             with self._connection.cursor() as cursor:
                 cursor.execute(
                     f"UPDATE {self._table_name} "
                     f"SET {column_name}={column_name}+%s "
                     f"WHERE {self._primary_key_column}=%s",
                     (increment_by, key))
                 cursor.execute(
                     f"SELECT {column_name} FROM {self._table_name} "
                     f"WHERE {self._primary_key_column}=%s", (key,))
                 value_updated = cursor.fetchone()
-        except pymysql.MySQLError as error:
+        except psycopg2.Error as error:
             self._connection.rollback()
-            if (error.args[0] == pymysql.constants.ER.BAD_FIELD_ERROR
-                and "Unknown column" in error.args[1]):
+            if (error.pgcode in (errorcodes.UNDEFINED_COLUMN,
+                                 errorcodes.UNDEFINED_FUNCTION)):
                 value_updated = None
             else:
                 raise error
         else:
             self._connection.commit()
 
         if value_updated is None:
-            raise ValueError(
-                f"Column {column_name} does not exist in table "
-                f"{self._table_name}.")
+            raise ValueError(f"Column {column_name} or key {key} does not"
+                             f"exist in table {self._table_name}.")
         return value_updated[column_name]
```

### Comparing `inductor-0.2.8/inductor/data/table/postgresql.py` & `inductor-0.2.9/inductor/data/table/sqlalchemy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,708 +1,853 @@
 # Copyright 2022 Inductor, Inc.
 
-"""Abstractions for PostgreSQL tables."""
+"""Abstractions for SQLAlchemy tables."""
 
+import abc
 import datetime
 import re
-import sys  # pylint: disable=unused-import
 from typing import Any, Dict, Iterable, Optional, Tuple, Union
 
-import psycopg2
-from psycopg2 import errorcodes
-from psycopg2 import extras
+from alembic import migration, operations
+import sqlalchemy
 
 from inductor.data.table import table
 
-# Name of empty placeholder column used to ensure that PostgreSQL tables never
+
+# Name of empty placeholder column used to ensure that SQLAlchemy tables never
 # contain no columns
 _PLACEHOLDER_COLUMN = "inductor_placeholder_column"
 
 # Suffix appended to names of columns that thus far contain only null values.
 _ALL_NULL_COLUMN_SUFFIX = "__allnull__"
 
 
-def _clean_row_dict(row_dict: table.Row) -> table.Row:
-    """Returns a copy of row_dict with modifications.
-
-    Args:
-        row: A raw row dictionary returned by a psycopg2.cursors.DictCursor.
-
-    Returns:
-        A new dictionary containing the same contents as row_dict, but with
-        the following modifications:
-            - The placeholder column, _PLACEHOLDER_COLUMN, is removed.
-            - Columns with names ending in _ALL_NULL_COLUMN_SUFFIX are renamed
-                to remove the suffix.
-    """
-    clean_row_dict = {}
-    for key in row_dict.keys():
-        if key != _PLACEHOLDER_COLUMN:
-            if key.endswith(_ALL_NULL_COLUMN_SUFFIX):
-                clean_row_dict[
-                    key[:-len(_ALL_NULL_COLUMN_SUFFIX)]] = row_dict[key]
-            else:
-                clean_row_dict[key] = row_dict[key]
-    return clean_row_dict
-
-
-def _standardize_output(value: Any) -> Any:
-    """Converts values from PostgreSQL to their original Python data types.
-
-    Converts memoryview objects to bytes objects.
-
-    Args:
-        value: The value to convert.
-
-    Returns:
-        The converted value.
-    """
-    if isinstance(value, memoryview):
-        return bytes(value)
-    elif isinstance(value, dict):
-        return {
-            k: _standardize_output(v)
-            for k, v in value.items()}
-    elif isinstance(value, set):
-        return set(
-            _standardize_output(item)
-            for item in value)
-    elif isinstance(value, list):
-        return [
-            _standardize_output(item)
-            for item in value]
-    else:
-        return value
-
-
-def _format_metadata(metadata: Dict[str, Any]) -> Dict[str, Any]:
-    """Formats metadata to have the right params for PostgresqlTable.
-
-    Args:
-        metadata: Metadata representing a PostgresqlTable.
-    """
-    table_metadata = metadata.copy()
-    if "postgresql_password" in table_metadata:
-        table_metadata["password"] = table_metadata["postgresql_password"]
-        del table_metadata["postgresql_password"]
-    return table_metadata
-
-
-class PostgresqlView(table.Table):
-    """A view of a PostgreSQL table."""
+class SqlAlchemyView(table.Table, abc.ABC):
+    """A view of a SQLAlchemy table."""
 
     def __init__(
         self,
-        parent: "PostgresqlTable",
-        query: table.SqlSelectQuery):
-        """Constructs a new PostgresqlView instance.
+        parent: "SqlAlchemyTable",
+        query: table.SqlSelectQuery,
+    ):
+        """Constructs a new SqlAlchemyView instance.
 
         Args:
-            parent: The underlying PostgresqlTable of which
-                this instance is a view.
+            parent: The underlying SqlAlchemyTable of which this instance
+                is a view.
             query: The query (over parent) defining this view.
         """
         self._parent = parent
         self._query = query
 
-    def _query_string(self) -> Tuple[str, Tuple[Any]]:
-        """Returns the SQL query string and values underlying this view."""
-        # pylint: disable-next=protected-access
-        return self._query.to_sql_query_string(self._parent._table_name)
+    @abc.abstractmethod
+    def to_metadata(self) -> Dict[str, Any]:
+        """See base class."""
+
+    @staticmethod
+    @abc.abstractmethod
+    def from_metadata(metadata: Dict[str, Any]) -> table.Table:
+        """See base class."""
+
+    def _query_string(self) -> Tuple[str, Dict[str, Any]]:
+        """Returns the SQL query string and values underlying this view.
+
+        SQLAlchemy requires that query values be contained in a dictionary,
+        with query placeholders consisting of keys of that dictionary preceded
+        by colons.  Therefore, this method replaces all instances of
+        self._query.placeholder in the query with such keys, and constructs
+        a corresponding dictionary of values.
+
+        Returns:
+            Internal query and values in a form that SQLAlchemy accepts for
+            query execution.
+        """
+        # Get query with placeholders
+        query_string, values_seq = self._query.to_sql_query_string(
+            self._parent._table_name)  # pylint: disable=protected-access
+        placeholder = self._query.placeholder
+        if not placeholder:
+            assert not values_seq
+            return (query_string, {})
+        assert len(values_seq) == query_string.count(placeholder)
+        # Reformat query for use with SQLAlchemy
+        formatted_query = ""
+        formatted_values = {}
+        split_query_string = query_string.split(placeholder)
+        assert len(split_query_string) == len(values_seq) + 1
+        colon_segments = query_string.split(":")[1:]
+        i = 0
+        for query_segment, value in zip(split_query_string[:-1], values_seq):
+            # Generate a unique key that is not already present in query_string
+            i += 1
+            key = f"interpval{i}"
+            while any(s.startswith(key) for s in colon_segments):
+                i += 1
+                key = f"interpval{i}"
+            # Update formatted_query and formatted_values
+            formatted_query += f"{query_segment}:{key}"
+            formatted_values[key] = value
+        formatted_query += split_query_string[-1]
+        return (formatted_query, formatted_values)
 
     def __iter__(self) -> Iterable[table.Row]:
         """See base class."""
         query_string, query_values = self._query_string()
         rows = []
-        try:
-            with self._parent._connection.cursor() as cursor:  # pylint: disable=protected-access
-                cursor.execute(query_string, query_values)
-                row_dict = cursor.fetchone()
-                while row_dict is not None:
-                    if self._parent._auto_ddl:  # pylint: disable=protected-access
-                        row_dict = _clean_row_dict(row_dict)
-                    row_dict = _standardize_output(row_dict)
+        with self._parent._engine.connect() as connection:  # pylint: disable=protected-access
+            try:
+                result = connection.execute(
+                    sqlalchemy.text(query_string),
+                    query_values,
+                )
+                for row in result:
+                    row_dict = row._asdict()  # pylint: disable=protected-access
+                    if self._parent._auto_ddl:
+                        row_dict = self._parent._clean_row_dict(row_dict)
                     rows.append(row_dict)
-                    row_dict = cursor.fetchone()
-            self._parent._connection.commit()  # pylint: disable=protected-access
-        except psycopg2.Error as error:
-            self._parent._connection.rollback()  # pylint: disable=protected-access
-            with self._parent._connection.cursor() as cursor:  # pylint: disable=protected-access
-                cursor.execute(
-                    f"SELECT COUNT(*) AS c FROM {self._parent._table_name}")  # pylint: disable=protected-access
-                total_num_rows = cursor.fetchone()["c"]
-            self._parent._connection.commit()  # pylint: disable=protected-access
-            if total_num_rows == 0:
-                rows = []
-            else:
-                raise error
+                connection.commit()
+            except sqlalchemy.exc.OperationalError as error:
+                connection.rollback()
+                if self._parent.columns:
+                    raise error
+                else:
+                    rows = []
         return rows.__iter__()
 
     def first_row(self) -> Optional[table.Row]:
         """See base class."""
         query_string, query_values = self._query_string()
-        try:
-            with self._parent._connection.cursor() as cursor:  # pylint: disable=protected-access
-                cursor.execute(
-                    f"SELECT * FROM ({query_string}) AS subquery LIMIT 1",
-                    query_values)
-                row_dict = cursor.fetchone()
-            self._parent._connection.commit()  # pylint: disable=protected-access
-        except psycopg2.Error as error:
-            self._parent._connection.rollback()  # pylint: disable=protected-access
-            with self._parent._connection.cursor() as cursor:  # pylint: disable=protected-access
-                cursor.execute(
-                    f"SELECT COUNT(*) AS c FROM {self._parent._table_name}")  # pylint: disable=protected-access
-                total_num_rows = cursor.fetchone()["c"]
-            self._parent._connection.commit()  # pylint: disable=protected-access
-            if total_num_rows == 0:
-                return None
-            raise error
-        if row_dict is not None:
-            if self._parent._auto_ddl:  # pylint: disable=protected-access
-                row_dict = _clean_row_dict(row_dict)
-            row_dict = _standardize_output(row_dict)
+        with self._parent._engine.connect() as connection:  # pylint: disable=protected-access
+            try:
+                result = connection.execute(
+                    sqlalchemy.text(
+                        f"SELECT * FROM ({query_string}) AS sq LIMIT 1"
+                    ),
+                    query_values,
+                )
+                row = result.first()
+                connection.commit()
+            except sqlalchemy.exc.OperationalError as error:
+                connection.rollback()
+                if self._parent.columns:
+                    raise error
+                row = None
+        if row is None:
+            return None
+        row_dict = row._asdict()  # pylint: disable=protected-access
+        if self._parent._auto_ddl:  # pylint: disable=protected-access
+            return self._parent._clean_row_dict(row_dict)  # pylint: disable=protected-access
         return row_dict
 
     @property
     def columns(self) -> Iterable[str]:
         """See base class."""
         row = self.first_row()
         return list(row.keys()) if row is not None else []
 
-    def to_metadata(self) -> Dict[str, Any]:
-        """See base class."""
-        return NotImplementedError()
-
-    @staticmethod
-    def from_metadata(metadata: Dict[str, Any]) -> table.Table:
-        return NotImplementedError()
-
 
-class PostgresqlTable(table.SqlQueryable, table.Appendable):
-    """A Table backed by a PostgreSQL table."""
+class SqlAlchemyTable(table.SqlQueryable, table.Appendable, abc.ABC):
+    """A Table utilizing SQLAlchemy."""
 
     def __init__(
         self,
-        host: str,
-        user: str,
-        password: str,
-        database: str,
         table_name: str,
+        sqlalchemy_url: str,
         indexed_columns: Iterable[str] = tuple(),
-        port: Optional[int] = None,
-        auto_ddl: bool = True):
-        """Constructs a new PostgresqlTable instance.
+        auto_ddl: bool = True,
+    ):
+        """Constructs a new SqlAlchemyTable instance.
 
         Args:
-            host: Name of database server host hosting the PostgreSQL database
-                containing this table.
-            user: PostgreSQL database server username.
-            password: Password for user.
-            database: Name of database containing table.
-            table_name: Name of table in database given by preceding arguments.
+            table_name: Name of table in database.
+            sqlalchemy_url: A SQLAlchemy-compatible database URL.
+                https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls
             indexed_columns: Names of columns that should be indexed for faster
                 queries.
-            port: Optionally, the port on which to connect to the database
-                server.
             auto_ddl: Boolean value indicating whether or not to automatically
                 execute DDL commands to create the table and add and modify
-                columns.  If False, then no processing of retrieved rows to
+                columns. If False, then no processing of retrieved rows to
                 account for prior automatic DDL is performed.
         """
-        self._connection_params = {
-            "host": host, "user": user,
-            "password": password, "database": database,
-            "cursor_factory": extras.RealDictCursor
-        }
-        if port is not None:
-            self._connection_params["port"] = port
         self._table_name = table_name
+        self._engine = sqlalchemy.create_engine(sqlalchemy_url)
         self._indexed_columns = list(indexed_columns)
         self._auto_ddl = auto_ddl
-        self._connection = psycopg2.connect(**self._connection_params)
-        if self._auto_ddl:
-            with self._connection.cursor() as cursor:
-                cursor.execute(
+        if auto_ddl:
+            with self._engine.connect() as connection:
+                connection.execute(sqlalchemy.text(
                     f"CREATE TABLE IF NOT EXISTS {self._table_name} "
-                    f"({_PLACEHOLDER_COLUMN} INTEGER)")
-            self._connection.commit()
+                    f"({_PLACEHOLDER_COLUMN} INTEGER)"
+                ))
+                connection.commit()
+
+    @abc.abstractmethod
+    def _is_undefined_column_error(
+        self, error: sqlalchemy.exc.DBAPIError
+    ) -> bool:
+        """Returns True if error is related to an undefined column.
+
+        Args:
+            error: The SQLAlchemy error.
+
+        Returns:
+            True if the error was caused by an undefined column, otherwise
+            False.
+        """
+
+    @abc.abstractmethod
+    def _gen_view(self, query: table.SqlSelectQuery) -> SqlAlchemyView:
+        """Creates a view over a provided query.
+
+        Args:
+            query: A SqlSelectQuery.
+
+        Returns:
+            An instance of a view class which extends SqlAlchemyView.
+        """
+
+    @abc.abstractmethod
+    def to_metadata(self) -> Dict[str, Any]:
+        """See base class."""
+
+    @staticmethod
+    @abc.abstractmethod
+    def from_metadata(metadata: Dict[str, Any]) -> table.Table:
+        """See base class."""
 
     def __del__(self):
-        """Closes self._connection as necessary on object destruction."""
-        if (not self._connection.closed and
-            # To ensure that the Python interpreter is not currently exiting
-            # (self._connection.close() here may raise an exception if called
-            # while interpreter is exiting).
-            "sys" in globals() and
-            hasattr("sys", "modules")):
-            self._connection.close()
+        """Disposes self._engine as necessary on object destruction."""
+        self._engine.dispose()
 
     def __iter__(self) -> Iterable[table.Row]:
         """See base class."""
-        return PostgresqlView(self, table.SqlSelectQuery("*")).__iter__()
+        return self._gen_view(table.SqlSelectQuery("*")).__iter__()
 
     def first_row(self) -> Optional[table.Row]:
         """See base class."""
-        return PostgresqlView(self, table.SqlSelectQuery("*")).first_row()
+        return self._gen_view(table.SqlSelectQuery("*")).first_row()
 
     @property
-    def columns(self) -> Iterable[str]:
-        """See base class."""
-        row = self.first_row()
-        return list(row.keys()) if row is not None else []
+    def _columns_with_nulls(self) -> Iterable[str]:
+        """Returns names of all columns except for placeholder column."""
+        metadata = sqlalchemy.MetaData()
+        metadata.reflect(
+            self._engine, only=[self._table_name], resolve_fks=False)
+        sqlalchemy_table = metadata.tables[self._table_name]
+        cols = sqlalchemy_table.columns
+        return [c.name for c in cols if c.name != _PLACEHOLDER_COLUMN]
 
-    def to_metadata(self) -> Dict[str, Any]:
-        """See base class."""
-        metadata = self._connection_params.copy()
-        del metadata["cursor_factory"]
-        del metadata["password"]
-        metadata["table_name"] = self._table_name
-        metadata["indexed_columns"] = self._indexed_columns
-        metadata["auto_ddl"] = self._auto_ddl
-        return metadata
-
-    @staticmethod
-    def from_metadata(metadata: Dict[str, Any]) -> "PostgresqlTable":
+    @property
+    def columns(self) -> Iterable[str]:
         """See base class."""
-        return PostgresqlTable(**_format_metadata(metadata))
+        cols = self._columns_with_nulls
+        return [c for c in cols if not c.endswith(_ALL_NULL_COLUMN_SUFFIX)]
 
     def indexed_columns(self) -> Iterable[str]:
         """See base class."""
         return self._indexed_columns.copy()
 
-    def select(self, expression: str, after_from: str = "") -> PostgresqlView:
+    def select(self, expression: str, after_from: str = "") -> SqlAlchemyView:
         """See base class."""
-        return PostgresqlView(
-            self,
+        # Generate placeholder that does not appear in expression,
+        # after_from, or self._table_name
+        i = 0
+        placeholder = f"[~placeholder{i}~]"
+        while (
+            placeholder in expression or
+            placeholder in after_from or
+            placeholder in self._table_name):
+            i += 1
+            placeholder = f"[~placeholder{i}~]"
+        # Return view
+        return self._gen_view(
             table.SqlSelectQuery(
-                expression=expression, after_from=after_from, placeholder="%s"))
+                expression=expression,
+                after_from=after_from,
+                placeholder=placeholder,
+            ),
+        )
+
+    def _consolidate_rows(self, rows: Iterable[table.Row]) -> Dict[str, Any]:
+        """Consolidates a collection of rows into a single row.
+
+        Given a collection of rows, this method returns a single row whose
+        columns are the union of all columns in the provided rows. If a
+        column exists in multiple rows, the value from the first non-None
+        value in the collection is used. A column that has both None and
+        non-None values will never be None in the returned row.
+
+        Args:
+            rows: The rows to consolidate.
+
+        Returns:
+            A dictionary containing the consolidated row.
+        """
+        return_dict = {}
+        for row in rows:
+            for col_name, value in row.items():
+                # Ensure every column is present
+                # If a value for a column is non-None, ensure
+                # it's present
+                if (col_name not in return_dict
+                    or return_dict[col_name] is None):
+                    return_dict[col_name] = value
+        return return_dict
+
+    def _validate_col_name(self, col_name: Optional[str]):
+        """Raises a ValueError if column name is invalid.
+
+        Args:
+            col_name: The column name to validate.
+
+        Raises:
+            ValueError if the provided column name is invalid.
+        """
+        if col_name == _PLACEHOLDER_COLUMN:
+            raise ValueError(
+                "Cannot add a column having name equal to "
+                f"placeholder column name ({_PLACEHOLDER_COLUMN})."
+            )
+        elif col_name.endswith(_ALL_NULL_COLUMN_SUFFIX):
+            raise ValueError(
+                "Column names cannot end with "
+                f"\"{_ALL_NULL_COLUMN_SUFFIX}\" "
+                f"(encountered column name {col_name})."
+            )
+        elif not re.match(r"\A[a-zA-Z0-9_]+\Z", col_name):
+            raise ValueError(
+                "Column names must match "
+                r"\A[a-zA-Z0-9_]+\Z "
+                f"(encountered column name {col_name})."
+            )
+
+    def _get_sqlalchemy_type(
+        self,
+        value: Any,
+        is_primary_key: bool,
+    ) -> Tuple[sqlalchemy.types.TypeEngine, Optional[str]]:
+        """Returns the SQLAlchemy type for a provided value.
+
+        Args:
+            value: A column value.
+            is_primary_key: True if this column is a primary key,
+                otherwise False.
+
+        Returns:
+            Tuple of (SQLAlchemy type, index postfix), where "index postfix"
+            refers to a string which some databases require to accompany a
+            type when that type is used to create an index.
+            If the index postfix is not required by a type, the return tuple
+            will be (SQLAlchemy type, None).
+        """
+        index_postfix = None
+        if isinstance(value, bool):
+            sqlalchemy_type = sqlalchemy.Boolean
+        elif isinstance(value, int):
+            sqlalchemy_type = sqlalchemy.Integer
+        elif isinstance(value, float):
+            sqlalchemy_type = sqlalchemy.Double
+        elif isinstance(value, str):
+            if is_primary_key:
+                sqlalchemy_type = sqlalchemy.String(255)
+                index_postfix = "(255)"
+            else:
+                sqlalchemy_type = sqlalchemy.Text
+                index_postfix = "(300)"
+        elif isinstance(value, bytes):
+            sqlalchemy_type = sqlalchemy.LargeBinary
+            index_postfix = "(600)"
+        elif isinstance(value, datetime.datetime):
+            sqlalchemy_type = sqlalchemy.DateTime
+        elif isinstance(value, datetime.date):
+            sqlalchemy_type = sqlalchemy.Date
+        else:
+            raise TypeError(f"Unsupported value type: {type(value)}")
+        return (sqlalchemy_type, index_postfix)
 
     def _add_table_columns(self, rows: Iterable[table.Row]):
-        """Adds columns to underlying table for any new columns in rows.
+        """Adds columns to the underlying table for any new columns in rows.
 
         Args:
-            rows: New rows based upon which to update table columns.
+            rows: Rows that may contain columns not present in the underlying
+                table.
         """
         if not self._auto_ddl:
             return
-        # Determine set of existing column names
-        existing_col_names = set()
-        with self._connection.cursor() as cursor:
-            cursor.execute(f"SELECT * FROM {self._table_name} LIMIT 0")
-            for col in cursor.description:
-                if col.name != _PLACEHOLDER_COLUMN:
-                    existing_col_names.add(col.name)
-        self._connection.commit()
-        # Add table columns as necessary
-        for row in rows:
-            for col_name in row.keys():
-                if (col_name not in existing_col_names
-                    or (row[col_name] is not None and
-                    col_name + _ALL_NULL_COLUMN_SUFFIX
-                    in existing_col_names)):
-                    if col_name == _PLACEHOLDER_COLUMN:
-                        raise ValueError(
-                            f"Cannot add a column having name equal to "
-                            f"placeholder column name ({_PLACEHOLDER_COLUMN}).")
-                    elif col_name.endswith(_ALL_NULL_COLUMN_SUFFIX):
-                        raise ValueError(
-                            f"Column names cannot end with "
-                            f"\"{_ALL_NULL_COLUMN_SUFFIX}\" "
-                            f"(encountered column name {col_name}).")
-                    elif not re.match(r"\A[a-zA-Z0-9_]+\Z", col_name):
-                        raise ValueError(
-                            "Column names must match "
-                            r"\A[a-zA-Z0-9_]+\Z "
-                            f"(encountered column name {col_name}).")
-                    value = row[col_name]
+        existing_col_names = set(self._columns_with_nulls)
+        consolidated_rows = self._consolidate_rows(rows)
+        with self._engine.connect() as connection:
+            ctx = migration.MigrationContext.configure(connection)
+            op = operations.Operations(ctx)
+            for col_name, value in consolidated_rows.items():
+                self._validate_col_name(col_name)
+                null_col_name = col_name + _ALL_NULL_COLUMN_SUFFIX
+                is_null_present = null_col_name in existing_col_names
+                should_add_col = col_name not in existing_col_names
+                should_alter_col = value is not None and is_null_present
+                if should_add_col or should_alter_col:
                     if value is None:
-                        # Create two columns: col_name and col_name_all_null
-                        col_name_all_null = col_name + _ALL_NULL_COLUMN_SUFFIX
-                        with self._connection.cursor() as cursor:
-                            cursor.execute(
-                                f"ALTER TABLE {self._table_name} ADD COLUMN "
-                                f"{col_name} TEXT DEFAULT NULL")
-                            cursor.execute(
-                                f"ALTER TABLE {self._table_name} ADD COLUMN "
-                                f"{col_name_all_null} TEXT DEFAULT NULL")
-                        existing_col_names.add(col_name)
-                        existing_col_names.add(col_name_all_null)
+                        # Create column and null column
+                        for col_to_add in [col_name, null_col_name]:
+                            op.add_column(  # pylint: disable=no-member
+                                self._table_name,
+                                sqlalchemy.Column(col_to_add, sqlalchemy.Text),
+                            )
+                            existing_col_names.add(col_to_add)
                     else:
-                        if isinstance(value, bool):
-                            postgresql_type = "BOOLEAN"
-                        elif isinstance(value, int):
-                            postgresql_type = "INTEGER"
-                        elif isinstance(value, float):
-                            postgresql_type = "DOUBLE PRECISION"
-                        elif isinstance(value, str):
-                            postgresql_type = "TEXT"
-                        elif isinstance(value, bytes):
-                            postgresql_type = "BYTEA"
-                        elif isinstance(value, datetime.datetime):
-                            postgresql_type = "TIMESTAMP"
-                        elif isinstance(value, datetime.date):
-                            postgresql_type = "DATE"
+                        is_keyed_table = isinstance(self, SqlAlchemyKeyedTable)
+                        primary_key_column = (self.primary_key_column()
+                            if is_keyed_table
+                            else None)
+                        assert col_name is not None
+                        is_primary_key = col_name == primary_key_column
+                        (sqlalchemy_type, index_postfix) = (
+                            self._get_sqlalchemy_type(value, is_primary_key))
+                        # Null-placeholder columns should be dropped
+                        if is_null_present:
+                            op.drop_column(  # pylint: disable=no-member
+                                self._table_name, null_col_name)
+                            existing_col_names.remove(null_col_name)
+                        # If column exists, alter existing column
+                        if col_name in existing_col_names:
+                            op.alter_column(  # pylint: disable=no-member
+                                self._table_name,
+                                col_name,
+                                type_=sqlalchemy_type,
+                                nullable=not is_primary_key,
+                            )
+                        # Otherwise, add new column
                         else:
-                            raise TypeError(
-                                f"Unsupported value type: {type(value)}")
-                        with self._connection.cursor() as cursor:
-                            if col_name in existing_col_names:
-                                cursor.execute(
-                                    f"ALTER TABLE {self._table_name} "
-                                    f"DROP COLUMN "
-                                    f"{col_name + _ALL_NULL_COLUMN_SUFFIX}")
-                                existing_col_names.remove(
-                                    col_name + _ALL_NULL_COLUMN_SUFFIX)
-                                cursor.execute(
-                                    f"ALTER TABLE {self._table_name} "
-                                    f"ALTER COLUMN {col_name} "
-                                    f"TYPE {postgresql_type} "
-                                    f"USING {col_name}::{postgresql_type}")
-                            else:
-                                cursor.execute(
-                                    f"ALTER TABLE {self._table_name} "
-                                    f"ADD COLUMN {col_name} {postgresql_type} "
-                                    "DEFAULT NULL")
-                                existing_col_names.add(col_name)
-                                if (col_name + _ALL_NULL_COLUMN_SUFFIX in
-                                    existing_col_names):
-                                    cursor.execute(
-                                        f"ALTER TABLE {self._table_name} "
-                                        "DROP COLUMN "
-                                        f"{col_name + _ALL_NULL_COLUMN_SUFFIX}")
-                                    existing_col_names.remove(
-                                        col_name + _ALL_NULL_COLUMN_SUFFIX)
-                            if col_name in self._indexed_columns:
-                                cursor.execute(
-                                    "CREATE INDEX "
-                                    f"{self._table_name}__{col_name}_index "
-                                    f"ON {self._table_name} "
-                                    f"({col_name})")
-                            if (isinstance(self, PostgresqlKeyedTable) and
-                                # pylint: disable=no-member
-                                col_name == self.primary_key_column()):
-                                # pylint: enable=no-member
-                                cursor.execute(
-                                    f"ALTER TABLE {self._table_name} "
-                                    f"ADD PRIMARY KEY ({col_name})")
-                        self._connection.commit()
+                            op.add_column(  # pylint: disable=no-member
+                                self._table_name,
+                                sqlalchemy.Column(
+                                    col_name,
+                                    sqlalchemy_type,
+                                    nullable=not is_primary_key,
+                                ),
+                            )
+                            existing_col_names.add(col_name)
+                        # Create index if required.
+                        if col_name in self._indexed_columns:
+                            index_col_name = (
+                                f"{col_name}{index_postfix}"
+                                if index_postfix
+                                else col_name)
+                            op.create_index(  # pylint: disable=no-member
+                                f"{self._table_name}__{col_name}_index",
+                                self._table_name,
+                                [sqlalchemy.text(index_col_name)],
+                            )
+                        # Add primary key if required.
+                        if is_primary_key:
+                            connection.execute(sqlalchemy.text(
+                                f"ALTER TABLE {self._table_name} "
+                                f"ADD PRIMARY KEY ({col_name})"
+                            ))
+            connection.commit()
+
+    def _get_clauses_from_row(
+        self,
+        row: table.Row,
+        omit_none_values: bool = False,
+    ) -> Tuple[str, str, Dict[str, Any]]:
+        """Returns columns and values clause and values dict from row.
+
+        Args:
+            row: A table row.
+            omit_none_values: Boolean flag indicating whether or not columns
+                and values should be added to their respective clauses if the
+                value is None.
+
+        Returns:
+            Tuple of (column clause, values clause, dictionary of values).
+        """
+        col_names = []
+        values = []
+        values_dict = {}
+        for i, (col, value) in enumerate(row.items()):
+            if value is not None or not omit_none_values:
+                key = f"val{i}"
+                col_names.append(col)
+                values.append(f":{key}")
+                values_dict[key] = value
+        col_names_clause = ",".join(col_names)
+        values_clause = ",".join(values)
+        return (col_names_clause, values_clause, values_dict)
 
     def extend(self, rows: Iterable[table.Row]):
         """See base class."""
         self._add_table_columns(rows)
-        with self._connection.cursor() as cursor:
+        with self._engine.connect() as connection:
+            columns = None
             for row in rows:
                 all_values_none = all(value is None for value in row.values())
                 if all_values_none:
-                    cursor.execute(
+                    if columns is None:
+                        columns = self.columns
+                    col_names_clause = ",".join(columns)
+                    default_values = ",".join(["DEFAULT" for _ in columns])
+                    connection.execute(sqlalchemy.text(
                         f"INSERT INTO {self._table_name} "
-                        f"DEFAULT VALUES")
+                        f"({col_names_clause}) "
+                        f"VALUES({default_values})"
+                    ))
                 else:
-                    col_names = [k for k, v in row.items() if v is not None]
-                    col_names_clause = ",".join(col_names)
-                    values_clause = ",".join(["%s" for _ in col_names])
-                    cursor.execute(
+                    (col_names_clause, values_clause, values) = (
+                        self._get_clauses_from_row(row, omit_none_values=True))
+                    query = sqlalchemy.text(
                         f"INSERT INTO {self._table_name} "
                         f"({col_names_clause}) "
-                        f"VALUES({values_clause})",
-                        tuple(row[c] for c in col_names))
-        self._connection.commit()
+                        f"VALUES({values_clause})"
+                    )
+                    connection.execute(query, values)
+            connection.commit()
+
+    def _clean_row_dict(self, row_dict: table.Row) -> table.Row:
+        """Cleans a raw row dictionary returned by sqlalchemy.cursors._asdict().
+
+        By default, only _PLACEHOLDER_COLUMN and any columns ending with the
+        _ALL_NULL_COLUMN_SUFFIX are removed from the return dictionary.
+        Implementations which require additional cleaning should override this
+        method.
 
+        Args:
+            row: A raw row dictionary returned by sqlalchemy.cursors._asdict().
+
+        Returns:
+            A new dictionary containing the cleaned contents of row_dict.
+        """
+        clean_row_dict = {}
+        for key, value in row_dict.items():
+            if key != _PLACEHOLDER_COLUMN:
+                if key.endswith(_ALL_NULL_COLUMN_SUFFIX):
+                    clean_row_dict[
+                        key[:-len(_ALL_NULL_COLUMN_SUFFIX)]] = value
+                else:
+                    clean_row_dict[key] = value
+        return clean_row_dict
 
-class PostgresqlKeyedTable(PostgresqlTable, table.WithPrimaryKey):
-    """A PostgresqlTable having a primary key."""
+
+class SqlAlchemyKeyedTable(SqlAlchemyTable, table.WithPrimaryKey, abc.ABC):
+    """A SqlAlchemyTable having a primary key."""
 
     def __init__(
         self,
-        host: str,
-        user: str,
-        password: str,
-        database: str,
         table_name: str,
+        sqlalchemy_url: str,
         primary_key_column: str,
         indexed_columns: Iterable[str] = tuple(),
-        port: Optional[int] = None,
-        auto_ddl: bool = True):
-        """Constructs a new PostgresqlKeyedTable instance.
+        auto_ddl: bool = True,
+    ):
+        """Constructs a new SqlAlchemyKeyedTable instance.
 
         Args:
-            host: Name of database server host hosting the PostgreSQL database
-                containing this table.
-            user: PostgreSQL database server username.
-            password: Password for user.
-            database: Name of database containing table.
-            table_name: Name of table in database given by preceding arguments.
+            table_name: Name of table in database.
+            sqlalchemy_url: A SQLAlchemy-compatible database URL.
+                https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls
             primary_key_column: Name of column containing primary key.
             indexed_columns: Names of columns that should be indexed for faster
                 queries.
-            port: Optionally, the port on which to connect to the database
-                server.
             auto_ddl: Boolean value indicating whether or not to automatically
                 execute DDL commands to create the table and add and modify
-                columns.  If False, then no processing of retrieved rows to
+                columns. If False, then no processing of retrieved rows to
                 account for prior automatic DDL is performed.
         """
         super().__init__(
-            host=host, user=user, password=password, database=database,
-            table_name=table_name, indexed_columns=indexed_columns, port=port,
-            auto_ddl=auto_ddl)
+            table_name=table_name,
+            sqlalchemy_url=sqlalchemy_url,
+            indexed_columns=indexed_columns,
+            auto_ddl=auto_ddl,
+        )
         self._primary_key_column = primary_key_column
 
+    @property
+    @abc.abstractmethod
+    def _insert_skip_if_exists_suffix(self) -> str:
+        """Returns INSERT statement suffix that yields skip-if-exists behavior.
+
+        In particular, appending the returned string to an INSERT statement
+        should cause the statement to skip the insert if a row already exists
+        having the same primary key.
+        """
+
+    @abc.abstractmethod
     def to_metadata(self) -> Dict[str, Any]:
         """See base class."""
-        super_metadata = super().to_metadata()
-        if "primary_key_column" in super_metadata:
-            raise RuntimeError(
-                "super_metadata already contains key \"primary_key_column\".")
-        super_metadata["primary_key_column"] = self._primary_key_column
-        return super_metadata
 
     @staticmethod
-    def from_metadata(metadata: Dict[str, Any]) -> "PostgresqlKeyedTable":
+    @abc.abstractmethod
+    def from_metadata(metadata: Dict[str, Any]) -> table.Table:
         """See base class."""
-        return PostgresqlKeyedTable(**_format_metadata(metadata))
 
     def extend(self, rows: Iterable[table.Row]):
         """See base class.
 
         All rows in rows must contain a primary key in the column named
-        self.primary_key_column().
+        self.primary_key_column(). If a row in rows contains a primary key
+        that already exists in the table, then the existing row in the table
+        will be replaced.
         """
         for row in rows:
             if (self._primary_key_column not in row
                 or row[self._primary_key_column] is None):
                 raise ValueError(
                     f"All rows in rows must contain a primary key in the "
-                    f"column named {self._primary_key_column}.")
-
+                    f"column named {self._primary_key_column}."
+                )
         self._add_table_columns(rows)
-
-        # Extend the table using the `INSERT INTO... ON CONFLICT DO UPDATE SET`
-        # statement in order to avoid duplicate primary keys. This will have
-        # the same effect as `REPLACE INTO` in MySQL or SQLite, but requires
-        # including all columns in the `INSERT` statement, even if they are
-        # not being updated.
-        columns_in_rows = set()
-        for row in rows:
-            for col in row.keys():
-                columns_in_rows.add(col)
-        all_columns = list(set(self.columns).union(columns_in_rows))
-        with self._connection.cursor() as cursor:
+        with self._engine.connect() as connection:
             for row in rows:
-                col_names_clause = ",".join(all_columns)
-                values_clause = ""
-                parameters = []
-                for col in all_columns:
-                    if col in row:
-                        values_clause += "%s,"
-                        parameters.append(row[col])
-                    else:
-                        values_clause += "DEFAULT,"
-                values_clause = values_clause[:-1]
-
-                set_clause = ",".join(f"{c}=EXCLUDED.{c}" for c in all_columns)
-
-                cursor.execute(
+                delete_query = sqlalchemy.text(
+                    f"DELETE FROM {self._table_name} "
+                    f"WHERE {self._primary_key_column}=:key"
+                )
+                delete_values = {"key": row[self._primary_key_column]}
+                connection.execute(delete_query, delete_values)
+                (col_names_clause, values_clause, insert_values) = (
+                    self._get_clauses_from_row(row, omit_none_values=True))
+                insert_query = sqlalchemy.text(
                     f"INSERT INTO {self._table_name} "
                     f"({col_names_clause}) "
-                    f"VALUES({values_clause}) "
-                    f"ON CONFLICT ({self._primary_key_column}) "
-                    f"DO UPDATE SET {set_clause}",
-                    parameters)
-        self._connection.commit()
+                    f"VALUES({values_clause})"
+                )
+                connection.execute(insert_query, insert_values)
+            connection.commit()
 
     def primary_key_column(self) -> str:
         """See base class."""
         return self._primary_key_column
 
     def get(
         self,
         key: Any,
-        default: Optional[table.Row] = None) -> Optional[table.Row]:
+        default: Optional[table.Row] = None,
+    ) -> Optional[table.Row]:
         """See base class."""
-        with self._connection.cursor() as cursor:
+        with self._engine.connect() as connection:
             try:
-                cursor.execute(
+                query = sqlalchemy.text(
                     f"SELECT * FROM {self._table_name} "
-                    f"WHERE {self._primary_key_column}=%s", (key,))
-                table_rows = cursor.fetchall()
-                self._connection.commit()
-            except psycopg2.Error as error:
-                self._connection.rollback()
-                if error.pgcode == errorcodes.UNDEFINED_COLUMN:
-                    table_rows = None
+                    f"WHERE {self._primary_key_column}=:key"
+                )
+                values = {"key": key}
+                result = connection.execute(query, values)
+                table_rows = result.fetchall()
+                connection.commit()
+            except sqlalchemy.exc.DBAPIError as error:
+                connection.rollback()
+                if self._is_undefined_column_error(error):
+                    columns = self.columns
+                    if columns or columns is None:
+                        raise error
+                    table_rows = []
                 else:
                     raise error
         if not table_rows:
             return default
         if len(table_rows) > 1:
             raise RuntimeError("Found multiple rows having same primary key.")
         table_row = table_rows[0]
+        row_dict = table_row._asdict()
         if self._auto_ddl:
-            table_row = _clean_row_dict(table_row)
-        table_row = _standardize_output(table_row)
-        return table_row
+            row_dict = self._clean_row_dict(row_dict)
+        return row_dict
 
     def __contains__(self, key: Any) -> bool:
         """See base class."""
-        try:
-            with self._connection.cursor() as cursor:
-                cursor.execute(
-                    f"SELECT COUNT(*) AS c FROM {self._table_name} "
-                    f"WHERE {self._primary_key_column}=%s", (key,))
-                c = cursor.fetchone()["c"]
-            self._connection.commit()
-            return c > 0
-        except psycopg2.Error as error:
-            self._connection.rollback()
-            with self._connection.cursor() as cursor:
-                cursor.execute(f"SELECT COUNT(*) AS c FROM {self._table_name}")
-                total_num_rows = cursor.fetchone()["c"]
-            self._connection.commit()
-            if total_num_rows == 0:
-                return False
-            else:
-                raise error
+        with self._engine.connect() as connection:
+            try:
+                query = sqlalchemy.text(
+                    f"SELECT COUNT(*) FROM {self._table_name} "
+                    f"WHERE {self._primary_key_column}=:key"
+                )
+                values = {"key": key}
+                result = connection.execute(query, values)
+                return_value = result.scalar_one() > 0
+                connection.commit()
+                return return_value
+            except sqlalchemy.exc.DBAPIError as error:
+                connection.rollback()
+                if self._is_undefined_column_error(error):
+                    columns = self.columns
+                    if columns or columns is None:
+                        raise error
+                    return False
+                else:
+                    raise error
 
     def set(
-        self, key: Any, row: table.Row, skip_if_exists: bool = False) -> bool:
+        self,
+        key: Any,
+        row: table.Row,
+        skip_if_exists: bool = False,
+    ) -> bool:
         """See base class.
 
         Primary key value cannot be None.
         """
         # Ensure that key is not None
         if key is None:
             raise ValueError("Primary key value cannot be None.")
         # Ensure that row contains primary key value
         if self._primary_key_column in row:
             if key != row[self._primary_key_column]:
                 raise ValueError(
-                    "Primary key value in row does not match key argument.")
+                    "Primary key value in row does not match key argument."
+                )
         else:
             row = row.copy()
             row[self._primary_key_column] = key
         # Add any new table columns
         self._add_table_columns([row])
         # Insert or replace row
-        with self._connection.cursor() as cursor:
-            if not skip_if_exists:
-                cursor.execute(
-                    f"DELETE FROM {self._table_name} "
-                    f"WHERE {self._primary_key_column}=%s", (key,))
-            col_names = [k for k, v in row.items() if v is not None]
-            col_names_clause = ",".join(col_names)
-            values_clause = ",".join(["%s" for _ in col_names])
-            if skip_if_exists:
-                on_conflict_key_clause = "ON CONFLICT DO NOTHING"
-            else:
-                on_conflict_key_clause = ""
-            cursor.execute(
-                (f"INSERT INTO {self._table_name} ({col_names_clause}) " +
-                f"VALUES({values_clause}) {on_conflict_key_clause}"),
-                tuple(row[c] for c in col_names))
+        with self._engine.connect() as connection:
             if skip_if_exists:
-                rc = cursor.rowcount
-                return_value = rc is not None and rc > 0
+                # Check if the key exists if skip_if_exists is True
+                query = sqlalchemy.text(
+                    f"SELECT COUNT(*) FROM {self._table_name} "
+                    f"WHERE {self._primary_key_column}=:key"
+                )
+                values = {"key": key}
+                result = connection.execute(query, values)
+                if result.scalar_one() > 0:
+                    return False
             else:
-                return_value = True
-        self._connection.commit()
-        return return_value
+                # Delete any existing row having given key if skip_if_exists
+                # is False
+                query = sqlalchemy.text(
+                    f"DELETE FROM {self._table_name} "
+                    f"WHERE {self._primary_key_column}=:key"
+                )
+                values = {"key": key}
+                connection.execute(query, values)
+            # Insert row
+            (col_names_clause, values_clause, values) = (
+                self._get_clauses_from_row(row, omit_none_values=True))
+            query = sqlalchemy.text(
+                f"INSERT INTO {self._table_name} ({col_names_clause}) "
+                f"VALUES({values_clause})"
+            )
+            connection.execute(query, values)
+            connection.commit()
+        return True
 
     def update(self, key: Any, values: table.Row):
         """See base class.
 
         Primary key value cannot be None.
         """
         # Ensure that key is not None
         if key is None:
             raise ValueError("Primary key value cannot be None.")
         # Ensure that values contains a primary key value
         if self._primary_key_column in values:
             if key != values[self._primary_key_column]:
                 raise ValueError(
-                    "Primary key value in values does not match key argument.")
+                    "Primary key value in values does not match key argument."
+                )
         else:
             values = values.copy()
             values[self._primary_key_column] = key
         # Add any new table columns
         self._add_table_columns([values])
         # Insert or update values
-        # (Note: We only insert or update values for columns that explicitly
-        # exist in the table, as, by virtue of the preceding call to
-        # self._add_table_columns(), all other values must be None in the values
-        # argument and are already null in the table.)
-        with self._connection.cursor() as cursor:
-            cursor.execute(
+        with self._engine.connect() as connection:
+            query = sqlalchemy.text(
                 f"INSERT INTO {self._table_name} ({self._primary_key_column}) "
-                f"VALUES(%s) ON CONFLICT DO NOTHING", (key,))
-            # We do not update a column that is null/None in the values
-            #   argument and all null/None in the table. Therefore we
-            #   use the raw columns (that contain _ALL_NULL_COLUMN_SUFFIX
-            #   suffixes) to determine which columns to update.
-            existing_col_names = set()
-            cursor.execute(f"SELECT * FROM {self._table_name} LIMIT 0")
-            for col in cursor.description:
-                if not self._auto_ddl or col.name != _PLACEHOLDER_COLUMN:
-                    existing_col_names.add(col.name)
-            update_col_names = [
-                k for k in values.keys() if k in existing_col_names]
-            set_clause = ",".join([f"{c}=%s" for c in update_col_names])
-            cursor.execute(
-                f"UPDATE {self._table_name} SET {set_clause} "
-                f"WHERE {self._primary_key_column}=%s",
-                tuple([values[c] for c in update_col_names] + [key]))
-        self._connection.commit()
+                f"VALUES(:key) {self._insert_skip_if_exists_suffix}"
+            )
+            query_values = {"key": key}
+            connection.execute(query, query_values)
+            if len(values) > 1:  # if values does not contain only primary key
+                set_clauses = []
+                query_values = {}
+                for i, (col_name, col_value) in enumerate(values.items()):
+                    if col_name != self._primary_key_column:
+                        query_key = f"val{i}"
+                        set_clauses.append(f"{col_name}=:{query_key}")
+                        query_values[query_key] = col_value
+                query_values["key"] = values[self._primary_key_column]
+                query = sqlalchemy.text(
+                    f"UPDATE {self._table_name} SET " +
+                    ",".join(set_clauses) +
+                    f" WHERE {self._primary_key_column}=:key")
+                connection.execute(query, query_values)
+            connection.commit()
 
     def __delitem__(self, key: Any):
         """See base class."""
-        with self._connection.cursor() as cursor:
+        # Ensure that key is not None.
+        if key is None:
+            raise ValueError("Primary key value cannot be None.")
+        with self._engine.connect() as connection:
+            query = sqlalchemy.text(
+                f"DELETE FROM {self._table_name} "
+                f"WHERE {self._primary_key_column}=:key"
+            )
+            query_values = {"key": key}
             try:
-                cursor.execute(
-                    f"DELETE FROM {self._table_name} "
-                    f"WHERE {self._primary_key_column}=%s", (key,))
-            except psycopg2.Error as error:
-                self._connection.rollback()
-                if error.pgcode == errorcodes.UNDEFINED_COLUMN:
-                    pass
+                connection.execute(query, query_values)
+                connection.commit()
+            except sqlalchemy.exc.DBAPIError as error:
+                connection.rollback()
+                if self._is_undefined_column_error(error):
+                    columns = self.columns
+                    if columns or columns is None:
+                        raise error
                 else:
                     raise error
-        self._connection.commit()
 
     def increment(
         self,
         key: Any,
         column_name: str,
-        increment_by: int) -> Union[int, float]:
+        increment_by: int
+    ) -> Union[int, float]:
         """See base class."""
         # Ensure that key is not None.
         if key is None:
             raise ValueError("Primary key value cannot be None.")
-        # Ensure that the column_name is not the primary key column.
+        # Ensure that column_name is not the primary key column.
         if column_name == self._primary_key_column:
-            raise ValueError("Cannot increment primary key column.")
+            raise ValueError(
+                "Cannot increment primary key column."
+            )
         # Increment column.
-        try:
-            with self._connection.cursor() as cursor:
-                cursor.execute(
+        with self._engine.connect() as connection:
+            try:
+                update_query = sqlalchemy.text(
                     f"UPDATE {self._table_name} "
-                    f"SET {column_name}={column_name}+%s "
-                    f"WHERE {self._primary_key_column}=%s",
-                    (increment_by, key))
-                cursor.execute(
+                    f"SET {column_name}={column_name}+:increment "
+                    f"WHERE {self._primary_key_column}=:key"
+                )
+                update_values = {
+                    "increment": increment_by,
+                    "key": key,
+                }
+                connection.execute(update_query, update_values)
+                select_query = sqlalchemy.text(
                     f"SELECT {column_name} FROM {self._table_name} "
-                    f"WHERE {self._primary_key_column}=%s", (key,))
-                value_updated = cursor.fetchone()
-        except psycopg2.Error as error:
-            self._connection.rollback()
-            if (error.pgcode in (errorcodes.UNDEFINED_COLUMN,
-                                 errorcodes.UNDEFINED_FUNCTION)):
-                value_updated = None
-            else:
-                raise error
-        else:
-            self._connection.commit()
-
-        if value_updated is None:
-            raise ValueError(f"Column {column_name} or key {key} does not"
-                             f"exist in table {self._table_name}.")
-        return value_updated[column_name]
+                    f"WHERE {self._primary_key_column}=:key"
+                )
+                select_values = {"key": key}
+                result = connection.execute(
+                    select_query, select_values
+                ).fetchone()
+                if result is not None:
+                    result = result._asdict()
+                connection.commit()
+            except sqlalchemy.exc.DBAPIError as error:
+                connection.rollback()
+                if self._is_undefined_column_error(error):
+                    columns = self.columns
+                    if columns or columns is None:
+                        raise error
+                    result = None
+                else:
+                    raise error
+        if result is None or column_name not in result:
+            raise ValueError(
+                f"Column name {column_name} does not exist in table "
+                f"{self._table_name}."
+            )
+        return result[column_name]
```

### Comparing `inductor-0.2.8/inductor/data/table/snowflake.py` & `inductor-0.2.9/inductor/data/table/snowflake.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/data/table/sqlite.py` & `inductor-0.2.9/inductor/data/table/sqlite.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/data/table/table.py` & `inductor-0.2.9/inductor/data/table/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,40 +72,54 @@
     def __init__(
         self,
         expression: str,
         after_from: str = "",
         placeholder: str = ""):
         """Initializes a SqlSelectQuery instance.
 
-        Interpolates expression or after_from if either contains segments
-        enclosed in curly braces; the interpolation is done using the values of
-        the variables in the stack frame two frames above. The semantics of the
-        interpolation are those of Python's built-in `str.format()`.
+        If placeholder is not the empty string, then interpolates expression or
+        after_from if either contains segments enclosed in curly braces; the
+        interpolation is done using the values of the variables in the stack
+        frame two frames above. The semantics of the interpolation are those of
+        Python's built-in `str.format()`.
 
         Args:
             expression: SQL clause that will appear between SELECT and FROM.
             after_from: SQL clause that will appear after FROM clause.
             placeholder: Placeholder that will replace curly-braced segments in
                 `expression` and `after_from` (generally should be placeholder
-                required by the data system's Python connector library).
+                required by the data system's Python connector library).  No
+                interpolation is performed if placeholder is the empty string.
         """
-        self.expression, self.expression_values = _interpolate_sql(
-            expression, placeholder)
-        self.after_from, self.after_from_values = _interpolate_sql(
-            after_from, placeholder)
+        if placeholder:
+            self._expression, self._expression_values = _interpolate_sql(
+                expression, placeholder)
+            self._after_from, self._after_from_values = _interpolate_sql(
+                after_from, placeholder)
+        else:
+            self._expression = expression
+            self._expression_values = tuple()
+            self._after_from = after_from
+            self._after_from_values = tuple()
+        self._placeholder = placeholder
+
+    @property
+    def placeholder(self) -> str:
+        """Placeholder used for interpolation."""
+        return self._placeholder
 
     def to_sql_query_string(self, from_string: str) -> Tuple[str, Tuple[Any]]:
         """Returns SQL SELECT query string and values implied by this instance.
 
         Args:
             from_string: String to be used in the query's FROM clause.
         """
-        return (f"SELECT {self.expression} FROM {from_string} "
-                f"{self.after_from}",
-                self.expression_values + self.after_from_values)
+        return (f"SELECT {self._expression} FROM {from_string} "
+                f"{self._after_from}",
+                self._expression_values + self._after_from_values)
 
 
 class Table(abc.ABC):
     """A set of Rows, backed by structured storage.
 
     All tables must allow scans.  Subclasses may provide additional modes of
     access (e.g., fast range queries, general SQL SELECT queries) and/or the
```

### Comparing `inductor-0.2.8/inductor/data/table/table_catalog.py` & `inductor-0.2.9/inductor/data/table/table_catalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -436,15 +436,15 @@
             mysql_database: Name of MySQL database containing existing table.
             mysql_table_name: Name of existing table in database given by
                 preceding arguments. If not provided, the value of the name
                 argument is used.
             primary_key_column: If non-None, then the table will be treated as
                 being keyed by the column having name given by this parameter.
                 If None, then
-                
+
                 - If the existing table has exactly one primary key column, then
                   the table will be treated as being keyed on that column.
                 - Otherwise, if the existing table has no primary key column
                   and exactly one unique index column, then the table will be
                   treated as being keyed on that column.
                 - Otherwise, the table will not be treated as being keyed.
             mysql_port: Optionally, the port on which to connect to the database
@@ -628,15 +628,15 @@
                 existing table.
             postgresql_table_name: Name of existing table in database given by
                 preceding arguments. If not provided, the value of the name
                 argument is used.
             primary_key_column: If non-None, then the table will be treated as
                 being keyed by the column having name given by this parameter.
                 If None, then
-                
+
                 - If the existing table has exactly one primary key column,
                   then the table will be treated as being keyed on that column.
                 - Otherwise, if the existing table has no primary key column
                   and exactly one unique index column, then the table will be
                   treated as being keyed on that column.
                 - Otherwise, the table will not be treated as being keyed.
             postgresql_port: Optionally, the port on which to connect to the
@@ -776,14 +776,15 @@
         from inductor.data.table import snowflake  # pylint: disable=import-outside-toplevel
 
         if snowflake_table_name is None:
             snowflake_table_name = name
 
         table_spec = locals().copy()
         del table_spec["self"]
+        del table_spec["snowflake"]
 
         if not self._run_time:
             self._table_creation_instructions.append(
                 (self.add_existing_snowflake_table.__name__, table_spec))
             return
 
         del table_spec["snowflake_password"]
@@ -817,7 +818,73 @@
                 name, t, table_spec, table_secrets=secrets, skip_if_exists=True,
                 existing_table=True)
             if (already_exists and
                 self.table_spec(name) != table_spec):
                 raise RuntimeError(
                     f"Table {name} already exists but has different "
                     "table_spec.")
+
+    def add_existing_bigquery_table(
+        self,
+        name: str,
+        bigquery_dataset_name: str,
+        bigquery_table_name: Optional[str] = None,
+        gcp_project_id: Optional[str] = None):
+        """Adds a reference in this app to an existing BigQuery table.
+
+        If using this method, Inductor must have been installed with
+        BigQuery support enabled, as follows:
+        `pip install --upgrade inductor[bigquery]`
+
+        If a table is already referenced in this app under the given name, then
+        it must have the characteristics specified by this method call's
+        arguments; otherwise, this method raises an exception.
+
+        Args:
+            name: Name in this app under which to add a reference to the
+                specified existing BigQuery table.
+            bigquery_dataset_name: Name of BigQuery dataset containing the
+                table.
+            bigquery_table_name: Name of existing BigQuery table.  If not
+                provided, the value of the `name` argument is used.
+            gcp_project_id: Optionally, the ID of the Google Cloud project
+                containing the BigQuery table.  If None, then will be inferred
+                from the environment in which this code is running (by Google's
+                BigQuery Python library).
+
+        Raises:
+            RuntimeError: if a table having given name already exists but does
+                not have the characteristics specified by this method call's
+                arguments.
+        """
+        from inductor.data.table import bigquery  # pylint: disable=import-outside-toplevel
+
+        if bigquery_table_name is None:
+            bigquery_table_name = name
+
+        table_spec = locals().copy()
+        del table_spec["self"]
+        del table_spec["bigquery"]
+
+        if not self._run_time:
+            self._table_creation_instructions.append(
+                (self.add_existing_bigquery_table.__name__, table_spec))
+            return
+
+        if name in self:
+            if self.table_spec(name) != table_spec:
+                raise RuntimeError(
+                    f"Table {name} already exists but has different "
+                    "table_spec.")
+        else:
+            t = bigquery.BigQueryTable(
+                dataset_name=bigquery_dataset_name,
+                table_name=bigquery_table_name,
+                project_id=gcp_project_id,
+                auto_ddl=False)
+            already_exists = not self._add_table(
+                name, t, table_spec, skip_if_exists=True, existing_table=True)
+            if (already_exists and
+                self.table_spec(name) != table_spec):
+                raise RuntimeError(
+                    f"Table {name} already exists but has different "
+                    "table_spec.")
```

### Comparing `inductor-0.2.8/inductor/data/table/table_util.py` & `inductor-0.2.9/inductor/data/table/table_util.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/environment.py` & `inductor-0.2.9/inductor/environment.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,57 +35,69 @@
         self,
         app_name: str,
         database_url: str,
         object_store_url: str,
         *,
         http_host: str = "0.0.0.0",
         http_port: int = 80):
+        # pylint: disable=anomalous-backslash-in-string
         """Constructs a new instance.
 
         Args:
             app_name: Name for app in this environment.  Should uniquely
                 identify app among all apps run using Server environment
                 with the same database_url.
             database_url: URL identifying database to be used for storage of
                 app metadata and Inductor-created tables.  This database should
                 be persistent independently of (and accessible from) the compute
                 node or container used to run the app.  The URL should have
                 format
                     system://username:password@host:port/database
-                where ``system`` is either mysql or postgresql.  The database role
-                identified by username should have the ability to create and
-                write to (as well as read) tables in the specified database.
+                where ``system`` is either mysql or postgresql.  The database
+                role identified by username should have the ability to create
+                and write to (as well as read) tables in the specified database.
             object_store_url: URL identifying object storage location to be
                 used for storage of app metadata and data.  This storage
                 location should be persisent independently of (and accessible
                 from) the server (e.g., compute node or container) used to run
                 the app.  The URL should have the following format\:
-                
+
                 - If using a filesystem mounted into node/container (e.g., via
                   Amazon Elastic File System): ``file://path/to/use/``
-                - If using AWS S3: ``s3://bucket/prefix/``, 
+                - If using AWS S3: ``s3://bucket/prefix/``,
+                  where prefix is optional.
+                - If using Google Cloud Storage (GCS): ``gs://bucket/prefix/``,
                   where prefix is optional.
             http_host: Host to which Inductor's web server should bind.
             http_port: Port to which Inductor's web server should bind.
         """
+        # pylint: enable=anomalous-backslash-in-string
+        # Validate arguments
+        if not database_url.startswith(("mysql", "postgresql", "postgres")):
+            raise ValueError(
+                "database_url must start with mysql:// or postgresql://")
+        if not object_store_url.startswith(("file://", "s3://", "gs://")):
+            raise ValueError(
+                "object_store_url must start with file://, s3://, or gs://")
+        # Set instance fields
         self.app_name = app_name
         self.database_url = database_url
         self.object_store_url = object_store_url
         self.http_host = http_host
         self.http_port = http_port
 
 
 class InductorCloud(Local):
     """Environment representing Inductor's cloud deployment service."""
 
     def __init__(
         self,
         app_name: str):
         """Constructs a new InductorCloud instance.
-        
+
         Args:
             app_name: Name for app in this environment.  Should uniquely
                 identify app among all apps run using InductorCloud
                 environment within a given deployment account.
         """
         super().__init__(
             base_dir="/home/app_data",
```

### Comparing `inductor-0.2.8/inductor/ml/model_store.py` & `inductor-0.2.9/inductor/ml/model_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import posixpath
 import re
 import tempfile
 import threading
 from typing import Any, Dict, Optional, Tuple
 
 import boto3
+from google.cloud import storage
 import joblib
 
 from inductor import util
 from inductor.data.table import table
 
 class ModelStore(abc.ABC):
     """A persistent collection of models."""
@@ -500,15 +501,15 @@
             local_model_zip_name = f"{model_dir}.zip"
             model_zip_name = f"{model_id}.zip"
             if self._model_prefix is not None:
                 model_zip_name = posixpath.join(
                     self._model_prefix,
                     model_zip_name
                 )
-            shutil.make_archive(model_dir, "zip")
+            shutil.make_archive(model_dir, "zip", model_dir)
             # Upload the zipped model directory.
             with open(local_model_zip_name, "rb") as model_binary:
                 self._client.upload_fileobj(
                     model_binary,
                     self._bucket_name,
                     model_zip_name
                 )
@@ -545,7 +546,100 @@
             shutil.unpack_archive(local_model_zip_name, model_filepath)
             # Read the unzipped model.
             return self._read_model_from_disk(
                 model_filepath,
                 framework_name,
                 storage_metadata
             )
+
+
+class GCSModelStore(_CachedDiskModelStore):
+    """ModelStore backed by Google Cloud Storage (GCS)."""
+
+    def __init__(
+        self,
+        gcs_url: str,
+        metadata_table: table.WithPrimaryKey,
+        unique_id_gen: util.UniqueIdGen,
+    ):
+        """Constructs a new GCSModelStore.
+
+        Args:
+            gcs_url: The GCS URL to be used for model storage, in the format
+                gs://bucket/prefix/ where prefix is optional (and will be
+                prepended to all object names, if provided).
+            metadata_table: Table to be used to persist this ModelStore's
+                metadata.
+            unique_id_gen: UniqueIdGen to be used to generate unique IDs for
+                models added to this ModelStore.  Should produce IDs that are
+                guaranteed to be globally unique within the currently running
+                Inductor app.
+        """
+        super().__init__(metadata_table, unique_id_gen)
+        self._client = storage.Client()
+        # Deconstruct gcs_url
+        gcs_url_blob = storage.Blob.from_string(gcs_url, self._client)
+        self._bucket: storage.Bucket = gcs_url_blob.bucket
+        self._model_prefix = None
+        if gcs_url_blob.name != "":
+            self._model_prefix = gcs_url_blob.name
+
+    def _store_model(self, model: Any, model_id: str) -> Dict[str, Any]:
+        """See base class.
+
+        For consistency with LocalModelStore, this method does not
+        allow model_id to contain "..".
+        """
+        if ".." in model_id:
+            raise ValueError("model_id cannot contain \"..\".")
+        with tempfile.TemporaryDirectory() as tempdir:
+            model_dir = os.path.join(tempdir, model_id)
+            os.makedirs(model_dir)
+            storage_metadata = self._write_model_to_disk(model, model_dir)
+            # Zip the temporary directory.
+            local_model_zip_name = f"{model_dir}.zip"
+            model_zip_name = f"{model_id}.zip"
+            if self._model_prefix is not None:
+                model_zip_name = posixpath.join(
+                    self._model_prefix,
+                    model_zip_name
+                )
+            shutil.make_archive(model_dir, "zip", model_dir)
+            # Upload the zipped model directory.
+            blob = self._bucket.blob(model_zip_name)
+            blob.upload_from_filename(
+                local_model_zip_name,
+                if_generation_match=0)
+            return storage_metadata
+
+    def _get_uncached_model(self, model_name: str) -> Optional[Any]:
+        """See base class."""
+        model_metadata = self._metadata_table.get(model_name)
+        if model_metadata is None:
+            return None
+        storage_metadata_json = model_metadata[
+            "storage_metadata_json"
+        ]
+        storage_metadata = json.loads(storage_metadata_json)
+        framework_name = model_metadata["storage_framework_name"]
+        assert framework_name is not None
+        model_id = model_metadata["model_id"]
+        with tempfile.TemporaryDirectory() as tempdir:
+            model_filepath = os.path.join(tempdir, model_id)
+            os.makedirs(model_filepath)
+            # Download the zipped model.
+            local_model_zip_name = f"{model_filepath}.zip"
+            model_zip_name = f"{model_id}.zip"
+            if self._model_prefix is not None:
+                model_zip_name = posixpath.join(
+                    self._model_prefix,
+                    model_zip_name
+                )
+            blob = self._bucket.blob(model_zip_name)
+            blob.download_to_filename(local_model_zip_name)
+            shutil.unpack_archive(local_model_zip_name, model_filepath)
+            # Read the unzipped model.
+            return self._read_model_from_disk(
+                model_filepath,
+                framework_name,
+                storage_metadata
+            )
```

### Comparing `inductor-0.2.8/inductor/ui/__init__.py` & `inductor-0.2.9/inductor/ui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     def __init__(
         self,
         container_stack: "_ContainerStack",
         element: _Element,
         id: str,
         get_value: Callable[[Tuple[bool, Any]], Any]):
         """Constructs a new DeferredElement.
-        
+
         Args:
             container_stack: The container stack onto which to append the
                 element.
             element: The element to be deferred.
             id: The id of the element to be deferred.
             get_value: A function that returns the element's current value,
                 given a tuple as returned by _ContainerStack._append().
```

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/asset-manifest.json` & `inductor-0.2.9/inductor/ui/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/index.html` & `inductor-0.2.9/inductor/ui/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/logo192.png` & `inductor-0.2.9/inductor/ui/frontend/build/logo192.png`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/logo512.png` & `inductor-0.2.9/inductor/ui/frontend/build/logo512.png`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/main.742afa3c.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/main.742afa3c.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/main.742afa3c.js.LICENSE.txt` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/main.742afa3c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/main.742afa3c.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/main.742afa3c.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arff.c5d78406.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arff.c5d78406.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brainfuck.373a8f58.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brainfuck.373a8f58.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csv.3eb58e61.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csv.3eb58e61.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gcode.d23c9ac3.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gcode.d23c9ac3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_git.8814e653.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_git.8814e653.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hpkp.74d3b1ac.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hpkp.74d3b1ac.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hsts.f4e5dec7.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hsts.f4e5dec7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js.map` & `inductor-0.2.9/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor/util.py` & `inductor-0.2.9/inductor/util.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.8/inductor.egg-info/SOURCES.txt` & `inductor-0.2.9/inductor.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 inductor.egg-info/requires.txt
 inductor.egg-info/top_level.txt
 inductor/compute/__init__.py
 inductor/compute/common.py
 inductor/compute/local.py
 inductor/data/__init__.py
 inductor/data/table/__init__.py
+inductor/data/table/bigquery.py
 inductor/data/table/dynamodb.py
 inductor/data/table/mysql.py
 inductor/data/table/postgresql.py
 inductor/data/table/snowflake.py
+inductor/data/table/sqlalchemy.py
 inductor/data/table/sqlite.py
 inductor/data/table/table.py
 inductor/data/table/table_catalog.py
 inductor/data/table/table_util.py
 inductor/ml/__init__.py
 inductor/ml/model_store.py
 inductor/ui/__init__.py
```

### Comparing `inductor-0.2.8/setup.cfg` & `inductor-0.2.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = inductor
-version = 0.2.8
+version = 0.2.9
 url = https://inductor.ai
 license_files = LICENSE
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
@@ -21,17 +21,23 @@
 	joblib>=1.2,<2
 	PyMySQL>=1.0.2,<2
 	Pillow>=9.2,<10
 	plotly>=5.11,<6
 	numpy>=1.21.6,<2
 	boto3>=1.24.76,<2
 	psycopg2>=2.9.5,<3
+	google-cloud-storage>=2.8.0,<3
+	SQLAlchemy>=2.0.6,<3
+	alembic>=1.10.2,<2
 python_requires = >=3.7
 
 [options.extras_require]
+bigquery = 
+	google-cloud-bigquery>=3.10.0,<4
+	db-dtypes>=1.1.1,<2
 mysql = 
 	PyMySQL>=1.0.2,<2
 postgres = 
 	psycopg2>=2.9.5,<3
 postgresql = 
 	psycopg2>=2.9.5,<3
 snowflake =
```

