# Comparing `tmp/django-taggit-3.1.0.tar.gz` & `tmp/django-taggit-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-taggit-3.1.0.tar", last modified: Fri Nov 18 04:56:53 2022, max compression
+gzip compressed data, was "django-taggit-4.0.0.tar", last modified: Thu May  4 02:12:21 2023, max compression
```

## Comparing `django-taggit-3.1.0.tar` & `django-taggit-4.0.0.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.237284 django-taggit-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-11-18 04:56:41.000000 django-taggit-3.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)    12895 2022-11-18 04:56:41.000000 django-taggit-3.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-11-18 04:56:41.000000 django-taggit-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-11-18 04:56:41.000000 django-taggit-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3472 2022-11-18 04:56:53.237284 django-taggit-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-11-18 04:56:41.000000 django-taggit-3.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.229283 django-taggit-3.1.0/django_taggit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3472 2022-11-18 04:56:53.000000 django-taggit-3.1.0/django_taggit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-11-18 04:56:53.000000 django-taggit-3.1.0/django_taggit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 04:56:53.000000 django-taggit-3.1.0/django_taggit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 04:56:53.000000 django-taggit-3.1.0/django_taggit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-18 04:56:53.000000 django-taggit-3.1.0/django_taggit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-18 04:56:53.000000 django-taggit-3.1.0/django_taggit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.229283 django-taggit-3.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-11-18 04:56:41.000000 django-taggit-3.1.0/docs/admin.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4396 2022-11-18 04:56:41.000000 django-taggit-3.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-18 04:56:41.000000 django-taggit-3.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-11-18 04:56:41.000000 django-taggit-3.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-18 04:56:41.000000 django-taggit-3.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8350 2022-11-18 04:56:41.000000 django-taggit-3.1.0/docs/custom_tagging.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2092 2022-11-18 04:56:41.000000 django-taggit-3.1.0/docs/external_apps.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-11-18 04:56:41.000000 django-taggit-3.1.0/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2378 2022-11-18 04:56:41.000000 django-taggit-3.1.0/docs/forms.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-11-18 04:56:41.000000 django-taggit-3.1.0/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-11-18 04:56:41.000000 django-taggit-3.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-11-18 04:56:41.000000 django-taggit-3.1.0/docs/serializers.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-11-18 04:56:53.241284 django-taggit-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-18 04:56:41.000000 django-taggit-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.229283 django-taggit-3.1.0/taggit/
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.229283 django-taggit-3.1.0/taggit/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.229283 django-taggit-3.1.0/taggit/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/eo/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/eo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2162 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1928 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2073 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1904 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2144 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/taggit/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.233283 django-taggit-3.1.0/taggit/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)    25337 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.237284 django-taggit-3.1.0/taggit/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/migrations/0002_auto_20150616_2121.py
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/migrations/0003_taggeditem_add_unique_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/migrations/0004_alter_taggeditem_content_type_alter_taggeditem_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/migrations/0005_auto_20220424_2025.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6041 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4382 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4295 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-11-18 04:56:41.000000 django-taggit-3.1.0/taggit/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.237284 django-taggit-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/custom_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.237284 django-taggit-3.1.0/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    39439 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/migrations/0002_auto_20200214_1129.py
--rw-r--r--   0 runner    (1001) docker     (121)     2995 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/migrations/0003_auto_20210310_0918.py
--rw-r--r--   0 runner    (1001) docker     (121)     4420 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/migrations/0004_auto_20210619_0826.py
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/migrations/0005_auto_20210713_2301.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10007 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.225283 django-taggit-3.1.0/tests/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 04:56:53.237284 django-taggit-3.1.0/tests/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/templates/tests/food_tag_list.html
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3357 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    48472 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-11-18 04:56:41.000000 django-taggit-3.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.831687 django-taggit-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-04 02:12:10.000000 django-taggit-4.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-05-04 02:12:10.000000 django-taggit-4.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-04 02:12:10.000000 django-taggit-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-04 02:12:10.000000 django-taggit-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-04 02:12:21.831687 django-taggit-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-04 02:12:10.000000 django-taggit-4.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.819687 django-taggit-4.0.0/django_taggit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-04 02:12:21.000000 django-taggit-4.0.0/django_taggit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-04 02:12:21.000000 django-taggit-4.0.0/django_taggit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 02:12:21.000000 django-taggit-4.0.0/django_taggit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 02:12:21.000000 django-taggit-4.0.0/django_taggit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 02:12:21.000000 django-taggit-4.0.0/django_taggit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 02:12:21.000000 django-taggit-4.0.0/django_taggit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.819687 django-taggit-4.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-04 02:12:10.000000 django-taggit-4.0.0/docs/admin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-04 02:12:10.000000 django-taggit-4.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 02:12:10.000000 django-taggit-4.0.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-04 02:12:10.000000 django-taggit-4.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 02:12:10.000000 django-taggit-4.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-04 02:12:10.000000 django-taggit-4.0.0/docs/custom_tagging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-04 02:12:10.000000 django-taggit-4.0.0/docs/external_apps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-04 02:12:10.000000 django-taggit-4.0.0/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-04 02:12:10.000000 django-taggit-4.0.0/docs/forms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-04 02:12:10.000000 django-taggit-4.0.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-04 02:12:10.000000 django-taggit-4.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-04 02:12:10.000000 django-taggit-4.0.0/docs/serializers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-04 02:12:21.831687 django-taggit-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 02:12:10.000000 django-taggit-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.823687 django-taggit-4.0.0/taggit/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.823687 django-taggit-4.0.0/taggit/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.823687 django-taggit-4.0.0/taggit/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.823687 django-taggit-4.0.0/taggit/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.823687 django-taggit-4.0.0/taggit/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.823687 django-taggit-4.0.0/taggit/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.823687 django-taggit-4.0.0/taggit/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.823687 django-taggit-4.0.0/taggit/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/eo/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/eo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.823687 django-taggit-4.0.0/taggit/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.823687 django-taggit-4.0.0/taggit/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.823687 django-taggit-4.0.0/taggit/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.823687 django-taggit-4.0.0/taggit/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.827687 django-taggit-4.0.0/taggit/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.827687 django-taggit-4.0.0/taggit/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.827687 django-taggit-4.0.0/taggit/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.827687 django-taggit-4.0.0/taggit/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.827687 django-taggit-4.0.0/taggit/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.827687 django-taggit-4.0.0/taggit/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.827687 django-taggit-4.0.0/taggit/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.827687 django-taggit-4.0.0/taggit/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.827687 django-taggit-4.0.0/taggit/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.815687 django-taggit-4.0.0/taggit/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.827687 django-taggit-4.0.0/taggit/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)    26195 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.827687 django-taggit-4.0.0/taggit/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/migrations/0002_auto_20150616_2121.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/migrations/0003_taggeditem_add_unique_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/migrations/0004_alter_taggeditem_content_type_alter_taggeditem_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/migrations/0005_auto_20220424_2025.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-04 02:12:10.000000 django-taggit-4.0.0/taggit/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.831687 django-taggit-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/custom_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.831687 django-taggit-4.0.0/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    39438 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/migrations/0002_auto_20200214_1129.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/migrations/0003_auto_20210310_0918.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/migrations/0004_auto_20210619_0826.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/migrations/0005_auto_20210713_2301.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.819687 django-taggit-4.0.0/tests/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:12:21.831687 django-taggit-4.0.0/tests/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/templates/tests/food_tag_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51080 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 02:12:10.000000 django-taggit-4.0.0/tox.ini
```

### Comparing `django-taggit-3.1.0/AUTHORS` & `django-taggit-4.0.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/CHANGELOG.rst` & `django-taggit-4.0.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 =========
 
 (Unreleased)
 ~~~~~~~~~~~~
 
+4.0.0 (2023-05-04)
+~~~~~~~~~~~~~~~~~~
+* Remove Python 3.6 support (no code changes occurred, but we no longer test this release).
+* Remove Django 4.0 support (no code changes occurred, but we no longer test this release).
+* Add Django 4.2 support.
+
 3.1.0 (2022-11-08)
 ~~~~~~~~~~~~~~~~~~
 
 * Add Python 3.11 support (no code changes were needed, but now we test this release).
 * Add Django 4.1 support (no code changes were needed, but now we test this release).
 * Fixed an issue where object caches would not be properly cleared after updating tags, leading
   to stale reads in cases where ``prefetch_related`` is used.
```

### Comparing `django-taggit-3.1.0/LICENSE` & `django-taggit-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/PKG-INFO` & `django-taggit-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-taggit
-Version: 3.1.0
+Version: 4.0.0
 Summary: django-taggit is a reusable Django application for simple tagging.
 Home-page: https://github.com/jazzband/django-taggit
 Author: Alex Gaynor
 Author-email: alex.gaynor@gmail.com
 License: BSD
 Project-URL: Documentation, https://django-taggit.readthedocs.io
 Project-URL: Source, https://github.com/jazzband/django-taggit
```

### Comparing `django-taggit-3.1.0/README.rst` & `django-taggit-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/django_taggit.egg-info/PKG-INFO` & `django-taggit-4.0.0/django_taggit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-taggit
-Version: 3.1.0
+Version: 4.0.0
 Summary: django-taggit is a reusable Django application for simple tagging.
 Home-page: https://github.com/jazzband/django-taggit
 Author: Alex Gaynor
 Author-email: alex.gaynor@gmail.com
 License: BSD
 Project-URL: Documentation, https://django-taggit.readthedocs.io
 Project-URL: Source, https://github.com/jazzband/django-taggit
```

### Comparing `django-taggit-3.1.0/django_taggit.egg-info/SOURCES.txt` & `django-taggit-4.0.0/django_taggit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/docs/admin.rst` & `django-taggit-4.0.0/docs/admin.rst`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/docs/api.rst` & `django-taggit-4.0.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/docs/custom_tagging.rst` & `django-taggit-4.0.0/docs/custom_tagging.rst`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/docs/external_apps.rst` & `django-taggit-4.0.0/docs/external_apps.rst`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/docs/faq.rst` & `django-taggit-4.0.0/docs/faq.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 - How can I get all my tags?
 
  If you are using just an out-of-the-box setup, your tags are stored in the `Tag` model (found in `taggit.models`). If this is a custom model (for example you have your own models derived from `ItemBase`), then you'll need to query that one instead.
 
  So if you are using the standard setup, ``Tag.objects.all()`` will give you the tags.
 
- - How can I use this with factory_boy?
+- How can I use this with factory_boy?
 
  Since these are all built off of many-to-many relationships, you can check out `factory_boy's documentation on this topic <https://factoryboy.readthedocs.io/en/stable/recipes.html#simple-many-to-many-relationship>`_ and get some ideas on how to deal with tags.
 
 
  One way to handle this is with post-generation hooks::
 
    class ProductFactory(DjangoModelFactory):
```

### Comparing `django-taggit-3.1.0/docs/forms.rst` & `django-taggit-4.0.0/docs/forms.rst`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/docs/getting_started.rst` & `django-taggit-4.0.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/docs/serializers.rst` & `django-taggit-4.0.0/docs/serializers.rst`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/setup.cfg` & `django-taggit-4.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/forms.py` & `django-taggit-4.0.0/taggit/forms.py`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/ar/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/ar/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/cs/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/cs/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/da/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/da/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/de/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/de/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/el/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/el/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/en/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/eo/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/eo/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/eo/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/es/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/es/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/fa/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/fa/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/fi/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/fi/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/fr/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/fr/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/he/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/he/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/it/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/it/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/ja/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/ja/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/nb/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/nb/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/nl/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/nl/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/pt_BR/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/pt_BR/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/ru/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/ru/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/tr/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/tr/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/uk/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/uk/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-taggit-4.0.0/taggit/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/locale/zh_Hans/LC_MESSAGES/django.po` & `django-taggit-4.0.0/taggit/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/managers.py` & `django-taggit-4.0.0/taggit/managers.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 class ExtraJoinRestriction:
     """
     An extra restriction used for contenttype restriction in joins.
     """
 
     contains_aggregate = False
+    contains_over_clause = False
 
     def __init__(self, alias, col, content_types):
         self.alias = alias
         self.col = col
         self.content_types = content_types
 
     def as_sql(self, compiler, connection):
@@ -697,19 +698,37 @@
             )
 
     @cached_property
     def reverse_path_infos(self):
         return self.get_reverse_path_info()
 
     def get_joining_columns(self, reverse_join=False):
+        # RemovedInDjango60Warning
+        # https://github.com/django/django/commit/8b1ff0da4b162e87edebd94e61f2cd153e9e159d
         if reverse_join:
             return ((self.model._meta.pk.column, "object_id"),)
         else:
             return (("object_id", self.model._meta.pk.column),)
 
+    def get_joining_fields(self, reverse_join=False):
+        if reverse_join:
+            return (
+                (
+                    self.model._meta.pk,
+                    self.remote_field.through._meta.get_field("object_id"),
+                ),
+            )
+        else:
+            return (
+                (
+                    self.remote_field.through._meta.get_field("object_id"),
+                    self.model._meta.pk,
+                ),
+            )
+
     def _get_extra_restriction(self, alias, related_alias):
         extra_col = self.through._meta.get_field("content_type").column
         content_type_ids = [
             ContentType.objects.get_for_model(subclass).pk
             for subclass in _get_subclasses(self.model)
         ]
         return ExtraJoinRestriction(related_alias, extra_col, content_type_ids)
@@ -723,16 +742,21 @@
     # the signature of the (private) function was changed
     if django.VERSION < (4, 0):
         get_extra_restriction = _get_extra_restriction_legacy
     else:
         get_extra_restriction = _get_extra_restriction
 
     def get_reverse_joining_columns(self):
+        # RemovedInDjango60Warning
+        # https://github.com/django/django/commit/8b1ff0da4b162e87edebd94e61f2cd153e9e159d
         return self.get_joining_columns(reverse_join=True)
 
+    def get_reverse_joining_fields(self):
+        return self.get_joining_fields(reverse_join=True)
+
     @property
     def related_fields(self):
         return [(self.through._meta.get_field("object_id"), self.model._meta.pk)]
 
     @property
     def foreign_related_fields(self):
         return [self.related_fields[0][1]]
```

### Comparing `django-taggit-3.1.0/taggit/migrations/0001_initial.py` & `django-taggit-4.0.0/taggit/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("contenttypes", "0001_initial")]
 
     operations = [
         migrations.CreateModel(
             name="Tag",
             fields=[
                 (
```

### Comparing `django-taggit-3.1.0/taggit/migrations/0004_alter_taggeditem_content_type_alter_taggeditem_tag.py` & `django-taggit-4.0.0/taggit/migrations/0004_alter_taggeditem_content_type_alter_taggeditem_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # update to Django 4.0.
 # See https://docs.djangoproject.com/en/stable/releases/4.0/#migrations-autodetector-changes
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("contenttypes", "0002_remove_content_type_name"),
         ("taggit", "0003_taggeditem_add_unique_index"),
     ]
 
     operations = [
         migrations.AlterField(
```

### Comparing `django-taggit-3.1.0/taggit/models.py` & `django-taggit-4.0.0/taggit/models.py`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/serializers.py` & `django-taggit-4.0.0/taggit/serializers.py`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/utils.py` & `django-taggit-4.0.0/taggit/utils.py`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/taggit/views.py` & `django-taggit-4.0.0/taggit/views.py`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/tests/forms.py` & `django-taggit-4.0.0/tests/forms.py`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/tests/migrations/0001_initial.py` & `django-taggit-4.0.0/tests/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import django.db.models.deletion
 from django.db import migrations, models
 
 import taggit.managers
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("taggit", "0003_taggeditem_add_unique_index"),
         ("contenttypes", "0002_remove_content_type_name"),
     ]
```

### Comparing `django-taggit-3.1.0/tests/migrations/0002_auto_20200214_1129.py` & `django-taggit-4.0.0/tests/migrations/0002_auto_20200214_1129.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import django.utils.timezone
 from django.db import migrations, models
 
 import taggit.managers
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("taggit", "0003_taggeditem_add_unique_index"),
         ("contenttypes", "0002_remove_content_type_name"),
         ("tests", "0001_initial"),
     ]
 
     operations = [
```

### Comparing `django-taggit-3.1.0/tests/migrations/0003_auto_20210310_0918.py` & `django-taggit-4.0.0/tests/migrations/0003_auto_20210310_0918.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import django.db.models.deletion
 from django.db import migrations, models
 
 import taggit.managers
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("taggit", "0003_taggeditem_add_unique_index"),
         ("contenttypes", "0002_remove_content_type_name"),
         ("tests", "0002_auto_20200214_1129"),
     ]
 
     operations = [
```

### Comparing `django-taggit-3.1.0/tests/migrations/0004_auto_20210619_0826.py` & `django-taggit-4.0.0/tests/migrations/0004_auto_20210619_0826.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import django.db.models.deletion
 from django.db import migrations, models
 
 import taggit.managers
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("contenttypes", "0002_remove_content_type_name"),
         ("taggit", "0003_taggeditem_add_unique_index"),
         ("tests", "0003_auto_20210310_0918"),
     ]
 
     operations = [
```

### Comparing `django-taggit-3.1.0/tests/migrations/0005_auto_20210713_2301.py` & `django-taggit-4.0.0/tests/migrations/0005_auto_20210713_2301.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from django.db import migrations, models
 
 import taggit.managers
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("tests", "0004_auto_20210619_0826"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="OrderedModel",
```

### Comparing `django-taggit-3.1.0/tests/models.py` & `django-taggit-4.0.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/tests/settings.py` & `django-taggit-4.0.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/tests/test_admin.py` & `django-taggit-4.0.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/tests/test_forms.py` & `django-taggit-4.0.0/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/tests/test_models.py` & `django-taggit-4.0.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/tests/test_serializers.py` & `django-taggit-4.0.0/tests/test_serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         """
         request_data = {"tags": '["1", "2", "3"]'}
 
         serializer = TestModelSerializer(data=request_data)
         assert serializer.is_valid(), serializer.errors
         test_model = serializer.save()
 
-        assert set(tag.name for tag in test_model.tags.all()) == {"1", "2", "3"}
+        assert {tag.name for tag in test_model.tags.all()} == {"1", "2", "3"}
 
     def test_taggit_removes_tags(self):
         """
         Test if the old assigned tags are removed
         """
         test_model = TestModel.objects.create()
         test_model.tags.add("1")
```

### Comparing `django-taggit-3.1.0/tests/test_utils.py` & `django-taggit-4.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-taggit-3.1.0/tests/tests.py` & `django-taggit-4.0.0/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from io import StringIO
 from unittest import mock
 
+from django import VERSION as DJANGO_VERSION
 from django.contrib.contenttypes.models import ContentType
 from django.core import serializers
 from django.core.exceptions import ValidationError
 from django.core.management import call_command
 from django.db import IntegrityError, connection, models
 from django.test import RequestFactory, SimpleTestCase, TestCase
 from django.test.utils import override_settings
@@ -915,33 +916,50 @@
 
 
 class TaggableFormTestCase(BaseTaggingTestCase):
     form_class = FoodForm
     food_model = Food
 
     def _get_form_str(self, form_str):
-        form_str %= {
-            "help_start": '<span class="helptext">',
-            "help_stop": "</span>",
-            "required": "required",
-        }
+        if DJANGO_VERSION >= (5, 0):
+            # Django defaults to div-based form rendering in 5.0
+            # https://github.com/django/django/commit/98756c685ee173bbd43f21ed0553f808be835ce5
+            # https://github.com/django/django/commit/232b60a21b951bd16b8c95b34fcbcbf3ecd89fca
+            form_str %= {
+                "help_start": '<div class="helptext">',
+                "help_stop": "</div>",
+                "required": "required",
+            }
+        else:
+            form_str %= {
+                "help_start": '<span class="helptext">',
+                "help_stop": "</span>",
+                "required": "required",
+            }
         return form_str
 
     def assertFormRenders(self, form, html):
         self.assertHTMLEqual(str(form), self._get_form_str(html))
 
     def test_form(self):
         self.assertEqual(list(self.form_class.base_fields), ["name", "tags"])
 
         f = self.form_class({"name": "apple", "tags": "green, red, yummy"})
-        self.assertFormRenders(
-            f,
-            """<tr><th><label for="id_name">Name:</label></th><td><input id="id_name" type="text" name="name" value="apple" maxlength="50" %(required)s /></td></tr>
-<tr><th><label for="id_tags">Tags:</label></th><td><input type="text" name="tags" value="green, red, yummy" id="id_tags" %(required)s /><br />%(help_start)sA comma-separated list of tags.%(help_stop)s</td></tr>""",
-        )
+        if DJANGO_VERSION >= (5, 0):
+            self.assertFormRenders(
+                f,
+                """<div><label for="id_name">Name:</label><input id="id_name" type="text" name="name" value="apple" maxlength="50" %(required)s /></div>
+    <div><label for="id_tags">Tags:</label>%(help_start)sA comma-separated list of tags.%(help_stop)s<input type="text" name="tags" value="green, red, yummy" id="id_tags" %(required)s /></div>""",
+            )
+        else:
+            self.assertFormRenders(
+                f,
+                """<tr><th><label for="id_name">Name:</label></th><td><input id="id_name" type="text" name="name" value="apple" maxlength="50" %(required)s /></td></tr>
+    <tr><th><label for="id_tags">Tags:</label></th><td><input type="text" name="tags" value="green, red, yummy" id="id_tags" %(required)s /><br />%(help_start)sA comma-separated list of tags.%(help_stop)s</td></tr>""",
+            )
         f.save()
         apple = self.food_model.objects.get(name="apple")
         self.assert_tags_equal(apple.tags.all(), ["green", "red", "yummy"])
 
         f = self.form_class(
             {"name": "apple", "tags": "green, red, yummy, delicious"}, instance=apple
         )
@@ -950,35 +968,56 @@
         self.assert_tags_equal(apple.tags.all(), ["green", "red", "yummy", "delicious"])
         self.assertEqual(self.food_model.objects.count(), 1)
 
         f = self.form_class({"name": "raspberry"})
         self.assertFalse(f.is_valid())
 
         f = self.form_class(instance=apple)
-        self.assertFormRenders(
-            f,
-            """<tr><th><label for="id_name">Name:</label></th><td><input id="id_name" type="text" name="name" value="apple" maxlength="50" %(required)s /></td></tr>
-<tr><th><label for="id_tags">Tags:</label></th><td><input type="text" name="tags" value="delicious, green, red, yummy" id="id_tags" %(required)s /><br />%(help_start)sA comma-separated list of tags.%(help_stop)s</td></tr>""",
-        )
+        if DJANGO_VERSION >= (5, 0):
+            self.assertFormRenders(
+                f,
+                """<div><label for="id_name">Name:</label><input id="id_name" type="text" name="name" value="apple" maxlength="50" %(required)s /></div>
+    <div><label for="id_tags">Tags:</label>%(help_start)sA comma-separated list of tags.%(help_stop)s<input type="text" name="tags" value="delicious, green, red, yummy" id="id_tags" %(required)s /></div>""",
+            )
+        else:
+            self.assertFormRenders(
+                f,
+                """<tr><th><label for="id_name">Name:</label></th><td><input id="id_name" type="text" name="name" value="apple" maxlength="50" %(required)s /></td></tr>
+    <tr><th><label for="id_tags">Tags:</label></th><td><input type="text" name="tags" value="delicious, green, red, yummy" id="id_tags" %(required)s /><br />%(help_start)sA comma-separated list of tags.%(help_stop)s</td></tr>""",
+            )
 
         apple.tags.add("has,comma")
         f = self.form_class(instance=apple)
-        self.assertFormRenders(
-            f,
-            """<tr><th><label for="id_name">Name:</label></th><td><input id="id_name" type="text" name="name" value="apple" maxlength="50" %(required)s /></td></tr>
-<tr><th><label for="id_tags">Tags:</label></th><td><input type="text" name="tags" value="&quot;has,comma&quot;, delicious, green, red, yummy" id="id_tags" %(required)s /><br />%(help_start)sA comma-separated list of tags.%(help_stop)s</td></tr>""",
-        )
+        if DJANGO_VERSION >= (5, 0):
+            self.assertFormRenders(
+                f,
+                """<div><label for="id_name">Name:</label><input id="id_name" type="text" name="name" value="apple" maxlength="50" %(required)s /></div>
+    <div><label for="id_tags">Tags:</label>%(help_start)sA comma-separated list of tags.%(help_stop)s<input type="text" name="tags" value="&quot;has,comma&quot;, delicious, green, red, yummy" id="id_tags" %(required)s /></div>""",
+            )
+        else:
+            self.assertFormRenders(
+                f,
+                """<tr><th><label for="id_name">Name:</label></th><td><input id="id_name" type="text" name="name" value="apple" maxlength="50" %(required)s /></td></tr>
+    <tr><th><label for="id_tags">Tags:</label></th><td><input type="text" name="tags" value="&quot;has,comma&quot;, delicious, green, red, yummy" id="id_tags" %(required)s /><br />%(help_start)sA comma-separated list of tags.%(help_stop)s</td></tr>""",
+            )
 
         apple.tags.add("has space")
         f = self.form_class(instance=apple)
-        self.assertFormRenders(
-            f,
-            """<tr><th><label for="id_name">Name:</label></th><td><input id="id_name" type="text" name="name" value="apple" maxlength="50" %(required)s /></td></tr>
-<tr><th><label for="id_tags">Tags:</label></th><td><input type="text" name="tags" value="&quot;has space&quot;, &quot;has,comma&quot;, delicious, green, red, yummy" id="id_tags" %(required)s /><br />%(help_start)sA comma-separated list of tags.%(help_stop)s</td></tr>""",
-        )
+        if DJANGO_VERSION >= (5, 0):
+            self.assertFormRenders(
+                f,
+                """<div><label for="id_name">Name:</label><input id="id_name" type="text" name="name" value="apple" maxlength="50" %(required)s /></div>
+    <div><label for="id_tags">Tags:</label>%(help_start)sA comma-separated list of tags.%(help_stop)s<input type="text" name="tags" value="&quot;has space&quot;, &quot;has,comma&quot;, delicious, green, red, yummy" id="id_tags" %(required)s /></div>""",
+            )
+        else:
+            self.assertFormRenders(
+                f,
+                """<tr><th><label for="id_name">Name:</label></th><td><input id="id_name" type="text" name="name" value="apple" maxlength="50" %(required)s /></td></tr>
+    <tr><th><label for="id_tags">Tags:</label></th><td><input type="text" name="tags" value="&quot;has space&quot;, &quot;has,comma&quot;, delicious, green, red, yummy" id="id_tags" %(required)s /><br />%(help_start)sA comma-separated list of tags.%(help_stop)s</td></tr>""",
+            )
 
     def test_formfield(self):
         tm = TaggableManager(
             verbose_name="categories", help_text="Add some categories", blank=True
         )
         ff = tm.formfield()
         self.assertEqual(ff.label, "Categories")
```

### Comparing `django-taggit-3.1.0/tox.ini` & `django-taggit-4.0.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [tox]
 minversion = 1.9
 envlist =
     black
     flake8
     isort
-    py{36,37,38,39,310}-dj32
-    py{38,39,310}-dj40
-    py{38,39,310,311}-dj{41,main}
+    py{37,38,39,310}-dj32
+    py{38,39,310,311}-dj{41,42}
+    py{310,311}-djmain
     docs
 
 [gh-actions]
 python =
-    3.6: py36
     3.7: py37
     3.8: py38, black, flake8, isort
     3.9: py39
     3.10: py310
     3.11: py311
 
 [testenv]
 deps =
     dj32: Django>=3.2,<3.3
-    dj40: Django>=4.0,<4.1
     dj41: Django>=4.1,<4.2
+    dj42: Django>=4.2,<5.0
     djmain: https://github.com/django/django/archive/main.tar.gz
     coverage
     djangorestframework
 commands =
     coverage run -m django test --settings=tests.settings {posargs}
     coverage report
     coverage xml
@@ -35,15 +34,15 @@
 ignore_errors =
     djmain: True
 
 [testenv:black]
 basepython = python3
 skip_install = true
 deps = black
-commands = black --target-version=py36 --check --diff .
+commands = black --target-version=py37 --check --diff .
 
 [testenv:flake8]
 basepython = python3
 skip_install = true
 deps = flake8
 commands = flake8
```

