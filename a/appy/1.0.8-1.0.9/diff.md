# Comparing `tmp/appy-1.0.8.tar.gz` & `tmp/appy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appy-1.0.8.tar", last modified: Mon Jul  5 10:28:20 2021, max compression
+gzip compressed data, was "appy-1.0.9.tar", last modified: Tue Oct 26 12:39:34 2021, max compression
```

## Comparing `appy-1.0.8.tar` & `appy-1.0.9.tar`

### file list

```diff
@@ -1,1142 +1,1147 @@
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.186733 appy-1.0.8/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      269 2021-07-05 10:28:20.186733 appy-1.0.8/PKG-INFO
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      345 2021-07-05 10:28:19.866732 appy-1.0.8/README
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.146733 appy-1.0.8/py2/
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.150733 appy-1.0.8/py2/appy/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7263 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/__init__.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.150733 appy-1.0.8/py2/appy/bin/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3657 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/asksap.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    21952 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/backup.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2051 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/checkldap.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     3233 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/checklo.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1011 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/clean.py
--rwxrwxr-x   0 gdy999    (1000) gdy999    (1000)     1088 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/createdebrepo.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8473 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/eggify.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3864 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/generate.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3885 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/job.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17560 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/new.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10676 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/odfgrep.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3045 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/odfwalk.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4393 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/restore.py
--rwxrwxr-x   0 gdy999    (1000) gdy999    (1000)      284 2020-03-04 05:39:19.104383 appy-1.0.8/py2/appy/bin/startlo
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1753 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/zip.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1027 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/bin/zopectl.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.154733 appy-1.0.8/py2/appy/fields/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    80263 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    25381 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/fields/action.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8530 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/boolean.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)   114826 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/fields/calendar.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2714 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/color.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10535 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/computed.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2639 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/custom.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18211 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/date.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9897 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/dict.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    31099 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/fields/file.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3674 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/float.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22449 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/fields/group.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10324 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/fields/hour.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2102 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/info.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6916 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/integer.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    16046 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/fields/list.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13292 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/multilingual.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4104 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/fields/page.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9576 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/fields/phase.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    52905 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/fields/pod.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)   114526 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/fields/ref.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    16205 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/rich.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    54928 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/search.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    20257 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/select.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    59432 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/fields/string.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5774 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/fields/switch.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    35275 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/fields/text.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2402 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/fields/translations.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    32644 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/fields/workflow.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.154733 appy-1.0.8/py2/appy/gen/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15989 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8099 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/authenticate.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    23929 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/descriptors.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    37751 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/generator.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6960 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/indexer.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    21566 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/installer.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    20833 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/layout.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6682 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/mail.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3909 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/migrator.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.154733 appy-1.0.8/py2/appy/gen/mixins/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3448 2021-07-05 10:28:15.082720 appy-1.0.8/py2/appy/gen/mixins/TestMixin.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    78971 2021-07-05 10:28:15.082720 appy-1.0.8/py2/appy/gen/mixins/ToolMixin.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)   103940 2021-07-05 10:28:15.082720 appy-1.0.8/py2/appy/gen/mixins/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19000 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/model.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3171 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/monitoring.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18521 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/navigate.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    14178 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/po.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.154733 appy-1.0.8/py2/appy/gen/templates/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1218 2016-10-11 18:35:13.241440 appy-1.0.8/py2/appy/gen/templates/Class.pyt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11575 2020-04-13 13:43:13.403474 appy-1.0.8/py2/appy/gen/templates/Page.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1464 2016-10-11 18:35:13.237439 appy-1.0.8/py2/appy/gen/templates/__init__.pyt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1424 2016-10-11 18:35:13.241440 appy-1.0.8/py2/appy/gen/templates/config.pyt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      967 2016-10-11 18:35:13.237439 appy-1.0.8/py2/appy/gen/templates/testAll.pyt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1019 2018-07-30 10:01:33.277339 appy-1.0.8/py2/appy/gen/templates/wrappers.pyt
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.154733 appy-1.0.8/py2/appy/gen/tr/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    21051 2020-12-08 12:33:01.908456 appy-1.0.8/py2/appy/gen/tr/Appy.pot
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    21422 2020-12-08 12:33:01.912456 appy-1.0.8/py2/appy/gen/tr/ar.po
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    23517 2020-12-08 12:33:01.916456 appy-1.0.8/py2/appy/gen/tr/de.po
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    28163 2020-12-08 12:33:01.916456 appy-1.0.8/py2/appy/gen/tr/en.po
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22603 2020-12-08 12:33:01.920456 appy-1.0.8/py2/appy/gen/tr/es.po
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    29826 2020-12-08 12:33:00.716461 appy-1.0.8/py2/appy/gen/tr/fr.po
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22639 2020-12-08 12:33:01.928456 appy-1.0.8/py2/appy/gen/tr/it.po
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    25781 2021-04-19 09:41:13.951888 appy-1.0.8/py2/appy/gen/tr/nl.po
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.158733 appy-1.0.8/py2/appy/gen/ui/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      566 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/action.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      240 2016-10-11 18:35:13.669445 appy-1.0.8/py2/appy/gen/ui/add.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      349 2017-12-03 10:34:35.198912 appy-1.0.8/py2/appy/gen/ui/addAbove.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      356 2017-12-03 10:34:31.814888 appy-1.0.8/py2/appy/gen/ui/addAboveFrom.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      346 2017-12-02 13:05:25.147843 appy-1.0.8/py2/appy/gen/ui/addBelow.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      238 2016-10-11 18:35:14.181452 appy-1.0.8/py2/appy/gen/ui/addFrom.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      209 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/angled.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    15738 2021-07-02 12:35:42.495385 appy-1.0.8/py2/appy/gen/ui/appy.css
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    70727 2021-07-02 12:20:41.324547 appy-1.0.8/py2/appy/gen/ui/appy.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      317 2016-10-11 18:35:14.181452 appy-1.0.8/py2/appy/gen/ui/appyrtl.css
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      234 2016-10-11 18:35:14.193452 appy-1.0.8/py2/appy/gen/ui/arrowDown.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      218 2016-10-11 18:35:14.181452 appy-1.0.8/py2/appy/gen/ui/arrowLeft.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      229 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/arrowRight.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      234 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/arrowUp.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      242 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/arrowsDown.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      236 2016-10-11 18:35:14.177452 appy-1.0.8/py2/appy/gen/ui/arrowsLeft.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      235 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/arrowsRight.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      241 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/arrowsUp.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      821 2016-10-11 18:35:14.181452 appy-1.0.8/py2/appy/gen/ui/back.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    62923 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/banner.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    63085 2016-10-11 18:35:13.669445 appy-1.0.8/py2/appy/gen/ui/bannerrtl.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      953 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/calendar.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9852 2017-12-20 08:06:29.446130 appy-1.0.8/py2/appy/gen/ui/calendar.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      272 2016-10-11 18:35:14.193452 appy-1.0.8/py2/appy/gen/ui/cancel.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      255 2016-10-11 18:35:14.189453 appy-1.0.8/py2/appy/gen/ui/changes.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      250 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/changesNo.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      235 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/checkall.png
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.158733 appy-1.0.8/py2/appy/gen/ui/ckeditor/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      289 2016-10-11 18:35:14.189453 appy-1.0.8/py2/appy/gen/ui/ckeditor/Readme
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1471 2019-02-26 14:12:27.837745 appy-1.0.8/py2/appy/gen/ui/ckeditor/config.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1855 2016-10-11 18:35:14.189453 appy-1.0.8/py2/appy/gen/ui/ckeditor/contents.css
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      365 2016-12-20 19:09:41.746375 appy-1.0.8/py2/appy/gen/ui/ckeditor/styles.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      219 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/close.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      159 2017-01-11 15:15:14.258984 appy-1.0.8/py2/appy/gen/ui/collapse.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      883 2016-10-11 18:35:14.181452 appy-1.0.8/py2/appy/gen/ui/config.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      244 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/current.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      231 2016-10-11 18:35:14.181452 appy-1.0.8/py2/appy/gen/ui/delete.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      259 2016-10-11 18:35:14.177452 appy-1.0.8/py2/appy/gen/ui/deleteMany.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      475 2019-12-03 14:05:11.171558 appy-1.0.8/py2/appy/gen/ui/doc.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      514 2016-10-11 18:35:14.193452 appy-1.0.8/py2/appy/gen/ui/docFrozen.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      544 2019-12-03 14:05:00.663564 appy-1.0.8/py2/appy/gen/ui/docx.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      540 2019-12-03 14:07:37.223567 appy-1.0.8/py2/appy/gen/ui/docxFrozen.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      248 2016-10-11 18:35:14.193452 appy-1.0.8/py2/appy/gen/ui/done.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      424 2016-10-11 18:35:14.193452 appy-1.0.8/py2/appy/gen/ui/edit.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      760 2016-10-11 18:35:14.177452 appy-1.0.8/py2/appy/gen/ui/email.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      163 2017-01-11 15:15:40.939234 appy-1.0.8/py2/appy/gen/ui/expand.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      685 2016-10-11 18:35:14.193452 appy-1.0.8/py2/appy/gen/ui/external.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      657 2016-10-11 18:35:14.181452 appy-1.0.8/py2/appy/gen/ui/fake.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       62 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/fakeTransition.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4286 2016-10-11 18:35:13.669445 appy-1.0.8/py2/appy/gen/ui/favicon.ico
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      903 2016-10-11 18:35:13.665445 appy-1.0.8/py2/appy/gen/ui/folder.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      350 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/freeze.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      177 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/frozen.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      719 2016-10-11 18:35:14.177452 appy-1.0.8/py2/appy/gen/ui/funnel.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      235 2016-10-11 18:35:13.669445 appy-1.0.8/py2/appy/gen/ui/gotoNumber.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      222 2020-03-27 14:21:32.474700 appy-1.0.8/py2/appy/gen/ui/gotoSource.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      591 2016-10-11 18:35:14.177452 appy-1.0.8/py2/appy/gen/ui/help.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      240 2017-01-12 08:32:32.441065 appy-1.0.8/py2/appy/gen/ui/hide.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      143 2019-04-16 12:16:08.856283 appy-1.0.8/py2/appy/gen/ui/icon_blank.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      281 2019-04-11 18:56:00.291958 appy-1.0.8/py2/appy/gen/ui/icon_bold.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      140 2019-04-16 12:16:46.960454 appy-1.0.8/py2/appy/gen/ui/icon_dash.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      396 2019-04-16 10:26:15.605046 appy-1.0.8/py2/appy/gen/ui/icon_highlight.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      279 2019-04-12 05:54:24.481362 appy-1.0.8/py2/appy/gen/ui/icon_italic.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      343 2019-04-16 12:21:21.257668 appy-1.0.8/py2/appy/gen/ui/icon_lengthen.png
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.158733 appy-1.0.8/py2/appy/gen/ui/jscalendar/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4830 2016-10-11 18:35:13.677446 appy-1.0.8/py2/appy/gen/ui/jscalendar/calendar-blue.css
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5057 2016-10-11 18:35:13.945449 appy-1.0.8/py2/appy/gen/ui/jscalendar/calendar-setup.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    34353 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/jscalendar/calendar.js
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.158733 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1011 2016-10-11 18:35:13.933449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-af.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2135 2016-10-11 18:35:13.933449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-al.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3723 2016-10-11 18:35:13.941449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-bg.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3525 2016-10-11 18:35:13.945449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-big5-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3290 2016-10-11 18:35:13.941449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-big5.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3706 2016-10-11 18:35:13.937449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-br.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3597 2016-10-11 18:35:13.941449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-ca.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2940 2016-10-11 18:35:13.941449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-cs-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2810 2016-10-11 18:35:13.933449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-cs-win.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3500 2016-10-11 18:35:13.941449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-da.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3863 2016-10-11 18:35:13.941449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-de.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1143 2016-10-11 18:35:13.945449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-du.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3241 2016-10-11 18:35:13.933449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-el.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3600 2016-10-11 18:35:13.933449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-en.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3917 2016-10-11 18:35:13.941449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-es.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3827 2016-10-11 18:35:13.945449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-eu.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2782 2016-10-11 18:35:13.941449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-fi.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4071 2016-10-11 18:35:13.937449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-fr.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3919 2016-10-11 18:35:13.929449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-he-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1553 2016-10-11 18:35:13.933449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-hr-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3088 2016-10-11 18:35:13.937449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-hr.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3603 2016-10-11 18:35:13.945449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-hu.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3633 2016-10-11 18:35:13.937449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-it.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      913 2016-10-11 18:35:13.937449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-jp.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3568 2016-10-11 18:35:13.941449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-ko-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3256 2016-10-11 18:35:13.945449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-ko.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3432 2016-10-11 18:35:13.937449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-lt-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3400 2016-10-11 18:35:13.937449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-lt.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3603 2016-10-11 18:35:13.937449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-lv.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2234 2016-10-11 18:35:13.937449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-nl.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3178 2016-10-11 18:35:13.945449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-no.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2635 2016-10-11 18:35:13.933449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-pl-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2414 2016-10-11 18:35:13.937449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-pl.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3526 2016-10-11 18:35:13.937449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-pt.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2058 2016-10-11 18:35:13.929449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-ro.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3985 2016-10-11 18:35:13.929449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-ru-UTF.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4357 2016-10-11 18:35:13.933449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-ru.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3643 2016-10-11 18:35:13.941449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-ru_win_.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2684 2016-10-11 18:35:13.945449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-si.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2661 2016-10-11 18:35:13.945449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-sk.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3015 2016-10-11 18:35:13.937449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-sp.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2759 2016-10-11 18:35:13.945449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-sr-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5492 2016-10-11 18:35:13.941449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-sr.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3973 2016-10-11 18:35:13.941449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-sv.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1736 2016-10-11 18:35:13.941449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-tr.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3082 2016-10-11 18:35:13.937449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-zh.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4751 2016-10-11 18:35:13.941449 appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/cn_utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       68 2016-10-11 18:35:13.945449 appy-1.0.8/py2/appy/gen/ui/jscalendar/menuarrow.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       49 2016-10-11 18:35:13.677446 appy-1.0.8/py2/appy/gen/ui/jscalendar/menuarrow2.gif
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.150733 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.158733 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/aqua/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       89 2016-10-11 18:35:13.677446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/aqua/active-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       85 2016-10-11 18:35:13.677446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/aqua/dark-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       89 2016-10-11 18:35:13.677446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/aqua/hover-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       49 2016-10-11 18:35:13.677446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/aqua/menuarrow.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      110 2016-10-11 18:35:13.677446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/aqua/normal-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      110 2016-10-11 18:35:13.677446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/aqua/rowhover-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      116 2016-10-11 18:35:13.677446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/aqua/status-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5576 2016-10-11 18:35:13.677446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/aqua/theme.css
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      116 2016-10-11 18:35:13.677446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/aqua/title-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1122 2016-10-11 18:35:13.677446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/aqua/today-bg.gif
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.162733 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/tiger/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/tiger/active-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/tiger/dark-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/tiger/hover-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       49 2016-10-11 18:35:13.681446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/tiger/menuarrow.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/tiger/normal-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/tiger/rowhover-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      149 2016-10-11 18:35:13.685446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/tiger/status-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5772 2016-10-11 18:35:13.681446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/tiger/theme.css
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      149 2016-10-11 18:35:13.681446 appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/tiger/title-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       51 2016-10-11 18:35:14.193452 appy-1.0.8/py2/appy/gen/ui/li.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      234 2016-10-11 18:35:13.665445 appy-1.0.8/py2/appy/gen/ui/link.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      288 2016-10-11 18:35:14.193452 appy-1.0.8/py2/appy/gen/ui/linkMany.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.669445 appy-1.0.8/py2/appy/gen/ui/lirtl.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1281 2016-10-11 18:35:13.665445 appy-1.0.8/py2/appy/gen/ui/loading.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10766 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/loadingBig.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1516 2016-10-11 18:35:14.181452 appy-1.0.8/py2/appy/gen/ui/loadingBtn.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3429 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/loadingPod.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      648 2016-10-11 18:35:13.665445 appy-1.0.8/py2/appy/gen/ui/locked.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1634 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/lockedBig.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      173 2016-10-11 18:35:13.669445 appy-1.0.8/py2/appy/gen/ui/login.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5251 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/logo.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      647 2019-04-13 09:53:33.530200 appy-1.0.8/py2/appy/gen/ui/logout.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      281 2019-04-25 08:27:36.922217 appy-1.0.8/py2/appy/gen/ui/more.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      233 2016-10-11 18:35:14.189453 appy-1.0.8/py2/appy/gen/ui/move.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      229 2016-10-11 18:35:13.669445 appy-1.0.8/py2/appy/gen/ui/next.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      114 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/object.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      663 2016-10-11 18:35:14.177452 appy-1.0.8/py2/appy/gen/ui/ods.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      668 2016-10-11 18:35:14.189453 appy-1.0.8/py2/appy/gen/ui/odsFrozen.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      470 2016-10-11 18:35:14.177452 appy-1.0.8/py2/appy/gen/ui/odt.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      493 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/odtFrozen.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2403 2016-10-11 18:35:14.177452 appy-1.0.8/py2/appy/gen/ui/ogone.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      665 2017-04-03 19:23:17.060212 appy-1.0.8/py2/appy/gen/ui/paperclip.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      432 2016-10-11 18:35:14.189453 appy-1.0.8/py2/appy/gen/ui/pdf.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      485 2016-10-11 18:35:13.669445 appy-1.0.8/py2/appy/gen/ui/pdfFrozen.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      251 2016-10-11 18:35:14.177452 appy-1.0.8/py2/appy/gen/ui/plus.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      225 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/previous.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      607 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/pwd.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      834 2019-09-05 19:39:24.843870 appy-1.0.8/py2/appy/gen/ui/refresh.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      632 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/reindex.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      168 2018-09-27 14:01:52.821020 appy-1.0.8/py2/appy/gen/ui/repeated.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      179 2018-09-27 14:03:43.909542 appy-1.0.8/py2/appy/gen/ui/repeated_last.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       53 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/required.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      513 2016-10-11 18:35:13.669445 appy-1.0.8/py2/appy/gen/ui/save.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      297 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/search.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      240 2017-01-12 08:32:59.861142 appy-1.0.8/py2/appy/gen/ui/show.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      367 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/sortAsc.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      316 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/sortDesc.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      165 2016-12-20 19:09:41.746375 appy-1.0.8/py2/appy/gen/ui/sortDown.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      165 2016-12-20 19:09:41.746375 appy-1.0.8/py2/appy/gen/ui/sortUp.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       43 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/space.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      211 2016-10-11 18:35:14.193452 appy-1.0.8/py2/appy/gen/ui/to.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      250 2016-10-11 18:35:13.669445 appy-1.0.8/py2/appy/gen/ui/toggleDetails.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      653 2016-10-11 18:35:14.177452 appy-1.0.8/py2/appy/gen/ui/transition.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      442 2016-10-11 18:35:14.177452 appy-1.0.8/py2/appy/gen/ui/unfreeze.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      231 2016-10-11 18:35:14.181452 appy-1.0.8/py2/appy/gen/ui/unlink.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      256 2016-10-11 18:35:14.177452 appy-1.0.8/py2/appy/gen/ui/unlinkMany.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      243 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/unlinkManyUp.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      234 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/unlinkUp.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      649 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/unlock.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1662 2016-10-11 18:35:14.189453 appy-1.0.8/py2/appy/gen/ui/unlockBig.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      391 2016-10-11 18:35:13.669445 appy-1.0.8/py2/appy/gen/ui/unselect.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      421 2016-10-11 18:35:13.669445 appy-1.0.8/py2/appy/gen/ui/upload.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      620 2017-04-03 19:27:08.317931 appy-1.0.8/py2/appy/gen/ui/url.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      643 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/user.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      208 2016-10-11 18:35:14.185452 appy-1.0.8/py2/appy/gen/ui/validate.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      314 2016-10-11 18:35:14.181452 appy-1.0.8/py2/appy/gen/ui/warning.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2003 2016-10-11 18:35:13.669445 appy-1.0.8/py2/appy/gen/ui/warningBig.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      823 2016-10-11 18:35:13.673446 appy-1.0.8/py2/appy/gen/ui/warning_no.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      623 2016-10-11 18:35:13.665445 appy-1.0.8/py2/appy/gen/ui/xls.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      621 2016-10-11 18:35:14.193452 appy-1.0.8/py2/appy/gen/ui/xlsFrozen.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      967 2019-12-04 17:19:06.274123 appy-1.0.8/py2/appy/gen/ui/xlsx.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      908 2019-12-04 17:19:21.402216 appy-1.0.8/py2/appy/gen/ui/xlsxFrozen.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    19476 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/utils.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6824 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/gen/validate.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.162733 appy-1.0.8/py2/appy/gen/wrappers/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1760 2021-07-05 10:28:15.082720 appy-1.0.8/py2/appy/gen/wrappers/GroupWrapper.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2753 2021-07-05 10:28:15.082720 appy-1.0.8/py2/appy/gen/wrappers/PageWrapper.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    29396 2021-07-05 10:28:15.082720 appy-1.0.8/py2/appy/gen/wrappers/ToolWrapper.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3987 2021-07-05 10:28:15.082720 appy-1.0.8/py2/appy/gen/wrappers/TranslationWrapper.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    24774 2021-07-05 10:28:15.082720 appy-1.0.8/py2/appy/gen/wrappers/UserWrapper.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    78360 2021-07-05 10:28:15.082720 appy-1.0.8/py2/appy/gen/wrappers/__init__.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.162733 appy-1.0.8/py2/appy/pod/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4102 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/pod/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    25928 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/pod/actions.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    41228 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/pod/buffers.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1588 2020-06-18 10:20:35.111440 appy-1.0.8/py2/appy/pod/content.xmlt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    40864 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/pod/converter.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    32711 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/pod/doc_importers.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11932 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/pod/elements.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      861 2016-10-11 18:35:10.749406 appy-1.0.8/py2/appy/pod/imageNotFound.jpg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13624 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/pod/lo_pool.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1755 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/pod/metadata.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2627 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/pod/odf_parser.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4755 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/pod/parts.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18249 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/pod/pod_parser.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    47977 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/pod/renderer.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7399 2020-06-18 10:20:24.867400 appy-1.0.8/py2/appy/pod/styles.xmlt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    76691 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/pod/styles_manager.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.162733 appy-1.0.8/py2/appy/pod/test/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      896 2016-10-11 18:35:11.569417 appy-1.0.8/py2/appy/pod/test/Readme.txt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10345 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/pod/test/Tester.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    32792 2019-04-30 18:41:55.458187 appy-1.0.8/py2/appy/pod/test/Tests.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)        2 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/pod/test/__init__.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.162733 appy-1.0.8/py2/appy/pod/test/contexts/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       64 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/Chart1.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      164 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/ElseStatements.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       29 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/Empty.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       24 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/FieldExpressions.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      138 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/FileHandlerImport.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      897 2016-10-11 18:35:11.569417 appy-1.0.8/py2/appy/pod/test/contexts/ForCell6.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      222 2018-03-21 10:11:39.856653 appy-1.0.8/py2/appy/pod/test/contexts/IfAndFors1.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      674 2021-03-19 11:00:49.881946 appy-1.0.8/py2/appy/pod/test/contexts/ImagesImport.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      145 2020-03-30 13:54:07.615859 appy-1.0.8/py2/appy/pod/test/contexts/OdsSimple.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       35 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/OnlyExpressions.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       90 2016-10-11 18:35:11.569417 appy-1.0.8/py2/appy/pod/test/contexts/PathImport.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      177 2016-10-11 18:35:11.569417 appy-1.0.8/py2/appy/pod/test/contexts/PersonsEight.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      110 2016-10-11 18:35:11.569417 appy-1.0.8/py2/appy/pod/test/contexts/PersonsFour.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       96 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/PersonsThree.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       82 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/PersonsTwo.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       11 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/SimpleForEmptyList.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       37 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/SimpleForFilledList.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      109 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/SimpleForRow.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       11 2016-10-11 18:35:11.569417 appy-1.0.8/py2/appy/pod/test/contexts/SimpleIfIsFalse.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       10 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/SimpleIfIsTrue.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       59 2016-10-11 18:35:11.569417 appy-1.0.8/py2/appy/pod/test/contexts/SimpleTest.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      200 2018-04-18 08:13:19.908963 appy-1.0.8/py2/appy/pod/test/contexts/VarStatements.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11773 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlColgroupTable.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      703 2018-05-09 13:51:33.061535 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1849 2019-01-21 10:35:00.678872 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex2.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4299 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex3.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2790 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex4.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1805 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex5.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      278 2016-10-11 18:35:11.569417 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex6.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      582 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex7.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      965 2016-10-11 18:35:11.569417 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex8.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17472 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex9.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1883 2017-02-21 15:47:38.805767 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplexTables.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2897 2018-11-30 09:19:28.792011 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlCustomStyles.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)       45 2021-05-05 10:01:24.912056 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlEmpty.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      224 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlEntities.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      128 2018-03-21 17:53:35.842060 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlHtml.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2424 2020-03-30 15:33:06.485025 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlKeepWithNext.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      507 2017-08-24 11:13:10.512979 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlListProperties.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      536 2016-12-20 19:09:41.282375 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlNominal.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      666 2018-08-10 09:28:18.208453 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlPIntoLis.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      449 2020-09-10 06:25:29.085683 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlPIntoTds.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1903 2020-11-12 08:06:18.007973 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlSpan.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      241 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlStylesErrors.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      533 2018-04-18 13:44:15.821519 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlStylesMapping.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      251 2019-04-05 09:02:47.358611 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlStylesMapping2.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      372 2017-08-24 13:20:05.929231 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlTableProperties.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4047 2020-12-18 09:01:19.997088 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlTables.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2466 2017-05-24 07:34:37.512122 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlTwisted.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      629 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/XhtmlWithStyle.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      596 2016-10-11 18:35:11.565417 appy-1.0.8/py2/appy/pod/test/contexts/__init__.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.162733 appy-1.0.8/py2/appy/pod/test/images/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    34607 2016-12-20 19:09:41.142375 appy-1.0.8/py2/appy/pod/test/images/imio.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1495 2016-10-11 18:35:11.193412 appy-1.0.8/py2/appy/pod/test/images/linux.jpg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2412 2016-10-11 18:35:11.193412 appy-1.0.8/py2/appy/pod/test/images/plone.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1194 2016-10-11 18:35:11.193412 appy-1.0.8/py2/appy/pod/test/images/python.blob
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1194 2016-10-11 18:35:11.193412 appy-1.0.8/py2/appy/pod/test/images/python.gif
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.166733 appy-1.0.8/py2/appy/pod/test/results/
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    19703 2018-10-25 14:45:50.975494 appy-1.0.8/py2/appy/pod/test/results/chart1.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    19091 2018-10-25 14:42:01.882667 appy-1.0.8/py2/appy/pod/test/results/elseStatements.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7135 2016-10-11 18:35:11.173412 appy-1.0.8/py2/appy/pod/test/results/errorExpression.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11203 2018-10-25 14:50:32.400074 appy-1.0.8/py2/appy/pod/test/results/errorFooter.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7897 2019-07-25 15:08:59.443306 appy-1.0.8/py2/appy/pod/test/results/errorForParsetime.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7493 2016-10-11 18:35:11.189412 appy-1.0.8/py2/appy/pod/test/results/errorForRuntime.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11078 2016-12-20 19:09:40.962375 appy-1.0.8/py2/appy/pod/test/results/errorIf.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10870 2017-03-10 11:06:25.495770 appy-1.0.8/py2/appy/pod/test/results/fieldExpression.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    32790 2016-10-11 18:35:11.173412 appy-1.0.8/py2/appy/pod/test/results/fileHandlerImport.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11477 2018-10-25 13:41:43.473558 appy-1.0.8/py2/appy/pod/test/results/forCellBug.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10603 2018-10-25 13:42:31.293675 appy-1.0.8/py2/appy/pod/test/results/forCellBug2.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10676 2018-10-25 11:43:47.720535 appy-1.0.8/py2/appy/pod/test/results/forCellCorrectNumber.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10675 2018-10-25 13:28:27.919030 appy-1.0.8/py2/appy/pod/test/results/forCellNotEnough.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7234 2018-10-25 13:41:03.329466 appy-1.0.8/py2/appy/pod/test/results/forCellOnlyOne.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10671 2018-10-25 13:36:23.156984 appy-1.0.8/py2/appy/pod/test/results/forCellTooMuch1.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7300 2018-10-25 13:37:22.705060 appy-1.0.8/py2/appy/pod/test/results/forCellTooMuch2.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7373 2018-10-25 13:39:50.333311 appy-1.0.8/py2/appy/pod/test/results/forCellTooMuch3.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7393 2018-10-25 13:40:12.865357 appy-1.0.8/py2/appy/pod/test/results/forCellTooMuch4.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7042 2018-10-25 13:43:24.941812 appy-1.0.8/py2/appy/pod/test/results/forTable.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7819 2016-10-11 18:35:11.173412 appy-1.0.8/py2/appy/pod/test/results/forTableMinus.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8351 2018-10-25 14:39:09.105860 appy-1.0.8/py2/appy/pod/test/results/forTableMinus2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8140 2016-10-11 18:35:11.181412 appy-1.0.8/py2/appy/pod/test/results/forTableMinusError.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8175 2016-10-11 18:35:11.177412 appy-1.0.8/py2/appy/pod/test/results/forTableMinusError2.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11104 2018-10-25 14:39:58.542092 appy-1.0.8/py2/appy/pod/test/results/headerFooter.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    16676 2019-08-01 13:30:20.267359 appy-1.0.8/py2/appy/pod/test/results/ifAndFors1.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12528 2018-10-25 14:51:25.620213 appy-1.0.8/py2/appy/pod/test/results/ifElseErrors.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    59201 2021-04-20 14:20:52.878622 appy-1.0.8/py2/appy/pod/test/results/imagesImport.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8882 2018-10-25 11:46:29.553242 appy-1.0.8/py2/appy/pod/test/results/noPython.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12331 2020-03-30 13:54:09.699867 appy-1.0.8/py2/appy/pod/test/results/odsSimple.ods
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     9183 2018-10-25 11:54:22.215347 appy-1.0.8/py2/appy/pod/test/results/onlyExpressions.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    32780 2016-10-11 18:35:11.181412 appy-1.0.8/py2/appy/pod/test/results/pathImport.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6867 2016-10-11 18:35:11.189412 appy-1.0.8/py2/appy/pod/test/results/simpleForEmptyList.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6966 2016-10-11 18:35:11.189412 appy-1.0.8/py2/appy/pod/test/results/simpleForFilledList.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7560 2018-10-25 11:55:36.451696 appy-1.0.8/py2/appy/pod/test/results/simpleForRow.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10991 2018-10-25 14:41:02.730392 appy-1.0.8/py2/appy/pod/test/results/simpleFromTest.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6910 2016-10-11 18:35:11.177412 appy-1.0.8/py2/appy/pod/test/results/simpleIfIsFalse.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6923 2016-10-11 18:35:11.189412 appy-1.0.8/py2/appy/pod/test/results/simpleIfIsTrue.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8666 2016-10-11 18:35:11.185412 appy-1.0.8/py2/appy/pod/test/results/simpleIfIsTrue003.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7919 2016-10-11 18:35:11.181412 appy-1.0.8/py2/appy/pod/test/results/simpleMinusError.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8606 2016-10-11 18:35:11.169412 appy-1.0.8/py2/appy/pod/test/results/simpleTest.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    13100 2018-10-25 14:43:25.231053 appy-1.0.8/py2/appy/pod/test/results/varDef.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    15538 2018-10-25 11:53:33.595124 appy-1.0.8/py2/appy/pod/test/results/withAnImage.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11053 2016-10-11 18:35:11.193412 appy-1.0.8/py2/appy/pod/test/results/xhtmlColgroup.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    13969 2019-11-15 14:58:08.486379 appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11785 2019-01-21 13:08:50.714374 appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex2.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11178 2019-07-25 11:50:40.717704 appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex3.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8796 2019-07-25 11:52:03.761669 appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex4.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8906 2019-07-25 11:52:51.685670 appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex5.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8469 2018-11-30 09:50:11.162546 appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex6.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8576 2016-10-11 18:35:11.165412 appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex7.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11010 2019-07-25 11:53:44.341687 appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex8.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13568 2017-02-21 15:05:31.684520 appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex9.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    17763 2018-10-25 14:46:49.543589 appy-1.0.8/py2/appy/pod/test/results/xhtmlComplexTables.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    13090 2018-11-30 09:44:53.993350 appy-1.0.8/py2/appy/pod/test/results/xhtmlCustomStyles.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11729 2017-02-21 16:29:51.874710 appy-1.0.8/py2/appy/pod/test/results/xhtmlEmpty.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11948 2016-10-11 18:35:11.177412 appy-1.0.8/py2/appy/pod/test/results/xhtmlEntities.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10430 2018-03-21 16:01:33.686184 appy-1.0.8/py2/appy/pod/test/results/xhtmlHtml.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12045 2016-10-11 18:35:11.185412 appy-1.0.8/py2/appy/pod/test/results/xhtmlIgnoreStyles.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    13512 2019-07-25 11:58:13.653988 appy-1.0.8/py2/appy/pod/test/results/xhtmlInHeader.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15813 2020-12-18 09:47:54.242437 appy-1.0.8/py2/appy/pod/test/results/xhtmlKeepWithNext.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12143 2019-07-25 11:56:13.833816 appy-1.0.8/py2/appy/pod/test/results/xhtmlListProperties.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    35579 2016-12-20 19:09:40.962375 appy-1.0.8/py2/appy/pod/test/results/xhtmlNominal.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12112 2019-07-25 11:57:05.201883 appy-1.0.8/py2/appy/pod/test/results/xhtmlPIntoLis.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12010 2020-09-10 06:25:34.225663 appy-1.0.8/py2/appy/pod/test/results/xhtmlPIntoTds.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12521 2020-11-12 08:19:53.610753 appy-1.0.8/py2/appy/pod/test/results/xhtmlSpan.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13311 2016-10-11 18:35:11.189412 appy-1.0.8/py2/appy/pod/test/results/xhtmlStylesErrors.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15494 2018-04-18 16:14:08.596004 appy-1.0.8/py2/appy/pod/test/results/xhtmlStylesMapping.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11978 2019-04-05 09:10:26.884697 appy-1.0.8/py2/appy/pod/test/results/xhtmlStylesMapping2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12008 2017-08-24 12:42:14.129789 appy-1.0.8/py2/appy/pod/test/results/xhtmlTableProperties.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10632 2020-11-12 11:15:48.436856 appy-1.0.8/py2/appy/pod/test/results/xhtmlTables.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10944 2017-05-24 07:39:04.437787 appy-1.0.8/py2/appy/pod/test/results/xhtmlTwisted.odt
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.166733 appy-1.0.8/py2/appy/pod/test/templates/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19316 2016-10-11 18:35:10.757406 appy-1.0.8/py2/appy/pod/test/templates/Chart1.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18252 2016-10-11 18:35:10.761406 appy-1.0.8/py2/appy/pod/test/templates/ElseStatements.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6410 2016-10-11 18:35:10.753406 appy-1.0.8/py2/appy/pod/test/templates/ErrorExpression.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10018 2016-10-11 18:35:10.753406 appy-1.0.8/py2/appy/pod/test/templates/ErrorFooter.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6916 2016-10-11 18:35:10.753406 appy-1.0.8/py2/appy/pod/test/templates/ErrorForParsetime.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6832 2016-10-11 18:35:10.761406 appy-1.0.8/py2/appy/pod/test/templates/ErrorForRuntime.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10085 2018-03-28 10:15:57.831696 appy-1.0.8/py2/appy/pod/test/templates/ErrorIf.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9928 2017-03-10 10:26:07.118621 appy-1.0.8/py2/appy/pod/test/templates/FieldExpressions.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7465 2016-10-11 18:35:10.753406 appy-1.0.8/py2/appy/pod/test/templates/FileHandlerImport.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9790 2018-10-25 11:43:44.328520 appy-1.0.8/py2/appy/pod/test/templates/ForCell.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6881 2016-10-11 18:35:10.761406 appy-1.0.8/py2/appy/pod/test/templates/ForCell2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6934 2016-10-11 18:35:10.765406 appy-1.0.8/py2/appy/pod/test/templates/ForCell3.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6952 2016-10-11 18:35:10.765406 appy-1.0.8/py2/appy/pod/test/templates/ForCell4.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6732 2016-10-11 18:35:10.765406 appy-1.0.8/py2/appy/pod/test/templates/ForCell5.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11001 2016-10-11 18:35:10.765406 appy-1.0.8/py2/appy/pod/test/templates/ForCell6.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10009 2016-10-11 18:35:10.765406 appy-1.0.8/py2/appy/pod/test/templates/ForCell7.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6542 2016-10-11 18:35:10.761406 appy-1.0.8/py2/appy/pod/test/templates/ForTable.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6798 2016-10-11 18:35:10.753406 appy-1.0.8/py2/appy/pod/test/templates/ForTableMinus.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7323 2016-10-11 18:35:10.761406 appy-1.0.8/py2/appy/pod/test/templates/ForTableMinus2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7098 2016-10-11 18:35:10.757406 appy-1.0.8/py2/appy/pod/test/templates/ForTableMinusError.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7099 2016-10-11 18:35:10.761406 appy-1.0.8/py2/appy/pod/test/templates/ForTableMinusError2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10215 2016-10-11 18:35:10.761406 appy-1.0.8/py2/appy/pod/test/templates/HeaderFooter.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    16196 2019-08-01 13:30:18.675353 appy-1.0.8/py2/appy/pod/test/templates/IfAndFors1.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11041 2016-10-11 18:35:10.761406 appy-1.0.8/py2/appy/pod/test/templates/IfElseErrors.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13788 2021-04-20 14:20:51.446617 appy-1.0.8/py2/appy/pod/test/templates/ImagesImport.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8298 2016-10-11 18:35:10.757406 appy-1.0.8/py2/appy/pod/test/templates/NoPython.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11234 2020-03-30 13:53:05.075600 appy-1.0.8/py2/appy/pod/test/templates/OdsSimple.ods
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8810 2016-10-11 18:35:10.757406 appy-1.0.8/py2/appy/pod/test/templates/OnlyExpressions.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7483 2016-10-11 18:35:10.757406 appy-1.0.8/py2/appy/pod/test/templates/PathImport.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6345 2016-10-11 18:35:10.765406 appy-1.0.8/py2/appy/pod/test/templates/SimpleForEmptyList.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6520 2016-10-11 18:35:10.753406 appy-1.0.8/py2/appy/pod/test/templates/SimpleForFilledList.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7160 2016-10-11 18:35:10.761406 appy-1.0.8/py2/appy/pod/test/templates/SimpleForRow.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9750 2016-10-11 18:35:10.757406 appy-1.0.8/py2/appy/pod/test/templates/SimpleFromTest.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6378 2016-10-11 18:35:10.757406 appy-1.0.8/py2/appy/pod/test/templates/SimpleIfIsFalse.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6378 2016-10-11 18:35:10.753406 appy-1.0.8/py2/appy/pod/test/templates/SimpleIfIsTrue.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8227 2016-10-11 18:35:10.765406 appy-1.0.8/py2/appy/pod/test/templates/SimpleIfIsTrue003.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6567 2016-10-11 18:35:10.757406 appy-1.0.8/py2/appy/pod/test/templates/SimpleMinusError.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8250 2016-10-11 18:35:10.761406 appy-1.0.8/py2/appy/pod/test/templates/SimpleTest.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    20714 2017-10-14 13:08:00.664723 appy-1.0.8/py2/appy/pod/test/templates/TablesToOptimize.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12089 2018-04-18 08:14:26.894173 appy-1.0.8/py2/appy/pod/test/templates/VarStatements.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15044 2016-10-11 18:35:10.749406 appy-1.0.8/py2/appy/pod/test/templates/WithAnImage.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12696 2019-11-15 14:58:03.398363 appy-1.0.8/py2/appy/pod/test/templates/Xhtml.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9156 2016-10-11 18:35:10.753406 appy-1.0.8/py2/appy/pod/test/templates/XhtmlColGroup.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10089 2018-04-18 11:50:50.825343 appy-1.0.8/py2/appy/pod/test/templates/XhtmlComplex2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8784 2016-10-11 18:35:10.761406 appy-1.0.8/py2/appy/pod/test/templates/XhtmlComplex3.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7730 2016-10-11 18:35:10.765406 appy-1.0.8/py2/appy/pod/test/templates/XhtmlComplex4.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10801 2016-10-11 18:35:10.765406 appy-1.0.8/py2/appy/pod/test/templates/XhtmlComplex8.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    16551 2016-10-11 18:35:10.757406 appy-1.0.8/py2/appy/pod/test/templates/XhtmlComplexTables.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9431 2018-03-21 15:46:22.391030 appy-1.0.8/py2/appy/pod/test/templates/XhtmlHtml.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12421 2016-10-11 18:35:10.749406 appy-1.0.8/py2/appy/pod/test/templates/XhtmlInHeader.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    14774 2020-03-30 15:36:03.041817 appy-1.0.8/py2/appy/pod/test/templates/XhtmlKeepWithNext.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    34605 2016-10-11 18:35:10.765406 appy-1.0.8/py2/appy/pod/test/templates/XhtmlNominal.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11284 2019-08-07 08:02:36.111421 appy-1.0.8/py2/appy/pod/test/templates/XhtmlSimple.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10674 2017-01-31 15:30:32.145286 appy-1.0.8/py2/appy/pod/test/templates/XhtmlSpan.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14445 2018-04-18 13:45:22.585631 appy-1.0.8/py2/appy/pod/test/templates/XhtmlStyles.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11839 2016-10-11 18:35:10.761406 appy-1.0.8/py2/appy/pod/test/templates/XhtmlStylesErrors.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7834 2016-10-11 18:35:10.761406 appy-1.0.8/py2/appy/pod/test/templates/XhtmlTables.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8930 2017-05-24 07:36:40.164945 appy-1.0.8/py2/appy/pod/test/templates/XhtmlTwisted.odt
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.166733 appy-1.0.8/py2/appy/pod/xhtml/
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      201 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/pod/xhtml/__init__.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     6263 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/pod/xhtml/parser.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10701 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/pod/xhtml/tags.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    15644 2021-07-05 10:28:15.070720 appy-1.0.8/py2/appy/pod/xhtml/visitors.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    63790 2021-07-05 10:28:15.066720 appy-1.0.8/py2/appy/pod/xhtml2odt.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.166733 appy-1.0.8/py2/appy/px/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11440 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/px/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7169 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/px/px_parser.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py2/appy/shared/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3030 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/shared/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9010 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/account.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    20757 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/css.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13090 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/csv_parser.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py2/appy/shared/data/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)   164300 2016-10-11 18:35:13.049437 appy-1.0.8/py2/appy/shared/data/BelgianCommunes.txt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4089 2016-10-11 18:35:13.049437 appy-1.0.8/py2/appy/shared/data/CountryCodesIso3166.1.txt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15371 2016-10-11 18:35:13.049437 appy-1.0.8/py2/appy/shared/data/LanguageCodesIso639.2.txt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9128 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/shared/data/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5457 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/shared/dates.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22926 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/dav.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    33809 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/diff.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1510 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/errors.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4663 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/google.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4922 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/ical.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22457 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/ldap_connector.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2806 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/odf.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14228 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/packaging.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11267 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/sap.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    21740 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/sso.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18472 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/tables.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14857 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/test.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    36843 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/utils.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    58271 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/xml_parser.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7392 2021-07-05 10:28:15.074720 appy-1.0.8/py2/appy/shared/zip.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py2/appy/test/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       77 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/test/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4098 2021-07-05 10:28:15.078720 appy-1.0.8/py2/appy/test/profiler.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       52 2021-07-05 10:28:15.082720 appy-1.0.8/py2/appy/version.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.150733 appy-1.0.8/py3/
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5153 2021-07-05 10:28:19.842732 appy-1.0.8/py3/appy/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2627 2021-07-05 10:28:19.842732 appy-1.0.8/py3/appy/all.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/bin/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2454 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/bin/__init__.py
--rwxr-xr-x   0 gdy999    (1000) gdy999    (1000)     3835 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/bin/deploy.py
--rwxrwxr-x   0 gdy999    (1000) gdy999    (1000)     4681 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/bin/lo.py
--rwxrwxr-x   0 gdy999    (1000) gdy999    (1000)    19152 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/bin/make.py
--rwxrwxr-x   0 gdy999    (1000) gdy999    (1000)     1936 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/bin/perform.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8558 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/bin/run.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/data/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4089 2017-07-31 20:04:30.105511 appy-1.0.8/py3/appy/data/Countries.Iso3166-1
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15371 2017-07-31 20:04:30.105511 appy-1.0.8/py3/appy/data/Languages.Iso639-2
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8658 2021-07-05 10:28:19.866732 appy-1.0.8/py3/appy/data/__init__.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/database/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    42109 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/database/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22244 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/database/catalog.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/database/indexes/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13573 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/database/indexes/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1363 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/database/indexes/boolean.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     3418 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/database/indexes/date.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1604 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/database/indexes/float.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2355 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/database/indexes/ref.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2255 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/database/indexes/rich.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2949 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/database/indexes/text.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5318 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/database/lazy.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7006 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/database/lock.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5379 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/database/log.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9310 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/database/operators.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4675 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/database/sorter.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/deploy/
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10173 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/deploy/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3468 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/deploy/subversion.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/model/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8078 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    65883 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/base.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6189 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/batch.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13492 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/carousel.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8456 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/document.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/model/fields/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    75224 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    26741 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/action.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9012 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/boolean.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)   113499 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/fields/calendar.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2974 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/color.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5485 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/colset.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12130 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/computed.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2912 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/custom.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17499 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/date.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10435 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/dict.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    29254 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/file.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3969 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/float.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    20954 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/fields/group.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10289 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/fields/hour.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2608 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/info.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7130 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/integer.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22023 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/fields/list.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14769 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/multilingual.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12533 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/fields/ogone.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7413 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/password.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22880 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/phase.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    59682 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/fields/pod.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7737 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/python.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)   123734 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/fields/ref.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    24032 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/rich.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    22669 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/select.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14247 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/fields/string.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     5982 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/fields/switch.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    37421 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/fields/text.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2800 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/group.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    16657 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/loader.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/model/meta/
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     4286 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/meta/__init__.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    33587 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/meta/class_.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11812 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/meta/workflow.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    17506 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/page.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/model/pod/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12395 2021-05-09 13:30:32.398004 appy-1.0.8/py3/appy/model/pod/Page.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7314 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/query.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/model/searches/
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    43596 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/searches/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4266 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/searches/gridder.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7053 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/searches/initiators.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    29067 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/searches/modes.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    23247 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/tool.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7547 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/translation.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    31557 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/user.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8172 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/model/utils.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/model/workflow/
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     3653 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/workflow/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    24100 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/workflow/history.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6113 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/workflow/localRoles.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     3508 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/workflow/standard.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     9171 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/workflow/state.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    21154 2021-07-05 10:28:19.854732 appy-1.0.8/py3/appy/model/workflow/transition.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/peer/
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11639 2021-07-05 10:28:19.866732 appy-1.0.8/py3/appy/peer/__init__.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     4957 2021-07-05 10:28:19.866732 appy-1.0.8/py3/appy/peer/appy0.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10937 2021-07-05 10:28:19.866732 appy-1.0.8/py3/appy/peer/importer.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6947 2021-07-05 10:28:19.866732 appy-1.0.8/py3/appy/peer/unresolved.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/pod/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5688 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    27474 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/actions.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    41597 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/buffers.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1588 2020-06-19 06:42:25.671990 appy-1.0.8/py3/appy/pod/content.xmlt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    40794 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/converter.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    30039 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/doc_importers.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12645 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/elements.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      861 2017-07-26 14:43:09.919476 appy-1.0.8/py3/appy/pod/imageNotFound.jpg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13715 2021-07-05 10:28:19.842732 appy-1.0.8/py3/appy/pod/lo_pool.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2755 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/odf_parser.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4840 2021-07-05 10:28:19.842732 appy-1.0.8/py3/appy/pod/parts.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18318 2021-07-05 10:28:19.842732 appy-1.0.8/py3/appy/pod/pod_parser.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    56256 2021-07-05 10:28:19.842732 appy-1.0.8/py3/appy/pod/renderer.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7399 2020-06-19 06:42:33.848014 appy-1.0.8/py3/appy/pod/styles.xmlt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    76930 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/styles_manager.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.170733 appy-1.0.8/py3/appy/pod/test/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      896 2017-07-26 14:43:09.919476 appy-1.0.8/py3/appy/pod/test/Readme.txt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9726 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/test/Tester.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    32727 2020-02-23 10:02:23.292374 appy-1.0.8/py3/appy/pod/test/Tests.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      785 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/test/__init__.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.174733 appy-1.0.8/py3/appy/pod/test/contexts/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       64 2017-07-26 14:43:09.911476 appy-1.0.8/py3/appy/pod/test/contexts/Chart1.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      164 2017-07-26 14:43:09.911476 appy-1.0.8/py3/appy/pod/test/contexts/ElseStatements.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       29 2020-02-22 13:45:39.328852 appy-1.0.8/py3/appy/pod/test/contexts/Empty.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       24 2017-07-26 14:43:09.911476 appy-1.0.8/py3/appy/pod/test/contexts/FieldExpressions.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      138 2017-10-04 14:00:32.106218 appy-1.0.8/py3/appy/pod/test/contexts/FileHandlerImport.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      893 2017-10-04 13:22:14.323421 appy-1.0.8/py3/appy/pod/test/contexts/ForCell6.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      222 2018-03-21 13:34:02.632546 appy-1.0.8/py3/appy/pod/test/contexts/IfAndFors1.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      674 2019-02-08 13:14:02.033243 appy-1.0.8/py3/appy/pod/test/contexts/ImagesImport.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      145 2020-03-30 14:06:40.458959 appy-1.0.8/py3/appy/pod/test/contexts/OdsSimple.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       35 2017-07-26 14:43:09.911476 appy-1.0.8/py3/appy/pod/test/contexts/OnlyExpressions.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       90 2017-07-26 14:43:09.915476 appy-1.0.8/py3/appy/pod/test/contexts/PathImport.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      177 2017-07-26 14:43:09.915476 appy-1.0.8/py3/appy/pod/test/contexts/PersonsEight.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      110 2017-07-26 14:43:09.915476 appy-1.0.8/py3/appy/pod/test/contexts/PersonsFour.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       96 2017-07-26 14:43:09.911476 appy-1.0.8/py3/appy/pod/test/contexts/PersonsThree.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       82 2017-07-26 14:43:09.911476 appy-1.0.8/py3/appy/pod/test/contexts/PersonsTwo.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       11 2017-07-26 14:43:09.907476 appy-1.0.8/py3/appy/pod/test/contexts/SimpleForEmptyList.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       37 2017-07-26 14:43:09.907476 appy-1.0.8/py3/appy/pod/test/contexts/SimpleForFilledList.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      109 2017-07-26 14:43:09.911476 appy-1.0.8/py3/appy/pod/test/contexts/SimpleForRow.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       11 2017-07-26 14:43:09.915476 appy-1.0.8/py3/appy/pod/test/contexts/SimpleIfIsFalse.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       10 2017-07-26 14:43:09.907476 appy-1.0.8/py3/appy/pod/test/contexts/SimpleIfIsTrue.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       59 2017-07-26 14:43:09.915476 appy-1.0.8/py3/appy/pod/test/contexts/SimpleTest.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      200 2018-04-18 09:38:51.803129 appy-1.0.8/py3/appy/pod/test/contexts/VarStatements.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11773 2017-07-26 14:43:09.907476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlColgroupTable.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      703 2017-07-26 14:43:09.911476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1849 2019-01-21 13:13:06.007441 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex2.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4299 2017-07-26 14:43:09.907476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex3.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2790 2017-07-26 14:43:09.915476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex4.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1805 2017-07-26 14:43:09.907476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex5.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      278 2017-07-26 14:43:09.915476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex6.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      582 2017-07-26 14:43:09.907476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex7.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      965 2017-07-26 14:43:09.915476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex8.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17472 2017-07-26 14:43:09.907476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex9.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1883 2017-07-26 14:43:09.903476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplexTables.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2888 2020-02-23 09:39:39.765688 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlCustomStyles.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       45 2021-03-27 12:19:55.818879 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlEmpty.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      224 2017-07-26 14:43:09.907476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlEntities.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      128 2018-03-21 15:59:07.176655 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlHtml.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2424 2019-11-15 10:38:18.049595 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlKeepWithNext.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      507 2017-08-24 11:37:48.121121 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlListProperties.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      536 2017-07-26 14:43:09.903476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlNominal.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      666 2018-08-10 09:28:18.208453 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlPIntoLis.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      449 2020-09-10 08:28:52.116400 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlPIntoTds.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1903 2020-11-12 08:49:44.926234 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlSpan.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      241 2017-07-26 14:43:09.907476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlStylesErrors.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      533 2018-04-18 16:40:08.640038 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlStylesMapping.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      251 2019-04-05 11:20:44.233306 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlStylesMapping2.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      372 2017-08-24 13:20:08.317236 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlTableProperties.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4047 2020-12-18 09:35:25.760508 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlTables.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2466 2017-07-26 14:43:09.903476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlTwisted.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      629 2017-07-26 14:43:09.915476 appy-1.0.8/py3/appy/pod/test/contexts/XhtmlWithStyle.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      596 2017-07-26 14:43:09.907476 appy-1.0.8/py3/appy/pod/test/contexts/__init__.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.174733 appy-1.0.8/py3/appy/pod/test/images/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    34607 2017-07-26 14:43:09.899476 appy-1.0.8/py3/appy/pod/test/images/imio.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1495 2017-07-26 14:43:09.899476 appy-1.0.8/py3/appy/pod/test/images/linux.jpg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2412 2017-07-26 14:43:09.899476 appy-1.0.8/py3/appy/pod/test/images/plone.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1194 2017-07-26 14:43:09.903476 appy-1.0.8/py3/appy/pod/test/images/python.blob
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1194 2017-07-26 14:43:09.899476 appy-1.0.8/py3/appy/pod/test/images/python.gif
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.178733 appy-1.0.8/py3/appy/pod/test/results/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19703 2018-10-26 07:00:22.417921 appy-1.0.8/py3/appy/pod/test/results/chart1.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19091 2018-10-26 07:00:36.537943 appy-1.0.8/py3/appy/pod/test/results/elseStatements.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7135 2017-07-26 14:43:09.883476 appy-1.0.8/py3/appy/pod/test/results/errorExpression.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11203 2018-10-26 07:01:05.593989 appy-1.0.8/py3/appy/pod/test/results/errorFooter.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7897 2019-07-25 15:27:06.620385 appy-1.0.8/py3/appy/pod/test/results/errorForParsetime.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7493 2017-07-26 14:43:09.899476 appy-1.0.8/py3/appy/pod/test/results/errorForRuntime.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11078 2017-07-26 14:43:09.863476 appy-1.0.8/py3/appy/pod/test/results/errorIf.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10870 2017-07-26 14:43:09.867476 appy-1.0.8/py3/appy/pod/test/results/fieldExpression.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    32790 2017-07-26 14:43:09.879476 appy-1.0.8/py3/appy/pod/test/results/fileHandlerImport.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11477 2018-10-26 07:01:39.442042 appy-1.0.8/py3/appy/pod/test/results/forCellBug.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10603 2018-10-26 07:01:48.722056 appy-1.0.8/py3/appy/pod/test/results/forCellBug2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10676 2018-10-26 07:01:56.974070 appy-1.0.8/py3/appy/pod/test/results/forCellCorrectNumber.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10675 2018-10-26 07:02:07.042086 appy-1.0.8/py3/appy/pod/test/results/forCellNotEnough.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7234 2018-10-26 07:02:17.918103 appy-1.0.8/py3/appy/pod/test/results/forCellOnlyOne.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10671 2018-10-26 07:02:28.102119 appy-1.0.8/py3/appy/pod/test/results/forCellTooMuch1.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7300 2018-10-26 07:02:34.502130 appy-1.0.8/py3/appy/pod/test/results/forCellTooMuch2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7373 2018-10-26 07:02:42.746143 appy-1.0.8/py3/appy/pod/test/results/forCellTooMuch3.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7393 2018-10-26 07:02:51.646157 appy-1.0.8/py3/appy/pod/test/results/forCellTooMuch4.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7042 2018-10-26 07:03:33.290224 appy-1.0.8/py3/appy/pod/test/results/forTable.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7819 2017-07-26 14:43:09.883476 appy-1.0.8/py3/appy/pod/test/results/forTableMinus.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8351 2018-10-26 07:03:51.130253 appy-1.0.8/py3/appy/pod/test/results/forTableMinus2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8140 2017-07-26 14:43:09.887476 appy-1.0.8/py3/appy/pod/test/results/forTableMinusError.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8175 2017-07-26 14:43:09.883476 appy-1.0.8/py3/appy/pod/test/results/forTableMinusError2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11104 2018-10-26 07:04:12.142288 appy-1.0.8/py3/appy/pod/test/results/headerFooter.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    16676 2019-08-01 13:36:53.492831 appy-1.0.8/py3/appy/pod/test/results/ifAndFors1.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12580 2020-08-22 18:28:01.490383 appy-1.0.8/py3/appy/pod/test/results/ifElseErrors.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    59201 2021-04-20 14:29:29.072725 appy-1.0.8/py3/appy/pod/test/results/imagesImport.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8882 2018-10-26 07:04:39.662333 appy-1.0.8/py3/appy/pod/test/results/noPython.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12341 2020-03-30 14:11:22.632117 appy-1.0.8/py3/appy/pod/test/results/odsSimple.ods
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9183 2018-10-26 07:04:57.958363 appy-1.0.8/py3/appy/pod/test/results/onlyExpressions.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    32780 2017-07-26 14:43:09.887476 appy-1.0.8/py3/appy/pod/test/results/pathImport.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6867 2017-07-26 14:43:09.895476 appy-1.0.8/py3/appy/pod/test/results/simpleForEmptyList.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6966 2017-07-26 14:43:09.895476 appy-1.0.8/py3/appy/pod/test/results/simpleForFilledList.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7560 2018-10-26 07:05:07.310379 appy-1.0.8/py3/appy/pod/test/results/simpleForRow.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11135 2020-02-23 08:45:30.387467 appy-1.0.8/py3/appy/pod/test/results/simpleFromTest.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6910 2017-07-26 14:43:09.883476 appy-1.0.8/py3/appy/pod/test/results/simpleIfIsFalse.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6923 2017-07-26 14:43:09.895476 appy-1.0.8/py3/appy/pod/test/results/simpleIfIsTrue.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8666 2017-07-26 14:43:09.887476 appy-1.0.8/py3/appy/pod/test/results/simpleIfIsTrue003.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7919 2017-07-26 14:43:09.883476 appy-1.0.8/py3/appy/pod/test/results/simpleMinusError.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8606 2017-07-26 14:43:09.879476 appy-1.0.8/py3/appy/pod/test/results/simpleTest.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    13028 2020-04-09 10:11:08.867661 appy-1.0.8/py3/appy/pod/test/results/varDef.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15538 2018-10-26 07:05:35.146425 appy-1.0.8/py3/appy/pod/test/results/withAnImage.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11053 2017-07-26 14:43:09.899476 appy-1.0.8/py3/appy/pod/test/results/xhtmlColgroup.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13969 2019-11-15 15:07:42.104245 appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11785 2019-01-21 13:13:15.135479 appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11178 2019-07-25 12:05:47.030991 appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex3.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8796 2019-07-25 12:05:54.659011 appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex4.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8906 2019-07-25 12:06:02.407031 appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex5.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8469 2018-11-30 10:56:13.107674 appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex6.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8576 2017-07-26 14:43:09.875476 appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex7.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11010 2019-07-25 12:06:10.763054 appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex8.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13568 2017-07-26 14:43:09.867476 appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex9.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17763 2018-10-26 07:05:43.714439 appy-1.0.8/py3/appy/pod/test/results/xhtmlComplexTables.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    13090 2018-11-30 10:56:23.379712 appy-1.0.8/py3/appy/pod/test/results/xhtmlCustomStyles.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11729 2017-07-26 14:43:09.867476 appy-1.0.8/py3/appy/pod/test/results/xhtmlEmpty.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11948 2017-07-26 14:43:09.883476 appy-1.0.8/py3/appy/pod/test/results/xhtmlEntities.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10430 2018-03-21 16:01:33.686184 appy-1.0.8/py3/appy/pod/test/results/xhtmlHtml.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12045 2017-07-26 14:43:09.891476 appy-1.0.8/py3/appy/pod/test/results/xhtmlIgnoreStyles.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13512 2019-07-25 12:06:19.711078 appy-1.0.8/py3/appy/pod/test/results/xhtmlInHeader.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15893 2020-12-18 09:51:30.485914 appy-1.0.8/py3/appy/pod/test/results/xhtmlKeepWithNext.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12143 2019-07-25 12:06:37.775126 appy-1.0.8/py3/appy/pod/test/results/xhtmlListProperties.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    35579 2017-07-26 14:43:09.863476 appy-1.0.8/py3/appy/pod/test/results/xhtmlNominal.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12112 2019-07-25 12:06:48.043154 appy-1.0.8/py3/appy/pod/test/results/xhtmlPIntoLis.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12010 2020-09-10 08:29:51.072435 appy-1.0.8/py3/appy/pod/test/results/xhtmlPIntoTds.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12521 2020-11-12 08:50:11.406453 appy-1.0.8/py3/appy/pod/test/results/xhtmlSpan.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13311 2017-07-26 14:43:09.895476 appy-1.0.8/py3/appy/pod/test/results/xhtmlStylesErrors.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15494 2018-04-18 16:14:08.596004 appy-1.0.8/py3/appy/pod/test/results/xhtmlStylesMapping.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11978 2019-04-05 11:21:06.457405 appy-1.0.8/py3/appy/pod/test/results/xhtmlStylesMapping2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12008 2017-08-24 12:42:14.129789 appy-1.0.8/py3/appy/pod/test/results/xhtmlTableProperties.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10632 2020-11-12 11:30:17.155001 appy-1.0.8/py3/appy/pod/test/results/xhtmlTables.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10944 2017-07-26 14:43:09.867476 appy-1.0.8/py3/appy/pod/test/results/xhtmlTwisted.odt
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.178733 appy-1.0.8/py3/appy/pod/test/templates/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19316 2017-07-26 14:43:09.851476 appy-1.0.8/py3/appy/pod/test/templates/Chart1.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18252 2017-07-26 14:43:09.855476 appy-1.0.8/py3/appy/pod/test/templates/ElseStatements.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6410 2017-07-26 14:43:09.847476 appy-1.0.8/py3/appy/pod/test/templates/ErrorExpression.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10018 2017-07-26 14:43:09.843476 appy-1.0.8/py3/appy/pod/test/templates/ErrorFooter.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6916 2017-07-26 14:43:09.847476 appy-1.0.8/py3/appy/pod/test/templates/ErrorForParsetime.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6832 2017-07-26 14:43:09.855476 appy-1.0.8/py3/appy/pod/test/templates/ErrorForRuntime.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10085 2018-03-28 10:15:57.831696 appy-1.0.8/py3/appy/pod/test/templates/ErrorIf.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9928 2017-07-26 14:43:09.851476 appy-1.0.8/py3/appy/pod/test/templates/FieldExpressions.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7465 2017-07-26 14:43:09.847476 appy-1.0.8/py3/appy/pod/test/templates/FileHandlerImport.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9790 2018-10-26 07:05:57.190461 appy-1.0.8/py3/appy/pod/test/templates/ForCell.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6881 2017-07-26 14:43:09.859476 appy-1.0.8/py3/appy/pod/test/templates/ForCell2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6934 2017-07-26 14:43:09.859476 appy-1.0.8/py3/appy/pod/test/templates/ForCell3.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6952 2017-07-26 14:43:09.859476 appy-1.0.8/py3/appy/pod/test/templates/ForCell4.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6732 2017-07-26 14:43:09.859476 appy-1.0.8/py3/appy/pod/test/templates/ForCell5.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11001 2017-07-26 14:43:09.863476 appy-1.0.8/py3/appy/pod/test/templates/ForCell6.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10009 2017-07-26 14:43:09.863476 appy-1.0.8/py3/appy/pod/test/templates/ForCell7.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6542 2017-07-26 14:43:09.855476 appy-1.0.8/py3/appy/pod/test/templates/ForTable.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6798 2017-07-26 14:43:09.847476 appy-1.0.8/py3/appy/pod/test/templates/ForTableMinus.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7323 2017-07-26 14:43:09.855476 appy-1.0.8/py3/appy/pod/test/templates/ForTableMinus2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7098 2017-07-26 14:43:09.851476 appy-1.0.8/py3/appy/pod/test/templates/ForTableMinusError.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7099 2017-07-26 14:43:09.855476 appy-1.0.8/py3/appy/pod/test/templates/ForTableMinusError2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8774 2019-04-30 19:29:28.745345 appy-1.0.8/py3/appy/pod/test/templates/FromPod.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10215 2017-07-26 14:43:09.855476 appy-1.0.8/py3/appy/pod/test/templates/HeaderFooter.odt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    16196 2020-08-22 17:54:56.295078 appy-1.0.8/py3/appy/pod/test/templates/IfAndFors1.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11041 2017-07-26 14:43:09.855476 appy-1.0.8/py3/appy/pod/test/templates/IfElseErrors.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13788 2021-04-20 14:29:37.852760 appy-1.0.8/py3/appy/pod/test/templates/ImagesImport.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8298 2017-07-26 14:43:09.847476 appy-1.0.8/py3/appy/pod/test/templates/NoPython.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11234 2020-03-30 14:07:09.155077 appy-1.0.8/py3/appy/pod/test/templates/OdsSimple.ods
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8810 2017-07-26 14:43:09.851476 appy-1.0.8/py3/appy/pod/test/templates/OnlyExpressions.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7483 2017-07-26 14:43:09.851476 appy-1.0.8/py3/appy/pod/test/templates/PathImport.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6345 2017-07-26 14:43:09.859476 appy-1.0.8/py3/appy/pod/test/templates/SimpleForEmptyList.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6520 2017-07-26 14:43:09.847476 appy-1.0.8/py3/appy/pod/test/templates/SimpleForFilledList.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7160 2017-07-26 14:43:09.851476 appy-1.0.8/py3/appy/pod/test/templates/SimpleForRow.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9750 2017-07-26 14:43:09.847476 appy-1.0.8/py3/appy/pod/test/templates/SimpleFromTest.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6378 2017-07-26 14:43:09.847476 appy-1.0.8/py3/appy/pod/test/templates/SimpleIfIsFalse.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6378 2017-07-26 14:43:09.843476 appy-1.0.8/py3/appy/pod/test/templates/SimpleIfIsTrue.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8227 2017-07-26 14:43:09.863476 appy-1.0.8/py3/appy/pod/test/templates/SimpleIfIsTrue003.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6567 2017-07-26 14:43:09.847476 appy-1.0.8/py3/appy/pod/test/templates/SimpleMinusError.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8250 2017-07-26 14:43:09.851476 appy-1.0.8/py3/appy/pod/test/templates/SimpleTest.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    20714 2017-10-14 13:08:00.664723 appy-1.0.8/py3/appy/pod/test/templates/TablesToOptimize.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12089 2018-04-18 08:14:26.894172 appy-1.0.8/py3/appy/pod/test/templates/VarStatements.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15044 2017-07-26 14:43:09.843476 appy-1.0.8/py3/appy/pod/test/templates/WithAnImage.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12696 2019-11-15 15:07:52.912282 appy-1.0.8/py3/appy/pod/test/templates/Xhtml.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9156 2017-07-26 14:43:09.843476 appy-1.0.8/py3/appy/pod/test/templates/XhtmlColGroup.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10089 2018-04-18 11:50:50.825343 appy-1.0.8/py3/appy/pod/test/templates/XhtmlComplex2.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8784 2017-07-26 14:43:09.859476 appy-1.0.8/py3/appy/pod/test/templates/XhtmlComplex3.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7730 2017-07-26 14:43:09.859476 appy-1.0.8/py3/appy/pod/test/templates/XhtmlComplex4.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10801 2017-07-26 14:43:09.859476 appy-1.0.8/py3/appy/pod/test/templates/XhtmlComplex8.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    16551 2017-07-26 14:43:09.851476 appy-1.0.8/py3/appy/pod/test/templates/XhtmlComplexTables.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9431 2018-03-21 15:46:22.391030 appy-1.0.8/py3/appy/pod/test/templates/XhtmlHtml.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12421 2017-07-26 14:43:09.839476 appy-1.0.8/py3/appy/pod/test/templates/XhtmlInHeader.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14774 2019-11-15 10:38:42.585725 appy-1.0.8/py3/appy/pod/test/templates/XhtmlKeepWithNext.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    34605 2017-07-26 14:43:09.859476 appy-1.0.8/py3/appy/pod/test/templates/XhtmlNominal.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11284 2017-07-26 14:43:09.843476 appy-1.0.8/py3/appy/pod/test/templates/XhtmlSimple.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10674 2017-07-26 14:43:09.863476 appy-1.0.8/py3/appy/pod/test/templates/XhtmlSpan.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14445 2018-04-18 13:45:22.585631 appy-1.0.8/py3/appy/pod/test/templates/XhtmlStyles.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11839 2017-07-26 14:43:09.855476 appy-1.0.8/py3/appy/pod/test/templates/XhtmlStylesErrors.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7834 2017-07-26 14:43:09.851476 appy-1.0.8/py3/appy/pod/test/templates/XhtmlTables.odt
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8930 2017-07-26 14:43:09.839476 appy-1.0.8/py3/appy/pod/test/templates/XhtmlTwisted.odt
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.178733 appy-1.0.8/py3/appy/pod/xhtml/
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      960 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/xhtml/__init__.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     6687 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/xhtml/parser.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10660 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/xhtml/tags.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    15756 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/xhtml/visitors.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    65316 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/pod/xhtml2odt.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.178733 appy-1.0.8/py3/appy/px/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18981 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/px/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7465 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/px/parser.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.178733 appy-1.0.8/py3/appy/server/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    26881 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15274 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/backup.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10796 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/context.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4185 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/cookie.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5657 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/error.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    25826 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/guard.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    24311 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/handler.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1856 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/languages.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22526 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/ldap.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19055 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/pool.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7195 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/request.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13770 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/response.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    20887 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/scheduler.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    21472 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/sso.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    13325 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/static.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    16746 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/server/traversal.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.178733 appy-1.0.8/py3/appy/test/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      777 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/test/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15249 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/test/integration.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3956 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/test/monitoring.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14169 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/test/performance.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.178733 appy-1.0.8/py3/appy/tr/
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     3477 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/tr/__init__.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.178733 appy-1.0.8/py3/appy/tr/po/
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    35809 2021-07-02 13:01:26.529389 appy-1.0.8/py3/appy/tr/po/Appy.pot
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    16361 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/tr/po/__init__.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    36190 2021-07-02 13:01:56.553355 appy-1.0.8/py3/appy/tr/po/ar.po
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    38207 2021-07-02 13:02:32.553315 appy-1.0.8/py3/appy/tr/po/de.po
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    49235 2021-07-02 13:02:32.561315 appy-1.0.8/py3/appy/tr/po/en.po
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    37372 2021-07-02 13:02:32.569315 appy-1.0.8/py3/appy/tr/po/es.po
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    51846 2021-07-02 13:02:21.449327 appy-1.0.8/py3/appy/tr/po/fr.po
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    37394 2021-07-02 13:02:32.577315 appy-1.0.8/py3/appy/tr/po/it.po
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    40833 2021-07-02 13:02:32.581315 appy-1.0.8/py3/appy/tr/po/nl.po
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    20618 2021-07-05 10:28:19.858732 appy-1.0.8/py3/appy/tr/updater.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.182733 appy-1.0.8/py3/appy/ui/
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    45218 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/__init__.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8952 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/account.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     4543 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/criteria.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    21023 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/css.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5939 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/globals.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2741 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/iframe.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4013 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/includer.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2001 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/js.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3611 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/language.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    26057 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/layout.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     4769 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/message.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17183 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/navigate.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5996 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/portlet.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.182733 appy-1.0.8/py3/appy/ui/static/
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1431 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/action.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      963 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/add.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      349 2017-12-03 10:34:35.198912 appy-1.0.8/py3/appy/ui/static/addAbove.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      356 2017-12-03 10:34:31.814888 appy-1.0.8/py3/appy/ui/static/addAboveFrom.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      346 2017-12-02 13:05:25.147842 appy-1.0.8/py3/appy/ui/static/addBelow.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      238 2016-10-11 18:35:14.181452 appy-1.0.8/py3/appy/ui/static/addFrom.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      209 2016-10-11 18:35:14.185452 appy-1.0.8/py3/appy/ui/static/angled.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7185 2020-05-21 07:59:58.067896 appy-1.0.8/py3/appy/ui/static/appleicon.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    14298 2021-07-02 13:05:26.593588 appy-1.0.8/py3/appy/ui/static/appy.css
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)    55077 2021-07-02 12:45:12.526545 appy-1.0.8/py3/appy/ui/static/appy.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      266 2019-10-12 15:36:04.076676 appy-1.0.8/py3/appy/ui/static/appyrtl.css
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      393 2020-12-02 12:55:54.083870 appy-1.0.8/py3/appy/ui/static/arrow.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      484 2020-12-02 12:56:13.691835 appy-1.0.8/py3/appy/ui/static/arrows.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      482 2020-12-02 13:29:57.086885 appy-1.0.8/py3/appy/ui/static/arrowsA.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1048 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/asc.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      821 2016-10-11 18:35:14.181452 appy-1.0.8/py3/appy/ui/static/back.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      518 2020-10-19 13:10:30.352504 appy-1.0.8/py3/appy/ui/static/baseBG.jpg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      735 2020-10-07 12:23:43.251580 appy-1.0.8/py3/appy/ui/static/burger.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9878 2020-05-23 09:16:10.586025 appy-1.0.8/py3/appy/ui/static/calendar.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1958 2020-05-25 06:11:43.916825 appy-1.0.8/py3/appy/ui/static/calendar.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     3450 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/cancel.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      255 2016-10-11 18:35:14.189452 appy-1.0.8/py3/appy/ui/static/changes.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      250 2016-10-11 18:35:14.185452 appy-1.0.8/py3/appy/ui/static/changesNo.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      926 2020-05-03 09:12:26.925560 appy-1.0.8/py3/appy/ui/static/checkAll.svg
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.186733 appy-1.0.8/py3/appy/ui/static/ckeditor/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      289 2016-10-11 18:35:14.189452 appy-1.0.8/py3/appy/ui/static/ckeditor/Readme
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1471 2020-06-07 09:46:31.266478 appy-1.0.8/py3/appy/ui/static/ckeditor/config.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2574 2020-06-07 09:47:03.614665 appy-1.0.8/py3/appy/ui/static/ckeditor/contents.css
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      365 2016-12-20 19:09:41.746375 appy-1.0.8/py3/appy/ui/static/ckeditor/styles.js
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      656 2020-05-25 07:37:30.287932 appy-1.0.8/py3/appy/ui/static/close.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      159 2017-01-11 15:15:14.258984 appy-1.0.8/py3/appy/ui/static/collapse.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1052 2020-10-07 12:22:36.658985 appy-1.0.8/py3/appy/ui/static/config.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      244 2016-10-11 18:35:14.185452 appy-1.0.8/py3/appy/ui/static/current.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2391 2021-05-01 08:21:13.319728 appy-1.0.8/py3/appy/ui/static/custom.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1277 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/delete.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1650 2020-12-02 13:34:29.666668 appy-1.0.8/py3/appy/ui/static/deleteMany.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1102 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/deleteS.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      248 2016-10-11 18:35:14.193452 appy-1.0.8/py3/appy/ui/static/done.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      888 2020-12-02 13:27:34.158976 appy-1.0.8/py3/appy/ui/static/download.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      971 2020-11-29 18:01:53.222345 appy-1.0.8/py3/appy/ui/static/edit.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      971 2020-11-29 18:01:53.222345 appy-1.0.8/py3/appy/ui/static/editPage.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      760 2016-10-11 18:35:14.177452 appy-1.0.8/py3/appy/ui/static/email.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      163 2017-01-11 15:15:40.939234 appy-1.0.8/py3/appy/ui/static/expand.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      685 2016-10-11 18:35:14.193452 appy-1.0.8/py3/appy/ui/static/external.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4286 2016-10-11 18:35:13.669445 appy-1.0.8/py3/appy/ui/static/favicon.ico
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      350 2016-10-11 18:35:13.673445 appy-1.0.8/py3/appy/ui/static/freeze.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      177 2016-10-11 18:35:13.673445 appy-1.0.8/py3/appy/ui/static/frozen.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1517 2020-05-01 12:54:01.725035 appy-1.0.8/py3/appy/ui/static/funnel.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      235 2016-10-11 18:35:13.669445 appy-1.0.8/py3/appy/ui/static/gotoNumber.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1130 2021-05-01 07:08:58.405262 appy-1.0.8/py3/appy/ui/static/grid.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1939 2020-06-30 09:36:30.869973 appy-1.0.8/py3/appy/ui/static/groups.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1686 2020-10-07 15:26:15.420097 appy-1.0.8/py3/appy/ui/static/headerBG.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1521 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/help.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1547 2020-05-15 05:19:57.938326 appy-1.0.8/py3/appy/ui/static/history.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      638 2020-10-07 12:23:17.711351 appy-1.0.8/py3/appy/ui/static/home.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)   809708 2020-10-07 15:29:39.334362 appy-1.0.8/py3/appy/ui/static/homeBG.jpg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1686 2020-10-07 15:26:15.420097 appy-1.0.8/py3/appy/ui/static/homeLogo.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      143 2019-04-16 17:17:42.056992 appy-1.0.8/py3/appy/ui/static/icon_blank.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      281 2019-04-13 17:14:40.738721 appy-1.0.8/py3/appy/ui/static/icon_bold.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      140 2019-04-16 17:17:48.161005 appy-1.0.8/py3/appy/ui/static/icon_dash.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      396 2019-04-16 17:17:55.733023 appy-1.0.8/py3/appy/ui/static/icon_highlight.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      279 2019-04-13 17:14:53.938858 appy-1.0.8/py3/appy/ui/static/icon_italic.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      343 2019-04-16 17:18:05.225044 appy-1.0.8/py3/appy/ui/static/icon_lengthen.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2012 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/internals.svg
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.186733 appy-1.0.8/py3/appy/ui/static/jscalendar/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4830 2016-10-11 18:35:13.677445 appy-1.0.8/py3/appy/ui/static/jscalendar/calendar-blue.css
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5057 2016-10-11 18:35:13.945449 appy-1.0.8/py3/appy/ui/static/jscalendar/calendar-setup.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    34353 2016-10-11 18:35:13.673445 appy-1.0.8/py3/appy/ui/static/jscalendar/calendar.js
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.186733 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1011 2016-10-11 18:35:13.933449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-af.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2135 2016-10-11 18:35:13.933449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-al.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3723 2016-10-11 18:35:13.941449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-bg.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3525 2016-10-11 18:35:13.945449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-big5-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3290 2016-10-11 18:35:13.941449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-big5.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3706 2016-10-11 18:35:13.937449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-br.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3597 2016-10-11 18:35:13.941449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-ca.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2940 2016-10-11 18:35:13.941449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-cs-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2810 2016-10-11 18:35:13.933449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-cs-win.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3500 2016-10-11 18:35:13.941449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-da.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3863 2016-10-11 18:35:13.941449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-de.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1143 2016-10-11 18:35:13.945449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-du.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3241 2016-10-11 18:35:13.933449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-el.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3600 2016-10-11 18:35:13.933449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-en.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3917 2016-10-11 18:35:13.941449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-es.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3827 2016-10-11 18:35:13.945449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-eu.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2782 2016-10-11 18:35:13.941449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-fi.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4071 2016-10-11 18:35:13.937449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-fr.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3919 2016-10-11 18:35:13.929449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-he-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1553 2016-10-11 18:35:13.933449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-hr-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3088 2016-10-11 18:35:13.937449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-hr.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3603 2016-10-11 18:35:13.945449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-hu.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3633 2016-10-11 18:35:13.937449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-it.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      913 2016-10-11 18:35:13.937449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-jp.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3568 2016-10-11 18:35:13.941449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-ko-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3256 2016-10-11 18:35:13.945449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-ko.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3432 2016-10-11 18:35:13.937449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-lt-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3400 2016-10-11 18:35:13.937449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-lt.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3603 2016-10-11 18:35:13.937449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-lv.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2234 2016-10-11 18:35:13.937449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-nl.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3178 2016-10-11 18:35:13.945449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-no.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2635 2016-10-11 18:35:13.933449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-pl-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2414 2016-10-11 18:35:13.937449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-pl.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3526 2016-10-11 18:35:13.937449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-pt.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2058 2016-10-11 18:35:13.929449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-ro.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3985 2016-10-11 18:35:13.929449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-ru-UTF.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4357 2016-10-11 18:35:13.933449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-ru.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3643 2016-10-11 18:35:13.941449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-ru_win_.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2684 2016-10-11 18:35:13.945449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-si.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2661 2016-10-11 18:35:13.945449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-sk.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3015 2016-10-11 18:35:13.937449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-sp.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2759 2016-10-11 18:35:13.945449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-sr-utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5492 2016-10-11 18:35:13.941449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-sr.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3973 2016-10-11 18:35:13.941449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-sv.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1736 2016-10-11 18:35:13.941449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-tr.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3082 2016-10-11 18:35:13.937449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-zh.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4751 2016-10-11 18:35:13.941449 appy-1.0.8/py3/appy/ui/static/jscalendar/lang/cn_utf8.js
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       68 2016-10-11 18:35:13.945449 appy-1.0.8/py3/appy/ui/static/jscalendar/menuarrow.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       49 2016-10-11 18:35:13.677445 appy-1.0.8/py3/appy/ui/static/jscalendar/menuarrow2.gif
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.150733 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.186733 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/aqua/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       89 2016-10-11 18:35:13.677445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/aqua/active-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       85 2016-10-11 18:35:13.677445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/aqua/dark-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       89 2016-10-11 18:35:13.677445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/aqua/hover-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       49 2016-10-11 18:35:13.677445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/aqua/menuarrow.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      110 2016-10-11 18:35:13.677445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/aqua/normal-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      110 2016-10-11 18:35:13.677445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/aqua/rowhover-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      116 2016-10-11 18:35:13.677445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/aqua/status-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5576 2016-10-11 18:35:13.677445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/aqua/theme.css
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      116 2016-10-11 18:35:13.677445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/aqua/title-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1122 2016-10-11 18:35:13.677445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/aqua/today-bg.gif
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.186733 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/tiger/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/tiger/active-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/tiger/dark-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/tiger/hover-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       49 2016-10-11 18:35:13.681445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/tiger/menuarrow.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/tiger/normal-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/tiger/rowhover-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      149 2016-10-11 18:35:13.685446 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/tiger/status-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5772 2016-10-11 18:35:13.681445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/tiger/theme.css
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      149 2016-10-11 18:35:13.681445 appy-1.0.8/py3/appy/ui/static/jscalendar/skins/tiger/title-bg.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       51 2016-10-11 18:35:14.193452 appy-1.0.8/py3/appy/ui/static/li.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      234 2016-10-11 18:35:13.665445 appy-1.0.8/py3/appy/ui/static/link.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1385 2020-05-03 09:11:58.405420 appy-1.0.8/py3/appy/ui/static/linkMany.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.669445 appy-1.0.8/py3/appy/ui/static/lirtl.gif
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1428 2021-05-01 07:02:35.257410 appy-1.0.8/py3/appy/ui/static/list.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10766 2016-10-11 18:35:14.185452 appy-1.0.8/py3/appy/ui/static/loading_big.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1516 2016-10-11 18:35:14.181452 appy-1.0.8/py3/appy/ui/static/loading_button.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3429 2016-10-11 18:35:13.673445 appy-1.0.8/py3/appy/ui/static/loading_icon.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1281 2016-10-11 18:35:13.665445 appy-1.0.8/py3/appy/ui/static/loading_link.gif
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1076 2020-05-04 11:36:14.632703 appy-1.0.8/py3/appy/ui/static/locked.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1420 2020-10-07 12:18:31.232851 appy-1.0.8/py3/appy/ui/static/login.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     4179 2019-10-13 13:08:38.809234 appy-1.0.8/py3/appy/ui/static/loginLogo.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1195 2020-10-07 12:20:12.697721 appy-1.0.8/py3/appy/ui/static/logout.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      281 2019-04-25 08:34:17.501090 appy-1.0.8/py3/appy/ui/static/more.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      233 2016-10-11 18:35:14.189452 appy-1.0.8/py3/appy/ui/static/move.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      114 2016-10-11 18:35:14.185452 appy-1.0.8/py3/appy/ui/static/object.gif
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1907 2020-04-30 09:28:48.404131 appy-1.0.8/py3/appy/ui/static/page.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1406 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/pagePages.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3678 2020-05-01 12:09:02.985098 appy-1.0.8/py3/appy/ui/static/pagePassword.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1237 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/pageProfile.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1637 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/pageTranslations.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1899 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/pageUsers.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      665 2017-04-03 19:23:17.060212 appy-1.0.8/py3/appy/ui/static/paperclip.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1972 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/password.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2011 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/pay.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      251 2016-10-11 18:35:14.177452 appy-1.0.8/py3/appy/ui/static/plus.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      518 2020-10-19 13:10:30.352504 appy-1.0.8/py3/appy/ui/static/popupBG.jpg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      963 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/portletAdd.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     4179 2019-10-13 13:08:38.809234 appy-1.0.8/py3/appy/ui/static/portletLogo.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      607 2016-10-11 18:35:14.185452 appy-1.0.8/py3/appy/ui/static/pwd.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1315 2021-05-16 20:28:31.050907 appy-1.0.8/py3/appy/ui/static/python.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      834 2019-09-05 20:18:39.232602 appy-1.0.8/py3/appy/ui/static/refresh.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      632 2016-10-11 18:35:13.673445 appy-1.0.8/py3/appy/ui/static/reindex.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      168 2018-09-27 14:01:52.821020 appy-1.0.8/py3/appy/ui/static/repeated.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      179 2018-09-27 14:03:43.909542 appy-1.0.8/py3/appy/ui/static/repeated_last.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       86 2021-03-29 11:33:47.143711 appy-1.0.8/py3/appy/ui/static/robots.txt
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1346 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/save.svg
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1174 2020-04-28 18:31:30.000000 appy-1.0.8/py3/appy/ui/static/search.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      165 2016-12-20 19:09:41.746375 appy-1.0.8/py3/appy/ui/static/select.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      211 2016-10-11 18:35:14.193452 appy-1.0.8/py3/appy/ui/static/to.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      442 2016-10-11 18:35:14.177452 appy-1.0.8/py3/appy/ui/static/unfreeze.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      697 2020-05-04 07:42:51.901919 appy-1.0.8/py3/appy/ui/static/unlink.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1371 2020-05-04 07:42:49.773909 appy-1.0.8/py3/appy/ui/static/unlinkMany.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      243 2016-10-11 18:35:14.185452 appy-1.0.8/py3/appy/ui/static/unlinkManyUp.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      234 2016-10-11 18:35:13.673445 appy-1.0.8/py3/appy/ui/static/unlinkUp.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      391 2016-10-11 18:35:13.669445 appy-1.0.8/py3/appy/ui/static/unselect.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      421 2016-10-11 18:35:13.669445 appy-1.0.8/py3/appy/ui/static/upload.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      620 2017-04-03 19:27:08.317931 appy-1.0.8/py3/appy/ui/static/url.png
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)      789 2020-10-07 12:21:22.946334 appy-1.0.8/py3/appy/ui/static/user.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      208 2016-10-11 18:35:14.185452 appy-1.0.8/py3/appy/ui/static/validate.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      314 2016-10-11 18:35:14.181452 appy-1.0.8/py3/appy/ui/static/warning.png
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      854 2020-05-03 10:44:35.869767 appy-1.0.8/py3/appy/ui/static/warning.svg
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12437 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/template.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7763 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/title.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9317 2021-07-05 10:28:19.862732 appy-1.0.8/py3/appy/ui/validate.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.186733 appy-1.0.8/py3/appy/utils/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15255 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/utils/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1775 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/utils/analytics.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    25012 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/utils/client.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8110 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/utils/dates.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    33353 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/utils/diff.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3847 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/utils/inject.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8204 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/utils/loc.py
--rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8512 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/utils/mail.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8698 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/utils/path.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12890 2021-07-05 10:28:19.850732 appy-1.0.8/py3/appy/utils/pretty.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17986 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/utils/string.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18492 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/utils/tables.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2580 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/utils/url.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7717 2021-07-05 10:28:19.846732 appy-1.0.8/py3/appy/utils/zip.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       52 2021-07-05 10:28:19.866732 appy-1.0.8/py3/appy/version.py
-drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-07-05 10:28:20.186733 appy-1.0.8/py3/appy/xml/
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8030 2021-07-05 10:28:19.866732 appy-1.0.8/py3/appy/xml/__init__.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7000 2021-07-05 10:28:19.866732 appy-1.0.8/py3/appy/xml/cleaner.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6923 2021-07-05 10:28:19.866732 appy-1.0.8/py3/appy/xml/diff.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4622 2021-07-05 10:28:19.866732 appy-1.0.8/py3/appy/xml/escape.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3692 2021-07-05 10:28:19.866732 appy-1.0.8/py3/appy/xml/extractor.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13356 2021-07-05 10:28:19.866732 appy-1.0.8/py3/appy/xml/marshaller.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14646 2021-07-05 10:28:19.866732 appy-1.0.8/py3/appy/xml/unmarshaller.py
--rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      903 2021-07-05 10:28:19.866732 appy-1.0.8/setup.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.797118 appy-1.0.9/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      269 2021-10-26 12:39:34.797118 appy-1.0.9/PKG-INFO
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      345 2021-10-26 12:39:34.433114 appy-1.0.9/README
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.745117 appy-1.0.9/py2/
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.749117 appy-1.0.9/py2/appy/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7263 2021-10-26 12:39:29.073065 appy-1.0.9/py2/appy/__init__.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.749117 appy-1.0.9/py2/appy/bin/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3657 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/asksap.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    21952 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/backup.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2051 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/checkldap.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     3317 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/checklo.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1011 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/clean.py
+-rwxrwxr-x   0 gdy999    (1000) gdy999    (1000)     1088 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/createdebrepo.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8473 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/eggify.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3864 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/generate.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3885 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/job.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17560 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/new.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1577 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/odfclean.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11719 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/odfgrep.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3045 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/odfwalk.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4393 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/restore.py
+-rwxrwxr-x   0 gdy999    (1000) gdy999    (1000)      284 2020-03-04 05:39:19.104383 appy-1.0.9/py2/appy/bin/startlo
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1753 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/zip.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1027 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/bin/zopectl.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.753117 appy-1.0.9/py2/appy/fields/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    80716 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    26981 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/action.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8530 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/boolean.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)   115346 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/fields/calendar.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2714 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/color.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10535 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/computed.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2639 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/custom.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18231 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/date.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9883 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/dict.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    31099 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/file.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3674 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/float.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22449 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/fields/group.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10324 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/fields/hour.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2102 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/info.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6916 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/integer.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17822 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/fields/list.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13292 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/multilingual.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4104 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/fields/page.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9576 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/phase.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    52905 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/fields/pod.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)   115891 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/fields/ref.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    16210 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/rich.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    60506 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/search.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    21304 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/select.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    59433 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/fields/string.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5774 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/fields/switch.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    35275 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/fields/text.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2402 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/translations.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    32939 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/fields/workflow.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.753117 appy-1.0.9/py2/appy/gen/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15989 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8303 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/authenticate.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    24070 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/descriptors.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    37751 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/gen/generator.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6960 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/indexer.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    21566 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/installer.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    20833 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/layout.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6682 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/mail.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3909 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/gen/migrator.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.753117 appy-1.0.9/py2/appy/gen/mixins/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3448 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/mixins/TestMixin.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    78978 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/mixins/ToolMixin.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)   104147 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/mixins/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19000 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/model.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3171 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/monitoring.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18521 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/gen/navigate.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    14178 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/po.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.753117 appy-1.0.9/py2/appy/gen/templates/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1218 2016-10-11 18:35:13.241440 appy-1.0.9/py2/appy/gen/templates/Class.pyt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11575 2020-04-13 13:43:13.403474 appy-1.0.9/py2/appy/gen/templates/Page.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1464 2016-10-11 18:35:13.237439 appy-1.0.9/py2/appy/gen/templates/__init__.pyt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1424 2016-10-11 18:35:13.241440 appy-1.0.9/py2/appy/gen/templates/config.pyt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      967 2016-10-11 18:35:13.237439 appy-1.0.9/py2/appy/gen/templates/testAll.pyt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1019 2018-07-30 10:01:33.277339 appy-1.0.9/py2/appy/gen/templates/wrappers.pyt
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.753117 appy-1.0.9/py2/appy/gen/tr/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    21051 2020-12-08 12:33:01.908456 appy-1.0.9/py2/appy/gen/tr/Appy.pot
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    21422 2020-12-08 12:33:01.912456 appy-1.0.9/py2/appy/gen/tr/ar.po
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    23517 2020-12-08 12:33:01.916456 appy-1.0.9/py2/appy/gen/tr/de.po
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    28163 2020-12-08 12:33:01.916456 appy-1.0.9/py2/appy/gen/tr/en.po
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22603 2020-12-08 12:33:01.920456 appy-1.0.9/py2/appy/gen/tr/es.po
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    29826 2020-12-08 12:33:00.716461 appy-1.0.9/py2/appy/gen/tr/fr.po
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22639 2020-12-08 12:33:01.928456 appy-1.0.9/py2/appy/gen/tr/it.po
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    25781 2021-04-19 09:41:13.951888 appy-1.0.9/py2/appy/gen/tr/nl.po
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.757117 appy-1.0.9/py2/appy/gen/ui/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      566 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/action.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      240 2016-10-11 18:35:13.669445 appy-1.0.9/py2/appy/gen/ui/add.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      349 2017-12-03 10:34:35.198912 appy-1.0.9/py2/appy/gen/ui/addAbove.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      356 2017-12-03 10:34:31.814888 appy-1.0.9/py2/appy/gen/ui/addAboveFrom.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      346 2017-12-02 13:05:25.147843 appy-1.0.9/py2/appy/gen/ui/addBelow.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      238 2016-10-11 18:35:14.181452 appy-1.0.9/py2/appy/gen/ui/addFrom.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      209 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/angled.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    15606 2021-09-16 12:22:55.912590 appy-1.0.9/py2/appy/gen/ui/appy.css
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    70727 2021-09-16 18:59:40.181576 appy-1.0.9/py2/appy/gen/ui/appy.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      317 2016-10-11 18:35:14.181452 appy-1.0.9/py2/appy/gen/ui/appyrtl.css
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      234 2016-10-11 18:35:14.193452 appy-1.0.9/py2/appy/gen/ui/arrowDown.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      218 2016-10-11 18:35:14.181452 appy-1.0.9/py2/appy/gen/ui/arrowLeft.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      229 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/arrowRight.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      234 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/arrowUp.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      242 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/arrowsDown.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      236 2016-10-11 18:35:14.177452 appy-1.0.9/py2/appy/gen/ui/arrowsLeft.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      235 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/arrowsRight.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      241 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/arrowsUp.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      821 2016-10-11 18:35:14.181452 appy-1.0.9/py2/appy/gen/ui/back.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    62923 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/banner.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    63085 2016-10-11 18:35:13.669445 appy-1.0.9/py2/appy/gen/ui/bannerrtl.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      953 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/calendar.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9852 2017-12-20 08:06:29.446130 appy-1.0.9/py2/appy/gen/ui/calendar.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      272 2016-10-11 18:35:14.193452 appy-1.0.9/py2/appy/gen/ui/cancel.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      255 2016-10-11 18:35:14.189453 appy-1.0.9/py2/appy/gen/ui/changes.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      250 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/changesNo.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      235 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/checkall.png
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.757117 appy-1.0.9/py2/appy/gen/ui/ckeditor/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      289 2016-10-11 18:35:14.189453 appy-1.0.9/py2/appy/gen/ui/ckeditor/Readme
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1471 2019-02-26 14:12:27.837745 appy-1.0.9/py2/appy/gen/ui/ckeditor/config.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1855 2016-10-11 18:35:14.189453 appy-1.0.9/py2/appy/gen/ui/ckeditor/contents.css
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      365 2016-12-20 19:09:41.746375 appy-1.0.9/py2/appy/gen/ui/ckeditor/styles.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      219 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/close.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      159 2017-01-11 15:15:14.258984 appy-1.0.9/py2/appy/gen/ui/collapse.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      883 2016-10-11 18:35:14.181452 appy-1.0.9/py2/appy/gen/ui/config.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      244 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/current.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      231 2016-10-11 18:35:14.181452 appy-1.0.9/py2/appy/gen/ui/delete.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      259 2016-10-11 18:35:14.177452 appy-1.0.9/py2/appy/gen/ui/deleteMany.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      475 2019-12-03 14:05:11.171558 appy-1.0.9/py2/appy/gen/ui/doc.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      514 2016-10-11 18:35:14.193452 appy-1.0.9/py2/appy/gen/ui/docFrozen.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      544 2019-12-03 14:05:00.663564 appy-1.0.9/py2/appy/gen/ui/docx.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      540 2019-12-03 14:07:37.223567 appy-1.0.9/py2/appy/gen/ui/docxFrozen.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      248 2016-10-11 18:35:14.193452 appy-1.0.9/py2/appy/gen/ui/done.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      424 2016-10-11 18:35:14.193452 appy-1.0.9/py2/appy/gen/ui/edit.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      760 2016-10-11 18:35:14.177452 appy-1.0.9/py2/appy/gen/ui/email.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      163 2017-01-11 15:15:40.939234 appy-1.0.9/py2/appy/gen/ui/expand.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      685 2016-10-11 18:35:14.193452 appy-1.0.9/py2/appy/gen/ui/external.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      657 2016-10-11 18:35:14.181452 appy-1.0.9/py2/appy/gen/ui/fake.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       62 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/fakeTransition.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4286 2016-10-11 18:35:13.669445 appy-1.0.9/py2/appy/gen/ui/favicon.ico
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      903 2016-10-11 18:35:13.665445 appy-1.0.9/py2/appy/gen/ui/folder.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      350 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/freeze.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      177 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/frozen.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      719 2016-10-11 18:35:14.177452 appy-1.0.9/py2/appy/gen/ui/funnel.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      235 2016-10-11 18:35:13.669445 appy-1.0.9/py2/appy/gen/ui/gotoNumber.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      222 2020-03-27 14:21:32.474700 appy-1.0.9/py2/appy/gen/ui/gotoSource.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      591 2016-10-11 18:35:14.177452 appy-1.0.9/py2/appy/gen/ui/help.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      240 2017-01-12 08:32:32.441065 appy-1.0.9/py2/appy/gen/ui/hide.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      143 2019-04-16 12:16:08.856283 appy-1.0.9/py2/appy/gen/ui/icon_blank.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      281 2019-04-11 18:56:00.291958 appy-1.0.9/py2/appy/gen/ui/icon_bold.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      140 2019-04-16 12:16:46.960454 appy-1.0.9/py2/appy/gen/ui/icon_dash.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      396 2019-04-16 10:26:15.605046 appy-1.0.9/py2/appy/gen/ui/icon_highlight.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      279 2019-04-12 05:54:24.481362 appy-1.0.9/py2/appy/gen/ui/icon_italic.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      343 2019-04-16 12:21:21.257668 appy-1.0.9/py2/appy/gen/ui/icon_lengthen.png
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.757117 appy-1.0.9/py2/appy/gen/ui/jscalendar/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4830 2016-10-11 18:35:13.677446 appy-1.0.9/py2/appy/gen/ui/jscalendar/calendar-blue.css
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5057 2016-10-11 18:35:13.945449 appy-1.0.9/py2/appy/gen/ui/jscalendar/calendar-setup.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    34353 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/jscalendar/calendar.js
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.761117 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1011 2016-10-11 18:35:13.933449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-af.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2135 2016-10-11 18:35:13.933449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-al.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3723 2016-10-11 18:35:13.941449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-bg.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3525 2016-10-11 18:35:13.945449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-big5-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3290 2016-10-11 18:35:13.941449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-big5.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3706 2016-10-11 18:35:13.937449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-br.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3597 2016-10-11 18:35:13.941449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-ca.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2940 2016-10-11 18:35:13.941449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-cs-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2810 2016-10-11 18:35:13.933449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-cs-win.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3500 2016-10-11 18:35:13.941449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-da.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3863 2016-10-11 18:35:13.941449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-de.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1143 2016-10-11 18:35:13.945449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-du.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3241 2016-10-11 18:35:13.933449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-el.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3600 2016-10-11 18:35:13.933449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-en.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3917 2016-10-11 18:35:13.941449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-es.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3827 2016-10-11 18:35:13.945449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-eu.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2782 2016-10-11 18:35:13.941449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-fi.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4071 2016-10-11 18:35:13.937449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-fr.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3919 2016-10-11 18:35:13.929449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-he-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1553 2016-10-11 18:35:13.933449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-hr-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3088 2016-10-11 18:35:13.937449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-hr.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3603 2016-10-11 18:35:13.945449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-hu.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3633 2016-10-11 18:35:13.937449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-it.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      913 2016-10-11 18:35:13.937449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-jp.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3568 2016-10-11 18:35:13.941449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-ko-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3256 2016-10-11 18:35:13.945449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-ko.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3432 2016-10-11 18:35:13.937449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-lt-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3400 2016-10-11 18:35:13.937449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-lt.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3603 2016-10-11 18:35:13.937449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-lv.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2234 2016-10-11 18:35:13.937449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-nl.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3178 2016-10-11 18:35:13.945449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-no.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2635 2016-10-11 18:35:13.933449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-pl-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2414 2016-10-11 18:35:13.937449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-pl.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3526 2016-10-11 18:35:13.937449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-pt.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2058 2016-10-11 18:35:13.929449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-ro.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3985 2016-10-11 18:35:13.929449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-ru-UTF.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4357 2016-10-11 18:35:13.933449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-ru.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3643 2016-10-11 18:35:13.941449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-ru_win_.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2684 2016-10-11 18:35:13.945449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-si.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2661 2016-10-11 18:35:13.945449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-sk.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3015 2016-10-11 18:35:13.937449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-sp.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2759 2016-10-11 18:35:13.945449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-sr-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5492 2016-10-11 18:35:13.941449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-sr.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3973 2016-10-11 18:35:13.941449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-sv.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1736 2016-10-11 18:35:13.941449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-tr.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3082 2016-10-11 18:35:13.937449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-zh.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4751 2016-10-11 18:35:13.941449 appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/cn_utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       68 2016-10-11 18:35:13.945449 appy-1.0.9/py2/appy/gen/ui/jscalendar/menuarrow.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       49 2016-10-11 18:35:13.677446 appy-1.0.9/py2/appy/gen/ui/jscalendar/menuarrow2.gif
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.749117 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.761117 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/aqua/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       89 2016-10-11 18:35:13.677446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/aqua/active-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       85 2016-10-11 18:35:13.677446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/aqua/dark-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       89 2016-10-11 18:35:13.677446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/aqua/hover-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       49 2016-10-11 18:35:13.677446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/aqua/menuarrow.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      110 2016-10-11 18:35:13.677446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/aqua/normal-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      110 2016-10-11 18:35:13.677446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/aqua/rowhover-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      116 2016-10-11 18:35:13.677446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/aqua/status-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5576 2016-10-11 18:35:13.677446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/aqua/theme.css
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      116 2016-10-11 18:35:13.677446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/aqua/title-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1122 2016-10-11 18:35:13.677446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/aqua/today-bg.gif
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.761117 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/tiger/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/tiger/active-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/tiger/dark-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/tiger/hover-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       49 2016-10-11 18:35:13.681446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/tiger/menuarrow.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/tiger/normal-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/tiger/rowhover-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      149 2016-10-11 18:35:13.685446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/tiger/status-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5772 2016-10-11 18:35:13.681446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/tiger/theme.css
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      149 2016-10-11 18:35:13.681446 appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/tiger/title-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       51 2016-10-11 18:35:14.193452 appy-1.0.9/py2/appy/gen/ui/li.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      234 2016-10-11 18:35:13.665445 appy-1.0.9/py2/appy/gen/ui/link.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      288 2016-10-11 18:35:14.193452 appy-1.0.9/py2/appy/gen/ui/linkMany.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.669445 appy-1.0.9/py2/appy/gen/ui/lirtl.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1281 2016-10-11 18:35:13.665445 appy-1.0.9/py2/appy/gen/ui/loading.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10766 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/loadingBig.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1516 2016-10-11 18:35:14.181452 appy-1.0.9/py2/appy/gen/ui/loadingBtn.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3429 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/loadingPod.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      648 2016-10-11 18:35:13.665445 appy-1.0.9/py2/appy/gen/ui/locked.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1634 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/lockedBig.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      173 2016-10-11 18:35:13.669445 appy-1.0.9/py2/appy/gen/ui/login.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5251 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/logo.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      647 2019-04-13 09:53:33.530200 appy-1.0.9/py2/appy/gen/ui/logout.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      281 2019-04-25 08:27:36.922217 appy-1.0.9/py2/appy/gen/ui/more.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      233 2016-10-11 18:35:14.189453 appy-1.0.9/py2/appy/gen/ui/move.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      229 2016-10-11 18:35:13.669445 appy-1.0.9/py2/appy/gen/ui/next.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      114 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/object.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      663 2016-10-11 18:35:14.177452 appy-1.0.9/py2/appy/gen/ui/ods.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      668 2016-10-11 18:35:14.189453 appy-1.0.9/py2/appy/gen/ui/odsFrozen.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      470 2016-10-11 18:35:14.177452 appy-1.0.9/py2/appy/gen/ui/odt.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      493 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/odtFrozen.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2403 2016-10-11 18:35:14.177452 appy-1.0.9/py2/appy/gen/ui/ogone.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      665 2017-04-03 19:23:17.060212 appy-1.0.9/py2/appy/gen/ui/paperclip.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      432 2016-10-11 18:35:14.189453 appy-1.0.9/py2/appy/gen/ui/pdf.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      485 2016-10-11 18:35:13.669445 appy-1.0.9/py2/appy/gen/ui/pdfFrozen.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      251 2016-10-11 18:35:14.177452 appy-1.0.9/py2/appy/gen/ui/plus.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      225 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/previous.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      607 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/pwd.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      834 2019-09-05 19:39:24.843870 appy-1.0.9/py2/appy/gen/ui/refresh.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      632 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/reindex.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      168 2018-09-27 14:01:52.821020 appy-1.0.9/py2/appy/gen/ui/repeated.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      179 2018-09-27 14:03:43.909542 appy-1.0.9/py2/appy/gen/ui/repeated_last.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       53 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/required.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      513 2016-10-11 18:35:13.669445 appy-1.0.9/py2/appy/gen/ui/save.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      297 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/search.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      240 2017-01-12 08:32:59.861142 appy-1.0.9/py2/appy/gen/ui/show.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      367 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/sortAsc.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      316 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/sortDesc.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      165 2016-12-20 19:09:41.746375 appy-1.0.9/py2/appy/gen/ui/sortDown.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      165 2016-12-20 19:09:41.746375 appy-1.0.9/py2/appy/gen/ui/sortUp.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       43 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/space.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      211 2016-10-11 18:35:14.193452 appy-1.0.9/py2/appy/gen/ui/to.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      250 2016-10-11 18:35:13.669445 appy-1.0.9/py2/appy/gen/ui/toggleDetails.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      653 2016-10-11 18:35:14.177452 appy-1.0.9/py2/appy/gen/ui/transition.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      442 2016-10-11 18:35:14.177452 appy-1.0.9/py2/appy/gen/ui/unfreeze.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      231 2016-10-11 18:35:14.181452 appy-1.0.9/py2/appy/gen/ui/unlink.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      256 2016-10-11 18:35:14.177452 appy-1.0.9/py2/appy/gen/ui/unlinkMany.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      243 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/unlinkManyUp.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      234 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/unlinkUp.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      649 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/unlock.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1662 2016-10-11 18:35:14.189453 appy-1.0.9/py2/appy/gen/ui/unlockBig.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      391 2016-10-11 18:35:13.669445 appy-1.0.9/py2/appy/gen/ui/unselect.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      421 2016-10-11 18:35:13.669445 appy-1.0.9/py2/appy/gen/ui/upload.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      620 2017-04-03 19:27:08.317931 appy-1.0.9/py2/appy/gen/ui/url.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      643 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/user.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      208 2016-10-11 18:35:14.185452 appy-1.0.9/py2/appy/gen/ui/validate.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      314 2016-10-11 18:35:14.181452 appy-1.0.9/py2/appy/gen/ui/warning.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2003 2016-10-11 18:35:13.669445 appy-1.0.9/py2/appy/gen/ui/warningBig.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      823 2016-10-11 18:35:13.673446 appy-1.0.9/py2/appy/gen/ui/warning_no.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      623 2016-10-11 18:35:13.665445 appy-1.0.9/py2/appy/gen/ui/xls.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      621 2016-10-11 18:35:14.193452 appy-1.0.9/py2/appy/gen/ui/xlsFrozen.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      967 2019-12-04 17:19:06.274123 appy-1.0.9/py2/appy/gen/ui/xlsx.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      908 2019-12-04 17:19:21.402216 appy-1.0.9/py2/appy/gen/ui/xlsxFrozen.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    19476 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/utils.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6824 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/validate.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.761117 appy-1.0.9/py2/appy/gen/wrappers/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1760 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/wrappers/GroupWrapper.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2753 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/wrappers/PageWrapper.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    29396 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/wrappers/ToolWrapper.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3987 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/wrappers/TranslationWrapper.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    24774 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/wrappers/UserWrapper.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    78379 2021-10-26 12:39:29.089065 appy-1.0.9/py2/appy/gen/wrappers/__init__.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.761117 appy-1.0.9/py2/appy/pod/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4102 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/pod/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    28301 2021-10-26 12:39:29.073065 appy-1.0.9/py2/appy/pod/actions.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    41719 2021-10-26 12:39:29.073065 appy-1.0.9/py2/appy/pod/buffers.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1588 2020-06-18 10:20:35.111440 appy-1.0.9/py2/appy/pod/content.xmlt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    40864 2021-10-26 12:39:29.073065 appy-1.0.9/py2/appy/pod/converter.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    32711 2021-10-26 12:39:29.073065 appy-1.0.9/py2/appy/pod/doc_importers.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12105 2021-10-26 12:39:29.073065 appy-1.0.9/py2/appy/pod/elements.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      861 2016-10-11 18:35:10.749406 appy-1.0.9/py2/appy/pod/imageNotFound.jpg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13624 2021-10-26 12:39:29.073065 appy-1.0.9/py2/appy/pod/lo_pool.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1755 2021-10-26 12:39:29.073065 appy-1.0.9/py2/appy/pod/metadata.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2670 2021-10-26 12:39:29.073065 appy-1.0.9/py2/appy/pod/odf_parser.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4755 2021-10-26 12:39:29.073065 appy-1.0.9/py2/appy/pod/parts.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18259 2021-10-26 12:39:29.073065 appy-1.0.9/py2/appy/pod/pod_parser.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    48075 2021-10-26 12:39:29.073065 appy-1.0.9/py2/appy/pod/renderer.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7399 2020-06-18 10:20:24.867400 appy-1.0.9/py2/appy/pod/styles.xmlt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    76695 2021-10-26 12:39:29.073065 appy-1.0.9/py2/appy/pod/styles_manager.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.761117 appy-1.0.9/py2/appy/pod/test/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      896 2016-10-11 18:35:11.569417 appy-1.0.9/py2/appy/pod/test/Readme.txt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10345 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/pod/test/Tester.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    33348 2021-10-18 13:42:14.143712 appy-1.0.9/py2/appy/pod/test/Tests.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)        2 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/pod/test/__init__.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.765118 appy-1.0.9/py2/appy/pod/test/contexts/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       64 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/Chart1.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      164 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/ElseStatements.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       29 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/Empty.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       24 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/FieldExpressions.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      138 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/FileHandlerImport.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      897 2016-10-11 18:35:11.569417 appy-1.0.9/py2/appy/pod/test/contexts/ForCell6.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      222 2018-03-21 10:11:39.856653 appy-1.0.9/py2/appy/pod/test/contexts/IfAndFors1.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      674 2021-03-19 11:00:49.881946 appy-1.0.9/py2/appy/pod/test/contexts/ImagesImport.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      145 2020-03-30 13:54:07.615859 appy-1.0.9/py2/appy/pod/test/contexts/OdsSimple.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       35 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/OnlyExpressions.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       90 2016-10-11 18:35:11.569417 appy-1.0.9/py2/appy/pod/test/contexts/PathImport.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      177 2016-10-11 18:35:11.569417 appy-1.0.9/py2/appy/pod/test/contexts/PersonsEight.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      110 2016-10-11 18:35:11.569417 appy-1.0.9/py2/appy/pod/test/contexts/PersonsFour.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       96 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/PersonsThree.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       82 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/PersonsTwo.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       11 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/SimpleForEmptyList.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       37 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/SimpleForFilledList.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      109 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/SimpleForRow.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       11 2016-10-11 18:35:11.569417 appy-1.0.9/py2/appy/pod/test/contexts/SimpleIfIsFalse.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       10 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/SimpleIfIsTrue.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       59 2016-10-11 18:35:11.569417 appy-1.0.9/py2/appy/pod/test/contexts/SimpleTest.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      200 2018-04-18 08:13:19.908963 appy-1.0.9/py2/appy/pod/test/contexts/VarStatements.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11773 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlColgroupTable.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      703 2018-05-09 13:51:33.061535 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1849 2019-01-21 10:35:00.678872 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex2.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4299 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex3.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2790 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex4.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1805 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex5.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      278 2016-10-11 18:35:11.569417 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex6.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      582 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex7.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      996 2021-07-29 15:22:03.715092 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex8.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17472 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex9.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1883 2017-02-21 15:47:38.805767 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplexTables.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2897 2018-11-30 09:19:28.792011 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlCustomStyles.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       45 2021-09-13 09:07:17.859993 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlEmpty.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      224 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlEntities.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      128 2018-03-21 17:53:35.842060 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlHtml.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2424 2020-03-30 15:33:06.485025 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlKeepWithNext.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      507 2017-08-24 11:13:10.512979 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlListProperties.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      536 2016-12-20 19:09:41.282375 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlNominal.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      710 2021-07-12 07:48:43.845458 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlPIntoLis.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      449 2020-09-10 06:25:29.085683 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlPIntoTds.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1903 2020-11-12 08:06:18.007973 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlSpan.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      241 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlStylesErrors.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      533 2018-04-18 13:44:15.821519 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlStylesMapping.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      251 2019-04-05 09:02:47.358611 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlStylesMapping2.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      372 2017-08-24 13:20:05.929231 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlTableProperties.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4047 2020-12-18 09:01:19.997088 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlTables.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2466 2017-05-24 07:34:37.512122 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlTwisted.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      629 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/XhtmlWithStyle.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      596 2016-10-11 18:35:11.565417 appy-1.0.9/py2/appy/pod/test/contexts/__init__.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.765118 appy-1.0.9/py2/appy/pod/test/images/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    34607 2016-12-20 19:09:41.142375 appy-1.0.9/py2/appy/pod/test/images/imio.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1495 2016-10-11 18:35:11.193412 appy-1.0.9/py2/appy/pod/test/images/linux.jpg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2412 2016-10-11 18:35:11.193412 appy-1.0.9/py2/appy/pod/test/images/plone.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1194 2016-10-11 18:35:11.193412 appy-1.0.9/py2/appy/pod/test/images/python.blob
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1194 2016-10-11 18:35:11.193412 appy-1.0.9/py2/appy/pod/test/images/python.gif
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.769117 appy-1.0.9/py2/appy/pod/test/results/
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    19703 2018-10-25 14:45:50.975494 appy-1.0.9/py2/appy/pod/test/results/chart1.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19772 2021-07-29 10:36:35.397108 appy-1.0.9/py2/appy/pod/test/results/elseStatements.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7135 2016-10-11 18:35:11.173412 appy-1.0.9/py2/appy/pod/test/results/errorExpression.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11203 2018-10-25 14:50:32.400074 appy-1.0.9/py2/appy/pod/test/results/errorFooter.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7888 2021-09-13 14:29:03.699671 appy-1.0.9/py2/appy/pod/test/results/errorForParsetime.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7493 2016-10-11 18:35:11.189412 appy-1.0.9/py2/appy/pod/test/results/errorForRuntime.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11078 2016-12-20 19:09:40.962375 appy-1.0.9/py2/appy/pod/test/results/errorIf.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10870 2017-03-10 11:06:25.495770 appy-1.0.9/py2/appy/pod/test/results/fieldExpression.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    32790 2016-10-11 18:35:11.173412 appy-1.0.9/py2/appy/pod/test/results/fileHandlerImport.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11477 2018-10-25 13:41:43.473558 appy-1.0.9/py2/appy/pod/test/results/forCellBug.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10603 2018-10-25 13:42:31.293675 appy-1.0.9/py2/appy/pod/test/results/forCellBug2.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10676 2018-10-25 11:43:47.720535 appy-1.0.9/py2/appy/pod/test/results/forCellCorrectNumber.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10675 2018-10-25 13:28:27.919030 appy-1.0.9/py2/appy/pod/test/results/forCellNotEnough.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7234 2018-10-25 13:41:03.329466 appy-1.0.9/py2/appy/pod/test/results/forCellOnlyOne.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10671 2018-10-25 13:36:23.156984 appy-1.0.9/py2/appy/pod/test/results/forCellTooMuch1.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7300 2018-10-25 13:37:22.705060 appy-1.0.9/py2/appy/pod/test/results/forCellTooMuch2.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7373 2018-10-25 13:39:50.333311 appy-1.0.9/py2/appy/pod/test/results/forCellTooMuch3.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7393 2018-10-25 13:40:12.865357 appy-1.0.9/py2/appy/pod/test/results/forCellTooMuch4.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7042 2018-10-25 13:43:24.941812 appy-1.0.9/py2/appy/pod/test/results/forTable.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7819 2016-10-11 18:35:11.173412 appy-1.0.9/py2/appy/pod/test/results/forTableMinus.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8351 2018-10-25 14:39:09.105860 appy-1.0.9/py2/appy/pod/test/results/forTableMinus2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8140 2016-10-11 18:35:11.181412 appy-1.0.9/py2/appy/pod/test/results/forTableMinusError.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8175 2016-10-11 18:35:11.177412 appy-1.0.9/py2/appy/pod/test/results/forTableMinusError2.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11104 2018-10-25 14:39:58.542092 appy-1.0.9/py2/appy/pod/test/results/headerFooter.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    16676 2019-08-01 13:30:20.267359 appy-1.0.9/py2/appy/pod/test/results/ifAndFors1.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12528 2018-10-25 14:51:25.620213 appy-1.0.9/py2/appy/pod/test/results/ifElseErrors.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    59201 2021-04-20 14:20:52.878622 appy-1.0.9/py2/appy/pod/test/results/imagesImport.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8882 2018-10-25 11:46:29.553242 appy-1.0.9/py2/appy/pod/test/results/noPython.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12331 2020-03-30 13:54:09.699867 appy-1.0.9/py2/appy/pod/test/results/odsSimple.ods
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     9183 2018-10-25 11:54:22.215347 appy-1.0.9/py2/appy/pod/test/results/onlyExpressions.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    32780 2016-10-11 18:35:11.181412 appy-1.0.9/py2/appy/pod/test/results/pathImport.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6867 2016-10-11 18:35:11.189412 appy-1.0.9/py2/appy/pod/test/results/simpleForEmptyList.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6966 2016-10-11 18:35:11.189412 appy-1.0.9/py2/appy/pod/test/results/simpleForFilledList.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7560 2018-10-25 11:55:36.451696 appy-1.0.9/py2/appy/pod/test/results/simpleForRow.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10991 2018-10-25 14:41:02.730392 appy-1.0.9/py2/appy/pod/test/results/simpleFromTest.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6910 2016-10-11 18:35:11.177412 appy-1.0.9/py2/appy/pod/test/results/simpleIfIsFalse.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6923 2016-10-11 18:35:11.189412 appy-1.0.9/py2/appy/pod/test/results/simpleIfIsTrue.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8666 2016-10-11 18:35:11.185412 appy-1.0.9/py2/appy/pod/test/results/simpleIfIsTrue003.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7919 2016-10-11 18:35:11.181412 appy-1.0.9/py2/appy/pod/test/results/simpleMinusError.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8606 2016-10-11 18:35:11.169412 appy-1.0.9/py2/appy/pod/test/results/simpleTest.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    13100 2018-10-25 14:43:25.231053 appy-1.0.9/py2/appy/pod/test/results/varDef.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    15538 2018-10-25 11:53:33.595124 appy-1.0.9/py2/appy/pod/test/results/withAnImage.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11053 2016-10-11 18:35:11.193412 appy-1.0.9/py2/appy/pod/test/results/xhtmlColgroup.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    13969 2019-11-15 14:58:08.486379 appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11785 2019-01-21 13:08:50.714374 appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex2.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11178 2019-07-25 11:50:40.717704 appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex3.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8796 2019-07-25 11:52:03.761669 appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex4.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8906 2019-07-25 11:52:51.685670 appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex5.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8469 2018-11-30 09:50:11.162546 appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex6.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8576 2016-10-11 18:35:11.165412 appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex7.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11747 2021-07-29 15:37:23.051030 appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex8.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13568 2017-02-21 15:05:31.684520 appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex9.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    17763 2018-10-25 14:46:49.543589 appy-1.0.9/py2/appy/pod/test/results/xhtmlComplexTables.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    13090 2018-11-30 09:44:53.993350 appy-1.0.9/py2/appy/pod/test/results/xhtmlCustomStyles.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11729 2017-02-21 16:29:51.874710 appy-1.0.9/py2/appy/pod/test/results/xhtmlEmpty.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11948 2016-10-11 18:35:11.177412 appy-1.0.9/py2/appy/pod/test/results/xhtmlEntities.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10430 2018-03-21 16:01:33.686184 appy-1.0.9/py2/appy/pod/test/results/xhtmlHtml.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12045 2016-10-11 18:35:11.185412 appy-1.0.9/py2/appy/pod/test/results/xhtmlIgnoreStyles.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    13512 2019-07-25 11:58:13.653988 appy-1.0.9/py2/appy/pod/test/results/xhtmlInHeader.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15813 2020-12-18 09:47:54.242437 appy-1.0.9/py2/appy/pod/test/results/xhtmlKeepWithNext.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12143 2019-07-25 11:56:13.833816 appy-1.0.9/py2/appy/pod/test/results/xhtmlListProperties.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    35579 2016-12-20 19:09:40.962375 appy-1.0.9/py2/appy/pod/test/results/xhtmlNominal.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12146 2021-07-12 21:19:05.188170 appy-1.0.9/py2/appy/pod/test/results/xhtmlPIntoLis.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12010 2020-09-10 06:25:34.225663 appy-1.0.9/py2/appy/pod/test/results/xhtmlPIntoTds.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12521 2020-11-12 08:19:53.610753 appy-1.0.9/py2/appy/pod/test/results/xhtmlSpan.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13311 2016-10-11 18:35:11.189412 appy-1.0.9/py2/appy/pod/test/results/xhtmlStylesErrors.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15494 2018-04-18 16:14:08.596004 appy-1.0.9/py2/appy/pod/test/results/xhtmlStylesMapping.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11978 2019-04-05 09:10:26.884697 appy-1.0.9/py2/appy/pod/test/results/xhtmlStylesMapping2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12008 2017-08-24 12:42:14.129789 appy-1.0.9/py2/appy/pod/test/results/xhtmlTableProperties.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10632 2020-11-12 11:15:48.436856 appy-1.0.9/py2/appy/pod/test/results/xhtmlTables.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10944 2017-05-24 07:39:04.437787 appy-1.0.9/py2/appy/pod/test/results/xhtmlTwisted.odt
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.769117 appy-1.0.9/py2/appy/pod/test/templates/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19316 2016-10-11 18:35:10.757406 appy-1.0.9/py2/appy/pod/test/templates/Chart1.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9500 2021-10-18 15:32:31.820419 appy-1.0.9/py2/appy/pod/test/templates/DoDoc.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19106 2021-07-29 10:36:33.665111 appy-1.0.9/py2/appy/pod/test/templates/ElseStatements.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6410 2016-10-11 18:35:10.753406 appy-1.0.9/py2/appy/pod/test/templates/ErrorExpression.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10018 2016-10-11 18:35:10.753406 appy-1.0.9/py2/appy/pod/test/templates/ErrorFooter.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6916 2016-10-11 18:35:10.753406 appy-1.0.9/py2/appy/pod/test/templates/ErrorForParsetime.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6832 2016-10-11 18:35:10.761406 appy-1.0.9/py2/appy/pod/test/templates/ErrorForRuntime.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10085 2018-03-28 10:15:57.831696 appy-1.0.9/py2/appy/pod/test/templates/ErrorIf.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9928 2017-03-10 10:26:07.118621 appy-1.0.9/py2/appy/pod/test/templates/FieldExpressions.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7465 2016-10-11 18:35:10.753406 appy-1.0.9/py2/appy/pod/test/templates/FileHandlerImport.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9790 2018-10-25 11:43:44.328520 appy-1.0.9/py2/appy/pod/test/templates/ForCell.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6881 2016-10-11 18:35:10.761406 appy-1.0.9/py2/appy/pod/test/templates/ForCell2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6934 2016-10-11 18:35:10.765406 appy-1.0.9/py2/appy/pod/test/templates/ForCell3.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6952 2016-10-11 18:35:10.765406 appy-1.0.9/py2/appy/pod/test/templates/ForCell4.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6732 2016-10-11 18:35:10.765406 appy-1.0.9/py2/appy/pod/test/templates/ForCell5.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11001 2016-10-11 18:35:10.765406 appy-1.0.9/py2/appy/pod/test/templates/ForCell6.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10009 2016-10-11 18:35:10.765406 appy-1.0.9/py2/appy/pod/test/templates/ForCell7.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6542 2016-10-11 18:35:10.761406 appy-1.0.9/py2/appy/pod/test/templates/ForTable.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6798 2016-10-11 18:35:10.753406 appy-1.0.9/py2/appy/pod/test/templates/ForTableMinus.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7323 2016-10-11 18:35:10.761406 appy-1.0.9/py2/appy/pod/test/templates/ForTableMinus2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7098 2016-10-11 18:35:10.757406 appy-1.0.9/py2/appy/pod/test/templates/ForTableMinusError.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7099 2016-10-11 18:35:10.761406 appy-1.0.9/py2/appy/pod/test/templates/ForTableMinusError2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10215 2016-10-11 18:35:10.761406 appy-1.0.9/py2/appy/pod/test/templates/HeaderFooter.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    16196 2019-08-01 13:30:18.675353 appy-1.0.9/py2/appy/pod/test/templates/IfAndFors1.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11041 2016-10-11 18:35:10.761406 appy-1.0.9/py2/appy/pod/test/templates/IfElseErrors.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13788 2021-04-20 14:20:51.446617 appy-1.0.9/py2/appy/pod/test/templates/ImagesImport.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8298 2016-10-11 18:35:10.757406 appy-1.0.9/py2/appy/pod/test/templates/NoPython.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11234 2020-03-30 13:53:05.075600 appy-1.0.9/py2/appy/pod/test/templates/OdsSimple.ods
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8810 2016-10-11 18:35:10.757406 appy-1.0.9/py2/appy/pod/test/templates/OnlyExpressions.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7483 2016-10-11 18:35:10.757406 appy-1.0.9/py2/appy/pod/test/templates/PathImport.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6345 2016-10-11 18:35:10.765406 appy-1.0.9/py2/appy/pod/test/templates/SimpleForEmptyList.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6520 2016-10-11 18:35:10.753406 appy-1.0.9/py2/appy/pod/test/templates/SimpleForFilledList.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7160 2016-10-11 18:35:10.761406 appy-1.0.9/py2/appy/pod/test/templates/SimpleForRow.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9750 2016-10-11 18:35:10.757406 appy-1.0.9/py2/appy/pod/test/templates/SimpleFromTest.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6378 2016-10-11 18:35:10.757406 appy-1.0.9/py2/appy/pod/test/templates/SimpleIfIsFalse.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6378 2016-10-11 18:35:10.753406 appy-1.0.9/py2/appy/pod/test/templates/SimpleIfIsTrue.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8227 2016-10-11 18:35:10.765406 appy-1.0.9/py2/appy/pod/test/templates/SimpleIfIsTrue003.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6567 2016-10-11 18:35:10.757406 appy-1.0.9/py2/appy/pod/test/templates/SimpleMinusError.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8250 2016-10-11 18:35:10.761406 appy-1.0.9/py2/appy/pod/test/templates/SimpleTest.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    20714 2017-10-14 13:08:00.664723 appy-1.0.9/py2/appy/pod/test/templates/TablesToOptimize.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12089 2018-04-18 08:14:26.894173 appy-1.0.9/py2/appy/pod/test/templates/VarStatements.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15044 2016-10-11 18:35:10.749406 appy-1.0.9/py2/appy/pod/test/templates/WithAnImage.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12696 2019-11-15 14:58:03.398363 appy-1.0.9/py2/appy/pod/test/templates/Xhtml.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9156 2016-10-11 18:35:10.753406 appy-1.0.9/py2/appy/pod/test/templates/XhtmlColGroup.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10089 2018-04-18 11:50:50.825343 appy-1.0.9/py2/appy/pod/test/templates/XhtmlComplex2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8784 2016-10-11 18:35:10.761406 appy-1.0.9/py2/appy/pod/test/templates/XhtmlComplex3.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7730 2016-10-11 18:35:10.765406 appy-1.0.9/py2/appy/pod/test/templates/XhtmlComplex4.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10531 2021-07-29 15:20:58.043191 appy-1.0.9/py2/appy/pod/test/templates/XhtmlComplex8.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    16551 2016-10-11 18:35:10.757406 appy-1.0.9/py2/appy/pod/test/templates/XhtmlComplexTables.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9431 2018-03-21 15:46:22.391030 appy-1.0.9/py2/appy/pod/test/templates/XhtmlHtml.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12421 2016-10-11 18:35:10.749406 appy-1.0.9/py2/appy/pod/test/templates/XhtmlInHeader.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    14774 2020-03-30 15:36:03.041817 appy-1.0.9/py2/appy/pod/test/templates/XhtmlKeepWithNext.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    34605 2016-10-11 18:35:10.765406 appy-1.0.9/py2/appy/pod/test/templates/XhtmlNominal.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11284 2019-08-07 08:02:36.111421 appy-1.0.9/py2/appy/pod/test/templates/XhtmlSimple.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10674 2017-01-31 15:30:32.145286 appy-1.0.9/py2/appy/pod/test/templates/XhtmlSpan.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14445 2018-04-18 13:45:22.585631 appy-1.0.9/py2/appy/pod/test/templates/XhtmlStyles.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11839 2016-10-11 18:35:10.761406 appy-1.0.9/py2/appy/pod/test/templates/XhtmlStylesErrors.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7834 2016-10-11 18:35:10.761406 appy-1.0.9/py2/appy/pod/test/templates/XhtmlTables.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8930 2017-05-24 07:36:40.164945 appy-1.0.9/py2/appy/pod/test/templates/XhtmlTwisted.odt
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.769117 appy-1.0.9/py2/appy/pod/xhtml/
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      201 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/pod/xhtml/__init__.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     6263 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/pod/xhtml/parser.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10701 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/pod/xhtml/tags.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    15644 2021-10-26 12:39:29.077065 appy-1.0.9/py2/appy/pod/xhtml/visitors.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    64756 2021-10-26 12:39:29.073065 appy-1.0.9/py2/appy/pod/xhtml2odt.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.773118 appy-1.0.9/py2/appy/px/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11440 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/px/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7165 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/px/px_parser.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.773118 appy-1.0.9/py2/appy/shared/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3030 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/shared/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9010 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/shared/account.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    20757 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/shared/css.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13090 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/shared/csv_parser.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.773118 appy-1.0.9/py2/appy/shared/data/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)   164300 2016-10-11 18:35:13.049437 appy-1.0.9/py2/appy/shared/data/BelgianCommunes.txt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4089 2016-10-11 18:35:13.049437 appy-1.0.9/py2/appy/shared/data/CountryCodesIso3166.1.txt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15371 2016-10-11 18:35:13.049437 appy-1.0.9/py2/appy/shared/data/LanguageCodesIso639.2.txt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9128 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/shared/data/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7267 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/shared/dates.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22926 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/shared/dav.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    33882 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/shared/diff.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1510 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/shared/errors.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4663 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/shared/google.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4922 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/shared/ical.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22457 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/shared/ldap_connector.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2806 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/shared/odf.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14228 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/shared/packaging.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11267 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/shared/sap.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    21740 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/shared/sso.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18472 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/shared/tables.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14857 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/shared/test.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    36843 2021-10-26 12:39:29.081065 appy-1.0.9/py2/appy/shared/utils.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    58271 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/shared/xml_parser.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7392 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/shared/zip.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.773118 appy-1.0.9/py2/appy/test/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       77 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/test/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4098 2021-10-26 12:39:29.085065 appy-1.0.9/py2/appy/test/profiler.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       52 2021-10-26 12:39:29.093065 appy-1.0.9/py2/appy/version.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.749117 appy-1.0.9/py3/
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.773118 appy-1.0.9/py3/appy/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5153 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2627 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/all.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.773118 appy-1.0.9/py3/appy/bin/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2454 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/bin/__init__.py
+-rwxr-xr-x   0 gdy999    (1000) gdy999    (1000)     3835 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/bin/deploy.py
+-rwxrwxr-x   0 gdy999    (1000) gdy999    (1000)     4865 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/bin/lo.py
+-rwxrwxr-x   0 gdy999    (1000) gdy999    (1000)    19152 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/bin/make.py
+-rwxrwxr-x   0 gdy999    (1000) gdy999    (1000)     1936 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/bin/perform.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8558 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/bin/run.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.773118 appy-1.0.9/py3/appy/data/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4089 2017-07-31 20:04:30.105511 appy-1.0.9/py3/appy/data/Countries.Iso3166-1
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15371 2017-07-31 20:04:30.105511 appy-1.0.9/py3/appy/data/Languages.Iso639-2
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8658 2021-10-26 12:39:34.433114 appy-1.0.9/py3/appy/data/__init__.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.773118 appy-1.0.9/py3/appy/database/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    42852 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/database/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22244 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/database/catalog.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.773118 appy-1.0.9/py3/appy/database/indexes/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13573 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/database/indexes/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1363 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/database/indexes/boolean.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     3418 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/database/indexes/date.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1604 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/database/indexes/float.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2355 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/database/indexes/ref.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2255 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/database/indexes/rich.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2949 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/database/indexes/text.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5318 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/database/lazy.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7006 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/database/lock.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5379 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/database/log.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9310 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/database/operators.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4675 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/database/sorter.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.773118 appy-1.0.9/py3/appy/deploy/
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10191 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/deploy/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3468 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/deploy/subversion.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.773118 appy-1.0.9/py3/appy/model/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8087 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    66720 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/base.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6189 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/batch.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13492 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/carousel.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8526 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/document.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.777118 appy-1.0.9/py3/appy/model/fields/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    75504 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/fields/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    28350 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/action.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9397 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/boolean.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)   113930 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/calendar.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2974 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/color.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5485 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/colset.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12130 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/fields/computed.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2912 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/fields/custom.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17511 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/date.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10481 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/dict.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    29254 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/file.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3969 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/fields/float.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    20954 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/fields/group.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10289 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/hour.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2608 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/info.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7130 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/integer.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    23615 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/list.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14357 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/multilingual.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13062 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/ogone.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7413 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/password.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22874 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/phase.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    59682 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/pod.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7737 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/python.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)   125046 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/ref.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    24075 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/rich.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    22717 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/fields/select.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14247 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/string.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     5982 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/switch.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    37421 2021-10-26 12:39:34.417114 appy-1.0.9/py3/appy/model/fields/text.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2800 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/group.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    16657 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/loader.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.777118 appy-1.0.9/py3/appy/model/meta/
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     4286 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/meta/__init__.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    34353 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/meta/class_.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11639 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/meta/workflow.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5189 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/mover.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    17445 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/page.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.777118 appy-1.0.9/py3/appy/model/pod/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12395 2021-05-09 13:30:32.398004 appy-1.0.9/py3/appy/model/pod/Page.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7314 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/query.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.777118 appy-1.0.9/py3/appy/model/searches/
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    43813 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/searches/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4266 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/searches/gridder.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7053 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/searches/initiators.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    34546 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/searches/modes.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22935 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/tool.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7547 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/translation.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    31552 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/user.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8172 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/model/utils.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.777118 appy-1.0.9/py3/appy/model/workflow/
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     3653 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/workflow/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    25431 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/workflow/history.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6113 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/workflow/localRoles.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     3508 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/workflow/standard.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     9565 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/workflow/state.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    21932 2021-10-26 12:39:34.421114 appy-1.0.9/py3/appy/model/workflow/transition.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.777118 appy-1.0.9/py3/appy/peer/
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11639 2021-10-26 12:39:34.433114 appy-1.0.9/py3/appy/peer/__init__.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     4957 2021-10-26 12:39:34.433114 appy-1.0.9/py3/appy/peer/appy0.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10937 2021-10-26 12:39:34.433114 appy-1.0.9/py3/appy/peer/importer.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6947 2021-10-26 12:39:34.433114 appy-1.0.9/py3/appy/peer/unresolved.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.777118 appy-1.0.9/py3/appy/pod/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5688 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    29919 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/actions.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    42056 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/buffers.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1588 2020-06-19 06:42:25.671990 appy-1.0.9/py3/appy/pod/content.xmlt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    40794 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/converter.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    30039 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/doc_importers.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13019 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/elements.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      861 2017-07-26 14:43:09.919476 appy-1.0.9/py3/appy/pod/imageNotFound.jpg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13715 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/lo_pool.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2799 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/odf_parser.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4840 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/parts.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18302 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/pod_parser.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    56347 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/renderer.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7399 2020-06-19 06:42:33.848014 appy-1.0.9/py3/appy/pod/styles.xmlt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    76934 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/styles_manager.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.777118 appy-1.0.9/py3/appy/pod/test/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      896 2017-07-26 14:43:09.919476 appy-1.0.9/py3/appy/pod/test/Readme.txt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9726 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/test/Tester.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    33288 2021-10-25 11:03:45.393942 appy-1.0.9/py3/appy/pod/test/Tests.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      785 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/test/__init__.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.781118 appy-1.0.9/py3/appy/pod/test/contexts/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       64 2017-07-26 14:43:09.911476 appy-1.0.9/py3/appy/pod/test/contexts/Chart1.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      164 2017-07-26 14:43:09.911476 appy-1.0.9/py3/appy/pod/test/contexts/ElseStatements.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       29 2020-02-22 13:45:39.328852 appy-1.0.9/py3/appy/pod/test/contexts/Empty.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       24 2017-07-26 14:43:09.911476 appy-1.0.9/py3/appy/pod/test/contexts/FieldExpressions.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      138 2017-10-04 14:00:32.106218 appy-1.0.9/py3/appy/pod/test/contexts/FileHandlerImport.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      893 2017-10-04 13:22:14.323421 appy-1.0.9/py3/appy/pod/test/contexts/ForCell6.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      222 2018-03-21 13:34:02.632546 appy-1.0.9/py3/appy/pod/test/contexts/IfAndFors1.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      674 2019-02-08 13:14:02.033243 appy-1.0.9/py3/appy/pod/test/contexts/ImagesImport.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      145 2020-03-30 14:06:40.458959 appy-1.0.9/py3/appy/pod/test/contexts/OdsSimple.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       35 2017-07-26 14:43:09.911476 appy-1.0.9/py3/appy/pod/test/contexts/OnlyExpressions.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       90 2017-07-26 14:43:09.915476 appy-1.0.9/py3/appy/pod/test/contexts/PathImport.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      177 2017-07-26 14:43:09.915476 appy-1.0.9/py3/appy/pod/test/contexts/PersonsEight.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      110 2017-07-26 14:43:09.915476 appy-1.0.9/py3/appy/pod/test/contexts/PersonsFour.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       96 2017-07-26 14:43:09.911476 appy-1.0.9/py3/appy/pod/test/contexts/PersonsThree.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       82 2017-07-26 14:43:09.911476 appy-1.0.9/py3/appy/pod/test/contexts/PersonsTwo.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       11 2017-07-26 14:43:09.907476 appy-1.0.9/py3/appy/pod/test/contexts/SimpleForEmptyList.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       37 2017-07-26 14:43:09.907476 appy-1.0.9/py3/appy/pod/test/contexts/SimpleForFilledList.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      109 2017-07-26 14:43:09.911476 appy-1.0.9/py3/appy/pod/test/contexts/SimpleForRow.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       11 2017-07-26 14:43:09.915476 appy-1.0.9/py3/appy/pod/test/contexts/SimpleIfIsFalse.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       10 2017-07-26 14:43:09.907476 appy-1.0.9/py3/appy/pod/test/contexts/SimpleIfIsTrue.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       59 2017-07-26 14:43:09.915476 appy-1.0.9/py3/appy/pod/test/contexts/SimpleTest.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      200 2018-04-18 09:38:51.803129 appy-1.0.9/py3/appy/pod/test/contexts/VarStatements.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11773 2017-07-26 14:43:09.907476 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlColgroupTable.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      703 2017-07-26 14:43:09.911476 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1849 2019-01-21 13:13:06.007441 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex2.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4299 2017-07-26 14:43:09.907476 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex3.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2790 2017-07-26 14:43:09.915476 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex4.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1805 2017-07-26 14:43:09.907476 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex5.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      278 2017-07-26 14:43:09.915476 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex6.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      582 2017-07-26 14:43:09.907476 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex7.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      996 2021-07-29 15:48:24.038504 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex8.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17472 2017-07-26 14:43:09.907476 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex9.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1883 2017-07-26 14:43:09.903476 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplexTables.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2888 2020-02-23 09:39:39.765688 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlCustomStyles.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       45 2021-03-27 12:19:55.818879 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlEmpty.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      224 2017-07-26 14:43:09.907476 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlEntities.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      128 2018-03-21 15:59:07.176655 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlHtml.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2424 2019-11-15 10:38:18.049595 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlKeepWithNext.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      507 2017-08-24 11:37:48.121121 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlListProperties.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      536 2017-07-26 14:43:09.903476 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlNominal.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      710 2021-07-12 21:26:43.296266 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlPIntoLis.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      449 2020-09-10 08:28:52.116400 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlPIntoTds.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1903 2020-11-12 08:49:44.926234 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlSpan.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      241 2017-07-26 14:43:09.907476 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlStylesErrors.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      533 2018-04-18 16:40:08.640038 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlStylesMapping.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      251 2019-04-05 11:20:44.233306 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlStylesMapping2.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      372 2017-08-24 13:20:08.317236 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlTableProperties.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4047 2020-12-18 09:35:25.760508 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlTables.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2466 2017-07-26 14:43:09.903476 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlTwisted.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      629 2017-07-26 14:43:09.915476 appy-1.0.9/py3/appy/pod/test/contexts/XhtmlWithStyle.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      596 2017-07-26 14:43:09.907476 appy-1.0.9/py3/appy/pod/test/contexts/__init__.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.781118 appy-1.0.9/py3/appy/pod/test/images/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    34607 2017-07-26 14:43:09.899476 appy-1.0.9/py3/appy/pod/test/images/imio.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1495 2017-07-26 14:43:09.899476 appy-1.0.9/py3/appy/pod/test/images/linux.jpg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2412 2017-07-26 14:43:09.899476 appy-1.0.9/py3/appy/pod/test/images/plone.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1194 2017-07-26 14:43:09.903476 appy-1.0.9/py3/appy/pod/test/images/python.blob
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1194 2017-07-26 14:43:09.899476 appy-1.0.9/py3/appy/pod/test/images/python.gif
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.781118 appy-1.0.9/py3/appy/pod/test/results/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19703 2018-10-26 07:00:22.417921 appy-1.0.9/py3/appy/pod/test/results/chart1.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19772 2021-07-29 12:55:59.076664 appy-1.0.9/py3/appy/pod/test/results/elseStatements.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7135 2017-07-26 14:43:09.883476 appy-1.0.9/py3/appy/pod/test/results/errorExpression.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11203 2018-10-26 07:01:05.593989 appy-1.0.9/py3/appy/pod/test/results/errorFooter.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7888 2021-09-21 11:30:16.783079 appy-1.0.9/py3/appy/pod/test/results/errorForParsetime.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7493 2017-07-26 14:43:09.899476 appy-1.0.9/py3/appy/pod/test/results/errorForRuntime.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11078 2017-07-26 14:43:09.863476 appy-1.0.9/py3/appy/pod/test/results/errorIf.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10870 2017-07-26 14:43:09.867476 appy-1.0.9/py3/appy/pod/test/results/fieldExpression.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    32790 2017-07-26 14:43:09.879476 appy-1.0.9/py3/appy/pod/test/results/fileHandlerImport.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11477 2018-10-26 07:01:39.442042 appy-1.0.9/py3/appy/pod/test/results/forCellBug.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10603 2018-10-26 07:01:48.722056 appy-1.0.9/py3/appy/pod/test/results/forCellBug2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10676 2018-10-26 07:01:56.974070 appy-1.0.9/py3/appy/pod/test/results/forCellCorrectNumber.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10675 2018-10-26 07:02:07.042086 appy-1.0.9/py3/appy/pod/test/results/forCellNotEnough.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7234 2018-10-26 07:02:17.918103 appy-1.0.9/py3/appy/pod/test/results/forCellOnlyOne.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10671 2018-10-26 07:02:28.102119 appy-1.0.9/py3/appy/pod/test/results/forCellTooMuch1.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7300 2018-10-26 07:02:34.502130 appy-1.0.9/py3/appy/pod/test/results/forCellTooMuch2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7373 2018-10-26 07:02:42.746143 appy-1.0.9/py3/appy/pod/test/results/forCellTooMuch3.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7393 2018-10-26 07:02:51.646157 appy-1.0.9/py3/appy/pod/test/results/forCellTooMuch4.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7042 2018-10-26 07:03:33.290224 appy-1.0.9/py3/appy/pod/test/results/forTable.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7819 2017-07-26 14:43:09.883476 appy-1.0.9/py3/appy/pod/test/results/forTableMinus.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8351 2018-10-26 07:03:51.130253 appy-1.0.9/py3/appy/pod/test/results/forTableMinus2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8140 2017-07-26 14:43:09.887476 appy-1.0.9/py3/appy/pod/test/results/forTableMinusError.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8175 2017-07-26 14:43:09.883476 appy-1.0.9/py3/appy/pod/test/results/forTableMinusError2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11104 2018-10-26 07:04:12.142288 appy-1.0.9/py3/appy/pod/test/results/headerFooter.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    16676 2019-08-01 13:36:53.492831 appy-1.0.9/py3/appy/pod/test/results/ifAndFors1.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12580 2020-08-22 18:28:01.490383 appy-1.0.9/py3/appy/pod/test/results/ifElseErrors.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    59201 2021-04-20 14:29:29.072725 appy-1.0.9/py3/appy/pod/test/results/imagesImport.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8882 2018-10-26 07:04:39.662333 appy-1.0.9/py3/appy/pod/test/results/noPython.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12341 2020-03-30 14:11:22.632117 appy-1.0.9/py3/appy/pod/test/results/odsSimple.ods
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9183 2018-10-26 07:04:57.958363 appy-1.0.9/py3/appy/pod/test/results/onlyExpressions.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    32780 2017-07-26 14:43:09.887476 appy-1.0.9/py3/appy/pod/test/results/pathImport.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6867 2017-07-26 14:43:09.895476 appy-1.0.9/py3/appy/pod/test/results/simpleForEmptyList.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6966 2017-07-26 14:43:09.895476 appy-1.0.9/py3/appy/pod/test/results/simpleForFilledList.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7560 2018-10-26 07:05:07.310379 appy-1.0.9/py3/appy/pod/test/results/simpleForRow.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11135 2020-02-23 08:45:30.387467 appy-1.0.9/py3/appy/pod/test/results/simpleFromTest.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6910 2017-07-26 14:43:09.883476 appy-1.0.9/py3/appy/pod/test/results/simpleIfIsFalse.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6923 2017-07-26 14:43:09.895476 appy-1.0.9/py3/appy/pod/test/results/simpleIfIsTrue.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8666 2017-07-26 14:43:09.887476 appy-1.0.9/py3/appy/pod/test/results/simpleIfIsTrue003.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7919 2017-07-26 14:43:09.883476 appy-1.0.9/py3/appy/pod/test/results/simpleMinusError.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8606 2017-07-26 14:43:09.879476 appy-1.0.9/py3/appy/pod/test/results/simpleTest.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    13028 2020-04-09 10:11:08.867661 appy-1.0.9/py3/appy/pod/test/results/varDef.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15538 2018-10-26 07:05:35.146425 appy-1.0.9/py3/appy/pod/test/results/withAnImage.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11053 2017-07-26 14:43:09.899476 appy-1.0.9/py3/appy/pod/test/results/xhtmlColgroup.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13969 2019-11-15 15:07:42.104245 appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11785 2019-01-21 13:13:15.135479 appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11178 2019-07-25 12:05:47.030991 appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex3.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8796 2019-07-25 12:05:54.659011 appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex4.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8906 2019-07-25 12:06:02.407031 appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex5.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8469 2018-11-30 10:56:13.107674 appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex6.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8576 2017-07-26 14:43:09.875476 appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex7.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11747 2021-07-29 15:48:43.078487 appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex8.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13568 2017-07-26 14:43:09.867476 appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex9.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17763 2018-10-26 07:05:43.714439 appy-1.0.9/py3/appy/pod/test/results/xhtmlComplexTables.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    13090 2018-11-30 10:56:23.379712 appy-1.0.9/py3/appy/pod/test/results/xhtmlCustomStyles.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11729 2017-07-26 14:43:09.867476 appy-1.0.9/py3/appy/pod/test/results/xhtmlEmpty.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11948 2017-07-26 14:43:09.883476 appy-1.0.9/py3/appy/pod/test/results/xhtmlEntities.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10430 2018-03-21 16:01:33.686184 appy-1.0.9/py3/appy/pod/test/results/xhtmlHtml.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12045 2017-07-26 14:43:09.891476 appy-1.0.9/py3/appy/pod/test/results/xhtmlIgnoreStyles.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13512 2019-07-25 12:06:19.711078 appy-1.0.9/py3/appy/pod/test/results/xhtmlInHeader.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15893 2020-12-18 09:51:30.485914 appy-1.0.9/py3/appy/pod/test/results/xhtmlKeepWithNext.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12143 2019-07-25 12:06:37.775126 appy-1.0.9/py3/appy/pod/test/results/xhtmlListProperties.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    35579 2017-07-26 14:43:09.863476 appy-1.0.9/py3/appy/pod/test/results/xhtmlNominal.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    12146 2021-07-12 21:27:46.316281 appy-1.0.9/py3/appy/pod/test/results/xhtmlPIntoLis.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12010 2020-09-10 08:29:51.072435 appy-1.0.9/py3/appy/pod/test/results/xhtmlPIntoTds.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12521 2020-11-12 08:50:11.406453 appy-1.0.9/py3/appy/pod/test/results/xhtmlSpan.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13311 2017-07-26 14:43:09.895476 appy-1.0.9/py3/appy/pod/test/results/xhtmlStylesErrors.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15494 2018-04-18 16:14:08.596004 appy-1.0.9/py3/appy/pod/test/results/xhtmlStylesMapping.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    11978 2019-04-05 11:21:06.457405 appy-1.0.9/py3/appy/pod/test/results/xhtmlStylesMapping2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12008 2017-08-24 12:42:14.129789 appy-1.0.9/py3/appy/pod/test/results/xhtmlTableProperties.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10632 2020-11-12 11:30:17.155001 appy-1.0.9/py3/appy/pod/test/results/xhtmlTables.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10944 2017-07-26 14:43:09.867476 appy-1.0.9/py3/appy/pod/test/results/xhtmlTwisted.odt
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.785118 appy-1.0.9/py3/appy/pod/test/templates/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19316 2017-07-26 14:43:09.851476 appy-1.0.9/py3/appy/pod/test/templates/Chart1.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9500 2021-10-25 10:57:45.502605 appy-1.0.9/py3/appy/pod/test/templates/DoDoc.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19106 2021-07-29 12:56:07.652624 appy-1.0.9/py3/appy/pod/test/templates/ElseStatements.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6410 2017-07-26 14:43:09.847476 appy-1.0.9/py3/appy/pod/test/templates/ErrorExpression.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10018 2017-07-26 14:43:09.843476 appy-1.0.9/py3/appy/pod/test/templates/ErrorFooter.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6916 2017-07-26 14:43:09.847476 appy-1.0.9/py3/appy/pod/test/templates/ErrorForParsetime.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6832 2017-07-26 14:43:09.855476 appy-1.0.9/py3/appy/pod/test/templates/ErrorForRuntime.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10085 2018-03-28 10:15:57.831696 appy-1.0.9/py3/appy/pod/test/templates/ErrorIf.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9928 2017-07-26 14:43:09.851476 appy-1.0.9/py3/appy/pod/test/templates/FieldExpressions.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7465 2017-07-26 14:43:09.847476 appy-1.0.9/py3/appy/pod/test/templates/FileHandlerImport.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9790 2018-10-26 07:05:57.190461 appy-1.0.9/py3/appy/pod/test/templates/ForCell.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6881 2017-07-26 14:43:09.859476 appy-1.0.9/py3/appy/pod/test/templates/ForCell2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6934 2017-07-26 14:43:09.859476 appy-1.0.9/py3/appy/pod/test/templates/ForCell3.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6952 2017-07-26 14:43:09.859476 appy-1.0.9/py3/appy/pod/test/templates/ForCell4.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6732 2017-07-26 14:43:09.859476 appy-1.0.9/py3/appy/pod/test/templates/ForCell5.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11001 2017-07-26 14:43:09.863476 appy-1.0.9/py3/appy/pod/test/templates/ForCell6.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10009 2017-07-26 14:43:09.863476 appy-1.0.9/py3/appy/pod/test/templates/ForCell7.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6542 2017-07-26 14:43:09.855476 appy-1.0.9/py3/appy/pod/test/templates/ForTable.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6798 2017-07-26 14:43:09.847476 appy-1.0.9/py3/appy/pod/test/templates/ForTableMinus.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7323 2017-07-26 14:43:09.855476 appy-1.0.9/py3/appy/pod/test/templates/ForTableMinus2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7098 2017-07-26 14:43:09.851476 appy-1.0.9/py3/appy/pod/test/templates/ForTableMinusError.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7099 2017-07-26 14:43:09.855476 appy-1.0.9/py3/appy/pod/test/templates/ForTableMinusError2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8774 2019-04-30 19:29:28.745345 appy-1.0.9/py3/appy/pod/test/templates/FromPod.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10215 2017-07-26 14:43:09.855476 appy-1.0.9/py3/appy/pod/test/templates/HeaderFooter.odt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    16196 2020-08-22 17:54:56.295078 appy-1.0.9/py3/appy/pod/test/templates/IfAndFors1.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11041 2017-07-26 14:43:09.855476 appy-1.0.9/py3/appy/pod/test/templates/IfElseErrors.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13788 2021-04-20 14:29:37.852760 appy-1.0.9/py3/appy/pod/test/templates/ImagesImport.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8298 2017-07-26 14:43:09.847476 appy-1.0.9/py3/appy/pod/test/templates/NoPython.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11234 2020-03-30 14:07:09.155077 appy-1.0.9/py3/appy/pod/test/templates/OdsSimple.ods
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8810 2017-07-26 14:43:09.851476 appy-1.0.9/py3/appy/pod/test/templates/OnlyExpressions.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7483 2017-07-26 14:43:09.851476 appy-1.0.9/py3/appy/pod/test/templates/PathImport.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6345 2017-07-26 14:43:09.859476 appy-1.0.9/py3/appy/pod/test/templates/SimpleForEmptyList.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6520 2017-07-26 14:43:09.847476 appy-1.0.9/py3/appy/pod/test/templates/SimpleForFilledList.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7160 2017-07-26 14:43:09.851476 appy-1.0.9/py3/appy/pod/test/templates/SimpleForRow.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9750 2017-07-26 14:43:09.847476 appy-1.0.9/py3/appy/pod/test/templates/SimpleFromTest.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6378 2017-07-26 14:43:09.847476 appy-1.0.9/py3/appy/pod/test/templates/SimpleIfIsFalse.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6378 2017-07-26 14:43:09.843476 appy-1.0.9/py3/appy/pod/test/templates/SimpleIfIsTrue.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8227 2017-07-26 14:43:09.863476 appy-1.0.9/py3/appy/pod/test/templates/SimpleIfIsTrue003.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6567 2017-07-26 14:43:09.847476 appy-1.0.9/py3/appy/pod/test/templates/SimpleMinusError.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8250 2017-07-26 14:43:09.851476 appy-1.0.9/py3/appy/pod/test/templates/SimpleTest.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    20714 2017-10-14 13:08:00.664723 appy-1.0.9/py3/appy/pod/test/templates/TablesToOptimize.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12089 2018-04-18 08:14:26.894172 appy-1.0.9/py3/appy/pod/test/templates/VarStatements.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15044 2017-07-26 14:43:09.843476 appy-1.0.9/py3/appy/pod/test/templates/WithAnImage.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12696 2019-11-15 15:07:52.912282 appy-1.0.9/py3/appy/pod/test/templates/Xhtml.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9156 2017-07-26 14:43:09.843476 appy-1.0.9/py3/appy/pod/test/templates/XhtmlColGroup.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10089 2018-04-18 11:50:50.825343 appy-1.0.9/py3/appy/pod/test/templates/XhtmlComplex2.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8784 2017-07-26 14:43:09.859476 appy-1.0.9/py3/appy/pod/test/templates/XhtmlComplex3.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7730 2017-07-26 14:43:09.859476 appy-1.0.9/py3/appy/pod/test/templates/XhtmlComplex4.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10531 2021-07-29 15:48:56.902474 appy-1.0.9/py3/appy/pod/test/templates/XhtmlComplex8.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    16551 2017-07-26 14:43:09.851476 appy-1.0.9/py3/appy/pod/test/templates/XhtmlComplexTables.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9431 2018-03-21 15:46:22.391030 appy-1.0.9/py3/appy/pod/test/templates/XhtmlHtml.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12421 2017-07-26 14:43:09.839476 appy-1.0.9/py3/appy/pod/test/templates/XhtmlInHeader.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14774 2019-11-15 10:38:42.585725 appy-1.0.9/py3/appy/pod/test/templates/XhtmlKeepWithNext.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    34605 2017-07-26 14:43:09.859476 appy-1.0.9/py3/appy/pod/test/templates/XhtmlNominal.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11284 2017-07-26 14:43:09.843476 appy-1.0.9/py3/appy/pod/test/templates/XhtmlSimple.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10674 2017-07-26 14:43:09.863476 appy-1.0.9/py3/appy/pod/test/templates/XhtmlSpan.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14445 2018-04-18 13:45:22.585631 appy-1.0.9/py3/appy/pod/test/templates/XhtmlStyles.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11839 2017-07-26 14:43:09.855476 appy-1.0.9/py3/appy/pod/test/templates/XhtmlStylesErrors.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7834 2017-07-26 14:43:09.851476 appy-1.0.9/py3/appy/pod/test/templates/XhtmlTables.odt
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8930 2017-07-26 14:43:09.839476 appy-1.0.9/py3/appy/pod/test/templates/XhtmlTwisted.odt
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.785118 appy-1.0.9/py3/appy/pod/xhtml/
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      960 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/xhtml/__init__.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     6687 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/xhtml/parser.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    10660 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/xhtml/tags.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    15756 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/xhtml/visitors.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    66259 2021-10-26 12:39:34.409114 appy-1.0.9/py3/appy/pod/xhtml2odt.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.785118 appy-1.0.9/py3/appy/px/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18984 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/px/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7461 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/px/parser.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.785118 appy-1.0.9/py3/appy/server/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    27835 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/server/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15274 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/server/backup.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    11021 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/server/context.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4185 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/server/cookie.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5657 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/server/error.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    26386 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/server/guard.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    24375 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/server/handler.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1856 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/server/languages.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    22526 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/server/ldap.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    19055 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/server/pool.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7187 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/server/request.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14071 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/server/response.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    20887 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/server/scheduler.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    21464 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/server/sso.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    13325 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/server/static.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17386 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/server/traversal.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.785118 appy-1.0.9/py3/appy/test/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      777 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/test/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15249 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/test/integration.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3956 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/test/monitoring.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14169 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/test/performance.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.785118 appy-1.0.9/py3/appy/tr/
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     3477 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/tr/__init__.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.785118 appy-1.0.9/py3/appy/tr/po/
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    37167 2021-10-25 21:46:08.249155 appy-1.0.9/py3/appy/tr/po/Appy.pot
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    16361 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/tr/po/__init__.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    37548 2021-10-25 21:46:43.289914 appy-1.0.9/py3/appy/tr/po/ar.po
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    39565 2021-10-25 21:46:43.293914 appy-1.0.9/py3/appy/tr/po/de.po
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    51307 2021-10-25 21:47:01.406306 appy-1.0.9/py3/appy/tr/po/en.po
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    38730 2021-10-25 21:46:43.309914 appy-1.0.9/py3/appy/tr/po/es.po
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    53982 2021-10-25 21:46:58.778249 appy-1.0.9/py3/appy/tr/po/fr.po
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    38752 2021-10-25 21:46:43.329915 appy-1.0.9/py3/appy/tr/po/it.po
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    42191 2021-10-25 21:46:43.337915 appy-1.0.9/py3/appy/tr/po/nl.po
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    20689 2021-10-26 12:39:34.425114 appy-1.0.9/py3/appy/tr/updater.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.785118 appy-1.0.9/py3/appy/ui/
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    45347 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/__init__.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     9050 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/account.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     4543 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/criteria.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    21023 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/css.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5939 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/globals.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2741 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/iframe.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4013 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/includer.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2001 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/js.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3611 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/language.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    26106 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/layout.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     4769 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/message.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17529 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/navigate.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5996 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/portlet.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.793118 appy-1.0.9/py3/appy/ui/static/
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1431 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/action.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      963 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/add.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      349 2017-12-03 10:34:35.198912 appy-1.0.9/py3/appy/ui/static/addAbove.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      356 2017-12-03 10:34:31.814888 appy-1.0.9/py3/appy/ui/static/addAboveFrom.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      346 2017-12-02 13:05:25.147842 appy-1.0.9/py3/appy/ui/static/addBelow.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      238 2016-10-11 18:35:14.181452 appy-1.0.9/py3/appy/ui/static/addFrom.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      209 2016-10-11 18:35:14.185452 appy-1.0.9/py3/appy/ui/static/angled.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     7185 2020-05-21 07:59:58.067896 appy-1.0.9/py3/appy/ui/static/appleicon.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    14345 2021-10-21 12:32:15.405011 appy-1.0.9/py3/appy/ui/static/appy.css
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)    55077 2021-07-02 12:45:12.526545 appy-1.0.9/py3/appy/ui/static/appy.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      266 2019-10-12 15:36:04.076676 appy-1.0.9/py3/appy/ui/static/appyrtl.css
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      393 2020-12-02 12:55:54.083870 appy-1.0.9/py3/appy/ui/static/arrow.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      484 2020-12-02 12:56:13.691835 appy-1.0.9/py3/appy/ui/static/arrows.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      482 2020-12-02 13:29:57.086885 appy-1.0.9/py3/appy/ui/static/arrowsA.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1048 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/asc.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      821 2016-10-11 18:35:14.181452 appy-1.0.9/py3/appy/ui/static/back.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      518 2020-10-19 13:10:30.352504 appy-1.0.9/py3/appy/ui/static/baseBG.jpg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      735 2020-10-07 12:23:43.251580 appy-1.0.9/py3/appy/ui/static/burger.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9878 2020-05-23 09:16:10.586025 appy-1.0.9/py3/appy/ui/static/calendar.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1958 2020-05-25 06:11:43.916825 appy-1.0.9/py3/appy/ui/static/calendar.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     3450 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/cancel.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      255 2016-10-11 18:35:14.189452 appy-1.0.9/py3/appy/ui/static/changes.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      250 2016-10-11 18:35:14.185452 appy-1.0.9/py3/appy/ui/static/changesNo.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      926 2020-05-03 09:12:26.925560 appy-1.0.9/py3/appy/ui/static/checkAll.svg
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.793118 appy-1.0.9/py3/appy/ui/static/ckeditor/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      289 2016-10-11 18:35:14.189452 appy-1.0.9/py3/appy/ui/static/ckeditor/Readme
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1471 2020-06-07 09:46:31.266478 appy-1.0.9/py3/appy/ui/static/ckeditor/config.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2574 2020-06-07 09:47:03.614665 appy-1.0.9/py3/appy/ui/static/ckeditor/contents.css
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      365 2016-12-20 19:09:41.746375 appy-1.0.9/py3/appy/ui/static/ckeditor/styles.js
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      656 2020-05-25 07:37:30.287932 appy-1.0.9/py3/appy/ui/static/close.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      159 2017-01-11 15:15:14.258984 appy-1.0.9/py3/appy/ui/static/collapse.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1052 2020-10-07 12:22:36.658985 appy-1.0.9/py3/appy/ui/static/config.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      244 2016-10-11 18:35:14.185452 appy-1.0.9/py3/appy/ui/static/current.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2391 2021-05-01 08:21:13.319728 appy-1.0.9/py3/appy/ui/static/custom.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1277 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/delete.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1650 2020-12-02 13:34:29.666668 appy-1.0.9/py3/appy/ui/static/deleteMany.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1102 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/deleteS.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      248 2016-10-11 18:35:14.193452 appy-1.0.9/py3/appy/ui/static/done.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      888 2020-12-02 13:27:34.158976 appy-1.0.9/py3/appy/ui/static/download.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      971 2020-11-29 18:01:53.222345 appy-1.0.9/py3/appy/ui/static/edit.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      971 2020-11-29 18:01:53.222345 appy-1.0.9/py3/appy/ui/static/editPage.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      760 2016-10-11 18:35:14.177452 appy-1.0.9/py3/appy/ui/static/email.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      163 2017-01-11 15:15:40.939234 appy-1.0.9/py3/appy/ui/static/expand.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      685 2016-10-11 18:35:14.193452 appy-1.0.9/py3/appy/ui/static/external.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4286 2016-10-11 18:35:13.669445 appy-1.0.9/py3/appy/ui/static/favicon.ico
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      350 2016-10-11 18:35:13.673445 appy-1.0.9/py3/appy/ui/static/freeze.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      177 2016-10-11 18:35:13.673445 appy-1.0.9/py3/appy/ui/static/frozen.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1517 2020-05-01 12:54:01.725035 appy-1.0.9/py3/appy/ui/static/funnel.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      235 2016-10-11 18:35:13.669445 appy-1.0.9/py3/appy/ui/static/gotoNumber.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1130 2021-05-01 07:08:58.405262 appy-1.0.9/py3/appy/ui/static/grid.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1939 2020-06-30 09:36:30.869973 appy-1.0.9/py3/appy/ui/static/groups.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1686 2020-10-07 15:26:15.420097 appy-1.0.9/py3/appy/ui/static/headerBG.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1521 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/help.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1547 2020-05-15 05:19:57.938326 appy-1.0.9/py3/appy/ui/static/history.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      638 2020-10-07 12:23:17.711351 appy-1.0.9/py3/appy/ui/static/home.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)   809708 2020-10-07 15:29:39.334362 appy-1.0.9/py3/appy/ui/static/homeBG.jpg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1686 2020-10-07 15:26:15.420097 appy-1.0.9/py3/appy/ui/static/homeLogo.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      143 2019-04-16 17:17:42.056992 appy-1.0.9/py3/appy/ui/static/icon_blank.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      281 2019-04-13 17:14:40.738721 appy-1.0.9/py3/appy/ui/static/icon_bold.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      140 2019-04-16 17:17:48.161005 appy-1.0.9/py3/appy/ui/static/icon_dash.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      396 2019-04-16 17:17:55.733023 appy-1.0.9/py3/appy/ui/static/icon_highlight.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      279 2019-04-13 17:14:53.938858 appy-1.0.9/py3/appy/ui/static/icon_italic.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      343 2019-04-16 17:18:05.225044 appy-1.0.9/py3/appy/ui/static/icon_lengthen.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2012 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/internals.svg
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.793118 appy-1.0.9/py3/appy/ui/static/jscalendar/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4830 2016-10-11 18:35:13.677445 appy-1.0.9/py3/appy/ui/static/jscalendar/calendar-blue.css
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5057 2016-10-11 18:35:13.945449 appy-1.0.9/py3/appy/ui/static/jscalendar/calendar-setup.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    34353 2016-10-11 18:35:13.673445 appy-1.0.9/py3/appy/ui/static/jscalendar/calendar.js
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.793118 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1011 2016-10-11 18:35:13.933449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-af.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2135 2016-10-11 18:35:13.933449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-al.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3723 2016-10-11 18:35:13.941449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-bg.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3525 2016-10-11 18:35:13.945449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-big5-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3290 2016-10-11 18:35:13.941449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-big5.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3706 2016-10-11 18:35:13.937449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-br.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3597 2016-10-11 18:35:13.941449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-ca.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2940 2016-10-11 18:35:13.941449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-cs-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2810 2016-10-11 18:35:13.933449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-cs-win.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3500 2016-10-11 18:35:13.941449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-da.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3863 2016-10-11 18:35:13.941449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-de.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1143 2016-10-11 18:35:13.945449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-du.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3241 2016-10-11 18:35:13.933449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-el.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3600 2016-10-11 18:35:13.933449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-en.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3917 2016-10-11 18:35:13.941449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-es.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3827 2016-10-11 18:35:13.945449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-eu.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2782 2016-10-11 18:35:13.941449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-fi.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4071 2016-10-11 18:35:13.937449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-fr.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3919 2016-10-11 18:35:13.929449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-he-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1553 2016-10-11 18:35:13.933449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-hr-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3088 2016-10-11 18:35:13.937449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-hr.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3603 2016-10-11 18:35:13.945449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-hu.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3633 2016-10-11 18:35:13.937449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-it.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      913 2016-10-11 18:35:13.937449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-jp.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3568 2016-10-11 18:35:13.941449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-ko-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3256 2016-10-11 18:35:13.945449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-ko.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3432 2016-10-11 18:35:13.937449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-lt-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3400 2016-10-11 18:35:13.937449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-lt.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3603 2016-10-11 18:35:13.937449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-lv.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2234 2016-10-11 18:35:13.937449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-nl.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3178 2016-10-11 18:35:13.945449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-no.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2635 2016-10-11 18:35:13.933449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-pl-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2414 2016-10-11 18:35:13.937449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-pl.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3526 2016-10-11 18:35:13.937449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-pt.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2058 2016-10-11 18:35:13.929449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-ro.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3985 2016-10-11 18:35:13.929449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-ru-UTF.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4357 2016-10-11 18:35:13.933449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-ru.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3643 2016-10-11 18:35:13.941449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-ru_win_.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2684 2016-10-11 18:35:13.945449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-si.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2661 2016-10-11 18:35:13.945449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-sk.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3015 2016-10-11 18:35:13.937449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-sp.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2759 2016-10-11 18:35:13.945449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-sr-utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5492 2016-10-11 18:35:13.941449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-sr.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3973 2016-10-11 18:35:13.941449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-sv.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1736 2016-10-11 18:35:13.941449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-tr.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3082 2016-10-11 18:35:13.937449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-zh.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4751 2016-10-11 18:35:13.941449 appy-1.0.9/py3/appy/ui/static/jscalendar/lang/cn_utf8.js
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       68 2016-10-11 18:35:13.945449 appy-1.0.9/py3/appy/ui/static/jscalendar/menuarrow.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       49 2016-10-11 18:35:13.677445 appy-1.0.9/py3/appy/ui/static/jscalendar/menuarrow2.gif
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.749117 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.793118 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/aqua/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       89 2016-10-11 18:35:13.677445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/aqua/active-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       85 2016-10-11 18:35:13.677445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/aqua/dark-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       89 2016-10-11 18:35:13.677445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/aqua/hover-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       49 2016-10-11 18:35:13.677445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/aqua/menuarrow.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      110 2016-10-11 18:35:13.677445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/aqua/normal-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      110 2016-10-11 18:35:13.677445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/aqua/rowhover-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      116 2016-10-11 18:35:13.677445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/aqua/status-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5576 2016-10-11 18:35:13.677445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/aqua/theme.css
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      116 2016-10-11 18:35:13.677445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/aqua/title-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1122 2016-10-11 18:35:13.677445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/aqua/today-bg.gif
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.793118 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/tiger/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/tiger/active-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/tiger/dark-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/tiger/hover-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       49 2016-10-11 18:35:13.681445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/tiger/menuarrow.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/tiger/normal-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.681445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/tiger/rowhover-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      149 2016-10-11 18:35:13.685446 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/tiger/status-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     5772 2016-10-11 18:35:13.681445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/tiger/theme.css
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      149 2016-10-11 18:35:13.681445 appy-1.0.9/py3/appy/ui/static/jscalendar/skins/tiger/title-bg.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       51 2016-10-11 18:35:14.193452 appy-1.0.9/py3/appy/ui/static/li.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      234 2016-10-11 18:35:13.665445 appy-1.0.9/py3/appy/ui/static/link.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1385 2020-05-03 09:11:58.405420 appy-1.0.9/py3/appy/ui/static/linkMany.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       50 2016-10-11 18:35:13.669445 appy-1.0.9/py3/appy/ui/static/lirtl.gif
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1428 2021-05-01 07:02:35.257410 appy-1.0.9/py3/appy/ui/static/list.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    10766 2016-10-11 18:35:14.185452 appy-1.0.9/py3/appy/ui/static/loading_big.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1516 2016-10-11 18:35:14.181452 appy-1.0.9/py3/appy/ui/static/loading_button.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3429 2016-10-11 18:35:13.673445 appy-1.0.9/py3/appy/ui/static/loading_icon.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1281 2016-10-11 18:35:13.665445 appy-1.0.9/py3/appy/ui/static/loading_link.gif
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1076 2020-05-04 11:36:14.632703 appy-1.0.9/py3/appy/ui/static/locked.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1420 2020-10-07 12:18:31.232851 appy-1.0.9/py3/appy/ui/static/login.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     4179 2019-10-13 13:08:38.809234 appy-1.0.9/py3/appy/ui/static/loginLogo.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1195 2020-10-07 12:20:12.697721 appy-1.0.9/py3/appy/ui/static/logout.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      281 2019-04-25 08:34:17.501090 appy-1.0.9/py3/appy/ui/static/more.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      233 2016-10-11 18:35:14.189452 appy-1.0.9/py3/appy/ui/static/move.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      114 2016-10-11 18:35:14.185452 appy-1.0.9/py3/appy/ui/static/object.gif
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1907 2020-04-30 09:28:48.404131 appy-1.0.9/py3/appy/ui/static/page.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1406 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/pagePages.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3678 2020-05-01 12:09:02.985098 appy-1.0.9/py3/appy/ui/static/pagePassword.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1237 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/pageProfile.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1637 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/pageTranslations.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1899 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/pageUsers.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      665 2017-04-03 19:23:17.060212 appy-1.0.9/py3/appy/ui/static/paperclip.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1972 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/password.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     2011 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/pay.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      251 2016-10-11 18:35:14.177452 appy-1.0.9/py3/appy/ui/static/plus.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      518 2020-10-19 13:10:30.352504 appy-1.0.9/py3/appy/ui/static/popupBG.jpg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      963 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/portletAdd.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     4179 2019-10-13 13:08:38.809234 appy-1.0.9/py3/appy/ui/static/portletLogo.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      607 2016-10-11 18:35:14.185452 appy-1.0.9/py3/appy/ui/static/pwd.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1315 2021-05-16 20:28:31.050907 appy-1.0.9/py3/appy/ui/static/python.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      834 2019-09-05 20:18:39.232602 appy-1.0.9/py3/appy/ui/static/refresh.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      632 2016-10-11 18:35:13.673445 appy-1.0.9/py3/appy/ui/static/reindex.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      168 2018-09-27 14:01:52.821020 appy-1.0.9/py3/appy/ui/static/repeated.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      179 2018-09-27 14:03:43.909542 appy-1.0.9/py3/appy/ui/static/repeated_last.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       86 2021-03-29 11:33:47.143711 appy-1.0.9/py3/appy/ui/static/robots.txt
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1346 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/save.svg
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     1174 2020-04-28 18:31:30.000000 appy-1.0.9/py3/appy/ui/static/search.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      165 2016-12-20 19:09:41.746375 appy-1.0.9/py3/appy/ui/static/select.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      211 2016-10-11 18:35:14.193452 appy-1.0.9/py3/appy/ui/static/to.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      442 2016-10-11 18:35:14.177452 appy-1.0.9/py3/appy/ui/static/unfreeze.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      697 2020-05-04 07:42:51.901919 appy-1.0.9/py3/appy/ui/static/unlink.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1371 2020-05-04 07:42:49.773909 appy-1.0.9/py3/appy/ui/static/unlinkMany.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      243 2016-10-11 18:35:14.185452 appy-1.0.9/py3/appy/ui/static/unlinkManyUp.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      234 2016-10-11 18:35:13.673445 appy-1.0.9/py3/appy/ui/static/unlinkUp.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      391 2016-10-11 18:35:13.669445 appy-1.0.9/py3/appy/ui/static/unselect.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      421 2016-10-11 18:35:13.669445 appy-1.0.9/py3/appy/ui/static/upload.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      620 2017-04-03 19:27:08.317931 appy-1.0.9/py3/appy/ui/static/url.png
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)      789 2020-10-07 12:21:22.946334 appy-1.0.9/py3/appy/ui/static/user.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      208 2016-10-11 18:35:14.185452 appy-1.0.9/py3/appy/ui/static/validate.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      314 2016-10-11 18:35:14.181452 appy-1.0.9/py3/appy/ui/static/warning.png
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      854 2020-05-03 10:44:35.869767 appy-1.0.9/py3/appy/ui/static/warning.svg
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12437 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/template.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7763 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/title.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9317 2021-10-26 12:39:34.429114 appy-1.0.9/py3/appy/ui/validate.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.797118 appy-1.0.9/py3/appy/utils/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    15255 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     1775 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/analytics.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    25647 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/client.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     9920 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/dates.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    33372 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/diff.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4888 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/ical.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3847 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/inject.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8204 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/loc.py
+-rw-r--r--   0 gdy999    (1000) gdy999    (1000)     8512 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/mail.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8698 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/path.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    12890 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/pretty.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    17986 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/string.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    18492 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/tables.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     2580 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/url.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7717 2021-10-26 12:39:34.413114 appy-1.0.9/py3/appy/utils/zip.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)       52 2021-10-26 12:39:34.433114 appy-1.0.9/py3/appy/version.py
+drwxrwxr-x   0 gdy999    (1000) gdy999    (1000)        0 2021-10-26 12:39:34.797118 appy-1.0.9/py3/appy/xml/
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     8030 2021-10-26 12:39:34.433114 appy-1.0.9/py3/appy/xml/__init__.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     7000 2021-10-26 12:39:34.433114 appy-1.0.9/py3/appy/xml/cleaner.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     6923 2021-10-26 12:39:34.433114 appy-1.0.9/py3/appy/xml/diff.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     4622 2021-10-26 12:39:34.433114 appy-1.0.9/py3/appy/xml/escape.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)     3677 2021-10-26 12:39:34.433114 appy-1.0.9/py3/appy/xml/extractor.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    13290 2021-10-26 12:39:34.433114 appy-1.0.9/py3/appy/xml/marshaller.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)    14646 2021-10-26 12:39:34.433114 appy-1.0.9/py3/appy/xml/unmarshaller.py
+-rw-rw-r--   0 gdy999    (1000) gdy999    (1000)      903 2021-10-26 12:39:34.433114 appy-1.0.9/setup.py
```

### Comparing `appy-1.0.8/py2/appy/__init__.py` & `appy-1.0.9/py2/appy/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/bin/asksap.py` & `appy-1.0.9/py2/appy/bin/asksap.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/bin/backup.py` & `appy-1.0.9/py2/appy/bin/backup.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/bin/checkldap.py` & `appy-1.0.9/py2/appy/bin/checkldap.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/bin/checklo.py` & `appy-1.0.9/py2/appy/bin/checklo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-'''This script allows to check the UNO interface to LibreOffice'''
+'''Check the UNO interface to LibreOffice'''
 
+# ------------------------------------------------------------------------------
 import os.path, sys, time
+
 import appy
 from appy.shared.utils import executeCommand
 
 # ------------------------------------------------------------------------------
 usage = '''Usage: python checklo.py [port]
 
 If port is not speficied, it defaults to 2002.'''
@@ -60,14 +62,15 @@
         print('CHECK - done in %.2f second(s).' % (time.time() - start))
 
     def run(self):
         # Check PDF generation (and connection to LO)
         success = self.checkRenderPdf()
         if not success:
             print('Error while contacting LibreOffice.')
+            sys.exit(1)
         else:
             # Launch the remaining tests.
             # Check performance of the "optimize tables" functionality
             self.checkOptimizeTables()
 
 # ------------------------------------------------------------------------------
 if __name__ == '__main__':
```

### Comparing `appy-1.0.8/py2/appy/bin/clean.py` & `appy-1.0.9/py2/appy/bin/clean.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/bin/createdebrepo.py` & `appy-1.0.9/py2/appy/bin/createdebrepo.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/bin/eggify.py` & `appy-1.0.9/py2/appy/bin/eggify.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/bin/generate.py` & `appy-1.0.9/py2/appy/bin/generate.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/bin/job.py` & `appy-1.0.9/py2/appy/bin/job.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/bin/new.py` & `appy-1.0.9/py2/appy/bin/new.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/bin/odfgrep.py` & `appy-1.0.9/py2/appy/bin/odfgrep.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,19 @@
                              False: 'No replacement was made.'},
                      False: {True:  '%s matches %d time(s).',
                              False: 'No match found.'}}
 
     # ODF tags used by POD statements or expressions
     podTags = ('office:annotation', 'text:conditional-text', 'text:text-input')
 
+    # Regex used to remove formatting possibly found in notes
+    spanRex = re.compile('<text:span[^>]*>(.*?)</text:span>')
+
     def __init__(self, keyword, fileOrFolder, repl=None, zone=None,
-                 onFileChanged=False):
+                 onFileChanged=False, silent=None):
         # Create a regex from the passed p_keyword
         self.keyword = re.compile(keyword, re.S)
         # The file or folder where to find POD templates
         self.fileOrFolder = fileOrFolder
         # A temp folder where to unzip the POD templates
         self.tempFolder = sutils.getOsTempFolder()
         # (optional) The replacement text
@@ -58,17 +61,22 @@
         self.zoneRex = self.getZoneRex(zone)
         # If called from another program (ie class RamGrep below),
         # p_onFileChanged is a function that will be called every time a file
         # will be modified by this class, with the absolute file name as single
         # argument.
         self.onFileChanged = onFileChanged
         # If called programmatically, we don't want any output on stdout
-        self.silent = bool(onFileChanged)
+        if silent is None:
+            silent = bool(onFileChanged)
+        self.silent = silent
         if self.silent:
             self.messages = []
+        # When replacing, count the number of styled text parts whose style was
+        # removed (see m_cleanNote).
+        self.cleaned = 0
 
     def getZoneRex(self, zone):
         '''Return the regex representing pod zones within content|styles.xml.
            If no p_zone is passed, return None.'''
         if not zone: return
         elif zone != 'pod':
             raise Exception(ZONE_KO)
@@ -96,19 +104,35 @@
 
     def getReplacement(self):
         '''Return p_self.repl and increment p_self.tempCount'''
         # This method is used to count the number of replacements
         self.tempCount += 1
         return self.repl
 
+    def cleanStyle(self, match):
+        '''A styled text part has been found in p_match. Clean it and update the
+           count in p_self.cleaned.'''
+        self.cleaned += 1
+        return match.group(1)
+
+    def cleanNote(self, note):
+        '''Returns the content of this p_note, where any formatting has been
+           removed.'''
+        return self.spanRex.sub(self.cleanStyle, note)
+
     def getZoneReplacement(self, match):
         '''A POD zone has been found in a file, in m_match. Perform replacements
            within this zone.'''
-        r = self.keyword.sub(lambda m: self.getReplacement(), match.group(2))
         tag = match.group(1)
+        content = match.group(2)
+        if tag == 'office:annotation':
+            # Ensure there is no formatting in the note before applying the
+            # replacement.
+            content = self.cleanNote(content)
+        r = self.keyword.sub(lambda m: self.getReplacement(), content)
         return '<%s%s</%s>' % (tag, r, tag)
 
     def greplace(self, name, content, tempFolder):
         '''Replace, in file named p_name lying in p_tempFolder and whose content
            is in p_content as a string, every occurrence of p_self.keyword (a
            regex) by p_self.repl. Return the number of replacements
            performed.'''
@@ -186,14 +210,16 @@
                 for name in filenames:
                     if os.path.splitext(name)[1] in self.toUnzip:
                         nb += self.grepFile(os.path.join(dir, name))
         else:
             self.dump('%s does not exist.' % self.fileOrFolder)
         if not nb:
             self.dump(self.messageTexts[bool(self.repl)][False])
+        if self.cleaned:
+            self.dump('%d styles text part(s) cleaned.' % self.cleaned)
         return nb
 
 # ------------------------------------------------------------------------------
 class RamGrep:
     '''Wrapper around class Grep allowing to use it programmatically, from an
        ODF file given as a StringIO. The result is stored in RamGrep's
        attributes, instead of (a) messages produced on stdout and (b) files
```

### Comparing `appy-1.0.8/py2/appy/bin/odfwalk.py` & `appy-1.0.9/py2/appy/bin/odfwalk.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/bin/restore.py` & `appy-1.0.9/py2/appy/bin/restore.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/bin/zip.py` & `appy-1.0.9/py2/appy/bin/zip.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/bin/zopectl.py` & `appy-1.0.9/py2/appy/bin/zopectl.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/__init__.py` & `appy-1.0.9/py2/appy/fields/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,23 +566,25 @@
         wp = self.specificWritePermission
         if wp and not isinstance(wp, basestring):
             self.writePermission = '%s: Write %s %s' % (appName, prefix, name)
         elif wp and isinstance(wp, basestring):
             self.writePermission = wp
         else:
             self.writePermission = 'write'
-        if (self.type == 'Ref') and not self.isBack and self.back:
-            # We must initialise the corresponding back reference
-            self.back.klass = klass
-            self.back.init(self.back.attribute, self.klass, appName)
-        if self.type in ('List', 'Dict'):
-            for subName, subField in self.fields:
-                fullName = '%s_%s' % (name, subName)
-                subField.init(fullName, klass, appName)
-                subField.name = '%s*%s' % (name, subName)
+        # Field-specific lazy initialisation
+        if self.type == 'Ref':
+            if not self.isBack and self.back:
+                # Initialise the corresponding back reference
+                self.back.klass = klass
+                self.back.init(self.back.attribute, self.klass, appName)
+        elif self.type in ('List', 'Dict'):
+            subs = self.fields
+            if not callable(subs):
+                # Lazy-initialise sub-fields
+                self.lazyInitSubFields(subs, klass, appName)
         elif self.type == 'Switch':
             for case, fields in self.fields:
                 for name, field in fields:
                     field.init(name, klass, appName)
 
     def __repr__(self):
         name = hasattr(self, 'name') and (':%s' % self.name) or ''
@@ -846,25 +848,25 @@
         return res
 
     def computeDefaultLayouts(self):
         '''This method gets the default layouts from a Field or the global
            default field layouts when they are not available.'''
         return self.getDefaultLayouts() or Layouts.defaults(self)
 
-    def getCss(self, layoutType, res, config):
+    def getCss(self, obj, layoutType, res, config):
         '''This method completes the list p_res with the names of CSS files
            that are required for displaying widgets of self's type on a given
            p_layoutType. p_res is not a set because order of inclusion of CSS
            files may be important and may be loosed by using sets.'''
         if layoutType in self.cssFiles:
             for fileName in self.cssFiles[layoutType]:
                 if fileName not in res:
                     res.append(fileName)
 
-    def getJs(self, layoutType, res, config):
+    def getJs(self, obj, layoutType, res, config):
         '''This method completes the list p_res with the names of Javascript
            files that are required for displaying widgets of self's type on a
            given p_layoutType. p_res is not a set because order of inclusion of
            CSS files may be important and may be loosed by using sets.'''
         if layoutType in self.jsFiles:
             for fileName in self.jsFiles[layoutType]:
                 if fileName not in res:
@@ -1337,18 +1339,24 @@
                                  sortOrder=sortOrder, maxResults='NO_LIMIT',
                                  filters=tool.getFilters(class_, filters),
                                  refObject=refObject, refField=refField)
         r = [o.appy() for o in objs.objects]
         tool.log(SEARCH_DONE % len(r))
         return r
 
-    def keepCheckedResults(self, req, objects):
+    def keepCheckedResults(self, req, objects, unchecked=None):
         '''Among p_objects as retrieved via m_getSearchResults, keep only those
            being checked, according to m_getCheckedInfo.'''
-        ids, unchecked = self.getCheckedInfo(req)
+        # If p_unchecked is not None, we already know the IDs of the objects
+        # being unchecked.
+        if unchecked:
+            ids = unchecked
+            unchecked = True
+        else:
+            ids, unchecked = self.getCheckedInfo(req)
         i = len(objects) - 1
         # Remove, from search results, unchecked objects
         while i >= 0:
             if unchecked: remove = objects[i].id in ids
             else:         remove = objects[i].id not in ids
             if remove:
                 del objects[i]
@@ -1459,19 +1467,23 @@
             if isHistorized and previousData: obj.historizeData(previousData)
         else:
             # An inner field. No historization (yet) for it.
             part = ''
             # Retrieve the outer, inner fields and row number
             name, px = rq['px'].rsplit(':', 1)
             outer, inner, i = name.split('*')
+            i = int(i)
             outer = obj.getAppyType(outer)
-            # Update the value
+            # Update the value. Clone the row to ensure the ZODB will detect the
+            # object change. Indeed, rows are instances of not-persistent class
+            # appy.Object.
             value = outer.getValue(obj)
-            row = value[int(i)]
+            row = value[i]
             setattr(row, inner, requestValue)
+            value[i] = row.clone()
             # Store the complete value again on p_obj
             setattr(obj.aq_base, outer.name, value)
         # Update obj's last modification date
         from DateTime import DateTime
         obj.modified = DateTime()
         obj.reindex()
         obj.log('ajax-edited %s%s on %s.' % (self.name, part, obj.id))
```

### Comparing `appy-1.0.8/py2/appy/fields/action.py` & `appy-1.0.9/py2/appy/fields/action.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,30 +50,42 @@
             # been aborted by developer's code.
             pass
         # If we are back from a popup, must we force the back URL?
         if self.field.result == 'redirect':
             self.backFromPopupUrl = msg
 
 # ------------------------------------------------------------------------------
+class Multi:
+    '''Management of muti-actions = actions that execute on a set of objects,
+       and not on a single one.'''
+
+    def __init__(self, back, check):
+        # The DOM node to ajax-refresh once the multi-action has been executed
+        self.back = back
+        # The DOM node storing the un/checked objects onto which the
+        # multi-action must be executed.
+        self.check = check
+
+# ------------------------------------------------------------------------------
 class Action(Field):
     '''An action is a Python method that can be triggered by the user on a
        given Appy class. An action is rendered as a button.'''
     # Action-specific initiator class
     initiator = ActionInitiator
 
     # Getting an action is something special: disable the standard Appy
     # machinery for this.
     customGetValue = True
 
     # PX for viewing the Action button
     pxView = pxCell = Px('''
      <form var="isFake=field.isFake(zobj, _);
                 formId='%s_%s_form' % (zobj.id, name);
-                label=_(field.labelId);
-                multi=multi|False;
+                label=_('label', field=field);
+                multi=multi|None;
                 className=className|zobj.portal_type;
                 inputTitle=field.getInputTitle(zobj, label);
                 inputLabel=field.getInputLabel(label, layoutType);
                 smallButtons=smallButtons|False;
                 css=ztool.getButtonCss(label, smallButtons, field.render)"
            id=":formId" action=":field.getFormAction(zobj, ztool)"
            target=":field.options and 'appyIFrame' or '_self'"
@@ -310,26 +322,27 @@
         if self.options:
             # Submitting the form will lead to creating an object, in order to
             # retrieve action's options.
             return '%s/do' % ztool.absolute_url()
         else:
             # Submitting the form will really trigger the action
             return '%s/onExecuteAction' % zobj.absolute_url()
-    
+
     def getOnClick(self, zobj, name, req, layoutType, q, multi):
         '''Gets the JS code to execute when the action button is clicked'''
         # Determine the ID of the form to submit
         formId = '%s_%s_form' % (zobj.id, name)
         # Determine the back hook and check hook (if multi)
         if multi:
-            back = 'queryResult'
-            check = q(req.search)
+            back = multi.back
+            check = multi.check
         else:
             back = (layoutType == 'cell') and zobj.id or None
-            check = 'null'
+            check = None
+        check = check and q(check) or 'null'
         if not self.options:
             # Determine the parameters for executing the action
             showComment = (self.confirm == 'comment') and 'true' or 'false'
             confirmText = self.getConfirmText(zobj)
             back = back and q(back) or 'null'
             # If the action produces a file, the page will not be refreshed. So
             # the action must remain visible: if, as it is done by default, it
@@ -343,32 +356,53 @@
             # Determine the parameters for creating an options instance
             target = gutils.LinkTarget(klass=self.options,
                                        forcePopup=True, back=back)
             js = '%s; submitForm(%s,null,null,null,%s)' % \
                  (target.onClick, q(formId), check)
         return js
 
+    def getTargetObjects(self, obj, req):
+        '''In the context of a multi-action, retrieve the list of target objects
+           onto which the action must be applied.'''
+        # If semantics indicates that checked objects must be kept, retrieve
+        # these objects.
+        tool = obj.tool
+        ids, unchecked = self.getCheckedInfo(req)
+        if not unchecked:
+            r = []
+            for id in ids:
+                cobj = tool.getObject(id)
+                if cobj: # The object may have been deleted in the meanwhile
+                    r.append(cobj)
+            return r
+        # Get all the potential target objects, from a Search or Ref
+        searchParams = req['searchParams']
+        if searchParams:
+            # Re-trigger the search
+            r = self.getSearchResults(tool.o, req['searchParams'])
+        else:
+            # Get objets from a ref
+            r = getattr(obj, req['fieldName'].split('*',1)[0])
+        # Remove those not being checked in the UI
+        self.keepCheckedResults(req, r, unchecked=ids)
+        return r
+
     def __call__(self, obj, options=None):
         '''Calls the action on p_obj. Returns a tuple (b_success, s_message)'''
         # Get args to give to method(s) in self.action
         args = {}
         # Is that a multi-action? A multi-action is an action to perform on a
         # list of objects instead of a single object.
         req = obj.request
         multi = req.get('multi') == '1'
         if options: args['options'] = options
         if self.confirm == 'comment':
             args['comment'] = req.get('popupComment')
         if multi:
-            # Re-trigger the search to get the list of objects
-            tool = obj.o.getTool()
-            objects = self.getSearchResults(tool, req['searchParams'])
-            # Remove those not being checked in the UI
-            self.keepCheckedResults(req, objects)
-            args['objects'] = objects
+            args['objects'] = self.getTargetObjects(obj, req)
         # Call method(s) in self.action
         if type(self.action) in sutils.sequenceTypes:
             # There are multiple methods
             res = [True, '']
             for act in self.action:
                 actRes = act(obj, **args)
                 if type(actRes) in sutils.sequenceTypes:
@@ -484,8 +518,14 @@
             # msg does not contain a message, but the URL where to redirect
             # the user. Redirecting is different if we are in an Ajax request.
             if hasattr(rq, 'pxContext') and rq.pxContext['ajax']:
                 rq.RESPONSE.setHeader('Appy-Redirect', msg)
                 obj.setMessageCookie()
             else:
                 return obj.goto(msg)
+
+    def getMulti(self, back, check):
+        '''In the context of a multi-action, create and return a Multi instance
+           defining useful info about the action, like the back and check
+           hooks.'''
+        return Multi(back, check)
 # ------------------------------------------------------------------------------
```

### Comparing `appy-1.0.8/py2/appy/fields/boolean.py` & `appy-1.0.9/py2/appy/fields/boolean.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/calendar.py` & `appy-1.0.9/py2/appy/fields/calendar.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,15 +402,17 @@
         # "initValue" is the initial value given to created Total instances
         self.initValue = initValue
 
 # ------------------------------------------------------------------------------
 class Layer:
     '''A layer is a set of additional data that can be activated or not on top
        of calendar data. Currently available for timelines only.'''
-    def __init__(self, name, label, onCell, activeByDefault=False, legend=None):
+
+    def __init__(self, name, label, onCell, activeByDefault=False, legend=None,
+                 merge=False):
         # "name" must hold a short name or acronym, unique among all layers
         self.name = name
         # "label" is a i18n label that will be used to produce the layer name in
         # the user interface.
         self.label = label
         # "onCell" must be a method that will be called for every calendar cell
         # and must return a 3-tuple (style, title, content). "style" will be
@@ -432,14 +434,17 @@
         # to this layer. The method must accept no arg and must return a list of
         # objects (you can use class appy.Object) having these attributes:
         # * name        - the legend item name as shown in the calendar
         # * style       - the content of the "style" attribute that will be
         #                 applied to the little square ("td" tag) for this item;
         # * content     - the content of this "td" (if any).
         self.legend = legend
+        # When p_merge is False, if the layer contains info for a given day, the
+        # base info will be hidden. Else, it will be merged.
+        self.merge = merge
         # Layers will be chained: one layer will access the previous one in the
         # stack via attribute "previous". "previous" fields will automatically
         # be filled by the Calendar.
         self.previous = None
 
     def getCellInfo(self, obj, activeLayers, date, other, events, preComputed):
         '''Get the cell info from this layer or one previous layer when
@@ -795,15 +800,15 @@
                   mayValidate=mayValidate and other.mayValidate();
                   css=other.getCss()">
          <td class=":('tlLeft ' + css).strip()">::tlName</td>
          <!-- A cell in this other calendar -->
          <x for="date in grid"
             var2="inRange=field.dateInRange(date, startDate, endDate)">
           <td if="not inRange"></td>
-          <x if="inRange">::field.getTimelineCell(req, obj, date, actions)</x>
+          <x if="inRange">::field.getTimelineCell(_ctx_, obj, date, actions)</x>
          </x>
          <td class=":('tlRight ' + css).strip()">::tlName</td>
         </tr>
         <!-- The separator between groups of other calendars -->
         <x if="not loop.otherGroup.last">::field.getOthersSep(len(grid)+2)</x>
        </x>
       </tbody>
@@ -978,23 +983,22 @@
      <!-- Validate button, with checkbox for automatic checbox selection -->
      <x if="mayValidate" var2="cbId='%s_auto' % ajaxHookId">
       <input if="mayValidate" type="button" value=":_('validate_events')"
              class="buttonSmall button" style=":url('validate', bg=True)"
              var2="js='validateEvents(%s,%s)' % (q(ajaxHookId), q(month))"
              onclick=":'askConfirm(%s,%s,%s)' % (q('script'), q(js, False), \
                        q(_('validate_events_confirm')))"/>
-      <input type="checkbox" checked="checked" id=":cbId" class="smallbox"/>
+      <input type="checkbox" checked="checked" id=":cbId"/>
       <label lfor=":cbId" class="simpleLabel">:_('select_auto')</label>
      </x>
      <!-- Checkboxes for (de-)activating layers -->
      <x if="field.layers and field.layersSelector">
       <x for="layer in field.layers"
          var2="cbId='%s_layer_%s' % (ajaxHookId, layer.name)">
-       <input type="checkbox" id=":cbId" class="smallbox"
-              checked=":layer.name in activeLayers"
+       <input type="checkbox" id=":cbId" checked=":layer.name in activeLayers"
               onclick=":'switchCalendarLayer(%s, this)' % q(ajaxHookId)"/>
        <label lfor=":cbId" class="simpleLabel">:_(layer.label)</label>
       </x>
      </x>
      <x if="actions"> <!-- Custom actions -->
       <input for="action in actions" type="button" value=":_(action.label)"
              var2="js='calendarAction(%s,%s,comment)' % \
@@ -1484,96 +1488,103 @@
         '''Returns the name of some p_other calendar as must be shown in a
            timeline.'''
         if not self.timelineName:
             return '<a href="%s?month=%s">%s</a>' % \
                    (other.obj.url, month, other.obj.title)
         return self.timelineName(obj, other, month, grid)
 
-    def getCellSelectParams(self, date, actions, cellContent, disable=False):
+    def getCellSelectParams(self, date, content):
         '''For a timeline cell, gets the parameters allowing to (de)select it,
            as a tuple ("onclick", "class") to be used as HTML attributes for
            the cell (td tag).'''
-        if disable or not actions: return '', ''
-        if not cellContent and not self.selectableEmptyCells: return '', ''
+        if not content and not self.selectableEmptyCells: return '', ''
         return ' onclick="onCell(this,\'%s\')"' % date.strftime('%Y%m%d'), \
                ' class="clickable"'
 
     def getColorFor(self, obj, eventType, preCompute):
         '''Gets the background color for a cell containing some p_eventType'''
         colors = self.colors
         if colors is None:
             r = None
         elif isinstance(colors, dict):
             r = colors.get(eventType)
         else: # A method
             r = colors(obj, eventType, preCompute)
         return r
 
-    def getTimelineCell(self, req, obj, date, actions):
+    def buildTimelineCell(self, date, style, title, content, actions,
+                          disableSelect=False):
+        '''Called by m_getTimelineCell to build the final XHTML "td" tag
+           representing the timeline cell.'''
+        style = style and (' style="%s"' % style) or ''
+        title = title and (' title="%s"' % title) or ''
+        content = content or ''
+        if disableSelect or not actions:
+            onClick = css = ''
+        else:
+            onClick, css = self.getCellSelectParams(date, content)
+        return '<td%s%s%s%s>%s</td>' % (onClick, css, style, title, content)
+
+    def getTimelineCell(self, c, obj, date, actions):
         '''Gets the content of a cell in a timeline calendar'''
         # Unwrap some variables from the PX context
-        c = req.pxContext
         date = c['date']; other = c['other']; render = 'timeline'
         allEventNames = c['allEventNames']; activeLayers = c['activeLayers']
         # Get the events defined at that day, in the current calendar
         events = self.getOtherEventsAt(date, other, allEventNames, render,
                                        c['preComputed'], c['gradients'])
-        # In priority we will display info from a layer
+        # Compute the cell attributes
+        style = title = content = None
+        # In priority, get info from layers
         if activeLayers:
             # Walk layers in reverse order
             layer = self.layers[-1]
             info = layer.getCellInfo(obj, activeLayers, date, other, events,
                                      c['preComputed'])
             if info:
                 style, title, content = info
-                style = style and (' style="%s"' % style) or ''
-                title = title and (' title="%s"' % title) or ''
-                content = content or ''
-                onClick, css = self.getCellSelectParams(date, actions, content)
-                return '<td%s%s%s%s>%s</td>' % (onClick, css, style, title,
-                                                content)
+                if not layer.merge:
+                    # Exclusively display the layer info, ignoring the base info
+                    return self.buildTimelineCell(date, style, title,
+                                                  content, actions)
         # Define the cell's style
-        style = self.getCellStyle(obj, date, render, events) or ''
-        if style: style = ' style="%s"' % style
+        style = style or self.getCellStyle(obj, date, render, events)
         # If a timeline cell hides more than one event, put event names in the
         # "title" attribute.
-        title = ''
-        if len(events) > 1:
+        if not title and len(events) > 1:
             title = ', '.join(['%s (%s)' % (\
               allEventNames.get(e.event.eventType) or '?', e.event.timeslot) \
               for e in events])
-            title = ' title="%s"' % title
         # Define its content
-        content = ''
         disableSelect = False
-        if events and c['mayValidate']:
-            # If at least one event from p_events is in the validation schema,
-            # propose a unique checkbox, that will allow to validate or not all
-            # validable events at p_date.
-            for info in events:
-                if info.event.eventType in other.field.validation.schema:
-                    cbId = '%s_%s_%s' % (other.obj.id, other.field.name,
-                                         date.strftime('%Y%m%d'))
-                    totalRows = self.totalRows and 'true' or 'false'
-                    totalCols = self.totalCols and 'true' or 'false'
-                    content = '<input type="checkbox" checked="checked" ' \
-                      'class="smallbox" id="%s" onclick="onCheckCbCell(this,' \
-                      '\'%s\',%s,%s)"/>' % \
-                      (cbId, c['ajaxHookId'], totalRows, totalCols)
-                    # Disable selection if a validation checkbox is there
-                    disableSelect = True
-                    break
-        elif len(events) == 1:
-            # A single event: if not colored, show a symbol. When there are
-            # multiple events, a background image is already shown (see the
-            # "style" attribute), so do not show any additional info.
-            content = events[0].symbol or ''
-        onClick, css = self.getCellSelectParams(date, actions, content,
-                                                disableSelect)
-        return '<td%s%s%s%s>%s</td>' % (onClick, css, style, title, content)
+        if not content:
+            if events and c['mayValidate']:
+                # If at least one event from p_events is in the validation
+                # schema, propose a unique checkbox, that will allow to validate
+                # or not all validable events at p_date.
+                for info in events:
+                    if info.event.eventType in other.field.validation.schema:
+                        cbId = '%s_%s_%s' % (other.obj.id, other.field.name,
+                                             date.strftime('%Y%m%d'))
+                        totalRows = self.totalRows and 'true' or 'false'
+                        totalCols = self.totalCols and 'true' or 'false'
+                        content = '<input type="checkbox" checked="checked" ' \
+                          'class="smallbox" id="%s" onclick="onCheckCbCell(' \
+                          'this,\'%s\',%s,%s)"/>' % \
+                          (cbId, c['ajaxHookId'], totalRows, totalCols)
+                        # Disable selection if a validation checkbox is there
+                        disableSelect = True
+                        break
+            elif len(events) == 1:
+                # A single event: if not colored, show a symbol. When there are
+                # multiple events, a background image is already shown (see the
+                # "style" attribute), so do not show any additional info.
+                content = events[0].symbol
+        return self.buildTimelineCell(date, style, title, content, actions,
+                                      disableSelect=disableSelect)
 
     def getTimelineMonths(self, grid, obj, preComputed):
         '''Given the p_grid of dates, this method returns the list of
            corresponding months.'''
         res = []
         for date in grid:
             if not res:
```

### Comparing `appy-1.0.8/py2/appy/fields/color.py` & `appy-1.0.9/py2/appy/fields/color.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/computed.py` & `appy-1.0.9/py2/appy/fields/computed.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/custom.py` & `appy-1.0.9/py2/appy/fields/custom.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/date.py` & `appy-1.0.9/py2/appy/fields/date.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,21 +224,21 @@
         Field.__init__(self, validator, multiplicity, default, defaultOnEdit,
           show, page, group, layouts, move, indexed, mustIndex, indexValue,
           searchable, specificReadPermission, specificWritePermission, width,
           height, None, colspan, master, masterValue, focus, historized,
           mapping, generateLabel, label, sdefault, scolspan, swidth, sheight,
           persist, False, view, cell, edit, xml, translations)
 
-    def getCss(self, layoutType, res, config):
+    def getCss(self, obj, layoutType, res, config):
         # CSS files are only required if the calendar must be shown
-        if self.calendar: Field.getCss(self, layoutType, res, config)
+        if self.calendar: Field.getCss(self, obj, layoutType, res, config)
 
-    def getJs(self, layoutType, res, config):
+    def getJs(self, obj, layoutType, res, config):
         # Javascript files are only required if the calendar must be shown
-        if self.calendar: Field.getJs(self, layoutType, res, config)
+        if self.calendar: Field.getJs(self, obj, layoutType, res, config)
 
     def getSelectableYears(self, obj):
         '''Gets the list of years one may select for this field'''
         startYear = self.getAttribute(obj, 'startYear')
         r = range(startYear, self.endYear + 1)
         if self.reverseYears: r.reverse()
         return r
```

### Comparing `appy-1.0.8/py2/appy/fields/dict.py` & `appy-1.0.9/py2/appy/fields/dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,20 +62,21 @@
 
     # PX for rendering the dict (shared between pxView and pxEdit)
     pxTable = Px('''
      <table var="isEdit=layoutType == 'edit'" if="isEdit or value"
             id=":'list_%s' % name" class="grid" width=":field.width"
             var2="keys=field.keys(obj);
                   subFields=field.getSubFields(zobj, layoutType);
+                  swidths=field.getWidths(subFields);
                   zobj=oobj|zobj">
       <!-- Header -->
       <tr valign="bottom">
-       <th width=":field.widths[0]"></th>
+       <th width=":swidths[0]"></th>
        <th for="subName, sub in subFields" if="sub"
-           width=":field.widths[loop.subName.nb + 1]">::_(sub.labelId)</th>
+           width=":swidths[loop.subName.nb + 1]">::sub.getListHeader(_ctx_)</th>
       </tr>
       <!-- Rows of data -->
       <x for="rowId, text in keys">:field.pxRow</x>
      </table>''')
 
     def __init__(self, keys, fields, validator=None, multiplicity=(0,1),
       default=None, defaultOnEdit=None, show=True, page='main', group=None,
@@ -102,20 +103,17 @@
         # For a nice rendering of your dict, some of the tuples returned by
         # method "keys" can be "separator rows". The tuple representing such a
         # row must have the form (None, sepRow). "None" indicates that this is
         # not a row of data; "sepRow" must be a SepRow instance (see hereabove)
         # that will determine content and style for the separator row.
         self.keys = keys
 
-    def computeWidths(self, widths):
-        '''Set given p_widths or compute default ones if not given'''
-        if not widths:
-            self.widths = [''] * (len(self.fields) + 1)
-        else:
-            self.widths = widths
+    def getWidths(self, subFields):
+        '''Get the widths to appply to these p_subFields'''
+        return self.widths or [''] * (len(subFields) + 1)
 
     def getStorableValue(self, obj, value, complete=False):
         '''Gets p_value in a form that can be stored in the database'''
         from persistent.mapping import PersistentMapping
         res = PersistentMapping()
         for k, v in value.iteritems():
             res[k] = self.getStorableRowValue(obj, v)
@@ -156,15 +154,15 @@
                     # Force the mapping to take the change into account
                     dbValue[key] = dbValue[key]
             setattr(obj, self.name, dbValue)
 
     def subValidate(self, obj, value, errors):
         '''Validates inner fields'''
         for key, row in value.iteritems():
-            for name, subField in self.fields:
+            for name, subField in self.getSubFields(obj):
                 message = subField.validate(obj, getattr(row, name, None))
                 if message:
                     setattr(errors, '%s*%s' % (subField.name, key), message)
 
     def getDiffSubValue(self, old, new, texts):
         '''Produce a diff between this p_old sub-value and its p_new version.
            p_texts contain precomputed translated texts about the user that
```

### Comparing `appy-1.0.8/py2/appy/fields/file.py` & `appy-1.0.9/py2/appy/fields/file.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/float.py` & `appy-1.0.9/py2/appy/fields/float.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/group.py` & `appy-1.0.9/py2/appy/fields/group.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/hour.py` & `appy-1.0.9/py2/appy/fields/hour.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/info.py` & `appy-1.0.9/py2/appy/fields/info.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/integer.py` & `appy-1.0.9/py2/appy/fields/integer.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/list.py` & `appy-1.0.9/py2/appy/fields/list.py`

 * *Files 10% similar despite different names*

```diff
@@ -109,22 +109,23 @@
     # PX for rendering the list (shared between pxView, pxEdit and pxCell)
     pxTable = Px('''
      <table var="isEdit=layoutType == 'edit';
                  isCell=layoutType == 'cell';
                  tableId='list_%s' % name" if="isEdit or value"
             id=":tableId" width=":field.width" class="grid"
             var2="subFields=field.getSubFields(zobj, layoutType);
+                  swidths=field.getWidths(subFields);
                   totals=field.createTotals(isEdit);
                   showTotals=not isEdit and totals">
       <!-- Header -->
       <thead>
        <tr valign="middle">
         <th if="showTotals"></th>
         <th for="name, sub in subFields" if="sub"
-            width=":field.widths[loop.name.nb]">
+            width=":swidths[loop.name.nb]">
          <x var="field=sub">::field.getListHeader(_ctx_)</x></th>
         <!-- Icon for adding a new row -->
         <th if="isEdit">
          <img class="clickable" src=":url('plus')" title=":_('object_add')"
               onclick=":'insertRow(%s)' % q(tableId)"/>
         </th>
        </tr>
@@ -161,75 +162,106 @@
          show, page, group, layouts, move, False, True, None, False,
          specificReadPermission, specificWritePermission, width, height, None,
          colspan, master, masterValue, focus, historized, mapping,
          generateLabel, label, None, None, None, None, True, False, view, cell,
          edit, xml, translations)
         self.validable = True
         # Tuple of elements of the form (name, Field instance) determining the
-        # format of every element in the list.
+        # format of every element in the list. It can also be a method returning
+        # this tuple. In that case, however, no i18n label will be generated for
+        # the sub-fields: these latters must be created with a value for
+        # attribute "translations".
         self.fields = fields
-        # Force some layouting for sub-fields, if subLayouts are given. So the
-        # one who wants freedom on tuning layouts at the field level must
-        # specify subLayouts=None.
-        if subLayouts:
-            for name, field in self.fields:
-                field.layouts = field.formatLayouts(subLayouts)
+        # Force some layouting for sub-fields, if p_subLayouts are passed. If
+        # you want freedom to tune layouts at the field level, you must specify
+        # p_subLayouts=None.
+        self.subLayouts = subLayouts
         # One may specify the width of every column in the list. Indeed, using
-        # widths and layouts of sub-fields may not be sufficient.
-        self.computeWidths(widths)
+        # widths and layouts at the sub-field level may not be sufficient.
+        self.widths = widths
+        # Initialize sub-fields, if statically known
+        if not callable(fields):
+            self.initSubFields(fields)
         # When deleting a row, must we display a popup for confirming it ?
         self.deleteConfirm = deleteConfirm
         # If you want to specify additional rows representing totals, give in
         # "totalRows" a list of Totals instances (see above).
         self.totalRows = totalRows or []
 
-    def computeWidths(self, widths):
-        '''Set given p_widths or compute default ones if not given'''
-        if not widths:
-            self.widths = [''] * len(self.fields)
-        else:
-            self.widths = widths
+    def initSubFields(self, subFields):
+        '''Initialises sub-fields' attributes'''
+        # Initialise sub-layouts
+        subLayouts = self.subLayouts
+        if subLayouts:
+            for name, field in subFields:
+                field.layouts = field.formatLayouts(subLayouts)
+
+    def lazyInitSubFields(self, subFields, klass, appName):
+        '''Lazy-initialise sub-fields, when known'''
+        # It can be at server startup, if sub-fields are statically defined, or
+        # everytime a List field is solicited, if sub-fields are dynamically
+        # computed.
+        for subName, subField in subFields:
+            fullName = '%s_%s' % (self.name, subName)
+            subField.init(fullName, klass, appName)
+            subField.name = '%s*%s' % (self.name, subName)
+
+    def getWidths(self, subFields):
+        '''Get the widths to appply to these p_subFields'''
+        return self.widths or [''] * len(subFields)
 
     def getDefaultLayouts(self):
         '''Returns default layouts for a List field'''
         # When None is returned, global default layouts will be used
         return self.inGrid() and Layouts.List.g or None
 
     def getField(self, name):
         '''Gets the field definition whose name is p_name'''
         for n, field in self.fields:
             if n == name: return field
 
-    def getSubFields(self, obj, layoutType):
-        '''Returns the sub-fields (name, Field) that are showable among
-           field.fields on the given p_layoutType. Fields that cannot appear in
-           the result are nevertheless present as a tuple (name, None). This
-           way, it keeps a nice layouting of the table.'''
-        res = []
-        for n, field in self.fields:
-            elem = (n, None)
+    def getSubFields(self, obj, layoutType=None):
+        '''Returns the sub-fields, as a list of tuples ~[(s_name, Field)]~,
+           being showable, among p_self.fields on this p_layoutType. Fields that
+           cannot appear in the result are nevertheless present as a tuple
+           (s_name, None). This way, it keeps a nice layouting of the table.'''
+        fields = self.fields
+        if callable(fields):
+            # Dynamically computed fields: get and completely initialise them
+            aobj = obj.appy()
+            fields = self.getAttribute(aobj, 'fields') # Involves caching
+            self.initSubFields(fields)
+            self.lazyInitSubFields(fields, aobj.klass,
+                                   obj.getTool().getAppName())
+        # Stop here if no p_layoutType is passed
+        if layoutType is None: return fields
+        # Retain only sub-fields being showable on this p_layoutType
+        r = []
+        for name, field in fields:
             if field.isShowable(obj, layoutType):
-                elem = (n, field)
-            res.append(elem)
-        return res
+                elem = (name, field)
+            else:
+                elem = (name, None)
+            r.append(elem)
+        return r
 
     def getRequestValue(self, obj, requestName=None):
         '''Concatenates the list from distinct form elements in the request'''
         request = obj.REQUEST
         name = requestName or self.name # A List may be into another List (?)
         prefix = name + '*-row-*' # Allows to detect a row of data for this List
         res = {}
         isDict = True # We manage both List and Dict
         for key in request.keys():
             if not key.startswith(prefix): continue
             # I have found a row: get its index
             row = Object()
             rowId = key.split('*')[-1]
             if rowId == '-1': continue # Ignore the template row
-            for subName, subField in self.fields:
+            for subName, subField in self.getSubFields(obj):
                 keyName = '%s*%s*%s' % (name, subName, rowId)
                 if request.has_key(keyName + subField.getRequestSuffix()):
                     v = subField.getRequestValue(obj, requestName=keyName)
                     setattr(row, subName, v)
             if rowId.isdigit():
                 rowId = int(rowId)
                 isDict = False
@@ -262,15 +294,15 @@
                     req[key] = v
                 i += 1
 
     def getStorableRowValue(self, obj, requestValue):
         '''Gets a ready-to-store Object instance representing a single row,
            from p_requestValue.'''
         res = Object()
-        for name, field in self.fields:
+        for name, field in self.getSubFields(obj):
             if not hasattr(requestValue, name) and \
                not field.isShowable(obj, 'edit'):
                 # Some fields, although present on "edit", may not be part of
                 # the p_requestValue (ie, a "select multiple" with no value at
                 # all will not be part of the POST HTTP request). If we want to
                 # know if the field was in the request or not, we must then
                 # check if it is showable on layout "edit".
@@ -293,35 +325,37 @@
         return [self.getStorableRowValue(obj, v) for v in value]
 
     def getCopyValue(self, obj):
         '''Return a (deep) copy of field value on p_obj''' 
         r = getattr(obj.aq_base, self.name, None)
         if r: return copy.deepcopy(r)
 
-    def getCss(self, layoutType, res, config):
+    def getCss(self, obj, layoutType, res, config):
         '''Gets the CSS required by sub-fields if any'''
-        for name, field in self.fields:
-            field.getCss(layoutType, res, config)
+        for name, field in self.getSubFields(obj, layoutType):
+            if field:
+                field.getCss(obj, layoutType, res, config)
 
-    def getJs(self, layoutType, res, config):
+    def getJs(self, obj, layoutType, res, config):
         '''Gets the JS required by sub-fields if any'''
-        for name, field in self.fields:
-            field.getJs(layoutType, res, config)
+        for name, field in self.getSubFields(obj, layoutType):
+            if field:
+                field.getJs(obj, layoutType, res, config)
 
     def jsDeleteConfirm(self, q, tableId):
         '''Gets the JS code to call when the user wants to delete a row'''
         confirm = self.deleteConfirm and 'true' or 'false'
         return 'deleteRow(%s,this,%s)' % (q(tableId), confirm)
 
     def subValidate(self, obj, value, errors):
         '''Validates inner fields'''
         i = -1
         for row in value:
             i += 1
-            for name, subField in self.fields:
+            for name, subField in self.getSubFields(obj):
                 message = subField.validate(obj, getattr(row, name, None))
                 if message:
                     setattr(errors, '%s*%d' % (subField.name, i), message)
 
     def createTotals(self, isEdit):
         '''When rendering the List field, if total rows are defined, create a
            Total instance for every sub-field for which a total must be
```

### Comparing `appy-1.0.8/py2/appy/fields/multilingual.py` & `appy-1.0.9/py2/appy/fields/multilingual.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/page.py` & `appy-1.0.9/py2/appy/fields/page.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/phase.py` & `appy-1.0.9/py2/appy/fields/phase.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/pod.py` & `appy-1.0.9/py2/appy/fields/pod.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/ref.py` & `appy-1.0.9/py2/appy/fields/ref.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,55 +170,67 @@
              page=pageName, inPopup=inPopup, selectJs=selectJs)</x>
       <x if="not selectable">
        <span style=":showSubTitles and 'display:inline' or 'display:none'"
             name="subTitle" class=":tied.o.getCssFor('subTitle')"
             var="sub=field.getSubTitle(obj, tied)" if="sub">::sub</span>
       </x></x>''')
 
-    # This PX displays buttons for triggering global actions on several linked
-    # objects (delete many, unlink many,...)
+    # Buttons triggering global actions on several linked objects: delete many,
+    # unlink many, etc.
     pxGlobalActions = Px('''
      <div class="globalActions">
+
       <!-- Insert several objects (if in pick list) -->
       <input if="inPickList"
              var2="action='link'; label=_('object_link_many');
                    css=ztool.getButtonCss(label)"
              type="button" class=":css" value=":label"
              onclick=":'onLinkMany(%s,%s,%s)' % \
                         (q(action), q(ajaxHookId), q(batch.start))"
              style=":url('linkMany', bg=True)"/>
+
       <!-- Unlink several objects -->
       <input if="mayUnlink and not selector"
              var2="imgName=linkList and 'unlinkManyUp' or 'unlinkMany';
                    action='unlink'; label=_('object_unlink_many');
                    css=ztool.getButtonCss(label)"
              type="button" class=":css" value=":label"
              onclick=":'onLinkMany(%s,%s,%s)' % \
                         (q(action), q(ajaxHookId), q(batch.start))"
              style=":url(imgName, bg=True)"/>
+
       <!-- Delete several objects -->
       <input if="mayEdit and field.delete and not selector"
              var2="action='delete'; label=_('object_delete_many');
                    css=ztool.getButtonCss(label)"
              type="button" class=":css" value=":label"
              onclick=":'onLinkMany(%s,%s,%s)' % \
                         (q(action), q(ajaxHookId), q(batch.start))"
              style=":url('deleteMany', bg=True)"/>
+
       <!-- Select objects and close the popup -->
       <input if="selector" type="button"
              var="label=_('object_link_many'); css=ztool.getButtonCss(label)"
              value=":label" class=":css" style=":url('linkMany', bg=True)"
              onclick=":'onSelectObjects(%s,%s,%s,%s,%s)' % \
               (q('%s_%s' % (zobj.id, field.name)), q(selector.initiatorHook), \
                q(selector.initiator.url), q(selector.initiatorMode), \
                q(selector.onav))"/>
+
+      <!-- Custom actions -->
+      <x if="not inPopup">
+       <div for="action in field.getActions(obj)"
+            var2="checkHook='%s_%s' % (zobj.id, field.name);
+                  fieldName='%s*%s' % (field.name, action.name); field=action;
+                  multi=action.getMulti(ajaxHookId, checkHook);
+                  smallButtons=True">:action.pxRender</div>
+      </x>
      </div>''')
 
-    # This PX displays icons for triggering actions on some tied object
-    # (edit, delete, etc).
+    # Icons for triggering actions on some tied object (edit, delete, etc)
     pxObjectActions = Px('''
      <div if="field.showActions" class="objectActions"
           style=":'display:%s' % field.actionsDisplay"
           var2="layoutType='buttons';
                 ztied=tied.o;
                 editable=ztied.mayEdit();
                 locked=ztied.isLocked(user, 'main')">
@@ -741,15 +753,15 @@
       sheight=None, sselect=None, persist=True, render='list',
       renderMinimalSep=', ', menuIdMethod=None, menuInfoMethod=None,
       menuUrlMethod=None, menuCss=None, view=None, cell=None, edit=None,
       xml=None, translations=None, showActions='all', actionsDisplay='block',
       showGlobalActions=True, collapsible=False, links=True, viewAdded=True,
       noValueLabel='choose_a_value', noObjectLabel='no_ref',
       addLabel='object_add', filterable=True, supTitle=None, subTitle=None,
-      separator=None):
+      separator=None, actions=None):
         # The class whose tied objects will be instances of
         self.klass = klass
         # Specify "attribute" only for a back reference: it will be the name
         # (a string) of the attribute that will be defined on self's class and
         # will allow, from a linked object, to access the source object.
         self.attribute = attribute
         # If this Ref is "composite", it means that the source object will be
@@ -1099,14 +1111,16 @@
         # a Separator instance (see class above). This method must accept 2
         # args: "previous" and "next", and must return a Separator instance if a
         # separator must be inserted between the "previous" and "next" tied
         # objects. When the first tied object is rendered, the method is called
         # with parameter "previous" being None. Specifying a separator has only
         # sense when p_render is "list".
         self.separator = separator
+        # These p_actions fields will be shown as global actions
+        self.actions = actions
         # Call the base constructor
         Field.__init__(self, validator, multiplicity, default, defaultOnEdit,
           show, page, group, layouts, move, indexed, mustIndex, indexValue,
           searchable, specificReadPermission, specificWritePermission, width,
           height, None, colspan, master, masterValue, focus, historized,
           mapping, generateLabel, label, sdefault, scolspan, swidth, sheight,
           persist, False, view, cell, edit, xml, translations)
@@ -2249,14 +2263,41 @@
         if not self.separator: return ''
         sep = self.separator(obj, previous, next)
         if not sep: return ''
         css = sep.css and ' class="%s"' % sep.css or ''
         return '<tr><td colspan="%d"><div%s>%s</div></td></tr>' % \
                (len(columns), css, sep.translated or obj.translate(sep.label))
 
+    def getActions(self, obj):
+        '''Return the custom actions that must be shown among global actions'''
+        actions = self.actions
+        if not actions: return ()
+        r = []
+        i = 0
+        tool = obj.o.getTool()
+        for action in actions:
+            show = action.show
+            if callable(show): show = show(obj)
+            if show:
+                i += 1
+                # Lazy-init the action if not done yet
+                if not hasattr(action, 'name'):
+                    action.init('action%d' % i, obj.klass, tool.getAppName())
+                r.append(action)
+        return r
+
+    def getField(self, subName):
+        '''Returns the sub-field whose name in p_subName, among
+           p_self.actions.'''
+        actions = self.actions
+        if not actions: return
+        for action in actions:
+            if subName == action.name:
+                return action
+
 def autoref(klass, field):
     '''klass.field is a Ref to p_klass. This kind of auto-reference can't be
        declared in the "normal" way, like this:
 
        class A:
            attr1 = Ref(A)
```

### Comparing `appy-1.0.8/py2/appy/fields/rich.py` & `appy-1.0.9/py2/appy/fields/rich.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
             if isinstance(v, int): sv = str(v)
             elif isinstance(v, bool): sv = str(v).lower()
             elif isinstance(v, dict): sv = str(v)
             else: sv = '"%s"' % v
             ck.append('%s: %s' % (k, sv))
         return ', '.join(ck)
 
-    def getJs(self, layoutType, r, config):
+    def getJs(self, obj, layoutType, r, config):
         if layoutType not in ('edit', 'view'): return
         # Compute the URL to ckeditor CDN
         ckUrl = Rich.cdnUrl % (config.ckVersion, config.ckDistribution)
         if ckUrl not in r: r.append(ckUrl)
 
     def getJsInit(self, obj, language):
         '''Gets the Javascript init code for displaying ckeditor for this field.
```

### Comparing `appy-1.0.8/py2/appy/fields/search.py` & `appy-1.0.9/py2/appy/fields/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,16 +66,16 @@
     # All available predefined concrete modes
     concrete = ('list', 'grid', 'calendar')
 
     # The list of custom actions that can be triggered on search results
     pxActions = Px('''
      <table>
       <tr><td for="action in actions"
-            var2="field=action; fieldName=field.name;
-                  multi=True">:action.pxRender</td></tr>
+            var2="multi=action.getMulti('queryResult', req['search']);
+                  field=action; fieldName=field.name">:action.pxRender</td></tr>
      </table>''')
 
     @staticmethod
     def get(klass, className, uiSearch, inPopup, tool, req, dir):
         '''Create and return the Mode instance corresponding to the current
            result mode to apply to a list of p_klass instances.'''
         name = req.get('resultMode') or uiSearch.getModes(klass, tool)[0]
@@ -377,41 +377,64 @@
     def __init__(self, *args):
         List.__init__(self, *args)
         # Extract the gridder defined on p_self.klass or create a default one
         self.gridder = getattr(self.klass, 'gridder', None) or Gridder()
 
 class Calendar(Mode):
     '''Displays search results in a monthly calendar view'''
+
     px = Px('''<x var="layoutType='view';
                        field=tool.getField('calendar')">:field.pxView</x>''')
 
+    # Formats for keys representing dates
+    dayKey = '%Y%m%d'
+
+    # Format for representing hours in the UI
+    hourFormat = '%H:%M'
+
     def __init__(self, *args):
         Mode.__init__(self, *args)
         # For this calendar view to work properly, objects to show inside it
-        # must have the following attributes:
+        # must have the following fields:
         # ----------------------------------------------------------------------
         # date    | an indexed and required Date field with format =
         #         | Date.WITH_HOUR storing the object's start date and hour;
         # ----------------------------------------------------------------------
         # endDate | a not necessarily required Date field with format =
         #         | Date.WITH_HOUR storing the object's end date and hour.
         # ----------------------------------------------------------------------
-        # Optionally, if objects define the following attributes, special icons
-        # indicating repeated events will be shown.
+        # Optionnally, if you want to use index "months" (we advice you to do
+        # so), an indexed Computed field with this name, whose attribute p_index
+        # must be "TextIndex", must also be defined (see details in m_init
+        # below).
+        # ----------------------------------------------------------------------
+        # Optionally, too, if objects define the following attributes, special
+        # icons indicating repeated events will be shown.
         # ----------------------------------------------------------------------
         # successor   | Ref field with multiplicity = (0,1), allowing to
         #             | navigate to the next object in the list (for a repeated
         #             | event);
         # ----------------------------------------------------------------------
         # predecessor | Ref field with multiplicity = (0,1), allowing to
         #             | navigate to the previous object in the list.
         #             | "predecessor" must be the back ref of field "successor"
         #             | hereabove.
         # ----------------------------------------------------------------------
 
+    def getMonthIndex(self):
+        '''Deduce, from p_self.klass, what is the month index to use'''
+        # Is there, on p_self.klass, a field name "months" ?
+        months = getattr(self.klass, 'months', None)
+        if not months: return 'date'
+        if months.type == 'Computed' and months.indexed == 'TextIndex':
+            r = 'months'
+        else:
+            r = 'date'
+        return r
+
     def init(self, req, dir):
         '''Creates a stub calendar field'''
         Mode.init(self, req, dir)
         # Always consider the result as not empty. This way, the calendar is
         # always shown, even if no object is visible.
         self.empty = False
         # The matched objects, keyed by day. For every day, a list of entries to
@@ -428,20 +451,73 @@
         #  "end"    | the object started at a previous day and ends at this day.
         #           | Display its title and a sign indicating this fact;
         # ----------------------------------------------------------------------
         #  "pass"   | The object started at a previous day and ends at a future
         #           | day.
         # ----------------------------------------------------------------------
         self.objects = {} # ~{s_YYYYmmdd: [(s_entryType, Object)]}~
-        # Formats for keys representing dates
-        self.dayKey = '%Y%m%d'
-        # Format for representing hours in the UI
-        self.hourFormat = '%H:%M'
         # If filters are defined from a list mode, get it
         self.filters = self.tool.getFilters(self.klass)
+        # The name of the index to use to restrict the search to the currently
+        # shown month. If p_self.klass defines a Computed indexed TextIndex
+        # field named "months", this index will be used. Else, index "date" will
+        # be used. These 2 indexes are described hereafter.
+        # ----------------------------------------------------------------------
+        # "date"   | This index is expected to define the (start) date of the
+        #          | objects to search. So, the search will match any object
+        #          | whose (start) date is included in the range of dates
+        #          | defined by the currently shown month. Recall that this
+        #          | range may be larger than the month itself: because complete
+        #          | weeks are shown, some days from the previous and next
+        #          | months may be present, too.
+        #          |
+        #          | While this index is the easiest to implement, it has the
+        #          | following problem: objects spanning several days (by using
+        #          | fields "date" and "endate") and whose start date is not
+        #          | among the range of visible dates, will not be part of the
+        #          | result. This is why an alternate index named "month' is
+        #          | also proposed (see below).
+        # ----------------------------------------------------------------------
+        # "months" | When using index "months", every object is expected to
+        #          | hold, in a Computed indexed TextIndex field named "months",
+        #          | the space-separated list of months the object crosses
+        #          | (every crossing month must be represented as a string of
+        #          | the form YYYYmm). "Crossing a month" means: there must be a
+        #          | not-empty intersection between the range of visible days
+        #          | for this month, and the object's range of days. For objects
+        #          | defining no end date, this range is reduced to a unique day
+        #          | (defined by field "date").
+        #          |
+        #          | Because this list of crossing months is relatively complex
+        #          | to produce, Appy provides a function that computes it:
+        #          |
+        #          |           appy.shared.dates.getCalendarMonths
+        #          |
+        #          | Here is a complete example of a Appy class using index
+        #          | "months".
+        #          |
+        #          | from appy.shared.dates import getCalendarMonths
+        #          |
+        #          | class Event:
+        #          |     ...
+        #          |     date    = Date(format=Date.Date.WITH_HOUR,
+        #          |                    multiplicity=(1,1), indexed=True, ...)
+        #          |     endDate = Date(format=Date.Date.WITH_HOUR,
+        #          |                    indexed=True, ...)
+        #          |     ...
+        #          |     def computeMonths(self):
+        #          |         '''Compute the months crossed by p_self'''
+        #          |         # p_self.endDate may be None
+        #          |         return ' '.join(getCalendarMonths(self.date,
+        #          |                                           self.endDate))
+        #          |
+        #          |     months  = Computed(method=computeMonths,
+        #          |                        indexed='TextIndex', show=False)
+        # ----------------------------------------------------------------------
+        self.monthIndex = self.getMonthIndex()
 
     def updateAjaxParameters(self, params):
         '''Grid-specific ajax parameters'''
         # If filters are in use, carry them
         if self.filters:
             params['filters'] = self.filters
 
@@ -466,69 +542,94 @@
            @key p_dateKey.'''
         r = self.objects
         if dateKey not in r:
             r[dateKey] = [entry]
         else:
             r[dateKey].append(entry)
 
-    def addEntries(self, obj):
+    def addEntries(self, obj, gridFirst, gridLast):
         '''Add, in self.objects, entries corresponding to p_obj. If p_obj spans
            a single day, a single entry of the form ("start", p_obj) is added at
            the key corresponding to this day. Else, a series of entries are
            added, each of the form (s_entryType, p_obj), with the same object,
-           for every day in p_obj's timespan.
-
-           For example, for an p_obj starting at "1975/12/11 12:00" and ending
-           at "1975/12/13 14:00" will produce the following entries:
-              key "19751211"  >  value ("start+", obj)
-              key "19751212"  >  value ("pass", obj)
-              key "19751213"  >  value ("end", obj)
-        '''
+           for every day in p_obj's timespan.'''
+        # For example, for an p_obj starting at "1975/12/11 12:00" and ending at
+        # "1975/12/13 14:00", m_addEntries will produce the following entries:
+        #      key "19751211"  >  value ("start+", obj)
+        #      key "19751212"  >  value ("pass", obj)
+        #      key "19751213"  >  value ("end", obj)
+        # ~~~
         # Get p_obj's start and end dates
+        fmt = Calendar.dayKey
         start = obj.date
-        startKey = start.strftime(self.dayKey)
+        startKey = start.strftime(fmt)
         end = obj.endDate
-        endKey = end and end.strftime(self.dayKey) or None
+        endKey = end and end.strftime(fmt) or None
         # Shorthand for self.objects
         r = self.objects
-        if not endKey or (endKey == startKey):
+        if not endKey or endKey == startKey:
             # A single entry must be added for p_obj, at the start date
             self.addEntry(startKey, ("start", obj))
         else:
+            # Insert one event per day, provided the events are in the grid
+            # ~~~
             # Add one entry at the start day
-            self.addEntry(startKey, ("start+", obj))
-            # Add "pass" entries for every day between the start and end days
-            next = start + 1
-            nextKey = next.strftime(self.dayKey)
-            while nextKey != endKey:
+            if start >= gridFirst:
+                self.addEntry(startKey, ("start+", obj))
+                next = start + 1
+            else:
+                # Ignore any day between v_start and p_gridFirst
+                next = gridFirst
+            # Add "pass" entries for every day between the event's start and end
+            # dates.
+            nextKey = next.strftime(fmt)
+            while nextKey != endKey and next <= gridLast:
                 # Add a "pass" event
                 self.addEntry(nextKey, ('pass', obj))
                 # Go the the next day
                 next += 1
-                nextKey = next.strftime(self.dayKey)
+                nextKey = next.strftime(fmt)
             # Add an "end" entry at the end day
-            self.addEntry(endKey, ('end', obj))
+            if end <= gridLast:
+                self.addEntry(endKey, ('end', obj))
 
     def search(self, first, grid):
-        '''Performs the query, limited to the date range defined by p_grid'''
-        # Performs the query, restricted to the visible date range
-        last = DateTime(grid[-1][-1].strftime('%Y/%m/%d 23:59:59'))
-        dateSearch = Search(date=(first, last), sortBy='date', sortOrder='asc')
-        res = self.tool.executeQuery(self.className,
-          search=self.uiSearch.search, maxResults='NO_LIMIT',
-          search2=dateSearch, filters=self.filters)
+        '''Performs the search, restricted to the date range defined by
+           p_grid.'''
+        # # The first date in the p_grid, that may be earlier than the p_first
+        # day of the month.
+        gridFirst = grid[0][0]
+        # The last date in the grid, calibrated
+        gridLast = DateTime(grid[-1][-1].strftime('%Y/%m/%d 23:59:59'))
+        # Get the search parameters being specific to the range of dates
+        params = {'sortBy':'date', 'sortOrder':'asc'}
+        if self.monthIndex == 'date':
+            # Define the search based on every event's (start) date.
+            # ~~~
+            # As first date, prefer the first visible date in the p_grid instead
+            # of the p_first day of the month.
+            params['date'] = gridFirst, gridLast
+        else: # p_self.monthIndex is "months"
+            # Define the search based on index "months"
+            params['months'] = first.strftime('%Y%m')
+        # Create a Search instance for the search-related parameters
+        dateSearch = Search(**params)
+        # Perform the search
+        r = self.tool.executeQuery(self.className, search=self.uiSearch.search,
+                                   maxResults='NO_LIMIT', search2=dateSearch,
+                                   filters=self.filters)
         # Produce, in self.objects, the dict of matched objects
-        for zobj in res.objects:
-            self.addEntries(zobj.appy())
+        for zobj in r.objects:
+            self.addEntries(zobj.appy(), gridFirst, gridLast)
 
     def dumpObjectsAt(self, date):
         '''Returns info about the object(s) that must be shown in the cell
            corresponding to p_date.'''
         # There may be no object dump at this date
-        dateStr = date.strftime(self.dayKey)
+        dateStr = date.strftime(Calendar.dayKey)
         if dateStr not in self.objects: return
         # Objects exist
         r = []
         types = self.entryTypes
         url = self.tool.getIncludeUrl
         for entryType, obj in self.objects[dateStr]:
             # Dump the event hour and title. The back hook allows to refresh the
```

### Comparing `appy-1.0.8/py2/appy/fields/select.py` & `appy-1.0.9/py2/appy/fields/select.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,27 +32,42 @@
             'Select field.'
 
 # ------------------------------------------------------------------------------
 class Selection:
     '''If you want to have dynamically computed possible values for a Select
        field, use a Selection instance.'''
 
-    def __init__(self, methodName):
+    def __init__(self, methodName, single=None):
         # p_methodName must be the name of a method that will be called every
         # time Appy will need to get the list of possible values for the related
         # field. It must correspond to an instance method of the class defining
         # the related field. This method accepts no argument and must return a
         # list (or tuple) of pairs (lists or tuples): (id, text), where "id" is
         # one of the possible values for the field, and "text" is the value as
         # will be shown on the screen. You can use self.translate within this
         # method to produce an i18n version of "text" if needed.
         self.methodName = methodName
 
+        # While the method whose name is p_methodName is called on edit and
+        # filter layouts to list the possible values to select, the method you
+        # specify in p_single allows to produce the translated text for a single
+        # value. It accepts a single arg, being one of the values as stored by
+        # the select field, and must return its translated text. If you don't
+        # specify a p_single method, p_methodName will be used instead, but
+        # useless processing will take place, because p_method produces texts
+        # for the complete list of possible values. Moreover, a stored select
+        # value may not be among the list of values as returned by p_method
+        # anymore.
+        self.single = single
+
     def getText(self, obj, value, field, language=None):
         '''Gets the text that corresponds to p_value'''
+        # Use method p_single if specified
+        if self.single: return self.single(obj.appy(), value)
+        # Use p_self.methodName
         if language:
             withTranslations = language
         else:
             withTranslations = True
         vals = field.getPossibleValues(obj, ignoreMasterValues=True,\
                                        withTranslations=withTranslations)
         for v, text in vals:
@@ -301,15 +316,18 @@
             if master.valueIsInRequest(obj, req):
                 # ... from the request if available
                 requestValue = master.getRequestValue(obj)
                 masterValues = master.getStorableValue(obj, requestValue,
                                                        complete=True)
             elif not className:
                 # ... or from the database if we are editing an object
-                masterValues = master.getValue(obj)
+                if master.type == 'Ref':
+                    masterValues = master.getValue(obj, noListIfSingleObj=True)
+                else:
+                    masterValues = master.getValue(obj)
             else:
                 # We don't have any master value
                 masterValues = None
             # Get possible values by calling self.masterValue
             if masterValues:
                 values = self.masterValue(aobj, masterValues)
             else:
```

### Comparing `appy-1.0.8/py2/appy/fields/string.py` & `appy-1.0.9/py2/appy/fields/string.py`

 * *Files 0% similar despite different names*

```diff
@@ -1095,16 +1095,16 @@
             return 'ListIndex'
         elif self.format == String.TEXT:
             return 'TextIndex'
         elif self.format == String.XHTML:
             return 'XhtmlIndex'
         return Field.getIndexType(self)
 
-    def getJs(self, layoutType, res, config):
-        if (self.format == String.XHTML) and (layoutType in ('edit', 'view')):
+    def getJs(self, obj, layoutType, res, config):
+        if self.format == String.XHTML and layoutType in ('edit', 'view'):
             # Compute the URL to ckeditor CDN
             ckUrl = String.cdnUrl % (config.ckVersion, config.ckDistribution)
             if ckUrl not in res: res.append(ckUrl)
 
     def getCaptchaChallenge(self, session, minLength=5, maxLength=9):
         '''Returns a Captcha challenge in the form of a dict. At key "text",
            value is a string that the user will be required to re-type, but
```

### Comparing `appy-1.0.8/py2/appy/fields/switch.py` & `appy-1.0.9/py2/appy/fields/switch.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/text.py` & `appy-1.0.9/py2/appy/fields/text.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/translations.py` & `appy-1.0.9/py2/appy/fields/translations.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/fields/workflow.py` & `appy-1.0.9/py2/appy/fields/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 # Appy is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License along with
 # Appy. If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------------
-import types, string, copy
+import copy
+
 from group import Group
 from appy.px import Px
-from appy.shared.utils import sequenceTypes
 from appy.gen.utils import User
+from appy.shared.utils import sequenceTypes
 
 # Default Appy permissions -----------------------------------------------------
 r, w, d = ('read', 'write', 'delete')
 emptyDict = {}
 class WorkflowException(Exception): pass
 
 # ------------------------------------------------------------------------------
@@ -102,14 +103,18 @@
         for permission, roles in self.permissions.iteritems():
             if isinstance(roles, basestring) or isinstance(roles, Role):
                 role = self.getRole(roles)
                 self.permissions[permission] = {role.name: role}
             elif isinstance(roles, dict):
                 for name, role in roles.iteritems():
                     roles[name] = self.getRole(role)
+            elif callable(roles):
+                # v_roles is a method: it is not possible to standardize it. It
+                # will be called at check time.
+                pass
             else:
                 # "roles" is a list or tuple, or None (nobody may have this
                 # permission).
                 d = {}
                 if roles is not None:
                     for role in roles:
                         role = self.getRole(role)
@@ -123,15 +128,17 @@
            instance or a list of names and/or Role instances. If p_permissions
            is specified, roles are added to those permissions only. Else, roles
            are added for every permission within self.permissions.'''
         # Standardize parameters
         if type(roles) not in sequenceTypes: roles = (roles,)
         if isinstance(permissions, basestring): permissions = (permissions,)
         for perm, existingRoles in self.permissions.iteritems():
-            if permissions and (perm not in permissions): continue
+            if permissions and perm not in permissions: continue
+            # It is not possible to add p_roles if v_existingRoles is a method
+            if callable(existingRoles): continue
             for role in roles:
                 # Do nothing if "role" is already among existing roles
                 name = isinstance(role, basestring) and role or role.name
                 if name in existingRoles: continue
                 # Add the role for this permission
                 existingRoles[name] = self.getRole(role)
```

### Comparing `appy-1.0.8/py2/appy/gen/__init__.py` & `appy-1.0.9/py2/appy/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/authenticate.py` & `appy-1.0.9/py2/appy/gen/authenticate.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,17 +123,20 @@
         # The authentication context in itself (a short identifier)
         req.authContext = ctx
         # Its human-readable name
         req.authContextName = self.getName(tool, ctx)
         # The corresponding object, if any
         req.authObject = self.getObject(tool, ctx)
 
-    def isMandatory(self, tool):
+    def isMandatory(self, tool, authenticate=False):
         '''When authentication contexts are activated, is the user forced to
            choose one ?'''
+        # Not if the user must be p_authenticate(d) and it is impossible to
+        # choose any context.
+        if authenticate and not tool.config.authContext.chooseOnLogin: return
         return True
 
     def switchContext(self, tool):
         '''Is the user allowed to switch context once logged ?'''
         return True
 
     def getContexts(self, tool):
```

### Comparing `appy-1.0.8/py2/appy/gen/descriptors.py` & `appy-1.0.9/py2/appy/gen/descriptors.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,15 +329,18 @@
         # Add the label for the confirm message if relevant
         if self.appyType.addConfirm:
             label = '%s_%s_addConfirm' % (self.classDescr.name, self.fieldName)
             self.i18n(label, po.CONFIRM, nice=False)
 
     def walkList(self):
         '''Generate List-specific i18n labels'''
-        for name, field in self.appyType.fields:
+        subFields = self.appyType.fields
+        # Do not generate anything if the list of sub-fields is dynamic
+        if callable(subFields): return
+        for name, field in subFields:
             if not self.mustGenerateLabels(field): continue
             prefix = '%s_%s_%s' % (self.classDescr.name, self.fieldName, name)
             self.generateLabels(field, prefix, forceLabel=True)
     walkDict = walkList # Same i18n labels for Dict field
 
     def walkCalendar(self):
         '''Generate Calendar-specific i18n labels'''
```

### Comparing `appy-1.0.8/py2/appy/gen/generator.py` & `appy-1.0.9/py2/appy/gen/generator.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/indexer.py` & `appy-1.0.9/py2/appy/gen/indexer.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/installer.py` & `appy-1.0.9/py2/appy/gen/installer.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/layout.py` & `appy-1.0.9/py2/appy/gen/layout.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/mail.py` & `appy-1.0.9/py2/appy/gen/mail.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/migrator.py` & `appy-1.0.9/py2/appy/gen/migrator.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/mixins/TestMixin.py` & `appy-1.0.9/py2/appy/gen/mixins/TestMixin.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/mixins/ToolMixin.py` & `appy-1.0.9/py2/appy/gen/mixins/ToolMixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1258,19 +1258,19 @@
                 self.log(USER_NOT_FOUND % login, noUser=True, type='error')
                 self._disableUser(req)
                 return tool.search1('User', noSecurity=True, login='anon')
         if not user: return
         login = user.login # May have been transformed by a source
         # Authenticate the user if required. In the case of SSO, authentication
         # has already been performed by the reverse proxy.
-        if authenticate and (place != 'sso'):
-            if (user.state == 'inactive') or \
-               (not user.checkPassword(password)) or \
-               (cfg.authContext and cfg.authContext.isMandatory(tool) and \
-                not ctx and (place != 'basic')):
+        if authenticate and place != 'sso':
+            if user.state == 'inactive' or not user.checkPassword(password) or \
+               (cfg.authContext and \
+                cfg.authContext.isMandatory(tool, authenticate) and \
+                not ctx and place != 'basic'):
                 # Disable the user
                 self._disableUser(req)
                 return
             # Create an authentication cookie for this user
             gutils.writeCookie(login, password, ctx, req)
         # Cache the user and some precomputed values, for performance
         req.user = user
```

### Comparing `appy-1.0.8/py2/appy/gen/mixins/__init__.py` & `appy-1.0.9/py2/appy/gen/mixins/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1021,17 +1021,17 @@
         if refresh: klass = self.getClass(reloaded=True)
         for field in (fields or self.getAllAppyTypes()):
             if refresh: field = field.reload(klass, self)
             if field.page.name != pageName: continue
             if not field.isShowable(self, layoutType): continue
             if collectCssJs:
                 if css == None: css = []
-                field.getCss(layoutType, css, config)
+                field.getCss(self, layoutType, css, config)
                 if js == None: js = []
-                field.getJs(layoutType, js, config)
+                field.getJs(self, layoutType, js, config)
             if not field.group:
                 res.append(field)
             else:
                 group = field.getGroup(layoutType)
                 if not group:
                     res.append(field)
                 else:
@@ -1065,16 +1065,16 @@
            on p_layoutType.'''
         # Lists css and js below are not sets, because order of Javascript
         # inclusion can be important, and this could be losed by using sets.
         css = []
         js = []
         config = self.getProductConfig(True)
         for field in fields:
-            field.getCss(layoutType, css, config)
-            field.getJs(layoutType, js, config)
+            field.getCss(self, layoutType, css, config)
+            field.getJs(self, layoutType, js, config)
         res['css'] = css
         res['js'] = js
 
     def getCssFor(self, elem):
         '''Gets the name of the CSS class to use for styling some p_elem. If
            self's class does not define a dict or method named "styles", the
            defaut CSS class to use will be named p_elem.'''
@@ -1673,15 +1673,20 @@
            p_permission on this object.'''
         state = self.State(name=False)
         if permission not in state.permissions:
             wf = self.getWorkflow().__name__
             raise Exception('Permission "%s" not in permissions dict for ' \
                             'state %s.%s' % \
                             (permission, wf, self.State(name=True)))
-        return state.permissions[permission]
+        r = state.permissions[permission]
+        # If v_r is a method, it *must* return Role instances
+        if callable(r):
+            wf = self.getWorkflow()
+            r = r(wf, self.appy(), permission)
+        return r
 
     def getLocalRolesOnly(self):
         '''Must we only take care of local roles when checking security on
            p_self ?'''
         try:
             r = self.workflow_history['appy'][0].get('local', False)
         except AttributeError:
```

### Comparing `appy-1.0.8/py2/appy/gen/model.py` & `appy-1.0.9/py2/appy/gen/model.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/monitoring.py` & `appy-1.0.9/py2/appy/gen/monitoring.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/navigate.py` & `appy-1.0.9/py2/appy/gen/navigate.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/po.py` & `appy-1.0.9/py2/appy/gen/po.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/templates/Class.pyt` & `appy-1.0.9/py2/appy/gen/templates/Class.pyt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/templates/Page.odt` & `appy-1.0.9/py2/appy/gen/templates/Page.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/templates/__init__.pyt` & `appy-1.0.9/py2/appy/gen/templates/__init__.pyt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/templates/config.pyt` & `appy-1.0.9/py2/appy/gen/templates/config.pyt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/templates/testAll.pyt` & `appy-1.0.9/py2/appy/gen/templates/testAll.pyt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/templates/wrappers.pyt` & `appy-1.0.9/py2/appy/gen/templates/wrappers.pyt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/tr/Appy.pot` & `appy-1.0.9/py2/appy/gen/tr/Appy.pot`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/tr/ar.po` & `appy-1.0.9/py2/appy/gen/tr/ar.po`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/tr/de.po` & `appy-1.0.9/py2/appy/gen/tr/de.po`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/tr/en.po` & `appy-1.0.9/py2/appy/gen/tr/en.po`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/tr/es.po` & `appy-1.0.9/py2/appy/gen/tr/es.po`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/tr/fr.po` & `appy-1.0.9/py2/appy/gen/tr/fr.po`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/tr/it.po` & `appy-1.0.9/py2/appy/gen/tr/it.po`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/tr/nl.po` & `appy-1.0.9/py2/appy/gen/tr/nl.po`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/action.png` & `appy-1.0.9/py2/appy/gen/ui/action.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/appy.css` & `appy-1.0.9/py2/appy/gen/ui/appy.css`

 * *Files 0% similar despite different names*

```diff
@@ -260,31 +260,24 @@
 .tabSep { border-bottom: |tabBorder|; padding-bottom: 1px }
 .tab { background-color: #f1eeee }
 
 .language {color: #555555; font-size: 7pt; border: grey 1px solid; padding: 2px;
            margin: 0 2px 0 4px; font-family: monospace }
 .highlight { background-color: yellow }
 .highlightRow { font-weight: bold; background-color: yellow; opacity: 0.6 }
-.globalActions { margin-bottom: 4px }
+.globalActions { display:flex; margin-bottom: 4px }
 .objectActions { margin: 7px 4px }
 .smallbox { margin: 0; vertical-align: middle }
 @keyframes blinkingBg {
-  0% { background-color: white; color: grey }
-  50% { background-color: grey; color: white }
-  100% { background-color: white; color: grey }
-}
-@-webkit-keyframes blinkingBg {
-  0% { background-color: white; color: grey }
-  50% { background-color: grey; color: white }
-  100% { background-color: white; color: grey }
-}
-.blinkBg {
-  -webkit-animation: blinkingBg 1s infinite;
-  animation: blinkingBg 1s infinite;
+  0%   { background-color: white; color: grey  }
+  50%  { background-color: grey ; color: white }
+  100% { background-color: white; color: grey  }
 }
+.blinkBg { animation: blinkingBg 1s infinite }
+.ct { color:white; font-family:sans-serif; mix-blend-mode:difference }
 .legend { font-size: 90%; color: grey }
 .legendRight { float: right; margin-left: 10px }
 .legend td { padding: 1px 0px; border: 0 !important }
 .footer { width:100%; font-size: 95%; height: 14px; padding: 0.5em 0;
   position: absolute; bottom: 0; background-color: #CBCBC9;
   border-top: 3px solid #e4e4e4; text-align:right }
 .footerWide { position: fixed }
```

### Comparing `appy-1.0.8/py2/appy/gen/ui/appy.js` & `appy-1.0.9/py2/appy/gen/ui/appy.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/back.png` & `appy-1.0.9/py2/appy/gen/ui/back.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/banner.png` & `appy-1.0.9/py2/appy/gen/ui/banner.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/bannerrtl.png` & `appy-1.0.9/py2/appy/gen/ui/bannerrtl.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/calendar.gif` & `appy-1.0.9/py2/appy/gen/ui/calendar.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/calendar.js` & `appy-1.0.9/py2/appy/gen/ui/calendar.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/ckeditor/config.js` & `appy-1.0.9/py2/appy/gen/ui/ckeditor/config.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/ckeditor/contents.css` & `appy-1.0.9/py2/appy/gen/ui/ckeditor/contents.css`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/config.png` & `appy-1.0.9/py2/appy/gen/ui/config.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/docFrozen.png` & `appy-1.0.9/py2/appy/gen/ui/docFrozen.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/docx.png` & `appy-1.0.9/py2/appy/gen/ui/docx.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/docxFrozen.png` & `appy-1.0.9/py2/appy/gen/ui/docxFrozen.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/email.png` & `appy-1.0.9/py2/appy/gen/ui/email.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/external.png` & `appy-1.0.9/py2/appy/gen/ui/external.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/fake.png` & `appy-1.0.9/py2/appy/gen/ui/fake.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/favicon.ico` & `appy-1.0.9/py2/appy/gen/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/folder.gif` & `appy-1.0.9/py2/appy/gen/ui/folder.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/funnel.png` & `appy-1.0.9/py2/appy/gen/ui/funnel.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/help.png` & `appy-1.0.9/py2/appy/gen/ui/help.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/calendar-blue.css` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/calendar-blue.css`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/calendar-setup.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/calendar-setup.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/calendar.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/calendar.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-af.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-af.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-al.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-al.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-bg.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-bg.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-big5-utf8.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-big5-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-big5.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-big5.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-br.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-br.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-ca.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-ca.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-cs-utf8.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-cs-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-cs-win.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-cs-win.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-da.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-da.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-de.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-de.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-du.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-du.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-el.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-el.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-en.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-en.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-es.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-es.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-eu.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-eu.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-fi.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-fi.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-fr.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-fr.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-he-utf8.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-he-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-hr-utf8.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-hr-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-hr.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-hr.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-hu.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-hu.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-it.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-it.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-jp.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-jp.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-ko-utf8.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-ko-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-ko.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-ko.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-lt-utf8.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-lt-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-lt.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-lt.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-lv.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-lv.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-nl.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-nl.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-no.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-no.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-pl-utf8.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-pl-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-pl.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-pl.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-pt.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-pt.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-ro.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-ro.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-ru-UTF.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-ru-UTF.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-ru.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-ru.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-ru_win_.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-ru_win_.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-si.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-si.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-sk.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-sk.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-sp.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-sp.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-sr-utf8.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-sr-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-sr.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-sr.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-sv.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-sv.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-tr.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-tr.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/calendar-zh.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/calendar-zh.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/lang/cn_utf8.js` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/lang/cn_utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/aqua/theme.css` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/aqua/theme.css`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/aqua/today-bg.gif` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/aqua/today-bg.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/jscalendar/skins/tiger/theme.css` & `appy-1.0.9/py2/appy/gen/ui/jscalendar/skins/tiger/theme.css`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/loading.gif` & `appy-1.0.9/py2/appy/gen/ui/loading.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/loadingBig.gif` & `appy-1.0.9/py2/appy/gen/ui/loadingBig.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/loadingBtn.gif` & `appy-1.0.9/py2/appy/gen/ui/loadingBtn.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/loadingPod.gif` & `appy-1.0.9/py2/appy/gen/ui/loadingPod.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/locked.png` & `appy-1.0.9/py2/appy/gen/ui/locked.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/lockedBig.png` & `appy-1.0.9/py2/appy/gen/ui/lockedBig.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/logo.png` & `appy-1.0.9/py2/appy/gen/ui/logo.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/logout.png` & `appy-1.0.9/py2/appy/gen/ui/logout.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/ods.png` & `appy-1.0.9/py2/appy/gen/ui/ods.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/odsFrozen.png` & `appy-1.0.9/py2/appy/gen/ui/odsFrozen.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/ogone.gif` & `appy-1.0.9/py2/appy/gen/ui/ogone.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/paperclip.png` & `appy-1.0.9/py2/appy/gen/ui/paperclip.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/pwd.png` & `appy-1.0.9/py2/appy/gen/ui/pwd.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/refresh.png` & `appy-1.0.9/py2/appy/gen/ui/refresh.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/reindex.png` & `appy-1.0.9/py2/appy/gen/ui/reindex.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/save.png` & `appy-1.0.9/py2/appy/gen/ui/save.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/transition.png` & `appy-1.0.9/py2/appy/gen/ui/transition.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/unlock.png` & `appy-1.0.9/py2/appy/gen/ui/unlock.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/unlockBig.png` & `appy-1.0.9/py2/appy/gen/ui/unlockBig.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/url.png` & `appy-1.0.9/py2/appy/gen/ui/url.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/user.png` & `appy-1.0.9/py2/appy/gen/ui/user.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/warningBig.png` & `appy-1.0.9/py2/appy/gen/ui/warningBig.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/warning_no.gif` & `appy-1.0.9/py2/appy/gen/ui/warning_no.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/xls.png` & `appy-1.0.9/py2/appy/gen/ui/xls.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/xlsFrozen.png` & `appy-1.0.9/py2/appy/gen/ui/xlsFrozen.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/xlsx.png` & `appy-1.0.9/py2/appy/gen/ui/xlsx.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/ui/xlsxFrozen.png` & `appy-1.0.9/py2/appy/gen/ui/xlsxFrozen.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/utils.py` & `appy-1.0.9/py2/appy/gen/utils.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/validate.py` & `appy-1.0.9/py2/appy/gen/validate.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/wrappers/GroupWrapper.py` & `appy-1.0.9/py2/appy/gen/wrappers/GroupWrapper.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/wrappers/PageWrapper.py` & `appy-1.0.9/py2/appy/gen/wrappers/PageWrapper.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/wrappers/ToolWrapper.py` & `appy-1.0.9/py2/appy/gen/wrappers/ToolWrapper.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/wrappers/TranslationWrapper.py` & `appy-1.0.9/py2/appy/gen/wrappers/TranslationWrapper.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/wrappers/UserWrapper.py` & `appy-1.0.9/py2/appy/gen/wrappers/UserWrapper.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/gen/wrappers/__init__.py` & `appy-1.0.9/py2/appy/gen/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1147,18 +1147,18 @@
             raise Exception('Only Pod and Computed fields can be unfrozen.')
 
     def delete(self, executeMethods=True, unindex=True):
         '''Deletes myself'''
         self.o.delete(executeMethods=executeMethods, unindex=unindex)
 
     def translate(self, label, mapping=None, language=None, format='html',
-                  blankOnError=False):
+                  field=None, blankOnError=False):
         '''Check documentation of self.o.translate'''
         return self.o.translate(label, mapping, language=language,
-                                format=format, blankOnError=blankOnError)
+                          format=format, field=field, blankOnError=blankOnError)
 
     def do(self, name, comment='', doAction=True, doHistory=True,
            noSecurity=False, data=None):
         '''Programmatically triggers on p_self a transition named p_name. p_data
            can be a dict that will be included into the history event, if one
            wants to add custom data in the history event.'''
         o = self.o
```

### Comparing `appy-1.0.8/py2/appy/pod/__init__.py` & `appy-1.0.9/py2/appy/pod/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/actions.py` & `appy-1.0.9/py2/appy/pod/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,28 +147,38 @@
             eRes = None
             if self.expr:
                 eRes,error = self.evaluateExpression(result, context, self.expr)
             if not error:
                 # Trigger action-specific behaviour
                 self.do(result, context, eRes)
 
+    def getBufferStart(self):
+        '''If the start of the tied buffer must be ignored (=not be part of the
+           buffer, once evaluated), this method may return the start index
+           from which content will effectively be dumped.'''
+        return
+
     def evaluateBuffer(self, result, context,
                        forceSource=None, ignoreMinus=False):
         '''Evaluates the buffer tied to this action and add the result in
            p_result. The source for evaluation can be forced to p_forceSource
            but in most cases depends on self.source.'''
         # Determine the source
         source = forceSource or self.source
         # Determine "minus"
         if ignoreMinus:
             minus = False
         else:
             minus = self.minus
         if source == 'buffer':
-            self.buffer.evaluate(result, context, removeMainElems=minus)
+            self.buffer.evaluate(result, context, removeMainElems=minus,
+                                 forceStart=self.getBufferStart())
+            # m_getBufferStart may determine if the start of the buffer must be
+            # ignored, by forcing a start index: everything before this index
+            # will be ignored.
         else:
             # Evaluate self.fromExpr in fromRes
             fromRes = None
             error = False
             try:
                 fromRes = eval(self.fromExpr, context)
             except Exception, e:
@@ -194,14 +204,24 @@
             # Transmit "minus" to the sub-action. Indeed, the responsiblity to
             # dump content in the buffer is delegated to the sub-action,
             # "minus-ity" included.
             action.minus = self.minus
         else:
             self.subAction.addSubAction(action)
 
+    def getAction(self, type):
+        '''If p_self or one of its sub-actions (recursively) is of this p_type,
+           returns it.'''
+        # Return p_self itself, if it has this p_type
+        if self.__class__.__name__ == type: return self
+        # Check subAction
+        sub = self.subAction
+        if not sub: return
+        return sub.getAction(type)
+
     def check(self):
         '''Returns a tuple (success, message) indicating if the action is well
            formed or not.'''
         return True, None
 
 class If(Action):
     '''Action that determines if we must include the content of the buffer in
@@ -420,14 +440,19 @@
         context.update(hiddenVars)
         if elems:
             for name in self.iters:
                 if (name not in hiddenVars) and (name in context):
                     # On error, name may not be in the context
                     del context[name]
 
+    def getBufferStart(self):
+        '''In the context of a "do doc" statement, some tags must only be
+           dumped once and must be ignored in the subsequent iterations.'''
+        return
+
 class Null(Action):
     '''Action that does nothing. Used in conjunction with a "from" clause, it
        allows to insert in a buffer arbitrary odt content.'''
     noFromError = 'There was a problem with this action. Possible causes: ' \
       '(1) you specified no action (ie "do text") while not specifying any ' \
       'from clause; (2) you specified the from clause on the same line as ' \
       'the action, which is not allowed (ie "do text from ...").'
@@ -482,59 +507,78 @@
                                         afterClosing='office:annotation')
             self.evaluateBuffer(result, context,
                                 forceSource='buffer', ignoreMinus=True)
 
 class Variables(Action):
     '''Action that allows to define a set of variables somewhere in the
        template.'''
-    def __init__(self, name, buff, elem, minus, variables):
-        # We do not use the default Buffer.expr attribute for storing the Python
-        # expression, because here we will have several expressions, one for
+
+    def __init__(self, name, buff, elem, minus, variables, lasting=False):
+        # The default Buffer.expr attribute is not used for storing the Python
+        # expression, because several expressions can exist here, one for
         # every defined variable.
         Action.__init__(self, name, buff, None, elem, minus)
         # Definitions of variables: ~[(s_name|[s_name], s_expr)]~
         self.variables = variables
+        # If p_lasting is:
+        # ----------------------------------------------------------------------
+        # False | (the default) every variable's scope will be the target
+        #       | element (as determined by the corresponding buffer), not more.
+        #       | Any homonym variable being defined in the outer scope will be
+        #       | hidden in the context of the target element, and will be
+        #       | visible again as soon as the walk leaves this sub-scope.
+        # ----------------------------------------------------------------------
+        # True  | From the moment such a "lasting" variable is defined, its
+        #       | scope will be the remaining of the document. So, its scope
+        #       | encompasses the target element + the remaining of the
+        #       | document. Any homonym variable being previously defined will
+        #       | be hidden forever, as soon as the lasting variable is defined.
+        # ----------------------------------------------------------------------
+        self.lasting = lasting
 
     def storeVariable(self, name, value, context, hidden):
         '''Adds a variable named p_name with this p_value in the p_context.
            Updates the dict of p_hidden variables and r_eturn it.'''
         if name.startswith('@'):
             # "name" represents a global variable. Update its value in the
             # context with p_value.
             context[name[1:]] = value
         else:
             # Store variable p_name with p_value in the p_context. If this
             # variable already exists in the context, remember its previous
-            # value in p_hidden.
-            if name in context:
+            # value in p_hidden, excepted if the currently defined variables are
+            # lasting.
+            if not self.lasting and name in context:
                 if not hidden:
                     hidden = {name: context[name]}
                 else:
                     hidden[name] = context[name]
             # Store the result into the context
             context[name] = value
         return hidden
 
     def removeVariable(self, name, context, hidden):
         '''Remove, when relevant, variable p_name from the p_context'''
         # Do not remove it if it is a global variable
         if name.startswith('@'): return
         # Do not remove it if it is an overridden variable
-        if hidden and (name in hidden): return
+        if hidden and name in hidden: return
         del context[name]
 
     def do(self, result, context, exprRes):
-        '''Evaluate the variables' expressions: because there are several
-           expressions, we do not use the standard, single-expression-minded
-           Action code for evaluating expressions.
-
-           We remember the names and values of the variables that we will hide
-           in the context: after execution of this buffer, we will restore those
-           values.
-        '''
+        '''Evaluate the variables' expressions'''
+
+        # Because there are several expressions, the standard,
+        # single-expression-minded Action code is not used for evaluating
+        # expressions.
+
+        # If the currently defined variables are not lasting, the names and
+        # values of the variables that will be hidden in the context will be
+        # stored: after execution of this buffer, their values will be restored.
+
         hidden = None
         for names, expr in self.variables:
             # Evaluate variable expression in v_value
             value, error = self.evaluateExpression(result, context, expr)
             if error: return
             if isinstance(names, basestring):
                 # A single variable name
@@ -550,15 +594,16 @@
         if self.subAction:
             self.subAction.execute(result, context)
         else:
             # Evaluate the buffer directly
             self.evaluateBuffer(result, context)
         # Restore hidden variables if any
         if hidden: context.update(hidden)
-        # Delete not-hidden variables
-        for names, expr in self.variables:
-            if isinstance(names, basestring):
-                self.removeVariable(names, context, hidden)
-            else:
-                for name in names:
-                    self.removeVariable(name, context, hidden)
+        # Delete not-hidden variables, if not lasting
+        if not self.lasting:
+            for names, expr in self.variables:
+                if isinstance(names, basestring):
+                    self.removeVariable(names, context, hidden)
+                else:
+                    for name in names:
+                        self.removeVariable(name, context, hidden)
 # ------------------------------------------------------------------------------
```

### Comparing `appy-1.0.8/py2/appy/pod/buffers.py` & `appy-1.0.9/py2/appy/pod/buffers.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,24 +290,29 @@
         # Attributes instance is tied to an Expression; because dumping
         # expressions directly into FileBuffer instances seems to be rare, it
         # should not be a severe problem.
         pass
 
 # ------------------------------------------------------------------------------
 class MemoryBuffer(Buffer):
+    '''Buffer whose content is loaded in RAM'''
+
     class Rex:
         '''Regular expressions in use for a memory buffer'''
-        part = '(for|if|else|with|meta-if)\s*(.*)'
+        part = '(for|if|else|with\+|with|meta-if)\s*(.*)'
         action = re.compile('(?:(\w+)\s*\:\s*)?do\s+(\w+)(-)?(?:\s+%s)?' % part)
         subAction = re.compile(part)
         for_ = re.compile('\s*([\w\-_,\s]+)\s+in\s+(.*)')
         vars_ = re.compile('\s*([\w\-_,\s@]+)\s*=\s*(.*)')
         var_ = re.compile('@?[\w\-_]+')
         from_ = re.compile('from(\+)?\s+(.*)')
 
+    # Existing variants for the "with" statement
+    withVariants = {'with': None, 'with+': None}
+
     def __init__(self, env, parent):
         Buffer.__init__(self, env, parent)
         self.content = u''
         self.elements = {}
         self.action = None
 
     def clone(self):
@@ -479,16 +484,16 @@
             for index, buf in self.subBuffers.iteritems():
                 self.parent.subBuffers[oldParentLength + index] = buf
         # Empty the buffer
         MemoryBuffer.__init__(self, self.env, self.parent)
         # Change buffer position wrt parent
         self.parent.pushSubBuffer(self)
 
-    def addElement(self, elem, elemType='pod'):
-        if elemType == 'pod':
+    def addElement(self, elem, pod=True):
+        if pod:
             elem = PodElement.create(elem)
         self.elements[self.getLength()] = elem
         if isinstance(elem, Cell) or isinstance(elem, Table):
             elem.tableInfo = self.env.getTable()
             if isinstance(elem, Cell):
                 # Remember where this cell is in the table
                 elem.colIndex = elem.tableInfo.curColIndex
@@ -570,15 +575,17 @@
         return r
 
     def createPodAction(self, actionType, statements, statementName, subExpr,
                         podElem, minus, main=True):
         '''Creates an Action instance, depending on p_actionType'''
         if actionType == 'if':
             r = actions.If(statementName, self, subExpr, podElem, minus)
-            if main:
+            # In the case of multi-statements, only the first "if" will be
+            # connectable to an "else" statement.
+            if main or not self.action.getAction('If'):
                 self.env.ifActions.append(r)
                 if r.name:
                     # We must register this action as a named action
                     if self.env.namedIfActions.has_key(r.name):
                         raise ParsingError(DUPLICATE_NAMED_IF)
                     self.env.namedIfActions[r.name] = r
         elif actionType == 'else':
@@ -602,17 +609,18 @@
         elif actionType == 'for':
             forRes = self.Rex.for_.match(subExpr.strip())
             if not forRes:
                 raise ParsingError(BAD_FOR_EXPRESSION % subExpr)
             iters, subExpr = forRes.groups()
             iters = self._getForIterators(iters)
             r = actions.For(statementName, self, subExpr, podElem, minus, iters)
-        elif actionType == 'with':
-            variables = self._getVariables(subExpr)
-            r = actions.Variables(statementName, self, podElem, minus,variables)
+        elif actionType in self.withVariants:
+            r = actions.Variables(statementName, self, podElem, minus,
+                                  self._getVariables(subExpr),
+                                  lasting=actionType.endswith('+'))
         elif actionType == 'meta-if':
             r = actions.MetaIf(self, subExpr, podElem, minus, statements)
         else:
             r = actions.Null(self, podElem)
         return r
 
     def createPodActions(self, statements):
@@ -625,17 +633,17 @@
             if not statements: raise ParsingError(EMPTY_NOTE)
             # Get the main statement (starting with "do...") and check it
             main = statements[0]
             aRes = self.Rex.action.match(main)
             if not aRes:
                 raise ParsingError(BAD_STATEMENT % main)
             statementName, podElem, minus, actionType, subExpr = aRes.groups()
-            if not (podElem in PodElement.POD_ELEMS):
+            if podElem not in PodElement.POD_ELEMS:
                 raise ParsingError(BAD_ELEMENT % podElem)
-            if minus and (not podElem in PodElement.MINUS_ELEMS):
+            if minus and podElem not in PodElement.MINUS_ELEMS:
                 raise ParsingError(BAD_MINUS % (podElem,PodElement.MINUS_ELEMS))
             # Find the target element in the buffer
             i = self.getIndex(podElem)
             if i == -1:
                 raise ParsingError(ELEMENT_NOT_FOUND % (podElem, str([
                         e.__class__.__name__.lower() \
                         for e in self.elements.values()])))
@@ -835,15 +843,15 @@
         pos = self.content.find('>', pos)
         for index in self.elements.keys():
             if index < pos: del self.elements[index]
 
     reTagContent = re.compile('<(?P<p>[\w-]+):(?P<f>[\w-]+)(.*?)>.*</(?P=p):' \
                               '(?P=f)>', re.S)
     def evaluate(self, result, context, subElements=True,
-                 removeMainElems=False):
+                 removeMainElems=False, forceStart=None):
         '''Evaluates this buffer given the current p_context and add the result
            into p_result. With pod, p_result is the root file buffer; with px
            it is a memory buffer.'''
         if not subElements:
             # Dump the root tag in this buffer, but not its content
             res = self.reTagContent.match(self.content.strip())
             if not res: result.write(self.content)
@@ -853,15 +861,18 @@
                 if self.env.parser.caller.protection and (g2 == 'table-cell'):
                     # Attribute "protected" must be removed
                     g3 = g3.replace('table:protected=" "', '')
                 r = '<%s:%s%s></%s:%s>' % (g1, g2, g3, g1, g2)
                 result.write(r)
         else:
             if removeMainElems: self.removeAutomaticExpressions()
-            currentIndex = self.getStartIndex(removeMainElems)
+            if forceStart is not None:
+                currentIndex = forceStart
+            else:
+                currentIndex = self.getStartIndex(removeMainElems)
             for index, evalEntry in BufferIterator(self):
                 result.write(self.content[currentIndex:index])
                 currentIndex = index + 1
                 if isinstance(evalEntry, Expression):
                     try:
                         res, escape = evalEntry.evaluate(context)
                         if escape: result.dumpContent(res)
```

### Comparing `appy-1.0.8/py2/appy/pod/content.xmlt` & `appy-1.0.9/py2/appy/pod/content.xmlt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/converter.py` & `appy-1.0.9/py2/appy/pod/converter.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/doc_importers.py` & `appy-1.0.9/py2/appy/pod/doc_importers.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/elements.py` & `appy-1.0.9/py2/appy/pod/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 from appy.pod.odf_parser import OdfEnvironment as ns
 from appy.pod import PodError
 
 # ------------------------------------------------------------------------------
 class PodElement:
     OD_TO_POD = {'p': 'Text', 'h': 'Title', 'list-item': 'Item',
                  'section': 'Section', 'table': 'Table', 'table-row': 'Row',
-                 'table-cell': 'Cell', None: 'Expression', 'frame': 'Frame'}
+                 'table-cell': 'Cell', None: 'Expression', 'frame': 'Frame',
+                 'text': 'Doc'}
     POD_ELEMS = ('text', 'title', 'item', 'section', 'table', 'row', 'cell',
-                 'frame')
+                 'frame', 'doc')
     subTags = []
 
     # Elements for which the '-' operator can be applied
     MINUS_ELEMS = ('section', 'table')
 
     @staticmethod
     def create(elem):
@@ -75,14 +76,18 @@
     DEEPEST_TO_REMOVE = Cell.OD
     def __init__(self):
         self.tableInfo = None # ~OdTable~
 
 class Frame(PodElement):
     OD = XmlElement('frame', nsUri=ns.NS_DRAW)
 
+class Doc(PodElement):
+    '''Represents the base tag for a complete ODT document'''
+    OD = XmlElement('text', nsUri=ns.NS_OFFICE)
+
 class Expression(PodElement):
     '''Represents a Python expression that is found in a pod or px.'''
     OD = None
     metaWraps = {'"': '&quot;', "'": '&apos;'}
 
     def extractInfo(self, py):
         '''Within p_py, several elements can be included:
```

### Comparing `appy-1.0.8/py2/appy/pod/imageNotFound.jpg` & `appy-1.0.9/py2/appy/pod/imageNotFound.jpg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/lo_pool.py` & `appy-1.0.9/py2/appy/pod/lo_pool.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/metadata.py` & `appy-1.0.9/py2/appy/pod/metadata.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/odf_parser.py` & `appy-1.0.9/py2/appy/pod/odf_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,36 +16,36 @@
 # ------------------------------------------------------------------------------
 from appy.shared.xml_parser import XmlEnvironment, XmlParser
 
 class OdfEnvironment(XmlEnvironment):
     '''This environment is specific for parsing ODF files.'''
     # URIs of namespaces found in ODF files
     NS_OFFICE = 'urn:oasis:names:tc:opendocument:xmlns:office:1.0'
-    NS_STYLE = 'urn:oasis:names:tc:opendocument:xmlns:style:1.0'
-    NS_TEXT = 'urn:oasis:names:tc:opendocument:xmlns:text:1.0'
-    NS_TABLE = 'urn:oasis:names:tc:opendocument:xmlns:table:1.0'
-    NS_DRAW = 'urn:oasis:names:tc:opendocument:xmlns:drawing:1.0'
-    NS_FO = 'urn:oasis:names:tc:opendocument:xmlns:xsl-fo-compatible:1.0'
-    NS_XLINK = 'http://www.w3.org/1999/xlink'
-    NS_DC = 'http://purl.org/dc/elements/1.1/'
-    NS_META = 'urn:oasis:names:tc:opendocument:xmlns:meta:1.0'
+    NS_STYLE  = 'urn:oasis:names:tc:opendocument:xmlns:style:1.0'
+    NS_TEXT   = 'urn:oasis:names:tc:opendocument:xmlns:text:1.0'
+    NS_TABLE  = 'urn:oasis:names:tc:opendocument:xmlns:table:1.0'
+    NS_DRAW   = 'urn:oasis:names:tc:opendocument:xmlns:drawing:1.0'
+    NS_FO     = 'urn:oasis:names:tc:opendocument:xmlns:xsl-fo-compatible:1.0'
+    NS_XLINK  = 'http://www.w3.org/1999/xlink'
+    NS_DC     = 'http://purl.org/dc/elements/1.1/'
+    NS_META   = 'urn:oasis:names:tc:opendocument:xmlns:meta:1.0'
     NS_NUMBER = 'urn:oasis:names:tc:opendocument:xmlns:datastyle:1.0'
-    NS_SVG = 'urn:oasis:names:tc:opendocument:xmlns:svg-compatible:1.0'
-    NS_CHART = 'urn:oasis:names:tc:opendocument:xmlns:chart:1.0'
-    NS_DR3D = 'urn:oasis:names:tc:opendocument:xmlns:dr3d:1.0'
-    NS_MATH = 'http://www.w3.org/1998/Math/MathML'
-    NS_FORM = 'urn:oasis:names:tc:opendocument:xmlns:form:1.0'
+    NS_SVG    = 'urn:oasis:names:tc:opendocument:xmlns:svg-compatible:1.0'
+    NS_CHART  = 'urn:oasis:names:tc:opendocument:xmlns:chart:1.0'
+    NS_DR3D   = 'urn:oasis:names:tc:opendocument:xmlns:dr3d:1.0'
+    NS_MATH   = 'http://www.w3.org/1998/Math/MathML'
+    NS_FORM   = 'urn:oasis:names:tc:opendocument:xmlns:form:1.0'
     NS_SCRIPT = 'urn:oasis:names:tc:opendocument:xmlns:script:1.0'
-    NS_OOO = 'http://openoffice.org/2004/office'
-    NS_OOOW = 'http://openoffice.org/2004/writer'
-    NS_OOOC = 'http://openoffice.org/2004/calc'
-    NS_DOM = 'http://www.w3.org/2001/xml-events'
+    NS_OOO    = 'http://openoffice.org/2004/office'
+    NS_OOOW   = 'http://openoffice.org/2004/writer'
+    NS_OOOC   = 'http://openoffice.org/2004/calc'
+    NS_DOM    = 'http://www.w3.org/2001/xml-events'
     NS_XFORMS = 'http://www.w3.org/2002/xforms'
-    NS_XSD = 'http://www.w3.org/2001/XMLSchema'
-    NS_XSI = 'http://www.w3.org/2001/XMLSchema-instance'
+    NS_XSD    = 'http://www.w3.org/2001/XMLSchema'
+    NS_XSI    = 'http://www.w3.org/2001/XMLSchema-instance'
 
 class OdfParser(XmlParser):
     '''XML parser that is specific for parsing ODF files.'''
     def __init__(self, env=None, caller=None):
         if not env: env = OdfEnvironment()
         XmlParser.__init__(self, env, caller)
 # ------------------------------------------------------------------------------
```

### Comparing `appy-1.0.8/py2/appy/pod/parts.py` & `appy-1.0.9/py2/appy/pod/parts.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/pod_parser.py` & `appy-1.0.9/py2/appy/pod/pod_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,22 +18,24 @@
 from appy.shared.xml_parser import XmlElement
 from appy.pod.buffers import FileBuffer, MemoryBuffer
 from appy.pod.odf_parser import OdfEnvironment, OdfParser
 from appy.pod.elements import *
 
 # ------------------------------------------------------------------------------
 class OdTable:
-    '''Informations about the currently parsed Open Document (Od)table.'''
+    '''Informations about the currently parsed Open Document (Od)table'''
+
     def __init__(self):
         self.nbOfColumns = 0
         self.nbOfRows = 0
         self.curColIndex = None
         self.curRowAttrs = None
+
     def isOneCell(self):
-        return (self.nbOfColumns == 1) and (self.nbOfRows == 1)
+        return self.nbOfColumns == 1 and self.nbOfRows == 1
 
 class OdInsert:
     '''While parsing an odt/pod file, we may need to insert a specific odt chunk
        at a given place in the odt file (ie: add the pod-specific fonts and
        styles). OdInsert instances define such 'inserts' (what to insert and
        when).'''
     def __init__(self, odtChunk, elem, nsUris={}):
@@ -221,15 +223,15 @@
         self.ignorableElems = (tags['tracked-changes'], tags['change'])
         self.exprStartElems = [self.exprStartTags[holder] \
                                for holder in self.expressionsHolders]
         self.exprEndElems = [self.exprEndTags[holder] \
                              for holder in self.expressionsHolders]
         self.impactableElems = (Text.OD.elem, Title.OD.elem, Item.OD.elem,
                                 Table.OD.elem, Row.OD.elem, Cell.OD.elem,
-                                Section.OD.elem, Frame.OD.elem)
+                                Section.OD.elem, Frame.OD.elem, Doc.OD.elem)
         self.inserts = self.transformInserts()
 
     def getExpression(self, elem):
         '''We have found a pod expression within p_elem, get its value'''
         # Expression may have been found at various places
         if self.currentDbExpression:
             r = self.currentDbExpression
```

### Comparing `appy-1.0.8/py2/appy/pod/renderer.py` & `appy-1.0.9/py2/appy/pod/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import zipfile, shutil, xml.sax, os, os.path, re, mimetypes, time
 
 import appy.pod
 from appy.pod import PodError
 from appy.pod.lo_pool import LoPool
 from appy.shared.zip import unzip, zip
 from appy.pod.buffers import FileBuffer
+from appy.shared.xml_parser import Escape
 from appy.pod import styles_manager as sm
 from appy.pod.converter import FILE_TYPES
 from appy.pod import doc_importers as imps
 from appy.shared.xml_parser import XmlElement
 from appy.shared import mimeTypes, mimeTypesExts
 from appy.pod.xhtml2odt import Xhtml2OdtConverter
 from appy.shared.utils import FolderDeleter, FileWrapper
@@ -528,15 +529,16 @@
                 css = lastCss
             else:
                 css = otherCss
             if css:
                 css = ' class="%s"' % css
             else:
                 css = ''
-            r[i] = '<p%s>%s%s%s%s</p>' % (css, pre, opening, r[i], closing)
+            r[i] = '<p%s>%s%s%s%s</p>' % (css, pre, opening,
+                                          Escape.xhtml(r[i]), closing)
             i -= 1
         return self.renderXhtml(''.join(r), stylesMapping=stylesMapping)
 
     def evalIfExpression(self, condition, ifTrue, ifFalse):
         '''This method implements the method 'test' which is proposed in the
            default pod context. It represents an 'if' expression (as opposed to
            the 'if' statement): depending on p_condition, expression result is
```

### Comparing `appy-1.0.8/py2/appy/pod/styles.xmlt` & `appy-1.0.9/py2/appy/pod/styles.xmlt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/styles_manager.py` & `appy-1.0.9/py2/appy/pod/styles_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,21 +55,23 @@
 HTML_TEXT_ODT_PARA = 'For XHTML element "%s", you must associate an ' \
   'OpenDocument "text" style (that applies to only a chunk of text within a ' \
   'paragraph). "%s" is a paragraph-wide style.'
 
 # ------------------------------------------------------------------------------
 class Properties:
     '''Abstract base class for table and list properties'''
+
     # HTML elements whose styles are defined by Property instances instead of
     # Style instances.
     elems = ('table', 'ol', 'ul')
 
 class TableProperties(Properties):
     '''In a styles mapping, the value @key "table" must be an instance of this
        class.'''
+
     defaultMargins = (0.0, 0.0, 0.0, 0.0)
     columnModifiersPrefixes = {'optimize': 'OCW', 'distribute': 'DC'}
 
     def __init__(self, pageWidth=None, px2cm=px2cm, cellPx2cm=10.0,
               wideAbove=495, minColumnWidth=0.07, columnModifier=None,
               minCellPadding=0.0, cellContentStyle='podCellContent',
               headerContentStyle='podHeaderCellContent', margins=defaultMargins,
@@ -263,14 +265,15 @@
     def getTextProperties(self, i, nsText, nsStyle):
         '''Allows to define text properties at level p_i'''
         return ''
 
 class BulletedProperties(ListProperties):
     '''In a styles mapping, the value @key "ul" must be an instance of this
        class.'''
+
     type = 'bullet'
     defaultFormats = (u'•', u'◦', u'▪')
     textStyle = 'podBulletStyle'
 
     def __init__(self, levels=4, formats=defaultFormats,
                  delta=0.32, firstDelta=None, space=0.32, paraStyle=None):
         ListProperties.__init__(self, levels, formats, delta, firstDelta,
@@ -280,14 +283,15 @@
         '''Dumps bullet-specific attributes for level p_i'''
         # Get the bullet to render at this level
         return u'%s:bullet-char="%s"' % (nsText, getElementAt(self.formats, i))
 
 class NumberedProperties(ListProperties):
     '''In a styles mapping, the value @key "ol" must be an instance of this
        class.'''
+
     type = 'number'
     defaultFormats = ('1',)
     defaultSuffixes = ('.',)
     textStyle = 'podNumberStyle'
 
     def __init__(self, levels=4, formats=defaultFormats,
                  suffixes=defaultSuffixes, delta=0.32, firstDelta=None,
```

### Comparing `appy-1.0.8/py2/appy/pod/test/Readme.txt` & `appy-1.0.9/py2/appy/pod/test/Readme.txt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/Tester.py` & `appy-1.0.9/py2/appy/pod/test/Tester.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/ForCell6.py` & `appy-1.0.9/py2/appy/pod/test/contexts/ForCell6.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/ImagesImport.py` & `appy-1.0.9/py2/appy/pod/test/contexts/ImagesImport.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlColgroupTable.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlColgroupTable.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex2.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex2.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex3.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex3.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex4.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex4.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex5.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex5.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex7.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex7.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex8.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex8.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,7 +21,9 @@
 </blockquote>
 
 <p>Only flowing text passes :</p>
 <blockquote>
 This text is rendered.
 </blockquote>
 '''
+
+text1 = '''IMIO & Geezteem'''
```

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplex9.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplex9.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlComplexTables.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlComplexTables.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlCustomStyles.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlCustomStyles.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlKeepWithNext.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlKeepWithNext.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlNominal.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlNominal.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlPIntoLis.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlPIntoLis.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 xhtmlInput = '''
 <ol>
  <li>Row 1;</li>
  <li>row 2 :
   <p>- sub-paragraph, row 1</p>
   <p>- sub-paragraph, row 2</p>
  </li>
- <li><p>row 3;</p></li>
+ <li><p class="Signature">row 3 (Signature style applied);</p></li>
  <li>row 4:
    <ul>
      <li>Sub list:<p>aa</p><div>bb</div><div>aa</div></li>
      <li><div>Hello</div></li>
      <li>Normal</li>
    </ul>
  </li>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- xhtmlInput = '''
    1. Row 1;
    2. row 2 :
       - sub-paragraph, row 1
       - sub-paragraph, row 2
-   3. row 3;
+   3. row 3 (Signature style applied);
    4. row 4:
           o Sub list:
             aa
             bb
             aa
           o Hello
           o Normal
```

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlSpan.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlSpan.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlStylesMapping.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlStylesMapping.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlTables.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlTables.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlTwisted.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlTwisted.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/XhtmlWithStyle.py` & `appy-1.0.9/py2/appy/pod/test/contexts/XhtmlWithStyle.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/contexts/__init__.py` & `appy-1.0.9/py2/appy/pod/test/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/images/imio.png` & `appy-1.0.9/py2/appy/pod/test/images/imio.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/images/linux.jpg` & `appy-1.0.9/py2/appy/pod/test/images/linux.jpg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/images/plone.png` & `appy-1.0.9/py2/appy/pod/test/images/plone.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/images/python.blob` & `appy-1.0.9/py2/appy/pod/test/images/python.blob`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/images/python.gif` & `appy-1.0.9/py2/appy/pod/test/images/python.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/chart1.odt` & `appy-1.0.9/py2/appy/pod/test/results/chart1.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/errorExpression.odt` & `appy-1.0.9/py2/appy/pod/test/results/errorExpression.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/errorFooter.odt` & `appy-1.0.9/py2/appy/pod/test/results/errorFooter.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/errorForRuntime.odt` & `appy-1.0.9/py2/appy/pod/test/results/errorForRuntime.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/errorIf.odt` & `appy-1.0.9/py2/appy/pod/test/results/errorIf.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/fieldExpression.odt` & `appy-1.0.9/py2/appy/pod/test/results/fieldExpression.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/fileHandlerImport.odt` & `appy-1.0.9/py2/appy/pod/test/results/fileHandlerImport.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/forCellBug.odt` & `appy-1.0.9/py2/appy/pod/test/results/forCellBug.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/forCellBug2.odt` & `appy-1.0.9/py2/appy/pod/test/results/forCellBug2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/forCellCorrectNumber.odt` & `appy-1.0.9/py2/appy/pod/test/results/forCellCorrectNumber.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/forCellNotEnough.odt` & `appy-1.0.9/py2/appy/pod/test/results/forCellNotEnough.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/forCellOnlyOne.odt` & `appy-1.0.9/py2/appy/pod/test/results/forCellOnlyOne.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/forCellTooMuch1.odt` & `appy-1.0.9/py2/appy/pod/test/results/forCellTooMuch1.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/forCellTooMuch2.odt` & `appy-1.0.9/py2/appy/pod/test/results/forCellTooMuch2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/forCellTooMuch3.odt` & `appy-1.0.9/py2/appy/pod/test/results/forCellTooMuch3.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/forCellTooMuch4.odt` & `appy-1.0.9/py2/appy/pod/test/results/forCellTooMuch4.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/forTable.odt` & `appy-1.0.9/py2/appy/pod/test/results/forTable.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/forTableMinus.odt` & `appy-1.0.9/py2/appy/pod/test/results/forTableMinus.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/forTableMinus2.odt` & `appy-1.0.9/py2/appy/pod/test/results/forTableMinus2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/forTableMinusError.odt` & `appy-1.0.9/py2/appy/pod/test/results/forTableMinusError.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/forTableMinusError2.odt` & `appy-1.0.9/py2/appy/pod/test/results/forTableMinusError2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/headerFooter.odt` & `appy-1.0.9/py2/appy/pod/test/results/headerFooter.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/ifAndFors1.odt` & `appy-1.0.9/py2/appy/pod/test/results/ifAndFors1.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/ifElseErrors.odt` & `appy-1.0.9/py2/appy/pod/test/results/ifElseErrors.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/imagesImport.odt` & `appy-1.0.9/py2/appy/pod/test/results/imagesImport.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/noPython.odt` & `appy-1.0.9/py2/appy/pod/test/results/noPython.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/odsSimple.ods` & `appy-1.0.9/py2/appy/pod/test/results/odsSimple.ods`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/onlyExpressions.odt` & `appy-1.0.9/py2/appy/pod/test/results/onlyExpressions.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/pathImport.odt` & `appy-1.0.9/py2/appy/pod/test/results/pathImport.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/simpleForEmptyList.odt` & `appy-1.0.9/py2/appy/pod/test/results/simpleForEmptyList.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/simpleForFilledList.odt` & `appy-1.0.9/py2/appy/pod/test/results/simpleForFilledList.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/simpleForRow.odt` & `appy-1.0.9/py2/appy/pod/test/results/simpleForRow.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/simpleFromTest.odt` & `appy-1.0.9/py2/appy/pod/test/results/simpleFromTest.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/simpleIfIsFalse.odt` & `appy-1.0.9/py2/appy/pod/test/results/simpleIfIsFalse.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/simpleIfIsTrue.odt` & `appy-1.0.9/py2/appy/pod/test/results/simpleIfIsTrue.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/simpleIfIsTrue003.odt` & `appy-1.0.9/py2/appy/pod/test/results/simpleIfIsTrue003.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/simpleMinusError.odt` & `appy-1.0.9/py2/appy/pod/test/results/simpleMinusError.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/simpleTest.odt` & `appy-1.0.9/py2/appy/pod/test/results/simpleTest.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/varDef.odt` & `appy-1.0.9/py2/appy/pod/test/results/varDef.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/withAnImage.odt` & `appy-1.0.9/py2/appy/pod/test/results/withAnImage.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlColgroup.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlColgroup.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex2.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex3.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex3.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex4.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex4.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex5.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex5.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex6.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex6.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex7.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex7.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlComplex9.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlComplex9.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlComplexTables.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlComplexTables.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlCustomStyles.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlCustomStyles.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlEmpty.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlEmpty.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlEntities.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlEntities.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlHtml.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlHtml.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlIgnoreStyles.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlIgnoreStyles.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlInHeader.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlInHeader.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlKeepWithNext.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlKeepWithNext.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlListProperties.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlListProperties.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlNominal.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlNominal.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlPIntoLis.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlPIntoLis.odt`

 * *Files 19% similar despite different names*

#### odt2txt

```diff
@@ -1,14 +1,14 @@
 Row 1;
 
 row 2 :
 - sub-paragraph, row 1
 - sub-paragraph, row 2
 
-row 3;
+row 3 (Signature style applied);
 
 row 4:
 
 Sub list:
 aa
 bb
 aa
```

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlPIntoTds.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlPIntoTds.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlSpan.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlSpan.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlStylesErrors.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlStylesErrors.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlStylesMapping.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlStylesMapping.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlStylesMapping2.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlStylesMapping2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlTableProperties.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlTableProperties.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlTables.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlTables.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/results/xhtmlTwisted.odt` & `appy-1.0.9/py2/appy/pod/test/results/xhtmlTwisted.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/Chart1.odt` & `appy-1.0.9/py2/appy/pod/test/templates/Chart1.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ErrorExpression.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ErrorExpression.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ErrorFooter.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ErrorFooter.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ErrorForParsetime.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ErrorForParsetime.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ErrorForRuntime.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ErrorForRuntime.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ErrorIf.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ErrorIf.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/FieldExpressions.odt` & `appy-1.0.9/py2/appy/pod/test/templates/FieldExpressions.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/FileHandlerImport.odt` & `appy-1.0.9/py2/appy/pod/test/templates/FileHandlerImport.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ForCell.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ForCell.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ForCell2.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ForCell2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ForCell3.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ForCell3.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ForCell4.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ForCell4.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ForCell5.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ForCell5.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ForCell6.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ForCell6.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ForCell7.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ForCell7.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ForTable.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ForTable.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ForTableMinus.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ForTableMinus.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ForTableMinus2.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ForTableMinus2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ForTableMinusError.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ForTableMinusError.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ForTableMinusError2.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ForTableMinusError2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/HeaderFooter.odt` & `appy-1.0.9/py2/appy/pod/test/templates/HeaderFooter.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/IfAndFors1.odt` & `appy-1.0.9/py2/appy/pod/test/templates/IfAndFors1.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/IfElseErrors.odt` & `appy-1.0.9/py2/appy/pod/test/templates/IfElseErrors.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/ImagesImport.odt` & `appy-1.0.9/py2/appy/pod/test/templates/ImagesImport.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/NoPython.odt` & `appy-1.0.9/py2/appy/pod/test/templates/NoPython.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/OdsSimple.ods` & `appy-1.0.9/py2/appy/pod/test/templates/OdsSimple.ods`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/OnlyExpressions.odt` & `appy-1.0.9/py2/appy/pod/test/templates/OnlyExpressions.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/PathImport.odt` & `appy-1.0.9/py2/appy/pod/test/templates/PathImport.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/SimpleForEmptyList.odt` & `appy-1.0.9/py2/appy/pod/test/templates/SimpleForEmptyList.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/SimpleForFilledList.odt` & `appy-1.0.9/py2/appy/pod/test/templates/SimpleForFilledList.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/SimpleForRow.odt` & `appy-1.0.9/py2/appy/pod/test/templates/SimpleForRow.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/SimpleFromTest.odt` & `appy-1.0.9/py2/appy/pod/test/templates/SimpleFromTest.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/SimpleIfIsFalse.odt` & `appy-1.0.9/py2/appy/pod/test/templates/SimpleIfIsFalse.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/SimpleIfIsTrue.odt` & `appy-1.0.9/py2/appy/pod/test/templates/SimpleIfIsTrue.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/SimpleIfIsTrue003.odt` & `appy-1.0.9/py2/appy/pod/test/templates/SimpleIfIsTrue003.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/SimpleMinusError.odt` & `appy-1.0.9/py2/appy/pod/test/templates/SimpleMinusError.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/SimpleTest.odt` & `appy-1.0.9/py2/appy/pod/test/templates/SimpleTest.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/TablesToOptimize.odt` & `appy-1.0.9/py2/appy/pod/test/templates/TablesToOptimize.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/VarStatements.odt` & `appy-1.0.9/py2/appy/pod/test/templates/VarStatements.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/WithAnImage.odt` & `appy-1.0.9/py2/appy/pod/test/templates/WithAnImage.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/Xhtml.odt` & `appy-1.0.9/py2/appy/pod/test/templates/Xhtml.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlColGroup.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlColGroup.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlComplex2.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlComplex2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlComplex3.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlComplex3.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlComplex4.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlComplex4.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlComplexTables.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlComplexTables.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlHtml.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlHtml.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlInHeader.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlInHeader.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlKeepWithNext.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlKeepWithNext.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlNominal.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlNominal.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlSimple.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlSimple.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlSpan.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlSpan.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlStyles.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlStyles.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlStylesErrors.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlStylesErrors.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlTables.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlTables.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/test/templates/XhtmlTwisted.odt` & `appy-1.0.9/py2/appy/pod/test/templates/XhtmlTwisted.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/xhtml/parser.py` & `appy-1.0.9/py2/appy/pod/xhtml/parser.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/xhtml/tags.py` & `appy-1.0.9/py2/appy/pod/xhtml/tags.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/xhtml/visitors.py` & `appy-1.0.9/py2/appy/pod/xhtml/visitors.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/pod/xhtml2odt.py` & `appy-1.0.9/py2/appy/pod/xhtml2odt.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         # Sometimes we must remember the ODT style that has been computed and
         # applied to this HTML element (for lists).
         self.odStyle = None
         # For cells, the style to apply to their inner paragraphs (set later)
         self.innerStyle = None
         # We must know if a style must be applied on inner paragraphs within
         # "li" tags.
-        if (elem == 'li') and attrs.has_key('class'):
+        if elem == 'li' and attrs.has_key('class'):
             self.paraStyle = attrs['class']
         else:
             self.paraStyle = None # Will also be set on "ol" and "ul" tags.
         # Must we only keep tag content and remove the tag itself ?
         self.removeTag = False
         # Must we dump a line-break just before encountering a tag from
         # INNER_TAGS within this tag ?
@@ -199,15 +199,15 @@
            just dumped a "p", we can't dump a table within the "p". Such
            constraints do not hold in XHTML code but hold in ODF code.'''
         if not env.currentElements: return ()
         parent = env.getCurrentElement()
         # Special case: check elements that can't be found within a "li".
         # Instead of being noted as "conflictual", note that we must keep
         # these element's contents but remove the surrounding tags.
-        if (parent.elem == 'li') and (self.elem in PARA_TAGS):
+        if parent.elem == 'li' and self.elem in PARA_TAGS:
             self.removeTag = True
             parent.addInnerCssStyles(self)
             return ()
         # Check elements that can't be found within a paragraph / li. The list
         # of such elements is different for a "li", but "li" has elemType
         # "para", so we must explicitly check the "li" case before checking
         # "elemType" being "para" or not.
@@ -265,17 +265,33 @@
                             styleName = env.itemStyles[itemStyle + '_kwn']
                         else:
                             styleName = css
                 styleName = styleName or env.itemStyles[itemStyle]
                 dump(' text:style-name="%s"' % styleName)
             else:
                 # Check if a style must be applied on 'p' tags
-                if self.innerCssStyles:
-                    p.cssStyles.merge(self.innerCssStyles)
-                innerStyle = listElem.paraStyle or env.itemStyles[itemStyle]
+                innerStyles = self.innerCssStyles
+                paraStyle = None
+                if innerStyles:
+                    p.cssStyles.merge(innerStyles)
+                    class_ = getattr(innerStyles, 'classes', None)
+                    if class_:
+                        # Take the last CSS class if several are defined
+                        paraStyle = class_.split()[-1]
+                # Some remarks here.
+                # 1) The CSS class defined on the "p" tag, when present, takes
+                #    precedence over the one defined at the list level (itself
+                #    copied from the applicable ListProperties instance. This
+                #    precedence rule is hard-coded: it is not possible to choose
+                #    which one prevails, as opposed to what happens with
+                #    TableProperties instances via boolean attribute "prevails".
+                # 2) The CSS class potentially defined at the level of the "li"
+                #    tag is currently ignored.
+                innerStyle = paraStyle or listElem.paraStyle or \
+                             env.itemStyles[itemStyle]
                 if innerStyle:
                     p.cssStyles.addClass(innerStyle)
                 dump(env.getOdfAttributes(p))
         else:
             dump(env.getOdfAttributes(p))
         dump('>')
         if not self.tagsToClose: self.tagsToClose = []
```

### Comparing `appy-1.0.8/py2/appy/px/__init__.py` & `appy-1.0.9/py2/appy/px/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/px/px_parser.py` & `appy-1.0.9/py2/appy/px/px_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                 # Add the action
                 e.currentBuffer.createPxAction(elem, name, attrs[name])
         if e.isActionElem(elem):
             # Add a temp element in the buffer (that will be unreferenced
             # later). This way, when encountering the corresponding end element,
             # we will be able to check whether the end element corresponds to
             # the main element or to a sub-element.
-            e.currentBuffer.addElement(elem, elemType='px')
+            e.currentBuffer.addElement(elem, pod=False)
         if elem != 'x':
             # Dump the start element and its attributes. But as a preamble,
             # manage special attributes that could not be dumped at all, like
             # "selected" or "checked".
             hook = None
             ignorableAttrs = self.pxAttributes
             for name in self.noDumpTags:
```

### Comparing `appy-1.0.8/py2/appy/shared/__init__.py` & `appy-1.0.9/py2/appy/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/account.py` & `appy-1.0.9/py2/appy/shared/account.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/css.py` & `appy-1.0.9/py2/appy/shared/css.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/csv_parser.py` & `appy-1.0.9/py2/appy/shared/csv_parser.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/data/BelgianCommunes.txt` & `appy-1.0.9/py2/appy/shared/data/BelgianCommunes.txt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/data/CountryCodesIso3166.1.txt` & `appy-1.0.9/py2/appy/shared/data/CountryCodesIso3166.1.txt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/data/LanguageCodesIso639.2.txt` & `appy-1.0.9/py2/appy/shared/data/LanguageCodesIso639.2.txt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/data/__init__.py` & `appy-1.0.9/py2/appy/shared/data/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/dates.py` & `appy-1.0.9/py2/appy/shared/dates.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 
 # ------------------------------------------------------------------------------
 # Days of the week
 weekDays = ('Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun')
 weekDays_ = weekDays + ('Off',)
 
 # ------------------------------------------------------------------------------
+S_E_KO   = 'End date cannot be prior to start date.'
+
+# ------------------------------------------------------------------------------
 def toUTC(d):
     '''When manipulating DateTime instances, like p_d, errors can raise when
        performing operations on dates that are not in Universal time, during
        months when changing from/to summer/winter hour. This function returns
        p_d set to UTC.'''
     return DateTime('%d/%d/%d UTC' % (d.year(), d.month(), d.day()))
 
@@ -121,15 +124,57 @@
     fmt = '%d/%s/%%d %%H:%%M:%%S' % (year, month)
     dateStr = date.strftime(fmt)
     try:
         r = DateTime(dateStr)
     except Exception, e:
         # Start with the first day of the target month and get its last day
         fmt = '%d/%s/01' % (year, month)
-        r = getLastDayOfMonth(DateTime(date.strftime(fmt)), hour='%H:%M:%S')
+        r = getLastDayOfMonth(DateTime(date.strftime(fmt)),
+                              hour=date.strftime('%H:%M:%S'))
+    return r
+
+def getCalendarMonths(date, end=None, fmt='%Y%m'):
+    '''Returns, as a set of strings with this p_fmt, the months being crossed
+       by p_date, or, if p_end is passed, being crossed by range
+       (p_date, p_end).'''
+    # By "month", we mean: the complete range of dates being shown when a month
+    # is shown in a monthly-view calendar. Because, in that kind of view, full
+    # weeks are rendered, the "month" generally encompasses several days from
+    # the previous and next months.
+    r = set()
+    fdate = date.strftime(fmt)
+    r.add(fdate)
+    # Get the first day of the week into which p_date is. dow
+    # (*d*ay *o*f *w*eek) for Sunday is 0: we convert it to 7.
+    dow = date.dow() or 7
+    first = date - (dow-1)
+    r.add(first.strftime(fmt)) # May be from the previous month
+    # Take p_end into account if present
+    if end:
+        # Ensure p_end is not prior to p_date
+        if end < date: raise Exception(S_E_KO)
+        fend = end.strftime(fmt)
+        r.add(fend)
+    else:
+        end = date
+        fend = fdate
+    # Get the last day of the week into which p_end is
+    dow = end.dow()
+    if dow != 0: # If Sunday, there will be no overflow on the next month
+        last = end + (7-dow)
+        r.add(last.strftime(fmt))
+    # Add intermediary months between p_date and p_end, if distant from more
+    # than one month.
+    if fdate != fend and end - date > 28:
+        month = getSiblingMonth(date)
+        smonth = month.strftime(fmt)
+        while smonth not in r:
+            r.add(smonth)
+            month = getSiblingMonth(month)
+            smonth = month.strftime(fmt)
     return r
 
 def periodsIntersect(start1, end1, start2, end2):
     '''Is there an intersection between intervals [start1, end1] and
        [start2, end2] ?'''
     # p_start1 and p_start2 must be DateTime instances.
     # p_end1 and p_end2 may be DateTime instances or None.
```

### Comparing `appy-1.0.8/py2/appy/shared/dav.py` & `appy-1.0.9/py2/appy/shared/dav.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/diff.py` & `appy-1.0.9/py2/appy/shared/diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,19 +394,22 @@
         '''
         if line.startswith(self.divDeletePrefix):
             return ('delete', line, None, None)
         if line.startswith(self.divInsertPrefix):
             # Return the line without the surrounding tag
             action = 'insert'
             outerTag = htmlTag.match(line)
-            line = outerTag.group(3)
+            if outerTag:
+                line = outerTag.group(3)
+            else:
+                line = '?'
         else:
             action = None
             outerTag = None
-        # Replace found inner inserts with their content.
+        # Replace found inner inserts with their content
         innerDiffs = []
         while True:
             match = innerDiff.search(line)
             if not match: break
             # I found one.
             innerDiffs.append(match)
             line = self.applyDiff(line, match)
```

### Comparing `appy-1.0.8/py2/appy/shared/errors.py` & `appy-1.0.9/py2/appy/shared/errors.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/google.py` & `appy-1.0.9/py2/appy/shared/google.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/ical.py` & `appy-1.0.9/py2/appy/shared/ical.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/ldap_connector.py` & `appy-1.0.9/py2/appy/shared/ldap_connector.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/odf.py` & `appy-1.0.9/py2/appy/shared/odf.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/packaging.py` & `appy-1.0.9/py2/appy/shared/packaging.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/sap.py` & `appy-1.0.9/py2/appy/shared/sap.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/sso.py` & `appy-1.0.9/py2/appy/shared/sso.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/tables.py` & `appy-1.0.9/py2/appy/shared/tables.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/test.py` & `appy-1.0.9/py2/appy/shared/test.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/utils.py` & `appy-1.0.9/py2/appy/shared/utils.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/xml_parser.py` & `appy-1.0.9/py2/appy/shared/xml_parser.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/shared/zip.py` & `appy-1.0.9/py2/appy/shared/zip.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py2/appy/test/profiler.py` & `appy-1.0.9/py2/appy/test/profiler.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/__init__.py` & `appy-1.0.9/py3/appy/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/all.py` & `appy-1.0.9/py3/appy/all.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/bin/__init__.py` & `appy-1.0.9/py3/appy/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/bin/deploy.py` & `appy-1.0.9/py3/appy/bin/deploy.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/bin/lo.py` & `appy-1.0.9/py3/appy/bin/lo.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License along with
 # Appy. If not, see <http://www.gnu.org/licenses/>.
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
+import sys
 from pathlib import Path
 
 from appy.pod import test
 from appy.bin import Program
 from appy.pod.renderer import Renderer
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
@@ -34,20 +35,22 @@
  DEFAULT_TEST: 'a simple test calling LO to convert an odt file into pdf',
  'subPods': 'renders a POD template incorporating sub-pods via a statement ' \
             'of the form "do ... from ..."'
 }
 HELP_SERVER = 'The hostname of the machine running LibreOffice. Defaults to ' \
   '"%s".' % DEFAULT_SERVER
 HELP_PORT = 'The port where LibreOffice listens. Defaults to %d.' % DEFAULT_PORT
-HELP_TEST = 'The test to execute. Available tests are %s.' % \
+HELP_TEST = 'The test to execute. Available tests are %s. ' \
+            'Default test is "convertToPdf".' % \
             ', '.join(['"%s" (%s)' % (k, v) for k, v in TESTS.items()])
 TEST_NOT_FOUND = 'Test %s does not exist.'
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class LO(Program):
+    '''Tests LO'''
 
     def defineArguments(self):
         '''Define the allowed arguments for this program'''
         parser = self.parser
         # Optional arguments: LO server and port
         parser.add_argument('-s', '--server', dest='server', help=HELP_SERVER,
                             default=DEFAULT_SERVER)
@@ -68,14 +71,15 @@
         odtFile = self.filesPath / 'NoPython.odt'
         # Create and run a Converter instance
         from appy.pod.converter import Converter
         try:
             converter = Converter(str(odtFile), 'pdf', server=self.server,
                                   port=self.port, verbose=True)
             converter.run()
+            return True
         except converter.Error as err:
             print(err)
 
     def subPods(self):
         '''Renders a POD template incorporating sub-pods (via a "do... from
            pod..." statement). Appy calls LO for doing this.'''
         # Create a Renderer for computing the POD...
@@ -83,29 +87,32 @@
         context = {'files': self.filesPath}
         result = self.filesPath / 'FromPod.pdf'
         renderer = Renderer(str(template), context, str(result),
                             ooServer=self.server, ooPort=self.port, stream=True,
                             overwriteExisting=True, forceOoCall=True)
         print('Rendering %s...' % str(template))
         renderer.run()
+        return True
         print('Result produced in %s.' % str(result))
 
     def run(self):
         '''Contacts LO'''
         print('Running test "%s" on LO %s:%s...' % \
               (self.test, self.server, self.port))
         # Abort if the specified test does not exist
         if not hasattr(self, self.test):
             print(TEST_NOT_FOUND % self.test)
-            return
+            sys.exit(1)
         method = getattr(self, self.test)
         if not callable(method):
             print(TEST_NOT_FOUND % self.test)
-            return
+            sys.exit(1)
         # Get the path to the POD test files
         self.filesPath = Path(test.__file__).parent / 'templates'
         # Execute the test
-        return method()
+        success = method()
+        if not success:
+            sys.exit(1)
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 if __name__ == '__main__': LO().run()
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
```

### Comparing `appy-1.0.8/py3/appy/bin/make.py` & `appy-1.0.9/py3/appy/bin/make.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/bin/perform.py` & `appy-1.0.9/py3/appy/bin/perform.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/bin/run.py` & `appy-1.0.9/py3/appy/bin/run.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/data/Countries.Iso3166-1` & `appy-1.0.9/py3/appy/data/Countries.Iso3166-1`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/data/Languages.Iso639-2` & `appy-1.0.9/py3/appy/data/Languages.Iso639-2`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/data/__init__.py` & `appy-1.0.9/py3/appy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/database/__init__.py` & `appy-1.0.9/py3/appy/database/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License along with
 # Appy. If not, see <http://www.gnu.org/licenses/>.
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
-import os, time, pathlib
+import os, sys, time, pathlib
 
 from DateTime import DateTime
 from zc.lockfile import LockError
 from BTrees.IOBTree import IOBTree
 from persistent.mapping import PersistentMapping
 import ZODB, ZODB.POSException, transaction, transaction.interfaces
 
@@ -185,27 +185,43 @@
             transaction.abort()
             connection.close()
 
     def listConnections(self):
         '''Returns the list of active connections to the database'''
         return self.db.connectionDebugInfo()
 
+    def listTransactions(self, start=None, end=None):
+        '''Lists the database transactions that occurred between this p_start
+           and p_end dates.'''
+        # p_start and/or p_end, if passed, must be DateTime instances
+        # If p_start is None, it will represent the start of the database life.
+        # If p_end is None, it will represent the end of times.
+        start = start.timeTime() if start else 0
+        end = end.timeTime() if end else sys.maxsize
+        return self.db.undoLog(start, end)
+
     def commit(self, handler):
         '''Commits the current transaction related to p_handler'''
         transaction.commit()
 
     def abort(self, connection=None, message=None, logger=None):
         '''Abort the current transaction'''
         # Logs a p_message when requested
         if message: logger.error(message)
         # Abort the ongoing transaction
         transaction.abort()
         # Close the p_connection if given
         if connection: connection.close()
 
+    def undo(self, handler, transactionIds):
+        '''Undo transactions whose IDs are in p_transactionIds'''
+        for id in transactionIds:
+            self.db.undo(id)
+            handler.dbConnection.sync()
+
     def close(self, abort=False):
         '''Closes the database'''
         # Must we first abort any ongoing transaction ?
         if abort: transaction.abort()
         try:
             self.db.close()
         except ZODB.POSException.ConnectionStateError:
```

### Comparing `appy-1.0.8/py3/appy/database/catalog.py` & `appy-1.0.9/py3/appy/database/catalog.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/database/indexes/__init__.py` & `appy-1.0.9/py3/appy/database/indexes/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/database/indexes/boolean.py` & `appy-1.0.9/py3/appy/database/indexes/boolean.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/database/indexes/date.py` & `appy-1.0.9/py3/appy/database/indexes/date.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/database/indexes/float.py` & `appy-1.0.9/py3/appy/database/indexes/float.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/database/indexes/ref.py` & `appy-1.0.9/py3/appy/database/indexes/ref.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/database/indexes/rich.py` & `appy-1.0.9/py3/appy/database/indexes/rich.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/database/indexes/text.py` & `appy-1.0.9/py3/appy/database/indexes/text.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/database/lazy.py` & `appy-1.0.9/py3/appy/database/lazy.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/database/lock.py` & `appy-1.0.9/py3/appy/database/lock.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/database/log.py` & `appy-1.0.9/py3/appy/database/log.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/database/operators.py` & `appy-1.0.9/py3/appy/database/operators.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/database/sorter.py` & `appy-1.0.9/py3/appy/database/sorter.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/deploy/__init__.py` & `appy-1.0.9/py3/appy/deploy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         # A list of Python dependencies to install on the distant app, in its
         # "lib" folder. For every dependency, a specifier must be used, with the
         # same syntax as attributes "siteApp/siteExt" hereabove.
         self.siteDependencies = siteDependencies or []
 
     def __repr__(self):
         '''p_self's string representation'''
-        return '<Target %s:%d>' % (self.sshHost, self.sshPort)
+        return '<Target %s:%d@%s>' % (self.sshHost, self.sshPort, self.sitePath)
 
     def execute(self, command):
         '''Executes p_command on this target'''
         r = ['ssh', '%s@%s' % (self.sshLogin, self.sshHost), '"%s"' % command]
         # Determine port
         if self.sshPort != 22: r.insert(1, '-p%d' % self.sshPort)
         # Determine "-i" option (path to the private key)
```

### Comparing `appy-1.0.8/py3/appy/deploy/subversion.py` & `appy-1.0.9/py3/appy/deploy/subversion.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/__init__.py` & `appy-1.0.9/py3/appy/model/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
        extended by the application model.'''
     class Error(Exception): pass
 
     # Names of base classes forming the base Appy model, in package appy.model,
     # and standard workflows defined in package appy.model.workflows.standard.
     # These classes and workflows are injected into any app's model.
     baseClasses = ('Page', 'User', 'Group', 'Tool', 'Translation', 'Carousel',
-                   'Document', 'Query')
+                   'Document', 'Query', 'Mover')
     baseWorkflows = ('Anonymous', 'Authenticated', 'Owner', 'TooPermissive')
 
     def __init__(self, config, classes, workflows):
         '''The unique Model instance is created by the
            appy.model.loader.Loader.'''
         # The app's global config
         self.config = config
```

### Comparing `appy-1.0.8/py3/appy/model/base.py` & `appy-1.0.9/py3/appy/model/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,28 +91,34 @@
     searchable = Text(show=False, persist=False, indexed=True,
                       default=getSearchableText, label='Base', page=None)
 
     # Attribute "title" is a mandatory field used at various places by default,
     # for displaying base information about an object.
     titleAttributes = {'multiplicity': (1,1), 'show': Show.EX, 'indexed': True,
       'searchable': True, 'filterField': searchable,
-      # This method allows to produce an index value suitable for sorting
-      'indexValue': lambda o, v: Normalize.text(o.getShownValue(),
+      # The following lambda allows to produce an index value suitable for
+      # sorting. In the call to m_getShownValue, language 'en' is forced in
+      # order to bypass the user language and always have a deterministic value.
+      'indexValue': lambda o, v: Normalize.text(o.getShownValue(language='en'),
                                                 keepBlank=False) if v else ''}
 
     title = String(**titleAttributes)
 
     # Attribute "creator" gets the login of the user having created the object
     p = {'multiplicity': (1,1), 'show': 'xml', 'indexed': True, 'label': 'Base'}
     creator = Computed(method=lambda o: o.history[-1].login, **p)
 
     def setCreator(self, login):
         '''Sets p_login as p_self's creator'''
         self.history[-1].login = login
 
+    def getCreator(self, title=True):
+        '''Return the User instance (or its p_title) behind p_self.creator'''
+        return self.history[-1].getUser(self, title=title)
+
     # Object's creation and last modification dates
     p['show'] = Show.VE_
     created = Date(default=lambda o: o.history[-1].date, persist=False, **p)
     modified = Date(default=lambda o: o.history.modified, persist=False, **p)
 
     # "state" is a field deduced from the object history and identifies the
     # object state according to its workflow. It must be a "select" field,
@@ -147,14 +153,15 @@
                      indexed=True, default=getAllowed, label='Base')
 
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # History
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     recordAttributes = {'method': History.view, 'label':'Base', 'layouts':'f',
+      'xml': lambda o, value: o.history,
       'page':Page('history', label='Base_page_history',
                   sticky=True, icon='history.svg',
                   show=lambda o: 'view' if o.user.hasRole('Manager') else None)}
 
     record = Computed(**recordAttributes)
 
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
@@ -170,14 +177,15 @@
     # Properties
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     # The following properties are read-only attributes allowing easy access,
     # from any object in the database, to (i) a series of heavily-demanded
     # objects, like the tool or the currently logged user, or (ii) commonly
     # used functions.
+
     # ~~~ All these properties will have this setter, raising an exception
     def raiseReadOnly(self, v): raise Exception(RO_EXPR)
 
     # The guard
     guard = property(lambda o: o.H().guard, raiseReadOnly)
 
     # The currently logged user
@@ -195,14 +203,17 @@
     # The request and response objects
     req = property(lambda o: o.H().req, raiseReadOnly)
     resp = property(lambda o: o.H().resp, raiseReadOnly)
 
     # The object (base) URL
     url = property(lambda o: o.H().server.getUrl(o), raiseReadOnly)
 
+    # An access to the developer's cache object, stored on the handler
+    cache = property(lambda o: o.H().cache, raiseReadOnly)
+
     # A potential initiator object
     initiator = property(lambda o: o.getInitiator(), raiseReadOnly)
 
     # The referer URL
     referer = property(lambda o: o.H().headers['Referer'], raiseReadOnly)
 
     # The object container
@@ -216,18 +227,24 @@
 
     # The path to the app folder
     appPath = property(lambda o: o.H().config.model.appPath, raiseReadOnly)
 
     # The current traversal
     traversal = property(lambda o: o.H().traversal, raiseReadOnly)
 
+    # The translated name of the current object state
+    stateLabel = property(lambda o: o.getLabel(o.state, field=False))
+
     # The catalog storing indexed data for this object
     traverse['catalog'] = 'Manager'
     catalog = property(lambda o: o.getCatalog(), raiseReadOnly)
 
+    # A reference the the database object
+    database = property(lambda o: o.H().server.database, raiseReadOnly)
+
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # Base methods
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def getHandler(self):
         '''Returns the current request handler'''
         # Class "Handler" has been injected to class Base in Base.Handler in
@@ -285,17 +302,23 @@
         # Try to get the page from the request, or return p_self's default
         # page on p_layout.
         return req.page or self.getDefaultPage(layout)
 
     def getObject(self, id, logMissing=False):
         '''Gets an object given its p_id'''
         if not id: raise Exception(NO_ID)
-        handler = self.H()
-        return handler.server.database.getObject(handler, id,
-                                                 logMissing=logMissing)
+        return self.database.getObject(self.H(), id, logMissing=logMissing)
+
+    def getRefObject(self):
+        '''This method returns the source object, if we are in the context of
+           performing some action (like a search) in the context of a Ref.'''
+        # Information about such Ref is found in the request
+        info = self.req.ref or Criteria.readFromRequest(self.H()).get('_ref')
+        if not info: return
+        return self.getObject(info.split(':', 1)[0])
 
     def __repr__(self):
         '''Returns the class name and Appy object ID'''
         return '<%s id=%s>' % (self.getClass().name, self.id)
 
     def isTemp(self):
         '''Is this object temporary ?'''
@@ -305,17 +328,18 @@
         '''Logs a p_message of some p_type'''
         return self.H().log('app', type, message)
 
     def say(self, message):
         '''Adds p_message to the global message returned in the response'''
         self.resp.addMessage(message)
 
-    def goto(self, url=None, message=None):
-        '''Return to some p_url or to the referer page'''
-        self.resp.goto(url, message)
+    def goto(self, url=None, message=None, fromPopup=False):
+        '''Return to some p_url or to the referer page. If you want to come back
+           from a popup, explicitly set p_fromPopup to True.'''
+        self.resp.goto(url, message, fromPopup)
 
     def gotoSet(self):
         '''Return True if m_goto has already been called and the response code
            is already a 303 "Redirect".'''
         return self.resp.code == 303
 
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
@@ -375,19 +399,19 @@
 
     def getFields(self, layout, page=None, phase=None, type=None, fields=None):
         '''Returns the list of fields to render on p_layout'''
         r = []
         # Browse p_self's fields, or p_fields if passed
         for field in (fields or self.class_.fields.values()):
             # Ignore fields not being on p_page
-            if page and (field.pageName != page): continue
+            if page and field.pageName != page: continue
             # Ignore fields not being on any page in p_phase
             if phase and (field.page and (field.page.phase != phase)): continue
             # Ignore fields not being of p_type
-            if type and (field.type != type): continue
+            if type and field.type != type: continue
             # Ignore fields that can't be rendered on p_layout
             if not field.isRenderable(layout): continue
             # Ignore unshowable fields 
             if not field.isShowable(self, layout): continue
             r.append(field)
         return r
 
@@ -425,17 +449,17 @@
             # Ignore fields whose page is not p_page
             if field.pageName != page: continue
             # Ignore fields that must not be shown
             if not field.isShowable(self, layout): continue
             if collect:
                 # Collect JS/CSS files
                 if css is None: css = []
-                field.getCss(layout, css)
+                field.getCss(self, layout, css)
                 if js is None: js = []
-                field.getJs(layout, js, config)
+                field.getJs(self, layout, js, config)
             # Insert the field directly in the result if it is not in a group
             if not field.group:
                 r.append(field)
             else:
                 # Insert it in the right group (if the group exists on p_layout)
                 group = field.getGroup(layout)
                 if not group:
@@ -459,23 +483,24 @@
         '''Returns True if value of field p_name is considered to be empty
            (or p_value if p_fromParam is True).'''
         field = self.getField(name, raiseError=True)
         if not fromParam:
             value = field.getStoredValue(self, name)
         return field.isEmptyValue(self, value)
 
-    def getLabel(self, name, field=True):
+    def getLabel(self, name, field=True, language=None):
         '''Gets the translated label for field (if p_field is True) or workflow
            state or transition (if p_field is False) named p_name.'''
         # Translate the name of a field
         if field:
             field = self.getField(name, raiseError=True)
-            return self.translate('labelId', field=field)
+            return self.translate('label', field=field, language=language)
         # Translate the name of a state or transition
-        return self.translate('%s_%s' % (self.getWorkflow().name, name))
+        return self.translate('%s_%s' % (self.getWorkflow().name, name),
+                              language=language)
 
     def getShownValue(self, name='title', layout='view', language=None):
         '''Call field.getShownValue on field named p_name'''
         field = self.getField(name)
         return field.getShownValue(self, field.getValue(self), layout,
                                    language=language)
 
@@ -620,15 +645,15 @@
     # It is illegal to have the same object being the target of more that one
     # composite Ref.
 
     def computeCid(self):
         '''Computes the container ID ("cid") for p_self'''
         r = None
         for field in self.class_.fields.values():
-            if (field.type == 'Ref') and field.isBack and field.back.composite:
+            if field.type == 'Ref' and field.isBack and field.back.composite:
                 container = getattr(self, field.name, None)
                 if container:
                     try:
                         iid = container.iid
                     except AttributeError:
                         iid = container[0].iid
                     r = '%d_%s' % (iid, field.name)
@@ -676,17 +701,16 @@
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def search(self, className=None, **kwargs):
         '''Performs a search in the database, for instances of class named
            p_className, or of self's class if not specified.'''
         if className and not isinstance(className, str): raise Exception(NO_STR)
         handler = self.H()
-        database = handler.server.database
         className = className or self.class_.name
-        return database.search(handler, className, **kwargs)
+        return self.database.search(handler, className, **kwargs)
 
     def search1(self, className=None, **kwargs):
         '''Performs a search for a single object'''
         r = self.search(className, **kwargs)
         return r[0] if r else None
 
     def count(self, className=None, **kwargs):
@@ -738,17 +762,15 @@
         return ctx
 
     def reindex(self, **kwargs):
         '''(re-/un-)indexes this object in the catalog corresponding to its
            class. Returns True if at least one change has been actually
            performed in at least one index.'''
         if self.isTemp(): raise Exception(INDEX_TEMP)
-        handler = self.H()
-        database = handler.server.database
-        return database.reindexObject(handler, self, **kwargs)
+        return self.database.reindexObject(self.H(), self, **kwargs)
 
     def getCatalog(self, raiseError=False):
         '''Returns the catalog storing p_self (if indexed)'''
         r = self.H().dbConnection.root.catalogs.get(self.class_.name)
         if not r and raiseError:
             raise Exception(CATALOG_KO % self.class_.name)
         return r
@@ -900,18 +922,17 @@
             # Check that the user can edit this field
             if secure: field.checkAdd(self)
         else:
             # p_name is the name of a root class
             className = _name
             field = None
         # Create the object
-        handler = self.H()
-        database = handler.server.database
-        o = database.new(handler, className, id=id, secure=secure,
-                       initialComment=initialComment, initialState=initialState)
+        o = self.database.new(self.H(), className, id=id, secure=secure,
+                              initialComment=initialComment,
+                              initialState=initialState)
         # Set object attributes
         for name, value in kwargs.items():
             try:
                 setattr(o, name, value)
             except AttributeError as ae:
                 if raiseOnWrongAttribute: raise ae
         # Call custom early initialization: a hook allowing the app developer to
@@ -978,15 +999,15 @@
             history[-1].date = other.created
             # Keep the same modification date
             history.modified = other.modified
         return r
 
     def delete(self, historize=False, executeMethods=True):
         '''Deletes p_self (see homonym method on the database object'''
-        return self.H().server.database.delete(self, historize, executeMethods)
+        return self.database.delete(self, historize, executeMethods)
 
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # Translation method
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def translate(self, label, mapping=None, language=None, asText=False,
                   field=None, blankOnError=False):
@@ -1148,14 +1169,16 @@
       <script>protectAppyForm()</script>
       <form id="appyForm" name="appyForm" method="post"
             enctype="multipart/form-data" action=":'%s/save' % o.url">
        <input type="hidden" name="action" value=""/>
        <input type="hidden" name="popup" value=":popup"/>
        <input type="hidden" name="page" value=":page"/>
        <input type="hidden" name="nav" value=":req.nav or ''"/>
+       <input type="hidden" name="referer"
+              value=":req.referer or o.referer or ''"/>
        <input type="hidden" name="_get_" value=":req._get_ or ''"/>
        <input type="hidden" name="gotoPage" value=""/>
        <input type="hidden" name="gotoLayout" value=""/>
        <input type="hidden" name="insert" value=":req.insert or ''"/>
        <input type="hidden" name="confirmed" value="False"/>
        <x var="tagId='pageLayout'; tagName=''; tagCss='';
                layoutTarget=o">:table.pxRender</x>
@@ -1249,15 +1272,15 @@
                 if criteria and ('_ref' in criteria): ref = criteria['_ref']
             if ref:
                 return self.getObject(ref.split(':')[0])
 
     def getFolder(self, create=False, withRelative=False):
         '''Gets, as a pathlib.Path instance, the folder where binary files
            related to this object are stored on the filesystem.'''
-        return self.H().server.database.getFolder(self, create, withRelative)
+        return self.database.getFolder(self, create, withRelative)
 
     def cancel(self, initiator=None, popup=False, isTemp=False):
         '''Redirect the user after an object edition has been canceled'''
         self.H().commit = True
         # Render a message for the user. This message (and the url to redirect
         # the user to) may be customized by method m_onCancel.
         req = self.req
@@ -1274,25 +1297,15 @@
         else:
             # Remove the lock set on the current page
             Lock.remove(self, page)
         # If we are in a popup, render a minimalist HTML page that will close it
         if popup: return Iframe.goBack(self.tool, initiator)
         # Determine, if not defined yet, the URL to go back to
         if self.gotoSet(): return
-        if not url:
-            if initiator:
-                # Go back to the initiator page
-                url = initiator.getUrl()
-            elif isTemp:
-                # Go back to home page
-                url = self.tool.computeHomePage()
-            else:
-                # Return to p_self's view page
-                url = self.getUrl(sub='view', page=page, nav=req.nav or 'no')
-        self.goto(url)
+        self.goto(url or self.req.referer)
 
     traverse['save'] = 'perm:write'
     def save(self):
         '''Called when p_self's data coming from the UI must be saved to disk.
            p_self can be a temporary object. In this case, "saving" consists in
            moving it to its "final" place.'''
         req = self.req
@@ -1308,15 +1321,15 @@
         # Create a validator: he will manage validation of request data
         validator = self.H().validator = Validator(self, saveConfirmed)
         r = validator.run()
         # If a result is returned, the "edit" page must be shown again:
         # validation failed or a confirmation is required.
         if r: return r
         # Update the object in the database
-        text = self.H().server.database.update(self, validator, initiator)
+        text = self.database.update(self, validator, initiator)
         # Recompute cached info on the guard: things may have changed
         guard = self.guard
         guard.cache()
         # If p_self has already been deleted ("text" being None in that case),
         # or if the logged user has lost the right to view it, redirect him to
         # its home page.
         if text is None or not guard.mayView(self):
@@ -1371,15 +1384,15 @@
             g = req._get_
             if g: params['_get_'] = g
             # Is the creation of the new object via the initiator allowed ?
             initiator.checkAllowed(log=True)
             # Let the initiator complete URL parameters when relevant
             initiator.updateParameters(params)
         # Create a temp object
-        o = handler.server.database.new(handler, className, temp=True)
+        o = self.database.new(handler, className, temp=True)
         # Populate p_o's edit form fields with a template object if present
         templateId = req.template
         if templateId: params['template'] = templateId
         # Call method "onCreate" if available. This method typically sets local
         # roles to the newly created object.
         if hasattr(o, 'onCreate'): o.onCreate()
         # Go to o's "edit" page
```

### Comparing `appy-1.0.8/py3/appy/model/batch.py` & `appy-1.0.9/py3/appy/model/batch.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/carousel.py` & `appy-1.0.9/py3/appy/model/carousel.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/document.py` & `appy-1.0.9/py3/appy/model/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,21 +45,22 @@
     #                               The file
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     do = {'label': 'Document'}
 
     def getMaxWidth(self):
         '''Get the maximum width for uploaded images. If the image is larger
            than this, it will be resized.'''
-        # The size depends on the container
+        # The size may be defined on the container
         try:
             container = self.container or self.initiator.o
         except AttributeError:
             # There is no container yet if the image is uploaded via ckeditor
             container = self.traversal.o
-        return '%dpx' % container.maxWidth
+        width = container.maxWidth if hasattr(container, 'maxWidth') else 700
+        return '%dpx' % width
 
     def getViewWidth(self):
         '''The width of the image as shown on the "view" layout varies depending
            on the it to be rendered in the popup or no.'''
         return '450px' if self.req.popup == 'True' else '700px'
 
     file = File(multiplicity=(1,1), isImage=True, resize=True, cache=True,
@@ -68,15 +69,15 @@
 
     # Its thumbnail
     thumb = File(isImage=True, resize=True, width='100px', show=Show.VE_, **do)
 
     def getCarousel(self):
         '''Returns the carousel into which this document is included'''
         container = self.container
-        if container and (container.class_.name == 'Carousel'):
+        if container and container.class_.name == 'Carousel':
             return container
 
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     #                  Elements to render on top of the file
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     # When used in a carousel, elements may be specified, that must be shown
```

### Comparing `appy-1.0.8/py3/appy/model/fields/__init__.py` & `appy-1.0.9/py3/appy/model/fields/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 # builtin types, use __builtins__['list'] and __builtins__['dict']
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 XSS_DETECTED = 'Detected Javascript in user input.'
 XSS_WARNING  = 'Your behaviour is considered a security attack. System ' \
                'administrator has been warned.'
 UNINDEXED    = 'Field "%s": cannot retrieve catalog version of unindexed field.'
+AJAX_EDITED  = 'Ajax-edited %s%s on %s.'
+METH_ERROR   = 'Method %s:\n%s'
+DEF_ERR      = 'Field "%s": error. %s.'
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Show:
     '''Provides some frequently used values for field's "show" attributes'''
     # As a convention, a trailing underscore indicates a negation
 
     # All layouts but edit. To use for users that can consult the field value
@@ -51,14 +54,16 @@
     # A variant, without "result"
     ER_ = ('view', 'xml')
     # A variant, with layout "buttons" instead of "result". "buttons"
     # corresponds, on lists, to the range of icons and/or buttons present in the
     # "title" column.
     E_B = ('view', 'buttons', 'xml')
     B = ('edit', 'view', 'buttons', 'xml')
+    # For some actions, being shown on "buttons" or "result" is appropriate
+    BR = ('buttons', 'result')
 
     # All layouts but view. To use typically when, on view, the field value is
     # already shown as a part of some custom widget.
     V_ = ('edit', 'result', 'xml')
     # All layouts but view and edit. To use when you need both E_ and V_.
     RX = VE_ = ('result', 'xml')
     # This set is used for showing workflow transitions in lists of objects
@@ -308,15 +313,15 @@
         <!-- Transitions -->
         <x if="class_.showTransitions(o, 'result')"
            var2="workflow=o.getWorkflow()">:workflow.pxTransitions</x>
 
         <!-- Edit -->
         <x if="editable">
          <a if="not locked"
-            var2="linkInPopup=popup or (target.target != '_self')"
+            var2="linkInPopup=popup or target.target != '_self'"
             target=":target.target"
             onclick=":target.getOnClick(backHook or str(o.iid))"
             href=":o.getUrl(sub='edit', page=o.getDefaultPage('edit'), \
                             nav=navInfo, popup=linkInPopup)">
           <img src=":url('edit.svg')" class="iconS" title=":_('object_edit')"/>
          </a>
          <x if="locked" var2="lockStyle='iconS'; page='main'">::o.Lock.px</x>
@@ -363,31 +368,26 @@
         return r
     
     pxValidation = Px(validationPx)
 
     # Displays the fact that a field is required
     pxRequired = Px(lambda c: '<span class="required">*</span>')
 
-    # Button for showing changes to the field
+    # Button for showing / hiding changes to the field
     pxChanges = Px('''
-     <div if="zobj.hasHistory(name)" style="margin-bottom: 5px">
-      <!-- Button for showing the field version containing changes -->
-      <input if="not showChanges"
-             var2="label=_('changes_show');
-                   css=ztool.getButtonCss(label)" type="button" class=":css"
-             value=":label" style=":url('changes', bg=True)"
-             onclick=":'askField(%s,%s,%s,null,%s)' % \
-                       (q(tagId), q(obj.url), q('view'), q('True'))"/>
-      <!-- Button for showing the field version without changes -->
-      <input if="showChanges"
-             var2="label=_('changes_hide');
-                  css=ztool.getButtonCss(label)" type="button" class=":css"
-             value=":label" style=":url('changesNo', bg=True)"
-             onclick=":'askField(%s,%s,%s,null,%s)' % \
-                       (q(tagId), q(obj.url), q('view'), q('False'))"/>
+     <div if="not o.history.isEmpty(name)" style="margin-bottom: 5px">
+      <input type="button"
+        var="suffix='hide' if showChanges else 'show';
+             label=_('changes_%s' % suffix);
+             css=ui.Button.getCss(label);
+             icon='changesNo' if showChanges else 'changes';
+             bp='False' if showChanges else 'True'"
+        class=":css" value=":label" style=":url(icon, bg=True)"
+        onclick=":'askField(%s,%s,%s,null,%s)' % (q(tagId), q(o.url),
+                                                  q('view'), q(bp))"/>
      </div>''')
 
     # Widget for filtering object values on query results
     pxFilterText = Px('''
      <x var="name=field.name;
              filterId='%s_%s' % (mode.hook, name);
              filterIdIcon='%s_icon' % filterId">
@@ -415,16 +415,16 @@
         self.multiplicity = multiplicity
         # Is the field required or not ? (derived from multiplicity)
         self.required = self.multiplicity[0] > 0
         # Default value
         self.default = default
         # Default value on layout "edit". If None, self.default is used instead.
         self.defaultOnEdit = defaultOnEdit
-        # Must the field be visible or not?
-        self.show = show
+        # Must the field be visible or not ?
+        self.show = show    
         # When displaying/editing the whole object, on what page and phase must
         # this field value appear ?
         if page:
             self.page = Page.get(page)
             self.pageName = self.page.name
         else:
             self.page = self.pageName = None
@@ -642,15 +642,15 @@
         name = '%s::%s' % (self.container.name, self.name) \
                if hasattr(self, 'container') else 'uninit'
         return '<field %s (%s)>' % (name, self.__class__.__name__.lower())
 
     def isMultiValued(self):
         '''Does this type definition allow to define multiple values?'''
         maxOccurs = self.multiplicity[1]
-        return (maxOccurs is None) or (maxOccurs > 1)
+        return maxOccurs is None or maxOccurs > 1
 
     def isSortable(self, inRefs=False):
         '''Can fields of this type be used for sorting purposes, when sorting
            search results (p_inRefs=False) or when sorting Ref fields
            (inRefs=True) ?'''
         if not inRefs:
             return self.indexed and (self.emptyIndexValue is not None) and \
@@ -667,15 +667,15 @@
         else:
             r = None, None
         return r
 
     def isShowable(self, o, layout):
         '''When displaying p_o on a given p_layout, must we show this field ?'''
         # Check if the user has the permission to view or edit the field
-        perm = self.writePermission if (layout=='edit') else self.readPermission
+        perm = self.writePermission if layout == 'edit' else self.readPermission
         if not o.allows(perm): return
         # Evaluate self.show
         if callable(self.show):
             r = self.callMethod(o, self.show)
         else:
             r = self.show
         # Take into account possible values 'view', 'edit', 'result', etc.
@@ -794,24 +794,24 @@
         # - if "masterValue" is anything but a method, the field will be shown
         #   only when the master has this value, or one of it if multivalued;
         # - if "masterValue" is a method, the value(s) of the slave field will
         #   be returned by this method, depending on the master value(s) that
         #   are given to it, as its unique parameter.
         self.masterValue = utils.initMasterValue(masterValue)
 
-    def getCss(self, layout, r):
+    def getCss(self, o, layout, r):
         '''Complete list p_r with the names of CSS files that are required for
            displaying widgets of self's type on a given p_layout. p_r is not a
            set because order of inclusion of CSS files may be important.'''
         if layout in self.cssFiles:
             for name in self.cssFiles[layout]:
                 if name not in r:
                     r.append(name)
 
-    def getJs(self, layout, r, config):
+    def getJs(self, o, layout, r, config):
         '''Completes list p_r with the names of Javascript files that are
            required for displaying widgets of self's type on a given p_layout.
            p_r is not a set because order of inclusion of Javascript files may
            be important.'''
         if layout in self.jsFiles:
             for name in self.jsFiles[layout]:
                 if name not in r:
@@ -856,31 +856,36 @@
             if fromRequest and (r is None): r = ''
         else:
             r = self.getRequestValue(o, self.name) if fromRequest \
                 else o.values.get(self.name)
         return r
 
     def getRequestValue(self, o, requestName=None):
-        '''Gets a value for this field as carried in the request. In the
-           simplest cases, the request value is a single value whose name in the
-           request is the name of the field.
-
-           Sometimes, several request values must be combined (ie: see the
-           overriden method in the Date class).
-
-           Sometimes (ie, a field within a List/Dict), the name of the request
-           value(s) representing the field value does not correspond to the
-           field name (ie: the request name includes information about
-           the container field). In this case, p_requestName must be used for
-           searching into the request, instead of the field name (self.name).'''
-        return o.req[requestName or self.name]
+        '''Gets a value for this field as carried in the request'''
+        #  In the simplest cases, the request value is a single value whose name
+        # in the request is the name of the field.
+
+        # Sometimes, several request values must be combined (ie: see the
+        # overriden method in the Date class).
+
+        # Sometimes (ie, a field within a List/Dict), the name of the request
+        # value(s) representing the field value does not correspond to the field
+        # name (ie: the request name includes information about the container
+        # field). In this case, p_requestName must be used for searching into
+        # the request, instead of the field name (self.name).
+
+        # Ensure multiplicities are respected
+        r = o.req[requestName or self.name]
+        if not isinstance(r, __builtins__['list']) and self.isMultiValued():
+            r = [] if r is None else [r]
+        return r
 
     def setRequestValue(self, o):
-        '''Sets, in the request, field value on p_obj in its "request" form
-           (=the way the value is carried in the request).'''
+        '''Sets, in the request, field value on p_o in its "request" form (=the
+           way the value is carried in the request).'''
         # Get a copy of the field value on p_obj and put it in the request
         value = self.getCopyValue(o)
         if value is not None:
             o.req[self.name] = value
 
     def getRequestSuffix(self):
         '''In most cases, in the user interface, there is one homonym HTML
@@ -932,19 +937,19 @@
                     # the process of creating an object from another one, or
                     # from some data, sometimes consists in (a) creating an
                     # "empty" object, (b) initializing its values and
                     # (c) reindexing it. Default values are computed in (a),
                     # but it they depend on values set at (b), and are cached
                     # and indexed, (c) will get the wrong, cached value.
                     default = self.callMethod(o, default, cache=False)
-                except Exception:
-                    # Already logged. Here I do not raise the exception,
-                    # because it can be raised as the result of reindexing
-                    # the object in situations that are not foreseen by
-                    # method in self.default.
+                except Exception as e:
+                    o.log(DEF_ERR % (self.name, str(e)), type='error')
+                    # Do not raise the exception, because it can be raised as
+                    # the result of reindexing the object in situations that are
+                    # not foreseen by v_default.
                     default = None
             return default
         return value
 
     def getValueIf(self, o, name, layout, disable=False):
         '''Special method only called by the framework. For some fields (or
            according to some p_disable condition), value retrieval as performed
@@ -1359,25 +1364,29 @@
                 o.history.historize(currentValues)
         else:
             # An inner field. No historization (yet) for it.
             part = ''
             # Retrieve the outer, inner fields and row number
             name, px = req.px.rsplit(':', 1)
             outer, inner, i = name.split('*')
+            i = int(i)
             outer = o.getField(outer)
-            # Update the value
+            # Update the value. Clone the row to ensure the ZODB will detect the
+            # object change. Indeed, rows are instances of not-persistent class
+            # appy.Object.
             value = outer.getValue(o)
-            row = value[int(i)]
+            row = value[i]
             setattr(row, inner, reqValue)
+            value[i] = row.clone()
             # Store the complete value again on p_o
             o.values[outer.name] = value
         # Update obj's last modification date
         o.modified = DateTime()
         o.reindex()
-        o.log('ajax-edited %s%s on %s.' % (self.name, part, o.id))
+        o.log(AJAX_EDITED % (self.name, part, o.id))
 
     def callMethod(self, o, method, cache=True):
         '''This method is used to call a p_method on p_o. p_method is part of
            this type definition (ie a default method, the method of a Computed
            field, a method used for showing or not a field...). Normally, those
            methods are called without any arg. But one may need, within the
            method, to access the related field. This method tries to call
@@ -1389,15 +1398,15 @@
             # additional parameter. In this case, we do not try to cache the
             # value (we do not call utils.callMethod), because the value may be
             # different depending on the parameter.
             tb = utils.Traceback.get()
             try:
                 return method(o, self)
             except Exception as e:
-                o.log('method %s:\n%s' % (method.__name__, tb), type='error')
+                o.log(METH_ERROR % (method.__name__, tb), type='error')
                 # Raise the initial error
                 raise te
 
     def getAttribute(self, o, name, cache=True):
         '''Gets the value of attribute p_name on p_self, which can be a simple
            value or the result of a method call on p_o.'''
         r = getattr(self, name)
```

### Comparing `appy-1.0.8/py3/appy/model/fields/action.py` & `appy-1.0.9/py3/appy/model/fields/action.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,30 @@
             self.backFromPopupUrl = msg
             r = None
         else:
             r = msg
         return r
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
+class Multi:
+    '''Management of muti-actions = actions that execute on a set of objects,
+       and not on a single one.'''
+
+    def __init__(self, back, check):
+        # The DOM node to ajax-refresh once the multi-action has been executed
+        self.back = back
+        # The DOM node storing the un/checked objects onto which the
+        # multi-action must be executed.
+        if check and ',' in check:
+            # This is a search being embedded into another field. In that
+            # case, the hook is simply 'search'.
+            check = 'search'
+        self.check = check
+
+#- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Action(Field):
     '''An action is a Python method that can be triggered by the user on a
        given Appy class. An action is rendered as a button or icon.'''
 
     # Some methods will be traversable
     traverse = {}
 
@@ -80,16 +96,16 @@
             '''Default layouts for this Action p_field'''
             return class_.b
 
     # PX for viewing the Action button
     view = cell = query = Px('''
      <form var="isFake=field.isFake(o, _);  
                 formId='%d_%s_form' % (o.iid, name);
-                label=_(field.labelId);
-                multi=multi|False;
+                label=_('label', field=field);
+                multi=multi|None;
                 className=className|o.class_.name;
                 inputTitle=field.getInputTitle(o, label);
                 inputLabel=field.getInputLabel(label, layout);
                 onCell=layout in field.cellLayouts;
                 picto=picto|'pictoB';
                 asPicto=not onCell and (picto != 'pictoB');
                 css=ui.Button.getCss(label, onCell, field.render)"
@@ -345,31 +361,27 @@
             # retrieve action's options.
             return '%s/new' % tool.url
         else:
             # Submitting the form will really trigger the action. Add the name
             # of the class in the path if p_self is a multi-action.
             part = '@%s/' % self.container.name if layout == 'query' else ''
             return '%s/%s%s/perform' % (o.url, part, self.name)
-    
+
     def getOnClick(self, o, name, req, layout, q, multi):
         '''Gets the JS code to execute when the action button is clicked'''
         # Determine the ID of the form to submit
         formId = '%d_%s_form' % (o.iid, name)
         # Determine the back hook and check hook (if multi)
         if multi:
-            back = 'searchResults'
-            check = req.search
-            if ',' in check:
-                # This is a search being embedded into another field. In that
-                # case, the hook is simply 'search'.
-                check = 'search'
-            check = q(check)
+            back = multi.back
+            check = multi.check
         else:
             back = str(o.iid) if layout == 'cell' else None
-            check = 'null'
+            check = None
+        check = q(check) if check else 'null'
         if not self.options:
             # Determine the parameters for executing the action
             showComment = 'true' if self.confirm == 'comment' else 'false'
             confirmText = self.getConfirmText(o)
             back = q(back) if back else 'null'
             # If the action produces a file, the page will not be refreshed. So
             # the action must remain visible: if, as it is done by default, it
@@ -386,30 +398,52 @@
         else:
             # Determine the parameters for creating an options instance
             target = LinkTarget(class_=self.options, forcePopup=True, back=back)
             js = '%s; submitForm(%s,null,null,null,%s)' % \
                  (target.onClick, q(formId), check)
         return js
 
+    def getTargetObjects(self, o, req):
+        '''In the context of a multi-action, retrieve the list of target objects
+           onto which the action must be applied.'''
+        # If semantics indicates that checked objects must be kept, retrieve
+        # these objects.
+        tool = o.tool
+        ids, unchecked = Search.getCheckedInfo(req)
+        if not unchecked:
+            r = []
+            for iid in ids:
+                cobj = tool.getObject(iid)
+                if cobj: # The object may have been deleted in the meanwhile
+                    r.append(cobj)
+            return r
+        # Get all the potential target objects, from a Search or Ref
+        searchParams = req.searchParams
+        if searchParams:
+            # Replay the search to get the list of objects
+            r = Search.replay(tool, searchParams)
+        else:
+            # Get objets from a ref
+            r = getattr(o, req.fieldName.split('*',1)[0])
+        # Remove those not being checked in the UI
+        Search.keepCheckedResults(req, r, unchecked=ids)
+        return r
+
     def execute(self, o, options=None):
         '''Execute the action on p_o. Returns a tuple (b_success, s_message)'''
         # Get args to give to method(s) in self.action
         args = {}
         req = o.req
         if options: args['options'] = options
         if self.confirm == 'comment':
             args['comment'] = o.req.popupComment
         # Is that a multi-action ? A multi-action is an action to perform on a
         # list of objects instead of a single object.
         if req.multi:
-            # Replay the search to get the list of objects
-            objects = Search.replay(o.tool, req.searchParams)
-            # Remove those not being checked in the UI
-            Search.keepCheckedResults(req, objects)
-            args['objects'] = objects
+            args['objects'] = self.getTargetObjects(o, req)
         # Call method(s) in self.action
         if type(self.action) in utils.sequenceTypes:
             # There are multiple methods
             r = [True, '']
             for act in self.action:
                 res = act(o, **args)
                 if type(res) in utils.sequenceTypes:
@@ -510,15 +544,15 @@
             header('Content-Disposition', '%s;filename="%s"' % \
                    (self.downloadDisposition, os.path.basename(msg.name)))
             msg.close()
         else:
             r = msg
         # Stop here if p_minimal is True
         if minimal: return r
-        if (result == 'computation') or not success:
+        if result == 'computation' or not success:
             # If we are called from an Ajax request, simply return msg
             if handler.isAjax():
                 r = msg
             else:
                 # The object may have been deleted by the action
                 exists = o.getObject(o.id)
                 url = o.tool.computeHomePage() if not exists else None
@@ -529,8 +563,14 @@
             # the user. Redirecting is different if we are in an Ajax request.
             if handler.isAjax():
                 o.resp.setHeader('Appy-Redirect', msg)
             else:
                 return o.goto(msg)
         else:
             return r
+
+    def getMulti(self, back, check):
+        '''In the context of a multi-action, create and return a Multi instance
+           defining useful info about the action, like the back and check
+           hooks.'''
+        return Multi(back, check)
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
```

### Comparing `appy-1.0.8/py3/appy/model/fields/boolean.py` & `appy-1.0.9/py3/appy/model/fields/boolean.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,34 +24,50 @@
 class Boolean(Field):
     '''Field for storing boolean values'''
     yesNo = {'true': 'yes', 'false': 'no', True: 'yes', False: 'no'}
     trueFalse = {True: 'true', False: 'false'}
 
     class Layouts(Layouts):
         '''Boolean-specific layouts'''
+        es = 'f;lrv;-'
+
         # Default layout (render = "checkbox") ("b" stands for "base"), followed
         # by the "grid" variant (if the field is in a group with "grid" style).
-        b   = Layouts(edit=Layout('f;lrv;-', width=None), view='lf')
-        g   = Layouts(edit=Layout('frvl', width=None), view='fl')
-        d   = Layouts(edit=Layout('flrv;=d', width=None), view='lf')
+
+        b   = Layouts(edit=Layout(es,        width=None),   view='lf')
+        g   = Layouts(edit=Layout('frvl',    width=None),   view='fl')
+        d   = Layouts(edit=Layout('flrv;=d', width=None),   view='lf')
+
         # *d*escription also visible on "view"
-        dv  = Layouts(edit=d['edit'], view='lf-d')
-        h   = Layouts(edit=Layout('flhv', width=None), view='lf')
-        gd  = Layouts(edit=Layout('f;dv-', width=None), view='fl')
+
+        dv  = Layouts(edit=d['edit'],                       view='lf-d')
+        h   = Layouts(edit=Layout('flhv',    width=None),   view='lf')
+        gd  = Layouts(edit=Layout('f;dv-',   width=None),   view='fl')
+
+        # The base layout, plus bottom space
+
+        bs = Layouts(edit=Layout(es,         width=None,
+                                 css_class='bottomSpaceS'), view='lf')
+
         # The "long" version of the previous layout (if the description is
         # long), with vertical alignment on top instead of middle.
-        gdl = Layouts(edit=Layout('f;dv=', width=None), view='fl')
+
+        gdl = Layouts(edit=Layout('f;dv=',   width=None),   view='fl')
+
         # Centered layout, no description
-        c   = Layouts(edit='flrv|', view='lf|')
+
+        c   = Layouts(edit='flrv|',                         view='lf|')
+
         # Layout for radio buttons (render = "radios")
-        r   = Layouts(edit='f', view='f')
-        rl  = Layouts(edit='l-f', view='lf')
-        rld = Layouts(edit='l-d-f', view='lf')
-        grl = Layouts(edit='fl', view='fl')
-        gdr = Layouts(edit=Layout('d-fv=', width=None), view='fl')
+
+        r   = Layouts(edit='f',                             view='f')
+        rl  = Layouts(edit='l-f',                           view='lf')
+        rld = Layouts(edit='l-d-f',                         view='lf')
+        grl = Layouts(edit='fl',                            view='fl')
+        gdr = Layouts(edit=Layout('d-fv=',   width=None),   view='fl')
 
         @classmethod
         def getDefault(class_, field):
             '''Default layouts for this Boolean p_field'''
             if field.render == 'radios': return class_.r
             return class_.g if field.inGrid() else class_.b
```

### Comparing `appy-1.0.8/py3/appy/model/fields/calendar.py` & `appy-1.0.9/py3/appy/model/fields/calendar.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,15 +405,17 @@
         # "initValue" is the initial value given to created Total instances
         self.initValue = initValue
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Layer:
     '''A layer is a set of additional data that can be activated or not on top
        of calendar data. Currently available for timelines only.'''
-    def __init__(self, name, label, onCell, activeByDefault=False, legend=None):
+
+    def __init__(self, name, label, onCell, activeByDefault=False, legend=None,
+                 merge=False):
         # "name" must hold a short name or acronym, unique among all layers
         self.name = name
         # "label" is a i18n label that will be used to produce the layer name in
         # the user interface.
         self.label = label
         # "onCell" must be a method that will be called for every calendar cell
         # and must return a 3-tuple (style, title, content). "style" will be
@@ -435,14 +437,17 @@
         # to this layer. The method must accept no arg and must return a list of
         # objects (you can use class appy.Object) having these attributes:
         # * name        - the legend item name as shown in the calendar
         # * style       - the content of the "style" attribute that will be
         #                 applied to the little square ("td" tag) for this item;
         # * content     - the content of this "td" (if any).
         self.legend = legend
+        # When p_merge is False, if the layer contains info for a given day, the
+        # base info will be hidden. Else, it will be merged.
+        self.merge = merge
         # Layers will be chained: one layer will access the previous one in the
         # stack via attribute "previous". "previous" fields will automatically
         # be filled by the Calendar.
         self.previous = None
 
     def getCellInfo(self, o, activeLayers, date, other, events, preComputed):
         '''Get the cell info from this layer or one previous layer when
@@ -816,15 +821,15 @@
                   mayValidate=mayValidate and other.mayValidate();
                   css=other.getCss()">
          <td class=":('tlLeft ' + css).strip()">::tlName</td>
          <!-- A cell in this other calendar -->
          <x for="date in grid"
             var2="inRange=field.dateInRange(date, startDate, endDate)">
           <td if="not inRange"></td>
-          <x if="inRange">::field.getTimelineCell(req, o, date, actions)</x>
+          <x if="inRange">::field.getTimelineCell(_ctx_, o, date, actions)</x>
          </x>
          <td class=":('tlRight ' + css).strip()">::tlName</td>
         </tr>
         <!-- The separator between groups of other calendars -->
         <x if="not loop.otherGroup.last">::field.getOthersSep(len(grid)+2)</x>
        </x>
       </tbody>
@@ -1000,23 +1005,22 @@
      <!-- Validate button, with checkbox for automatic checbox selection -->
      <x if="mayValidate" var2="cbId='%s_auto' % hook">
       <input if="mayValidate" type="button" value=":_('validate_events')"
              class="buttonSmall button" style=":url('validate', bg=True)"
              var2="js='validateEvents(%s,%s)' % (q(hook), q(month))"
              onclick=":'askConfirm(%s,%s,%s)' % (q('script'), q(js, False), \
                        q(_('validate_events_confirm')))"/>
-      <input type="checkbox" checked="checked" id=":cbId" class="smallbox"/>
+      <input type="checkbox" checked="checked" id=":cbId"/>
       <label lfor=":cbId" class="simpleLabel">:_('select_auto')</label>
      </x>
      <!-- Checkboxes for (de-)activating layers -->
      <x if="field.layers and field.layersSelector">
       <x for="layer in field.layers"
          var2="cbId='%s_layer_%s' % (hook, layer.name)">
-       <input type="checkbox" id=":cbId" class="smallbox"
-              checked=":layer.name in activeLayers"
+       <input type="checkbox" id=":cbId" checked=":layer.name in activeLayers"
               onclick=":'switchCalendarLayer(%s, this)' % q(hook)"/>
        <label lfor=":cbId" class="simpleLabel">:_(layer.label)</label>
       </x>
      </x>
      <x if="actions"> <!-- Custom actions -->
       <input for="action in actions" type="button" value=":_(action.label)"
              var2="js='calendarAction(%s,%s,comment)' % \
@@ -1503,96 +1507,102 @@
         '''Returns the name of some p_other calendar as must be shown in a
            timeline.'''
         if not self.timelineName:
             return '<a href="%s?month=%s">%s</a>' % \
                    (other.o.url, month, other.o.title)
         return self.timelineName(o, other, month, grid)
 
-    def getCellSelectParams(self, date, actions, cellContent, disable=False):
+    def getCellSelectParams(self, date, content):
         '''For a timeline cell, gets the parameters allowing to (de)select it,
            as a tuple ("onclick", "class") to be used as HTML attributes for
            the cell (td tag).'''
-        if disable or not actions: return '', ''
-        if not cellContent and not self.selectableEmptyCells: return '', ''
+        if not content and not self.selectableEmptyCells: return '', ''
         return ' onclick="onCell(this,\'%s\')"' % date.strftime('%Y%m%d'), \
                ' class="clickable"'
 
     def getColorFor(self, o, eventType, preCompute):
         '''Gets the background color for a cell containing some p_eventType'''
         colors = self.colors
         if colors is None:
             r = None
         elif isinstance(colors, dict):
             r = colors.get(eventType)
         else: # A method
             r = colors(o, eventType, preCompute)
         return r
 
-    def getTimelineCell(self, req, o, date, actions):
+    def buildTimelineCell(self, date, style, title, content, actions,
+                          disableSelect=False):
+        '''Called by m_getTimelineCell to build the final XHTML "td" tag
+           representing the timeline cell.'''
+        style = ' style="%s"' % style if style else ''
+        title = ' title="%s"' % title if title else ''
+        content = content or ''
+        if disableSelect or not actions:
+            onClick = css = ''
+        else:
+            onClick, css = self.getCellSelectParams(date, content)
+        return '<td%s%s%s%s>%s</td>' % (onClick, css, style, title, content)
+
+    def getTimelineCell(self, c, o, date, actions):
         '''Gets the content of a cell in a timeline calendar'''
         # Unwrap some variables from the PX context
-        c = req.pxContext
-        date = c['date']; other = c['other']; render = 'timeline'
-        allEventNames = c['allEventNames']; activeLayers = c['activeLayers']
+        date = c.date; other = c.other; render = 'timeline'; cache=c.preComputed
         # Get the events defined at that day, in the current calendar
-        events = self.getOtherEventsAt(date, other, allEventNames, render,
-                                       c['preComputed'], c['gradients'])
-        # In priority we will display info from a layer
-        if activeLayers:
+        events = self.getOtherEventsAt(date, other, c.allEventNames, render,
+                                       cache, c.gradients)
+        # Compute the cell attributes
+        style = title = content = None
+        # In priority, get info from layers
+        if c.activeLayers:
             # Walk layers in reverse order
             layer = self.layers[-1]
-            info = layer.getCellInfo(o, activeLayers, date, other, events,
-                                     c['preComputed'])
+            info = layer.getCellInfo(o, c.activeLayers, date,
+                                     other, events, cache)
             if info:
                 style, title, content = info
-                style = ' style="%s"' % style if style else ''
-                title = ' title="%s"' % title if title else ''
-                content = content or ''
-                onClick, css = self.getCellSelectParams(date, actions, content)
-                return '<td%s%s%s%s>%s</td>' % (onClick, css, style, title,
-                                                content)
+                if not layer.merge:
+                    # Exclusively display the layer info, ignoring the base info
+                    return self.buildTimelineCell(date, style, title,
+                                                  content, actions)
         # Define the cell's style
-        style = self.getCellStyle(o, date, render, events) or ''
-        if style: style = ' style="%s"' % style
+        style = style or self.getCellStyle(o, date, render, events)
         # If a timeline cell hides more than one event, put event names in the
         # "title" attribute.
-        title = ''
-        if len(events) > 1:
+        if not title and len(events) > 1:
             title = ', '.join(['%s (%s)' % (\
-              allEventNames.get(e.event.eventType) or '?', e.event.timeslot) \
+              c.allEventNames.get(e.event.eventType) or '?', e.event.timeslot) \
               for e in events])
-            title = ' title="%s"' % title
         # Define its content
-        content = ''
         disableSelect = False
-        if events and c['mayValidate']:
-            # If at least one event from p_events is in the validation schema,
-            # propose a unique checkbox, that will allow to validate or not all
-            # validable events at p_date.
-            for info in events:
-                if info.event.eventType in other.field.validation.schema:
-                    cbId = '%d_%s_%s' % (other.o.iid, other.field.name,
-                                         date.strftime('%Y%m%d'))
-                    totalRows = self.totalRows and 'true' or 'false'
-                    totalCols = self.totalCols and 'true' or 'false'
-                    content = '<input type="checkbox" checked="checked" ' \
-                      'class="smallbox" id="%s" onclick="onCheckCbCell(this,' \
-                      '\'%s\',%s,%s)"/>' % \
-                      (cbId, c['ajaxHookId'], totalRows, totalCols)
-                    # Disable selection if a validation checkbox is there
-                    disableSelect = True
-                    break
-        elif len(events) == 1:
-            # A single event: if not colored, show a symbol. When there are
-            # multiple events, a background image is already shown (see the
-            # "style" attribute), so do not show any additional info.
-            content = events[0].symbol or ''
-        onClick, css = self.getCellSelectParams(date, actions, content,
-                                                disableSelect)
-        return '<td%s%s%s%s>%s</td>' % (onClick, css, style, title, content)
+        if not content:
+            if events and c.mayValidate:
+                # If at least one event from p_events is in the validation
+                # schema, propose a unique checkbox, that will allow to validate
+                # or not all validable events at p_date.
+                for info in events:
+                    if info.event.eventType in other.field.validation.schema:
+                        cbId = '%d_%s_%s' % (other.o.iid, other.field.name,
+                                             date.strftime('%Y%m%d'))
+                        totalRows = 'true' if self.totalRows else 'false'
+                        totalCols = 'true' if self.totalCols else 'false'
+                        content = '<input type="checkbox" checked="checked" ' \
+                          'class="smallbox" id="%s" onclick="onCheckCbCell(' \
+                          'this,\'%s\',%s,%s)"/>' % \
+                          (cbId, c.hook, totalRows, totalCols)
+                        # Disable selection if a validation checkbox is there
+                        disableSelect = True
+                        break
+            elif len(events) == 1:
+                # A single event: if not colored, show a symbol. When there are
+                # multiple events, a background image is already shown (see the
+                # "style" attribute), so do not show any additional info.
+                content = events[0].symbol
+        return self.buildTimelineCell(date, style, title, content, actions,
+                                      disableSelect=disableSelect)
 
     def getTimelineMonths(self, grid, o, preComputed):
         '''Given the p_grid of dates, this method returns the list of
            corresponding months.'''
         r = []
         for date in grid:
             if not r:
```

### Comparing `appy-1.0.8/py3/appy/model/fields/color.py` & `appy-1.0.9/py3/appy/model/fields/color.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/fields/colset.py` & `appy-1.0.9/py3/appy/model/fields/colset.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/fields/computed.py` & `appy-1.0.9/py3/appy/model/fields/computed.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/fields/custom.py` & `appy-1.0.9/py3/appy/model/fields/custom.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/fields/date.py` & `appy-1.0.9/py3/appy/model/fields/date.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,21 +216,21 @@
         Field.__init__(self, validator, multiplicity, default, defaultOnEdit,
           show, page, group, layouts, move, indexed, mustIndex, indexValue,
           emptyIndexValue, searchable, filterField, readPermission,
           writePermission, width, height, None, colspan, master, masterValue,
           focus, historized, mapping, generateLabel, label, sdefault, scolspan,
           swidth, sheight, persist, False, view, cell, edit, xml, translations)
 
-    def getCss(self, layout, r):
+    def getCss(self, o, layout, r):
         '''CSS files are only required if the calendar must be shown'''
-        if self.calendar: Field.getCss(self, layout, r)
+        if self.calendar: Field.getCss(self, o, layout, r)
 
-    def getJs(self, layout, r, config):
+    def getJs(self, o, layout, r, config):
         '''Javascript files are only required if the calendar must be shown'''
-        if self.calendar: Field.getJs(self, layout, r, config)
+        if self.calendar: Field.getJs(self, o, layout, r, config)
 
     def getSelectableYears(self, o):
         '''Gets the list of years one may select for this field'''
         startYear = self.getAttribute(o, 'startYear')
         r = range(startYear, self.endYear + 1)
         if self.reverseYears: r.reverse()
         return r
```

### Comparing `appy-1.0.8/py3/appy/model/fields/dict.py` & `appy-1.0.9/py3/appy/model/fields/dict.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,20 +68,21 @@
 
     # PX for rendering the dict (shared between pxView and pxEdit)
     pxTable = Px('''
      <table var="isEdit=layout == 'edit'" if="isEdit or value"
             id=":'list_%s' % name" class="grid" width=":field.width"
             var2="keys=field.keys(o);
                   subFields=field.getSubFields(o, layout);
+                  swidths=field.getWidths(subFields);
                   o=alto|o">
       <!-- Header -->
       <tr valign="bottom">
-       <th width=":field.widths[0]"></th>
+       <th width=":swidths[0]"></th>
        <th for="subName, sub in subFields" if="sub"
-           width=":field.widths[loop.subName.nb + 1]">::_(sub.labelId)</th>
+           width=":swidths[loop.subName.nb + 1]">::sub.getListHeader(_ctx_)</th>
       </tr>
       <!-- Rows of data -->
       <x for="rowId, text in keys">:field.pxRow</x>
      </table>''')
 
     def __init__(self, keys, fields, validator=None, multiplicity=(0,1),
       default=None, defaultOnEdit=None, show=True, page='main', group=None,
@@ -106,17 +107,17 @@
         # For a nice rendering of your dict, some of the tuples returned by
         # method "keys" can be "separator rows". The tuple representing such a
         # row must have the form (None, sepRow). "None" indicates that this is
         # not a row of data; "sepRow" must be a SepRow instance (see hereabove)
         # that will determine content and style for the separator row.
         self.keys = keys
 
-    def computeWidths(self, widths):
-        '''Set given p_widths or compute default ones if not given'''
-        self.widths = widths or ([''] * (len(self.fields) + 1))
+    def getWidths(self, subFields):
+        '''Get the widths to appply to these p_subFields'''
+        return self.widths or [''] * (len(subFields) + 1)
 
     def getStorableValue(self, o, value, single=False):
         '''Gets p_value in a form that can be stored in the database'''
         r = PersistentMapping()
         for k, v in value.items():
             r[k] = self.getStorableRowValue(o, v)
         return r
@@ -154,15 +155,15 @@
                     dbValue[key].update(data)
                     # Force the mapping to take the change into account
                     dbValue[key] = dbValue[key]
 
     def subValidate(self, o, value, errors):
         '''Validates inner fields'''
         for key, row in value.items():
-            for name, subField in self.fields:
+            for name, subField in self.getSubFields(o):
                 message = subField.validate(o, getattr(row, name, None))
                 if message:
                     setattr(errors, '%s*%s' % (subField.name, key), message)
 
     def getDiffSubValue(self, old, new, texts):
         '''Produce a diff between this p_old sub-value and its p_new version.
            p_texts contain precomputed translated texts about the user that
```

### Comparing `appy-1.0.8/py3/appy/model/fields/file.py` & `appy-1.0.9/py3/appy/model/fields/file.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/fields/float.py` & `appy-1.0.9/py3/appy/model/fields/float.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/fields/group.py` & `appy-1.0.9/py3/appy/model/fields/group.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/fields/hour.py` & `appy-1.0.9/py3/appy/model/fields/hour.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/fields/info.py` & `appy-1.0.9/py3/appy/model/fields/info.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License along with
 # Appy. If not, see <http://www.gnu.org/licenses/>.
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
-from appy.ui.layout import Layout, Layouts
 from appy.model.fields import Field
+from appy.ui.layout import Layout, Layouts
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Info(Field):
     '''An info is a field whose purpose is to present information
        (text, html...) to the user.'''
 
     class Layouts(Layouts):
```

### Comparing `appy-1.0.8/py3/appy/model/fields/integer.py` & `appy-1.0.9/py3/appy/model/fields/integer.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/fields/list.py` & `appy-1.0.9/py3/appy/model/fields/list.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,22 +129,23 @@
     # PX for rendering the list (shared between pxView, pxEdit and pxCell)
     pxTable = Px('''
      <table var="isEdit=layout == 'edit';
                  isCell=layout == 'cell';
                  tableId='list_%s' % name" if="isEdit or value"
             id=":tableId" width=":field.width" class="grid"
             var2="subFields=field.getSubFields(o, layout);
+                  swidths=field.getWidths(subFields);
                   totals=field.createTotals(isEdit);
                   showTotals=not isEdit and totals">
       <!-- Header -->
       <thead>
        <tr valign="middle">
         <th if="showTotals"></th>
         <th for="name, sub in subFields" if="sub"
-            width=":field.widths[loop.name.nb]">
+            width=":swidths[loop.name.nb]">
          <x var="field=sub">::field.getListHeader(_ctx_)</x></th>
         <!-- Icon for adding a new row -->
         <th if="isEdit">
          <img class="clickable" src=":url('plus')" title=":_('object_add')"
               onclick=":'insertRow(%s)' % q(tableId)"/>
         </th>
        </tr>
@@ -309,59 +310,87 @@
         Field.__init__(self, validator, multiplicity, default, defaultOnEdit,
          show, page, group, layouts, move, False, True, None, None, False, None,
          readPermission, writePermission, width, height, None, colspan, master,
          masterValue, focus, historized, mapping, generateLabel, label, None,
          None, None, None, True, False, view, cell, edit, xml, translations)
         self.validable = True
         # Tuple of elements of the form (name, Field instance) determining the
-        # format of every element in the list.
+        # format of every element in the list. It can also be a method returning
+        # this tuple. In that case, however, no i18n label will be generated for
+        # the sub-fields: these latters must be created with a value for
+        # attribute "translations".
         self.fields = fields
-        # Force some layouting for sub-fields, if subLayouts are given. So the
-        # one who wants freedom on tuning layouts at the field level must
-        # specify subLayouts=None.
-        if subLayouts:
-            for name, field in self.fields:
-                field.layouts = subLayouts
+        # Force some layouting for sub-fields, if p_subLayouts are passed. If
+        # you want freedom to tune layouts at the field level, you must specify
+        # p_subLayouts=None.
+        self.subLayouts = subLayouts
         # One may specify the width of every column in the list. Indeed, using
-        # widths and layouts of sub-fields may not be sufficient.
-        self.computeWidths(widths)
+        # widths and layouts at the sub-field level may not be sufficient.
+        self.widths = widths
+        # Initialize sub-fields, if statically known
+        if not callable(fields):
+            self.initSubFields(fields)
         # When deleting a row, must we display a popup for confirming it ?
         self.deleteConfirm = deleteConfirm
         # If you want to specify additional rows representing totals, give in
         # "totalRows" a list of Totals instances (see above).
         self.totalRows = totalRows or []
 
+    def initSubFields(self, subFields):
+        '''Initialises sub-fields' attributes'''
+        # Initialise sub-layouts
+        subLayouts = self.subLayouts
+        if subLayouts:
+            for name, field in subFields:
+                field.layouts = Layouts.getFor(self, subLayouts)
+
+    def lazyInitSubFields(self, subFields, class_):
+        '''Lazy-initialise sub-fields, when known'''
+        # It can be at server startup, if sub-fields are statically defined, or
+        # everytime a List field is solicited, if sub-fields are dynamically
+        # computed.
+        for sub, field in subFields:
+            fullName = '%s_%s' % (self.name, sub)
+            field.init(class_, fullName)
+            field.name = '%s*%s' % (self.name, sub)
+
     def init(self, class_, name):
         '''List-specific lazy initialisation'''
         Field.init(self, class_, name)
-        for sub, field in self.fields:
-            fullName = '%s_%s' % (name, sub)
-            field.init(class_, fullName)
-            field.name = '%s*%s' % (name, sub)
-
-    def computeWidths(self, widths):
-        '''Set given p_widths or compute default ones if not given'''
-        self.widths = widths or ([''] * len(self.fields))
+        subs = self.fields
+        if not callable(subs):
+            self.lazyInitSubFields(subs, class_)
+
+    def getWidths(self, subFields):
+        '''Get the widths to appply to these p_subFields'''
+        return self.widths or [''] * len(subFields)
 
     def getField(self, name):
         '''Gets the field definition whose name is p_name'''
         for n, field in self.fields:
             if n == name: return field
 
-    def getSubFields(self, o, layout):
-        '''Returns the sub-fields (name, Field) that are showable among
-           field.fields on the given p_layout. Fields that cannot appear in
-           the result are nevertheless present as a tuple (name, None). This
-           way, it keeps a nice layouting of the table.'''
+    def getSubFields(self, o, layout=None):
+        '''Returns the sub-fields, as a list of tuples ~[(s_name, Field)]~,
+           being showable, among p_self.fields on this p_layout. Fields that
+           cannot appear in the result are nevertheless present as a tuple
+           (s_name, None). This way, it keeps a nice layouting of the table.'''
+        fields = self.fields
+        if callable(fields):
+            # Dynamically computed fields: get and completely initialise them
+            fields = self.getAttribute(o, 'fields') # Involves caching
+            self.initSubFields(fields)
+            self.lazyInitSubFields(fields, o.class_)
+        # Stop here if no p_layout is passed
+        if layout is None: return fields
+        # Retain only sub-fields being showable on this p_layout
         r = []
-        for n, field in self.fields:
-            elem = (n, None)
-            if field.isShowable(o, layout):
-                elem = (n, field)
-            r.append(elem)
+        for n, field in fields:
+            f = field if field.isShowable(o, layout) else None
+            r.append((n, f))
         return r
 
     def getRequestValue(self, o, requestName=None):
         '''Concatenates the list from distinct form elements in the request'''
         req = o.req
         name = requestName or self.name # A List may be into another List (?)
         prefix = name + '*-row-*' # Allows to detect a row of data for this List
@@ -369,15 +398,15 @@
         isDict = True # We manage both List and Dict
         for key in req.keys():
             if not key.startswith(prefix): continue
             # I have found a row: get its index
             row = O()
             rowId = key.split('*')[-1]
             if rowId == '-1': continue # Ignore the template row
-            for subName, subField in self.fields:
+            for subName, subField in self.getSubFields(o):
                 keyName = '%s*%s*%s' % (name, subName, rowId)
                 if keyName + subField.getRequestSuffix() in req:
                     v = subField.getRequestValue(o, requestName=keyName)
                     setattr(row, subName, v)
             if rowId.isdigit():
                 rowId = int(rowId)
                 isDict = False
@@ -410,26 +439,27 @@
                     req[key] = v
                 i += 1
 
     def getStorableRowValue(self, o, requestValue):
         '''Gets a ready-to-store Object instance representing a single row,
            from p_requestValue.'''
         r = O()
-        for name, field in self.fields:
+        for name, field in self.getSubFields(o):
             if not hasattr(requestValue, name) and \
                not field.isShowable(o, 'edit'):
                 # Some fields, although present on "edit", may not be part of
                 # the p_requestValue (ie, a "select multiple" with no value at
                 # all will not be part of the POST HTTP request). If we want to
                 # know if the field was in the request or not, we must then
                 # check if it is showable on layout "edit".
                 continue
             subValue = getattr(requestValue, name, None)
             try:
-                setattr(r, name, field.getStorableValue(o, subValue))
+                setattr(r, name,
+                        field.getStorableValue(o, subValue, single=True))
             except ValueError:
                 # The value for this field for this specific row is incorrect.
                 # It can happen in the process of validating the whole List
                 # field (a call to m_getStorableValue occurs at this time). We
                 # don't care about it, because later on we will have sub-field
                 # specific validation that will also detect the error and will
                 # prevent storing the wrong value in the database.
@@ -441,35 +471,37 @@
         return [self.getStorableRowValue(o, v) for v in value]
 
     def getCopyValue(self, o):
         '''Return a (deep) copy of field value on p_obj''' 
         r = getattr(o, self.name, None)
         if r: return copy.deepcopy(r)
 
-    def getCss(self, layout, r):
+    def getCss(self, o, layout, r):
         '''Gets the CSS required by sub-fields if any'''
-        for name, field in self.fields:
-            field.getCss(layout, r)
+        for name, field in self.getSubFields(o, layout):
+            if field:
+                field.getCss(o, layout, r)
 
-    def getJs(self, layout, r, config):
+    def getJs(self, o, layout, r, config):
         '''Gets the JS required by sub-fields if any'''
-        for name, field in self.fields:
-            field.getJs(layout, r, config)
+        for name, field in self.getSubFields(o, layout):
+            if field:
+                field.getJs(o, layout, r, config)
 
     def jsDeleteConfirm(self, q, tableId):
         '''Gets the JS code to call when the user wants to delete a row'''
         confirm = 'true' if self.deleteConfirm else 'false'
         return 'deleteRow(%s,this,%s)' % (q(tableId), confirm)
 
     def subValidate(self, o, value, errors):
         '''Validates inner fields'''
         i = -1
         for row in value:
             i += 1
-            for name, subField in self.fields:
+            for name, subField in self.getSubFields(o):
                 message = subField.validate(o, getattr(row, name, None))
                 if message:
                     setattr(errors, '%s*%d' % (subField.name, i), message)
 
     def createTotals(self, isEdit):
         '''When rendering the List field, if total rows are defined, create a
            Total instance for every sub-field for which a total must be
```

### Comparing `appy-1.0.8/py3/appy/model/fields/multilingual.py` & `appy-1.0.9/py3/appy/model/fields/multilingual.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,29 +29,22 @@
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Multilingual:
     '''Mixin class injected into any Field whose content can be multilingual'''
 
     # Default values to render when field values are empty
     emptyDefault = {'view': '-', 'edit': '', 'cell': ''}
-    # Default top space (in pixels) to apply in pxLanguage
-    lgTop = {'view': 1, 'edit': 3, 'cell': 3}
+
+    # Mapping between Appy and flex directions
+    directions = {'horizontal': 'row', 'vertical': 'column'}
 
     # Note that multilinguality is a dynamic feature: field values can be
     # unilingual or multilingual, depending on some condition on the container
     # object itself, or on some site-specific configuration.
 
-    # PX displaying the language code and name besides the part of the
-    # multilingual field storing content in this language.
-    pxLanguage = Px('''
-     <td style=":'padding-top:%dpx' % field.lgTop[layout]" width="25px">
-      <span class="language help"
-            title=":ui.Language.getName(lg)">:lg.upper()</span>
-     </td>''')
-
     # PX acting as a substitute for the field pxView. This PX determines if the
     # field content is multilingual or not. If the field is unilingual, it
     # simply calls a PX named "<layoutType>Uni" on the field. Else, it renders
     # such a PX for every supported language, calling "<layoutType>Uni" for
     # every language, and assembling the result according to the "languages
     # layout". The "Uni" PX receives the current language as variable "lg". If
     # the field is unilingual, the received "lg" variable is None.
@@ -60,37 +53,32 @@
              multilingual=len(languages) &gt; 1;
              pxUni=getattr(field, '%sUni' % layout)">
 
       <!-- Display the uni-lingual version of the field -->
       <x if="not multilingual" var2="lg=None">:pxUni</x>
 
       <!-- Display the multi-lingual version of the field -->
-      <x if="multilingual"
-         var2="languageLayout=field.getLanguagesLayout(layout)">
-
-       <!-- Horizontally-layouted multilingual field -->
-       <table if="languageLayout == 'horizontal'" width="100%"
-              class=":(layout == 'cell') and 'no' or ''"
-              var="count=len(languages)">
-        <tr valign="top"><x for="lg in languages"><x>:field.pxLanguage</x>
-         <td width=":'%d%%' % int(100.0/count)"
-             var="requestValue=requestValue[lg]|None;
-                  value=value[lg]|field.emptyDefault[layout]">:pxUni</td>
-        </x></tr></table>
-
-       <!-- Vertically-layouted multilingual field -->
-       <table if="languageLayout == 'vertical'"
-              class=":(layout == 'cell') and 'no' or ''">
-        <tr valign="top" height="20px" for="lg in languages">
-         <x>:field.pxLanguage</x>
-         <td var="requestValue=requestValue[lg]|None;
-                  value=value[lg]|field.emptyDefault[layout]">:pxUni</td>
-       </tr></table>
-      </x>
-     </x>''')
+      <div if="multilingual" class="lgMulti"
+           var2="direction=field.getLayoutDirection(layout)"
+           style=":'flex-direction:%s' % direction">
+       <div for="lg in languages">
+        <div class="language help"
+             title=":ui.Language.getName(lg)">:lg.upper()</div>
+        <div var="requestValue=requestValue[lg]|None;
+                value=value[lg]|field.emptyDefault[layout]">:pxUni</div>
+       </div>
+      </div>
+     </x>''',
+
+     css='''
+      .lgMulti { display:inline-flex; column-gap:20px }
+      .lgMulti > div { display:flex; flex-wrap:nowrap; align-items:flex-start }
+      .language {
+        color:|darkColor|; font-size:7pt; border:|darkColor| 1px solid;
+        padding:4px; margin:2px 10px 0 0; font-family:monospace }''')
 
     def __init__(self, languages, languagesLayouts):
         '''Inject multilingual-specific attributes on p_self'''
         # If "languages" holds more than one language, the field will be
         # multi-lingual and several widgets will allow to edit/visualize the
         # field content in all the supported languages. The field is also used
         # by the CK spell checker.
@@ -106,20 +94,21 @@
         if not o:
             if callable(self.languages):
                 # In that case, it is impossible to know
                 return dontKnow
             else: return len(self.languages) > 1
         return len(self.getAttribute(o, 'languages')) > 1
 
-    def getLanguagesLayout(self, layout):
-        '''Gets the way to render a multilingual field on p_layoutType.'''
-        if self.languagesLayouts and (layout in self.languagesLayouts):
-            return self.languagesLayouts[layout]
+    def getLayoutDirection(self, layout):
+        '''Gets the way to render a multilingual field on this p_layout'''
+        layouts = self.languagesLayouts
+        if layouts and layout in layouts:
+            return Multilingual.directions[layouts[layout]]
         # Else, return a default value that depends of the format
-        return self.defaultLanguagesLayouts[layout]
+        return Multilingual.directions[self.defaultLanguagesLayouts[layout]]
 
     def getCopyValue(self, o):
         '''A value being multilingual is stored in a dict. For such a value,
            standard method Field.getCopyValue must return a distinct copy of the
            value as stored on p_obj.'''
         r = self.getValue(o)
         if isinstance(r, dict): r = r.copy()
@@ -228,18 +217,19 @@
         # Be careful: p_language represents the UI language, while variable
         # "languages" below represents the content language(s) of this field.
         languages = self.getAttribute(o, 'languages')
         uni = self.getUniFormattedValue
         if len(languages) == 1:
             return uni(o, value, layout, showChanges, language=language)
         if not value: return value
-        # Try to propose the part that is in the user language, or the part of
-        # the first content language else.
-        lg = o.guard.userLanguage
-        if lg not in value: lg = languages[0]
+        # Manage a multilingual value. Try to propose the part that is in the
+        # user language (or some forced p_language). If it does not exist or is
+        # empty, return the part of the first content language.
+        lg = language or o.guard.userLanguage
+        if lg not in value or not value[lg]: lg = languages[0]
         return uni(o, value[lg], layout, showChanges, language=lg)
 
     def getIndexValue(self, o, searchable=False, raw=False):
         '''Multilingual variant of Field::getIndexValue. Language parts must be
            concatenated into a single value before being indexed.'''
         r = Field.getIndexValue(self, o, searchable=searchable, raw=True)
         if not r: return
```

### Comparing `appy-1.0.8/py3/appy/model/fields/ogone.py` & `appy-1.0.9/py3/appy/model/fields/ogone.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,40 +20,51 @@
 from appy.px import Px
 from appy.utils import asDict
 from appy.model.fields import Field
 from appy.model.utils import Object as O
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 PARAM_EMPTY = 'Ogone: parameter "%s" has no value and has been ignored.'
-RESP_KO     = 'Ogone response SHA failed. Params: %s'
-RESP_KO_ERR = 'Failure, fraud? An administrator has been contacted.'
+RESP_OK     = '%d - Ogone answered: %s'
+RESP_KO     = '%d - Ogone response SHA failed. Params: %s'
+RESP_KO_ERR = 'An administrator has been contacted.'
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Config:
     '''If you plan, in your app, to perform on-line payments via the Ingenico
        ePayments e-Commerce system (previouly named Ogone), create an instance
        of this class in your app and place it in the 'ogone' attr of your app's
        Config class.'''
 
     # The URL to redirect the user to for performing an on-line payment
-    payUrl = 'https://ogone.%s.v-psp.com/ncol/%s/orderstandard_utf8.asp'
+    payUrls = {
+      'test': 'https://ogone.test.v-psp.com/ncol/test/orderstandard_utf8.asp',
+      'prod': 'https://secure.ogone.com/ncol/prod/orderstandard_utf8.asp'
+    }
 
     # Fields below are those that must be sent in every request to Ogone
     sendable = ('pspid', 'currency', 'language')
 
     # Default parameters sent back by Ingenico to your app, after a payment has
     # been performed, being part of the HTTP GET request (payment accepted,
     # refused, etc).
+
+    # ! Compared to the predefined list as defined by Ingenico, params "CN" and
+    # "BRAND" have been removed. Indeed, it may contains spaces; these spaces
+    # are converted by Ingenico into + signs, but Appy does not convert them
+    # back to spaces for HTTP GET requests.
+
     defaultBackParams = asDict(
-      ('ORDERID', 'CURRENCY', 'AMOUNT', 'PM', 'ACCEPTANCE', 'STATUS', 'CARDNO',
-       'ED', 'CN', 'TRXDATE', 'PAYID', 'PAYIDSUB', 'NCERROR', 'BRAND', 'IPCTY',
-       'CCCTY', 'ECI', 'CVCCHECK', 'AAVCHECK', 'VC', 'DCC_INDICATOR',
-       'DCC_EXCHRATE', 'DCC_EXCHRATETS', 'DCC_CONVCCY', 'DCC_CONVAMOUNT',
-       'DCC_VALIDHOURS', 'DCC_EXCHRATESOURCE', 'DCC_MARGINPERCENTAGE',
-       'DCC_COMMPERCENTAGE', 'IP')
+      ('AAVCHECK', 'ACCEPTANCE', 'ALIAS', 'AMOUNT', 'CARDNO', 'CCCTY',
+       'COMPLUS', 'CREATION_STATUS', 'CURRENCY', 'CVCCHECK',
+       'DCC_COMMPERCENTAGE', 'DCC_CONVAMOUNT', 'DCC_CONVCCY', 'DCC_EXCHRATE',
+       'DCC_EXCHRATESOURCE', 'DCC_EXCHRATETS', 'DCC_INDICATOR',
+       'DCC_MARGINPERCENTAGE', 'DCC_VALIDHOURS', 'ECI', 'ED', 'IP', 'IPCTY',
+       'NCERROR', 'ORDERID', 'PAYID', 'PAYIDSUB', 'PM', 'STATUS',
+       'SUBSCRIPTION_ID', 'TRXDATE', 'VC')
     )
 
     def __init__(self):
         # self.env refers to the Ogone environment and can be "test" or "prod"
         self.env = 'test'
         # You merchant Ogone ID
         self.pspid = None
@@ -90,33 +101,33 @@
     traverse = Field.traverse.copy()
 
     urlTypes = ('accept', 'decline', 'exception', 'cancel')
 
     # Return status codes
     statuses = {
      '0': 'payment_abandoned', # Abandoned or aborted for an unknown reason
-     '1': 'payment_canceled',  # Canceled by the customer
-     '2': 'payment_refused',   # Payment refused
-     '5': 'payment_accepted',  # Payment authorized (in a 2-step process)
-     '9': 'payment_accepted',  # Payment accepted
+     '1': 'payment_canceled' , # Canceled by the customer
+     '2': 'payment_refused'  , # Payment refused
+     '5': 'payment_accepted' , # Payment authorized (in a 2-step process)
+     '9': 'payment_accepted' , # Payment accepted
     }
 
     # The "view" and "cell" layouts are used to display a button for performing
     # an on-line payment.
     # ~~~
     # Note that variable "value" may not be present in the context, because, if
     # the field is shown on layout "buttons", on lists of objects, caller fields
     # like Ref calls directly field.cell instead of field.pxRender.
     view = cell = Px('''
      <!-- The form for sending the payment request to Ogone.
           Variable "value" is misused and contains payment parameters. -->
 
      <form var="env=config.ogone.env; label=_('pay')"
            method="post" id="form1" name="form1"
-           action=":config.ogone.payUrl % (env, env)" class="inline">
+           action=":config.ogone.payUrls[env]" class="inline">
 
        <!-- The list of hidden fields required by Ogone -->
        <input type="hidden" for="key,val in value.items()"
               id=":key" name=":key" value=":val"/>
 
        <!-- Submit button on most layouts -->
        <input if="layout != 'view'" type="submit" id="submit2" name="submit2"
@@ -235,30 +246,32 @@
     def getBackParameters(self, req, configParams):
         '''Extracts, from the request, Ingenico-related parameters'''
         r = O()
         for name, value in req.items():
             # Upperize the name of the parameter
             name = name.upper()
             # Keep it only if mentioned in the config and not empty
-            if (name not in configParams) or not value: continue
+            if not value or name not in configParams: continue
             setattr(r, name, value)
         return r
 
     traverse['process'] = 'perm:read'
     def process(self, o):
         '''Processes a response from Ogone'''
         # Get parameters from the request sent back by Ingenico
         cfg = o.config.ogone
         req = o.req
         params = self.getBackParameters(req, cfg.backParams)
-        # Call the response method defined in this Ogone field
+        sparams = str(params)
+        # Log and check the response
         if not self.ogoneResponseOk(req.SHASIGN, cfg.shaOutKey, params):
-            o.log(RESP_KO % str(params))
+            o.log(RESP_KO % (o.iid, sparams))
             raise Exception(RESP_KO_ERR)
-        # Call the field method handling the response received from Ogone.
-        # Redirect the user to the correct page. If the field method returns
-        # some URL, use it. Else, use the p_o's view URL.
+        o.log(RESP_OK % (o.iid, sparams))
+        # Handle the Ogone response by calling the response method defined in
+        # this Ogone field, and redirect the user to the correct page. If the
+        # field method returns some URL, use it. Else, use the p_o's view URL.
         url, message = self.responseMethod(o, params)
         url = url or o.url
         o.H().commit = True
         o.goto(url, message)
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
```

### Comparing `appy-1.0.8/py3/appy/model/fields/password.py` & `appy-1.0.9/py3/appy/model/fields/password.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/fields/phase.py` & `appy-1.0.9/py3/appy/model/fields/phase.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,16 +226,16 @@
 
     view = Px('''
      <div class=":'phase phaseC' if compact else 'phase'"
           if="phase.showPages(singlePhase, isEdit)">
 
       <!-- Siblings navigation -->
       <div var="nav=req.nav"
-           if="not isEdit and (phase.name=='main') and (nav) and (nav != 'no')"
-           var2="self=ui.Siblings.get(nav, tool, _ctx_)">:self.pxNavigate</div>
+        if="not isEdit and phase.name == 'main' and nav and nav != 'no'"
+        var2="self=ui.Siblings.get(nav,tool,_ctx_)">:self.pxNavigate|'⚠'</div>
 
       <!-- Page(s) within the phase -->
       <div if="not isEdit" for="pag in phase.pages.values()"
            var2="isCurrent=pag.name == page"
            id=":'currentPage' if isCurrent else ''"
            class=":'currentPage' if isCurrent else ''">
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `appy-1.0.8/py3/appy/model/fields/pod.py` & `appy-1.0.9/py3/appy/model/fields/pod.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/fields/python.py` & `appy-1.0.9/py3/appy/model/fields/python.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/fields/ref.py` & `appy-1.0.9/py3/appy/model/fields/ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,16 +213,16 @@
              page=pageName, popup=popup, selectJs=selectJs)</x>
       <x if="not selectable">
        <span style=":showSubTitles and 'display:inline' or 'display:none'"
              name="subTitle" class=":tiedClass.getCssFor(o, 'subTitle')"
              var="sub=ifield.getSubTitle(initiator.o, o)" if="sub">::sub</span>
       </x></x>''')
 
-    # This PX displays buttons for triggering global actions on several linked
-    # objects (delete many, unlink many,...)
+    # Buttons triggering global actions on several linked objects: delete many,
+    # unlink many, etc.
     pxGlobalActions = Px('''
      <div class="globalActions">
 
       <!-- Insert several objects (if in pick list) -->
       <input if="inPickList"
              var2="action='link'; label=_('object_link_many');
                    css=ui.Button.getCss(label)"
@@ -255,18 +255,26 @@
              var="label=_('object_link_many'); css=ui.Button.getCss(label)"
              value=":label" class=":css"
              style=":url('linkMany.svg', bg='18px 18px')"
              onclick=":'onSelectObjects(%s,%s,%s,%s,%s)' %
               (q('%d_%s' % (o.iid, field.name)), q(selector.initiatorHook),
                q(selector.initiator.url), q(selector.initiatorMode),
                q(selector.onav))"/>
+
+      <!-- Custom actions -->
+      <x if="not popup">
+       <div for="action in field.getActions(o)"
+            var2="checkHook='%d_%s' % (o.iid, field.name);
+                  fieldName='%s*%s' % (field.name, action.name); field=action;
+                  multi=action.getMulti(hook, checkHook);
+                  smallButtons=True">:action.pxRender</div>
+      </x>
      </div>''')
 
-    # This PX displays icons for triggering actions on some tied object
-    # (edit, delete, etc).
+    # Icons for triggering actions on some tied object (edit, delete, etc)
     pxObjectActions = Px('''
      <div if="ifield.showActions"
           class=":ui.getActionsCss(ifield.actionsDisplay)"
           var2="layout='buttons';
                 editable=guard.mayEdit(o);
                 io=initiator.o;
                 locked=o.Lock.isSet(o, user, 'main')">
@@ -559,15 +567,15 @@
           if="not menu.icon">:menu.text</x>
      <!-- Nb of objects in the menu -->
      <b>:len(menu.objects)</b>''')
 
     pxViewMenus = Px('''
      <x var2="inMenu=True">
       <!-- One menu for every object type -->
-      <div for="menu in field.getLinkedObjectsByMenu(obj, objects)"
+      <div for="menu in field.getLinkedObjectsByMenu(o, objects)"
            class="inline"
            style=":not loop.menu.last and 'padding-right:4px' or ''">
        <div class="dropdownMenu inline"
             var2="singleObject=len(menu.objects) == 1"
             onmouseover="toggleDropdown(this)"
             onmouseout="toggleDropdown(this,'none')">
 
@@ -583,30 +591,32 @@
             var2="linkInPopup=popup or (target.target != '_self');
                   baseUrl=tied.getUrl(nav='no',
                     popup=linkInPopup)">::ui.Title.get(tied, target=target,
                 baseUrl=baseUrl, css='dropdownMenu',
                 linkTitle=tied.getShownValue(), title=field.pxMenu)</x>
         </x>
         <b if="not singleObject"
-           class=":field.getMenuCss(obj, menu)">:field.pxMenu</b>
+           class=":field.getMenuCss(o, menu)">:field.pxMenu</b>
 
         <!-- The dropdown menu containing tied objects -->
         <div class="dropdown" style="width:150px">
          <div for="tied in menu.objects"
               var2="batch=field.getBatchFor(batch.hook, len(menu.objects));
                     tiedId=tied.iid"
               class=":not loop.tied.first and 'refMenuItem' or ''">
+
           <!-- A specific link may have to be computed from
                field.menuUrlMethod -->
           <x if="field.menuUrlMethod"
-             var2="mUrl,mTarget=field.getMenuUrl(zobj,tied,
+             var2="mUrl, mTarget=field.getMenuUrl(o, tied,
                 target)">::ui.Title.get(tied, target=mTarget, baseUrl=mUrl)</x>
+
           <!-- Show standard pxObjectTitle else -->
           <x if="not field.menuUrlMethod">:field.pxObjectTitle</x>
-          <x if="tied.o.mayAct()">:field.pxObjectActions</x>
+          <x if="guard.mayAct(tied)">:field.pxObjectActions</x>
          </div>
         </div>
        </div>
       </div><x>:field.pxAdd</x></x> ''')
 
     # Simplified widget for fields with render="minimal"
     pxViewMinimal = Px('''
@@ -785,15 +795,15 @@
       render='list', renderMinimalSep=', ', menuIdMethod=None,
       menuInfoMethod=None, menuUrlMethod=None, menuCss=None, view=None,
       cell=None, edit=None, xml=None, translations=None, showActions='all',
       actionsDisplay='block', showGlobalActions=True, collapsible=False,
       links=True, viewAdded=True, noValueLabel='choose_a_value',
       noObjectLabel='no_ref', addLabel='object_add', addIcon='add.svg',
       filterable=True, supTitle=None, subTitle=None, toggleSubTitles=None,
-      separator=None, rowAlign='top', showControls=True):
+      separator=None, rowAlign='top', showControls=True, actions=None):
         # The class whose tied objects will be instances of
         self.class_ = class_
         # Specify "attribute" only for a back reference: it will be the name
         # (a string) of the attribute that will be defined on self's class and
         # will allow, from a linked object, to access the source object.
         self.attribute = attribute
         # If this Ref is "composite", it means that the source object will be
@@ -1265,14 +1275,17 @@
         # This attribute allows to hide, when rendering tied objects as a list
         # on "view", all standard controls tied to this Ref (icons/buttons for
         # adding or linking objects, etc). Use this only if you are sure you do
         # not use these controls, or if you display them elsewhere, in a custom
         # PX.
         self.showControls = showControls
 
+        # These p_actions fields will be shown as global actions
+        self.actions = actions
+
         # Call the base constructor
         Field.__init__(self, validator, multiplicity, default, defaultOnEdit,
           show, page, group, layouts, move, indexed, mustIndex, indexValue,
           emptyIndexValue, searchable, filterField, readPermission,
           writePermission, width, height, None, colspan, master, masterValue,
           focus, historized, mapping, generateLabel, label, sdefault, scolspan,
           swidth, sheight, persist, False, view, cell, edit, xml, translations)
@@ -2266,15 +2279,15 @@
     def getSelector(self, o, req):
         '''When this Ref field is shown in a popup for selecting objects to be
            included in an "originator" Ref field, this method gets info from the
            request about this originator.'''
         if 'selector' not in req: return
         id, name, mode = req.selector.split(',')
         initiator = o.getObject(id)
-        initiatorField = o.getField(name)
+        initiatorField = initiator.getField(name)
         # If several objects can be selected, show their checkboxes
         cbShown = initiatorField.isMultiValued()
         cbClass = '' if cbShown else 'hide'
         return O(initiator=initiator, initiatorField=initiatorField,
                  initiatorMode=mode, onav=req.onav or '',
                  initiatorHook='%d_%s' % (initiator.iid, name),
                  cbShown=cbShown, cbClass=cbClass,
@@ -2469,14 +2482,40 @@
         if not self.separator: return ''
         sep = self.separator(o, previous, next)
         if not sep: return ''
         css = ' class="%s"' % sep.css if sep.css else ''
         return '<tr><td colspan="%d"><div%s>%s</div></td></tr>' % \
                (len(columns), css, sep.translated or o.translate(sep.label))
 
+    def getActions(self, o):
+        '''Return the custom actions that must be shown among global actions'''
+        actions = self.actions
+        if not actions: return ()
+        r = []
+        i = 0
+        for action in actions:
+            show = action.show
+            show = show(o) if callable(show) else show
+            if show:
+                i += 1
+                # Lazy-init the action if not done yet
+                if not hasattr(action, 'name'):
+                    action.init(o.class_, 'action%d' % i)
+                r.append(action)
+        return r
+
+    def getField(self, subName):
+        '''Returns the sub-field whose name in p_subName, among
+           p_self.actions.'''
+        actions = self.actions
+        if not actions: return
+        for action in actions:
+            if subName == action.name:
+                return action
+
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 def autoref(class_, field):
     '''Defines, a posteriori, a Ref from one class the same one, or to another
        one but that could not be directly declared because it would have led to
        a circular import.'''
 
     # class_.field is a Ref to p_class_. This kind of auto-reference can't be
```

### Comparing `appy-1.0.8/py3/appy/model/fields/rich.py` & `appy-1.0.9/py3/appy/model/fields/rich.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,16 +101,16 @@
     # The name of the index class storing values of this field in the catalog
     indexType = 'RichIndex'
 
     # Unilingual view and cell
     viewUni = cellUni = Px('''
      <x var="inlineEdit=field.getAttribute(o, 'inlineEdit');
              css=field.getAttribute(o, 'viewCss');
-             mayAjaxEdit=inlineEdit and (layout != 'cell') and not \
-                       showChanges and guard.mayEdit(o, field.writePermission);
+             mayAjaxEdit=inlineEdit and layout != 'cell' and not showChanges \
+                         and guard.mayEdit(o, field.writePermission);
              value=field.injectContent(o, value) if field.inject else value">
       <div if="not mayAjaxEdit"
            class=":css">::value or field.valueIfEmpty</div>
       <x if="mayAjaxEdit" var2="name=lg and ('%s_%s' % (name, lg)) or name">
        <div class=":css" contenteditable="true"
             id=":'%d_%s_ck' % (o.iid, name)">::value or '-'</div>
        <script if="mayAjaxEdit">::field.getJsInlineInit(o, name, lg)</script>
@@ -267,15 +267,16 @@
 
            If p_i is not None, p_value is p_self's value as stored in the entry
            whose index is p_i+1 in p_o's history, and the method will return a
            diff between it and p_value's subsequent version, either to be found
            in a more recent entry in p_o's history or, failing that, the
            currently stored value on p_o.'''
         r = last = None
-        for event in o.history.iter(eventType='Change',chronological=True,i=i):
+        for event in o.history.iter(eventType='Change', chronological=True, \
+                                    i=i+1):
             # Ignore irrelevant events
             if not event.hasField(self.name, language=language): continue
             # We have a matching event
             if i is not None:
                 # Return the diff between p_value and the newer version stored
                 # in this event.
                 newer = event.getValue(self.name, language)
@@ -418,17 +419,17 @@
             if isinstance(v, int): sv = str(v)
             elif isinstance(v, bool): sv = str(v).lower()
             elif isinstance(v, dict): sv = str(v)
             else: sv = '"%s"' % v
             ck.append('%s: %s' % (k, sv))
         return ', '.join(ck)
 
-    def getJs(self, layout, r, config):
+    def getJs(self, o, layout, r, config):
         '''A rich field depend on CKeditor'''
-        if (layout not in ('edit', 'view')) or \
+        if layout not in ('edit', 'view') or \
            ((layout == 'view') and not self.inlineEdit): return
         # Compute the URL to ckeditor CDN
         ckUrl = Rich.cdnUrl % (config.ui.ckVersion, config.ui.ckDistribution)
         if ckUrl not in r: r.append(ckUrl)
 
     def getJsInit(self, o, language):
         '''Gets the Javascript init code for displaying a rich editor for this
```

### Comparing `appy-1.0.8/py3/appy/model/fields/select.py` & `appy-1.0.9/py3/appy/model/fields/select.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,15 @@
        style=":field.getSelectStyle(False, isMultiple)">
       <option for="val, text in possibleValues" value=":val"
               selected=":field.isSelected(o, name, val, rawValue)"
               title=":text">:Px.truncateValue(text, charsWidth)</option>
      </select>
 
      <!-- As radio buttons or checkboxes -->
-     <x if="not isSelect">
+     <div if="not isSelect" style=":field.getRadioStyle()">
 
       <!-- (Un)check all -->
       <div if="field.render == 'checkbox' and len(possibleValues) &gt; 1"
            class="divAll" var="allId='%s_all' % name">
        <input type="checkbox" class="checkAll" id=":allId" name=":allId"
               onclick="toggleCheckboxes(this)"/>
        <label lfor=":allId">:_('check_uncheck')</label>
@@ -188,15 +188,15 @@
       <div for="val, text in possibleValues"
            var2="vid='%s_%s' % (name, val)">
        <input type=":field.render" name=":name" id=":vid" value=":val"
               class=":masterCss" onchange=":field.getOnChange(o, layout)"
               checked=":field.isSelected(o, name, val, rawValue)"/>
        <label lfor=":vid" class="subLabel">:text</label>
       </div>
-     </x>
+     </div>
      <script if="hostLayout" var2="x=o.Lock.set(o, user, field=field)">:\
       'prepareForAjaxSave(%s,%s,%s,%s)' % \
        (q(name), q(o.iid), q(o.url), q(hostLayout))</script></x>''')
 
     # On the search form, show a multi-selection widget with a "AND/OR" selector
     search = Px('''
      <!-- The "and" / "or" radio buttons -->
@@ -400,15 +400,15 @@
             if master.valueIsInRequest(o, req):
                 # ... from the request if available
                 requestValue = master.getRequestValue(o)
                 masterValues = master.getStorableValue(o, requestValue,
                                                        single=True)
             elif not className:
                 # ... or from the database if we are editing an object
-                masterValues = master.getValue(o)
+                masterValues = master.getValue(o, single=True)
             else:
                 # We don't have any master value
                 masterValues = None
             # Get possible values by calling self.masterValue
             if masterValues:
                 values = self.masterValue(o, masterValues)
             else:
```

### Comparing `appy-1.0.8/py3/appy/model/fields/string.py` & `appy-1.0.9/py3/appy/model/fields/string.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/fields/switch.py` & `appy-1.0.9/py3/appy/model/fields/switch.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/fields/text.py` & `appy-1.0.9/py3/appy/model/fields/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,15 +440,15 @@
 
     def get(self, o):
         '''Returns the HTML chunk representing this icon'''
         shortcut = str(self.shortcut) if self.shortcut else ''
         r = '<img class="icon" src="%s" title="%s" name="%s"' \
             ' onmouseover="switchIconBack(this, true)"' \
             ' onmouseout="switchIconBack(this, false)"' \
-            ' data-type="%s" data-data="%s" data-shortcut="%d" ' \
+            ' data-type="%s" data-data="%s" data-shortcut="%s" ' \
             'onclick="useIcon(this)"/>' % \
              (o.buildUrl(self.icon), o.translate(self.label), self.name,
               self.type, self.data or '', shortcut)
         # Add specific stuff if icon type is "sentences"
         if self.type == 'sentences': r = self.asSentences(r, o)
         return r
```

### Comparing `appy-1.0.8/py3/appy/model/group.py` & `appy-1.0.9/py3/appy/model/group.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/loader.py` & `appy-1.0.9/py3/appy/model/loader.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/meta/__init__.py` & `appy-1.0.9/py3/appy/model/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/meta/class_.py` & `appy-1.0.9/py3/appy/model/meta/class_.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,22 +46,21 @@
 from appy.model.workflow.history import History
 from appy.model.searches.gridder import Gridder
 from appy.model.fields.computed import Computed
 from appy.model.workflow.localRoles import LocalRoles
 from appy.model.fields.phase import Page as FieldPage
 
 # Errors - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
-UNALLOWED_FIELD_NAME = 'You have defined a field or search named "%s" on ' \
-  'class "%s". This name is not allowed.'
-CREATOR_LOCAL_ROLE = '%s: local role "%s" cannot be used as creator.'
-DUPLICATE_SEARCH_NAME = '%s: duplicate search "%s".'
-SEARCH_FIELD_HOMONYM = '%s: "%s" is both used as search and field name, this ' \
-  'is not allowed.'
-CUSTOM_ID_NOT_STRING = 'The custom ID produced by method "generaeId" must be ' \
-  'a string.'
+F_NAME_KO   = 'You have defined a field or search named "%s" on class "%s". ' \
+              'This name is not allowed.'
+CR_LOC_ROLE = '%s: local role "%s" cannot be used as creator.'
+DUP_S_NAME  = '%s: duplicate search "%s".'
+S_F_HOM     = '%s: "%s" is both used as search and field name, this is not ' \
+              'allowed.'
+CUS_ID_KO   = 'The custom ID produced by method "generaeId" must be a string.'
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Class(Meta):
     '''Represents an Appy class'''
 
     # Attributes added on Appy classes
     attributes = {'fields': Field}
@@ -157,31 +156,44 @@
             #                appy.model.meta.class_.<genName>
             exec('self.concrete = %s' % genName)
             # Add the class in the namespace of the current package
             # (appy.model.meta.class_). Else, pickle, used by the ZODB to store
             # instances of this class, will not find it.
             setattr(appy.model.meta.class_, genName, self.concrete)
         else:
-            self.type = (self.name in Model.baseClasses) and 'over' or 'app'
+            self.type = 'over' if self.name in Model.baseClasses else 'app'
         # Fields are grouped into pages, themselves grouped into "phases"
         self.phases = collections.OrderedDict()
         # Read fields and static searches
         self.readFields()
         self.readSearches()
         # The class will be linked to a workflow (later, by the loader)
         self.workflow = None
         # Call the "update" method if present: it allows developers to modify
         # this class. One of the most frequent updates will be to update field
-        # "title".
+        # "title". If this method must add a new field, or replace an existing
+        # field with an alternate version, do not write things like:
+        #
+        #   @staticmethod
+        #   def update(class_):
+        #       class_.fields['title'] = Text(...)
+        #
+        # ... call method m_setField (defined hereafter) instead:
+        #
+        #   @staticmethod
+        #   def update(class_):
+        #       title = Text(...)
+        #       class_.setField('title', title)
         if self.type == 'over':
             # Execute the "update" method on the base class
             base = eval(self.name)
             if hasattr(base, 'update'):
                 base.update(self)
-        if hasattr(self.python, 'update'): self.python.update(self)
+        if hasattr(self.python, 'update'):
+            self.python.update(self)
 
     def getBaseClass(self):
         '''Returns the name of the class being p_self's base class'''
         name = self.name
         return name if name in Model.baseClasses else 'Base'
 
     def injectProperties(self):
@@ -241,15 +253,15 @@
             for name, field in aClass.__dict__.items():
                 if name.startswith('__'): continue
                 if isinstance(field, Field):
                     # Ensure the field name is acceptable
                     self.checkAttributeName(name)
                     if not aClass.__module__.startswith('appy.model') and \
                        (Class.unallowedName(name)):
-                        raise Err(UNALLOWED_FIELD_NAME % (name, self.name))
+                        raise Err(F_NAME_KO % (name, self.name))
                     # A field was found.
                     # ~~~
                     # Special fields "title" and "record" must be duplicated.
                     # Else, all app classes will get the modifications that the
                     # developer can apply to it via "update" methods.
                     if name == 'title':
                         field = String(**Base.titleAttributes)
@@ -259,31 +271,39 @@
                     # Late-initialize it
                     field.init(self, name)
                     r[name] = field
                     if field.page:
                         self.readPage(field.page)
         self.fields = r
 
+    def setField(self, name, field):
+        '''Possibly called by p_self.python's m_update method, this method adds,
+           to p_self.fields, a new p_field named p_name, or replaces the field
+           currently named p_name if the name is already in use.'''
+        self.fields[name] = field
+        # Late-initialise it
+        field.init(self, name)
+
     def readSearches(self):
         '''Create attribute "searches" as an ordered dict storing all static
            searches defined on this class.'''
         class_ = self.python
         r = collections.OrderedDict()
         Err = Model.Error
         if hasattr(class_, 'searches'):
             for search in class_.searches:
                 name = search.name
                 # Ensure the search name is acceptable
                 if Class.unallowedName(name):
-                    raise Err(UNALLOWED_FIELD_NAME % (name, self.name))
+                    raise Err(F_NAME_KO % (name, self.name))
                 # Ensure the search name is unique, also among fields
                 if name in r:
-                    raise Err(DUPLICATE_SEARCH_NAME % (self.name, name))
+                    raise Err(DUP_S_NAME % (self.name, name))
                 if name in self.fields:
-                    raise Err(SEARCH_FIELD_HOMONYM % (self.name, name))
+                    raise Err(S_F_HOM % (self.name, name))
                 # Ensure the field name is acceptable
                 self.checkAttributeName(name)
                 search.init(self)
                 r[search.name] = search
         self.searches = r
 
     def getCreators(self):
@@ -296,15 +316,15 @@
         # Athough a method can be specified in "creators", we can't execute it,
         # so we care about creators only if defined "statically", as a list.
         if not isinstance(creators, list): return r
         # Browse roles
         for creator in creators:
             if isinstance(creator, Role):
                 if creator.local:
-                    error = CREATOR_LOCAL_ROLE % (self.name,creator.name)
+                    error = CR_LOC_ROLE % (self.name,creator.name)
                     raise Model.Error(error)
                 r.append(creator)
             else:
                 r.append(Role(creator))
         return r
 
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
@@ -340,15 +360,15 @@
         # Return None if no such method is defined on p_self.python
         if not hasattr(self.python, 'generateId'): return
         r = self.python.generateId(o)
         # If the method return None, a standard ID will be generated by Appy
         if r is None: return
         # Raise an error if the returned ID is not a string
         if not isinstance(r, str):
-            raise Exception(CUSTOM_ID_NOT_STRING)
+            raise Exception(CUS_ID_KO)
         return r
 
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # Run-time methods
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # The following set of methods allow to compute, at run-time,
     # class-dependent elements.
@@ -571,16 +591,16 @@
             # If fields are not explicitly listed, take all indexed fields,
             # "title" excepted, "searchable" and "title" being mostly redundant.
             fields = [field for field in self.fields.values() \
              if field.indexed and (field.name not in Class.unsearchableFields)]
         # Collect CSS and JS files
         config = tool.config
         for field in fields:
-            field.getCss('edit', css)
-            field.getJs('edit', js, config)
+            field.getCss(None, 'edit', css)
+            field.getJs(None, 'edit', js, config)
         # Returns a gridder allowing to render the search field
         gridder = Gridder(cols=cols)
         return fields, css, js, gridder
 
     def getResultModes(self):
         '''Gets the search result modes for this class'''
         return getattr(self.python, 'resultModes', None)
```

### Comparing `appy-1.0.8/py3/appy/model/meta/workflow.py` & `appy-1.0.9/py3/appy/model/meta/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 from appy.model import Model
 from appy.model.meta import Meta
 from appy.model.workflow.state import State
 from appy.model.workflow.transition import Transition
 from appy.model.fields.phase import Page as FieldPage
 
 # Errors - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
-MULTIPLE_INITIAL_STATES = 'In workflow "%s", states "%s" and "%s" are both ' \
-  'defined as being initial.'
-NO_INITIAL_STATE = 'Workflow "%s" does not define any initial state.'
+MULTI_I_S = 'In workflow "%s", states "%s" and "%s" are both defined as ' \
+            'being initial.'
+NO_I_S    = 'Workflow "%s" does not define any initial state.'
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Workflow(Meta):
     '''Represents a Appy worflow'''
 
     # Attributes added on Appy workflows
     attributes = {'states': State, 'transitions': Transition}
@@ -107,26 +107,25 @@
                 # Late-initialize it
                 value.init(self, name)
                 # Store it
                 states[name] = value
                 if value.initial:
                     # There can be at most one initial state
                     if initial:
-                        raise Err(MULTIPLE_INITIAL_STATES % \
-                                  (self.name, initial.name, name))
+                        raise Err(MULTI_I_S % (self.name, initial.name, name))
                     initial = value
             elif isinstance(value, Transition):
                 # A transition was found. Ensure its name is acceptable.
                 self.checkAttributeName(name)
                 # Late-initialize it
                 value.init(self, name)
                 # Store it
                 transitions[name] = value
         # At least one initial state is required
-        if not initial: raise Err(NO_INITIAL_STATE % self.name)
+        if not initial: raise Err(NO_I_S % self.name)
         self.states = states
         self.transitions = transitions
         self.initialState = initial
         # Create a Transition instance representing the initial transition
         self.initialTransition = tr = Transition((initial, initial))
         tr.init(self, '_init_')
 
@@ -137,15 +136,15 @@
     # workflow-dependent elements.
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def getRolesFor(self, o, permission):
         '''Gets the roles that are currently granted p_permission on this
            p_o(bject). r_ is a list of role names.'''
         state = self.states[o.state]
-        return state.getRolesFor(permission)
+        return state.getRolesFor(o, permission)
 
     def getTransitions(self, o, includeFake=True, includeNotShowable=False,
                        grouped=True):
         '''Return transitions that the current user can trigger from the user
            interface, as a list of UiTransition instances.'''
         #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
         #    includeFake     | If True, it retrieves transitions that the user
@@ -172,15 +171,15 @@
             # Filter transitions that do not have currentState as start state
             if not transition.hasState(currentState, True): continue
             # Check if the transition can be triggered
             mayTrigger = transition.isTriggerable(o)
             # Compute the condition that will lead to including or not this
             # transition.
             includeIt = mayTrigger if not includeFake \
-                        else mayTrigger or isinstance(mayTrigger, No) 
+                        else mayTrigger or isinstance(mayTrigger, No)
             if not includeNotShowable:
                 includeIt = includeIt and transition.isShowable(o)
             if not includeIt: continue
             # Create the UiTransition instance
             ui = transition.ui(o, mayTrigger)
             # Add the transition into the result
             if not transition.group or not grouped:
@@ -213,13 +212,12 @@
        <input type="hidden" name="nav" value=":req.nav or 'no'"/>
        <input type="hidden" name="page" value=":req.page or 'main'"/>
        <!-- Input field for storing the comment coming from the popup -->
        <textarea name="popupComment" cols="30" rows="3"
                  style="display:none"></textarea>
       </form>
 
-      <!-- Render a transition or a group of transitions. "inline" will be
-           overridden if this transition is rendered inside a flexbox. -->
-      <div for="transition in transitions" class="inline"
+      <!-- Render a transition or a group of transitions -->
+      <div for="transition in transitions"
            var2="trGroup=transition">:transition.px</div>
      </x>''')
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
```

### Comparing `appy-1.0.8/py3/appy/model/page.py` & `appy-1.0.9/py3/appy/model/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,14 @@
 class Page(Base):
     '''Base class representing a web page'''
 
     # By default, web pages are public
     workflow = Anonymous
 
     pa = {'label': 'Page'}
-    # Pages are not indexed by default
-    indexable = False
 
     @staticmethod
     def getListColumns(tool):
         '''Show minimal info for the anonymous user'''
         if tool.user.isAnon(): return
         return ('title', 'expression', 'next', 'selectable*100px|',
                 'podable*80px|', 'viewCss*100px|')
```

### Comparing `appy-1.0.8/py3/appy/model/pod/Page.odt` & `appy-1.0.9/py3/appy/model/pod/Page.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/query.py` & `appy-1.0.9/py3/appy/model/query.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/searches/__init__.py` & `appy-1.0.9/py3/appy/model/searches/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -625,18 +625,24 @@
         # ----------------------------------------------------------------------
 
         ids = {int(v) for v in req.checkedIds.split(',')} if req.checkedIds \
                                                           else {}
         return ids, req.checkedSem == 'unchecked'
 
     @classmethod
-    def keepCheckedResults(class_, req, objects):
+    def keepCheckedResults(class_, req, objects, unchecked=None):
         '''Among p_objects as retrieved via m_replay, keep only those being
            checked, according to m_getCheckedInfo.'''
-        ids, unchecked = class_.getCheckedInfo(req)
+        # If p_unchecked is not None, we already know the IDs of the objects
+        # being unchecked.
+        if unchecked:
+            ids = unchecked
+            unchecked = True
+        else:
+            ids, unchecked = class_.getCheckedInfo(req)
         i = len(objects) - 1
         # Remove, from search results, unchecked objects
         while i >= 0:
             if unchecked: remove = objects[i].iid in ids
             else:         remove = objects[i].iid not in ids
             if remove:
                 del objects[i]
```

### Comparing `appy-1.0.8/py3/appy/model/searches/gridder.py` & `appy-1.0.9/py3/appy/model/searches/gridder.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/searches/initiators.py` & `appy-1.0.9/py3/appy/model/searches/initiators.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/searches/modes.py` & `appy-1.0.9/py3/appy/model/searches/modes.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,16 +37,17 @@
     # All available predefined concrete modes
     concrete = ('list', 'grid', 'calendar')
 
     # The list of custom actions that can be triggered on search results
     pxActions = Px('''
      <table>
       <tr><td for="action in actions"
-            var2="field=action; fieldName=field.name; layout='query';
-                  multi=True">:action.pxRender</td></tr>
+            var2="multi=action.getMulti('queryResult', req.search);
+                  field=action; fieldName=field.name;
+                  layout='query'">:action.pxRender</td></tr>
      </table>''')
 
     @classmethod
     def get(class_, uiSearch):
         '''Create and return the Mode instance corresponding to the current
            result mode to apply to a list of instances.'''
         name = uiSearch.req.resultMode or uiSearch.getModes()[0]
@@ -459,38 +460,55 @@
 
     # Name for this mode
     name = 'calendar'
 
     px = Px('''<x var="layoutType='view';
                        field=tool.getField('calendar')">:field.view</x>''')
 
+    # Formats for keys representing dates
+    dayKey = '%Y%m%d'
+
+    # Format for representing hours in the UI
+    hourFormat = '%H:%M'
+
     def __init__(self, *args):
         Mode.__init__(self, *args)
         # For this calendar view to work properly, objects to show inside it
-        # must have the following attributes:
+        # must have the following fields:
         # ----------------------------------------------------------------------
         # date    | an indexed and required Date field with format =
         #         | Date.WITH_HOUR storing the object's start date and hour;
         # ----------------------------------------------------------------------
         # endDate | a not necessarily required Date field with format =
         #         | Date.WITH_HOUR storing the object's end date and hour.
         # ----------------------------------------------------------------------
-        # Optionally, if objects define the following attributes, special icons
-        # indicating repeated events will be shown.
+        # Optionnally, if you want to use index "months" (we advice you to do
+        # so), an indexed Computed field with this name must also be defined
+        # (see details in m_init below).
+        # ----------------------------------------------------------------------
+        # Optionally, too, if objects define the following attributes, special
+        # icons indicating repeated events will be shown.
         # ----------------------------------------------------------------------
         # successor   | Ref field with multiplicity = (0,1), allowing to
         #             | navigate to the next object in the list (for a repeated
         #             | event);
         # ----------------------------------------------------------------------
         # predecessor | Ref field with multiplicity = (0,1), allowing to
         #             | navigate to the previous object in the list.
         #             | "predecessor" must be the back ref of field "successor"
         #             | hereabove.
         # ----------------------------------------------------------------------
 
+    def getMonthIndex(self):
+        '''Deduce, from p_self.class_, what is the month index to use'''
+        # Is there, on p_self.class_, a field name "months" ?
+        months = getattr(self.class_.python, 'months', None)
+        if not months: return 'date'
+        return 'months' if months.type=='Computed' and month.indexed else 'date'
+
     def init(self):
         '''Creates a stub calendar field'''
         Mode.init(self)
         # Always consider the result as not empty. This way, the calendar is
         # always shown, even if no object is visible.
         self.empty = False
         # The matched objects, keyed by day. For every day, a list of entries to
@@ -507,20 +525,73 @@
         #  "end"    | the object started at a previous day and ends at this day.
         #           | Display its title and a sign indicating this fact;
         # ----------------------------------------------------------------------
         #  "pass"   | The object started at a previous day and ends at a future
         #           | day.
         # ----------------------------------------------------------------------
         self.objects = {} # ~{s_YYYYmmdd: [(s_entryType, Object)]}~
-        # Formats for keys representing dates
-        self.dayKey = '%Y%m%d'
-        # Format for representing hours in the UI
-        self.hourFormat = '%H:%M'
         # If filters are defined from a list mode, get it
         self.filters = self.class_.getFilters(tool)
+        # The name of the index to use to restrict the search to the currently
+        # shown month. If p_self.klass defines a Computed indexed TextIndex
+        # field named "months", this index will be used. Else, index "date" will
+        # be used. These 2 indexes are described hereafter.
+        # ----------------------------------------------------------------------
+        # "date"   | This index is expected to define the (start) date of the
+        #          | objects to search. So, the search will match any object
+        #          | whose (start) date is included in the range of dates
+        #          | defined by the currently shown month. Recall that this
+        #          | range may be larger than the month itself: because complete
+        #          | weeks are shown, some days from the previous and next
+        #          | months may be present, too.
+        #          |
+        #          | While this index is the easiest to implement, it has the
+        #          | following problem: objects spanning several days (by using
+        #          | fields "date" and "endate") and whose start date is not
+        #          | among the range of visible dates, will not be part of the
+        #          | result. This is why an alternate index named "month' is
+        #          | also proposed (see below).
+        # ----------------------------------------------------------------------
+        # "months" | When using index "months", every object is expected to
+        #          | hold, in a Computed indexed TextIndex field named "months",
+        #          | the space-separated list of months the object crosses
+        #          | (every crossing month must be represented as a string of
+        #          | the form YYYYmm). "Crossing a month" means: there must be a
+        #          | not-empty intersection between the range of visible days
+        #          | for this month, and the object's range of days. For objects
+        #          | defining no end date, this range is reduced to a unique day
+        #          | (defined by field "date").
+        #          |
+        #          | Because this list of crossing months is relatively complex
+        #          | to produce, Appy provides a function that computes it:
+        #          |
+        #          |           appy.shared.dates.getCalendarMonths
+        #          |
+        #          | Here is a complete example of a Appy class using index
+        #          | "months".
+        #          |
+        #          | from appy.shared.dates import getCalendarMonths
+        #          |
+        #          | class Event:
+        #          |     ...
+        #          |     date    = Date(format=Date.Date.WITH_HOUR,
+        #          |                    multiplicity=(1,1), indexed=True, ...)
+        #          |     endDate = Date(format=Date.Date.WITH_HOUR,
+        #          |                    indexed=True, ...)
+        #          |     ...
+        #          |     def computeMonths(self):
+        #          |         '''Compute the months crossed by p_self'''
+        #          |         # p_self.endDate may be None
+        #          |         return ' '.join(getCalendarMonths(self.date,
+        #          |                                           self.endDate))
+        #          |
+        #          |     months  = Computed(method=computeMonths,
+        #          |                        indexed='TextIndex', show=False)
+        # ----------------------------------------------------------------------
+        self.monthIndex = self.getMonthIndex()
 
     def updateAjaxParameters(self, params):
         '''Grid-specific ajax parameters'''
         # If filters are in use, carry them
         if self.filters:
             params['filters'] = self.filters
 
@@ -545,69 +616,95 @@
            @key p_dateKey.'''
         r = self.objects
         if dateKey not in r:
             r[dateKey] = [entry]
         else:
             r[dateKey].append(entry)
 
-    def addEntries(self, obj):
-        '''Add, in self.objects, entries corresponding to p_obj. If p_obj spans
-           a single day, a single entry of the form ("start", p_obj) is added at
-           the key corresponding to this day. Else, a series of entries are
-           added, each of the form (s_entryType, p_obj), with the same object,
-           for every day in p_obj's timespan.
-
-           For example, for an p_obj starting at "1975/12/11 12:00" and ending
-           at "1975/12/13 14:00" will produce the following entries:
-              key "19751211"  >  value ("start+", obj)
-              key "19751212"  >  value ("pass", obj)
-              key "19751213"  >  value ("end", obj)
-        '''
+    def addEntries(self, o, gridFirst, gridLast):
+        '''Add, in self.objects, entries corresponding to p_o. If p_o spans a
+           single day, a single entry of the form ("start", p_o) is added at the
+           key corresponding to this day. Else, a series of entries are added,
+           each of the form (s_entryType, p_o), with the same object, for every
+           day in p_o's timespan.'''
+        # For example, for an p_o(bject) starting at "1975/12/11 12:00" and
+        # ending at "1975/12/13 14:00", m_addEntries will produce the following
+        # entries:
+        #      key "19751211"  >  value ("start+", obj)
+        #      key "19751212"  >  value ("pass", obj)
+        #      key "19751213"  >  value ("end", obj)
+        # ~~~
         # Get p_obj's start and end dates
-        start = obj.date
-        startKey = start.strftime(self.dayKey)
-        end = obj.endDate
-        endKey = end and end.strftime(self.dayKey) or None
+        fmt = Calendar.dayKey
+        start = o.date
+        startKey = start.strftime(fmt)
+        end = o.endDate
+        endKey = end.strftime(fmt) if end else None
         # Shorthand for self.objects
         r = self.objects
-        if not endKey or (endKey == startKey):
+        if not endKey or endKey == startKey:
             # A single entry must be added for p_obj, at the start date
-            self.addEntry(startKey, ("start", obj))
+            self.addEntry(startKey, ('start', o))
         else:
+            # Insert one event per day, provided the events are in the grid
+            # ~~~
             # Add one entry at the start day
-            self.addEntry(startKey, ("start+", obj))
-            # Add "pass" entries for every day between the start and end days
-            next = start + 1
-            nextKey = next.strftime(self.dayKey)
-            while nextKey != endKey:
+            if start >= gridFirst:
+                self.addEntry(startKey, ('start+', o))
+                next = start + 1
+            else:
+                # Ignore any day between v_start and p_gridFirst
+                next = gridFirst
+            # Add "pass" entries for every day between the event's start and end
+            # dates.
+            nextKey = next.strftime(fmt)
+            while nextKey != endKey and next <= gridLast:
                 # Add a "pass" event
-                self.addEntry(nextKey, ('pass', obj))
+                self.addEntry(nextKey, ('pass', o))
                 # Go the the next day
                 next += 1
-                nextKey = next.strftime(self.dayKey)
+                nextKey = next.strftime(fmt)
             # Add an "end" entry at the end day
-            self.addEntry(endKey, ('end', obj))
+            if end <= gridLast:
+                self.addEntry(endKey, ('end', o))
 
     def search(self, first, grid):
-        '''Performs the query, limited to the date range defined by p_grid'''
-        # Performs the query, restricted to the visible date range
-        last = DateTime(grid[-1][-1].strftime('%Y/%m/%d 23:59:59'))
-        dateSearch = Search(date=(first, last), sortBy='date', sortOrder='asc')
-        res = self.tool.executeQuery(self.className,
-          search=self.uiSearch.search, maxResults='NO_LIMIT',
-          search2=dateSearch, filters=self.filters)
+        '''Performs the search, restricted to the visible date range as defined
+           by p_grid.'''
+        # # The first date in the p_grid, that may be earlier than the p_first
+        # day of the month.
+        gridFirst = grid[0][0]
+        # The last date in the grid, calibrated
+        gridLast = DateTime(grid[-1][-1].strftime('%Y/%m/%d 23:59:59'))
+        # Get the search parameters being specific to the range of dates
+        params = {'sortBy':'date', 'sortOrder':'asc'}
+        if self.monthIndex == 'date':
+            # Define the search based on every event's (start) date.
+            # ~~~
+            # As first date, prefer the first visible date in the p_grid instead
+            # of the p_first day of the month.
+            params['date'] = gridFirst, gridLast
+        else: # p_self.monthIndex is "months"
+            # Define the search based on index "months"
+            params['months'] = first.strftime('%Y%m')
+        # Create a Search instance for the search-related parameters
+        dateSearch = Search(**params)
+        # Perform the search
+        r = self.tool.executeQuery(self.className, search=self.uiSearch.search,
+                                   maxResults='NO_LIMIT', search2=dateSearch,
+                                   filters=self.filters)
         # Produce, in self.objects, the dict of matched objects
-        for zobj in res.objects:
-            self.addEntries(zobj.appy())
+        for zobj in r.objects:
+            self.addEntries(zobj.appy(), gridFirst, gridLast)
 
     def dumpObjectsAt(self, date):
         '''Returns info about the object(s) that must be shown in the cell
            corresponding to p_date.'''
         # There may be no object dump at this date
-        dateStr = date.strftime(self.dayKey)
+        dateStr = date.strftime(Calendar.dayKey)
         if dateStr not in self.objects: return
         # Objects exist
         r = []
         types = self.entryTypes
         url = self.tool.getIncludeUrl
         for entryType, obj in self.objects[dateStr]:
             # Dump the event hour and title. The back hook allows to refresh the
```

### Comparing `appy-1.0.8/py3/appy/model/tool.py` & `appy-1.0.9/py3/appy/model/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from appy.model.base import Base
 from appy.model.user import User
 from appy.data import nativeNames
 from appy.utils.dates import Date
 from appy.model.group import Group
 from appy.model.fields import Show
 from appy.model.query import Query
+from appy.model.mover import Mover
 from appy.database import Database
 from appy.ui.layout import Layouts
 from appy.utils.mail import sendMail
 from appy.ui.template import Template
 from appy.model.fields.ref import Ref
 from appy.server.backup import Backup
 from appy.model.fields.rich import Rich
@@ -237,26 +238,14 @@
     # Ref(User) will maybe be transformed into Ref(AppUser)
     users = Ref(User, multiplicity=(0,None), add=True, link=False,
       composite=True, back=Ref(attribute='toTool', show=False, layouts='f'),
       page=userPage, queryable=True, queryFields=('searchable','login','roles'),
       show=forToolWriters, showHeaders=True, actionsDisplay='right',
       shownInfo=User.listColumns, **ta)
 
-    def getUserName(self, login=None, normalized=False):
-        '''Gets the user name corresponding to p_login (or the currently logged
-           user if None), or the p_login itself if the user does not exist
-           anymore. If p_normalized is True, special chars in the first and last
-           names are normalized.'''
-        if not login:
-            user = self.user
-        else:
-            user = self.search1('User', login=login)
-            if not user: return login
-        return user.getTitle(normalized=normalized)
-
     def doSynchronizeExternalUsers(self):
         '''Synchronizes the local User copies with a distant LDAP user base'''
         cfg, context = self.config.security.getLdap()
         if not cfg: raise Exception('LDAP config not found.')
         message = cfg.synchronizeUsers(self, sso=context)
         return True, message
 
@@ -315,14 +304,18 @@
 
     # The page, among "pages", being defined as the default one
     defaultPage = Ref(OPage, add=False, link=True, render='links', page=pp,
                       back=Ref(attribute='toTool2', show=False, layouts='f'),
                       show=lambda o: not o.isEmpty('pages'),
                       select=lambda o: o.pages, **ta)
 
+    # Update the base URL of all internal links within pages's rich fields
+    updateBaseUrl = Action(action=lambda o, options: options.run(),
+                           show='buttons', options=Mover, page=pp, **ta)
+
     #  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -
     #  Page "carousels"
     #  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -
 
     pc = Page('carousels', show=lambda o: 'view' if o.allows('write') else None,
               label='Tool_page_carousels')
 
@@ -460,16 +453,16 @@
        <!-- The home text must not be shown here, if shown on a public page -->
        <x if="not tool.isEmpty('defaultPage') and 
               not cfg.discreetLogin">::tool.defaultPage.content</x>
      </div>
 
      <!-- The backgrounds for px "homes" -->
      <div if="_px_.name == 'homes'" class="homes">
-      <div for="fileName, info in cfg.homesBackgrounds.items()"
-           var2="base,width=info; bg=tool.buildUrl(fileName, base=base,bg=True)"
+      <div for="fileName, width in cfg.homesBackgrounds.items()"
+           var2="bg=tool.buildUrl(fileName, bg=True)"
            style=":'%s;width:%s' % (bg, width)"></div>
      </div>''',
 
      css='''
       .homeText { position:fixed; left:45px; top:25px; color:|homeTextColor| }
       .homeText h1 { font-size: 300%; margin-left: -5px }
       .homeText h2 { font-size: 200% }
```

### Comparing `appy-1.0.8/py3/appy/model/translation.py` & `appy-1.0.9/py3/appy/model/translation.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/user.py` & `appy-1.0.9/py3/appy/model/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     password = Password(multiplicity=(1,1), show=showPassword, label='User',
                         page=pagePassword)
 
     # The encrypted password, carriable via the XML layout
     def showEncrypted(self):
         '''Allow to show encrypted password to admins only, via the xml
            layout.'''
-        if self.user.login == 'admin' and (self.source != 'sso'): return 'xml'
+        if self.user.login == 'admin' and self.source != 'sso': return 'xml'
 
     encrypted = Computed(show=showEncrypted, label='User',
                          method=lambda o: o.values['password'])
 
     #  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -
     #  Title, name, first name
     #  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -  -
@@ -598,18 +598,18 @@
                 if config.ldap:
                     user = config.ldap.getUser(tool, login, password)
             # Get the user from the local database if it was not found yet
             user = user or tool.search1('User', login=login)
             # Authentication fails (and user "anon" is returned) if the user was
             # not found or inactive, its password was invalid or the required
             # authentication context was not found.
-            if (user is None) or user.isAnon() or (user.state=='inactive') or \
-               (not user.getField('password').check(user, password)) or \
-               (not ctx and authContext and authContext.isMandatory(tool) and \
-                (place != 'basic')):
+            if user is None or user.isAnon() or user.state == 'inactive' or \
+               not user.getField('password').check(user, password) or \
+               (not ctx and authContext and authContext.isMandatory(tool,True))\
+               and place != 'basic':
                 # Disable the authentication cookie
                 guard.Cookie.disable(handler)
                 user = handler.dbConnection.root.objects.get('anon')
             else:
                 # The user is authenticated. Create an authentication cookie for
                 # him. Set a default context when appropriate.
                 if authContext and not ctx:
```

### Comparing `appy-1.0.8/py3/appy/model/utils.py` & `appy-1.0.9/py3/appy/model/utils.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/workflow/__init__.py` & `appy-1.0.9/py3/appy/model/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/workflow/history.py` & `appy-1.0.9/py3/appy/model/workflow/history.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
             # Try to return the next element
             self.increment()
             return self.__next__()
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Event(persistent.Persistent):
     '''An object's history is made of events'''
+
     # A format for representing dates at various (non ui) places
     dateFormat = '%Y/%m/%d %H:%M'
 
     # Some events can be deleted from the ui, but most aren't
     deletable = False
 
     # The PX displaying details about an event (basically the event's comment)
@@ -154,23 +155,31 @@
         return self.__class__.__name__
 
     def getLabel(self, o):
         '''Returns the i18n label for this event'''
         # To be overridden
 
     def getComment(self, empty='-'):
-        '''Returns the formatted version of p_self.comment'''
-        comment = self.comment
-        if not comment: return empty
-        return Escape.xhtml(comment, p=True)
+        '''Returns p_self.comment, ready to be included in a chunk of XHTML'''
+        return self.comment or empty
 
     def getId(self):
         '''Return an ID for this history p_event, based on its date.'''
         return str(self.date.millis())
 
+    def getUser(self, o, title=True):
+        '''Returns the complete name of the user with this p_self.login'''
+        login = self.login
+        if not login:
+            return '?' if title else None
+        user = o.search1('User', login=login)
+        if not user:
+            return '?' if title else None
+        return (user.getTitle() or login) if title else user
+
     def __repr__(self):
         '''String representation'''
         date = self.date.strftime(Event.dateFormat)
         return '<%s by %s on %s, state %s>' % \
                (self.getTypeName(), self.login, date, self.state)
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
@@ -361,17 +370,16 @@
        <tr for="event in batch.objects"
            class=":loop.event.odd and 'even' or 'odd'" valign="top">
         <td><x>:_(event.getLabel(o))</x>
          <img if="isManager and event.deletable" class="clickable iconS"
               src=":url('deleteS.svg')"
               onclick=":'onHistoryEvent(%s,%s,%s)' % \
                         (q('Delete'), q(o.iid), q(event.date))"/></td>
-        <td var="creator=o.search1('User', login=event.login)">
-         <x>:creator.getTitle() if creator else (event.login or '?')</x></td>
-        <td>:tool.formatDate(event.date)</td>
+        <td>:event.getUser(o)</td>
+        <td>:tool.formatDate(event.date, format=event.dateFormat)</td>
         <td>:event.pxDetail</td>
        </tr>
       </table>
      </div>''')
 
     view = Px('''
      <div if="not o.isTemp()"
@@ -569,8 +577,32 @@
            number of replacements done.'''
         r = 0
         for event in self:
             if event.login == old:
                 event.login = new
                 r += 1
         return r
+
+    def asXhtml(self, includeChanges=False):
+        '''Produce a XHTML version of this history, in the form of a discussion
+           thread, suitable to be injected as various places: in methods
+           getSubTitle, in PODs, etc.'''
+        # Browse history events
+        r = []
+        o = self.o
+        for event in self:
+            # Ignore inappropriate events
+            if not includeChanges and isinstance(event, Change): continue
+            # Define a prefix, being the name of the event
+            prefix = '<b>%s</b> ' % o.translate(event.getLabel(o)) or ''
+            # Get the comment when present
+            comment = event.comment or ''
+            if comment: comment = comment.replace('\n', '<br/>')
+            # Create the message line
+            msg = '<i>%s</i> – %s – %s' % \
+                  (event.date.strftime(Event.dateFormat), prefix,
+                   event.getUser(o))
+            if comment:
+                msg += ' – « %s »' % comment
+            r.append(msg)
+        return '<div style="margin-left: 20px">%s</div>' % '<br/>'.join(r)
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `appy-1.0.8/py3/appy/model/workflow/localRoles.py` & `appy-1.0.9/py3/appy/model/workflow/localRoles.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/workflow/standard.py` & `appy-1.0.9/py3/appy/model/workflow/standard.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/model/workflow/state.py` & `appy-1.0.9/py3/appy/model/workflow/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 import copy
 from appy.utils import sequenceTypes
 from appy.model.workflow import Role
 
 # Errors - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
-PERMISSION_NOT_FOUND = 'permission "%s" is not among permissions dict for ' \
-  'state %s in workflow %s.'
-                            
+PERM_N_F = 'permission "%s" is not among permissions dict for state %s in ' \
+           'workflow %s.'
+
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class State:
     '''Represents a workflow state'''
     def __init__(self, permissions, initial=False, phase=None):
         self.usedRoles = {}
         # Dict "permissions" lists, for every permission managed by a workflow,
         # the roles for which the permission is granted in this state. Standard
@@ -78,46 +78,56 @@
         '''This method converts, within self.permissions, every role to a
            Role instance. Every used role is stored in self.usedRoles.'''
         for permission, roles in self.permissions.items():
             if isinstance(roles, str) or isinstance(roles, Role):
                 role = self.getRole(roles)
                 self.permissions[permission] = {role.name: role}
             elif isinstance(roles, dict):
-                for name, role in roles.iteritems():
+                for name, role in roles.items():
                     roles[name] = self.getRole(role)
+            elif callable(roles):
+                # v_roles is a method: it is not possible to standardize it. It
+                # will be called at check time.
+                pass
             else:
                 # "roles" is a list or tuple, or None (nobody may have this
                 # permission).
                 d = {}
                 if roles is not None:
                     for role in roles:
                         role = self.getRole(role)
                         d[role.name] = role
                 self.permissions[permission] = d
 
     def getUsedRoles(self): return self.usedRoles.values()
 
-    def getRolesFor(self, permission):
+    def getRolesFor(self, o, permission):
         '''Gets the roles that are granted p_permission on this state. r_ is a
            dict ~{s_roleName: Role}.'''
         if permission not in self.permissions:
-            raise Exception(PERMISSION_NOT_FOUND % (permission, self.name, \
-                                                    self.workflow.name))
-        return self.permissions[permission]
+            raise Exception(PERM_N_F % (permission, self.name,
+                                        self.workflow.name))
+        r = self.permissions[permission]
+        # If v_r is a method, it *must* return Role instances
+        if callable(r):
+            r = r(self.workflow, o, permission)
+        return r
 
     def addRoles(self, roles, permissions=()):
         '''Adds p_roles in self.permissions. p_roles can be a role name, a Role
            instance or a list of names and/or Role instances. If p_permissions
            is specified, roles are added to those permissions only. Else, roles
            are added for every permission within self.permissions.'''
         # Standardize parameters
         if type(roles) not in sequenceTypes: roles = (roles,)
         if isinstance(permissions, str): permissions = (permissions,)
         for perm, existingRoles in self.permissions.items():
             if permissions and (perm not in permissions): continue
+            # It is not possible to add p_roles if v_existingRoles is a method
+            if callable(existingRoles): continue
             for role in roles:
                 # Do nothing if "role" is already among existing roles
                 name = role if isinstance(role, str) else role.name
                 if name in existingRoles: continue
                 # Add the role for this permission
                 existingRoles[name] = self.getRole(role)
 
@@ -177,13 +187,13 @@
             # isolated.
             if tr.isSingle():
                 for state in tr.states:
                     if state != self: return
             else:
                 for start, end in tr.states:
                     # Bypass (start, end) pairs having nothing to do with self
-                    if (start != self) and (end != self): continue
-                    if (start != self) or (end != self): return
+                    if start != self and end != self: continue
+                    if start != self or  end != self: return
         # If we are here, either there was no transition starting from self,
         # either all transitions were auto-transitions: self is then isolated.
         return True
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
```

### Comparing `appy-1.0.8/py3/appy/model/workflow/transition.py` & `appy-1.0.9/py3/appy/model/workflow/transition.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class Transition:
     '''Represents a workflow transition'''
     class Error(Exception): pass
     traverse = {}
 
     def __init__(self, states, condition=True, action=None, show=True,
                  confirm=False, group=None, icon=None, sicon=None,
-                 redirect=None, historizeActionMessage=False):
+                 redirect=None, historizeActionMessage=False, iconOnly=False):
         # In its simpler form, "states" is a list of 2 states:
         # (fromState, toState). But it can also be a list of several
         # (fromState, toState) sub-lists. This way, you may define only 1
         # transition at several places in the state-transition diagram. It may
         # be useful for "undo" transitions, for example.
         self.states = self.standardiseStates(states)
         self.condition = condition
@@ -73,14 +73,17 @@
         # ----------------------------------------------------------------------
         self.redirect = redirect
         # When a transition is triggered, the corresponding event is added in
         # the object's history. If p_historizeActionMessage is True, the message
         # returned by self.action (if any) will be appended to this event's
         # comment.
         self.historizeActionMessage = historizeActionMessage
+        # If p_iconOnly is True, the transition will be rendered as an icon (and
+        # not a button), even on the "buttons" layout.
+        self.iconOnly = iconOnly
 
     def init(self, workflow, name):
         '''Lazy initialisation'''
         self.workflow = workflow
         self.name = name
         self.labelId = '%s_%s' % (workflow.name, name)
 
@@ -303,20 +306,20 @@
         name = self.name
         isInit = name == '_init_'
         # "Triggerability" and security checks
         if not isInit and not self.isTriggerable(o, secure=secure):
             raise Transition.Error(UNTRIGGERABLE % (name, o.url))
         # Identify the target state for this transition
         target = forceTarget or self.getTargetState(o)
-        # Add the event in the object history
-        event = o.history.add('Trigger', target.name, transition=name,
-                              comment=comment)
         # Remember the source state, it will be necessary for executing the
         # common action.
         fromState = o.state if not isInit else None
+        # Add the event in the object history
+        event = o.history.add('Trigger', target.name, transition=name,
+                              comment=comment)
         # Execute the action that is common to all transitions, if defined. It
         # is named "onTrigger" on the workflow class by convention. This common
         # action is executed before the transition-specific action (if any).
         proto = self.workflow.proto
         if doAction and hasattr(proto, 'onTrigger'):
             proto.onTrigger(o, name, fromState)
         # Execute the transition-specific action
@@ -386,34 +389,40 @@
                     if (not endOk) and tr.hasState(start, False):
                         endOk = True
                     if startOk and endOk: return trName
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class UiTransition:
     '''Represents a widget that displays a transition'''
+
     px = Px('''
      <x var="label=transition.title;
              mayTrigger=transition.mayTrigger;
-             inButtons=layout == 'buttons'">
+             inButtons=layout == 'buttons';
+             asIcon=not inButtons or transition.iconOnly">
 
-      <!-- Picto -->
-      <a if="not inButtons" class=":'clickable' if mayTrigger else 'help fake'"
-         var="back=transition.getBackHook(o, inButtons, q, backHook)"
+      <!-- Picto or icon -->
+      <a if="asIcon" class=":'clickable' if mayTrigger else 'help fake'"
+         var="back=transition.getBackHook(o, inButtons, q, backHook);
+              iconAttr='sicon' if inButtons else 'icon';
+              iconBase='siconBase' if inButtons else 'iconBase'"
          name=":transition.name"
-         title=":'' if mayTrigger else transition.reason"
+         title=":transition.getIconTitle()"
          onclick=":'triggerTransition(%s,this.name,%s,%s)' % \
                     (q(formId), q(transition.confirm), back) \
                     if mayTrigger else ''">
-       <img src=":url(transition.icon, base=transition.iconBase)"
-            class=":picto"/>
-       <div style=":'display:%s' % config.ui.pageDisplay">::label</div>
+       <img src=":url(getattr(transition, iconAttr),
+                      base=getattr(transition, iconBase))"
+            class=":picto|'iconS'"/>
+       <div style=":'display:%s' % config.ui.pageDisplay"
+            if="not inButtons">::label</div>
       </a>
 
       <!-- Real button -->
-      <x if="inButtons" var2="css=ui.Button.getCss(label, inButtons)">
+      <x if="not asIcon" var2="css=ui.Button.getCss(label, inButtons)">
        <input if="mayTrigger" type="button" class=":css" value=":label"
               var="back=transition.getBackHook(o, inButtons, q, backHook)"
               name=":transition.name"
               style=":url(transition.sicon, base=transition.siconBase, \
                           bg='18px 18px')"
               onclick=":'triggerTransition(%s,this.name,%s,%s)' % \
                          (q(formId), q(transition.confirm), back)"/>
@@ -430,15 +439,15 @@
       function triggerTransition(formId, transition, msg, back) {
         var f = document.getElementById(formId);
         f.action = f.dataset.baseurl + '/' + transition + '/fire';
         submitForm(formId, msg, true, back);
       }''')
 
     # Fields to copy from Transition to UiTransition
-    copied = ('name', 'icon', 'iconBase', 'sicon', 'siconBase')
+    copied = ('name', 'icon', 'iconBase', 'sicon', 'siconBase', 'iconOnly')
 
     def __init__(self, transition, o, mayTrigger):
         _ = o.translate
         # The tied p_transition
         self.transition = transition
         # Copy p_transitions fields here
         for name in UiTransition.copied:
@@ -467,8 +476,19 @@
            DOM node. Else (ie, the entire page needs to be refreshed), it
            returns None.'''
         if inButtons and not self.transition.redirect:
             r = q(backHook or o.iid)
         else:
             r = 'null'
         return r
+
+    def getIconTitle(self):
+        '''Compute the title of the icon representing the transition, when this
+           latter is represented by an icon only.'''
+        if not self.mayTrigger:
+            r = self.reason
+        elif self.iconOnly:
+            r = self.title
+        else:
+            r = ''
+        return r
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
```

### Comparing `appy-1.0.8/py3/appy/peer/__init__.py` & `appy-1.0.9/py3/appy/peer/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/peer/appy0.py` & `appy-1.0.9/py3/appy/peer/appy0.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/peer/importer.py` & `appy-1.0.9/py3/appy/peer/importer.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/peer/unresolved.py` & `appy-1.0.9/py3/appy/peer/unresolved.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/__init__.py` & `appy-1.0.9/py3/appy/pod/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/actions.py` & `appy-1.0.9/py3/appy/pod/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,25 +146,35 @@
             eRes = None
             if self.expr:
                 eRes,error = self.evaluateExpression(result, context, self.expr)
             if not error:
                 # Trigger action-specific behaviour
                 self.do(result, context, eRes)
 
+    def getBufferStart(self):
+        '''If the start of the tied buffer must be ignored (=not be part of the
+           buffer, once evaluated), this method may return the start index
+           from which content will effectively be dumped.'''
+        return
+
     def evaluateBuffer(self, result, context,
                        forceSource=None, ignoreMinus=False):
         '''Evaluates the buffer tied to this action and add the result in
            p_result. The source for evaluation can be forced to p_forceSource
            but in most cases depends on self.source.'''
         # Determine the source
         source = forceSource or self.source
         # Determine "minus"
         minus = False if ignoreMinus else self.minus
         if source == 'buffer':
-            self.buffer.evaluate(result, context, removeMainElems=minus)
+            self.buffer.evaluate(result, context, removeMainElems=minus,
+                                 forceStart=self.getBufferStart())
+            # m_getBufferStart may determine if the start of the buffer must be
+            # ignored, by forcing a start index: everything before this index
+            # will be ignored.
         else:
             # Evaluate self.fromExpr in fromRes
             fromRes = None
             error = False
             try:
                 fromRes = Evaluator.run(self.fromExpr, context)
             except Exception as e:
@@ -190,14 +200,24 @@
             # Transmit "minus" to the sub-action. Indeed, the responsiblity to
             # dump content in the buffer is delegated to the sub-action,
             # "minus-ity" included.
             action.minus = self.minus
         else:
             self.subAction.addSubAction(action)
 
+    def getAction(self, type):
+        '''If p_self or one of its sub-actions (recursively) is of this p_type,
+           returns it.'''
+        # Return p_self itself, if it has this p_type
+        if self.__class__.__name__ == type: return self
+        # Check subAction
+        sub = self.subAction
+        if not sub: return
+        return sub.getAction(type)
+
     def check(self):
         '''Returns a tuple (success, message) indicating if the action is well
            formed or not.'''
         return True, None
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class If(Action):
@@ -422,14 +442,19 @@
         context.update(hiddenVars)
         if elems:
             for name in self.iters:
                 if (name not in hiddenVars) and (name in context):
                     # On error, name may not be in the context
                     del context[name]
 
+    def getBufferStart(self):
+        '''In the context of a "do doc" statement, some tags must only be
+           dumped once and must be ignored in the subsequent iterations.'''
+        return
+
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Null(Action):
     '''Action that does nothing. Used in conjunction with a "from" clause, it
        allows to insert in a buffer arbitrary odt content.'''
     noFromError = 'There was a problem with this action. Possible causes: ' \
       '(1) you specified no action (ie "do text") while not specifying any ' \
       'from clause; (2) you specified the from clause on the same line as ' \
@@ -487,63 +512,85 @@
             self.evaluateBuffer(result, context,
                                 forceSource='buffer', ignoreMinus=True)
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Variables(Action):
     '''Action that allows to define a set of variables somewhere in the
        template.'''
-    def __init__(self, name, buff, elem, minus, variables):
-        # We do not use the default Buffer.expr attribute for storing the Python
-        # expression, because here we will have several expressions, one for
+
+    def __init__(self, name, buff, elem, minus, variables, lasting=False):
+        # The default Buffer.expr attribute is not used for storing the Python
+        # expression, because several expressions can exist here, one for
         # every defined variable.
         Action.__init__(self, name, buff, None, elem, minus)
         # Definitions of variables: ~[(s_name|[s_name], s_expr)]~. It allows a
         # variable definition to be of the form ("*", s_expr). In that case, it
         # is a multi-variable definition: s_expr must return a dict-like object
         # whose keys are strings. For every entry in this dict, a variable will
         # be defined, whose name is the key in the dict, and whose value is the
         # corresponding value at that key.
         self.variables = variables
+        # If p_lasting is:
+        # ----------------------------------------------------------------------
+        # False | (the default) every variable's scope will be the target
+        #       | element (as determined by the corresponding buffer), not more.
+        #       | Any homonym variable being defined in the outer scope will be
+        #       | hidden in the context of the target element, and will be
+        #       | visible again as soon as the walk leaves this sub-scope.
+        # ----------------------------------------------------------------------
+        # True  | From the moment such a "lasting" variable is defined, its
+        #       | scope will be the remaining of the document. So, its scope
+        #       | encompasses the target element + the remaining of the
+        #       | document. Any homonym variable being previously defined will
+        #       | be hidden forever, as soon as the lasting variable is defined.
+        # ----------------------------------------------------------------------
+        self.lasting = lasting
 
     def storeVariable(self, name, value, context, hidden):
         '''Adds a variable named p_name with this p_value in the p_context.
            Updates the dict of p_hidden variables and r_eturn it.'''
         if name.startswith('@'):
             # "name" represents a global variable. Update its value in the
             # context with p_value.
             context[name[1:]] = value
         else:
             # Store variable p_name with p_value in the p_context. If this
             # variable already exists in the context, remember its previous
-            # value in p_hidden.
-            if name in context:
+            # value in p_hidden, excepted if the currently defined variables are
+            # lasting.
+            if not self.lasting and name in context:
                 if not hidden:
                     hidden = {name: context[name]}
                 else:
                     hidden[name] = context[name]
             # Store the result into the context
             context[name] = value
         return hidden
 
     def removeVariable(self, name, context, hidden):
         '''Remove, when relevant, variable p_name from the p_context'''
         # Do not remove it if it is a global variable
         if name.startswith('@'): return
         # Do not remove it if it is an overridden variable
-        if hidden and (name in hidden): return
+        if hidden and name in hidden: return
         del context[name]
 
     def do(self, result, context, exprRes):
         '''Evaluate the variables' expressions'''
-        # Because there are several expressions, we do not use the standard,
-        # single-expression-minded Action code for evaluating expressions.
 
-        # v_hidden stores names and values of the variables that we will hide in
-        # the context. After execution of this buffer, values will be restored.
-        # v_multi stores (in reverse order) encountered multivariable values.
+        # Because there are several expressions, the standard,
+        # single-expression-minded Action code is not used for evaluating
+        # expressions.
+
+        # If the currently defined variables are not lasting, the names and
+        # values of the variables that will be hidden in the context will be
+        # stored in v_hidden. After execution of this buffer, their values
+        # will be restored. v_multi stores (in reverse order) encountered
+        # multivariable values.
+
         hidden = multi = None
         for names, expr in self.variables:
             # Evaluate variable expression in v_expr
             value, error = self.evaluateExpression(result, context, expr)
             if error: return
             if names == '*':
                 # A multi-variable
@@ -569,20 +616,21 @@
         if self.subAction:
             self.subAction.execute(result, context)
         else:
             # Evaluate the buffer directly
             self.evaluateBuffer(result, context)
         # Restore hidden variables if any
         if hidden: context.update(hidden)
-        # Delete not-hidden variables
-        for names, expr in self.variables:
-            if names == '*':
-                values = multi.pop()
-                if values:
-                    for name in values.keys():
+        # Delete not-hidden variables, if not lasting
+        if not self.lasting:
+            for names, expr in self.variables:
+                if names == '*':
+                    values = multi.pop()
+                    if values:
+                        for name in values.keys():
+                            self.removeVariable(name, context, hidden)
+                elif isinstance(names, str):
+                    self.removeVariable(names, context, hidden)
+                else:
+                    for name in names:
                         self.removeVariable(name, context, hidden)
-            elif isinstance(names, str):
-                self.removeVariable(names, context, hidden)
-            else:
-                for name in names:
-                    self.removeVariable(name, context, hidden)
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
```

### Comparing `appy-1.0.8/py3/appy/pod/buffers.py` & `appy-1.0.9/py3/appy/pod/buffers.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,24 +299,29 @@
         # Attributes instance is tied to an Expression; because dumping
         # expressions directly into FileBuffer instances seems to be rare, it
         # should not be a severe problem.
         pass
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class MemoryBuffer(Buffer):
+    '''Buffer whose content is loaded in RAM'''
+
     class Rex:
         '''Regular expressions in use for a memory buffer'''
-        part = '(for|if|else|with|meta-if)\s*(.*)'
+        part = '(for|if|else|with\+|with|meta-if)\s*(.*)'
         action = re.compile('(?:(\w+)\s*\:\s*)?do\s+(\w+)(-)?(?:\s+%s)?' % part)
         subAction = re.compile(part)
         for_ = re.compile('\s*([\w\-_,\s]+)\s+in\s+(.*)')
         vars_ = re.compile('\s*([\w\-_*,\s@]+)\s*=\s*(.*)')
         var_ = re.compile('@?[\w\-_]+')
         from_ = re.compile('from(\+)?\s+(.*)')
 
+    # Existing variants for the "with" statement
+    withVariants = {'with': None, 'with+': None}
+
     def __init__(self, env, parent):
         Buffer.__init__(self, env, parent)
         self.content = ''
         self.elements = {}
         self.action = None
 
     def clone(self):
@@ -488,16 +493,16 @@
             for index, buf in self.subBuffers.items():
                 self.parent.subBuffers[oldParentLength + index] = buf
         # Empty the buffer
         MemoryBuffer.__init__(self, self.env, self.parent)
         # Change buffer position wrt parent
         self.parent.pushSubBuffer(self)
 
-    def addElement(self, elem, elemType='pod'):
-        if elemType == 'pod':
+    def addElement(self, elem, pod=True):
+        if pod:
             elem = PodElement.create(elem)
         self.elements[self.getLength()] = elem
         if isinstance(elem, Cell) or isinstance(elem, Table):
             elem.tableInfo = self.env.getTable()
             if isinstance(elem, Cell):
                 # Remember where this cell is in the table
                 elem.colIndex = elem.tableInfo.curColIndex
@@ -582,15 +587,17 @@
         return r
 
     def createPodAction(self, actionType, statements, statementName, subExpr,
                         podElem, minus, main=True):
         '''Creates an Action instance, depending on p_actionType'''
         if actionType == 'if':
             r = actions.If(statementName, self, subExpr, podElem, minus)
-            if main:
+            # In the case of multi-statements, only the first "if" will be
+            # connectable to an "else" statement.
+            if main or not self.action.getAction('If'):
                 self.env.ifActions.append(r)
                 if r.name:
                     # We must register this action as a named action
                     if r.name in self.env.namedIfActions:
                         raise ParsingError(DUP_N_IF)
                     self.env.namedIfActions[r.name] = r
         elif actionType == 'else':
@@ -614,17 +621,18 @@
         elif actionType == 'for':
             forRes = self.Rex.for_.match(subExpr.strip())
             if not forRes:
                 raise ParsingError(FOR_KO % subExpr)
             iters, subExpr = forRes.groups()
             iters = self._getForIterators(iters)
             r = actions.For(statementName, self, subExpr, podElem, minus, iters)
-        elif actionType == 'with':
-            variables = self._getVariables(subExpr)
-            r = actions.Variables(statementName, self, podElem, minus,variables)
+        elif actionType in self.withVariants:
+            r = actions.Variables(statementName, self, podElem, minus,
+                                  self._getVariables(subExpr),
+                                  lasting=actionType.endswith('+'))
         elif actionType == 'meta-if':
             r = actions.MetaIf(self, subExpr, podElem, minus, statements)
         else:
             r = actions.Null(self, podElem)
         return r
 
     def createPodActions(self, statements):
@@ -637,17 +645,17 @@
             if not statements: raise ParsingError(EMP_NOTE)
             # Get the main statement (starting with "do...") and check it
             main = statements[0]
             aRes = self.Rex.action.match(main)
             if not aRes:
                 raise ParsingError(BAD_ST % main)
             statementName, podElem, minus, actionType, subExpr = aRes.groups()
-            if not (podElem in PodElement.POD_ELEMS):
+            if podElem not in PodElement.POD_ELEMS_D:
                 raise ParsingError(BAD_ELT % podElem)
-            if minus and (not podElem in PodElement.MINUS_ELEMS):
+            if minus and podElem not in PodElement.MINUS_ELEMS_D:
                 raise ParsingError(BAD_MNS % (podElem,PodElement.MINUS_ELEMS))
             # Find the target element in the buffer
             i = self.getIndex(podElem)
             if i == -1:
                 raise ParsingError(ELT_N_F % (podElem, str([
                         e.__class__.__name__.lower() \
                         for e in self.elements.values()])))
@@ -847,15 +855,15 @@
         pos = self.content.find('>', pos)
         for index in list(self.elements.keys()):
             if index < pos: del(self.elements[index])
 
     reTagContent = re.compile('<(?P<p>[\w-]+):(?P<f>[\w-]+)(.*?)>.*</(?P=p):' \
                               '(?P=f)>', re.S)
     def evaluate(self, result, context, subElements=True,
-                 removeMainElems=False):
+                 removeMainElems=False, forceStart=None):
         '''Evaluates this buffer given the current p_context and add the result
            into p_result. With pod, p_result is the root file buffer; with px
            it is a memory buffer.'''
         if not subElements:
             # Dump the root tag in this buffer, but not its content
             res = self.reTagContent.match(self.content.strip())
             if not res: result.write(self.content)
@@ -865,15 +873,16 @@
                 if self.env.parser.caller.protection and (g2 == 'table-cell'):
                     # Attribute "protected" must be removed
                     g3 = g3.replace('table:protected=" "', '')
                 r = '<%s:%s%s></%s:%s>' % (g1, g2, g3, g1, g2)
                 result.write(r)
         else:
             if removeMainElems: self.removeAutomaticExpressions()
-            currentIndex = self.getStartIndex(removeMainElems)
+            currentIndex = self.getStartIndex(removeMainElems) \
+                           if forceStart is None else forceStart
             for index, evalEntry in BufferIterator(self):
                 result.write(self.content[currentIndex:index])
                 currentIndex = index + 1
                 if isinstance(evalEntry, Expression):
                     try:
                         res, escape = evalEntry.evaluate(context)
                         if escape: result.dumpContent(res)
```

### Comparing `appy-1.0.8/py3/appy/pod/content.xmlt` & `appy-1.0.9/py3/appy/pod/content.xmlt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/converter.py` & `appy-1.0.9/py3/appy/pod/converter.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/doc_importers.py` & `appy-1.0.9/py3/appy/pod/doc_importers.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/elements.py` & `appy-1.0.9/py3/appy/pod/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,32 @@
 # You should have received a copy of the GNU General Public License along with
 # Appy. If not, see <http://www.gnu.org/licenses/>.
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 from xml.sax.saxutils import quoteattr
 
 from appy.xml import Tag
+from appy.utils import asDict
 from appy.pod import PodError, Evaluator
 from appy.pod.odf_parser import OdfEnvironment as ns
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class PodElement:
-    OD_TO_POD = {'p': 'Text', 'h': 'Title', 'list-item': 'Item',
-                 'section': 'Section', 'table': 'Table', 'table-row': 'Row',
-                 'table-cell': 'Cell', None: 'Expression', 'frame': 'Frame'}
-    POD_ELEMS = ('text', 'title', 'item', 'section', 'table', 'row', 'cell',
-                 'frame')
+    OD_TO_POD   = {'p': 'Text', 'h': 'Title', 'list-item': 'Item',
+                   'section': 'Section', 'table': 'Table', 'table-row': 'Row',
+                   'table-cell': 'Cell', None: 'Expression', 'frame': 'Frame',
+                   'text': 'Doc'}
+    POD_ELEMS   = ('text', 'title', 'item', 'section', 'table', 'row', 'cell',
+                   'frame', 'doc')
+    POD_ELEMS_D = asDict(POD_ELEMS)
     subTags = []
 
     # Elements for which the '-' operator can be applied
     MINUS_ELEMS = ('section', 'table')
+    MINUS_ELEMS_D = asDict(('section', 'table'))
 
     @staticmethod
     def create(elem):
         '''Used to create any POD elem that has an equivalent OD element. Not
            for creating expressions, for example.'''
         return eval(PodElement.OD_TO_POD[elem])()
 
@@ -87,14 +91,19 @@
         self.tableInfo = None # ~OdTable~
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Frame(PodElement):
     OD = Tag('frame', nsUri=ns.NS_DRAW)
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
+class Doc(PodElement):
+    '''Represents the base tag for a complete ODT document'''
+    OD = Tag('text', nsUri=ns.NS_OFFICE)
+
+#- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Expression(PodElement):
     '''Represents a Python expression that is found in a pod or px.'''
     OD = None
     metaWraps = {'"': '&quot;', "'": '&apos;'}
 
     def extractInfo(self, py):
         '''Within p_py, several elements can be included:
```

### Comparing `appy-1.0.8/py3/appy/pod/imageNotFound.jpg` & `appy-1.0.9/py3/appy/pod/imageNotFound.jpg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/lo_pool.py` & `appy-1.0.9/py3/appy/pod/lo_pool.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/odf_parser.py` & `appy-1.0.9/py3/appy/pod/odf_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,40 +15,42 @@
 # You should have received a copy of the GNU General Public License along with
 # Appy. If not, see <http://www.gnu.org/licenses/>.
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 from appy.xml import Environment, Parser
 
 class OdfEnvironment(Environment):
-    '''This environment is specific for parsing ODF files.'''
+    '''This environment is specific for parsing ODF files'''
+
     # URIs of namespaces found in ODF files
     NS_OFFICE = 'urn:oasis:names:tc:opendocument:xmlns:office:1.0'
-    NS_STYLE = 'urn:oasis:names:tc:opendocument:xmlns:style:1.0'
-    NS_TEXT = 'urn:oasis:names:tc:opendocument:xmlns:text:1.0'
-    NS_TABLE = 'urn:oasis:names:tc:opendocument:xmlns:table:1.0'
-    NS_DRAW = 'urn:oasis:names:tc:opendocument:xmlns:drawing:1.0'
-    NS_FO = 'urn:oasis:names:tc:opendocument:xmlns:xsl-fo-compatible:1.0'
-    NS_XLINK = 'http://www.w3.org/1999/xlink'
-    NS_DC = 'http://purl.org/dc/elements/1.1/'
-    NS_META = 'urn:oasis:names:tc:opendocument:xmlns:meta:1.0'
+    NS_STYLE  = 'urn:oasis:names:tc:opendocument:xmlns:style:1.0'
+    NS_TEXT   = 'urn:oasis:names:tc:opendocument:xmlns:text:1.0'
+    NS_TABLE  = 'urn:oasis:names:tc:opendocument:xmlns:table:1.0'
+    NS_DRAW   = 'urn:oasis:names:tc:opendocument:xmlns:drawing:1.0'
+    NS_FO     = 'urn:oasis:names:tc:opendocument:xmlns:xsl-fo-compatible:1.0'
+    NS_XLINK  = 'http://www.w3.org/1999/xlink'
+    NS_DC     = 'http://purl.org/dc/elements/1.1/'
+    NS_META   = 'urn:oasis:names:tc:opendocument:xmlns:meta:1.0'
     NS_NUMBER = 'urn:oasis:names:tc:opendocument:xmlns:datastyle:1.0'
-    NS_SVG = 'urn:oasis:names:tc:opendocument:xmlns:svg-compatible:1.0'
-    NS_CHART = 'urn:oasis:names:tc:opendocument:xmlns:chart:1.0'
-    NS_DR3D = 'urn:oasis:names:tc:opendocument:xmlns:dr3d:1.0'
-    NS_MATH = 'http://www.w3.org/1998/Math/MathML'
-    NS_FORM = 'urn:oasis:names:tc:opendocument:xmlns:form:1.0'
+    NS_SVG    = 'urn:oasis:names:tc:opendocument:xmlns:svg-compatible:1.0'
+    NS_CHART  = 'urn:oasis:names:tc:opendocument:xmlns:chart:1.0'
+    NS_DR3D   = 'urn:oasis:names:tc:opendocument:xmlns:dr3d:1.0'
+    NS_MATH   = 'http://www.w3.org/1998/Math/MathML'
+    NS_FORM   = 'urn:oasis:names:tc:opendocument:xmlns:form:1.0'
     NS_SCRIPT = 'urn:oasis:names:tc:opendocument:xmlns:script:1.0'
-    NS_OOO = 'http://openoffice.org/2004/office'
-    NS_OOOW = 'http://openoffice.org/2004/writer'
-    NS_OOOC = 'http://openoffice.org/2004/calc'
-    NS_DOM = 'http://www.w3.org/2001/xml-events'
+    NS_OOO    = 'http://openoffice.org/2004/office'
+    NS_OOOW   = 'http://openoffice.org/2004/writer'
+    NS_OOOC   = 'http://openoffice.org/2004/calc'
+    NS_DOM    = 'http://www.w3.org/2001/xml-events'
     NS_XFORMS = 'http://www.w3.org/2002/xforms'
-    NS_XSD = 'http://www.w3.org/2001/XMLSchema'
-    NS_XSI = 'http://www.w3.org/2001/XMLSchema-instance'
+    NS_XSD    = 'http://www.w3.org/2001/XMLSchema'
+    NS_XSI    = 'http://www.w3.org/2001/XMLSchema-instance'
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class OdfParser(Parser):
     '''XML parser that is specific for parsing ODF files'''
+
     def __init__(self, env=None, caller=None):
         env = env or OdfEnvironment()
         Parser.__init__(self, env, caller)
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
```

### Comparing `appy-1.0.8/py3/appy/pod/parts.py` & `appy-1.0.9/py3/appy/pod/parts.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/pod_parser.py` & `appy-1.0.9/py3/appy/pod/pod_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,23 @@
 from appy.xml import Tag
 from appy.pod.elements import *
 from appy.pod.buffers import FileBuffer, MemoryBuffer
 from appy.pod.odf_parser import OdfEnvironment, OdfParser
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class OdTable:
-    '''Informations about the currently parsed Open Document (Od)table.'''
+    '''Informations about the currently parsed Open Document (Od)table'''
     def __init__(self):
         self.nbOfColumns = 0
         self.nbOfRows = 0
         self.curColIndex = None
         self.curRowAttrs = None
 
     def isOneCell(self):
-        return (self.nbOfColumns == 1) and (self.nbOfRows == 1)
+        return self.nbOfColumns == 1 and self.nbOfRows == 1
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class OdInsert:
     '''While parsing an odt/pod file, we may need to insert a specific odt chunk
        at a given place in the odt file (ie: add the pod-specific fonts and
        styles). OdInsert instances define such 'inserts' (what to insert and
        when).'''
@@ -225,17 +225,18 @@
         }
         self.tags = tags
         self.ignorableTags = (tags['tracked-changes'], tags['change'])
         self.exprStartElems = [self.exprStartTags[holder] \
                                for holder in self.expressionsHolders]
         self.exprEndElems = [self.exprEndTags[holder] \
                              for holder in self.expressionsHolders]
-        self.impactableTags = (Text.OD.nsName, Title.OD.nsName, Item.OD.nsName,
-                               Table.OD.nsName, Row.OD.nsName, Cell.OD.nsName,
-                               Section.OD.nsName, Frame.OD.nsName)
+        self.impactableTags = (
+          Text.OD.nsName, Title.OD.nsName, Item.OD.nsName   , Table.OD.nsName,
+          Row.OD.nsName , Cell.OD.nsName , Section.OD.nsName, Frame.OD.nsName,
+          Doc.OD.nsName)
         self.inserts = self.transformInserts()
 
     def getExpression(self, elem):
         '''We have found a pod expression within p_elem, get its value'''
         # Expression may have been found at various places
         if self.currentDbExpression:
             r = self.currentDbExpression
```

### Comparing `appy-1.0.8/py3/appy/pod/renderer.py` & `appy-1.0.9/py3/appy/pod/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from collections import UserDict
 import zipfile, shutil, xml.sax, os, os.path, re, mimetypes, time
 
 import appy.pod
 from appy import utils
 from appy.xml import Tag
 from appy.pod import PodError
+from appy.xml.escape import Escape
 from appy.pod.lo_pool import LoPool
 from appy.utils.zip import unzip, zip
 from appy.pod.buffers import FileBuffer
 from appy.utils.path import FolderDeleter
 from appy.pod.converter import FILE_TYPES
 from appy.pod import styles_manager as sm
 from appy.pod import doc_importers as importers
@@ -654,15 +655,16 @@
                 css = firstCss
                 pre = prefix
             elif i == length:
                 css = lastCss
             else:
                 css = otherCss
             css = ' class="%s"' % css if css else ''
-            r[i] = '<p%s>%s%s%s%s</p>' % (css, pre, opening, r[i], closing)
+            r[i] = '<p%s>%s%s%s%s</p>' % (css, pre, opening,
+                                          Escape.xhtml(r[i]), closing)
             i -= 1
         return self.renderXhtml(''.join(r), stylesMapping=stylesMapping)
 
     # Supported image formats. "image" represents any format
     imageFormats = ('png', 'jpeg', 'jpg', 'gif', 'svg', 'image')
     ooFormats = ('odt',)
     convertibleFormats = FILE_TYPES.keys()
```

### Comparing `appy-1.0.8/py3/appy/pod/styles.xmlt` & `appy-1.0.9/py3/appy/pod/styles.xmlt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/styles_manager.py` & `appy-1.0.9/py3/appy/pod/styles_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,22 +55,24 @@
 TXT_ODT_P  = 'For XHTML element "%s", you must associate an OpenDocument ' \
              '"text" style (that applies to only a chunk of text within a ' \
              'paragraph). "%s" is a paragraph-wide style.'
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Properties:
     '''Abstract base class for table and list properties'''
+
     # HTML elements whose styles are defined by Property instances instead of
     # Style instances.
     elems = ('table', 'ol', 'ul')
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class TableProperties(Properties):
     '''In a styles mapping, the value @key "table" must be an instance of this
        class.'''
+
     defaultMargins = (0.3, 0.0, 0.3, 0.0)
     columnModifiersPrefixes = {'optimize': 'OCW', 'distribute': 'DC'}
 
     def __init__(self, pageWidth=None, px2cm=px2cm, cellPx2cm=10.0,
               wideAbove=495, minColumnWidth=0.07, columnModifier=None,
               minCellPadding=0.0, cellContentStyle='podCellContent',
               headerContentStyle='podHeaderCellContent', margins=defaultMargins,
@@ -266,14 +268,15 @@
         '''Allows to define text properties at level p_i'''
         return ''
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class BulletedProperties(ListProperties):
     '''In a styles mapping, the value @key "ul" must be an instance of this
        class.'''
+
     type = 'bullet'
     defaultFormats = ('•', '◦', '▪')
     textStyle = 'podBulletStyle'
 
     def __init__(self, levels=4, formats=defaultFormats,
                  delta=0.32, firstDelta=None, space=0.32, paraStyle=None):
         ListProperties.__init__(self, levels, formats, delta, firstDelta,
@@ -285,14 +288,15 @@
         return '%s:bullet-char="%s"' % \
                (nsText, utils.getElementAt(self.formats, i))
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class NumberedProperties(ListProperties):
     '''In a styles mapping, the value @key "ol" must be an instance of this
        class.'''
+
     type = 'number'
     defaultFormats = ('1',)
     defaultSuffixes = ('.',)
     textStyle = 'podNumberStyle'
 
     def __init__(self, levels=4, formats=defaultFormats,
                  suffixes=defaultSuffixes, delta=0.32, firstDelta=None,
```

### Comparing `appy-1.0.8/py3/appy/pod/test/Readme.txt` & `appy-1.0.9/py3/appy/pod/test/Readme.txt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/Tester.py` & `appy-1.0.9/py3/appy/pod/test/Tester.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/__init__.py` & `appy-1.0.9/py3/appy/pod/test/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/ForCell6.py` & `appy-1.0.9/py3/appy/pod/test/contexts/ForCell6.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/ImagesImport.py` & `appy-1.0.9/py3/appy/pod/test/contexts/ImagesImport.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlColgroupTable.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlColgroupTable.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex2.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex2.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex3.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex3.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex4.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex4.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex5.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex5.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex7.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex7.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex8.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex8.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,7 +21,9 @@
 </blockquote>
 
 <p>Only flowing text passes :</p>
 <blockquote>
 This text is rendered.
 </blockquote>
 '''
+
+text1 = '''IMIO & Geezteem'''
```

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplex9.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplex9.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlComplexTables.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlComplexTables.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlCustomStyles.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlCustomStyles.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlKeepWithNext.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlKeepWithNext.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlNominal.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlNominal.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlPIntoLis.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlPIntoLis.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 xhtmlInput = '''
 <ol>
  <li>Row 1;</li>
  <li>row 2 :
   <p>- sub-paragraph, row 1</p>
   <p>- sub-paragraph, row 2</p>
  </li>
- <li><p>row 3;</p></li>
+ <li><p class="Signature">row 3 (Signature style applied);</p></li>
  <li>row 4:
    <ul>
      <li>Sub list:<p>aa</p><div>bb</div><div>aa</div></li>
      <li><div>Hello</div></li>
      <li>Normal</li>
    </ul>
  </li>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- xhtmlInput = '''
    1. Row 1;
    2. row 2 :
       - sub-paragraph, row 1
       - sub-paragraph, row 2
-   3. row 3;
+   3. row 3 (Signature style applied);
    4. row 4:
           o Sub list:
             aa
             bb
             aa
           o Hello
           o Normal
```

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlSpan.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlSpan.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlStylesMapping.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlStylesMapping.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlTables.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlTables.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlTwisted.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlTwisted.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/XhtmlWithStyle.py` & `appy-1.0.9/py3/appy/pod/test/contexts/XhtmlWithStyle.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/contexts/__init__.py` & `appy-1.0.9/py3/appy/pod/test/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/images/imio.png` & `appy-1.0.9/py3/appy/pod/test/images/imio.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/images/linux.jpg` & `appy-1.0.9/py3/appy/pod/test/images/linux.jpg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/images/plone.png` & `appy-1.0.9/py3/appy/pod/test/images/plone.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/images/python.blob` & `appy-1.0.9/py3/appy/pod/test/images/python.blob`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/images/python.gif` & `appy-1.0.9/py3/appy/pod/test/images/python.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/chart1.odt` & `appy-1.0.9/py3/appy/pod/test/results/chart1.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/errorExpression.odt` & `appy-1.0.9/py3/appy/pod/test/results/errorExpression.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/errorFooter.odt` & `appy-1.0.9/py3/appy/pod/test/results/errorFooter.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/errorForRuntime.odt` & `appy-1.0.9/py3/appy/pod/test/results/errorForRuntime.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/errorIf.odt` & `appy-1.0.9/py3/appy/pod/test/results/errorIf.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/fieldExpression.odt` & `appy-1.0.9/py3/appy/pod/test/results/fieldExpression.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/fileHandlerImport.odt` & `appy-1.0.9/py3/appy/pod/test/results/fileHandlerImport.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/forCellBug.odt` & `appy-1.0.9/py3/appy/pod/test/results/forCellBug.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/forCellBug2.odt` & `appy-1.0.9/py3/appy/pod/test/results/forCellBug2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/forCellCorrectNumber.odt` & `appy-1.0.9/py3/appy/pod/test/results/forCellCorrectNumber.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/forCellNotEnough.odt` & `appy-1.0.9/py3/appy/pod/test/results/forCellNotEnough.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/forCellOnlyOne.odt` & `appy-1.0.9/py3/appy/pod/test/results/forCellOnlyOne.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/forCellTooMuch1.odt` & `appy-1.0.9/py3/appy/pod/test/results/forCellTooMuch1.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/forCellTooMuch2.odt` & `appy-1.0.9/py3/appy/pod/test/results/forCellTooMuch2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/forCellTooMuch3.odt` & `appy-1.0.9/py3/appy/pod/test/results/forCellTooMuch3.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/forCellTooMuch4.odt` & `appy-1.0.9/py3/appy/pod/test/results/forCellTooMuch4.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/forTable.odt` & `appy-1.0.9/py3/appy/pod/test/results/forTable.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/forTableMinus.odt` & `appy-1.0.9/py3/appy/pod/test/results/forTableMinus.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/forTableMinus2.odt` & `appy-1.0.9/py3/appy/pod/test/results/forTableMinus2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/forTableMinusError.odt` & `appy-1.0.9/py3/appy/pod/test/results/forTableMinusError.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/forTableMinusError2.odt` & `appy-1.0.9/py3/appy/pod/test/results/forTableMinusError2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/headerFooter.odt` & `appy-1.0.9/py3/appy/pod/test/results/headerFooter.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/ifAndFors1.odt` & `appy-1.0.9/py3/appy/pod/test/results/ifAndFors1.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/ifElseErrors.odt` & `appy-1.0.9/py3/appy/pod/test/results/ifElseErrors.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/imagesImport.odt` & `appy-1.0.9/py3/appy/pod/test/results/imagesImport.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/noPython.odt` & `appy-1.0.9/py3/appy/pod/test/results/noPython.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/odsSimple.ods` & `appy-1.0.9/py3/appy/pod/test/results/odsSimple.ods`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/onlyExpressions.odt` & `appy-1.0.9/py3/appy/pod/test/results/onlyExpressions.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/pathImport.odt` & `appy-1.0.9/py3/appy/pod/test/results/pathImport.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/simpleForEmptyList.odt` & `appy-1.0.9/py3/appy/pod/test/results/simpleForEmptyList.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/simpleForFilledList.odt` & `appy-1.0.9/py3/appy/pod/test/results/simpleForFilledList.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/simpleForRow.odt` & `appy-1.0.9/py3/appy/pod/test/results/simpleForRow.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/simpleFromTest.odt` & `appy-1.0.9/py3/appy/pod/test/results/simpleFromTest.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/simpleIfIsFalse.odt` & `appy-1.0.9/py3/appy/pod/test/results/simpleIfIsFalse.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/simpleIfIsTrue.odt` & `appy-1.0.9/py3/appy/pod/test/results/simpleIfIsTrue.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/simpleIfIsTrue003.odt` & `appy-1.0.9/py3/appy/pod/test/results/simpleIfIsTrue003.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/simpleMinusError.odt` & `appy-1.0.9/py3/appy/pod/test/results/simpleMinusError.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/simpleTest.odt` & `appy-1.0.9/py3/appy/pod/test/results/simpleTest.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/varDef.odt` & `appy-1.0.9/py3/appy/pod/test/results/varDef.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/withAnImage.odt` & `appy-1.0.9/py3/appy/pod/test/results/withAnImage.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlColgroup.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlColgroup.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex2.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex3.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex3.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex4.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex4.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex5.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex5.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex6.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex6.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex7.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex7.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlComplex9.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlComplex9.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlComplexTables.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlComplexTables.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlCustomStyles.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlCustomStyles.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlEmpty.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlEmpty.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlEntities.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlEntities.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlHtml.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlHtml.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlIgnoreStyles.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlIgnoreStyles.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlInHeader.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlInHeader.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlKeepWithNext.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlKeepWithNext.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlListProperties.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlListProperties.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlNominal.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlNominal.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlPIntoLis.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlPIntoLis.odt`

 * *Files 19% similar despite different names*

#### odt2txt

```diff
@@ -1,14 +1,14 @@
 Row 1;
 
 row 2 :
 - sub-paragraph, row 1
 - sub-paragraph, row 2
 
-row 3;
+row 3 (Signature style applied);
 
 row 4:
 
 Sub list:
 aa
 bb
 aa
```

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlPIntoTds.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlPIntoTds.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlSpan.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlSpan.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlStylesErrors.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlStylesErrors.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlStylesMapping.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlStylesMapping.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlStylesMapping2.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlStylesMapping2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlTableProperties.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlTableProperties.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlTables.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlTables.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/results/xhtmlTwisted.odt` & `appy-1.0.9/py3/appy/pod/test/results/xhtmlTwisted.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/Chart1.odt` & `appy-1.0.9/py3/appy/pod/test/templates/Chart1.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ErrorExpression.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ErrorExpression.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ErrorFooter.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ErrorFooter.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ErrorForParsetime.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ErrorForParsetime.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ErrorForRuntime.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ErrorForRuntime.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ErrorIf.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ErrorIf.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/FieldExpressions.odt` & `appy-1.0.9/py3/appy/pod/test/templates/FieldExpressions.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/FileHandlerImport.odt` & `appy-1.0.9/py3/appy/pod/test/templates/FileHandlerImport.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ForCell.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ForCell.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ForCell2.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ForCell2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ForCell3.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ForCell3.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ForCell4.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ForCell4.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ForCell5.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ForCell5.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ForCell6.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ForCell6.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ForCell7.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ForCell7.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ForTable.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ForTable.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ForTableMinus.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ForTableMinus.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ForTableMinus2.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ForTableMinus2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ForTableMinusError.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ForTableMinusError.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ForTableMinusError2.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ForTableMinusError2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/FromPod.odt` & `appy-1.0.9/py3/appy/pod/test/templates/FromPod.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/HeaderFooter.odt` & `appy-1.0.9/py3/appy/pod/test/templates/HeaderFooter.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/IfAndFors1.odt` & `appy-1.0.9/py3/appy/pod/test/templates/IfAndFors1.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/IfElseErrors.odt` & `appy-1.0.9/py3/appy/pod/test/templates/IfElseErrors.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/ImagesImport.odt` & `appy-1.0.9/py3/appy/pod/test/templates/ImagesImport.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/NoPython.odt` & `appy-1.0.9/py3/appy/pod/test/templates/NoPython.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/OdsSimple.ods` & `appy-1.0.9/py3/appy/pod/test/templates/OdsSimple.ods`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/OnlyExpressions.odt` & `appy-1.0.9/py3/appy/pod/test/templates/OnlyExpressions.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/PathImport.odt` & `appy-1.0.9/py3/appy/pod/test/templates/PathImport.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/SimpleForEmptyList.odt` & `appy-1.0.9/py3/appy/pod/test/templates/SimpleForEmptyList.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/SimpleForFilledList.odt` & `appy-1.0.9/py3/appy/pod/test/templates/SimpleForFilledList.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/SimpleForRow.odt` & `appy-1.0.9/py3/appy/pod/test/templates/SimpleForRow.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/SimpleFromTest.odt` & `appy-1.0.9/py3/appy/pod/test/templates/SimpleFromTest.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/SimpleIfIsFalse.odt` & `appy-1.0.9/py3/appy/pod/test/templates/SimpleIfIsFalse.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/SimpleIfIsTrue.odt` & `appy-1.0.9/py3/appy/pod/test/templates/SimpleIfIsTrue.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/SimpleIfIsTrue003.odt` & `appy-1.0.9/py3/appy/pod/test/templates/SimpleIfIsTrue003.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/SimpleMinusError.odt` & `appy-1.0.9/py3/appy/pod/test/templates/SimpleMinusError.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/SimpleTest.odt` & `appy-1.0.9/py3/appy/pod/test/templates/SimpleTest.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/TablesToOptimize.odt` & `appy-1.0.9/py3/appy/pod/test/templates/TablesToOptimize.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/VarStatements.odt` & `appy-1.0.9/py3/appy/pod/test/templates/VarStatements.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/WithAnImage.odt` & `appy-1.0.9/py3/appy/pod/test/templates/WithAnImage.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/Xhtml.odt` & `appy-1.0.9/py3/appy/pod/test/templates/Xhtml.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlColGroup.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlColGroup.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlComplex2.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlComplex2.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlComplex3.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlComplex3.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlComplex4.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlComplex4.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlComplexTables.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlComplexTables.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlHtml.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlHtml.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlInHeader.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlInHeader.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlKeepWithNext.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlKeepWithNext.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlNominal.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlNominal.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlSimple.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlSimple.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlSpan.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlSpan.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlStyles.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlStyles.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlStylesErrors.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlStylesErrors.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlTables.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlTables.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/test/templates/XhtmlTwisted.odt` & `appy-1.0.9/py3/appy/pod/test/templates/XhtmlTwisted.odt`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/xhtml/__init__.py` & `appy-1.0.9/py3/appy/pod/xhtml/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/xhtml/parser.py` & `appy-1.0.9/py3/appy/pod/xhtml/parser.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/xhtml/tags.py` & `appy-1.0.9/py3/appy/pod/xhtml/tags.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/xhtml/visitors.py` & `appy-1.0.9/py3/appy/pod/xhtml/visitors.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/pod/xhtml2odt.py` & `appy-1.0.9/py3/appy/pod/xhtml2odt.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,17 +135,17 @@
         # If a conflict occurs on this element, we will note it
         self.isConflictual = False
         # Sometimes we must remember the ODT style that has been computed and
         # applied to this HTML element (for lists).
         self.odStyle = None
         # For cells, the style to apply to their inner paragraphs (set later)
         self.innerStyle = None
-        # We must know if a style must be applied on inner paragraphs within
-        # "li" tags.
-        if (elem == 'li') and ('class' in attrs):
+        # Determine if a style must be applied on inner paragraphs within "li"
+        # tags.
+        if elem == 'li' and 'class' in attrs:
             self.paraStyle = attrs['class']
         else:
             self.paraStyle = None # Will also be set on "ol" and "ul" tags.
         # Must we only keep tag content and remove the tag itself ?
         self.removeTag = False
         # Must we dump a ling-break just before encountering a tag from
         # INNER_TAGS within this tag ?
@@ -206,29 +206,29 @@
            dumped a "p", we can't dump a table within the "p". Such constraints
            do not hold in XHTML code but hold in ODF code.'''
         if not env.currentTags: return ()
         parent = env.getCurrentTag()
         # Special case: check elements that can't be found within a "li".
         # Instead of being noted as "conflictual", note that we must keep
         # these element's contents but remove the surrounding tags.
-        if (parent.elem == 'li') and (self.elem in PARA_TAGS):
+        if parent.elem == 'li' and self.elem in PARA_TAGS:
             self.removeTag = True
             parent.addInnerCssStyles(self)
             return ()
         # Check elements that can't be found within a paragraph / li. The list
         # of such elements is different for a "li", but "li" has elemType
         # "para", so we must explicitly check the "li" case before checking
         # "elemType" being "para" or not.
         if parent.elem == 'li':
             if self.elem in NOT_INSIDE_LI:
                 return (parent.parent.setConflictual(),parent.setConflictual(),)
-        elif (parent.elemType == 'para') and (self.elem in NOT_INSIDE_P_OR_P):
+        elif parent.elemType == 'para' and self.elem in NOT_INSIDE_P_OR_P:
             return (parent.setConflictual(),)
         # Check inner paragraphs
-        elif (parent.elem in INNER_TAGS) and (self.elemType == 'para'):
+        elif parent.elem in INNER_TAGS and self.elemType == 'para':
             res = [parent.setConflictual()]
             if len(env.currentTags) > 1:
                 i = 2
                 visitParents = True
                 while visitParents:
                     try:
                         nextParent = env.currentTags[-i]
@@ -236,19 +236,19 @@
                         res.insert(0, nextParent.setConflictual())
                         if nextParent.elemType == 'para':
                             visitParents = False
                     except IndexError:
                         visitParents = False
             return res
         if parent.tagsToClose and \
-            (parent.tagsToClose[-1].elemType == 'para') and \
-            (self.elem in NOT_INSIDE_P_OR_P):
+           parent.tagsToClose[-1].elemType == 'para' and \
+           self.elem in NOT_INSIDE_P_OR_P:
             return (parent.tagsToClose[-1].setConflictual(),)
         # Check elements that can't be found within a list
-        if (parent.elemType == 'list') and (self.elem in NOT_INSIDE_LIST):
+        if parent.elemType == 'list' and self.elem in NOT_INSIDE_LIST:
             return (parent.setConflictual(),)
         return ()
 
     def addInnerParagraph(self, env):
         '''Dump an inner paragraph inside self (if not already done)'''
         if self.tagsToClose: return # We already did it
         dump = env.dumpString
@@ -272,17 +272,33 @@
                             styleName = env.itemStyles[itemStyle + '_kwn']
                         else:
                             styleName = css
                 styleName = styleName or env.itemStyles[itemStyle]
                 dump(' text:style-name="%s"' % styleName)
             else:
                 # Check if a style must be applied on 'p' tags
-                if self.innerCssStyles:
-                    p.cssStyles.merge(self.innerCssStyles)
-                innerStyle = listElem.paraStyle or env.itemStyles[itemStyle]
+                innerStyles = self.innerCssStyles
+                paraStyle = None
+                if innerStyles:
+                    p.cssStyles.merge(innerStyles)
+                    class_ = getattr(innerStyles, 'classes', None)
+                    if class_:
+                        # Take the last CSS class if several are defined
+                        paraStyle = class_.split()[-1]
+                # Some remarks here.
+                # 1) The CSS class defined on the "p" tag, when present, takes
+                #    precedence over the one defined at the list level (itself
+                #    copied from the applicable ListProperties instance. This
+                #    precedence rule is hard-coded: it is not possible to choose
+                #    which one prevails, as opposed to what happens with
+                #    TableProperties instances via boolean attribute "prevails".
+                # 2) The CSS class potentially defined at the level of the "li"
+                #    tag is currently ignored.
+                innerStyle = paraStyle or listElem.paraStyle or \
+                             env.itemStyles[itemStyle]
                 if innerStyle:
                     p.cssStyles.addClass(innerStyle)
                 dump(env.getOdfAttributes(p))
         else:
             dump(env.getOdfAttributes(p))
         dump('>')
         if not self.tagsToClose: self.tagsToClose = []
```

### Comparing `appy-1.0.8/py3/appy/px/__init__.py` & `appy-1.0.9/py3/appy/px/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
         # Is this language LTR or RTL ?
         dir, dleft, dright = handler.Languages.getDirection(lang)
         # The main app config
         config = handler.server.config
         # Define and return the context
         r = O(
           traversal=traversal, handler=handler, guard=guard, tool=tool, req=req,
-          o=o, layout=layout, ui=tool.ui, _=o.translate, user=user,
+          o=o, layout=layout, ui=tool.ui, _=tool.translate, user=user,
           isAnon=user.isAnon(), Px=Px, config=config, field=traversal.field,
           appName=config.model.appName, q=Quote.js, url=tool.buildUrl,
           lang=lang, dir=dir, dleft=dleft, dright=dright,
           siteUrl=config.server.getUrl(handler), _css_=config.ui.patchCss)
         # Ensure keys "ajax" and "popup" are present
         for name in ('ajax', 'popup'):
             setattr(r, name, getattr(r, name) or False)
```

### Comparing `appy-1.0.8/py3/appy/px/parser.py` & `appy-1.0.9/py3/appy/px/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 content = buffer.crunchExpr(attrs[name])
                 buffer.createPxAction(elem, name, content)
         if e.isActionElem(elem):
             # Add a temp element in the buffer (that will be unreferenced
             # later). This way, when encountering the corresponding end element,
             # we will be able to check whether the end element corresponds to
             # the main element or to a sub-element.
-            e.currentBuffer.addElement(elem, elemType='px')
+            e.currentBuffer.addElement(elem, pod=False)
         if elem != 'x':
             # Dump the start element and its attributes. But as a preamble,
             # manage special attributes that could not be dumped at all, like
             # "selected" or "checked".
             hook = None
             ignorableAttrs = self.pxAttributes
             buffer = e.currentBuffer
```

### Comparing `appy-1.0.8/py3/appy/server/__init__.py` & `appy-1.0.9/py3/appy/server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,30 +49,29 @@
 MIN_THR_KO    = 'At least one thread must be in use.'
 THR_LIMITS_KO = 'killThreadLimit (%d) should be > hungThreadLimit (%d)'
 SPAWN_IF_KO   = 'spawnIfUnder (%d) should be < than the number of threads (%d)'
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Config:
     '''HTTP server configuration for a Appy site'''
+
     def __init__(self):
         # The server address
         self.address = '0.0.0.0'
         # The server port
         self.port = 8000
         # The protocol in use. Valid values are "http" or "https"
         self.protocol = 'http'
         # The version of HTTP in use, as a float value. Currently, 1.0 and 1.1
         # are supported.
         self.httpVersion = 1.1
         # The value of the "SameSite" attribute for cookies. Can be "Lax" or
         # "Strict". More info on https://developer.mozilla.org/en-US/docs/Web/
         #                         HTTP/Headers/Set-Cookie/SameSite
         self.sameSite = 'Lax'
-        # Configuration for static content (set by m_set below)
-        self.static = None
         # The size of the queue as defined on the server socket, passed as
         # parameter to the "listen" method.
         self.queueSize = 5
         # The "poll interval", in seconds. After having entered his infinite
         # loop, the server, while waiting for incoming connections or data on
         # these connections, will be interrupted every "pollInterval" seconds.
         # Avoid setting this value to 0.0: the Appy server would take 100% CPU
@@ -92,14 +91,35 @@
         #   | client connection.
         #   |
         #   | When using this debug level, set a poll interval being higher (2
         #   | seconds or more). It will slow down the server must will produce
         #   | less verbose output.
         #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
         self.debugLevel = 0
+        # Configuration for static content (set by m_set below)
+        self.static = None
+        # Traversers. A "traverser" is a name that can be used at the root of a
+        # URL path, to traverse something else than an object. Indeed, the
+        # standard traversal is based on database objects. For instance,
+        #
+        #                      <appUrl>/666
+        #
+        # requires 666 to be the iid of a database object;
+        #
+        #                      <appUrl>/something
+        #
+        # requires "something" to point to an object stored in the database
+        # under that name in database dict root.objects.
+        # If you want to use starting URL paths not being database objects,
+        # define a traverser as an entry in the following dict.
+        # - The key is the name to be used in the URL path;
+        # - The value is a Python expression, receiving the tool as variable
+        #   "tool" in its context.
+        # Take care of security when defining traversers.
+        self.traversers = {}
         # The path to the site. Will be set by m_set below.
         self.sitePath = None
         # ~~~
         # Options for the pool of threads
         # ~~~
         # The initial number of threads to run
         self.threads = 5
```

### Comparing `appy-1.0.8/py3/appy/server/backup.py` & `appy-1.0.9/py3/appy/server/backup.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/server/context.py` & `appy-1.0.9/py3/appy/server/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,17 +166,21 @@
         # The authentication context in itself (a short identifier)
         guard.authContext = ctx
         # Its human-readable name
         guard.authContextName = self.getName(tool, user, ctx)
         # The corresponding object, if any
         guard.authObject = self.getObject(tool, user, ctx)
 
-    def isMandatory(self, tool):
+    def isMandatory(self, tool, authenticate=False):
         '''When authentication contexts are activated, is the user forced to
            choose one ?'''
+        # Not if the user must be p_authenticate(d) and it is impossible to
+        # choose any context.
+        if authenticate and not tool.config.security.authContext.chooseOnLogin:
+            return
         return True
 
     def switchContext(self, tool):
         '''Is the user allowed to switch context once logged ?'''
         return True
 
     def getContexts(self, tool, user):
```

### Comparing `appy-1.0.8/py3/appy/server/cookie.py` & `appy-1.0.9/py3/appy/server/cookie.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/server/error.py` & `appy-1.0.9/py3/appy/server/error.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/server/guard.py` & `appy-1.0.9/py3/appy/server/guard.py`

 * *Files 4% similar despite different names*

```diff
@@ -424,14 +424,25 @@
     # PXs
     #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     # A custom zone, at the bottom of pxLogin, allowing an app to add custom
     # content.
     pxLoginBottom = Px('')
 
+    def getLoginLogo(self, discreet, url):
+        '''Returns the possibly clickable logo to include in the login box'''
+        # Compute the "img" tag representing the logo
+        r = '<img src="%s"/>' % url('loginLogo')
+        # Wrap it, when appropriate, in a link allowing to go back to the public
+        # page.
+        if discreet == 'home':
+            r = '<a onclick="goto(siteUrl+\'/tool/public\')" ' \
+                'class="clickable">%s</a>' % r
+        return r
+
     # The login form
     pxLogin = Px('''
      <!-- Popup for reinitializing the password -->
      <div if="isAnon and config.security.activateForgotPassword"
           id="askPasswordReinitPopup" class="popup">
       <form id="askPasswordReinitForm" method="post"
             action=":'%s/guard/askPasswordReinit' % tool.url">
@@ -454,15 +465,17 @@
                display='none' if discreet and not req.stay else 'block'"
           style=":'display:%s' % display">
 
       <!-- Allow to hide the box when relevant -->
       <img if="discreet == True" src=":url('close.svg')" style="float:right"
            onclick="toggleLoginBox(false)" class="clickable iconXS"/>
 
-      <div align="center"><img src=":url('loginLogo')"/></div>
+      <!-- A (possibly clickable) logo -->
+      <div align="center">::guard.getLoginLogo(discreet, url)</div>
+
       <h1>::_('app_name')</h1>
       <center class="sub">:_('please_connect')</center>
       <div class="loginSpace"></div>
       <form id="loginForm" name="loginForm" method="post" class="login"
             action=":'%s/guard/enter' % tool.url">
 
        <!-- Login fields  -->
@@ -516,20 +529,21 @@
            closePopup('askPasswordReinitPopup');
            f.submit();
          }
        }''',
 
      css='''
       .loginBox {
-         border:|loginBorder| |loginColorPh|; padding:35px; color:|darkColor|;
+         border:|loginBorder| |loginColorPh|; padding:35px; color:|loginColor|;
          background-color:|boxBgColor|; position:absolute; top:|loginTop|;
          left:50%; z-index:10; transform:translate(-50%,-50%);
          box-shadow:|loginShadow|; border-radius: |loginBorderRadius|
       }
-      .loginBox a, .loginBox a:visited { font-weight:bold; letter-spacing:1px }
+      .loginBox a, .loginBox a:visited {
+        font-weight:bold; letter-spacing:1px; color:|loginColor| }
       .loginBox h1 { padding-bottom:0; margin-bottom:3px; text-align:center;
                      font-size:160%; font-weight: |loginTitleWeight| }
       .loginBox .sub { font-size:120% }
       #loginForm input {
         background-color:|loginBgColor|; width:|loginWidth|; border:none;
         padding:|loginPadding|; margin:|loginMargin|; color:|loginColor| }
       .submitLogin { text-align:|submitAlign|
```

### Comparing `appy-1.0.8/py3/appy/server/handler.py` & `appy-1.0.9/py3/appy/server/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         # Call the method if cache is not needed
         if not cache: return method(o)
         # If first arg of method is named "tool" instead of the traditional
         # "self", we cheat and will call the method with the tool as first arg.
         # This will allow to consider this method as if it was a static method
         # on the tool.
         cheat = False
-        if not class_ and (method.__code__.co_varnames[0] == 'tool'):
+        if not class_ and method.__code__.co_varnames[0] == 'tool':
             prefix = o.class_.name
             o = o.tool
             cheat = True
         # Build the unique key allowing to store method results in the cache.
         # The key is of the form
         #                    <object id>:<method name>
         # In the case of a static method, "object id" is replaced with the class
@@ -144,15 +144,15 @@
 
     # Make the Language class available in the handler namespace
     Languages = Languages
 
     def init(self):
         '''Define attributes which are common to any handler'''
         # A lot of object methods are executed while handling a request. Dict
-        # "method" hereafter caches method results: it avoids executing more
+        # "methods" hereafter caches method results: it avoids executing more
         # than once the same method. Only methods without args are cached, like
         # methods defined on field attributes such as "show".
         self.methods = MethodsCache()
         # Appy and apps may use the following object to cache any other element
         self.cache = O()
         # Create a guard, a transient object for managing security
         self.guard = Guard(self)
@@ -283,17 +283,19 @@
         '''A security-related error has occurred: the logged user is not allowed
            to access the desired URL. If the user is anon, redirect him to the
            login page. Else, return an error. p_error may contain the raised
            exception instance.'''
         # Return the response content. In the case of a redirect, None will be
         # returned.
         if self.guard.user.isAnon():
-            siteUrl = self.config.server.getUrl(self)
+            config = self.config
+            siteUrl = config.server.getUrl(self)
             gotoUrl = urllib.parse.quote('%s%s' % (siteUrl, self.path))
-            resp.goto(url='%s/tool/home?goto=%s' % (siteUrl, gotoUrl),
+            resp.goto(url='%s/tool/%s?goto=%s&stay=1' % \
+                      (siteUrl, config.ui.home, gotoUrl),
                       message=self.tool.translate('please_authenticate'))
             r = None
         else:
             # Log and return a 403 error: forbidden
             resp.code = HTTPStatus.FORBIDDEN
             r = Error.get(resp, traversal, error=error)
         return r
@@ -386,27 +388,27 @@
         # If the first part of the path corresponds to the root static folder,
         # static content must be served.
         elif parts[0] == config.server.static.root:
             self.static = True
             del parts[0]
         # If the unique part corresponds to a file (ie, any name containing a
         # dot), it is static content, too (favicon.ico, robots.txt...)
-        elif (len(parts) == 1) and ('.' in parts[0]):
+        elif len(parts) == 1 and '.' in parts[0]:
             self.static = True
             # Get this file at the place configured in the UI config
             base = config.ui.images.get(parts[0]) or 'appy'
             parts.insert(0, base)
         # In any other case, dynamic content must be served
         else:
             self.static = False
         self.parts = parts
         # Must the client socket be closed after the request has been handled ?
         httpVersion = config.server.httpVersion
-        self.closeSocket = (httpVersion == 1) or \
-                           (self.headers.get('Connection') == 'close')
+        self.closeSocket = httpVersion == 1 or \
+                           self.headers.get('Connection') == 'close'
 
     def handle(self):
         '''Called by m_run to handle a HTTP request'''
         # Determine the type of the request: static or dynamic (boolean
         # self.static). Static content is any not-database-stored-and-editable
         # image, Javascript, CSS file, etc. Dynamic content is any request
         # reading and/or writing to/from the database.
```

### Comparing `appy-1.0.8/py3/appy/server/languages.py` & `appy-1.0.9/py3/appy/server/languages.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/server/ldap.py` & `appy-1.0.9/py3/appy/server/ldap.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/server/pool.py` & `appy-1.0.9/py3/appy/server/pool.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/server/request.py` & `appy-1.0.9/py3/appy/server/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,20 +86,20 @@
             else:
                 values = [values, value]
             value = values
         self[name] = value
 
     def parse(self, params, sep='&', post=False):
         '''Parse GET/POST p_param(eters) and add one attribute per parameter'''
+        method = 'unquote_plus' if post else 'unquote'
         for param in params.split(sep):
             # Every param is of the form <name>=<value> or simply <name>
             if '=' in param:
                 # <name>=<value>
                 name, value = param.split('=', 1)
-                method = 'unquote_plus' if post else 'unquote'
                 value = getattr(urllib.parse, method)(value)
             else:
                 # <name>
                 name = param
                 value = None
             self.addValue(name, value)
```

### Comparing `appy-1.0.8/py3/appy/server/response.py` & `appy-1.0.9/py3/appy/server/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,20 +152,27 @@
     def addMessage(self, message):
         '''Adds a message to p_self.message'''
         if self.message is None:
             self.message = message
         else:
             self.message = '%s<br/>%s' % (self.message, message)
 
-    def goto(self, url=None, message=None):
+    def goto(self, url=None, message=None, fromPopup=False):
         '''Redirect the user to p_url'''
         if message: self.addMessage(message)
-        self.code = HTTPStatus.SEE_OTHER # 303
-        # Redirect to p_url or to the referer URL if no p_url has been given
-        self.headers['Location'] = url or self.handler.headers['Referer']
+        req = self.handler.req
+        if fromPopup:
+            # Redirecting back to some URL from a popup requires an alternative
+            # technique, performed by the Appy IFrame.
+            req._back = url
+        else:
+            # The standard HTTP technique
+            self.code = HTTPStatus.SEE_OTHER # 303
+            # Redirect to p_url or to the referer URL if no p_url has been given
+            self.headers['Location'] = url or self.handler.headers['Referer']
 
     def write(self, s):
         '''Writes part p_s of the response to the client socket. Returns True if
            an error occurred.'''
         try:
             self.handler.clientSocket.sendall(s)
         except BrokenPipeError:
```

### Comparing `appy-1.0.8/py3/appy/server/scheduler.py` & `appy-1.0.9/py3/appy/server/scheduler.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/server/sso.py` & `appy-1.0.9/py3/appy/server/sso.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         '''Formats the user-related data from the request (HTTP headers), as a
            dict of params usable for creating or updating the corresponding
            Appy user.'''
         res = {}
         headers = req._orig_env
         encoding = self.extractEncoding(headers)
         decodeFunction = self.decodeFunction
-        for keyAttr, appyName in self.ssoAttributes.iteritems():
+        for keyAttr, appyName in self.ssoAttributes.items():
             if not appyName: continue
             # Get the name of the HTTP header corresponding to "keyAttr"
             keyName = getattr(self, keyAttr)
             if not keyName: continue
             # Get the value for this header if found in the request
             value = headers.get('HTTP_%s' % keyName, None)
             if value:
@@ -354,15 +354,15 @@
 
     def updateUser(self, tool, req, user):
         '''Updates the local p_user with data from request headers'''
         # The last sync date for this user is now
         user.syncDate = DateTime()
         # Update basic user attributes and recompute the user title
         params, roles, groups = self.extractUserInfo(req)
-        for name, value in params.iteritems(): setattr(user, name, value)
+        for name, value in params.items(): setattr(user, name, value)
         user.updateTitle()
         # Update global roles (when roles are provided by the SSO server)
         if self.roleKey:
             existing = user.roles
             # Remove roles not granted anymore
             for role in existing:
                 if not roles or (role not in roles): user.delRole(role)
```

### Comparing `appy-1.0.8/py3/appy/server/static.py` & `appy-1.0.9/py3/appy/server/static.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         # new version, ready to be deployed. That way, you will avoid helpdesk
         # calls, during which you'll have to repeat the old same "Please reload
         # the pages with CTRL-F5" sentence (or, for Mac users: "Take a breath,
         # try to identify and hit, at the same time, keys ⌘+⌥+R+😩").
         #
         # Keys must correspond to file names, not prefixed with any path-related
         # info.
-        self.versions = {'appy.css':2, 'appy.js':3}
+        self.versions = {'appy.css':3, 'appy.js':4}
 
     def check(self):
         '''Checks that every entry in p_self.map is valid'''
         for key, path in self.map.items():
             # Paths must be pathlib.Path instances
             if not isinstance(path, pathlib.Path):
                 raise Exception(MAP_VALUE_NOT_PATH)
```

### Comparing `appy-1.0.8/py3/appy/server/traversal.py` & `appy-1.0.9/py3/appy/server/traversal.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from persistent import Persistent
 
 from appy.px import Px
 from appy.ui.js import Quote
 from appy.model.base import Base
 from appy.model.fields import Field
 from appy.server.request import Request
+from appy.xml.marshaller import Marshaller
 from appy.model.workflow.transition import Transition
 
 # Errors - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 UNTRAVERSABLE = 'Untraversable element "%s" while traversing %s.'
 TRAVERSE_UNKNOWN = 'Unknown traversal type "%s".'
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
@@ -73,14 +74,15 @@
         if other:
             self.init(other)
             self.parent = other
             return
         # Perform standard initialisation
         self.handler = handler
         self.req = handler.req
+        self.tool = handler.tool
         # The path that will be traversed, splitted into parts
         self.parts = handler.parts
         # The currently logged user
         self.user = handler.guard.user
         # The current result of traversing
         self.r = None
         # The last encountered object
@@ -129,15 +131,15 @@
         '''Tries to get an object from "part" which is a part of the URL path'''
         if part:
             id = self.asObjectId(part)
             r = self.handler.server.database.getObject(self.handler, id)
             if not r: raise NotFound(self.getPath())
         else:
             # If "part" is empty, (path is "/"), use the tool as default object
-            r = self.handler.tool
+            r = self.tool
         # Check if the user is allowed to consult this object
         self.handler.guard.allows(r, raiseError=True)
         return r
 
     def getSpecialObject(self, name):
         '''Gets the special object named p_name'''
         # Currenly, the only type of supported "special object" is an app class
@@ -198,15 +200,15 @@
 
     def getTraversalInfo(self, previous, name, current):
         '''Get traversal info about p_previous.<p_name> = p_current'''
         # Do we have traversal information ? p_previous can be an object, a
         # field, a module...
         traverse = getattr(previous, 'traverse', None)
         # Is p_name mentioned in the traversal info ?
-        if traverse and (name in traverse):
+        if traverse and name in traverse:
             # Yes: retrieve "traverse info" from it
             r = traverse[name]
         else:
             # No: determine default "traverse info" based on p_current's type
             if isinstance(current, Field):
                 if self.mode == Traversal.STANDARD:
                     # One may traverse it if he has the read permission on the
@@ -226,27 +228,27 @@
                 # Any other element (method, attribute, property...) is not
                 # traversable by default.
                 r = False
         # If we are walking an element of a Field in static mode, and this
         # element is protected by an instance-related info (=a permission),
         # convert this info to True: indeed, in that case, permission can't be
         # checked (we have no instance).
-        if (self.mode == Traversal.STATIC) and isinstance(previous, Field) and \
+        if self.mode == Traversal.STATIC and isinstance(previous, Field) and \
            isinstance(r, str) and r.startswith('perm:'):
             r = True
         return r
 
     def executeMethod(self, method):
         '''Execute m_method and return the result. The args potentially given to
            the method may vary.'''
         if hasattr(method, '__self__'):
             # We have a bound method. If the last walked object is not the bound
             # object, give the last walked object as unique arg.
             o = self.o
-            if o and (method.__self__ != o):
+            if o and method.__self__ != o:
                 r = method(o)
             else:
                 r = method()
         else:
             r = method(self.o or self.handler)
         return r
 
@@ -356,17 +358,25 @@
                 part = parts[i]
                 if part and part.startswith('@'):
                     # Manage direct navigation to a special object
                     self.r = self.getSpecialObject(part[1:])
                     # Switch to "static" mode
                     self.mode = Traversal.STATIC
                 elif self.r is None:
-                    # If we are at the start of the traversal, and "r" is still
-                    # None, "part" must correspond to an object ID.
-                    self.r = self.o = self.getObject(part)
+                    # We are at the start of a traversal. p_self.r is still
+                    # None: v_part must either be a traverser, or correspond to
+                    # an object ID.
+                    expr = self.handler.config.server.traversers.get(part)
+                    if expr:
+                        tool = self.tool
+                        self.o = tool
+                        self.r = eval(expr)
+                    else:
+                        # v_part must be an object ID
+                        self.r = self.o = self.getObject(part)
                 # Manage any not-empty part
                 elif part:
                     # Try to get the attribute or method named "part" on self.r
                     self.r = self.getPart(part)
                     # Manage this part
                     self.managePart(previous, part, self.r)
                 i += 1
@@ -374,10 +384,14 @@
         # If self.r is an object, call the default PX on it
         if isinstance(self.r, Persistent):
             self.managePart(self.r, 'default', self.r.default)
         # If the result of the traversal is not a string, it is invalid. Produce
         # a 404 error in that case.
         r = self.r
         if r is not None and not isinstance(r, str):
-            raise NotFound(self.getPath())
+            # Can v_r be marshalled ? Currently, only XML marshalling is there
+            if self.handler.resp.contentType == 'xml':
+                r = Marshaller(rootTag=self.parts[-1]).marshall(r)
+            else:
+                raise NotFound(self.getPath())
         return r
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
```

### Comparing `appy-1.0.8/py3/appy/test/__init__.py` & `appy-1.0.9/py3/appy/test/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/test/integration.py` & `appy-1.0.9/py3/appy/test/integration.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/test/monitoring.py` & `appy-1.0.9/py3/appy/test/monitoring.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/test/performance.py` & `appy-1.0.9/py3/appy/test/performance.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/tr/__init__.py` & `appy-1.0.9/py3/appy/tr/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/tr/po/Appy.pot` & `appy-1.0.9/py3/appy/tr/po/Appy.pot`

 * *Files 2% similar despite different names*

```diff
@@ -271,14 +271,18 @@
 msgid "object_delete"
 msgstr ""
 
 #. Default: "Delete selection"
 msgid "object_delete_many"
 msgstr ""
 
+#. Default: "The element has been deleted."
+msgid "object_deleted"
+msgstr ""
+
 #. Default: "Remove"
 msgid "object_unlink"
 msgstr ""
 
 #. Default: "Remove selection"
 msgid "object_unlink_many"
 msgstr ""
@@ -335,14 +339,18 @@
 msgid "action_partial"
 msgstr ""
 
 #. Default: "Action had no effect."
 msgid "action_null"
 msgstr ""
 
+#. Default: "Action would have had no effect."
+msgid "action_null_test"
+msgstr ""
+
 #. Default: "This action can't currently be executed."
 msgid "action_unexecutable"
 msgstr ""
 
 #. Default: "Are you sure you want to apply this change?"
 msgid "save_confirm"
 msgstr ""
@@ -1724,14 +1732,18 @@
 msgid "Tool_defaultPage"
 msgstr ""
 
 #. Default: "The page defined here will be selected as home page."
 msgid "Tool_defaultPage_descr"
 msgstr ""
 
+#. Default: "Update URLs"
+msgid "Tool_updateBaseUrl"
+msgstr ""
+
 #. Default: "Carousels"
 msgid "Tool_page_carousels"
 msgstr ""
 
 #. Default: "Carousels"
 msgid "Tool_carousels"
 msgstr ""
@@ -1756,14 +1768,51 @@
 msgid "Tool_calendar"
 msgstr ""
 
 #. Default: " "
 msgid "Tool_calendar_descr"
 msgstr ""
 
+# ~~~~ Move-related labels ~~~~
+#. Default: "Mover"
+msgid "Mover"
+msgstr ""
+
+#. Default: "Current base URL"
+msgid "Mover_currentBase"
+msgstr ""
+
+#. Default: "Encode here the prefix of the URLs that can currently be found in web pages, to refer to any internal content: link to another page, image, or any other object."
+msgid "Mover_currentBase_descr"
+msgstr ""
+
+#. Default: "New base URL"
+msgid "Mover_newBase"
+msgstr ""
+
+#. Default: "Encode here the prefix that will replace the one you encoded in the hereabove field. Take care of to start both prefixes with the correct protocol: <b>http</b> or <b>https</b>."
+msgid "Mover_newBase_descr"
+msgstr ""
+
+#. Default: "Test mode ?"
+msgid "Mover_dryRun"
+msgstr ""
+
+#. Default: "If this checkbbox is checked, nothing will be actually performed, but a message will tell you what could have happened."
+msgid "Mover_dryRun_descr"
+msgstr ""
+
+#. Default: "${replacements} replacement·s done within ${updated}/${total} page·s."
+msgid "Mover_done"
+msgstr ""
+
+#. Default: "${replacements} replacement·s would have been done within ${updated}/${total} page·s."
+msgid "Mover_tested"
+msgstr ""
+
 # ~~~~ Standard workflow-related labels ~~~~
 #. Default: "Active"
 msgid "Anonymous_active"
 msgstr ""
 
 #. Default: "Active"
 msgid "Authenticated_active"
```

### Comparing `appy-1.0.8/py3/appy/tr/po/__init__.py` & `appy-1.0.9/py3/appy/tr/po/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/tr/po/ar.po` & `appy-1.0.9/py3/appy/tr/po/ar.po`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,18 @@
 msgid "object_delete"
 msgstr ""
 
 #. Default: "Delete selection"
 msgid "object_delete_many"
 msgstr ""
 
+#. Default: "The element has been deleted."
+msgid "object_deleted"
+msgstr ""
+
 #. Default: "Remove"
 msgid "object_unlink"
 msgstr ""
 
 #. Default: "Remove selection"
 msgid "object_unlink_many"
 msgstr ""
@@ -335,14 +339,18 @@
 msgid "action_partial"
 msgstr ""
 
 #. Default: "Action had no effect."
 msgid "action_null"
 msgstr ""
 
+#. Default: "Action would have had no effect."
+msgid "action_null_test"
+msgstr ""
+
 #. Default: "This action can't currently be executed."
 msgid "action_unexecutable"
 msgstr ""
 
 #. Default: "Are you sure you want to apply this change?"
 msgid "save_confirm"
 msgstr ""
@@ -1724,14 +1732,18 @@
 msgid "Tool_defaultPage"
 msgstr ""
 
 #. Default: "The page defined here will be selected as home page."
 msgid "Tool_defaultPage_descr"
 msgstr ""
 
+#. Default: "Update URLs"
+msgid "Tool_updateBaseUrl"
+msgstr ""
+
 #. Default: "Carousels"
 msgid "Tool_page_carousels"
 msgstr ""
 
 #. Default: "Carousels"
 msgid "Tool_carousels"
 msgstr ""
@@ -1756,14 +1768,51 @@
 msgid "Tool_calendar"
 msgstr ""
 
 #. Default: " "
 msgid "Tool_calendar_descr"
 msgstr ""
 
+# ~~~~ Move-related labels ~~~~
+#. Default: "Mover"
+msgid "Mover"
+msgstr ""
+
+#. Default: "Current base URL"
+msgid "Mover_currentBase"
+msgstr ""
+
+#. Default: "Encode here the prefix of the URLs that can currently be found in web pages, to refer to any internal content: link to another page, image, or any other object."
+msgid "Mover_currentBase_descr"
+msgstr ""
+
+#. Default: "New base URL"
+msgid "Mover_newBase"
+msgstr ""
+
+#. Default: "Encode here the prefix that will replace the one you encoded in the hereabove field. Take care of to start both prefixes with the correct protocol: <b>http</b> or <b>https</b>."
+msgid "Mover_newBase_descr"
+msgstr ""
+
+#. Default: "Test mode ?"
+msgid "Mover_dryRun"
+msgstr ""
+
+#. Default: "If this checkbbox is checked, nothing will be actually performed, but a message will tell you what could have happened."
+msgid "Mover_dryRun_descr"
+msgstr ""
+
+#. Default: "${replacements} replacement·s done within ${updated}/${total} page·s."
+msgid "Mover_done"
+msgstr ""
+
+#. Default: "${replacements} replacement·s would have been done within ${updated}/${total} page·s."
+msgid "Mover_tested"
+msgstr ""
+
 # ~~~~ Standard workflow-related labels ~~~~
 #. Default: "Active"
 msgid "Anonymous_active"
 msgstr ""
 
 #. Default: "Active"
 msgid "Authenticated_active"
```

### Comparing `appy-1.0.8/py3/appy/tr/po/de.po` & `appy-1.0.9/py3/appy/tr/po/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -271,14 +271,18 @@
 msgid "object_delete"
 msgstr "Löschen"
 
 #. Default: "Delete selection"
 msgid "object_delete_many"
 msgstr ""
 
+#. Default: "The element has been deleted."
+msgid "object_deleted"
+msgstr ""
+
 #. Default: "Remove"
 msgid "object_unlink"
 msgstr "Zurückziehen"
 
 #. Default: "Remove selection"
 msgid "object_unlink_many"
 msgstr ""
@@ -335,14 +339,18 @@
 msgid "action_partial"
 msgstr ""
 
 #. Default: "Action had no effect."
 msgid "action_null"
 msgstr ""
 
+#. Default: "Action would have had no effect."
+msgid "action_null_test"
+msgstr ""
+
 #. Default: "This action can't currently be executed."
 msgid "action_unexecutable"
 msgstr ""
 
 #. Default: "Are you sure you want to apply this change?"
 msgid "save_confirm"
 msgstr ""
@@ -1724,14 +1732,18 @@
 msgid "Tool_defaultPage"
 msgstr ""
 
 #. Default: "The page defined here will be selected as home page."
 msgid "Tool_defaultPage_descr"
 msgstr ""
 
+#. Default: "Update URLs"
+msgid "Tool_updateBaseUrl"
+msgstr ""
+
 #. Default: "Carousels"
 msgid "Tool_page_carousels"
 msgstr ""
 
 #. Default: "Carousels"
 msgid "Tool_carousels"
 msgstr ""
@@ -1756,14 +1768,51 @@
 msgid "Tool_calendar"
 msgstr ""
 
 #. Default: " "
 msgid "Tool_calendar_descr"
 msgstr ""
 
+# ~~~~ Move-related labels ~~~~
+#. Default: "Mover"
+msgid "Mover"
+msgstr ""
+
+#. Default: "Current base URL"
+msgid "Mover_currentBase"
+msgstr ""
+
+#. Default: "Encode here the prefix of the URLs that can currently be found in web pages, to refer to any internal content: link to another page, image, or any other object."
+msgid "Mover_currentBase_descr"
+msgstr ""
+
+#. Default: "New base URL"
+msgid "Mover_newBase"
+msgstr ""
+
+#. Default: "Encode here the prefix that will replace the one you encoded in the hereabove field. Take care of to start both prefixes with the correct protocol: <b>http</b> or <b>https</b>."
+msgid "Mover_newBase_descr"
+msgstr ""
+
+#. Default: "Test mode ?"
+msgid "Mover_dryRun"
+msgstr ""
+
+#. Default: "If this checkbbox is checked, nothing will be actually performed, but a message will tell you what could have happened."
+msgid "Mover_dryRun_descr"
+msgstr ""
+
+#. Default: "${replacements} replacement·s done within ${updated}/${total} page·s."
+msgid "Mover_done"
+msgstr ""
+
+#. Default: "${replacements} replacement·s would have been done within ${updated}/${total} page·s."
+msgid "Mover_tested"
+msgstr ""
+
 # ~~~~ Standard workflow-related labels ~~~~
 #. Default: "Active"
 msgid "Anonymous_active"
 msgstr ""
 
 #. Default: "Active"
 msgid "Authenticated_active"
```

### Comparing `appy-1.0.8/py3/appy/tr/po/en.po` & `appy-1.0.9/py3/appy/tr/po/en.po`

 * *Files 2% similar despite different names*

```diff
@@ -272,14 +272,18 @@
 msgid "object_delete"
 msgstr "Delete"
 
 #. Default: "Delete selection"
 msgid "object_delete_many"
 msgstr "Delete selection"
 
+#. Default: "The element has been deleted."
+msgid "object_deleted"
+msgstr "The element has been deleted."
+
 #. Default: "Remove"
 msgid "object_unlink"
 msgstr "Unlink"
 
 #. Default: "Remove selection"
 msgid "object_unlink_many"
 msgstr "Remove selection"
@@ -336,14 +340,18 @@
 msgid "action_partial"
 msgstr "Action could not be performed on ${nb} element(s)."
 
 #. Default: "Action had no effect."
 msgid "action_null"
 msgstr "Action had no effect."
 
+#. Default: "Action would have had no effect."
+msgid "action_null_test"
+msgstr "Action would have had no effect."
+
 #. Default: "This action can't currently be executed."
 msgid "action_unexecutable"
 msgstr "This action can't currently be executed."
 
 #. Default: "Are you sure you want to apply this change?"
 msgid "save_confirm"
 msgstr "Are you sure you want to apply this change?"
@@ -1725,14 +1733,18 @@
 msgid "Tool_defaultPage"
 msgstr "Default page"
 
 #. Default: "The page defined here will be selected as home page."
 msgid "Tool_defaultPage_descr"
 msgstr "The page defined here will be selected as home page."
 
+#. Default: "Update URLs"
+msgid "Tool_updateBaseUrl"
+msgstr "Update URLs"
+
 #. Default: "Carousels"
 msgid "Tool_page_carousels"
 msgstr "Carousels"
 
 #. Default: "Carousels"
 msgid "Tool_carousels"
 msgstr "Carousels"
@@ -1757,14 +1769,51 @@
 msgid "Tool_calendar"
 msgstr "Calendar"
 
 #. Default: " "
 msgid "Tool_calendar_descr"
 msgstr " "
 
+# ~~~~ Move-related labels ~~~~
+#. Default: "Mover"
+msgid "Mover"
+msgstr "Mover"
+
+#. Default: "Current base URL"
+msgid "Mover_currentBase"
+msgstr "Current base URL"
+
+#. Default: "Encode here the prefix of the URLs that can currently be found in web pages, to refer to any internal content: link to another page, image, or any other object."
+msgid "Mover_currentBase_descr"
+msgstr "Encode here the prefix of the URLs that can currently be found in web pages, to refer to any internal content: link to another page, image, or any other object."
+
+#. Default: "New base URL"
+msgid "Mover_newBase"
+msgstr "New base URL"
+
+#. Default: "Encode here the prefix that will replace the one you encoded in the hereabove field. Take care of to start both prefixes with the correct protocol: <b>http</b> or <b>https</b>."
+msgid "Mover_newBase_descr"
+msgstr "Encode here the prefix that will replace the one you encoded in the hereabove field. Take care of to start both prefixes with the correct protocol: <b>http</b> or <b>https</b>."
+
+#. Default: "Test mode ?"
+msgid "Mover_dryRun"
+msgstr "Test mode ?"
+
+#. Default: "If this checkbbox is checked, nothing will be actually performed, but a message will tell you what could have happened."
+msgid "Mover_dryRun_descr"
+msgstr "If this checkbbox is checked, nothing will be actually performed, but a message will tell you what could have happened."
+
+#. Default: "${replacements} replacement·s done within ${updated}/${total} page·s."
+msgid "Mover_done"
+msgstr "${replacements} done within ${updated}/${total} page·s."
+
+#. Default: "${replacements} replacement·s would have been done within ${updated}/${total} page·s."
+msgid "Mover_tested"
+msgstr "${replacements} replacement·s would have been done within ${updated}/${total} page·s."
+
 # ~~~~ Standard workflow-related labels ~~~~
 #. Default: "Active"
 msgid "Anonymous_active"
 msgstr "Active"
 
 #. Default: "Active"
 msgid "Authenticated_active"
```

### Comparing `appy-1.0.8/py3/appy/tr/po/es.po` & `appy-1.0.9/py3/appy/tr/po/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -271,14 +271,18 @@
 msgid "object_delete"
 msgstr "Eliminar"
 
 #. Default: "Delete selection"
 msgid "object_delete_many"
 msgstr ""
 
+#. Default: "The element has been deleted."
+msgid "object_deleted"
+msgstr ""
+
 #. Default: "Remove"
 msgid "object_unlink"
 msgstr ""
 
 #. Default: "Remove selection"
 msgid "object_unlink_many"
 msgstr ""
@@ -335,14 +339,18 @@
 msgid "action_partial"
 msgstr ""
 
 #. Default: "Action had no effect."
 msgid "action_null"
 msgstr ""
 
+#. Default: "Action would have had no effect."
+msgid "action_null_test"
+msgstr ""
+
 #. Default: "This action can't currently be executed."
 msgid "action_unexecutable"
 msgstr ""
 
 #. Default: "Are you sure you want to apply this change?"
 msgid "save_confirm"
 msgstr ""
@@ -1724,14 +1732,18 @@
 msgid "Tool_defaultPage"
 msgstr ""
 
 #. Default: "The page defined here will be selected as home page."
 msgid "Tool_defaultPage_descr"
 msgstr ""
 
+#. Default: "Update URLs"
+msgid "Tool_updateBaseUrl"
+msgstr ""
+
 #. Default: "Carousels"
 msgid "Tool_page_carousels"
 msgstr ""
 
 #. Default: "Carousels"
 msgid "Tool_carousels"
 msgstr ""
@@ -1756,14 +1768,51 @@
 msgid "Tool_calendar"
 msgstr ""
 
 #. Default: " "
 msgid "Tool_calendar_descr"
 msgstr ""
 
+# ~~~~ Move-related labels ~~~~
+#. Default: "Mover"
+msgid "Mover"
+msgstr ""
+
+#. Default: "Current base URL"
+msgid "Mover_currentBase"
+msgstr ""
+
+#. Default: "Encode here the prefix of the URLs that can currently be found in web pages, to refer to any internal content: link to another page, image, or any other object."
+msgid "Mover_currentBase_descr"
+msgstr ""
+
+#. Default: "New base URL"
+msgid "Mover_newBase"
+msgstr ""
+
+#. Default: "Encode here the prefix that will replace the one you encoded in the hereabove field. Take care of to start both prefixes with the correct protocol: <b>http</b> or <b>https</b>."
+msgid "Mover_newBase_descr"
+msgstr ""
+
+#. Default: "Test mode ?"
+msgid "Mover_dryRun"
+msgstr ""
+
+#. Default: "If this checkbbox is checked, nothing will be actually performed, but a message will tell you what could have happened."
+msgid "Mover_dryRun_descr"
+msgstr ""
+
+#. Default: "${replacements} replacement·s done within ${updated}/${total} page·s."
+msgid "Mover_done"
+msgstr ""
+
+#. Default: "${replacements} replacement·s would have been done within ${updated}/${total} page·s."
+msgid "Mover_tested"
+msgstr ""
+
 # ~~~~ Standard workflow-related labels ~~~~
 #. Default: "Active"
 msgid "Anonymous_active"
 msgstr ""
 
 #. Default: "Active"
 msgid "Authenticated_active"
```

### Comparing `appy-1.0.8/py3/appy/tr/po/fr.po` & `appy-1.0.9/py3/appy/tr/po/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -272,14 +272,18 @@
 msgid "object_delete"
 msgstr "Supprimer"
 
 #. Default: "Delete selection"
 msgid "object_delete_many"
 msgstr "Supprimer la sélection"
 
+#. Default: "The element has been deleted."
+msgid "object_deleted"
+msgstr "L'élément a été supprimé."
+
 #. Default: "Remove"
 msgid "object_unlink"
 msgstr "Retirer"
 
 #. Default: "Remove selection"
 msgid "object_unlink_many"
 msgstr "Retirer la sélection"
@@ -336,14 +340,18 @@
 msgid "action_partial"
 msgstr "L'action n'a pu être réalisée pour ${nb} élément(s)."
 
 #. Default: "Action had no effect."
 msgid "action_null"
 msgstr "L'action n'a eu aucun effet."
 
+#. Default: "Action would have had no effect."
+msgid "action_null_test"
+msgstr "L'action n'aurait eu aucun effet."
+
 #. Default: "This action can't currently be executed."
 msgid "action_unexecutable"
 msgstr "Cette action ne peut actuellement pas être exécutée."
 
 #. Default: "Are you sure you want to apply this change?"
 msgid "save_confirm"
 msgstr "Êtes-vous sûr de vouloir appliquer ce changement?"
@@ -1035,15 +1043,15 @@
 
 #. Default: "On"
 msgid "Base_created"
 msgstr "Le"
 
 #. Default: "Last updated on"
 msgid "Base_modified"
-msgstr "Dernière modification le"
+msgstr "Modifié·e le"
 
 #. Default: "State"
 msgid "Base_state"
 msgstr "État"
 
 #. Default: "Keywords"
 msgid "Base_searchable"
@@ -1725,14 +1733,18 @@
 msgid "Tool_defaultPage"
 msgstr "Page par défaut"
 
 #. Default: "The page defined here will be selected as home page."
 msgid "Tool_defaultPage_descr"
 msgstr "La page choisie ici sera utilisée comme page d'accueil du site."
 
+#. Default: "Update URLs"
+msgid "Tool_updateBaseUrl"
+msgstr "Changer les URLs"
+
 #. Default: "Carousels"
 msgid "Tool_page_carousels"
 msgstr "Carrousels"
 
 #. Default: "Carousels"
 msgid "Tool_carousels"
 msgstr "Carrousels"
@@ -1757,14 +1769,51 @@
 msgid "Tool_calendar"
 msgstr "Calendrier"
 
 #. Default: " "
 msgid "Tool_calendar_descr"
 msgstr " "
 
+# ~~~~ Move-related labels ~~~~
+#. Default: "Mover"
+msgid "Mover"
+msgstr "Déménageur"
+
+#. Default: "Current base URL"
+msgid "Mover_currentBase"
+msgstr "URL de base actuelle"
+
+#. Default: "Encode here the prefix of the URLs that can currently be found in web pages, to refer to any internal content: link to another page, image, or any other object."
+msgid "Mover_currentBase_descr"
+msgstr "Encodez ici le préfixe des URLs qui peuvent actuellement être trouvées dans vos pages web, et qui pointent vers tout contenu interne: autres pages, images ou tout autre objet."
+
+#. Default: "New base URL"
+msgid "Mover_newBase"
+msgstr "Nouvelle URL de base"
+
+#. Default: "Encode here the prefix that will replace the one you encoded in the hereabove field. Take care of to start both prefixes with the correct protocol: <b>http</b> or <b>https</b>."
+msgid "Mover_newBase_descr"
+msgstr "Encodez ici le préfixe qui remplacera celui que vous avez spécifié dans le champ précédent. Attention à entamer chaque préfixe par le procotole correct: <b>http</b> ou <b>https</b>."
+
+#. Default: "Test mode ?"
+msgid "Mover_dryRun"
+msgstr "Mode test ?"
+
+#. Default: "If this checkbbox is checked, nothing will be actually performed, but a message will tell you what could have happened."
+msgid "Mover_dryRun_descr"
+msgstr "Si cette case est cochée, rien ne se produira réellement, mais un message vous indiquera ce qui se serait produit."
+
+#. Default: "${replacements} replacement·s done within ${updated}/${total} page·s."
+msgid "Mover_done"
+msgstr "${replacements} remplacement·s fait·s dans ${updated}/${total} page·s."
+
+#. Default: "${replacements} replacement·s would have been done within ${updated}/${total} page·s."
+msgid "Mover_tested"
+msgstr "${replacements} remplacement·s aurai·en·t été fait·s dans ${updated}/${total} page·s."
+
 # ~~~~ Standard workflow-related labels ~~~~
 #. Default: "Active"
 msgid "Anonymous_active"
 msgstr "Actif∙ve"
 
 #. Default: "Active"
 msgid "Authenticated_active"
```

### Comparing `appy-1.0.8/py3/appy/tr/po/it.po` & `appy-1.0.9/py3/appy/tr/po/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,18 @@
 msgid "object_delete"
 msgstr "Elimina"
 
 #. Default: "Delete selection"
 msgid "object_delete_many"
 msgstr ""
 
+#. Default: "The element has been deleted."
+msgid "object_deleted"
+msgstr ""
+
 #. Default: "Remove"
 msgid "object_unlink"
 msgstr ""
 
 #. Default: "Remove selection"
 msgid "object_unlink_many"
 msgstr ""
@@ -335,14 +339,18 @@
 msgid "action_partial"
 msgstr ""
 
 #. Default: "Action had no effect."
 msgid "action_null"
 msgstr ""
 
+#. Default: "Action would have had no effect."
+msgid "action_null_test"
+msgstr ""
+
 #. Default: "This action can't currently be executed."
 msgid "action_unexecutable"
 msgstr ""
 
 #. Default: "Are you sure you want to apply this change?"
 msgid "save_confirm"
 msgstr ""
@@ -1724,14 +1732,18 @@
 msgid "Tool_defaultPage"
 msgstr ""
 
 #. Default: "The page defined here will be selected as home page."
 msgid "Tool_defaultPage_descr"
 msgstr ""
 
+#. Default: "Update URLs"
+msgid "Tool_updateBaseUrl"
+msgstr ""
+
 #. Default: "Carousels"
 msgid "Tool_page_carousels"
 msgstr ""
 
 #. Default: "Carousels"
 msgid "Tool_carousels"
 msgstr ""
@@ -1756,14 +1768,51 @@
 msgid "Tool_calendar"
 msgstr ""
 
 #. Default: " "
 msgid "Tool_calendar_descr"
 msgstr ""
 
+# ~~~~ Move-related labels ~~~~
+#. Default: "Mover"
+msgid "Mover"
+msgstr ""
+
+#. Default: "Current base URL"
+msgid "Mover_currentBase"
+msgstr ""
+
+#. Default: "Encode here the prefix of the URLs that can currently be found in web pages, to refer to any internal content: link to another page, image, or any other object."
+msgid "Mover_currentBase_descr"
+msgstr ""
+
+#. Default: "New base URL"
+msgid "Mover_newBase"
+msgstr ""
+
+#. Default: "Encode here the prefix that will replace the one you encoded in the hereabove field. Take care of to start both prefixes with the correct protocol: <b>http</b> or <b>https</b>."
+msgid "Mover_newBase_descr"
+msgstr ""
+
+#. Default: "Test mode ?"
+msgid "Mover_dryRun"
+msgstr ""
+
+#. Default: "If this checkbbox is checked, nothing will be actually performed, but a message will tell you what could have happened."
+msgid "Mover_dryRun_descr"
+msgstr ""
+
+#. Default: "${replacements} replacement·s done within ${updated}/${total} page·s."
+msgid "Mover_done"
+msgstr ""
+
+#. Default: "${replacements} replacement·s would have been done within ${updated}/${total} page·s."
+msgid "Mover_tested"
+msgstr ""
+
 # ~~~~ Standard workflow-related labels ~~~~
 #. Default: "Active"
 msgid "Anonymous_active"
 msgstr ""
 
 #. Default: "Active"
 msgid "Authenticated_active"
```

### Comparing `appy-1.0.8/py3/appy/tr/po/nl.po` & `appy-1.0.9/py3/appy/tr/po/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -271,14 +271,18 @@
 msgid "object_delete"
 msgstr "Verwijderen"
 
 #. Default: "Delete selection"
 msgid "object_delete_many"
 msgstr "Verwijder de selectie"
 
+#. Default: "The element has been deleted."
+msgid "object_deleted"
+msgstr ""
+
 #. Default: "Remove"
 msgid "object_unlink"
 msgstr "Intrekken"
 
 #. Default: "Remove selection"
 msgid "object_unlink_many"
 msgstr "Selectie losmaken"
@@ -335,14 +339,18 @@
 msgid "action_partial"
 msgstr "De actie kon niet uitgevoerd worden op ${nb} element(en)."
 
 #. Default: "Action had no effect."
 msgid "action_null"
 msgstr "De actie heeft geen effect gehad."
 
+#. Default: "Action would have had no effect."
+msgid "action_null_test"
+msgstr ""
+
 #. Default: "This action can't currently be executed."
 msgid "action_unexecutable"
 msgstr "Deze actie kan momenteel niet worden uitgevoerd."
 
 #. Default: "Are you sure you want to apply this change?"
 msgid "save_confirm"
 msgstr "Bent u zeker om deze wijziging door te voeren?"
@@ -1724,14 +1732,18 @@
 msgid "Tool_defaultPage"
 msgstr ""
 
 #. Default: "The page defined here will be selected as home page."
 msgid "Tool_defaultPage_descr"
 msgstr ""
 
+#. Default: "Update URLs"
+msgid "Tool_updateBaseUrl"
+msgstr ""
+
 #. Default: "Carousels"
 msgid "Tool_page_carousels"
 msgstr ""
 
 #. Default: "Carousels"
 msgid "Tool_carousels"
 msgstr ""
@@ -1756,14 +1768,51 @@
 msgid "Tool_calendar"
 msgstr ""
 
 #. Default: " "
 msgid "Tool_calendar_descr"
 msgstr ""
 
+# ~~~~ Move-related labels ~~~~
+#. Default: "Mover"
+msgid "Mover"
+msgstr ""
+
+#. Default: "Current base URL"
+msgid "Mover_currentBase"
+msgstr ""
+
+#. Default: "Encode here the prefix of the URLs that can currently be found in web pages, to refer to any internal content: link to another page, image, or any other object."
+msgid "Mover_currentBase_descr"
+msgstr ""
+
+#. Default: "New base URL"
+msgid "Mover_newBase"
+msgstr ""
+
+#. Default: "Encode here the prefix that will replace the one you encoded in the hereabove field. Take care of to start both prefixes with the correct protocol: <b>http</b> or <b>https</b>."
+msgid "Mover_newBase_descr"
+msgstr ""
+
+#. Default: "Test mode ?"
+msgid "Mover_dryRun"
+msgstr ""
+
+#. Default: "If this checkbbox is checked, nothing will be actually performed, but a message will tell you what could have happened."
+msgid "Mover_dryRun_descr"
+msgstr ""
+
+#. Default: "${replacements} replacement·s done within ${updated}/${total} page·s."
+msgid "Mover_done"
+msgstr ""
+
+#. Default: "${replacements} replacement·s would have been done within ${updated}/${total} page·s."
+msgid "Mover_tested"
+msgstr ""
+
 # ~~~~ Standard workflow-related labels ~~~~
 #. Default: "Active"
 msgid "Anonymous_active"
 msgstr "Actief"
 
 #. Default: "Active"
 msgid "Authenticated_active"
```

### Comparing `appy-1.0.8/py3/appy/tr/updater.py` & `appy-1.0.9/py3/appy/tr/updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self.model = updater.model
         # Build a dict mapping workflow prefixes in use in Appy 0.9 and
         # workflow names.
         r = {}
         for workflow in self.model.workflows.values():
             # This prefix was used, in Appy 0.9, for all i18n messages related
             # to this workflow.
-            moduleName = workflow.python.__module__.split('.')[0]
+            moduleName = workflow.python.__module__.split('.')[-1]
             oldPrefix = '%s_%s_%s_' % (self.appName, moduleName, workflow.name)
             r[oldPrefix.lower()] = '%s_' % workflow.name
         self.workflowNames = r
 
     def removeSearchPart(self, id):
         '''With Appy 0.9, label parts contained some part named "search".
            With Appy 1.0, it is not the case anymore.'''
@@ -233,15 +233,17 @@
         '''Generate Ref-specific labels'''
         # Add the label for the confirm message when relevant
         if field.addConfirm:
             self.addLabel('%s_addConfirm' % label, self.CONFIRM, nice=False)
 
     def visitList(self, class_, field, label):
         '''Generate List-specific labels'''
-        # Generate labels for sub-fields
+        # Generate labels for sub-fields, excepted if they are dynamically
+        # computed.
+        if callable(field.fields): return
         walkedGroups = set()
         for name, sub in field.fields:
             if not self.mustGenerateLabels(sub): continue
             # We set "forceLabel" to True because we need a label to dump for
             # every sub-field, within List' column headers.
             subLabel = '%s_%s' % (label, name)
             self.visitField(class_, sub, subLabel, walkedGroups,forceLabel=True)
@@ -305,16 +307,16 @@
 
     def visitClass(self, name, class_):
         '''Produce labels for a p_class_'''
         # Produce base labels for the class name (singular and plural), but
         # only for not-over classes.
         if class_.type == 'app':
             # Class name, singular and plural
-            self.addLabel(name, name, nice=False)
-            self.addLabel('%s_plural' % name, name + 's', nice=False)
+            self.addLabel(name, name)
+            self.addLabel('%s_plural' % name, name + 's')
         # While walking fields and searches, groups will be encountered. In
         # order to avoid generating labels several times for the same group,
         # remember the already walked groups.
         walkedGroups = set()
         # Produce labels for every search defined on this p_class_
         for search in class_.searches.values():
             self.visitSearch(class_, search, walkedGroups)
@@ -340,15 +342,15 @@
         add = self.addLabel
         # Generate a label for every state and transition
         for attribute in workflow.attributes:
             for element in getattr(workflow, attribute).values():
                 label = '%s_%s' % (name, element.name)
                 add(label, element.name)
                 # Add a label for a transition that must be confirmed
-                if (attribute == 'transitions') and element.confirm:
+                if attribute == 'transitions' and element.confirm:
                     add('%s_confirm' % label, self.CONFIRM, nice=False)
 
     def collectLabels(self):
         '''Collect all labels by visiting model elements'''
         model = self.model
         # Add a label for every role
         for role in model.getRoles(base=None):
```

### Comparing `appy-1.0.8/py3/appy/ui/__init__.py` & `appy-1.0.9/py3/appy/ui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,21 +112,24 @@
         #         | each other.
         # ----------------------------------------------------------------------
         self.home = 'home'
 
         # The background images to use when the home page is "homes". Every
         # entry looks like:
         #
-        #            "<file_name>": ("<app_name>", "<image_width>")
+        #                "<file_name>": "<image_width>"
         #
         # Here is an example, for a triptych:
         #
-        #               {"bg1.jpg": ("MyApp", "30%"),
-        #                "bg2.jpg": ("MyApp", "40%"),
-        #                "bg3.jpg": ("MyApp", "30%")}
+        #                     {"bg1.jpg": "30%",
+        #                      "bg2.jpg": "40%",
+        #                      "bg3.jpg": "30%"}*
+        #
+        # As usual, if the background files originate from an alternate place
+        # (ie, an ext), also add them in dict images as defined hereabove.
         self.homesBackgrounds = {}
 
         # Attribute "headerBackground" determines properties for the header's
         # background image, as a tuple or list
         # 
         #                      (name, repetition, position)
         #
@@ -903,13 +906,13 @@
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 def getActionsCss(display):
     '''Gets the CSS class to apply to the zone rendering object actions, having
        the specified p_display.'''
     if display == 'block':
         r = 'objectActions'
+    elif display == 'right':
+        r = 'alignedActions'
     else:
         r = 'inline'
-        if display == 'right':
-            r += ' alignedActions'
     return r
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
```

### Comparing `appy-1.0.8/py3/appy/ui/account.py` & `appy-1.0.9/py3/appy/ui/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         self.columns = columns or Account.defaultColumns
         # This default unit, if present, will be shown for every entry for which
         # no unit is defined.
         self.defaultUnit = defaultUnit
 
     def addAmount(self, field=None, value=None, expression=None, label=None,
                   mapping=None, positive=True, style=None, unit=None,
-                  sep=False, fieldValue=None, cellTag='td'):
+                  sep=False, fieldValue=None, cellTag='td', context=None):
         '''Adds an entry of type "amount" in the account'''
 
         # ----------------------------------------------------------------------
         # The label and value of the amount to display can be determined by:
         # ----------------------------------------------------------------------
         # p_field      | it must be the name of a Float or Integer field whose
         #              | value will be retrieved on p_self.o, excepted if
@@ -145,18 +145,19 @@
         # p_value      | it must be a float or int value. in that case, an i18n
         #              | p_label must be present and will be used (with an
         #              | optional p_mapping) to determine the label for this
         #              | amount;
         # ----------------------------------------------------------------------
         # p_expression | it must be a string containing a Python expression that
         #              | will be evaluated with "o" in its context ("o" being
-        #              | p_self.o). The expression must return the float or int
-        #              | amount; in that case, similarly to the previous case,
-        #              | an i18n p_label must be present, with its optional
-        #              | p_mapping.
+        #              | p_self.o). p_context, if passed, can also be used in
+        #              | the expression. The expression must return the float or
+        #              | int amount ; in that case, similarly to the previous
+        #              | case, an i18n p_label must be present, with its
+        #              | optional p_mapping.
         # ----------------------------------------------------------------------
         # p_positive is False, the amount will be negated. A specific p_style
         # can be applied to the entry "b" (bold) or "i" (italic).
         o = self.o
         if expression:
             label = o.translate(label, mapping=mapping)
             value = eval(expression)
```

### Comparing `appy-1.0.8/py3/appy/ui/criteria.py` & `appy-1.0.9/py3/appy/ui/criteria.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/css.py` & `appy-1.0.9/py3/appy/ui/css.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/globals.py` & `appy-1.0.9/py3/appy/ui/globals.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/iframe.py` & `appy-1.0.9/py3/appy/ui/iframe.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/includer.py` & `appy-1.0.9/py3/appy/ui/includer.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/js.py` & `appy-1.0.9/py3/appy/ui/js.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/language.py` & `appy-1.0.9/py3/appy/ui/language.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/layout.py` & `appy-1.0.9/py3/appy/ui/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,14 +537,15 @@
 Layouts.dc  = Layouts(d + '|')
 Layouts.h   = Layouts('lhrv-f')
 Layouts.n   = Layouts.b
 Layouts.nd  = Layouts(Layout(d, width=None))
 Layouts.w   = Layouts(Layout(b))
 # Layouts with content only (no label)
 Layouts.f   = Layouts(Layout('f', width=None))
+Layouts.fr  = Layouts(Layout('frv', width=None))
 Layouts.wf  = Layouts(Layout('f'))
 Layouts.fv  = Layouts(edit=Layout(b), view=Layout('f'))
 Layouts.fvd = Layouts(edit=Layout(d), view=Layout('f'))
 Layouts.g   = Layouts('frvl')
 # The *d*escription is visible, even on the *v*iew layout
 Layouts.dv  = Layouts(edit=d, view='l-d-f')
 # The *d*escription is shown on the *v*iew layout but not on *e*dit (=*s*imple)
```

### Comparing `appy-1.0.8/py3/appy/ui/message.py` & `appy-1.0.9/py3/appy/ui/message.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/navigate.py` & `appy-1.0.9/py3/appy/ui/navigate.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 # Appy. If not, see <http://www.gnu.org/licenses/>.
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 from appy.px import Px
 from appy.model.batch import Batch
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
+WRONG_NAV  = 'Wrong nav key "%s".'
+
+#- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Sibling:
     '''Represents a sibling element, accessible via navigation from
        another one.'''
     # Existing types of siblings
     types = ('previous', 'next', 'first', 'last')
 
     # Names of icons corresponding to sibling types
@@ -174,16 +177,22 @@
         }''')
 
     @staticmethod
     def get(nav, tool, ctx):
         '''Analyse the navigation info p_nav and returns the corresponding
           concrete Siblings instance.'''
         elems = nav.split('.')
-        Siblings = (elems[0] == 'ref') and RefSiblings or SearchSiblings
-        return Siblings(tool, ctx, *elems[1:])
+        Siblings = RefSiblings if elems[0] == 'ref' else SearchSiblings
+        try:
+            return Siblings(tool, ctx, *elems[1:])
+        except KeyError:
+            # Param "nav" may be broken. Example: the silly MSN bot replays Appy
+            # URLs, all lowercased.
+            tool.log(WRONG_NAV % nav, type='error')
+            return
 
     def computeStartNumber(self):
         '''Returns the start number of the batch where the current element
            lies.'''
         # First index starts at O, so we calibrate self.number
         number = self.number - 1
         batchSize = self.getBatchSize()
```

### Comparing `appy-1.0.8/py3/appy/ui/portlet.py` & `appy-1.0.9/py3/appy/ui/portlet.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/action.svg` & `appy-1.0.9/py3/appy/ui/static/action.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/add.svg` & `appy-1.0.9/py3/appy/ui/static/add.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/appleicon.png` & `appy-1.0.9/py3/appy/ui/static/appleicon.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/appy.css` & `appy-1.0.9/py3/appy/ui/static/appy.css`

 * *Files 6% similar despite different names*

```diff
@@ -79,15 +79,15 @@
   background-color:|buttonBgColor|; background-repeat:no-repeat;
   background-position:6px 50%; border:none; border-bottom:1px solid grey;
   text-transform:none }
 div.button {
   padding:4px 8px 4px 35px; background-color:transparent; margin-right:5px;
   background-repeat:no-repeat; border:none; border-bottom:1px solid grey }
 input.buttonSmall { font-size:95%; background-color:|sbuttonBgColor| }
-.buttonSmall { margin-bottom:10px }
+.buttonSmall {}
 input.buttonIcon { vertical-align:bottom; margin:0; border:0;
                    background-position:0 100%; padding-left:10px;
                    background-color:transparent }
 input.buttonFixed { width:150px; padding:0 0 0 10px; margin-bottom:6px }
 .fake { color:|warnColor| !important; cursor:help !important; font-style:italic}
 .required { color:|warnColor|; font-weight:bold }
 .xhtml { background-color:transparent; padding:4px }
@@ -170,15 +170,15 @@
 .compact { font-size:95%; width:100% }
 .compact th, .compact td { padding:5px }
 .compact tr { vertical-align: middle }
 .grid { border-collapse:separate; border-spacing:0px }
 .grid th { font-size:90%; text-align:left; background-color:|altColorLight|;
            position:sticky; top:-2px }
 .grid th, .grid td { padding:10px }
-.small { text-align:left; margin:5px 0 }
+.small { text-align:left; margin:8px 0 }
 .small th { background-color:|darkColor|; padding:1px 5px;
             border:1px solid grey; color:|brightColor| }
 .small td { border:1px solid grey; padding:1px 5px }
 .popup .grid th, .popup .grid td { border:1px solid grey }
 .calTable { font-size:95% }
 .calTable td { border:5px solid white; color:#555555; padding:10px }
 .calEvt { width:100% }
@@ -215,17 +215,17 @@
 .trLabel { margin:0.5em 0; border-bottom:1px dashed |altColor| }
 .trLabel img { width:18px; margin:0 10px 5px 0 }
 .section1 { font-size:120%; margin:0.45em 0em 0.1em 0;
             padding:0.3em 0em 0.2em 0.1em; background-color:#eef3f5;
             border-top:1px solid #8CACBB; border-bottom:1px solid #8cacbb }
 .section2 { font-size:14pt; padding:15px 0; text-transform:uppercase;
             border-top:1px dashed #cccccc; background-color:#f9f9f9 }
-.section3 { font-size:100%; font-weight:bold; text-transform:uppercase;
+.section3 { font-size:90%; font-weight:bold; text-transform:uppercase;
             background-color:|darkColor|; text-align:center; color:white;
-            padding:5px }
+            padding:8px 5px; margin-top:15px }
 .even { background-color:rgba(243,243,247,0.7) }
 .odd { background-color:rgba(255,255,255,0.5) }
 .refMenuItem { border-top:grey 1px dashed; margin-top:3px; padding-top:3px }
 .topSpace { margin-top:15px }
 .topSpaceS { margin-top:8px }
 .bottomCell { padding-bottom:30px }
 .bottomSpace { margin-bottom:30px }
@@ -256,28 +256,28 @@
           border-bottom:none !important }
 .tabSep { padding-bottom:|tabSep| }
 .tabBottom { border-bottom:|tabBorderBottom| }
 .tab { background-color:#f1eeee }
 .navText { font-weight:bold; font-size:90%; color:|linkColor|;
            line-height:1.5em }
 .navSep { color:|altColor|; margin:0 6px }
-.language {color:#555555; font-size:7pt; border:grey 1px solid; padding:2px;
-           margin:0 2px 0 4px; font-family:monospace }
 .highlight { background-color:yellow }
 .highlightRow { font-weight:bold; background-color:yellow; opacity:0.6 }
-.globalActions { margin-bottom:30px }
-.objectActions { margin:7px 4px }
-.alignedActions { float:right; padding-right:10px }
+.globalActions { display: flex; margin-bottom:30px }
+.objectActions { display: flex; align-items:center; margin:7px 4px }
+.alignedActions { display:flex; align-items:center; float:right;
+                  padding-right:10px }
 .smallbox { margin:0; vertical-align:middle }
 @keyframes blinkingBg {
-  0% { background-color:white; color:grey }
-  50% { background-color:grey; color:white }
-  100% { background-color:white; color:grey }
+  0%   { background-color:white; color:grey  }
+  50%  { background-color:grey ; color:white }
+  100% { background-color:white; color:grey  }
 }
 .blinkBg { animation:blinkingBg 1s infinite }
+.ct { color:white; font-family:sans-serif; mix-blend-mode:difference }
 .legend { font-size:90%; color:grey }
 .legendRight { float:right; margin-left:10px }
 .legend td { padding:1px 0px; border:0 !important }
 
 /* Bugfix for the calendar class from jscalendar */
 .calendar { z-index: 10 }
```

### Comparing `appy-1.0.8/py3/appy/ui/static/appy.js` & `appy-1.0.9/py3/appy/ui/static/appy.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/asc.svg` & `appy-1.0.9/py3/appy/ui/static/asc.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/back.png` & `appy-1.0.9/py3/appy/ui/static/back.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/baseBG.jpg` & `appy-1.0.9/py3/appy/ui/static/baseBG.jpg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/burger.svg` & `appy-1.0.9/py3/appy/ui/static/burger.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/calendar.js` & `appy-1.0.9/py3/appy/ui/static/calendar.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/calendar.svg` & `appy-1.0.9/py3/appy/ui/static/calendar.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/cancel.svg` & `appy-1.0.9/py3/appy/ui/static/cancel.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/checkAll.svg` & `appy-1.0.9/py3/appy/ui/static/checkAll.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/ckeditor/config.js` & `appy-1.0.9/py3/appy/ui/static/ckeditor/config.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/ckeditor/contents.css` & `appy-1.0.9/py3/appy/ui/static/ckeditor/contents.css`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/close.svg` & `appy-1.0.9/py3/appy/ui/static/close.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/config.svg` & `appy-1.0.9/py3/appy/ui/static/config.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/custom.svg` & `appy-1.0.9/py3/appy/ui/static/custom.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/delete.svg` & `appy-1.0.9/py3/appy/ui/static/delete.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/deleteMany.svg` & `appy-1.0.9/py3/appy/ui/static/deleteMany.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/deleteS.svg` & `appy-1.0.9/py3/appy/ui/static/deleteS.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/download.svg` & `appy-1.0.9/py3/appy/ui/static/download.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/edit.svg` & `appy-1.0.9/py3/appy/ui/static/edit.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/editPage.svg` & `appy-1.0.9/py3/appy/ui/static/editPage.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/email.png` & `appy-1.0.9/py3/appy/ui/static/email.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/external.png` & `appy-1.0.9/py3/appy/ui/static/external.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/favicon.ico` & `appy-1.0.9/py3/appy/ui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/funnel.svg` & `appy-1.0.9/py3/appy/ui/static/funnel.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/grid.svg` & `appy-1.0.9/py3/appy/ui/static/grid.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/groups.svg` & `appy-1.0.9/py3/appy/ui/static/groups.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/headerBG.png` & `appy-1.0.9/py3/appy/ui/static/headerBG.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/help.svg` & `appy-1.0.9/py3/appy/ui/static/help.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/history.svg` & `appy-1.0.9/py3/appy/ui/static/history.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/home.svg` & `appy-1.0.9/py3/appy/ui/static/home.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/homeBG.jpg` & `appy-1.0.9/py3/appy/ui/static/homeBG.jpg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/homeLogo.png` & `appy-1.0.9/py3/appy/ui/static/homeLogo.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/internals.svg` & `appy-1.0.9/py3/appy/ui/static/internals.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/calendar-blue.css` & `appy-1.0.9/py3/appy/ui/static/jscalendar/calendar-blue.css`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/calendar-setup.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/calendar-setup.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/calendar.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/calendar.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-af.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-af.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-al.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-al.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-bg.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-bg.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-big5-utf8.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-big5-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-big5.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-big5.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-br.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-br.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-ca.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-ca.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-cs-utf8.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-cs-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-cs-win.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-cs-win.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-da.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-da.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-de.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-de.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-du.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-du.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-el.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-el.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-en.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-en.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-es.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-es.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-eu.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-eu.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-fi.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-fi.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-fr.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-fr.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-he-utf8.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-he-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-hr-utf8.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-hr-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-hr.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-hr.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-hu.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-hu.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-it.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-it.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-jp.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-jp.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-ko-utf8.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-ko-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-ko.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-ko.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-lt-utf8.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-lt-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-lt.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-lt.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-lv.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-lv.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-nl.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-nl.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-no.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-no.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-pl-utf8.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-pl-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-pl.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-pl.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-pt.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-pt.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-ro.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-ro.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-ru-UTF.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-ru-UTF.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-ru.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-ru.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-ru_win_.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-ru_win_.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-si.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-si.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-sk.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-sk.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-sp.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-sp.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-sr-utf8.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-sr-utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-sr.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-sr.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-sv.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-sv.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-tr.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-tr.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/calendar-zh.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/calendar-zh.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/lang/cn_utf8.js` & `appy-1.0.9/py3/appy/ui/static/jscalendar/lang/cn_utf8.js`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/skins/aqua/theme.css` & `appy-1.0.9/py3/appy/ui/static/jscalendar/skins/aqua/theme.css`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/skins/aqua/today-bg.gif` & `appy-1.0.9/py3/appy/ui/static/jscalendar/skins/aqua/today-bg.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/jscalendar/skins/tiger/theme.css` & `appy-1.0.9/py3/appy/ui/static/jscalendar/skins/tiger/theme.css`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/linkMany.svg` & `appy-1.0.9/py3/appy/ui/static/linkMany.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/list.svg` & `appy-1.0.9/py3/appy/ui/static/list.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/loading_big.gif` & `appy-1.0.9/py3/appy/ui/static/loading_big.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/loading_button.gif` & `appy-1.0.9/py3/appy/ui/static/loading_button.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/loading_icon.gif` & `appy-1.0.9/py3/appy/ui/static/loading_icon.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/loading_link.gif` & `appy-1.0.9/py3/appy/ui/static/loading_link.gif`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/locked.svg` & `appy-1.0.9/py3/appy/ui/static/locked.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/login.svg` & `appy-1.0.9/py3/appy/ui/static/login.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/loginLogo.png` & `appy-1.0.9/py3/appy/ui/static/loginLogo.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/logout.svg` & `appy-1.0.9/py3/appy/ui/static/logout.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/page.svg` & `appy-1.0.9/py3/appy/ui/static/page.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/pagePages.svg` & `appy-1.0.9/py3/appy/ui/static/pagePages.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/pagePassword.svg` & `appy-1.0.9/py3/appy/ui/static/pagePassword.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/pageProfile.svg` & `appy-1.0.9/py3/appy/ui/static/pageProfile.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/pageTranslations.svg` & `appy-1.0.9/py3/appy/ui/static/pageTranslations.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/pageUsers.svg` & `appy-1.0.9/py3/appy/ui/static/pageUsers.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/paperclip.png` & `appy-1.0.9/py3/appy/ui/static/paperclip.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/password.svg` & `appy-1.0.9/py3/appy/ui/static/password.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/pay.svg` & `appy-1.0.9/py3/appy/ui/static/pay.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/popupBG.jpg` & `appy-1.0.9/py3/appy/ui/static/popupBG.jpg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/portletAdd.svg` & `appy-1.0.9/py3/appy/ui/static/portletAdd.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/portletLogo.png` & `appy-1.0.9/py3/appy/ui/static/portletLogo.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/pwd.png` & `appy-1.0.9/py3/appy/ui/static/pwd.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/python.svg` & `appy-1.0.9/py3/appy/ui/static/python.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/refresh.png` & `appy-1.0.9/py3/appy/ui/static/refresh.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/reindex.png` & `appy-1.0.9/py3/appy/ui/static/reindex.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/save.svg` & `appy-1.0.9/py3/appy/ui/static/save.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/search.svg` & `appy-1.0.9/py3/appy/ui/static/search.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/unlink.svg` & `appy-1.0.9/py3/appy/ui/static/unlink.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/unlinkMany.svg` & `appy-1.0.9/py3/appy/ui/static/unlinkMany.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/url.png` & `appy-1.0.9/py3/appy/ui/static/url.png`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/user.svg` & `appy-1.0.9/py3/appy/ui/static/user.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/static/warning.svg` & `appy-1.0.9/py3/appy/ui/static/warning.svg`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/template.py` & `appy-1.0.9/py3/appy/ui/template.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/title.py` & `appy-1.0.9/py3/appy/ui/title.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/ui/validate.py` & `appy-1.0.9/py3/appy/ui/validate.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/utils/__init__.py` & `appy-1.0.9/py3/appy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/utils/analytics.py` & `appy-1.0.9/py3/appy/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/utils/client.py` & `appy-1.0.9/py3/appy/utils/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -213,25 +213,32 @@
     def __repr__(self):
         pairs = ['%s=%s' % (k, v) for k, v in self.__dict__.items()]
         return '<Realm %s>' % ','.join(pairs)
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class HttpResponse:
     '''Stores information about a HTTP response'''
+
+    # Useful empty dict
+    emptyDict = {}
+
     def __init__(self, resource, response, body, duration=None, utf8=True,
-                 responseType=None):
+                 responseType=None, unmarshallParams=None):
         self.resource = resource
         self.code = response.status # The return code, ie 404, 200, 500...
         self.text = response.reason # Textual description of the code
         self.headers = response.msg # A dict-like object containing the headers
         self.body = body # The body of the HTTP response
         # p_duration, if given, is the time, in seconds, we have waited, before
         # getting this response after having sent the request.
         self.duration = duration
         self.utf8 = utf8
+        # If data must be unmarshalled, customizing the unmarshalling process
+        # can be done by specifying a dict of p_unmarshallParams.
+        self.unmarshallParams = unmarshallParams
         # The following attribute may contain specific data extracted from
         # the previous fields. For example, when response if 302 (Redirect),
         # self.data contains the URI where we must redirect the user to.
         self.data = self.extractData(responseType)
         self.response = response
 
     def __repr__(self, complete=False):
@@ -307,15 +314,16 @@
             return JsonDecoder.decode(self.body)
         # Manage XML content
         for xmlHeader in self.xmlHeaders:
             # Ensure this is XML
             if not contentType.startswith(xmlHeader): continue
             # Return an unmarshalled version of the XML content, for easy use
             try:
-                parser = Unmarshaller()
+                params = self.unmarshallParams or HttpResponse.emptyDict
+                parser = Unmarshaller(**params)
                 res = parser.parse(self.body)
                 if parser.rootTag == 'exception':
                     # This is an exception: "res" contains the traceback
                     raise Resource.Error('Distant server exception: %s' % res)
                 return res
             except xml.sax.SAXParseException as se:
                 raise Resource.Error('Invalid XML response (%s)' % str(se))
@@ -418,15 +426,15 @@
             try:
                 r = r.decode()
             except UnicodeDecodeError:
                 pass
         return r
 
     def send(self, method, uri, body=None, headers=None, bodyType=None,
-             responseType=None):
+             responseType=None, unmarshallParams=None):
         '''Sends a HTTP request with p_method, for p_uri'''
         hc = http.client
         if self.protocol == 'https':
             context = ssl.SSLContext()
             context.verify_mode = ssl.CERT_NONE
             conn = hc.HTTPSConnection(self.host, self.port,
                                       timeout=self.timeout, context=context)
@@ -462,15 +470,16 @@
         conn.close()
         # Return a smart object containing the various parts of the response
         duration = None
         if self.measure:
             duration = endTime - startTime
             self.serverTime += duration
         return HttpResponse(self, response, body, duration=duration,
-                            utf8=self.utf8, responseType=responseType)
+                            utf8=self.utf8, responseType=responseType,
+                            unmarshallParams=unmarshallParams)
 
     def mkdir(self, name):
         '''Creates a folder named p_name in this resource.'''
         folderUri = self.uri + '/' + name
         #body = '<d:propertyupdate xmlns:d="DAV:"><d:set><d:prop>' \
         #       '<d:displayname>%s</d:displayname></d:prop></d:set>' \
         #       '</d:propertyupdate>' % name
@@ -493,33 +502,36 @@
         if fileType: headers['Content-Type'] = fileType
         if encoding: headers['Content-Encoding'] = encoding
         r = self.send('PUT', fileUri, body, headers, bodyType='file')
         body.close()
         return r
 
     def get(self, uri=None, headers=None, params=None, followRedirect=True,
-            responseType=None):
+            responseType=None, unmarshallParams=None):
         '''Perform a HTTP GET on the server. Parameters can be given as a dict
            in p_params. p_responseType will be used if no "Content-Type" key is
-           found on the HTTP response.'''
+           found on the HTTP response. In the processs of unmarshalling received
+           data, specific parameters can be passed in dict
+           p_unmarshallParams. '''
         if not uri: uri = self.uri
         # Encode and append params if given
         if params:
             sep = ('?' in uri) and '&' or '?'
             uri = '%s%s%s' % (uri, sep, urllib.urlencode(params))
-        r = self.send('GET', uri, headers=headers, responseType=responseType)
+        r = self.send('GET', uri, headers=headers, responseType=responseType,
+                      unmarshallParams=unmarshallParams)
         # Follow redirect when relevant
-        if (r.code == 302) and followRedirect:
+        if r.code == 302 and followRedirect:
             # Addition durations when "measure" is True
             duration = r.duration
             r = self.get(r.data, headers=headers)
             if self.measure: r.duration += duration
             return r
         # Perform Digest-based authentication when relevant
-        if (r.code == 401) and (self.authMethod == 'Digest') and r.data:
+        if r.code == 401 and self.authMethod == 'Digest' and r.data:
             # Re-trigger the request with the correct authentication headers
             headers = headers or {}
             headers['Authorization'] = r.data.buildCredentials(self, uri)
             return self.get(uri=uri, headers=headers, params=params,
                        followRedirect=followRedirect, responseType=responseType)
         return r
     rss = get
```

### Comparing `appy-1.0.8/py3/appy/utils/dates.py` & `appy-1.0.9/py3/appy/utils/dates.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     pass
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 # Days of the week
 weekDays = ('Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun')
 weekDays_ = weekDays + ('Off',)
 
+S_E_KO   = 'End date cannot be prior to start date.'
+
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Date:
     '''Date-related methods'''
 
     @classmethod
     def toUTC(class_, d):
         '''When manipulating DateTime instances, like p_d, errors can raise when
@@ -159,15 +161,58 @@
     fmt = '%d/%s/%%d %%H:%%M:%%S' % (year, month)
     dateStr = date.strftime(fmt)
     try:
         r = DateTime(dateStr)
     except Exception as e:
         # Start with the first day of the target month and get its last day
         fmt = '%d/%s/01' % (year, month)
-        r = getLastDayOfMonth(DateTime(date.strftime(fmt)), hour='%H:%M:%S')
+        r = getLastDayOfMonth(DateTime(date.strftime(fmt)),
+                              hour=date.strftime('%H:%M:%S'))
+    return r
+
+#- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
+def getCalendarMonths(date, end=None, fmt='%Y%m'):
+    '''Returns, as a set of strings with this p_fmt, the months being crossed
+       by p_date, or, if p_end is passed, being crossed by range
+       (p_date, p_end).'''
+    # By "month", we mean: the complete range of dates being shown when a month
+    # is shown in a monthly-view calendar. Because, in that kind of view, full
+    # weeks are rendered, the "month" generally encompasses several days from
+    # the previous and next months.
+    r = set()
+    fdate = date.strftime(fmt)
+    r.add(fdate)
+    # Get the first day of the week into which p_date is. dow
+    # (*d*ay *o*f *w*eek) for Sunday is 0: we convert it to 7.
+    dow = date.dow() or 7
+    first = date - (dow-1)
+    r.add(first.strftime(fmt)) # May be from the previous month
+    # Take p_end into account if present
+    if end:
+        # Ensure p_end is not prior to p_date
+        if end < date: raise Exception(S_E_KO)
+        fend = end.strftime(fmt)
+        r.add(fend)
+    else:
+        end = date
+        fend = fdate
+    # Get the last day of the week into which p_end is
+    dow = end.dow()
+    if dow != 0: # If Sunday, there will be no overflow on the next month
+        last = end + (7-dow)
+        r.add(last.strftime(fmt))
+    # Add intermediary months between p_date and p_end, if distant from more
+    # than one month.
+    if fdate != fend and end - date > 28:
+        month = getSiblingMonth(date)
+        smonth = month.strftime(fmt)
+        while smonth not in r:
+            r.add(smonth)
+            month = getSiblingMonth(month)
+            smonth = month.strftime(fmt)
     return r
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 def periodsIntersect(start1, end1, start2, end2):
     '''Is there an intersection between intervals [start1, end1] and
        [start2, end2] ?'''
     # p_start1 and p_start2 must be DateTime instances.
```

### Comparing `appy-1.0.8/py3/appy/utils/diff.py` & `appy-1.0.9/py3/appy/utils/diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,27 +386,27 @@
         '''
         if line.startswith(self.divDeletePrefix):
             return ('delete', line, None, None)
         if line.startswith(self.divInsertPrefix):
             # Return the line without the surrounding tag
             action = 'insert'
             outerTag = htmlTag.match(line)
-            line = outerTag.group(3)
+            line = outerTag.group(3) if outerTag else '?'
         else:
             action = None
             outerTag = None
         # Replace found inner inserts with their content.
         innerDiffs = []
         while True:
             match = innerDiff.search(line)
             if not match: break
             # I found one.
             innerDiffs.append(match)
             line = self.applyDiff(line, match)
-        return (action, line, innerDiffs, outerTag)
+        return action, line, innerDiffs, outerTag
 
     def computeTag(self, regexTag, content):
         '''p_regexTag is a re.MatchObject from regex htmlTag. p_content is a
            new content to put within this tag. This method produces the new
            string tag filled with p_content.'''
         # Recompute start tag from p_regexTag
         startTag = '<%s' % regexTag.group(1)
```

### Comparing `appy-1.0.8/py3/appy/utils/inject.py` & `appy-1.0.9/py3/appy/utils/inject.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/utils/loc.py` & `appy-1.0.9/py3/appy/utils/loc.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/utils/mail.py` & `appy-1.0.9/py3/appy/utils/mail.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/utils/path.py` & `appy-1.0.9/py3/appy/utils/path.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/utils/pretty.py` & `appy-1.0.9/py3/appy/utils/pretty.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/utils/string.py` & `appy-1.0.9/py3/appy/utils/string.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/utils/tables.py` & `appy-1.0.9/py3/appy/utils/tables.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/utils/url.py` & `appy-1.0.9/py3/appy/utils/url.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/utils/zip.py` & `appy-1.0.9/py3/appy/utils/zip.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/xml/__init__.py` & `appy-1.0.9/py3/appy/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/xml/cleaner.py` & `appy-1.0.9/py3/appy/xml/cleaner.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/xml/diff.py` & `appy-1.0.9/py3/appy/xml/diff.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/xml/escape.py` & `appy-1.0.9/py3/appy/xml/escape.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/py3/appy/xml/extractor.py` & `appy-1.0.9/py3/appy/xml/extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 # Appy. If not, see <http://www.gnu.org/licenses/>.
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 from appy.xml import Parser
 from appy.utils.string import Normalize
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
-EXTRACTOR_WRONG_PARAMS = "You can't have both 'keepCRs' and 'normalize' " \
-  "being True. Normalizing implies CRs to be removed."
+PARAMS_KO = "You can't have both 'keepCRs' and 'normalize' being True. " \
+            "Normalizing implies CRs to be removed."
 
 #- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 class Extractor(Parser):
     '''Produces a text version of XML/XHTML content'''
+
     # There are 2 main usages to this parser. It can extract text:
     # - to produce a complete but textual version of some XHTML chunk, keeping
     #   accented chars and carriage returns;
     # - to extract text for search purposes, converting any accented char to its
     #   non-accented counterpart and removing any other element.
 
     paraTags = ('p', 'li', 'center', 'div', 'blockquote')
@@ -40,15 +41,15 @@
         # Must we keep carriage returns (and thus keep the global splitting of
         # the text into paragraphs) ?
         self.keepCRs = keepCRs
         # Must text be normalized ? When True, every accented char is converted
         # to its non-accented counterpart.
         self.normalize = normalize
         # Is is not possible to have both p_keepCRs and p_normalize being True
-        if keepCRs and normalize: raise Exception(EXTRACTOR_WRONG_PARAMS)
+        if keepCRs and normalize: raise Exception(PARAMS_KO)
         # Must be lowerise text ? (only if p_normalize is True)
         self.lower = lower
         # Must we keep dashes ? (only if p_normalize is True)
         self.keepDashes = keepDashes
 
     def startDocument(self):
         Parser.startDocument(self)
```

### Comparing `appy-1.0.8/py3/appy/xml/marshaller.py` & `appy-1.0.9/py3/appy/xml/marshaller.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     fieldsToExclude = {'History': 'o'}
 
     # The correspondence between classes and their equivalent base class
     typesMap = {'list': 'list', 'PersistentList': 'list', 'UserList': 'list',
                 'dict': 'dict', 'PersistentMapping': 'dict', 'UserDict': 'dict',
                 'FileInfo': 'file', 'bool': 'bool', 'int': 'int',
                 'float': 'float', 'bytes': 'bytes', 'tuple': 'tuple',
-                'DateTime': 'DateTime'}
+                'DateTime': 'DateTime', }
 
     def __init__(self, cdata=False, conversionFunctions={}, rootTag='appyData',
                  dumpXmlPrologue=True, namespaces={}, namespacedTags={}):
         # If p_cdata is True, all string values will be dumped as XML CDATA
         self.cdata = cdata
         # The following dict stores specific conversion (=Python to XML)
         # functions. Such functions are useful when you are not happy with the
@@ -80,15 +80,15 @@
         prefix = ''
         if name in self.namespacedTags: prefix = self.namespacedTags[name]
         elif '*' in self.namespacedTags: prefix = self.namespacedTags['*']
         return '%s:%s' % (prefix, name) if prefix else name
 
     def isAppy(self, o):
         '''Returns True if p_o is an Appy object'''
-        return hasattr(o, 'class_')
+        return hasattr(o, 'class_') and o.class_
 
     def isObject(self, o):
         '''Returns True if p_o is an instance of a custom class, False if it is
            a basic type, or tuple, sequence, etc.'''
         return hasattr(o, '__dict__')
 
     def dumpRootTag(self, r, o):
@@ -114,14 +114,18 @@
         '''Dumps a string into the result'''
         # Surround it with a CDATA when appropriate
         if self.cdata: r.write('<![CDATA[')
         # Escape XML chars
         r.write(Escape.xml(s))
         if self.cdata: r.write(']]>')
 
+    def dumpBytes(self, r, value):
+        '''Dumps p_value, which is a bytes value'''
+        self.dumpString(value.decode())
+
     def dumpFile(self, r, v):
         '''Dumps a file into the result'''
         if not v: return
         w = r.write
         # p_value contains an instance of class appy.model.fields.file.FileInfo.
         # Encode it in Base64, in one or several parts.
         partTag = self.getTagName('part')
@@ -163,27 +167,23 @@
     # Dumping a tuple is similar to dumping a list
     dumpTuple = dumpList
 
     def dumpBool(self, r, value):
         '''Dumps in p_r this p_boolean value'''
         r.write(str(bool(value)))
 
-    def dumpBytes(self, r, value):
-        '''Dumps p_value, which is a bytes value'''
-        r.write(value.decode())
-
     def dumpValue(self, r, value, type, className):
         '''Dumps in p_r the XML version of p_value'''
         # Use a custom function if one is defined for this type of value
         if className in self.conversionFunctions:
             self.conversionFunctions[className](r, value)
             return
         # Find the specific method for dumping this p_value
         if not type:
-            r.write(value or '')
+            self.dumpString(r, value or '')
         else:
             method = 'dump%s' % type.capitalize()
             if hasattr(self, method):
                 exec('self.%s(r, value)' % method)
             else:
                 r.write(str(value))
 
@@ -209,15 +209,15 @@
             type = None
         if type: r.write(' type="%s"' % type)
         # Dump the value's length if multi-valued
         if type in ('list', 'tuple'):
             length = len(value) if value else 0
             r.write(' count="%d"' % length)
         # Dump file-related attributes
-        if value and (type == 'file'):
+        if value and type == 'file':
             # Dump the MIME type
             r.write(' mimeType="%s"' % value.mimeType)
             # Dump the file name
             r.write(' name=%s' % quoteattr(value.uploadName))
         r.write('>')
         # Dump the field value
         self.dumpValue(r, value, type, className)
@@ -248,16 +248,14 @@
                 # Browse p_o's fields that must appear on the XML layout
                 for field in o.getFields('xml'):
                     # Dump only needed fields
                     if not self.mustDump(field.name, className): continue
                     val = field.getValue(o, single=False)
                     v = field.getXmlValue(o, val)
                     self.dumpField(r, field.name, v)
-                # Dump the object history
-                self.dumpField(r, 'history', o.history)
             else:
                 # Dump its URL
                 r.write('%s/xml' % o.url)
         else:
             # A non-Appy object: dump it in its entirety
             className = o.__class__.__name__
             if fieldNames:
```

### Comparing `appy-1.0.8/py3/appy/xml/unmarshaller.py` & `appy-1.0.9/py3/appy/xml/unmarshaller.py`

 * *Files identical despite different names*

### Comparing `appy-1.0.8/setup.py` & `appy-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 if base == 'py3':
     dependencies = ['zodb', 'DateTime']
     python = '>=3.6'
 else:
     dependencies = []
     python = '>=2.4'
 
-setup(name = "appy", version = "1.0.8",
+setup(name = "appy", version = "1.0.9",
       description = "The Appy framework",
       long_description = "Appy is the simpliest way to build complex webapps.",
       author = "Gaetan Delannay",
       author_email = "gaetan.delannay@geezteem.com",
       license = "GPL", platforms="all",
       url = 'https://appyframe.work',
       packages = findPackages(base),
```

