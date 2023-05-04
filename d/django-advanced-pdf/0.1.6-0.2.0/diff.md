# Comparing `tmp/django-advanced-pdf-0.1.6.tar.gz` & `tmp/django-advanced-pdf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-advanced-pdf-0.1.6.tar", last modified: Wed Mar 22 14:23:42 2023, max compression
+gzip compressed data, was "django-advanced-pdf-0.2.0.tar", last modified: Thu May  4 11:06:23 2023, max compression
```

## Comparing `django-advanced-pdf-0.1.6.tar` & `django-advanced-pdf-0.2.0.tar`

### file list

```diff
@@ -1,144 +1,149 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.178683 django-advanced-pdf-0.1.6/
--rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       83 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)      629 2023-03-22 14:23:42.178516 django-advanced-pdf-0.1.6/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      158 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.096886 django-advanced-pdf-0.1.6/django_advanced_pdf/
--rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:32.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/.DS_Store
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.103847 django-advanced-pdf-0.1.6/django_advanced_pdf/_trial_temp/
--rwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-20 15:07:58.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/_trial_temp/_trial_marker
--rw-r--r--   0 tom        (501) staff       (20)       41 2023-03-20 15:07:58.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/_trial_temp/test.log
--rw-r--r--   0 tom        (501) staff       (20)      223 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/admin.py
--rw-r--r--   0 tom        (501) staff       (20)      207 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/apps.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.107869 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.124490 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_paragraph/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_paragraph/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3083 2023-03-02 10:42:09.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_paragraph/enhanced_paragraph.py
--rw-r--r--   0 tom        (501) staff       (20)     2043 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_paragraph/parser.py
--rw-r--r--   0 tom        (501) staff       (20)     4197 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_paragraph/style.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.127978 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_table/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_table/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1281 2023-02-22 15:48:40.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_table/data.py
--rw-r--r--   0 tom        (501) staff       (20)     1413 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_table/data_paragraph.py
--rw-r--r--   0 tom        (501) staff       (20)    34502 2023-03-01 15:54:45.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_table/enhanced_tables.py
--rw-r--r--   0 tom        (501) staff       (20)      712 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/png_images.py
--rw-r--r--   0 tom        (501) staff       (20)    56388 2023-03-21 09:22:37.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/report_xml.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.134040 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/svglib/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/svglib/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    52517 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/svglib/svglib.py
--rw-r--r--   0 tom        (501) staff       (20)     7963 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/svglib/utils.py
--rw-r--r--   0 tom        (501) staff       (20)     9579 2023-02-22 15:48:40.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/engine/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.134809 django-advanced-pdf-0.1.6/django_advanced_pdf/migrations/
--rw-r--r--   0 tom        (501) staff       (20)      554 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1176 2023-02-22 15:48:40.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/models.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.136163 django-advanced-pdf-0.1.6/django_advanced_pdf/pagers/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/pagers/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     7756 2023-02-23 12:34:48.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/pagers/base.py
--rw-r--r--   0 tom        (501) staff       (20)     4973 2023-02-23 12:43:32.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/pagers/border.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.136560 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/
--rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:37.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/.DS_Store
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.137004 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/
--rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:37.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/.DS_Store
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.138649 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/abs2/
--rw-r--r--   0 tom        (501) staff       (20)   142408 2023-02-23 12:20:55.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/abs2/1.png
--rw-r--r--   0 tom        (501) staff       (20)   194803 2023-02-23 12:20:55.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/abs2/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:20:55.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/abs2/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.139207 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/abs3/
--rw-r--r--   0 tom        (501) staff       (20)    49895 2023-02-23 12:20:55.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/abs3/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:20:55.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/abs3/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.139977 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/background_colour/
--rw-r--r--   0 tom        (501) staff       (20)    32702 2023-02-23 12:19:01.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/background_colour/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:19:01.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/background_colour/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.140832 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/basic/
--rw-r--r--   0 tom        (501) staff       (20)   142700 2023-02-23 11:51:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/basic/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 11:51:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/basic/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.141682 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/border/
--rw-r--r--   0 tom        (501) staff       (20)    86430 2023-02-23 12:28:02.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/border/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:28:02.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/border/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.143680 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/change_header/
--rw-r--r--   0 tom        (501) staff       (20)   116046 2023-02-23 11:51:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/change_header/1.png
--rw-r--r--   0 tom        (501) staff       (20)   135419 2023-02-23 11:51:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/change_header/2.png
--rw-r--r--   0 tom        (501) staff       (20)   133527 2023-02-23 11:51:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/change_header/3.png
--rw-r--r--   0 tom        (501) staff       (20)    67070 2023-02-23 11:51:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/change_header/4.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 11:51:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/change_header/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.145362 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/hidden/
--rw-r--r--   0 tom        (501) staff       (20)   142804 2023-03-14 12:55:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/hidden/1.png
--rw-r--r--   0 tom        (501) staff       (20)   129438 2023-03-14 12:55:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/hidden/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-06 08:57:48.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/hidden/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.149811 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/
--rw-r--r--   0 tom        (501) staff       (20)   101102 2023-02-23 10:44:40.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/1.png
--rw-r--r--   0 tom        (501) staff       (20)   131206 2023-02-23 10:44:40.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/2.png
--rw-r--r--   0 tom        (501) staff       (20)   123455 2023-02-23 10:44:40.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/3.png
--rw-r--r--   0 tom        (501) staff       (20)   147016 2023-02-23 10:44:40.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/4.png
--rw-r--r--   0 tom        (501) staff       (20)   154909 2023-02-23 10:44:40.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/5.png
--rw-r--r--   0 tom        (501) staff       (20)   164056 2023-02-23 10:44:41.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/6.png
--rw-r--r--   0 tom        (501) staff       (20)   171134 2023-02-23 10:44:41.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/7.png
--rw-r--r--   0 tom        (501) staff       (20)   100782 2023-02-23 10:44:41.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/8.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 10:44:41.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.152242 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/overflow_gt_height/
--rw-r--r--   0 tom        (501) staff       (20)   752024 2023-03-02 10:39:31.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/overflow_gt_height/1.png
--rw-r--r--   0 tom        (501) staff       (20)   473318 2023-03-02 10:39:31.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/overflow_gt_height/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-02 10:39:31.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/overflow_gt_height/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.155200 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/
--rw-r--r--   0 tom        (501) staff       (20)     8996 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/abs2.xml
--rw-r--r--   0 tom        (501) staff       (20)      746 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/abs3.xml
--rw-r--r--   0 tom        (501) staff       (20)      203 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/background_colour.xml
--rw-r--r--   0 tom        (501) staff       (20)    49397 2023-02-22 15:48:40.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/basic.xml
--rw-r--r--   0 tom        (501) staff       (20)     1327 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/border.xml
--rw-r--r--   0 tom        (501) staff       (20)     7790 2023-02-22 15:48:40.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/change_header.xml
--rw-r--r--   0 tom        (501) staff       (20)     4192 2023-03-14 12:55:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/hidden.xml
--rw-r--r--   0 tom        (501) staff       (20)    12752 2023-02-23 11:40:06.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/keep_with_next.xml
--rw-r--r--   0 tom        (501) staff       (20)     7691 2023-03-02 10:18:57.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/overflow_gt_height.xml
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.091773 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.156917 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/abs2/
--rw-r--r--   0 tom        (501) staff       (20)   142408 2023-03-20 15:07:58.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/abs2/1.png
--rw-r--r--   0 tom        (501) staff       (20)   194803 2023-03-20 15:07:58.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/abs2/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:07:58.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/abs2/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.157889 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/abs3/
--rw-r--r--   0 tom        (501) staff       (20)    49895 2023-03-20 15:07:59.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/abs3/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:07:59.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/abs3/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.158486 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/background_colour/
--rw-r--r--   0 tom        (501) staff       (20)    32702 2023-03-20 15:07:59.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/background_colour/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:07:59.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/background_colour/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.159177 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/basic/
--rw-r--r--   0 tom        (501) staff       (20)   142700 2023-03-20 15:08:00.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/basic/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:00.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/basic/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.159731 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/border/
--rw-r--r--   0 tom        (501) staff       (20)    86430 2023-03-20 15:08:00.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/border/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:00.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/border/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.162435 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/change_header/
--rw-r--r--   0 tom        (501) staff       (20)   116046 2023-03-20 15:08:00.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/change_header/1.png
--rw-r--r--   0 tom        (501) staff       (20)   135419 2023-03-20 15:08:01.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/change_header/2.png
--rw-r--r--   0 tom        (501) staff       (20)   133527 2023-03-20 15:08:01.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/change_header/3.png
--rw-r--r--   0 tom        (501) staff       (20)    67070 2023-03-20 15:08:01.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/change_header/4.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:01.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/change_header/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.167300 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/hidden/
--rw-r--r--   0 tom        (501) staff       (20)   142804 2023-03-20 15:08:01.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/hidden/1.png
--rw-r--r--   0 tom        (501) staff       (20)   129438 2023-03-20 15:08:01.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/hidden/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:01.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/hidden/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.171931 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/
--rw-r--r--   0 tom        (501) staff       (20)   101102 2023-03-20 15:08:02.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/1.png
--rw-r--r--   0 tom        (501) staff       (20)   131206 2023-03-20 15:08:02.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/2.png
--rw-r--r--   0 tom        (501) staff       (20)   123455 2023-03-20 15:08:02.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/3.png
--rw-r--r--   0 tom        (501) staff       (20)   147016 2023-03-20 15:08:02.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/4.png
--rw-r--r--   0 tom        (501) staff       (20)   154909 2023-03-20 15:08:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/5.png
--rw-r--r--   0 tom        (501) staff       (20)   164056 2023-03-20 15:08:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/6.png
--rw-r--r--   0 tom        (501) staff       (20)   171134 2023-03-20 15:08:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/7.png
--rw-r--r--   0 tom        (501) staff       (20)   100782 2023-03-20 15:08:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/8.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:03.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.178138 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/overflow_gt_height/
--rw-r--r--   0 tom        (501) staff       (20)   752024 2023-03-20 15:08:05.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/overflow_gt_height/1.png
--rw-r--r--   0 tom        (501) staff       (20)   473318 2023-03-20 15:08:05.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/overflow_gt_height/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:05.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/overflow_gt_height/page_count.txt
--rw-r--r--   0 tom        (501) staff       (20)     4852 2023-03-06 08:57:48.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/tests.py
--rw-r--r--   0 tom        (501) staff       (20)      498 2023-01-16 11:14:24.000000 django-advanced-pdf-0.1.6/django_advanced_pdf/views.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-22 14:23:42.101754 django-advanced-pdf-0.1.6/django_advanced_pdf.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      629 2023-03-22 14:23:42.000000 django-advanced-pdf-0.1.6/django_advanced_pdf.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     5460 2023-03-22 14:23:42.000000 django-advanced-pdf-0.1.6/django_advanced_pdf.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-22 14:23:42.000000 django-advanced-pdf-0.1.6/django_advanced_pdf.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       20 2023-03-22 14:23:42.000000 django-advanced-pdf-0.1.6/django_advanced_pdf.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-03-22 14:23:42.178733 django-advanced-pdf-0.1.6/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      672 2023-03-22 14:22:44.000000 django-advanced-pdf-0.1.6/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.930203 django-advanced-pdf-0.2.0/
+-rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       83 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)      629 2023-05-04 11:06:23.929982 django-advanced-pdf-0.2.0/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      158 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.779524 django-advanced-pdf-0.2.0/django_advanced_pdf/
+-rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:32.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/.DS_Store
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.804060 django-advanced-pdf-0.2.0/django_advanced_pdf/_trial_temp/
+-rwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/_trial_temp/_trial_marker
+-rw-r--r--   0 tom        (501) staff       (20)       41 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/_trial_temp/test.log
+-rw-r--r--   0 tom        (501) staff       (20)      223 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)      207 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/apps.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.836642 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.839134 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_paragraph/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_paragraph/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3083 2023-03-02 10:42:09.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_paragraph/enhanced_paragraph.py
+-rw-r--r--   0 tom        (501) staff       (20)     2043 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_paragraph/parser.py
+-rw-r--r--   0 tom        (501) staff       (20)     4197 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_paragraph/style.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.841401 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_table/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_table/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1281 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_table/data.py
+-rw-r--r--   0 tom        (501) staff       (20)     1413 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_table/data_paragraph.py
+-rw-r--r--   0 tom        (501) staff       (20)    34502 2023-03-01 15:54:45.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_table/enhanced_tables.py
+-rw-r--r--   0 tom        (501) staff       (20)      712 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/png_images.py
+-rw-r--r--   0 tom        (501) staff       (20)    56762 2023-05-03 10:20:01.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/report_xml.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.848254 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/svglib/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/svglib/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    52517 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/svglib/svglib.py
+-rw-r--r--   0 tom        (501) staff       (20)     7963 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/svglib/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     9579 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/engine/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.849842 django-advanced-pdf-0.2.0/django_advanced_pdf/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)      554 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1176 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/models.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.851942 django-advanced-pdf-0.2.0/django_advanced_pdf/pagers/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/pagers/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     7952 2023-05-03 09:14:16.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/pagers/base.py
+-rw-r--r--   0 tom        (501) staff       (20)     5049 2023-05-03 09:07:57.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/pagers/border.py
+-rw-r--r--   0 tom        (501) staff       (20)     1999 2023-05-04 10:45:49.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/tasks.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.852688 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/
+-rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:37.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/.DS_Store
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.853505 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/
+-rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:37.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/.DS_Store
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.855805 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/abs2/
+-rw-r--r--   0 tom        (501) staff       (20)   142408 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/abs2/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   194803 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/abs2/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/abs2/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.856819 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/abs3/
+-rw-r--r--   0 tom        (501) staff       (20)    49895 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/abs3/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/abs3/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.858071 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/background_colour/
+-rw-r--r--   0 tom        (501) staff       (20)    32702 2023-02-23 12:19:01.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/background_colour/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:19:01.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/background_colour/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.862938 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/basic/
+-rw-r--r--   0 tom        (501) staff       (20)   142700 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/basic/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/basic/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.864302 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/border/
+-rw-r--r--   0 tom        (501) staff       (20)    86430 2023-02-23 12:28:02.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/border/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:28:02.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/border/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.869654 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/change_header/
+-rw-r--r--   0 tom        (501) staff       (20)   116046 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/change_header/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   135419 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/change_header/2.png
+-rw-r--r--   0 tom        (501) staff       (20)   133527 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/change_header/3.png
+-rw-r--r--   0 tom        (501) staff       (20)    67070 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/change_header/4.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/change_header/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.872637 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/hidden/
+-rw-r--r--   0 tom        (501) staff       (20)   142804 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/hidden/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   129438 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/hidden/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-06 08:57:48.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/hidden/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.881962 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/
+-rw-r--r--   0 tom        (501) staff       (20)   101102 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   131206 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/2.png
+-rw-r--r--   0 tom        (501) staff       (20)   123455 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/3.png
+-rw-r--r--   0 tom        (501) staff       (20)   147016 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/4.png
+-rw-r--r--   0 tom        (501) staff       (20)   154909 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/5.png
+-rw-r--r--   0 tom        (501) staff       (20)   164056 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/6.png
+-rw-r--r--   0 tom        (501) staff       (20)   171134 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/7.png
+-rw-r--r--   0 tom        (501) staff       (20)   100782 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/8.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.886059 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/overflow_gt_height/
+-rw-r--r--   0 tom        (501) staff       (20)   752024 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/overflow_gt_height/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   473318 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/overflow_gt_height/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/overflow_gt_height/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.894762 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/
+-rw-r--r--   0 tom        (501) staff       (20)     8996 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/abs2.xml
+-rw-r--r--   0 tom        (501) staff       (20)      746 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/abs3.xml
+-rw-r--r--   0 tom        (501) staff       (20)      203 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/background_colour.xml
+-rw-r--r--   0 tom        (501) staff       (20)    49397 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/basic.xml
+-rw-r--r--   0 tom        (501) staff       (20)     1327 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/border.xml
+-rw-r--r--   0 tom        (501) staff       (20)     7790 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/change_header.xml
+-rw-r--r--   0 tom        (501) staff       (20)     4192 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/hidden.xml
+-rw-r--r--   0 tom        (501) staff       (20)    12752 2023-02-23 11:40:06.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/keep_with_next.xml
+-rw-r--r--   0 tom        (501) staff       (20)     7691 2023-03-02 10:18:57.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/overflow_gt_height.xml
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.765811 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.897365 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/abs2/
+-rw-r--r--   0 tom        (501) staff       (20)   142408 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/abs2/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   194803 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/abs2/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/abs2/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.898708 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/abs3/
+-rw-r--r--   0 tom        (501) staff       (20)    49895 2023-03-20 15:07:59.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/abs3/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:07:59.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/abs3/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.900155 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/background_colour/
+-rw-r--r--   0 tom        (501) staff       (20)    32702 2023-03-20 15:07:59.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/background_colour/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:07:59.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/background_colour/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.901565 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/basic/
+-rw-r--r--   0 tom        (501) staff       (20)   142700 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/basic/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/basic/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.904031 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/border/
+-rw-r--r--   0 tom        (501) staff       (20)    86430 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/border/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/border/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.907265 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/change_header/
+-rw-r--r--   0 tom        (501) staff       (20)   116046 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/change_header/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   135419 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/change_header/2.png
+-rw-r--r--   0 tom        (501) staff       (20)   133527 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/change_header/3.png
+-rw-r--r--   0 tom        (501) staff       (20)    67070 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/change_header/4.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/change_header/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.912157 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/hidden/
+-rw-r--r--   0 tom        (501) staff       (20)   142804 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/hidden/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   129438 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/hidden/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/hidden/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.920591 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/
+-rw-r--r--   0 tom        (501) staff       (20)   101102 2023-03-20 15:08:02.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   131206 2023-03-20 15:08:02.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/2.png
+-rw-r--r--   0 tom        (501) staff       (20)   123455 2023-03-20 15:08:02.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/3.png
+-rw-r--r--   0 tom        (501) staff       (20)   147016 2023-03-20 15:08:02.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/4.png
+-rw-r--r--   0 tom        (501) staff       (20)   154909 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/5.png
+-rw-r--r--   0 tom        (501) staff       (20)   164056 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/6.png
+-rw-r--r--   0 tom        (501) staff       (20)   171134 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/7.png
+-rw-r--r--   0 tom        (501) staff       (20)   100782 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/8.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.927765 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/overflow_gt_height/
+-rw-r--r--   0 tom        (501) staff       (20)   752024 2023-03-20 15:08:05.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/overflow_gt_height/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   473318 2023-03-20 15:08:05.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/overflow_gt_height/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:05.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/overflow_gt_height/page_count.txt
+-rw-r--r--   0 tom        (501) staff       (20)     4852 2023-03-06 08:57:48.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/tests.py
+-rw-r--r--   0 tom        (501) staff       (20)      336 2023-05-04 10:30:08.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/urls.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.929212 django-advanced-pdf-0.2.0/django_advanced_pdf/views/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-05-03 10:37:37.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/views/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      499 2023-05-04 09:14:22.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/views/standard.py
+-rw-r--r--   0 tom        (501) staff       (20)     1387 2023-05-04 10:54:47.000000 django-advanced-pdf-0.2.0/django_advanced_pdf/views/tasks.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 11:06:23.800280 django-advanced-pdf-0.2.0/django_advanced_pdf.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      629 2023-05-04 11:06:23.000000 django-advanced-pdf-0.2.0/django_advanced_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     5599 2023-05-04 11:06:23.000000 django-advanced-pdf-0.2.0/django_advanced_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-04 11:06:23.000000 django-advanced-pdf-0.2.0/django_advanced_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)       20 2023-05-04 11:06:23.000000 django-advanced-pdf-0.2.0/django_advanced_pdf.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-05-04 11:06:23.930263 django-advanced-pdf-0.2.0/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      672 2023-05-04 10:59:34.000000 django-advanced-pdf-0.2.0/setup.py
```

### Comparing `django-advanced-pdf-0.1.6/LICENSE` & `django-advanced-pdf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/PKG-INFO` & `django-advanced-pdf-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-pdf
-Version: 0.1.6
+Version: 0.2.0
 Summary: Django app that helps one create pdf
 Home-page: https://github.com/django-advance-utils/django-advanced-pdf
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/.DS_Store` & `django-advanced-pdf-0.2.0/django_advanced_pdf/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_paragraph/enhanced_paragraph.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_paragraph/enhanced_paragraph.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_paragraph/parser.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_paragraph/parser.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_paragraph/style.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_paragraph/style.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_table/data.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_table/data.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_table/data_paragraph.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_table/data_paragraph.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/engine/enhanced_table/enhanced_tables.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/engine/enhanced_table/enhanced_tables.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/engine/png_images.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/engine/png_images.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/engine/report_xml.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/engine/report_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import copy
 import re
 from io import StringIO, BytesIO
+from time import sleep
 
 from lxml import etree
 from reportlab.lib.colors import HexColor, black
 from reportlab.lib.units import mm
 from reportlab.platypus import TableStyle, PageBreak, Spacer, Table
 
 from .enhanced_paragraph.enhanced_paragraph import EnhancedParagraph
@@ -54,15 +55,15 @@
         (u'sup3', u'³'),
         (u'frac14', u'¼'),
         (u'frac12', u'½'),
         (u'frac34', u'¾'),
         (u'rsquo', u'’'),
     ]
 
-    def __init__(self, object_lookup=None, pager_kwargs=None, test_mode=False):
+    def __init__(self, object_lookup=None, pager_kwargs=None, test_mode=False, status_method=None):
         self.styles = {}
         if object_lookup is not None:
             self.object_lookup = object_lookup
         else:
             self.object_lookup = {}
         self.background_image_first = None
         self.background_image_remaining = None
@@ -75,27 +76,29 @@
         self.border_bottom_first = 0
         self.border_left_continuation = 0
         self.border_right_continuation = 0
         self.border_top_continuation = 0
         self.border_bottom_continuation = 0
         self.page_style = None
         self.test_mode = test_mode
+        self.status_method = status_method
 
         if pager_kwargs is None:
             self.pager_kwargs = {}
         else:
             self.pager_kwargs = pager_kwargs
 
     def load_xml_and_make_pdf(self, xml, add_doctype=True, background_image_first=None,
                               background_image_remaining=None, background_image_footer=None):
 
         self.background_image_first = background_image_first
         self.background_image_remaining = background_image_remaining
         self.background_image_footer = background_image_footer
 
+        self.update_status("Loading")
         parser = etree.XMLParser(remove_blank_text=True, resolve_entities=False)
 
         if add_doctype:
             xml = self.get_doc_type() + xml
         tree = etree.parse(StringIO(xml), parser)
         root = tree.getroot()
         result = BytesIO()
@@ -176,14 +179,15 @@
                               border_right_continuation=self.border_right_continuation * mm,
                               border_top_continuation=self.border_top_continuation * mm,
                               border_bottom_continuation=self.border_bottom_continuation * mm,
                               background_image_first=self.background_image_first,
                               background_image_remaining=self.background_image_remaining,
                               background_image_footer=self.background_image_footer,
                               test_mode=self.test_mode,
+                              status_method=self.update_status,
                               **self.pager_kwargs)
 
     def canvasmaker(self, *args, **kwargs):
         return self.get_pager(*args,
                               footer_field='',
                               border_left_first=self.border_left_first * mm,
                               border_right_first=self.border_right_first * mm,
@@ -193,14 +197,15 @@
                               border_right_continuation=self.border_right_continuation * mm,
                               border_top_continuation=self.border_top_continuation * mm,
                               border_bottom_continuation=self.border_bottom_continuation * mm,
                               background_image_first=self.background_image_first,
                               background_image_remaining=self.background_image_remaining,
                               background_image_footer=self.background_image_footer,
                               test_mode=self.test_mode,
+                              status_method=self.update_status,
                               **self.pager_kwargs,
                               **kwargs)
 
     def process_xml(self, root_element, story, page_width, page_height, top_border, bottom_border):
         self.styles = {}
         children = root_element.getchildren()
 
@@ -1205,7 +1210,11 @@
             rows_variables.append(rows_variables[-1])
 
         return len(overflow_rows_xml)
 
     # noinspection PyMethodMayBeStatic
     def get_boolean_value(self, value):
         return value in ['1', 'True', 'yes']
+
+    def update_status(self, message):
+        if self.status_method is not None:
+            self.status_method(message)
```

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/engine/svglib/svglib.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/engine/svglib/svglib.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/engine/svglib/utils.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/engine/svglib/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/engine/utils.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/engine/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/migrations/0001_initial.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/models.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/models.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/pagers/base.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/pagers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,17 @@
                  encrypt=None, crop_marks=None, pdf_version=None, enforce_color_space=None,
                  border_left_first=0, border_right_first=0,
                  border_top_first=0, border_bottom_first=0,
                  border_left_continuation=0, border_right_continuation=0,
                  border_top_continuation=0, border_bottom_continuation=0,
                  program_name=None,
                  background_image_first=None, background_image_remaining=None,
-                 background_image_footer=None, test_mode=False, **kwargs):
+                 background_image_footer=None, test_mode=False, status_method=None, **kwargs):
 
+        self.status_method = status_method
         self.heading = heading
         self.pagesize = pagesize
         self.drawmethods = []
         self.image2 = None
         self._saved_page_states = []
         self.test_mode = test_mode
 
@@ -176,14 +177,16 @@
         have been added to the derived class.
         """
 
         num_pages = len(self._saved_page_states)
 
         for state in self._saved_page_states:
             self.__dict__.update(state)
+            if self.status_method is not None:
+                self.status_method(f'Processing page {self._pageNumber}/{num_pages}')
             self.draw_footer_image_block()
             self.draw_page_number(num_pages)
             canvas.Canvas.showPage(self)
 
         canvas.Canvas.save(self)
 
     def draw_background(self, image):
```

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/pagers/border.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/pagers/border.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 from django_advanced_pdf.engine.utils import GREYFILL_COLOUR, BLACK_COLOUR
 from django_advanced_pdf.pagers.base import BasePager
 
 
 class BorderPager(BasePager):
     def __init__(self, heading, filename, footer_field=None, pagesize=None, bottom_up=1, page_compression=None,
                  invariant=None, verbosity=0, encrypt=None, crop_marks=None, pdf_version=None, enforce_color_space=None,
-                 bottom_text=None, test_mode=False, **kwargs):
+                 bottom_text=None, test_mode=False, status_method=None, **kwargs):
         BasePager.__init__(self, heading=heading, filename=filename, pagesize=pagesize,
                            bottom_up=bottom_up, page_compression=page_compression,
                            invariant=invariant, verbosity=verbosity, encryp=encrypt,
                            crop_marks=crop_marks, pdf_version=pdf_version,
                            enforce_color_space=enforce_color_space, test_mode=test_mode,
+                           status_method=status_method,
                            **kwargs)
 
         self._saved_page_states = []
         self.bottom_text = bottom_text
 
         self.set_page_used(top=self.page_height() - (self.border_top() - 5 * mm),
                            bottom=(self.border_bottom() + 7 * mm),
```

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/.DS_Store` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/.DS_Store` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/abs2/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/abs2/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/abs2/2.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/abs2/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/abs3/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/abs3/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/background_colour/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/background_colour/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/basic/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/basic/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/border/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/border/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/change_header/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/change_header/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/change_header/2.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/change_header/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/change_header/3.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/change_header/3.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/change_header/4.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/change_header/4.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/hidden/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/hidden/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/hidden/2.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/hidden/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/2.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/3.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/3.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/4.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/4.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/5.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/5.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/6.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/6.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/7.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/7.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/keep_with_next/8.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/keep_with_next/8.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/overflow_gt_height/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/overflow_gt_height/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/held/overflow_gt_height/2.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/held/overflow_gt_height/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/abs2.xml` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/abs2.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/abs3.xml` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/abs3.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/basic.xml` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/basic.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/border.xml` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/border.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/change_header.xml` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/change_header.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/hidden.xml` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/hidden.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/keep_with_next.xml` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/keep_with_next.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/reports/overflow_gt_height.xml` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/reports/overflow_gt_height.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/abs2/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/abs2/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/abs2/2.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/abs2/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/abs3/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/abs3/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/background_colour/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/background_colour/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/basic/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/basic/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/border/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/border/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/change_header/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/change_header/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/change_header/2.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/change_header/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/change_header/3.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/change_header/3.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/change_header/4.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/change_header/4.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/hidden/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/hidden/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/hidden/2.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/hidden/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/2.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/3.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/3.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/4.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/4.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/5.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/5.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/6.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/6.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/7.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/7.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/keep_with_next/8.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/keep_with_next/8.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/overflow_gt_height/1.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/overflow_gt_height/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/test_data/temp/overflow_gt_height/2.png` & `django-advanced-pdf-0.2.0/django_advanced_pdf/test_data/temp/overflow_gt_height/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf/tests.py` & `django-advanced-pdf-0.2.0/django_advanced_pdf/tests.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf.egg-info/PKG-INFO` & `django-advanced-pdf-0.2.0/django_advanced_pdf.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-pdf
-Version: 0.1.6
+Version: 0.2.0
 Summary: Django app that helps one create pdf
 Home-page: https://github.com/django-advance-utils/django-advanced-pdf
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-pdf-0.1.6/django_advanced_pdf.egg-info/SOURCES.txt` & `django-advanced-pdf-0.2.0/django_advanced_pdf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 README.md
 setup.py
 django_advanced_pdf/.DS_Store
 django_advanced_pdf/__init__.py
 django_advanced_pdf/admin.py
 django_advanced_pdf/apps.py
 django_advanced_pdf/models.py
+django_advanced_pdf/tasks.py
 django_advanced_pdf/tests.py
-django_advanced_pdf/views.py
+django_advanced_pdf/urls.py
 django_advanced_pdf.egg-info/PKG-INFO
 django_advanced_pdf.egg-info/SOURCES.txt
 django_advanced_pdf.egg-info/dependency_links.txt
 django_advanced_pdf.egg-info/top_level.txt
 django_advanced_pdf/_trial_temp/_trial_marker
 django_advanced_pdf/_trial_temp/test.log
 django_advanced_pdf/engine/__init__.py
@@ -103,8 +104,11 @@
 django_advanced_pdf/test_data/temp/keep_with_next/5.png
 django_advanced_pdf/test_data/temp/keep_with_next/6.png
 django_advanced_pdf/test_data/temp/keep_with_next/7.png
 django_advanced_pdf/test_data/temp/keep_with_next/8.png
 django_advanced_pdf/test_data/temp/keep_with_next/page_count.txt
 django_advanced_pdf/test_data/temp/overflow_gt_height/1.png
 django_advanced_pdf/test_data/temp/overflow_gt_height/2.png
-django_advanced_pdf/test_data/temp/overflow_gt_height/page_count.txt
+django_advanced_pdf/test_data/temp/overflow_gt_height/page_count.txt
+django_advanced_pdf/views/__init__.py
+django_advanced_pdf/views/standard.py
+django_advanced_pdf/views/tasks.py
```

### Comparing `django-advanced-pdf-0.1.6/setup.py` & `django-advanced-pdf-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-advanced-pdf",
-    version="0.1.6",
+    version="0.2.0",
     author="Thomas Turner",
     description="Django app that helps one create pdf",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/django-advanced-pdf",
     include_package_data=True,
     packages=['django_advanced_pdf'],
```

