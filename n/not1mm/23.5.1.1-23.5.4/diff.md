# Comparing `tmp/not1mm-23.5.1.1.tar.gz` & `tmp/not1mm-23.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-23.5.1.1.tar", last modified: Mon May  1 21:18:17 2023, max compression
+gzip compressed data, was "not1mm-23.5.4.tar", last modified: Thu May  4 16:53:15 2023, max compression
```

## Comparing `not1mm-23.5.1.1.tar` & `not1mm-23.5.4.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.148401 not1mm-23.5.1.1/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.1.1/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21192 2023-05-01 21:18:17.147401 not1mm-23.5.1.1/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20445 2023-05-01 21:13:35.000000 not1mm-23.5.1.1/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.121401 not1mm-23.5.1.1/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.1.1/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    77167 2023-05-01 20:02:13.000000 not1mm-23.5.1.1/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    18880 2023-05-01 19:53:36.000000 not1mm-23.5.1.1/not1mm/bandmap.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.131401 not1mm-23.5.1.1/not1mm/data/
--rw-rw-rw-   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.1.1/not1mm/data/Combinear.qss
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.1.1/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.1.1/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.1.1/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.1.1/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.1.1/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.1.1/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39001 2023-05-01 19:49:53.000000 not1mm-23.5.1.1/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.1.1/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.1.1/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.1.1/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.1.1/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.1.1/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.1.1/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.1.1/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.1.1/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.1.1/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.1.1/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.1.1/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43658 2023-05-01 15:38:56.000000 not1mm-23.5.1.1/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17745 2023-05-01 21:11:17.000000 not1mm-23.5.1.1/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.1.1/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.140401 not1mm-23.5.1.1/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.1.1/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.1.1/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.1.1/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.1.1/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.1.1/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.1.1/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.1.1/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.1.1/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.1.1/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.1.1/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.1.1/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.1.1/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.1.1/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.1.1/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.1.1/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.1.1/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.1.1/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.1.1/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.1.1/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.1.1/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.1.1/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.1.1/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.1.1/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.1.1/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.1.1/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.1.1/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.1.1/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.1.1/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.1.1/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.1.1/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.1.1/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.1.1/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.1.1/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.1.1/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.1.1/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.1.1/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.1.1/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.1.1/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.1.1/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.1.1/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.1.1/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.1.1/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.1.1/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.1.1/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.1.1/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.1.1/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.1.1/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.1.1/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.1.1/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.1.1/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.1.1/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.1.1/not1mm/data/ssbmacros.txt
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.143401 not1mm-23.5.1.1/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.1.1/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.1.1/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12468 2023-04-25 15:08:00.000000 not1mm-23.5.1.1/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.1.1/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32966 2023-04-24 03:05:48.000000 not1mm-23.5.1.1/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.1.1/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.1.1/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.1.1/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.1.1/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.1.1/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.1.1/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.1.1/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.1.1/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.1.1/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.1.1/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5781 2023-05-01 19:29:49.000000 not1mm-23.5.1.1/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       48 2023-05-01 21:16:13.000000 not1mm-23.5.1.1/not1mm/lib/version.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    31143 2023-05-01 19:53:26.000000 not1mm-23.5.1.1/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.147401 not1mm-23.5.1.1/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13552 2023-05-01 21:04:22.000000 not1mm-23.5.1.1/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13558 2023-05-01 16:14:59.000000 not1mm-23.5.1.1/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13565 2023-05-01 21:07:00.000000 not1mm-23.5.1.1/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13568 2023-05-01 21:07:03.000000 not1mm-23.5.1.1/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.1.1/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14348 2023-04-24 14:53:10.000000 not1mm-23.5.1.1/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14351 2023-04-24 14:53:19.000000 not1mm-23.5.1.1/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12719 2023-04-24 14:53:32.000000 not1mm-23.5.1.1/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2590 2023-04-24 14:53:43.000000 not1mm-23.5.1.1/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2591 2023-04-24 14:53:53.000000 not1mm-23.5.1.1/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2594 2023-04-24 14:54:04.000000 not1mm-23.5.1.1/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14755 2023-04-24 14:54:20.000000 not1mm-23.5.1.1/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14759 2023-04-24 14:54:36.000000 not1mm-23.5.1.1/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13701 2023-04-24 14:54:47.000000 not1mm-23.5.1.1/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13772 2023-04-24 14:54:56.000000 not1mm-23.5.1.1/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14624 2023-04-24 14:52:00.000000 not1mm-23.5.1.1/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7272 2023-04-24 14:55:06.000000 not1mm-23.5.1.1/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13650 2023-04-24 14:55:15.000000 not1mm-23.5.1.1/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13651 2023-04-24 14:55:25.000000 not1mm-23.5.1.1/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2851 2023-04-24 14:55:37.000000 not1mm-23.5.1.1/not1mm/plugins/winter_field_day.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.147401 not1mm-23.5.1.1/not1mm/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2297 2023-03-29 19:50:12.000000 not1mm-23.5.1.1/not1mm/testing/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.122401 not1mm-23.5.1.1/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21192 2023-05-01 21:18:17.000000 not1mm-23.5.1.1/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3460 2023-05-01 21:18:17.000000 not1mm-23.5.1.1/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-01 21:18:17.000000 not1mm-23.5.1.1/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-01 21:18:17.000000 not1mm-23.5.1.1/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-01 21:18:17.000000 not1mm-23.5.1.1/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-01 21:18:17.000000 not1mm-23.5.1.1/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1219 2023-05-01 21:16:15.000000 not1mm-23.5.1.1/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-01 21:18:17.148401 not1mm-23.5.1.1/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.147401 not1mm-23.5.1.1/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.1.1/testing/test.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-21 20:18:16.000000 not1mm-23.5.1.1/testing/text2.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.873883 not1mm-23.5.4/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.4/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21350 2023-05-04 16:53:15.873883 not1mm-23.5.4/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20605 2023-05-04 16:51:42.000000 not1mm-23.5.4/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.841884 not1mm-23.5.4/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.4/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    77543 2023-05-04 02:56:26.000000 not1mm-23.5.4/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    18606 2023-05-03 01:46:35.000000 not1mm-23.5.4/not1mm/bandmap.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.850884 not1mm-23.5.4/not1mm/data/
+-rw-rw-rw-   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.4/not1mm/data/Combinear.qss
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.4/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.4/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.4/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.4/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.4/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.4/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39001 2023-05-01 19:49:53.000000 not1mm-23.5.4/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.4/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.4/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.4/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.4/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.4/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.4/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.4/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.4/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.4/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.4/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.4/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43658 2023-05-01 15:38:56.000000 not1mm-23.5.4/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17745 2023-05-01 21:11:17.000000 not1mm-23.5.4/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.4/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.862883 not1mm-23.5.4/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.4/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.4/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.4/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.4/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.4/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.4/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.4/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.4/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.4/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.4/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.4/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.4/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.4/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.4/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.4/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.4/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.4/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.4/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.4/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.4/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.4/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.4/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.4/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.4/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.4/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.4/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.4/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.4/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.4/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.4/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.4/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.4/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.4/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.4/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.4/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.4/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.4/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.4/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.4/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.4/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.4/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.4/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.4/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.4/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.4/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.4/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.4/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.4/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.4/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.4/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.4/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.4/not1mm/data/ssbmacros.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.869883 not1mm-23.5.4/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.4/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.4/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12468 2023-04-25 15:08:00.000000 not1mm-23.5.4/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.4/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32966 2023-04-24 03:05:48.000000 not1mm-23.5.4/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.4/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.4/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.4/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.4/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.4/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.4/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.4/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.4/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.4/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.4/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5781 2023-05-01 19:29:49.000000 not1mm-23.5.4/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-05-04 16:47:26.000000 not1mm-23.5.4/not1mm/lib/version.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    31143 2023-05-01 19:53:26.000000 not1mm-23.5.4/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.872883 not1mm-23.5.4/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13552 2023-05-01 21:04:22.000000 not1mm-23.5.4/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13558 2023-05-01 16:14:59.000000 not1mm-23.5.4/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13565 2023-05-01 21:07:00.000000 not1mm-23.5.4/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13568 2023-05-01 21:07:03.000000 not1mm-23.5.4/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.4/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14348 2023-04-24 14:53:10.000000 not1mm-23.5.4/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14351 2023-04-24 14:53:19.000000 not1mm-23.5.4/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12719 2023-04-24 14:53:32.000000 not1mm-23.5.4/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2590 2023-04-24 14:53:43.000000 not1mm-23.5.4/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2591 2023-04-24 14:53:53.000000 not1mm-23.5.4/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2594 2023-04-24 14:54:04.000000 not1mm-23.5.4/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14807 2023-05-04 16:44:11.000000 not1mm-23.5.4/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14811 2023-05-04 16:45:09.000000 not1mm-23.5.4/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13701 2023-04-24 14:54:47.000000 not1mm-23.5.4/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13772 2023-04-24 14:54:56.000000 not1mm-23.5.4/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14624 2023-04-24 14:52:00.000000 not1mm-23.5.4/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7272 2023-04-24 14:55:06.000000 not1mm-23.5.4/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13650 2023-04-24 14:55:15.000000 not1mm-23.5.4/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13651 2023-04-24 14:55:25.000000 not1mm-23.5.4/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2851 2023-04-24 14:55:37.000000 not1mm-23.5.4/not1mm/plugins/winter_field_day.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.872883 not1mm-23.5.4/not1mm/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2297 2023-03-29 19:50:12.000000 not1mm-23.5.4/not1mm/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.842884 not1mm-23.5.4/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21350 2023-05-04 16:53:15.000000 not1mm-23.5.4/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3460 2023-05-04 16:53:15.000000 not1mm-23.5.4/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-04 16:53:15.000000 not1mm-23.5.4/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-04 16:53:15.000000 not1mm-23.5.4/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-04 16:53:15.000000 not1mm-23.5.4/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-04 16:53:15.000000 not1mm-23.5.4/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1217 2023-05-04 16:47:34.000000 not1mm-23.5.4/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-04 16:53:15.873883 not1mm-23.5.4/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.873883 not1mm-23.5.4/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.4/testing/test.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-21 20:18:16.000000 not1mm-23.5.4/testing/text2.py
```

### Comparing `not1mm-23.5.1.1/LICENSE` & `not1mm-23.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/PKG-INFO` & `not1mm-23.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.1.1
+Version: 23.5.4
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -113,14 +113,16 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
+- [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
+- [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
 <summary>April 2023</summary>
 
 - [23-4-29] Added callsign and connect button to the bandmap. Fixed rxmarker not updateing.
@@ -346,14 +348,15 @@
 You can include a limited set of substitution instructions.
 
 - {MYCALL} Sends the station call.
 - {HISCALL} Send what's in the callsign field.
 - {SNT} Sends 5nn (cw) or 599 (ssb)
 - {SENTNR} Sends whats in the SentNR field.
 - {EXCH} Sends what's in the Sent Exchange field when contest is defined.
+- '#' Sends serial number.
 
 ### Macro use with voice
 
 The macros when used with voice, will also accept filenames of WAV files to play, excluding the file extension. The filename must be enclosed by brackets. For example `[CQ]` will play `cq.wav`, `[again]` will play `again.wav`. The wav files are stored in the operators personal data directory. The filenames must be in lowercase. See [Various data file locations](#various-data-file-locations) above for the location of your data files. For me, the macro `[cq]` will play `/home/mbridak/.local/share/not1mm/K6GTE/cq.wav`
 
 **The current wav files in place are not the ones you will want to use. They sound like an idiot.** You can use something like Audacity to record new wav files in your own voice.
```

### Comparing `not1mm-23.5.1.1/README.md` & `not1mm-23.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,16 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
+- [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
+- [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
 <summary>April 2023</summary>
 
 - [23-4-29] Added callsign and connect button to the bandmap. Fixed rxmarker not updateing.
@@ -327,14 +329,15 @@
 You can include a limited set of substitution instructions.
 
 - {MYCALL} Sends the station call.
 - {HISCALL} Send what's in the callsign field.
 - {SNT} Sends 5nn (cw) or 599 (ssb)
 - {SENTNR} Sends whats in the SentNR field.
 - {EXCH} Sends what's in the Sent Exchange field when contest is defined.
+- '#' Sends serial number.
 
 ### Macro use with voice
 
 The macros when used with voice, will also accept filenames of WAV files to play, excluding the file extension. The filename must be enclosed by brackets. For example `[CQ]` will play `cq.wav`, `[again]` will play `again.wav`. The wav files are stored in the operators personal data directory. The filenames must be in lowercase. See [Various data file locations](#various-data-file-locations) above for the location of your data files. For me, the macro `[cq]` will play `/home/mbridak/.local/share/not1mm/K6GTE/cq.wav`
 
 **The current wav files in place are not the ones you will want to use. They sound like an idiot.** You can use something like Audacity to record new wav files in your own voice.
```

### Comparing `not1mm-23.5.1.1/not1mm/__main__.py` & `not1mm-23.5.4/not1mm/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -572,14 +572,15 @@
                 self.pref.get("contest")
             )
             if self.contest_settings:
                 self.database.current_contest = self.pref.get("contest")
                 if self.contest_settings.get("ContestName"):
                     self.contest = doimp(self.contest_settings.get("ContestName"))
                     logger.debug("Loaded Contest Name = %s", self.contest.name)
+                    self.set_window_title()
                     self.contest.init_contest(self)
                     self.hide_band_mode(self.contest_settings.get("ModeCategory", ""))
 
                 if hasattr(self.contest, "mode"):
                     if self.contest.mode in ["CW", "BOTH"]:
                         self.cw_speed.show()
                     else:
@@ -832,20 +833,22 @@
         if vfoa:
             vfoa = int(vfoa) / 1000
         else:
             vfoa = 0.0
         contest_name = ""
         if self.contest:
             contest_name = self.contest.name
-        self.setWindowTitle(
-            f"{round(vfoa,2)} "
-            f"{self.radio_state.get('mode', '')} "
+        line = (
+            f"vfoa:{round(vfoa,2)} "
+            f"mode:{self.radio_state.get('mode', '')} "
             f"OP:{self.current_op} {contest_name} "
             f"- Not1MM v{__version__}"
         )
+        logger.debug("%s", line)
+        self.setWindowTitle(line)
 
     def clearinputs(self):
         """Clears the text input fields and sets focus to callsign field."""
         self.dupe_indicator.hide()
         self.contact = self.database.empty_contact
         self.heading_distance.setText("")
         self.dx_entity.setText("")
@@ -1130,15 +1133,22 @@
     def edit_F12(self):
         """stub"""
         logger.debug("F12 Right Clicked.")
         self.edit_macro(self.F12)
 
     def process_macro(self, macro: str) -> str:
         """Process CW macro substitutions"""
+        result = self.database.get_serial()
+        print(result)
+        next_serial = str(result.get("serial_nr", "1"))
+        if next_serial == "None":
+            next_serial = "1"
+        print(next_serial)
         macro = macro.upper()
+        macro = macro.replace("#", next_serial)
         macro = macro.replace("{MYCALL}", self.station.get("Call", ""))
         macro = macro.replace("{HISCALL}", self.callsign.text())
         if self.radio_state.get("mode") == "CW":
             macro = macro.replace("{SNT}", self.sent.text().replace("9", "n"))
         else:
             macro = macro.replace("{SNT}", self.sent.text())
         macro = macro.replace("{SENTNR}", self.other_1.text())
@@ -1739,16 +1749,16 @@
                 logger.debug("Creating Op Directory: %s", str(op_path))
                 os.mkdir(str(op_path))
             if op_path.is_dir():
                 source_path = Path(WORKING_PATH) / "data" / "phonetics"
                 logger.debug("source_path: %s", str(source_path))
                 for child in source_path.iterdir():
                     destination_file = op_path / child.name
-                    logger.debug("Destination: %s", str(destination_file))
                     if destination_file.is_file() is False:
+                        logger.debug("Destination: %s", str(destination_file))
                         destination_file.write_bytes(child.read_bytes())
 
     def poll_radio(self):
         """stub"""
         if self.rig_control:
             if self.rig_control.online:
                 vfo = self.rig_control.get_vfo()
@@ -1935,15 +1945,15 @@
 logger.info(families)
 window = MainWindow()
 height = window.pref.get("window_height", 300)
 width = window.pref.get("window_width", 700)
 x = window.pref.get("window_x", -1)
 y = window.pref.get("window_y", -1)
 window.setGeometry(x, y, width, height)
-window.setWindowTitle(f"Not1MM v{__version__}")
+# window.setWindowTitle(f"Not1MM v{__version__}")
 window.callsign.setFocus()
 window.show()
 timer = QtCore.QTimer()
 timer.timeout.connect(window.poll_radio)
 timer2 = QtCore.QTimer()
 timer2.timeout.connect(window.check_udp_traffic)
```

### Comparing `not1mm-23.5.1.1/not1mm/bandmap.py` & `not1mm-23.5.4/not1mm/bandmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,19 +269,15 @@
                 step, _ = self.determine_step_digits()
                 self.drawTXRXMarks(step)
 
     def spot_clicked(self):
         """dunno"""
         items = self.bandmap_scene.selectedItems()
         for item in items:
-            print(f"{item}")
             if item:
-                print(
-                    f"{item.toPlainText()} tip: {item.toolTip()} prop:{item.property('freq')}"
-                )
                 cmd = {}
                 cmd["cmd"] = "TUNE"
                 cmd["freq"] = items[0].property("freq")
                 cmd["spot"] = items[0].toPlainText().split()[0]
                 packet = bytes(dumps(cmd), encoding="ascii")
                 self.udpsocket.writeDatagram(
                     packet, QtNetwork.QHostAddress(MULTICAST_GROUP), MULTICAST_PORT
@@ -394,15 +390,14 @@
         if result:
             min_y = 0.0
             for items in result:
                 # lookup = cty_lookup(items.get("callsign"))
                 # if lookup:
                 #     for a in lookup.items():
                 #         entity = a[1].get("entity", "")
-
                 freq_y = (
                     (items.get("freq") - self.currentBand.start) / step
                 ) * PIXELSPERSTEP
                 text_y = max(min_y + 5, freq_y)
                 self.lineitemlist.append(
                     self.bandmap_scene.addLine(
                         22, freq_y, 55, text_y, QtGui.QPen(QtGui.QColor(192, 192, 192))
@@ -419,15 +414,15 @@
                 text.setPos(60, text_y - (text.boundingRect().height() / 2))
                 text.setFlags(
                     QtWidgets.QGraphicsItem.ItemIsFocusable
                     | QtWidgets.QGraphicsItem.ItemIsSelectable
                     | text.flags()
                 )
                 text.setProperty("freq", items.get("freq"))
-                text.setToolTip(items.get(entity, ""))
+                text.setToolTip(items.get("comment"))
 
                 min_y = text_y + text.boundingRect().height() / 2
 
                 # textColor = Data::statusToColor(lower.value().status, qApp->palette().color(QPalette::Text));
                 # text->setDefaultTextColor(textColor);
                 self.textItemList.append(text)
 
@@ -486,31 +481,30 @@
 
     def receive(self):
         """doc"""
         data = self.socket.readAll()
         data = str(data, "utf-8").strip()
         if "login:" in data:
             self.send_command(self.callsignField.text())
-            # self.send_command("Set DX Filter Not Skimmer AND SpotterCont=NA")
-            # self.send_command("sh dx o open")
-            # self.send_command("reject/spot 0 info FT8")
-            # self.send_command("accept/spot 0 freq hf/cw")
-            # self.send_command("accept/spot 1 freq hf/ssb")
+            # self.send_command("Set DX Filter SpotterCont=NA")
+            self.send_command("set dx mode filter")
             return
         if "DX de" in data:
             parts = data.split()
             spotter = parts[2]
             freq = parts[3]
             dx = parts[4]
             _time = parts[-1]
+            comment = " ".join(parts[5:-1])
             # spot = DxSpot()
             spot = {}
             spot["ts"] = datetime.utcnow().isoformat(" ")[:19]
             spot["callsign"] = dx
             spot["spotter"] = spotter
+            spot["comment"] = comment
             try:
                 spot["freq"] = float(freq) / 1000
             except ValueError:
                 logger.debug("%s", f"{data}")
             self.spots.addspot(spot)
             return
         if self.callsignField.text().upper() in data:
@@ -572,12 +566,14 @@
     logger.setLevel(logging.DEBUG)
     logger.debug("debugging on")
 else:
     logger.setLevel(logging.WARNING)
     logger.warning("debugging off")
 
 app = QtWidgets.QApplication(sys.argv)
+
+
 app.setStyle("Fusion")
 window = MainWindow()
 window.show()
 if __name__ == "__main__":
     run()
```

### Comparing `not1mm-23.5.1.1/not1mm/data/Combinear.qss` & `not1mm-23.5.4/not1mm/data/Combinear.qss`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-23.5.4/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/MASTER.SCP` & `not1mm-23.5.4/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/about.ui` & `not1mm-23.5.4/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/bandmap.ui` & `not1mm-23.5.4/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/configuration.ui` & `not1mm-23.5.4/not1mm/data/configuration.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/contests.sql` & `not1mm-23.5.4/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/cty.json` & `not1mm-23.5.4/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/editcontact.ui` & `not1mm-23.5.4/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/editmacro.ui` & `not1mm-23.5.4/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/k6gte.not1mm-128.png` & `not1mm-23.5.4/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/k6gte.not1mm-32.png` & `not1mm-23.5.4/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/k6gte.not1mm-64.png` & `not1mm-23.5.4/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/logwindow.ui` & `not1mm-23.5.4/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/main.ui` & `not1mm-23.5.4/not1mm/data/main.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/new_contest.ui` & `not1mm-23.5.4/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/opon.ui` & `not1mm-23.5.4/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/0.wav` & `not1mm-23.5.4/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/1.wav` & `not1mm-23.5.4/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/2.wav` & `not1mm-23.5.4/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/3.wav` & `not1mm-23.5.4/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/4.wav` & `not1mm-23.5.4/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/5.wav` & `not1mm-23.5.4/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/6.wav` & `not1mm-23.5.4/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/7.wav` & `not1mm-23.5.4/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/73.wav` & `not1mm-23.5.4/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/8.wav` & `not1mm-23.5.4/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/9.wav` & `not1mm-23.5.4/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/a.wav` & `not1mm-23.5.4/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/again.wav` & `not1mm-23.5.4/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/b.wav` & `not1mm-23.5.4/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/c.wav` & `not1mm-23.5.4/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/contest.wav` & `not1mm-23.5.4/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/cq.wav` & `not1mm-23.5.4/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/d.wav` & `not1mm-23.5.4/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/e.wav` & `not1mm-23.5.4/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/f.wav` & `not1mm-23.5.4/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/g.wav` & `not1mm-23.5.4/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/h.wav` & `not1mm-23.5.4/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/i.wav` & `not1mm-23.5.4/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/j.wav` & `not1mm-23.5.4/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/k.wav` & `not1mm-23.5.4/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/k6gte.wav` & `not1mm-23.5.4/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/l.wav` & `not1mm-23.5.4/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/m.wav` & `not1mm-23.5.4/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/mynumber.wav` & `not1mm-23.5.4/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/n.wav` & `not1mm-23.5.4/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/nil.wav` & `not1mm-23.5.4/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/o.wav` & `not1mm-23.5.4/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/p.wav` & `not1mm-23.5.4/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/q.wav` & `not1mm-23.5.4/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/r.wav` & `not1mm-23.5.4/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/roger.wav` & `not1mm-23.5.4/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/s.wav` & `not1mm-23.5.4/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/space.wav` & `not1mm-23.5.4/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/t.wav` & `not1mm-23.5.4/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/thankyou.wav` & `not1mm-23.5.4/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-23.5.4/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/u.wav` & `not1mm-23.5.4/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/v.wav` & `not1mm-23.5.4/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/w.wav` & `not1mm-23.5.4/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/x.wav` & `not1mm-23.5.4/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/y.wav` & `not1mm-23.5.4/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/yourcall.wav` & `not1mm-23.5.4/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/phonetics/z.wav` & `not1mm-23.5.4/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/pickcontest.ui` & `not1mm-23.5.4/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/reddot.png` & `not1mm-23.5.4/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/data/settings.ui` & `not1mm-23.5.4/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/lib/cat_interface.py` & `not1mm-23.5.4/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/lib/cwinterface.py` & `not1mm-23.5.4/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/lib/database.py` & `not1mm-23.5.4/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/lib/edit_macro.py` & `not1mm-23.5.4/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/lib/edit_station.py` & `not1mm-23.5.4/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/lib/ham_utility.py` & `not1mm-23.5.4/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/lib/lookup.py` & `not1mm-23.5.4/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/lib/multicast.py` & `not1mm-23.5.4/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/lib/n1mm.py` & `not1mm-23.5.4/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/lib/settings.py` & `not1mm-23.5.4/not1mm/lib/settings.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/logwindow.py` & `not1mm-23.5.4/not1mm/logwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/10_10_fall_cw.py` & `not1mm-23.5.4/not1mm/plugins/10_10_fall_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/10_10_spring_cw.py` & `not1mm-23.5.4/not1mm/plugins/10_10_spring_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/10_10_summer_phone.py` & `not1mm-23.5.4/not1mm/plugins/10_10_summer_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/10_10_winter_phone.py` & `not1mm-23.5.4/not1mm/plugins/10_10_winter_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/arrl_dx_cw.py` & `not1mm-23.5.4/not1mm/plugins/arrl_dx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-23.5.4/not1mm/plugins/arrl_dx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/arrl_field_day.py` & `not1mm-23.5.4/not1mm/plugins/arrl_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-23.5.4/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/arrl_ss_cw.py` & `not1mm-23.5.4/not1mm/plugins/arrl_ss_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/arrl_ss_phone.py` & `not1mm-23.5.4/not1mm/plugins/arrl_ss_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/cq_wpx_cw.py` & `not1mm-23.5.4/not1mm/plugins/cq_wpx_cw.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,15 +358,15 @@
 
             print(
                 f"CLAIMED-SCORE: {calc_score(self)}",
                 end="\r\n",
                 file=file_descriptor,
             )
             print(
-                "OPERATORS: ",
+                f"OPERATORS: {self.contest_settings.get('Operators','')}".upper(),
                 end="\r\n",
                 file=file_descriptor,
             )
             print(
                 f"NAME: {self.station.get('Name', '')}",
                 end="\r\n",
                 file=file_descriptor,
```

### Comparing `not1mm-23.5.1.1/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-23.5.4/not1mm/plugins/cq_wpx_ssb.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,15 +358,15 @@
 
             print(
                 f"CLAIMED-SCORE: {calc_score(self)}",
                 end="\r\n",
                 file=file_descriptor,
             )
             print(
-                "OPERATORS: ",
+                f"OPERATORS: {self.contest_settings.get('Operators','')}".upper(),
                 end="\r\n",
                 file=file_descriptor,
             )
             print(
                 f"NAME: {self.station.get('Name', '')}",
                 end="\r\n",
                 file=file_descriptor,
```

### Comparing `not1mm-23.5.1.1/not1mm/plugins/cq_ww_cw.py` & `not1mm-23.5.4/not1mm/plugins/cq_ww_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/cq_ww_ssb.py` & `not1mm-23.5.4/not1mm/plugins/cq_ww_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/cwt.py` & `not1mm-23.5.4/not1mm/plugins/cwt.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/general_logging.py` & `not1mm-23.5.4/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/jidx_cw.py` & `not1mm-23.5.4/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/jidx_ph.py` & `not1mm-23.5.4/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/plugins/winter_field_day.py` & `not1mm-23.5.4/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm/testing/test.py` & `not1mm-23.5.4/not1mm/testing/test.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/not1mm.egg-info/PKG-INFO` & `not1mm-23.5.4/not1mm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.1.1
+Version: 23.5.4
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -113,14 +113,16 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
+- [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
+- [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
 <summary>April 2023</summary>
 
 - [23-4-29] Added callsign and connect button to the bandmap. Fixed rxmarker not updateing.
@@ -346,14 +348,15 @@
 You can include a limited set of substitution instructions.
 
 - {MYCALL} Sends the station call.
 - {HISCALL} Send what's in the callsign field.
 - {SNT} Sends 5nn (cw) or 599 (ssb)
 - {SENTNR} Sends whats in the SentNR field.
 - {EXCH} Sends what's in the Sent Exchange field when contest is defined.
+- '#' Sends serial number.
 
 ### Macro use with voice
 
 The macros when used with voice, will also accept filenames of WAV files to play, excluding the file extension. The filename must be enclosed by brackets. For example `[CQ]` will play `cq.wav`, `[again]` will play `again.wav`. The wav files are stored in the operators personal data directory. The filenames must be in lowercase. See [Various data file locations](#various-data-file-locations) above for the location of your data files. For me, the macro `[cq]` will play `/home/mbridak/.local/share/not1mm/K6GTE/cq.wav`
 
 **The current wav files in place are not the ones you will want to use. They sound like an idiot.** You can use something like Audacity to record new wav files in your own voice.
```

### Comparing `not1mm-23.5.1.1/not1mm.egg-info/SOURCES.txt` & `not1mm-23.5.4/not1mm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1.1/pyproject.toml` & `not1mm-23.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "23.5.1.1"
+version = "23.5.4"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

### Comparing `not1mm-23.5.1.1/testing/test.py` & `not1mm-23.5.4/testing/test.py`

 * *Files identical despite different names*

