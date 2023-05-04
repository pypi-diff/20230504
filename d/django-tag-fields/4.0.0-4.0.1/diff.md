# Comparing `tmp/django-tag-fields-4.0.0.tar.gz` & `tmp/django-tag-fields-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tag-fields-4.0.0.tar", last modified: Fri Apr 28 06:52:08 2023, max compression
+gzip compressed data, was "django-tag-fields-4.0.1.tar", last modified: Thu May  4 08:41:56 2023, max compression
```

## Comparing `django-tag-fields-4.0.0.tar` & `django-tag-fields-4.0.1.tar`

### file list

```diff
@@ -1,158 +1,116 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/
--rw-r--r--   0 mark      (1000) mark      (1000)      665 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/AUTHORS
--rw-r--r--   0 mark      (1000) mark      (1000)    13204 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/CHANGELOG.rst
--rw-r--r--   0 mark      (1000) mark      (1000)     1562 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)      205 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/MANIFEST.in
--rw-r--r--   0 mark      (1000) mark      (1000)     3685 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     2297 2023-04-28 06:03:59.000000 django-tag-fields-4.0.0/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/django_tag_fields.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     3685 2023-04-28 06:52:07.000000 django-tag-fields-4.0.0/django_tag_fields.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     3420 2023-04-28 06:52:07.000000 django-tag-fields-4.0.0/django_tag_fields.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-28 06:52:07.000000 django-tag-fields-4.0.0/django_tag_fields.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-28 06:52:07.000000 django-tag-fields-4.0.0/django_tag_fields.egg-info/not-zip-safe
--rw-r--r--   0 mark      (1000) mark      (1000)       12 2023-04-28 06:52:07.000000 django-tag-fields-4.0.0/django_tag_fields.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       11 2023-04-28 06:52:07.000000 django-tag-fields-4.0.0/django_tag_fields.egg-info/top_level.txt
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/docs/
--rw-r--r--   0 mark      (1000) mark      (1000)     1525 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/docs/admin.rst
--rw-r--r--   0 mark      (1000) mark      (1000)     4396 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/docs/api.rst
--rw-r--r--   0 mark      (1000) mark      (1000)       30 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/docs/changelog.rst
--rw-r--r--   0 mark      (1000) mark      (1000)      473 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/docs/conf.py
--rw-r--r--   0 mark      (1000) mark      (1000)       33 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/docs/contributing.rst
--rw-r--r--   0 mark      (1000) mark      (1000)     8446 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/docs/custom_tagging.rst
--rw-r--r--   0 mark      (1000) mark      (1000)     2251 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/docs/external_apps.rst
--rw-r--r--   0 mark      (1000) mark      (1000)     1061 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/docs/faq.rst
--rw-r--r--   0 mark      (1000) mark      (1000)     2378 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/docs/forms.rst
--rw-r--r--   0 mark      (1000) mark      (1000)     1794 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/docs/getting_started.rst
--rw-r--r--   0 mark      (1000) mark      (1000)      619 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/docs/index.rst
--rw-r--r--   0 mark      (1000) mark      (1000)      782 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/docs/serializers.rst
--rw-r--r--   0 mark      (1000) mark      (1000)     1431 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/setup.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/tag_fields/
--rw-r--r--   0 mark      (1000) mark      (1000)      283 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      382 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/admin.py
--rw-r--r--   0 mark      (1000) mark      (1000)      253 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/apps.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1442 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/forms.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/ar/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/tag_fields/locale/ar/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)     1299 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     2206 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/cs/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/tag_fields/locale/cs/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)     1042 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     2005 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/da/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/tag_fields/locale/da/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)     1033 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     1941 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/de/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/tag_fields/locale/de/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)     1068 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     1839 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/el/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/tag_fields/locale/el/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)      991 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     2188 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/en/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/tag_fields/locale/en/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)      337 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     1738 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/eo/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/tag_fields/locale/eo/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)     1131 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/eo/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     1873 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/eo/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/es/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/tag_fields/locale/es/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)     1058 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     2021 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/fa/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/tag_fields/locale/fa/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)     1203 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     2162 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/fi/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/tag_fields/locale/fi/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)     1047 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     1928 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/fr/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/tag_fields/locale/fr/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)     1105 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     2073 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/he/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/tag_fields/locale/he/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)      828 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     1955 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/it/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/tag_fields/locale/it/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)      945 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     1904 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/ja/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/tag_fields/locale/ja/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)     1142 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     1908 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/nb/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/tag_fields/locale/nb/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)      993 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     1947 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/nl/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/tag_fields/locale/nl/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)      933 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     1739 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/pt_BR/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/tag_fields/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)     1045 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     1897 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/ru/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/tag_fields/locale/ru/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)     1870 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     2544 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/tr/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/tag_fields/locale/tr/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)     1051 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     2014 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/uk/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/tag_fields/locale/uk/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)     1211 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     2144 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.006041 django-tag-fields-4.0.0/tag_fields/locale/zh_Hans/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/tag_fields/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 mark      (1000) mark      (1000)      992 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 mark      (1000) mark      (1000)     1982 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 mark      (1000) mark      (1000)    25412 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/managers.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/tag_fields/migrations/
--rw-r--r--   0 mark      (1000) mark      (1000)     2694 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/migrations/0001_initial.py
--rw-r--r--   0 mark      (1000) mark      (1000)      280 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/migrations/0002_auto_20150616_2121.py
--rw-r--r--   0 mark      (1000) mark      (1000)      374 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/migrations/0003_taggeditem_add_unique_index.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1232 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/migrations/0004_alter_taggeditem_content_type_alter_taggeditem_tag.py
--rw-r--r--   0 mark      (1000) mark      (1000)      502 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/migrations/0005_auto_20220424_2025.py
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/migrations/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     6049 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/models.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4386 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/serializers.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4295 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/utils.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1534 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tag_fields/views.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/tests/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)       89 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/admin.py
--rw-r--r--   0 mark      (1000) mark      (1000)      168 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/custom_parser.py
--rw-r--r--   0 mark      (1000) mark      (1000)      834 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/forms.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/tests/migrations/
--rw-r--r--   0 mark      (1000) mark      (1000)    39683 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/migrations/0001_initial.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3529 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/migrations/0002_auto_20200214_1129.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3015 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/migrations/0003_auto_20210310_0918.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4440 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/migrations/0004_auto_20210619_0826.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1025 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/migrations/0005_auto_20210713_2301.py
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/migrations/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)    10015 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/models.py
--rw-r--r--   0 mark      (1000) mark      (1000)      329 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/serializers.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1333 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/settings.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.016041 django-tag-fields-4.0.0/tests/templates/
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-28 06:52:08.026041 django-tag-fields-4.0.0/tests/templates/tests/
--rw-r--r--   0 mark      (1000) mark      (1000)      124 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/templates/tests/food_tag_list.html
--rw-r--r--   0 mark      (1000) mark      (1000)     1394 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/test_admin.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1849 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/test_forms.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2339 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/test_models.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3366 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/test_serializers.py
--rw-r--r--   0 mark      (1000) mark      (1000)      984 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/test_utils.py
--rw-r--r--   0 mark      (1000) mark      (1000)    49826 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/tests.py
--rw-r--r--   0 mark      (1000) mark      (1000)      294 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/urls.py
--rw-r--r--   0 mark      (1000) mark      (1000)      182 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tests/views.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1174 2023-04-14 07:08:31.000000 django-tag-fields-4.0.0/tox.ini
+-rw-r--r--   0        0        0      235 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.coveragerc
+-rw-r--r--   0        0        0     1983 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/.git-commit-template.txt
+-rw-r--r--   0        0        0      907 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      136 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/ISSUE_TEMPLATE/chore.md
+-rw-r--r--   0        0        0      424 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/ISSUE_TEMPLATE/documentation-request.md
+-rw-r--r--   0        0        0      619 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0      841 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/semantic.yaml
+-rw-r--r--   0        0        0      923 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1503 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1198 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.gitignore
+-rw-r--r--   0        0        0     1389 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      751 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/AUTHORS
+-rw-r--r--   0        0        0    13599 2023-05-04 08:41:51.398888 django-tag-fields-4.0.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     5488 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5244 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1574 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/LICENSE
+-rw-r--r--   0        0        0      205 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/MANIFEST.in
+-rw-r--r--   0        0        0     2739 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/README.rst
+-rw-r--r--   0        0        0      853 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/codecov.yml
+-rw-r--r--   0        0        0     1525 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/admin.rst
+-rw-r--r--   0        0        0     4396 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/api.rst
+-rw-r--r--   0        0        0       30 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/changelog.rst
+-rw-r--r--   0        0        0      471 2023-05-04 08:41:51.410888 django-tag-fields-4.0.1/docs/conf.py
+-rw-r--r--   0        0        0       33 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/contributing.rst
+-rw-r--r--   0        0        0     8972 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/custom_tagging.rst
+-rw-r--r--   0        0        0     2251 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/external_apps.rst
+-rw-r--r--   0        0        0     1040 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/faq.rst
+-rw-r--r--   0        0        0     2378 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/forms.rst
+-rw-r--r--   0        0        0     1903 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/getting_started.rst
+-rw-r--r--   0        0        0      705 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/index.rst
+-rw-r--r--   0        0        0      983 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/serializers.rst
+-rw-r--r--   0        0        0     1855 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/requirements/docs.txt
+-rw-r--r--   0        0        0       36 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/requirements/test.txt
+-rw-r--r--   0        0        0       38 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/setup.py
+-rw-r--r--   0        0        0      259 2023-05-04 08:41:51.410888 django-tag-fields-4.0.1/tag_fields/__init__.py
+-rw-r--r--   0        0        0      382 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/admin.py
+-rw-r--r--   0        0        0      253 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/apps.py
+-rw-r--r--   0        0        0     1442 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/forms.py
+-rw-r--r--   0        0        0     1299 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2206 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1042 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2005 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1033 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1941 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/da/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1068 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1839 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      991 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2188 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1738 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1131 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/eo/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1873 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/eo/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1058 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2021 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1203 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2162 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1047 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1928 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/fi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1105 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2073 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      828 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1955 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      945 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1904 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1142 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1908 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      993 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1947 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      933 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1739 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1045 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1897 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1870 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2544 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1051 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2014 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1211 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2144 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      992 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1982 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    26666 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/managers.py
+-rw-r--r--   0        0        0     2694 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/migrations/0001_initial.py
+-rw-r--r--   0        0        0      280 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/migrations/0002_auto_20150616_2121.py
+-rw-r--r--   0        0        0      374 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/migrations/0003_taggeditem_add_unique_index.py
+-rw-r--r--   0        0        0     1232 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/migrations/0004_alter_taggeditem_content_type_alter_taggeditem_tag.py
+-rw-r--r--   0        0        0      502 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/migrations/0005_auto_20220424_2025.py
+-rw-r--r--   0        0        0        0 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/migrations/__init__.py
+-rw-r--r--   0        0        0     7780 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/models.py
+-rw-r--r--   0        0        0     4386 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/serializers.py
+-rw-r--r--   0        0        0     4295 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/utils.py
+-rw-r--r--   0        0        0     1583 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/views.py
+-rw-r--r--   0        0        0        0 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/__init__.py
+-rw-r--r--   0        0        0       89 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/admin.py
+-rw-r--r--   0        0        0      168 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/custom_parser.py
+-rw-r--r--   0        0        0      834 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/forms.py
+-rw-r--r--   0        0        0    39683 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3529 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/migrations/0002_auto_20200214_1129.py
+-rw-r--r--   0        0        0     3015 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/migrations/0003_auto_20210310_0918.py
+-rw-r--r--   0        0        0     4440 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/migrations/0004_auto_20210619_0826.py
+-rw-r--r--   0        0        0     1025 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/migrations/0005_auto_20210713_2301.py
+-rw-r--r--   0        0        0        0 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/migrations/__init__.py
+-rw-r--r--   0        0        0    10311 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/models.py
+-rw-r--r--   0        0        0      329 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/serializers.py
+-rw-r--r--   0        0        0     1333 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/settings.py
+-rw-r--r--   0        0        0      124 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/templates/tests/food_tag_list.html
+-rw-r--r--   0        0        0     1394 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/test_admin.py
+-rw-r--r--   0        0        0     1849 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/test_forms.py
+-rw-r--r--   0        0        0     2339 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/test_models.py
+-rw-r--r--   0        0        0     3366 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/test_serializers.py
+-rw-r--r--   0        0        0      984 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/test_utils.py
+-rw-r--r--   0        0        0    54037 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/tests.py
+-rw-r--r--   0        0        0      294 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/urls.py
+-rw-r--r--   0        0        0      182 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/views.py
+-rw-r--r--   0        0        0     1174 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tox.ini
+-rw-r--r--   0        0        0     4065 1970-01-01 00:00:00.000000 django-tag-fields-4.0.1/PKG-INFO
```

### Comparing `django-tag-fields-4.0.0/CHANGELOG.rst` & `django-tag-fields-4.0.1/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 Changelog
 =========
 
 (Unreleased)
 ~~~~~~~~~~~~
 
+<!--next-version-placeholder-->
+
+## v4.0.1 (2023-05-04)
+### Fix
+* **dev:** Add pre-commit to requirements #51 ([`5a27789`](https://github.com/imAsparky/django-tag-fields/commit/5a277893dd2b112fb57ac439c44c04b3f3e3183e))
+
+### Documentation
+* **all:** Update with all model changes #38 ([`0efc84b`](https://github.com/imAsparky/django-tag-fields/commit/0efc84b6b16789990a097318e58ffa92c44bf413))
+
 4.0.0 (2023-03-30)
 ~~~~~~~~~~~~~~~~~~
 * Initial release of django-tag-fields.
 * A renaming of cloned `django-taggit`
 
 This release functions the same as `django-taggit v3.1.0`.  The changes here are simply
 getting the project to be `django-tag-fields`, with all the necessary downstream changes
```

### Comparing `django-tag-fields-4.0.0/LICENSE` & `django-tag-fields-4.0.1/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) Alex Gaynor, Paul Oostenrijk, and individual contributors.
+Copyright (c) Alex Gaynor, Paul Oostenrijk, Mark Sevelj and individual contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
     1. Redistributions of source code must retain the above copyright notice,
        this list of conditions and the following disclaimer.
```

### Comparing `django-tag-fields-4.0.0/PKG-INFO` & `django-tag-fields-4.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,66 @@
 Metadata-Version: 2.1
 Name: django-tag-fields
-Version: 4.0.0
-Summary: django-tag-fields is an extension of django-taggit for tagging fields.
-Home-page: https://github.com/imAsparky/django-tag-fields
-Author: Alex Gaynor
-Author-email: alex.gaynor@gmail.com
-License: BSD
-Project-URL: Documentation, https://django-tag-fields.readthedocs.io
-Project-URL: Source, https://github.com/imAsparky/django-tag-fields
-Project-URL: Tracker, https://github.com/imAsparky/django-tag-fields/issues
-Classifier: Development Status :: 5 - Production/Stable
+Version: 4.0.1
+Summary: Add field tags to a Django project
+Keywords: Django,django,django tagging
+Author-email: Alex Gaynor <alex.gaynor@gmail.com>
+Maintainer-email: Mark Sevelj <mark.sevelj@dunwright.com.au>
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
-License-File: LICENSE
-License-File: AUTHORS
+Requires-Dist: Django>=3.2
+Project-URL: Documentation, https://django-tag-fields.readthedocs.io
+Project-URL: Repository, https://github.com/imAsparky/django-tag-fields
+Project-URL: Tracker, https://github.com/imAsparky/django-tag-fields/issues
 
 django-tag-fields
 =================
 
+.. image:: https://www.repostatus.org/badges/latest/active.svg
+   :alt: Project Status: Active - The project has reached a stable, usable state and is being actively developed.
+   :target: https://www.repostatus.org/#active
+
 .. image:: https://img.shields.io/pypi/pyversions/django-tag_fields.svg
-   :target: https://pypi.org/project/django-tag-fields/
+   :target: https://pypi.org/project/django-taggit/
    :alt: Supported Python versions
 
-.. image:: https://img.shields.io/pypi/djversions/django-taggit.svg
+.. image:: https://img.shields.io/pypi/frameworkversions/django/django-tag-fields?logo=django
    :target: https://pypi.org/project/django-taggit/
    :alt: Supported Django versions
 
 .. image:: https://github.com/imAsparky/django-tag-fields/workflows/Test/badge.svg
    :target: https://github.com/imAsparky/django-tag-fields/actions
    :alt: GitHub Actions
 
 .. image:: https://codecov.io/gh/imAsparky/django-tag-fields/branch/main/graph/badge.svg?token=6TPEAAOUUF
    :target: https://codecov.io/gh/imAsparky/django-tag-fields
 
+.. image:: https://readthedocs.org/projects/django-tag-fields/badge/?version=latest
+   :target: https://django-tag-fields.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+
 This is a clone of `Jazzband django-taggit <https://github.com/jazzband/django-taggit>`_ project.
+
 By contributing you agree to abide by the `Contributor Code of Conduct
 <https://github.com/imAsparky/django-tag-fields/blob/main/CODE_OF_CONDUCT.md>`_.
 
 
 .. note::
 
    This project was cloned from ``django-taggit v3.1.0`` and will continue to work in the same
@@ -96,8 +103,9 @@
 
 ``django-tag-fields`` requires Django 3.2 or greater.
 
 For more info check out the `documentation
 <https://django-tag-fields.readthedocs.io/>`_.
 
 For questions about usage or development you can create an issue on Github (if your question is about
-usage please add the `question` label).
+usage please add the ``question`` label).
+
```

### Comparing `django-tag-fields-4.0.0/README.rst` & `django-tag-fields-4.0.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 django-tag-fields
 =================
 
+.. image:: https://www.repostatus.org/badges/latest/active.svg
+   :alt: Project Status: Active - The project has reached a stable, usable state and is being actively developed.
+   :target: https://www.repostatus.org/#active
+
 .. image:: https://img.shields.io/pypi/pyversions/django-tag_fields.svg
-   :target: https://pypi.org/project/django-tag-fields/
+   :target: https://pypi.org/project/django-taggit/
    :alt: Supported Python versions
 
-.. image:: https://img.shields.io/pypi/djversions/django-taggit.svg
+.. image:: https://img.shields.io/pypi/frameworkversions/django/django-tag-fields?logo=django
    :target: https://pypi.org/project/django-taggit/
    :alt: Supported Django versions
 
 .. image:: https://github.com/imAsparky/django-tag-fields/workflows/Test/badge.svg
    :target: https://github.com/imAsparky/django-tag-fields/actions
    :alt: GitHub Actions
 
 .. image:: https://codecov.io/gh/imAsparky/django-tag-fields/branch/main/graph/badge.svg?token=6TPEAAOUUF
    :target: https://codecov.io/gh/imAsparky/django-tag-fields
 
+.. image:: https://readthedocs.org/projects/django-tag-fields/badge/?version=latest
+   :target: https://django-tag-fields.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+
 This is a clone of `Jazzband django-taggit <https://github.com/jazzband/django-taggit>`_ project.
+
 By contributing you agree to abide by the `Contributor Code of Conduct
 <https://github.com/imAsparky/django-tag-fields/blob/main/CODE_OF_CONDUCT.md>`_.
 
 
 .. note::
 
    This project was cloned from ``django-taggit v3.1.0`` and will continue to work in the same
@@ -63,8 +72,8 @@
 
 ``django-tag-fields`` requires Django 3.2 or greater.
 
 For more info check out the `documentation
 <https://django-tag-fields.readthedocs.io/>`_.
 
 For questions about usage or development you can create an issue on Github (if your question is about
-usage please add the `question` label).
+usage please add the ``question`` label).
```

### Comparing `django-tag-fields-4.0.0/docs/admin.rst` & `django-tag-fields-4.0.1/docs/admin.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/docs/api.rst` & `django-tag-fields-4.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/docs/custom_tagging.rst` & `django-tag-fields-4.0.1/docs/custom_tagging.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,109 +1,118 @@
 Customizing tag-fields
 ======================
 
 Using a Custom Tag or Through Model
 -----------------------------------
-By default ``django-tag-fields`` uses a "through model" with a
-``GenericForeignKey`` on it, that has another ``ForeignKey`` to an included
-``Tag`` model.  However, there are some cases where this isn't desirable, for
-example if you want the speed and referential guarantees of a real
-``ForeignKey``, if you have a model with a non-integer primary key, or if you
-want to store additional data about a tag, such as whether it is official.  In
-these cases ``django-tag-fields`` makes it easy to substitute your own through
-model, or ``Tag`` model.
-
-Note: Including 'tag-fields' in ``settings.py`` INSTALLED_APPS list will create the
-default ``django-tag-fields`` and "through model" models. If you would like to use
-your own models, you will need to remove `tag_fields` from ``settings.py``'s
-INSTALLED_APPS list.
-
-To change the behavior there are a number of classes you can subclass to obtain
-different behavior:
-
-=============================== =======================================================================
-Class name                      Behavior
-=============================== =======================================================================
-``TaggedItemBase``              Allows custom ``ForeignKeys`` to models.
-``GenericTaggedItemBase``       Allows custom ``Tag`` models. Tagged models use an integer primary key.
-``GenericUUIDTaggedItemBase``   Allows custom ``Tag`` models. Tagged models use a UUID primary key.
-``CommonGenericTaggedItemBase`` Allows custom ``Tag`` models and ``GenericForeignKeys`` to models.
-``ItemBase``                    Allows custom ``Tag`` models and ``ForeignKeys`` to models.
-=============================== =======================================================================
+The tool ``django-tag-fields`` uses a ``through model`` with a
+``GenericForeignKey`` and another ``ForeignKey`` to an included ``Tag`` model.
+
+However, this may not be ideal in certain situations, such as needing the speed
+and referential guarantees of a real ``ForeignKey,`` having a model with a
+non-integer primary key or wanting to store extra data about a tag.
+Fortunately, ``django-tag-fields`` allows you to easily substitute your own
+through model or Tag model to address these issues.
+
+Note that if you include ``tag-fields`` in the ``settings.py`` INSTALLED_APPS
+list, the default ``django-tag-fields`` and ``through model`` models will be
+created.
+
+If you prefer custom models, remove ``tag_fields`` from the INSTALLED_APPS list
+in ``settings.py.``
+
+To change the behaviour, you can subclass several classes to achieve different
+outcomes.
+
+==================================    ====================================================================================================
+Class name                            Behavior
+==================================    ====================================================================================================
+``ThroughTableBase``                  Abstract Base Class: ``through table`` for all ``through table`` subclasses.
+``TaggedItemThroughBase``             Abstract Base Class: ``through table`` for a ``Tagged Item`` model.
+``GenericFKTaggedItemThroughBase``    Abstract Base Class: ``through table`` for a ``Tagged Item`` model using an ``GenericForeignKey``.
+``IntegerFKTaggedItemThroughBase``    Abstract Base Class: ``through table`` for a ``Tagged Item`` model using an ``integer`` primary key.
+``UUIDFKTaggedItemThroughBase``       Abstract Base Class: ``through table`` for a ``Tagged Item`` model using an ``UUID`` primary key.
+==================================    ====================================================================================================
 
 Custom ForeignKeys
 ~~~~~~~~~~~~~~~~~~
 
 Your intermediary model must be a subclass of
-``tag_fields.models.TaggedItemBase`` with a foreign key to your content
-model named ``content_object``. Pass this intermediary model as the
-``through`` argument to ``TaggableManager``:
+``tag_fields.models.TaggedItemThroughBase`` with a foreign key to your content
+model named ``content_object``.
+
+Pass this intermediary model as the ``through`` argument to ``TaggableManager``:
 
   .. code-block:: python
 
     from django.db import models
 
     from tag_fields.managers import TaggableManager
-    from tag_fields.models import TaggedItemBase
+    from tag_fields.models import TaggedItemThroughBase
 
 
-    class TaggedFood(TaggedItemBase):
+    class TaggedFood(TaggedItemThroughBase):
         content_object = models.ForeignKey('Food', on_delete=models.CASCADE)
 
     class Food(models.Model):
         # ... fields here
 
         tags = TaggableManager(through=TaggedFood)
 
 
 Once this is done, the API works the same as for GFK-tagged models.
 
 Custom GenericForeignKeys
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The default ``GenericForeignKey`` used by ``django-tag-fields`` assume your
-tagged object use an integer primary key. For non-integer primary key,
-your intermediary model must be a subclass of ``tag_fields.models.CommonGenericTaggedItemBase``
-with a field named ``"object_id"`` of the type of your primary key.
+tagged object uses an integer primary key. For non-integer primary key,
+your intermediary model must be a subclass of ``tag_fields.models.GenericFKTaggedItemThroughBase``
+with a field named ``object_id`` of the type of your primary key.
 
 For example, if your primary key is a string:
 
   .. code-block:: python
 
     from django.db import models
 
     from tag_fields.managers import TaggableManager
-    from tag_fields.models import CommonGenericTaggedItemBase, TaggedItemBase
+    from tag_fields.models import (
+                                   GenericFKTaggedItemThroughBase,
+                                   TaggedItemThroughBase,
+                                  )
 
-    class GenericStringTaggedItem(CommonGenericTaggedItemBase, TaggedItemBase):
+    class GenericStringTaggedItem(GenericFKTaggedItemThroughBase, TaggedItemThroughBase):
         object_id = models.CharField(max_length=50, verbose_name=_('Object id'), db_index=True)
 
     class Food(models.Model):
         food_id = models.CharField(primary_key=True)
         # ... fields here
 
         tags = TaggableManager(through=GenericStringTaggedItem)
 
-GenericUUIDTaggedItemBase
-~~~~~~~~~~~~~~~~~~~~~~~~~
+UUIDFKTaggedItemThroughBase
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-A common use case of a non-integer primary key, is UUID primary key.
-``django-tag-fields`` provides a base class ``GenericUUIDTaggedItemBase`` ready
-to use with models using an UUID primary key:
+A common use case of a non-integer primary key is the UUID primary key.
+``django-tag-fields`` provides a base class ``UUIDFKTaggedItemThroughBase`` ready
+to use with models using a UUID primary key:
 
   .. code-block:: python
 
     from django.db import models
     from django.utils.translation import gettext_lazy as _
 
     from tag_fields.managers import TaggableManager
-    from tag_fields.models import GenericUUIDTaggedItemBase, TaggedItemBase
+    from tag_fields.models import (
+                                   UUIDFKTaggedItemThroughBase,
+                                   TaggedItemThroughBase,
+                                  )
 
-    class UUIDTaggedItem(GenericUUIDTaggedItemBase, TaggedItemBase):
-        # If you only inherit GenericUUIDTaggedItemBase, you need to define
+    class UUIDTaggedItem(UUIDFKTaggedItemThroughBase, TaggedItemThroughBase):
+        # If you only inherit UUIDFKTaggedItemThroughBase, you need to define
         # a tag field. e.g.
         # tag = models.ForeignKey(Tag, related_name="uuid_tagged_items", on_delete=models.CASCADE)
 
         class Meta:
             verbose_name = _("Tag")
             verbose_name_plural = _("Tags")
 
@@ -112,41 +121,45 @@
         # ... fields here
 
         tags = TaggableManager(through=UUIDTaggedItem)
 
 Custom tag
 ~~~~~~~~~~
 
-When providing a custom ``Tag`` model it should be a ``ForeignKey`` to your tag
-model named ``"tag"``. If your custom ``Tag`` model has extra parameters you want to initialize during setup, you can do so by passing it along via the ``tag_kwargs`` parameter of ``TaggableManager.add``. For example ``my_food.tags.add("tag_name1", "tag_name2", tag_kwargs={"my_field":3})``:
+When providing a custom ``Tag`` model, it should be a ``ForeignKey`` to your
+tag model named ``"tag"``. If your custom ``Tag`` model has extra parameters
+you want to initialize during setup, you can pass it along via the
+``tag_kwargs`` parameter of ``TaggableManager.add``.
 
-  .. code-block:: python
+For example, ``my_food.tags.add("tag_name1", "tag_name2", tag_kwargs={"my_field":3})``:
+
+.. code-block:: python
 
     from django.db import models
     from django.utils.translation import gettext_lazy as _
 
     from tag_fields.managers import TaggableManager
-    from tag_fields.models import TagBase, GenericTaggedItemBase
+    from tag_fields.models import TagBase, GenericFKTaggedItemThroughBase
 
 
     class MyCustomTag(TagBase):
         # ... fields here
 
         class Meta:
             verbose_name = _("Tag")
             verbose_name_plural = _("Tags")
 
         # ... methods (if any) here
 
 
-    class TaggedWhatever(GenericTaggedItemBase):
-        # TaggedWhatever can also extend TaggedItemBase or a combination of
-        # both TaggedItemBase and GenericTaggedItemBase. GenericTaggedItemBase
-        # allows using the same tag for different kinds of objects, in this
-        # example Food and Drink.
+    class TaggedWhatever(GenericFKTaggedItemThroughBase):
+        # TaggedWhatever can also extend TaggedItemThroughBase or a combination
+        # of both TaggedItemThroughBase and GenericFKTaggedItemThroughBase.
+        # GenericFKTaggedItemThroughBase allows using the same tag for
+        # different kinds of objects, in this example Food and Drink.
 
         # Here is where you provide your custom Tag class.
         tag = models.ForeignKey(
             MyCustomTag,
             on_delete=models.CASCADE,
             related_name="%(app_label)s_%(class)s_items",
         )
@@ -159,58 +172,79 @@
 
 
     class Drink(models.Model):
         # ... fields here
 
         tags = TaggableManager(through=TaggedWhatever)
 
+|
 
 .. class:: TagBase
 
     .. method:: slugify(tag, i=None)
 
         By default ``tag-fields`` uses :func:`django.utils.text.slugify` to
-        calculate a slug for a given tag. However, if you want to implement
-        your own logic you can override this method, which receives the ``tag``
-        (a string), and ``i``, which is either ``None`` or an integer, which
-        signifies how many times the slug for this tag has been attempted to be
-        calculated, it is ``None`` on the first time, and the counting begins
-        at ``1`` thereafter.
+        calculate a slug for a given tag.
+
+        However, if you want to implement your logic, you can override this
+        method, which receives the ``tag`` (a string), and ``i``, which is
+        either ``None`` or an integer, which signifies how many times the slug
+        for this tag has been attempted to be calculated.  It is ``None`` on
+        the first attempt, and the counting begins at ``1`` thereafter.
 
 
 Using a custom tag string parser
 --------------------------------
 
-By default ``django-tag-fields`` uses ``tag_fields.utils._parse_tags`` which accepts a
-string which may contain one or more tags and returns a list of tag names. This
-parser is quite intelligent and can handle a number of edge cases; however, you
-may wish to provide your own parser for various reasons (e.g. you can do some
-preprocessing on the tags so that they are converted to lowercase, reject
-certain tags, disallow certain characters, split only on commas rather than
-commas and whitespace, etc.). To provide your own parser, write a function that
-takes a tag string and returns a list of tag names. For example, a simple
-function to split on comma and convert to lowercase:
+By default, ``django-tag-fields`` uses ``tag_fields.utils._parse_tags``, which
+accepts a string that may contain one or more tags and returns a list of tag
+names.
+
+This parser is quite intelligent and can handle many edge cases; however, you
+may wish to provide your parser for various reasons e.g.
+
+* you can do some preprocessing on the tags so that they are converted to
+  lowercase
+* reject certain tags
+* disallow certain characters
+* split only on commas rather than commas and whitespace
+* etc
+
+To provide your parser, write a function that takes a tag string and returns
+a list of tag names.
+
+|
+
+For example, see a simple function to split on comma's and convert to lowercase
+below.
+
+|
 
   .. code-block:: python
 
     def comma_splitter(tag_string):
         return [t.strip().lower() for t in tag_string.split(',') if t.strip()]
 
-You need to tell ``tag_fields`` to use this function instead of the default by
-adding a new setting, ``TAGGIT_TAGS_FROM_STRING`` and providing it with the
-dotted path to your function. Likewise, you can provide a function to convert a
-list of tags to a string representation and use the setting
-``TAGGIT_STRING_FROM_TAGS`` to override the default value (which is
-``tag_fields.utils._edit_string_for_tags``):
+|
+
+To use a specific function instead of the string parser, add a new setting
+called "TAGGIT_TAGS_FROM_STRING" and provide its dotted path to your desired
+function.
+
+
+You can also offer a function that transforms a collection of tags into a
+string format. To change the default value
+(which is "tag_fields.utils._edit_string_for_tags"), use the
+"TAGGIT_STRING_FROM_TAGS" setting.
 
   .. code-block:: python
 
     def comma_joiner(tags):
         return ', '.join(t.name for t in tags)
 
-If the functions above were defined in a module, ``appname.utils``, then your
-project settings.py file should contain the following:
+To define the above functions in a module called "appname.utils", your
+project's settings.py file should include the following.
 
   .. code-block:: python
 
     TAGGIT_TAGS_FROM_STRING = 'appname.utils.comma_splitter'
     TAGGIT_STRING_FROM_TAGS = 'appname.utils.comma_joiner'
```

### Comparing `django-tag-fields-4.0.0/docs/external_apps.rst` & `django-tag-fields-4.0.1/docs/external_apps.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/docs/forms.rst` & `django-tag-fields-4.0.1/docs/forms.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/docs/serializers.rst` & `django-tag-fields-4.0.1/docs/serializers.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 Usage With Django Rest Framework
 ================================
 
-Because the tags in `django-tag-fields` need to be added into a `TaggableManager()`
-we cannot use the usual `Serializer` that we get from Django REST Framework.
-Because this is trying to save the tags into a `list`, which will throw an exception.
+Because the tags in ``django-tag-fields`` need to be added into a ``TaggableManager()``
+we cannot use the usual ``Serializer`` that we get from Django REST Framework.
+Because this is trying to save the tags into a ``list``, which will throw an exception.
 
-To accept tags through a `REST` API call we need to add the following to our `Serializer`::
+To accept tags through a `REST` API call we need to add the following to our ``Serializer``.
 
 
-    from tag_fields.serializers import (TagListSerializerField,
-                                    TaggitSerializer)
+.. code-block:: python
 
+    from tag_fields.serializers import (
+                                        TagListSerializerField,
+                                        TaggitSerializer,
+                                        )
 
-    class YourSerializer(TaggitSerializer, serializers.ModelSerializer):
 
-        tags = TagListSerializerField()
+    class YourSerializer(
+                          TaggitSerializer,
+                          serializers.ModelSerializer,
+                        ):
 
         class Meta:
             model = YourModel
             fields = '__all__'
 
+        tags = TagListSerializerField()
+
+
+
 And you're done, so now you can add tags to your model.
```

### Comparing `django-tag-fields-4.0.0/tag_fields/forms.py` & `django-tag-fields-4.0.1/tag_fields/forms.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/ar/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/ar/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/cs/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/cs/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/da/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/da/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/de/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/de/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/el/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/el/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/en/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/eo/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/eo/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/eo/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/es/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/es/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/fa/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/fa/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/fi/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/fi/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/fr/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/fr/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/he/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/he/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/it/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/it/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/ja/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/ja/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/nb/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/nb/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/nl/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/nl/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/pt_BR/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/pt_BR/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/ru/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/ru/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/tr/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/tr/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/uk/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/uk/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.1/tag_fields/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/locale/zh_Hans/LC_MESSAGES/django.po` & `django-tag-fields-4.0.1/tag_fields/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/managers.py` & `django-tag-fields-4.0.1/tag_fields/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from django.db.models.query_utils import PathInfo
 from django.utils.functional import cached_property
 from django.utils.text import capfirst
 from django.utils.translation import gettext_lazy as _
 
 from tag_fields.forms import TagField
 from tag_fields.models import (
-    CommonGenericTaggedItemBase,
-    GenericUUIDTaggedItemBase,
+    GenericFKTaggedItemThroughBase,
+    UUIDFKTaggedItemThroughBase,
     TaggedItem,
 )
 from tag_fields.utils import require_instance_manager
 
 
 class ExtraJoinRestriction:
     """
@@ -43,29 +43,38 @@
 
     def as_sql(self, compiler, connection):
         qn = compiler.quote_name_unless_alias
         if len(self.content_types) == 1:
             extra_where = f"{qn(self.alias)}.{qn(self.col)} = %s"
         else:
             extra_where = "{}.{} IN ({})".format(
-                qn(self.alias), qn(self.col), ",".join(["%s"] * len(self.content_types))
+                qn(self.alias),
+                qn(self.col),
+                ",".join(["%s"] * len(self.content_types)),
             )
         return extra_where, self.content_types
 
     def relabel_aliases(self, change_map):
         self.alias = change_map.get(self.alias, self.alias)
 
     def clone(self):
         return type(self)(self.alias, self.col, self.content_types[:])
 
 
 class _TaggableManager(models.Manager):
-    # TODO investigate whether we can use a RelatedManager instead of all this stuff
-    # to take advantage of all the Django goodness
-    def __init__(self, through, model, instance, prefetch_cache_name, ordering=None):
+    # TODO investigate whether we can use a RelatedManager instead of all this
+    # stuff to take advantage of all the Django goodness
+    def __init__(
+        self,
+        through,
+        model,
+        instance,
+        prefetch_cache_name,
+        ordering=None,
+    ):
         super().__init__()
         self.through = through
         self.model = model
         self.instance = instance
         self.prefetch_cache_name = prefetch_cache_name
         if ordering:
             self.ordering = ordering
@@ -73,31 +82,33 @@
             self.ordering = []
 
     def is_cached(self, instance):
         return self.prefetch_cache_name in instance._prefetched_objects_cache
 
     def get_queryset(self, extra_filters=None):
         try:
-            return self.instance._prefetched_objects_cache[self.prefetch_cache_name]
+            return self.instance._prefetched_objects_cache[
+                self.prefetch_cache_name
+            ]
         except (AttributeError, KeyError):
             kwargs = extra_filters if extra_filters else {}
-            return self.through.tags_for(self.model, self.instance, **kwargs).order_by(
-                *self.ordering
-            )
+            return self.through.tags_for(
+                self.model, self.instance, **kwargs
+            ).order_by(*self.ordering)
 
     def get_prefetch_queryset(self, instances, queryset=None):
         if queryset is not None:
             raise ValueError("Custom queryset can't be used for this lookup.")
 
         instance = instances[0]
         db = self._db or router.db_for_read(type(instance), instance=instance)
 
         fieldname = (
             "object_id"
-            if issubclass(self.through, CommonGenericTaggedItemBase)
+            if issubclass(self.through, GenericFKTaggedItemThroughBase)
             else "content_object"
         )
         fk = self.through._meta.get_field(fieldname)
         query = {
             "%s__%s__in"
             % (self.through.tag_relname(), fk.name): {
                 obj._get_pk_val() for obj in instances
@@ -115,15 +126,15 @@
                     "_prefetch_related_val": "{}.{}".format(
                         qn(join_table), qn(source_col)
                     )
                 }
             )
         )
 
-        if issubclass(self.through, GenericUUIDTaggedItemBase):
+        if issubclass(self.through, UUIDFKTaggedItemThroughBase):
 
             def uuid_rel_obj_attr(v):
                 value = attrgetter("_prefetch_related_val")(v)
                 if value is not None and not isinstance(value, uuid.UUID):
                     input_form = "int" if isinstance(value, int) else "hex"
                     value = uuid.UUID(**{input_form: value})
                 return value
@@ -141,15 +152,17 @@
             False,
         )
 
     def _lookup_kwargs(self):
         return self.through.lookup_kwargs(self.instance)
 
     def _remove_prefetched_objects(self):
-        prefetch_cache = getattr(self.instance, "_prefetched_objects_cache", None)
+        prefetch_cache = getattr(
+            self.instance, "_prefetched_objects_cache", None
+        )
         if prefetch_cache:
             prefetch_cache.pop(self.prefetch_cache_name, None)
 
     @require_instance_manager
     def add(self, *tags, through_defaults=None, tag_kwargs=None, **kwargs):
         self._remove_prefetched_objects()
         if tag_kwargs is None:
@@ -242,15 +255,17 @@
 
         for new_tag in tags_to_create:
             if case_insensitive:
                 lookup = {"name__iexact": new_tag, **tag_kwargs}
             else:
                 lookup = {"name": new_tag, **tag_kwargs}
 
-            tag, create = manager.get_or_create(**lookup, defaults={"name": new_tag})
+            tag, create = manager.get_or_create(
+                **lookup, defaults={"name": new_tag}
+            )
             tag_objs.add(tag)
 
         return tag_objs
 
     @require_instance_manager
     def names(self):
         return self.get_queryset().values_list("name", flat=True)
@@ -346,15 +361,17 @@
             instance=self.instance,
             reverse=False,
             model=self.through.tag_model(),
             pk_set=None,
             using=db,
         )
 
-        self.through._default_manager.using(db).filter(**self._lookup_kwargs()).delete()
+        self.through._default_manager.using(db).filter(
+            **self._lookup_kwargs()
+        ).delete()
 
         signals.m2m_changed.send(
             sender=self.through,
             action="post_clear",
             instance=self.instance,
             reverse=False,
             model=self.through.tag_model(),
@@ -390,29 +407,33 @@
             # somehow?
             f = self.through._meta.get_field(lookup_keys[0])
             remote_field = f.remote_field
             rel_model = remote_field.model
             objs = rel_model._default_manager.filter(
                 **{
                     "%s__in"
-                    % remote_field.field_name: [r["content_object"] for r in qs]
+                    % remote_field.field_name: [
+                        r["content_object"] for r in qs
+                    ]
                 }
             )
             actual_remote_field_name = f.target_field.get_attname()
             for obj in objs:
                 items[(getattr(obj, actual_remote_field_name),)] = obj
         else:
             preload = {}
             for result in qs:
                 preload.setdefault(result["content_type"], set())
                 preload[result["content_type"]].add(result["object_id"])
 
             for ct, obj_ids in preload.items():
                 ct = ContentType.objects.get_for_id(ct)
-                for obj in ct.model_class()._default_manager.filter(pk__in=obj_ids):
+                for obj in ct.model_class()._default_manager.filter(
+                    pk__in=obj_ids
+                ):
                     items[(ct.pk, obj.pk)] = obj
 
         results = []
         for result in qs:
             obj = items[tuple(result[k] for k in lookup_keys)]
             obj.similar_tags = result["n"]
             results.append(obj)
@@ -437,15 +458,17 @@
         related_name=None,
         to=None,
         ordering=None,
         manager=_TaggableManager,
     ):
         self.through = through or TaggedItem
 
-        rel = ManyToManyRel(self, to, related_name=related_name, through=self.through)
+        rel = ManyToManyRel(
+            self, to, related_name=related_name, through=self.through
+        )
 
         super().__init__(
             verbose_name=verbose_name,
             help_text=help_text,
             blank=blank,
             null=True,
             serialize=False,
@@ -475,15 +498,15 @@
         Deconstruct the object, used with migrations.
         """
         name, path, args, kwargs = super().deconstruct()
         # Remove forced kwargs.
         for kwarg in ("serialize", "null"):
             del kwargs[kwarg]
         # Add arguments related to relations.
-        # Ref: https://github.com/jazzband/django-taggit/issues/206#issuecomment-37578676
+        # Ref: https://github.com/jazzband/django-taggit/issues/206#issuecomment-37578676 # noqa: E501
         rel = self.remote_field
         if isinstance(rel.through, str):
             kwargs["through"] = rel.through
         elif not rel.through._meta.auto_created:
             kwargs["through"] = "{}.{}".format(
                 rel.through._meta.app_label, rel.through._meta.object_name
             )
@@ -508,15 +531,18 @@
         if not cls._meta.abstract:
             if isinstance(self.remote_field.model, str):
 
                 def resolve_related_class(cls, model, field):
                     field.remote_field.model = model
 
                 lazy_related_operation(
-                    resolve_related_class, cls, self.remote_field.model, field=self
+                    resolve_related_class,
+                    cls,
+                    self.remote_field.model,
+                    field=self,
                 )
             if isinstance(self.through, str):
 
                 def resolve_related_class(cls, model, field):
                     self.through = model
                     self.remote_field.through = model
                     self.post_through_setup(cls)
@@ -528,15 +554,15 @@
                 self.post_through_setup(cls)
 
     def get_internal_type(self):
         return "ManyToManyField"
 
     def post_through_setup(self, cls):
         self.use_gfk = self.through is None or issubclass(
-            self.through, CommonGenericTaggedItemBase
+            self.through, GenericFKTaggedItemThroughBase
         )
 
         if not self.remote_field.model:
             self.remote_field.model = self.through._meta.get_field(
                 "tag"
             ).remote_field.model
 
@@ -595,19 +621,21 @@
 
     def bulk_related_objects(self, new_objs, using):
         return []
 
     def _get_mm_case_path_info(self, direct=False, filtered_relation=None):
         pathinfos = []
         linkfield1 = self.through._meta.get_field("content_object")
-        linkfield2 = self.through._meta.get_field(self.m2m_reverse_field_name())
+        linkfield2 = self.through._meta.get_field(
+            self.m2m_reverse_field_name()
+        )
         if django.VERSION >= (4, 1) and not filtered_relation:
-            # Django >= 4.1 provides cached path_infos and reverse_path_infos properties
-            # to use in preference to get_path_info / get_reverse_path_info when not
-            # passing a filtered_relation
+            # Django >= 4.1 provides cached path_infos and reverse_path_infos
+            # properties to use in preference to get_path_info /
+            # get_reverse_path_info when not passing a filtered_relation
             if direct:
                 join1infos = linkfield1.reverse_path_infos
                 join2infos = linkfield2.path_infos
             else:
                 join1infos = linkfield2.reverse_path_infos
                 join2infos = linkfield1.path_infos
         else:
@@ -699,19 +727,37 @@
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
@@ -725,19 +771,26 @@
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
-        return [(self.through._meta.get_field("object_id"), self.model._meta.pk)]
+        return [
+            (self.through._meta.get_field("object_id"), self.model._meta.pk)
+        ]
 
     @property
     def foreign_related_fields(self):
         return [self.related_fields[0][1]]
 
 
 def _get_subclasses(model):
```

### Comparing `django-tag-fields-4.0.0/tag_fields/migrations/0001_initial.py` & `django-tag-fields-4.0.1/tag_fields/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/migrations/0004_alter_taggeditem_content_type_alter_taggeditem_tag.py` & `django-tag-fields-4.0.1/tag_fields/migrations/0004_alter_taggeditem_content_type_alter_taggeditem_tag.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/models.py` & `django-tag-fields-4.0.1/tag_fields/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,16 +12,23 @@
 except ImportError:
 
     def unidecode(tag):
         return tag
 
 
 class TagBase(models.Model):
+    """Abstract Base class for the tags."""
+
+    class Meta:
+        abstract = True
+
     name = models.CharField(
-        verbose_name=pgettext_lazy("A tag name", "name"), unique=True, max_length=100
+        verbose_name=pgettext_lazy("A tag name", "name"),
+        unique=True,
+        max_length=100,
     )
     slug = models.SlugField(
         verbose_name=pgettext_lazy("A tag slug", "slug"),
         unique=True,
         max_length=100,
         allow_unicode=True,
     )
@@ -31,17 +38,14 @@
 
     def __gt__(self, other):
         return self.name.lower() > other.name.lower()
 
     def __lt__(self, other):
         return self.name.lower() < other.name.lower()
 
-    class Meta:
-        abstract = True
-
     def save(self, *args, **kwargs):
         if self._state.adding and not self.slug:
             self.slug = self.slugify(self.name)
             using = kwargs.get("using") or router.db_for_write(
                 type(self), instance=self
             )
             # Make sure we write to the same db for all attempted writes,
@@ -81,30 +85,45 @@
             slug = slugify(tag, allow_unicode=True)
         if i is not None:
             slug += "_%d" % i
         return slug
 
 
 class Tag(TagBase):
+    """Model tag for use with your own model.
+
+    This is a model level tag, i.e. there can only be one per model.
+
+    """
+
     class Meta:
         verbose_name = _("tag")
         verbose_name_plural = _("tags")
         app_label = "tag_fields"
 
 
-class ItemBase(models.Model):
+class ThroughTableBase(models.Model):
+    """Base class for a model ``tags`` through table.
+
+    Abstract Base Class: ``through table`` for all ``through table``
+    sub classes.
+
+    taggit class name was ItemBase
+
+    """
+
+    class Meta:
+        abstract = True
+
     def __str__(self):
         return gettext("%(object)s tagged with %(tag)s") % {
             "object": self.content_object,
             "tag": self.tag,
         }
 
-    class Meta:
-        abstract = True
-
     @classmethod
     def tag_model(cls):
         field = cls._meta.get_field("tag")
         return field.remote_field.model
 
     @classmethod
     def tag_relname(cls):
@@ -117,39 +136,61 @@
 
     @classmethod
     def tags_for(cls, model, instance=None, **extra_filters):
         kwargs = extra_filters or {}
         if instance is not None:
             kwargs.update({"%s__content_object" % cls.tag_relname(): instance})
             return cls.tag_model().objects.filter(**kwargs)
-        kwargs.update({"%s__content_object__isnull" % cls.tag_relname(): False})
+        kwargs.update(
+            {"%s__content_object__isnull" % cls.tag_relname(): False}
+        )
         return cls.tag_model().objects.filter(**kwargs).distinct()
 
 
-class TaggedItemBase(ItemBase):
+class TaggedItemThroughBase(ThroughTableBase):
+    """Sub class of ``ThroughTableBase``
+
+    Base class: ``through table`` for a ``Tagged Item`` model.
+
+    taggit class name was TaggedItemBase
+
+    """
+
+    class Meta:
+        abstract = True
+
     tag = models.ForeignKey(
-        Tag, related_name="%(app_label)s_%(class)s_items", on_delete=models.CASCADE
+        Tag,
+        related_name="%(app_label)s_%(class)s_items",
+        on_delete=models.CASCADE,
     )
 
+
+class GenericFKTaggedItemThroughBase(ThroughTableBase):
+    """Abstract subclass of ``ThroughTableBase`` using a ``GenericForeignKey``.
+
+    Base class: ``through table`` for a ``Tagged Item`` model using an
+    ``GenericForeignKey``.
+
+    taggit class name was CommonGenericTaggedItemBase
+
+
+    """
+
     class Meta:
         abstract = True
 
-
-class CommonGenericTaggedItemBase(ItemBase):
     content_type = models.ForeignKey(
         ContentType,
         on_delete=models.CASCADE,
         verbose_name=_("content type"),
         related_name="%(app_label)s_%(class)s_tagged_items",
     )
     content_object = GenericForeignKey()
 
-    class Meta:
-        abstract = True
-
     @classmethod
     def lookup_kwargs(cls, instance):
         return {
             "object_id": instance.pk,
             "content_type": ContentType.objects.get_for_model(instance),
         }
 
@@ -164,28 +205,61 @@
         if instance is not None:
             kwargs["%s__object_id" % tag_relname] = instance.pk
         if extra_filters:
             kwargs.update(extra_filters)
         return cls.tag_model().objects.filter(**kwargs).distinct()
 
 
-class GenericTaggedItemBase(CommonGenericTaggedItemBase):
-    object_id = models.IntegerField(verbose_name=_("object ID"), db_index=True)
+class IntegerFKTaggedItemThroughBase(GenericFKTaggedItemThroughBase):
+    """Abstract subclass of ``GenericFKTaggedItemThroughBase`` with
+     ``Integer Foreign Key``.
+
+    Base class: ``through table`` for a ``Tagged Item`` model using an
+    ``integer`` primary key.
+
+    taggit class name was GenericTaggedItemBase
+
+    """
 
     class Meta:
         abstract = True
 
+    object_id = models.IntegerField(verbose_name=_("object ID"), db_index=True)
 
-class GenericUUIDTaggedItemBase(CommonGenericTaggedItemBase):
-    object_id = models.UUIDField(verbose_name=_("object ID"), db_index=True)
+
+class UUIDFKTaggedItemThroughBase(GenericFKTaggedItemThroughBase):
+    """Abstract subclass of CommonGenericTaggedItemBase with a
+      ```UUID Foreign Key``.
+
+    Base class: ``through table`` for a ``Tagged Item`` model using an ``UUID``
+    primary key.
+
+    taggit class name was GenericUUIDTaggedItemBase
+
+    """
 
     class Meta:
         abstract = True
 
+    object_id = models.UUIDField(verbose_name=_("object ID"), db_index=True)
+
+
+class TaggedItem(IntegerFKTaggedItemThroughBase, TaggedItemThroughBase):
+    """Tagged Item Through Table using Integer Foreign Key.
+
+    Allows custom Tag models. Tagged models use a ``Integer`` primary key.
+
+    taggit class name was TaggedItem
+
+    .. note::
+
+        Changing this class name breaks the tests. Some checks made to see what
+        was causing the error but it requires more time.
+
+    """
 
-class TaggedItem(GenericTaggedItemBase, TaggedItemBase):
     class Meta:
         verbose_name = _("tagged item")
         verbose_name_plural = _("tagged items")
         app_label = "tag_fields"
         index_together = [["content_type", "object_id"]]
         unique_together = [["content_type", "object_id", "tag"]]
```

### Comparing `django-tag-fields-4.0.0/tag_fields/serializers.py` & `django-tag-fields-4.0.1/tag_fields/serializers.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/utils.py` & `django-tag-fields-4.0.1/tag_fields/utils.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tag_fields/views.py` & `django-tag-fields-4.0.1/tag_fields/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,21 +25,24 @@
         self.tag = get_object_or_404(Tag, slug=slug)
         return super().dispatch(request, *args, **kwargs)
 
     def get_queryset(self, **kwargs):
         qs = super().get_queryset(**kwargs)
         return qs.filter(
             pk__in=TaggedItem.objects.filter(
-                tag=self.tag, content_type=ContentType.objects.get_for_model(qs.model)
+                tag=self.tag,
+                content_type=ContentType.objects.get_for_model(qs.model),
             ).values_list("object_id", flat=True)
         )
 
     def get_template_names(self):
         if self.tag_suffix:
-            self.template_name_suffix = self.tag_suffix + self.template_name_suffix
+            self.template_name_suffix = (
+                self.tag_suffix + self.template_name_suffix
+            )
         return super().get_template_names()
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         if "extra_context" not in context:
             context["extra_context"] = {}
         context["extra_context"]["tag"] = self.tag
```

### Comparing `django-tag-fields-4.0.0/tests/forms.py` & `django-tag-fields-4.0.1/tests/forms.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tests/migrations/0001_initial.py` & `django-tag-fields-4.0.1/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tests/migrations/0002_auto_20200214_1129.py` & `django-tag-fields-4.0.1/tests/migrations/0002_auto_20200214_1129.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tests/migrations/0003_auto_20210310_0918.py` & `django-tag-fields-4.0.1/tests/migrations/0003_auto_20210310_0918.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tests/migrations/0004_auto_20210619_0826.py` & `django-tag-fields-4.0.1/tests/migrations/0004_auto_20210619_0826.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tests/migrations/0005_auto_20210713_2301.py` & `django-tag-fields-4.0.1/tests/migrations/0005_auto_20210713_2301.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tests/models.py` & `django-tag-fields-4.0.1/tests/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 import uuid
 
 from django.db import models
 
 from tag_fields.managers import TaggableManager
 from tag_fields.models import (
-    CommonGenericTaggedItemBase,
-    GenericTaggedItemBase,
-    GenericUUIDTaggedItemBase,
-    ItemBase,
+    GenericFKTaggedItemThroughBase,
+    IntegerFKTaggedItemThroughBase,
+    UUIDFKTaggedItemThroughBase,
+    ThroughTableBase,
     Tag,
     TagBase,
     TaggedItem,
-    TaggedItemBase,
+    TaggedItemThroughBase,
 )
 
 
 # base test model
 class TestModel(models.Model):
     tags = TaggableManager()
 
 
 # Ensure that two TaggableManagers with custom through model are allowed.
-class Through1(TaggedItemBase):
-    content_object = models.ForeignKey("MultipleTags", on_delete=models.CASCADE)
+class Through1(TaggedItemThroughBase):
+    content_object = models.ForeignKey(
+        "MultipleTags", on_delete=models.CASCADE
+    )
 
 
-class Through2(TaggedItemBase):
-    content_object = models.ForeignKey("MultipleTags", on_delete=models.CASCADE)
+class Through2(TaggedItemThroughBase):
+    content_object = models.ForeignKey(
+        "MultipleTags", on_delete=models.CASCADE
+    )
 
 
 class MultipleTags(models.Model):
     tags1 = TaggableManager(through=Through1, related_name="tags1")
     tags2 = TaggableManager(through=Through2, related_name="tags2")
 
 
-# Ensure that two TaggableManagers with GFK via different through models are allowed.
-class ThroughGFK(GenericTaggedItemBase):
-    tag = models.ForeignKey(Tag, related_name="tagged_items", on_delete=models.CASCADE)
+# Ensure that two TaggableManagers with GFK via different through
+# models are allowed.
+class ThroughGFK(IntegerFKTaggedItemThroughBase):
+    tag = models.ForeignKey(
+        Tag, related_name="tagged_items", on_delete=models.CASCADE
+    )
 
 
 class MultipleTagsGFK(models.Model):
     tags1 = TaggableManager(related_name="tagsgfk1")
     tags2 = TaggableManager(through=ThroughGFK, related_name="tagsgfk2")
 
 
@@ -65,17 +72,19 @@
 class BaseFood(models.Model):
     name = models.CharField(max_length=50)
 
     def __str__(self):
         return self.name
 
 
-class MultiInheritanceLazyResolutionFoodTag(TaggedItemBase):
+class MultiInheritanceLazyResolutionFoodTag(TaggedItemThroughBase):
     content_object = models.ForeignKey(
-        "MultiInheritanceFood", related_name="tagged_items", on_delete=models.CASCADE
+        "MultiInheritanceFood",
+        related_name="tagged_items",
+        on_delete=models.CASCADE,
     )
 
     class Meta:
         unique_together = [["content_object", "tag"]]
 
 
 class MultiInheritanceFood(BaseFood):
@@ -97,22 +106,22 @@
 class HousePet(Pet):
     trained = models.BooleanField(default=False)
 
 
 # Test direct-tagging with custom through model
 
 
-class TaggedFood(TaggedItemBase):
+class TaggedFood(TaggedItemThroughBase):
     content_object = models.ForeignKey("DirectFood", on_delete=models.CASCADE)
 
     class Meta:
         unique_together = [["content_object", "tag"]]
 
 
-class TaggedPet(TaggedItemBase):
+class TaggedPet(TaggedItemThroughBase):
     content_object = models.ForeignKey("DirectPet", on_delete=models.CASCADE)
 
 
 class DirectFood(models.Model):
     name = models.CharField(max_length=50)
 
     tags = TaggableManager(through="TaggedFood")
@@ -139,28 +148,32 @@
 
 class TrackedTag(TagBase):
     created_by = models.CharField(max_length=50)
     created_dt = models.DateTimeField(auto_now_add=True)
     description = models.TextField(blank=True, max_length=255, null=True)
 
 
-class TaggedTrackedFood(ItemBase):
-    content_object = models.ForeignKey("DirectTrackedFood", on_delete=models.CASCADE)
+class TaggedTrackedFood(ThroughTableBase):
+    content_object = models.ForeignKey(
+        "DirectTrackedFood", on_delete=models.CASCADE
+    )
     tag = models.ForeignKey(
         TrackedTag, on_delete=models.CASCADE, related_name="%(class)s_items"
     )
     created_by = models.CharField(max_length=50)
     created_dt = models.DateTimeField(auto_now_add=True)
 
     class Meta:
         unique_together = ["content_object", "tag"]
 
 
-class TaggedTrackedPet(ItemBase):
-    content_object = models.ForeignKey("DirectTrackedPet", on_delete=models.CASCADE)
+class TaggedTrackedPet(ThroughTableBase):
+    content_object = models.ForeignKey(
+        "DirectTrackedPet", on_delete=models.CASCADE
+    )
     tag = models.ForeignKey(
         TrackedTag, on_delete=models.CASCADE, related_name="%(class)s_items"
     )
     created_by = models.CharField(max_length=50)
     created_dt = models.DateTimeField(auto_now_add=True)
 
 
@@ -185,23 +198,27 @@
 class DirectTrackedHousePet(DirectTrackedPet):
     trained = models.BooleanField(default=False)
 
 
 # Test custom through model to model with custom PK
 
 
-class TaggedCustomPKFood(TaggedItemBase):
-    content_object = models.ForeignKey("DirectCustomPKFood", on_delete=models.CASCADE)
+class TaggedCustomPKFood(TaggedItemThroughBase):
+    content_object = models.ForeignKey(
+        "DirectCustomPKFood", on_delete=models.CASCADE
+    )
 
     class Meta:
         unique_together = [["content_object", "tag"]]
 
 
-class TaggedCustomPKPet(TaggedItemBase):
-    content_object = models.ForeignKey("DirectCustomPKPet", on_delete=models.CASCADE)
+class TaggedCustomPKPet(TaggedItemThroughBase):
+    content_object = models.ForeignKey(
+        "DirectCustomPKPet", on_delete=models.CASCADE
+    )
 
     class Meta:
         unique_together = [["content_object", "tag"]]
 
 
 class DirectCustomPKFood(models.Model):
     name = models.CharField(max_length=50, primary_key=True)
@@ -221,16 +238,18 @@
 
 
 class DirectCustomPKHousePet(DirectCustomPKPet):
     trained = models.BooleanField(default=False)
 
 
 # Test custom through model to model with custom PK using GenericForeignKey
-class TaggedCustomPK(CommonGenericTaggedItemBase, TaggedItemBase):
-    object_id = models.CharField(max_length=50, verbose_name="Object id", db_index=True)
+class TaggedCustomPK(GenericFKTaggedItemThroughBase, TaggedItemThroughBase):
+    object_id = models.CharField(
+        max_length=50, verbose_name="Object id", db_index=True
+    )
 
     class Meta:
         unique_together = [["object_id", "tag"]]
 
 
 class CustomPKFood(models.Model):
     name = models.CharField(max_length=50, primary_key=True)
@@ -257,15 +276,15 @@
 # Test custom through model to a custom tag model
 
 
 class OfficialTag(TagBase):
     official = models.BooleanField(default=False)
 
 
-class OfficialThroughModel(GenericTaggedItemBase):
+class OfficialThroughModel(IntegerFKTaggedItemThroughBase):
     tag = models.ForeignKey(
         OfficialTag, related_name="tagged_items", on_delete=models.CASCADE
     )
     extra_field = models.CharField(max_length=10)
 
     class Meta:
         unique_together = [["content_type", "object_id", "tag"]]
@@ -363,52 +382,58 @@
 
     created_at = models.DateTimeField(auto_now_add=True)
 
     def __str__(self):
         return self.name
 
     class Meta:
-        # With a UUIDField pk, objects are not always ordered by creation time. So explicitly set ordering.
+        # With a UUIDField pk, objects are not always ordered by creation time.
+        # So explicitly set ordering.
         ordering = ["created_at"]
 
 
 class UUIDPet(models.Model):
     id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
     name = models.CharField(max_length=50)
 
     tags = TaggableManager(through="UUIDTaggedItem")
     created_at = models.DateTimeField(auto_now_add=True)
 
     def __str__(self):
         return self.name
 
     class Meta:
-        # With a UUIDField pk, objects are not always ordered by creation time. So explicitly set ordering.
+        # With a UUIDField pk, objects are not always ordered by creation time.
+        # So explicitly set ordering.
         ordering = ["created_at"]
 
 
 class UUIDHousePet(UUIDPet):
     trained = models.BooleanField(default=False)
 
 
 class UUIDTag(TagBase):
     id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
 
 
-class UUIDTaggedItem(GenericUUIDTaggedItemBase):
+class UUIDTaggedItem(UUIDFKTaggedItemThroughBase):
     tag = models.ForeignKey(
-        UUIDTag, related_name="%(app_label)s_%(class)s_items", on_delete=models.CASCADE
+        UUIDTag,
+        related_name="%(app_label)s_%(class)s_items",
+        on_delete=models.CASCADE,
     )
 
     class Meta:
         unique_together = [["content_type", "object_id", "tag"]]
 
 
 # Exists to verify system check failure.
-# tests.Name.tags: (fields.E303) Reverse query name for 'Name.tags' clashes with field name 'Tag.name'.
-# 	HINT: Rename field 'Tag.name', or add/change a related_name argument to the definition for field 'Name.tags'.
+# tests.Name.tags: (fields.E303) Reverse query name for 'Name.tags' clashes
+# with field name 'Tag.name'.
+# 	HINT: Rename field 'Tag.name', or add/change a related_name argument to
+# the definition for field 'Name.tags'.
 class Name(models.Model):
     tags = TaggableManager(related_name="a_unique_related_name")
 
 
 class OrderedModel(models.Model):
     tags = TaggableManager(ordering=["name"])
```

### Comparing `django-tag-fields-4.0.0/tests/settings.py` & `django-tag-fields-4.0.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tests/test_admin.py` & `django-tag-fields-4.0.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tests/test_forms.py` & `django-tag-fields-4.0.1/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tests/test_models.py` & `django-tag-fields-4.0.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tests/test_serializers.py` & `django-tag-fields-4.0.1/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tests/test_utils.py` & `django-tag-fields-4.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.0/tests/tests.py` & `django-tag-fields-4.0.1/tests/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from io import StringIO
 from unittest import mock
 import django
 
+from django import VERSION as DJANGO_VERSION
+
 from django.contrib.contenttypes.models import ContentType
 from django.core import serializers
 from django.core.exceptions import ValidationError
 from django.core.management import call_command
 from django.db import IntegrityError, connection, models
 from django.test import RequestFactory, SimpleTestCase, TestCase
 from django.test.utils import override_settings
@@ -198,15 +200,17 @@
         self.assert_tags_equal(self.food_model.tags.all(), ["green", "red"])
 
         self.assert_tags_equal(
             self.food_model.tags.most_common(), ["green", "red"], sort=False
         )
 
         self.assert_tags_equal(
-            self.food_model.tags.most_common(min_count=2), ["green"], sort=False
+            self.food_model.tags.most_common(min_count=2),
+            ["green"],
+            sort=False,
         )
 
         apple.tags.remove("green")
         self.assert_tags_equal(apple.tags.all(), ["red"])
         self.assert_tags_equal(self.food_model.tags.all(), ["green", "red"])
         tag = self.tag_model.objects.create(name="delicious")
         apple.tags.add(tag)
@@ -479,48 +483,50 @@
             ]
         )
 
     def test_add_queries(self):
         # Prefill content type cache:
         ContentType.objects.get_for_model(self.food_model)
         apple = self.food_model.objects.create(name="apple")
-        # 1. SELECT "tag_fields_tag"."id", "tag_fields_tag"."name", "tag_fields_tag"."slug" FROM "tag_fields_tag" WHERE "tag_fields_tag"."name" IN ('green', 'red', 'delicious')
-        # 2. SELECT "tag_fields_tag"."id", "tag_fields_tag"."name", "tag_fields_tag"."slug" FROM "tag_fields_tag" WHERE "tag_fields_tag"."name" = 'green'
+        # 1. SELECT "tag_fields_tag"."id", "tag_fields_tag"."name", "tag_fields_tag"."slug" FROM "tag_fields_tag" WHERE "tag_fields_tag"."name" IN ('green', 'red', 'delicious') # noqa: E501
+        # 2. SELECT "tag_fields_tag"."id", "tag_fields_tag"."name", "tag_fields_tag"."slug" FROM "tag_fields_tag" WHERE "tag_fields_tag"."name" = 'green' # noqa: E501
         # 3. SAVEPOINT
         # 4. SAVEPOINT
-        # 5. INSERT INTO "tag_fields_tag" ("name", "slug") VALUES ('green', 'green')
+        # 5. INSERT INTO "tag_fields_tag" ("name", "slug") VALUES ('green', 'green') # noqa: E501
         # 6. RELEASE SAVEPOINT
         # 7. RELEASE SAVEPOINT
-        # 8. SELECT "tag_fields_tag"."id", "tag_fields_tag"."name", "tag_fields_tag"."slug" FROM "tag_fields_tag" WHERE "tag_fields_tag"."name" = 'red'
+        # 8. SELECT "tag_fields_tag"."id", "tag_fields_tag"."name", "tag_fields_tag"."slug" FROM "tag_fields_tag" WHERE "tag_fields_tag"."name" = 'red' # noqa: E501
         # 9. SAVEPOINT
         # 10. SAVEPOINT
-        # 11. INSERT INTO "tag_fields_tag" ("name", "slug") VALUES ('red', 'red')
+        # 11. INSERT INTO "tag_fields_tag" ("name", "slug") VALUES ('red', 'red') # noqa: E501
         # 12. RELEASE SAVEPOINT
         # 13. RELEASE SAVEPOINT
-        # 14. SELECT "tag_fields_tag"."id", "tag_fields_tag"."name", "tag_fields_tag"."slug" FROM "tag_fields_tag" WHERE "tag_fields_tag"."name" = 'delicious'
+        # 14. SELECT "tag_fields_tag"."id", "tag_fields_tag"."name", "tag_fields_tag"."slug" FROM "tag_fields_tag" WHERE "tag_fields_tag"."name" = 'delicious' # noqa: E501
         # 15. SAVEPOINT
         # 16. SAVEPOINT
-        # 17. INSERT INTO "tag_fields_tag" ("name", "slug") VALUES ('delicious', 'delicious')
+        # 17. INSERT INTO "tag_fields_tag" ("name", "slug") VALUES ('delicious', 'delicious') # noqa: E501
         # 18. RELEASE SAVEPOINT
         # 19. RELEASE SAVEPOINT
-        # 20. SELECT "tag_fields_taggeditem"."tag_id" FROM "tag_fields_taggeditem" WHERE ("tag_fields_taggeditem"."content_type_id" = 20 AND "tag_fields_taggeditem"."object_id" = 1)
-        # 21. SELECT "tag_fields_taggeditem"."id", "tag_fields_taggeditem"."tag_id", "tag_fields_taggeditem"."content_type_id", "tag_fields_taggeditem"."object_id" FROM "tag_fields_taggeditem" WHERE ("tag_fields_taggeditem"."content_type_id" = 20 AND "tag_fields_taggeditem"."object_id" = 1 AND "tag_fields_taggeditem"."tag_id" = 1)
+        # 20. SELECT "tag_fields_taggeditem"."tag_id" FROM "tag_fields_taggeditem" WHERE ("tag_fields_taggeditem"."content_type_id" = 20 AND "tag_fields_taggeditem"."object_id" = 1) # noqa: E501
+        # 21. SELECT "tag_fields_taggeditem"."id", "tag_fields_taggeditem"."tag_id", "tag_fields_taggeditem"."content_type_id", "tag_fields_taggeditem"."object_id" FROM "tag_fields_taggeditem" WHERE ("tag_fields_taggeditem"."content_type_id" = 20 AND "tag_fields_taggeditem"."object_id" = 1 AND "tag_fields_taggeditem"."tag_id" = 1) # noqa: E501
         # 22. SAVEPOINT
-        # 23. INSERT INTO "tag_fields_taggeditem" ("tag_id", "content_type_id", "object_id") VALUES (1, 20, 1)
+        # 23. INSERT INTO "tag_fields_taggeditem" ("tag_id", "content_type_id", "object_id") VALUES (1, 20, 1) # noqa: E501
         # 24. RELEASE SAVEPOINT
-        # 25. SELECT "tag_fields_taggeditem"."id", "tag_fields_taggeditem"."tag_id", "tag_fields_taggeditem"."content_type_id", "tag_fields_taggeditem"."object_id" FROM "tag_fields_taggeditem" WHERE ("tag_fields_taggeditem"."content_type_id" = 20 AND "tag_fields_taggeditem"."object_id" = 1 AND "tag_fields_taggeditem"."tag_id" = 2)
+        # 25. SELECT "tag_fields_taggeditem"."id", "tag_fields_taggeditem"."tag_id", "tag_fields_taggeditem"."content_type_id", "tag_fields_taggeditem"."object_id" FROM "tag_fields_taggeditem" WHERE ("tag_fields_taggeditem"."content_type_id" = 20 AND "tag_fields_taggeditem"."object_id" = 1 AND "tag_fields_taggeditem"."tag_id" = 2) # noqa: E501
         # 26. SAVEPOINT
-        # 27. INSERT INTO "tag_fields_taggeditem" ("tag_id", "content_type_id", "object_id") VALUES (2, 20, 1)
+        # 27. INSERT INTO "tag_fields_taggeditem" ("tag_id", "content_type_id", "object_id") VALUES (2, 20, 1) # noqa: E501
         # 28. RELEASE SAVEPOINT
-        # 29. SELECT "tag_fields_taggeditem"."id", "tag_fields_taggeditem"."tag_id", "tag_fields_taggeditem"."content_type_id", "tag_fields_taggeditem"."object_id" FROM "tag_fields_taggeditem" WHERE ("tag_fields_taggeditem"."content_type_id" = 20 AND "tag_fields_taggeditem"."object_id" = 1 AND "tag_fields_taggeditem"."tag_id" = 3)
+        # 29. SELECT "tag_fields_taggeditem"."id", "tag_fields_taggeditem"."tag_id", "tag_fields_taggeditem"."content_type_id", "tag_fields_taggeditem"."object_id" FROM "tag_fields_taggeditem" WHERE ("tag_fields_taggeditem"."content_type_id" = 20 AND "tag_fields_taggeditem"."object_id" = 1 AND "tag_fields_taggeditem"."tag_id" = 3) # noqa: E501
         # 30. SAVEPOINT
-        # 31. INSERT INTO "tag_fields_taggeditem" ("tag_id", "content_type_id", "object_id") VALUES (3, 20, 1)
+        # 31. INSERT INTO "tag_fields_taggeditem" ("tag_id", "content_type_id", "object_id") VALUES (3, 20, 1) # noqa: E501
         # 32. RELEASE SAVEPOINT
         queries = 32
-        self.assertNumQueries(queries, apple.tags.add, "red", "delicious", "green")
+        self.assertNumQueries(
+            queries, apple.tags.add, "red", "delicious", "green"
+        )
 
         pear = self.food_model.objects.create(name="pear")
         #   1 query to see which tags exist
         #   1  query to check existing ids for sending m2m_changed signal
         # + 4 queries to create the intermediary things (including SELECTs, to
         #     make sure we dont't double create.
         # + 4 for save points.
@@ -529,16 +535,16 @@
 
         #   1  query to check existing ids for sending m2m_changed signal
         self.assertNumQueries(1, pear.tags.add)
 
     def test_require_pk(self):
         food_instance = self.food_model()
         msg = (
-            "%s objects need to have a primary key value before you can access "
-            "their tags." % type(self.food_model()).__name__
+            "%s objects need to have a primary key value before you can access"
+            " their tags." % type(self.food_model()).__name__
         )
         with self.assertRaisesMessage(ValueError, msg):
             food_instance.tags.all()
 
     def test_delete_obj(self):
         apple = self.food_model.objects.create(name="apple")
         apple.tags.add("red")
@@ -561,32 +567,39 @@
 
     def test_lookup_by_tag(self):
         apple = self.food_model.objects.create(name="apple")
         apple.tags.add("red", "green")
         pear = self.food_model.objects.create(name="pear")
         pear.tags.add("green")
         self.assertEqual(
-            list(self.food_model.objects.filter(tags__name__in=["red"])), [apple]
+            list(self.food_model.objects.filter(tags__name__in=["red"])),
+            [apple],
         )
         self.assertEqual(
             list(self.food_model.objects.filter(tags__name__in=["green"])),
             [apple, pear],
         )
 
         kitty = self.pet_model.objects.create(name="kitty")
         kitty.tags.add("fuzzy", "red")
         dog = self.pet_model.objects.create(name="dog")
         dog.tags.add("woof", "red")
         self.assertEqual(
-            list(self.food_model.objects.filter(tags__name__in=["red"]).distinct()),
+            list(
+                self.food_model.objects.filter(
+                    tags__name__in=["red"]
+                ).distinct()
+            ),
             [apple],
         )
 
         tag = self.tag_model.objects.get(name="woof")
-        self.assertEqual(list(self.pet_model.objects.filter(tags__in=[tag])), [dog])
+        self.assertEqual(
+            list(self.pet_model.objects.filter(tags__in=[tag])), [dog]
+        )
 
         cat = self.housepet_model.objects.create(name="cat", trained=True)
         cat.tags.add("fuzzy")
 
         pks = self.pet_model.objects.filter(tags__name__in=["fuzzy"])
         model_name = self.pet_model.__name__
 
@@ -638,22 +651,24 @@
                 pks,
                 [f"<{model_name}: pear>", f"<{model_name}: guava>"],
                 ordered=False,
                 transform=repr,
             )
 
     def test_multi_inheritance_similarity_by_tag(self):
-        """Test that pears are more similar to apples than watermelons using multi_inheritance"""
+        """Test pears are more similar to apples than watermelons using multi_inheritance"""  # noqa: E501
         apple = self.multi_inheritance_food_model.objects.create(name="apple")
         apple.tags.add("green", "juicy", "small", "sour")
 
         pear = self.multi_inheritance_food_model.objects.create(name="pear")
         pear.tags.add("green", "juicy", "small", "sweet")
 
-        watermelon = self.multi_inheritance_food_model.objects.create(name="watermelon")
+        watermelon = self.multi_inheritance_food_model.objects.create(
+            name="watermelon"
+        )
         watermelon.tags.add("green", "juicy", "large", "sweet")
 
         similar_objs = apple.tags.similar_objects()
         self.assertEqual(similar_objs, [pear, watermelon])
         self.assertEqual([obj.similar_tags for obj in similar_objs], [3, 2])
 
     def test_similarity_by_tag(self):
@@ -687,29 +702,34 @@
         )
 
     def test_taggeditem_str(self):
         apple = self.food_model.objects.create(name="apple")
         apple.tags.add("juicy")
 
         self.assertEqual(
-            str(self.taggeditem_model.objects.first()), "apple tagged with juicy"
+            str(self.taggeditem_model.objects.first()),
+            "apple tagged with juicy",
         )
 
     def test_taggeditem_through_defaults(self):
         if self.taggeditem_model != OfficialThroughModel:
             self.skipTest(
-                "Through default tests are only run when the tagged item model has extra_field"
+                "Through default tests are only run when the tagged item"
+                "model has extra_field"
             )
         apple = self.food_model.objects.create(name="kiwi")
         apple.tags.add("juicy", through_defaults={"extra_field": "green"})
 
         self.assertEqual(
-            str(self.taggeditem_model.objects.first()), "kiwi tagged with juicy"
+            str(self.taggeditem_model.objects.first()),
+            "kiwi tagged with juicy",
+        )
+        self.assertEqual(
+            self.taggeditem_model.objects.first().extra_field, "green"
         )
-        self.assertEqual(self.taggeditem_model.objects.first().extra_field, "green")
 
     def test_abstract_subclasses(self):
         p = Photo.objects.create()
         p.tags.add("outdoors", "pretty")
         self.assert_tags_equal(p.tags.all(), ["outdoors", "pretty"])
 
         m = Movie.objects.create()
@@ -741,15 +761,17 @@
         apple.tags.add("red")
         self.assertEqual(sorted(list(apple.tags.names())), ["green", "red"])
 
     def test_slugs_method(self):
         apple = self.food_model.objects.create(name="apple")
         apple.tags.add("green and juicy")
         apple.tags.add("red")
-        self.assertEqual(sorted(list(apple.tags.slugs())), ["green-and-juicy", "red"])
+        self.assertEqual(
+            sorted(list(apple.tags.slugs())), ["green-and-juicy", "red"]
+        )
 
     def test_serializes(self):
         apple = self.food_model.objects.create(name="apple")
         serializers.serialize("json", (apple,))
 
     def test_prefetch_related(self):
         apple = self.food_model.objects.create(name="apple")
@@ -757,26 +779,34 @@
         orange = self.food_model.objects.create(name="orange")
         orange.tags.add("2", "4")
         with self.assertNumQueries(2):
             list_prefetched = list(
                 self.food_model.objects.prefetch_related("tags").all()
             )
         with self.assertNumQueries(0):
-            foods = {f.name: {t.name for t in f.tags.all()} for f in list_prefetched}
-            self.assertEqual(foods, {"orange": {"2", "4"}, "apple": {"1", "2"}})
+            foods = {
+                f.name: {t.name for t in f.tags.all()} for f in list_prefetched
+            }
+            self.assertEqual(
+                foods, {"orange": {"2", "4"}, "apple": {"1", "2"}}
+            )
 
     def test_internal_type_is_manytomany(self):
-        self.assertEqual(TaggableManager().get_internal_type(), "ManyToManyField")
+        self.assertEqual(
+            TaggableManager().get_internal_type(), "ManyToManyField"
+        )
 
     def test_prefetch_no_extra_join(self):
         apple = self.food_model.objects.create(name="apple")
         apple.tags.add("1", "2")
         with self.assertNumQueries(2):
             list(self.food_model.objects.prefetch_related("tags").all())
-            join_clause = 'INNER JOIN "%s"' % self.taggeditem_model._meta.db_table
+            join_clause = (
+                'INNER JOIN "%s"' % self.taggeditem_model._meta.db_table
+            )
             self.assertEqual(
                 connection.queries[-1]["sql"].count(join_clause),
                 1,
                 connection.queries[-2:],
             )
 
     @override_settings(TAGGIT_CASE_INSENSITIVE=True)
@@ -881,15 +911,17 @@
         self.tag_model.objects.create(name="delicious", official=True)
         apple = self.food_model.objects.create(name="apple")
         apple.tags.add("delicious", "red")
 
         pear = self.food_model.objects.create(name="Pear")
         pear.tags.add("delicious")
 
-        self.assertEqual(apple, self.food_model.objects.get(tags__official=False))
+        self.assertEqual(
+            apple, self.food_model.objects.get(tags__official=False)
+        )
 
     def test_get_tags_with_count(self):
         apple = self.food_model.objects.create(name="apple")
         apple.tags.add("red", "green", "delicious")
         pear = self.food_model.objects.create(name="pear")
         pear.tags.add("green", "delicious")
 
@@ -909,15 +941,16 @@
 
         pear = self.food_model.objects.create(name="pear")
         pear.tags.add("green")
         pear.tags.add("yellow")
 
         self.assert_tags_equal(
             self.food_model.tags.most_common(
-                min_count=2, extra_filters={"officialfood__name__in": ["pear", "apple"]}
+                min_count=2,
+                extra_filters={"officialfood__name__in": ["pear", "apple"]},
             )[:1],
             ["green"],
             sort=False,
         )
 
         self.assert_tags_equal(
             self.food_model.tags.most_common(
@@ -943,74 +976,137 @@
 
 
 class TaggableFormTestCase(BaseTaggingTestCase):
     form_class = FoodForm
     food_model = Food
 
     def _get_form_str(self, form_str):
-        form_str %= {
-            "help_start": '<span class="helptext">',
-            "help_stop": "</span>",
-            "required": "required",
-        }
+        # Fix as per laymonage https://github.com/jazzband/django-taggit/issues/851 # noqa: E501
+        if DJANGO_VERSION >= (5, 0):
+            # Django defaults to div-based form rendering in 5.0
+            # https://github.com/django/django/commit/98756c685ee173bbd43f21ed0553f808be835ce5 # noqa: E501
+            # https://github.com/django/django/commit/232b60a21b951bd16b8c95b34fcbcbf3ecd89fca # noqa: E501
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
+
+        # Fix as per laymonage https://github.com/jazzband/django-taggit/issues/851 # noqa: E501
+        if DJANGO_VERSION >= (5, 0):
+            self.assertFormRenders(
+                f,
+                """<div><label for="id_name">Name:</label><input id="id_name"
+                type="text" name="name" value="apple" maxlength="50"
+                %(required)s /></div>
+                <div><label for="id_tags">Tags:</label>%(help_start)s
+                A comma-separated list of tags.%(help_stop)s<input type="text"
+                name="tags" value="green, red, yummy" id="id_tags" %(required)s
+                /></div>""",
+            )
+        else:
+            self.assertFormRenders(
+                f,
+                """<tr><th><label for="id_name">Name:</label></th><td><input
+                id="id_name" type="text" name="name" value="apple"
+                maxlength="50" %(required)s /></td></tr><tr><th><label
+                for="id_tags">Tags:</label></th><td><input type="text"
+                name="tags" value="green, red, yummy" id="id_tags"
+                %(required)s /><br />%(help_start)sA comma-separated list of
+                tags.%(help_stop)s</td></tr>""",
+            )
         f.save()
+
         apple = self.food_model.objects.get(name="apple")
         self.assert_tags_equal(apple.tags.all(), ["green", "red", "yummy"])
 
         f = self.form_class(
-            {"name": "apple", "tags": "green, red, yummy, delicious"}, instance=apple
+            {"name": "apple", "tags": "green, red, yummy, delicious"},
+            instance=apple,
         )
         f.save()
         apple = self.food_model.objects.get(name="apple")
-        self.assert_tags_equal(apple.tags.all(), ["green", "red", "yummy", "delicious"])
+        self.assert_tags_equal(
+            apple.tags.all(), ["green", "red", "yummy", "delicious"]
+        )
         self.assertEqual(self.food_model.objects.count(), 1)
 
         f = self.form_class({"name": "raspberry"})
         self.assertFalse(f.is_valid())
 
         f = self.form_class(instance=apple)
-        self.assertFormRenders(
-            f,
-            """<tr><th><label for="id_name">Name:</label></th><td><input id="id_name" type="text" name="name" value="apple" maxlength="50" %(required)s /></td></tr>
-<tr><th><label for="id_tags">Tags:</label></th><td><input type="text" name="tags" value="delicious, green, red, yummy" id="id_tags" %(required)s /><br />%(help_start)sA comma-separated list of tags.%(help_stop)s</td></tr>""",
-        )
+
+        # Fix as per laymonage https://github.com/jazzband/django-taggit/issues/851 # noqa: E501
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
+
+        # Fix as per laymonage https://github.com/jazzband/django-taggit/issues/851 # noqa: E501
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
+
+        # Fix as per laymonage https://github.com/jazzband/django-taggit/issues/851 # noqa: E501
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
-            verbose_name="categories", help_text="Add some categories", blank=True
+            verbose_name="categories",
+            help_text="Add some categories",
+            blank=True,
         )
         ff = tm.formfield()
         self.assertEqual(ff.label, "Categories")
         self.assertEqual(ff.help_text, "Add some categories")
         self.assertEqual(ff.required, False)
 
         self.assertEqual(ff.clean(""), [])
@@ -1139,50 +1235,57 @@
         Test with comma-delimited multiple words.
         An unquoted comma in the input will trigger this.
         """
         self.assertEqual(parse_tags(",one"), ["one"])
         self.assertEqual(parse_tags(",one two"), ["one two"])
         self.assertEqual(parse_tags(",one two three"), ["one two three"])
         self.assertEqual(
-            parse_tags("a-one, a-two and a-three"), ["a-one", "a-two and a-three"]
+            parse_tags("a-one, a-two and a-three"),
+            ["a-one", "a-two and a-three"],
         )
 
     def test_with_double_quoted_multiple_words(self):
         """
         Test with double-quoted multiple words.
         A completed quote will trigger this.  Unclosed quotes are ignored.
         """
         self.assertEqual(parse_tags('"one'), ["one"])
         self.assertEqual(parse_tags('"one two'), ["one", "two"])
         self.assertEqual(parse_tags('"one two three'), ["one", "three", "two"])
         self.assertEqual(parse_tags('"one two"'), ["one two"])
         self.assertEqual(
-            parse_tags('a-one "a-two and a-three"'), ["a-one", "a-two and a-three"]
+            parse_tags('a-one "a-two and a-three"'),
+            ["a-one", "a-two and a-three"],
         )
 
     def test_with_no_loose_commas(self):
         """
         Test with no loose commas -- split on spaces.
         """
-        self.assertEqual(parse_tags('one two "thr,ee"'), ["one", "thr,ee", "two"])
+        self.assertEqual(
+            parse_tags('one two "thr,ee"'), ["one", "thr,ee", "two"]
+        )
 
     def test_with_loose_commas(self):
         """
         Loose commas - split on commas
         """
         self.assertEqual(parse_tags('"one", two three'), ["one", "two three"])
 
     def test_tags_with_double_quotes_can_contain_commas(self):
         """
         Double quotes can contain commas
         """
         self.assertEqual(
-            parse_tags('a-one "a-two, and a-three"'), ["a-one", "a-two, and a-three"]
+            parse_tags('a-one "a-two, and a-three"'),
+            ["a-one", "a-two, and a-three"],
+        )
+        self.assertEqual(
+            parse_tags('"two", one, one, two, "one"'), ["one", "two"]
         )
-        self.assertEqual(parse_tags('"two", one, one, two, "one"'), ["one", "two"])
 
     def test_with_naughty_input(self):
         """
         Test with naughty input.
         """
         # Bad users! Naughty users!
         self.assertEqual(parse_tags(None), [])
@@ -1198,35 +1301,49 @@
         )
 
     def test_recreation_of_tag_list_string_representations(self):
         plain = Tag(name="plain")
         spaces = Tag(name="spa ces")
         comma = Tag(name="com,ma")
         self.assertEqual(edit_string_for_tags([plain]), "plain")
-        self.assertEqual(edit_string_for_tags([plain, spaces]), '"spa ces", plain')
         self.assertEqual(
-            edit_string_for_tags([plain, spaces, comma]), '"com,ma", "spa ces", plain'
+            edit_string_for_tags([plain, spaces]), '"spa ces", plain'
+        )
+        self.assertEqual(
+            edit_string_for_tags([plain, spaces, comma]),
+            '"com,ma", "spa ces", plain',
+        )
+        self.assertEqual(
+            edit_string_for_tags([plain, comma]), '"com,ma", plain'
+        )
+        self.assertEqual(
+            edit_string_for_tags([comma, spaces]), '"com,ma", "spa ces"'
         )
-        self.assertEqual(edit_string_for_tags([plain, comma]), '"com,ma", plain')
-        self.assertEqual(edit_string_for_tags([comma, spaces]), '"com,ma", "spa ces"')
 
-    @override_settings(TAGGIT_TAGS_FROM_STRING="tests.custom_parser.comma_splitter")
+    @override_settings(
+        TAGGIT_TAGS_FROM_STRING="tests.custom_parser.comma_splitter"
+    )
     def test_custom_comma_splitter(self):
         self.assertEqual(parse_tags("   Cued Speech "), ["Cued Speech"])
         self.assertEqual(parse_tags(" ,Cued Speech, "), ["Cued Speech"])
         self.assertEqual(parse_tags("Cued Speech"), ["Cued Speech"])
         self.assertEqual(
-            parse_tags("Cued Speech, dictionary"), ["Cued Speech", "dictionary"]
+            parse_tags("Cued Speech, dictionary"),
+            ["Cued Speech", "dictionary"],
         )
 
-    @override_settings(TAGGIT_STRING_FROM_TAGS="tests.custom_parser.comma_joiner")
+    @override_settings(
+        TAGGIT_STRING_FROM_TAGS="tests.custom_parser.comma_joiner"
+    )
     def test_custom_comma_joiner(self):
         a = Tag(name="Cued Speech")
         b = Tag(name="transliterator")
-        self.assertEqual(edit_string_for_tags([a, b]), "Cued Speech, transliterator")
+        self.assertEqual(
+            edit_string_for_tags([a, b]), "Cued Speech, transliterator"
+        )
 
 
 class DeconstructTestCase(SimpleTestCase):
     def test_deconstruct_kwargs_kept(self):
         instance = TaggableManager(through=OfficialThroughModel, to="dummy.To")
         name, path, args, kwargs = instance.deconstruct()
         new_instance = TaggableManager(*args, **kwargs)
@@ -1269,15 +1386,16 @@
         request = self.factory.get(f"/food/tags/{self.slug}/")
         queryset = self.model.objects.all()
         response = tagged_object_list(request, self.slug, queryset)
         self.assertEqual(response.status_code, 200)
         self.assertIn(self.apple, response.context_data["object_list"])
         self.assertNotIn(self.strawberry, response.context_data["object_list"])
         self.assertEqual(
-            self.apple.tags.first(), response.context_data["extra_context"]["tag"]
+            self.apple.tags.first(),
+            response.context_data["extra_context"]["tag"],
         )
 
     def test_list_view_returns_single(self):
         response = self.client.get(f"/food/tags/{self.slug}/")
         self.assertEqual(response.status_code, 200)
         self.assertIn(self.apple, response.context_data["object_list"])
         self.assertNotIn(self.strawberry, response.context_data["object_list"])
```

### Comparing `django-tag-fields-4.0.0/tox.ini` & `django-tag-fields-4.0.1/tox.ini`

 * *Files identical despite different names*

