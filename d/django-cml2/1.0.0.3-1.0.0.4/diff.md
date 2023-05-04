# Comparing `tmp/django-cml2-1.0.0.3.tar.gz` & `tmp/django-cml2-1.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cml2-1.0.0.3.tar", last modified: Sun Apr 30 12:39:20 2023, max compression
+gzip compressed data, was "django-cml2-1.0.0.4.tar", last modified: Thu May  4 13:44:22 2023, max compression
```

## Comparing `django-cml2-1.0.0.3.tar` & `django-cml2-1.0.0.4.tar`

### file list

```diff
@@ -1,36 +1,47 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-30 12:39:20.984120 django-cml2-1.0.0.3/
--rw-r--r--   0 admin      (501) staff       (20)     1515 2023-04-27 07:07:40.000000 django-cml2-1.0.0.3/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)      163 2023-04-28 21:29:48.000000 django-cml2-1.0.0.3/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     2052 2023-04-30 12:39:20.984444 django-cml2-1.0.0.3/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     1131 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/README.rst
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-30 12:39:20.977054 django-cml2-1.0.0.3/cml/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2440 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/admin.py
--rw-r--r--   0 admin      (501) staff       (20)     4159 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/auth.py
--rw-r--r--   0 admin      (501) staff       (20)      266 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/conf.py
--rw-r--r--   0 admin      (501) staff       (20)    30983 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/items.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-30 12:39:20.977366 django-cml2-1.0.0.3/cml/management/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/management/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-30 12:39:20.978179 django-cml2-1.0.0.3/cml/management/commands/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/management/commands/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      943 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/management/commands/cml_init.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-30 12:39:20.979673 django-cml2-1.0.0.3/cml/migrations/
--rw-r--r--   0 admin      (501) staff       (20)      905 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/migrations/0001_initial.py
--rw-r--r--   0 admin      (501) staff       (20)     5205 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/migrations/0002_reorganize_fields.py
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/migrations/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1559 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/models.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-30 12:39:20.968936 django-cml2-1.0.0.3/cml/templates/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-30 12:39:20.980042 django-cml2-1.0.0.3/cml/templates/cml/
--rw-r--r--   0 admin      (501) staff       (20)     1890 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/templates/cml/cml_delegate.py
--rw-r--r--   0 admin      (501) staff       (20)      248 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/urls.py
--rw-r--r--   0 admin      (501) staff       (20)     2515 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/utils.py
--rw-r--r--   0 admin      (501) staff       (20)    12883 2023-04-30 11:15:59.000000 django-cml2-1.0.0.3/cml/views.py
--rw-r--r--   0 admin      (501) staff       (20)     7583 2023-04-30 11:12:48.000000 django-cml2-1.0.0.3/cml/xml.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-30 12:39:20.983512 django-cml2-1.0.0.3/django_cml2.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     2052 2023-04-30 12:39:20.000000 django-cml2-1.0.0.3/django_cml2.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      584 2023-04-30 12:39:20.000000 django-cml2-1.0.0.3/django_cml2.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-30 12:39:20.000000 django-cml2-1.0.0.3/django_cml2.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       34 2023-04-30 12:39:20.000000 django-cml2-1.0.0.3/django_cml2.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        4 2023-04-30 12:39:20.000000 django-cml2-1.0.0.3/django_cml2.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       53 2023-04-30 12:39:20.985340 django-cml2-1.0.0.3/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1297 2023-04-30 12:38:12.000000 django-cml2-1.0.0.3/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-04 13:44:22.706733 django-cml2-1.0.0.4/
+-rw-r--r--   0 admin      (501) staff       (20)     1515 2023-04-27 07:07:40.000000 django-cml2-1.0.0.4/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)      163 2023-04-28 21:29:48.000000 django-cml2-1.0.0.4/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)     2873 2023-05-04 13:44:22.706911 django-cml2-1.0.0.4/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1972 2023-05-02 17:00:04.000000 django-cml2-1.0.0.4/README.rst
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-04 13:44:22.693061 django-cml2-1.0.0.4/cml/
+-rw-r--r--   0 admin      (501) staff       (20)       51 2023-05-02 17:03:05.000000 django-cml2-1.0.0.4/cml/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2493 2023-05-04 11:58:01.000000 django-cml2-1.0.0.4/cml/admin.py
+-rw-r--r--   0 admin      (501) staff       (20)     4159 2023-04-30 11:12:48.000000 django-cml2-1.0.0.4/cml/auth.py
+-rw-r--r--   0 admin      (501) staff       (20)      266 2023-04-30 11:12:48.000000 django-cml2-1.0.0.4/cml/conf.py
+-rw-r--r--   0 admin      (501) staff       (20)    31033 2023-05-04 10:33:44.000000 django-cml2-1.0.0.4/cml/items.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-04 13:44:22.693773 django-cml2-1.0.0.4/cml/management/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-30 11:12:48.000000 django-cml2-1.0.0.4/cml/management/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-04 13:44:22.694040 django-cml2-1.0.0.4/cml/management/__pycache__/
+-rw-r--r--   0 admin      (501) staff       (20)      181 2023-05-04 12:17:00.000000 django-cml2-1.0.0.4/cml/management/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-04 13:44:22.695032 django-cml2-1.0.0.4/cml/management/commands/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-30 11:12:48.000000 django-cml2-1.0.0.4/cml/management/commands/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      943 2023-04-30 11:12:48.000000 django-cml2-1.0.0.4/cml/management/commands/cml_init.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-04 13:44:22.698703 django-cml2-1.0.0.4/cml/migrations/
+-rw-r--r--   0 admin      (501) staff       (20)      905 2023-04-30 11:12:48.000000 django-cml2-1.0.0.4/cml/migrations/0001_initial.py
+-rw-r--r--   0 admin      (501) staff       (20)     5205 2023-04-30 11:12:48.000000 django-cml2-1.0.0.4/cml/migrations/0002_reorganize_fields.py
+-rw-r--r--   0 admin      (501) staff       (20)      590 2023-05-04 12:28:40.000000 django-cml2-1.0.0.4/cml/migrations/0003_add_operation.py
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-30 11:12:48.000000 django-cml2-1.0.0.4/cml/migrations/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-04 13:44:22.701815 django-cml2-1.0.0.4/cml/migrations/__pycache__/
+-rw-r--r--   0 admin      (501) staff       (20)     1560 2023-05-02 17:33:41.000000 django-cml2-1.0.0.4/cml/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     5889 2023-05-02 17:33:41.000000 django-cml2-1.0.0.4/cml/migrations/__pycache__/0002_reorganize_fields.cpython-311.pyc
+-rw-r--r--   0 admin      (501) staff       (20)      994 2023-05-04 12:31:42.000000 django-cml2-1.0.0.4/cml/migrations/__pycache__/0003_add_operation.cpython-311.pyc
+-rw-r--r--   0 admin      (501) staff       (20)      181 2023-05-02 17:33:41.000000 django-cml2-1.0.0.4/cml/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     1641 2023-05-04 12:28:28.000000 django-cml2-1.0.0.4/cml/models.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-04 13:44:22.685104 django-cml2-1.0.0.4/cml/templates/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-04 13:44:22.702549 django-cml2-1.0.0.4/cml/templates/cml/
+-rw-r--r--   0 admin      (501) staff       (20)     1890 2023-04-30 11:12:48.000000 django-cml2-1.0.0.4/cml/templates/cml/cml_delegate.py
+-rw-r--r--   0 admin      (501) staff       (20)      248 2023-04-30 11:12:48.000000 django-cml2-1.0.0.4/cml/urls.py
+-rw-r--r--   0 admin      (501) staff       (20)     2482 2023-05-02 17:05:22.000000 django-cml2-1.0.0.4/cml/utils.py
+-rw-r--r--   0 admin      (501) staff       (20)    13156 2023-05-04 13:30:18.000000 django-cml2-1.0.0.4/cml/views.py
+-rw-r--r--   0 admin      (501) staff       (20)     7529 2023-05-02 17:06:33.000000 django-cml2-1.0.0.4/cml/xml.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-04 13:44:22.705265 django-cml2-1.0.0.4/django_cml2.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     2873 2023-05-04 13:44:22.000000 django-cml2-1.0.0.4/django_cml2.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      944 2023-05-04 13:44:22.000000 django-cml2-1.0.0.4/django_cml2.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-05-04 13:44:22.000000 django-cml2-1.0.0.4/django_cml2.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       34 2023-05-04 13:44:22.000000 django-cml2-1.0.0.4/django_cml2.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        4 2023-05-04 13:44:22.000000 django-cml2-1.0.0.4/django_cml2.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       53 2023-05-04 13:44:22.707581 django-cml2-1.0.0.4/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1297 2023-05-04 13:40:57.000000 django-cml2-1.0.0.4/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-04 13:44:22.706191 django-cml2-1.0.0.4/tests/
+-rw-r--r--   0 admin      (501) staff       (20)     1557 2023-04-27 07:07:40.000000 django-cml2-1.0.0.4/tests/test_utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     2225 2023-04-25 22:44:47.000000 django-cml2-1.0.0.4/tests/tests.py
```

### Comparing `django-cml2-1.0.0.3/LICENSE` & `django-cml2-1.0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cml2-1.0.0.3/PKG-INFO` & `django-cml2-1.0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-cml2
-Version: 1.0.0.3
+Version: 1.0.0.4
 Summary: Application for data exchange in CommerceML 2 standard. This is a new version with new architecture
 Home-page: https://github.com/sergey-gru/django-cml2
 Author: Sergey Grunenko
 Author-email: grunenko.serg@gmail.com
 License: BSD License
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -24,15 +23,15 @@
 
 ===
 CML
 ===
 
 CML is a reusable Django app for data exchange in CommerceML 2 standard.
 
-This packet is avaliable here: https://pypi.org/project/django-cml2
+This packet is available here: https://pypi.org/project/django-cml2
 
 
 Requirements
 ------------
 
 - Python 3.3, 3.4, 3.5, 3.6
 - Django 3.2
@@ -40,17 +39,21 @@
 Quick start
 -----------
 
 1. Install using pip::
 
     pip install django-cml2
 
-   or clone the repo and add to your `PYTHONPATH`::
+   or clone the repo and add to your virtual environment `venv`::
+
+    # cd <your_project>
+    # source venv/bin/activate
 
     git clone https://github.com/sergey-gru/django-cml2.git
+    pip install --editable django-cml2
 
 
 2. Add 'cml' to your `settings.py` like this::
 
     INSTALLED_APPS = [
         ...
         'cml',
@@ -76,12 +79,39 @@
 
     CML_USER_DELEGATE = 'cml_delegate'
     # CML_USER_DELEGATE = 'app.cml_delegate'
 
 7. Modify methods to stack new cml packet with your django models.
 
 
-Release notes
-----------------
-- 1.0.0 This version was created based on https://github.com/ArtemiusUA/django-cml
+8. Add logger settings to your `settings.py`::
 
+    LOGGING = {
+        'version': 1,
+        ...
 
+        'handlers': {
+            'console': {...},
+            'log_debug': {...},
+            'log_info': {...},
+        },
+
+        'loggers': {
+            ...
+
+            # Logging important change process
+            'cml.views': {
+                'handlers': ['console', 'log_debug', 'log_info'] if DEBUG else ['log_info'],
+                'level': 'DEBUG',
+                'propagate': False,
+            },
+            'cml.utils': {
+                'handlers': ['console', 'log_debug', 'log_info'] if DEBUG else ['log_info'],
+                'level': 'INFO',
+                'propagate': False,
+            },
+        }
+    }
+
+Release notes
+----------------
+- 1.0.0 This version was forked from https://github.com/ArtemiusUA/django-cml
```

### Comparing `django-cml2-1.0.0.3/cml/admin.py` & `django-cml2-1.0.0.4/cml/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import absolute_import
-import datetime
 from datetime import timedelta
 from django.contrib import admin
 from .models import *
 
 
 @admin.register(Exchange)
 class ExchangeAdmin(admin.ModelAdmin):
     list_display = (
         'dt_start_iso',
         'duration',
         'user',
         'uploaded',
         'imported',
         'exported',
+        'operation',
         'file_name_short',
         'state',
         'report_short',
     )
     list_display_links = ('dt_start_iso', 'report_short',)
     readonly_fields = (
         'user',
@@ -40,34 +40,38 @@
         return rec.dt_start.isoformat(timespec='seconds')
     dt_start_iso.short_description = 'date start'
 
     def dt_action_iso(self, rec):
         return rec.dt_action.isoformat(timespec='seconds')
     dt_action_iso.short_description = 'date action'
 
-    def duration(self, rec):
+    @staticmethod
+    def duration(rec):
         diff = rec.dt_action - rec.dt_start
         sec = round(diff.total_seconds())
         diff = timedelta(seconds=sec)
         return str(diff)
 
-    def uploaded(self, rec):
+    @staticmethod
+    def uploaded(rec):
         fmt = 'xml={}\nimg={}\nall={}'
         return fmt.format(rec.c_up_xml,
                           rec.c_up_img,
                           rec.c_up)
 
-    def imported(self, rec):
+    @staticmethod
+    def imported(rec):
         fmt = 'cl={}\ncat={}\noff={}\ndocs={}'
         return fmt.format(rec.c_imp_classifier,
                           rec.c_imp_catalogue,
                           rec.c_imp_offers_pack,
                           rec.c_imp_doc)
 
-    def exported(self, rec):
+    @staticmethod
+    def exported(rec):
         fmt = 'docs={}'
         return fmt.format(rec.c_exp_doc)
 
     @staticmethod
     def _get_str_cut(val: str, max_len: int, cut_left=True) -> str:
         if len(val) <= max_len:
             return val
```

### Comparing `django-cml2-1.0.0.3/cml/auth.py` & `django-cml2-1.0.0.4/cml/auth.py`

 * *Files identical despite different names*

### Comparing `django-cml2-1.0.0.3/cml/items.py` & `django-cml2-1.0.0.4/cml/items.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 # -*- coding: utf-8 -
 from __future__ import absolute_import
-import logging
 import os
 from decimal import Decimal
 from datetime import datetime
 from enum import Enum, IntEnum
 from pathlib import Path
-from .xml import XmlElement
+from . import logger
 from .conf import settings
-
-
-logger = logging.getLogger(__name__)
+from .xml import XmlElement
 
 
 def time_from_string(s: str) -> datetime.time:
     return datetime.strptime(s, '%H:%M:%S').time()
 
 
 def time_to_string(time: datetime.time) -> str:
@@ -174,15 +171,14 @@
         return it
 
     def __repr__(self):
         return f'{self.name}: {self.groups}'
 
 
 class ValueType(Enum):
-    UNDEFINED = 0
     STRING = 'Строка'  # Boolean values represents as strings "Yes" "No"
     NUMBER = 'Число'   # float number
     DATETIME = 'Время'
     LIST = 'Справочник'
 
 
 class Property(ItemBase):
@@ -208,15 +204,16 @@
         it = cls(el)
         it.uid = el.find('Ид', converter=str)
         it.name = el.find('Наименование', converter=str)
         it.value_type = el.find('ТипЗначений', converter=ValueType)
         it.is_multi = el.find('Множественное', converter=as_bool, default=False)
         it.is_required = el.find('Обязательное', converter=as_bool, default=False)
         it.for_products = el.find('ДляТоваров', converter=as_bool)
-        it.variants = el.findall('ВариантыЗначений/Значение', converter=str)
+
+        it.variants = el.findall('ВариантыЗначений/*/Значение', converter=str)
         if it.value_type == ValueType.LIST:
             it.variants_list = el.findall('ВариантыЗначений/Справочник',
                                           converter_xml=PropertyVariant.parse_xml)
         return it
 
 
 class PropertyVariant(ItemBase):
@@ -343,15 +340,15 @@
 
 
 class Product(ItemBase):
     def __init__(self, *args, **kwargs):
         super(Product, self).__init__(*args, **kwargs)  # type: ignore
         self.status = ProductStatus.NEW
         self.uid = ''
-        self.vendor_uid = ''
+        self.vendor_code = ''
         self.code = ''
         self.name = ''
         self.unit = Unit()
         self.group_uids: [str] or None = None  # Note: if this is None, add product to the global group
         self.category_uid = ''
         self.desc = ''
         self.prop_values: [PropertyValue] = []
@@ -381,19 +378,21 @@
         it.uid = el.find('Ид', converter=str)
         it.vendor_code = el.find('Артикул', converter=str)
         it.code = el.find('Код', converter=str)
         it.name = el.find('Наименование', converter=str)
         it.unit = el.find('БазоваяЕдиница', converter_xml=Unit.parse_xml_ref)
         it.group_uids = el.findall('Группы/Ид', converter=str)
         it.category_uid = el.find('Категория', converter=str)
+        it.desc = el.find('Описание', converter=str, default='')
 
         pvals = el.findall('ЗначенияСвойств/ЗначенияСвойства', converter_xml=PropertyValue.parse_xml)
         it.prop_values = [pval for pval in pvals if not pval.is_empty()]
 
         it.requisites = cls._imp_requisites(el)
+        # files, images
         for fr in el.findall('Картинка', converter=FileRef):
             if fr.is_image_type():
                 it.images.append(fr)
             else:
                 it.files.append(fr)
         it.taxes = el.findall('СтавкиНалогов/СтавкаНалога', converter_xml=Tax.parse_xml)
```

### Comparing `django-cml2-1.0.0.3/cml/management/commands/cml_init.py` & `django-cml2-1.0.0.4/cml/management/commands/cml_init.py`

 * *Files identical despite different names*

### Comparing `django-cml2-1.0.0.3/cml/migrations/0001_initial.py` & `django-cml2-1.0.0.4/cml/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cml2-1.0.0.3/cml/migrations/0002_reorganize_fields.py` & `django-cml2-1.0.0.4/cml/migrations/0002_reorganize_fields.py`

 * *Files identical despite different names*

### Comparing `django-cml2-1.0.0.3/cml/models.py` & `django-cml2-1.0.0.4/cml/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,16 @@
                              null=True)
     state = models.CharField(max_length=15,
                              choices=ExchangeState.choices(),
                              default=str(ExchangeState.INIT))
     dt_start = models.DateTimeField(auto_now_add=True)
     dt_action = models.DateTimeField(auto_now=True, blank=True)
 
-    file_name = models.CharField(max_length=250, default='')
+    operation = models.CharField(max_length=30, default='', null=True)
+    file_name = models.CharField(max_length=250, default='', null=True)
 
     c_up = models.IntegerField(default=0)
     c_up_xml = models.IntegerField(default=0)
     c_up_img = models.IntegerField(default=0)
 
     c_imp_classifier = models.IntegerField(default=0)
     c_imp_catalogue = models.IntegerField(default=0)
```

### Comparing `django-cml2-1.0.0.3/cml/templates/cml/cml_delegate.py` & `django-cml2-1.0.0.4/cml/templates/cml/cml_delegate.py`

 * *Files identical despite different names*

### Comparing `django-cml2-1.0.0.3/cml/utils.py` & `django-cml2-1.0.0.4/cml/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 # -*- coding: utf-8 -
 from __future__ import absolute_import
-import logging
 import importlib
 import inspect
+from . import logger
 from . import items, xml
 from .conf import settings
 
 
-logger = logging.getLogger(__name__)
-
-
 class AbstractUserDelegate(object):
     def __init__(self):
         pass
 
     @classmethod
     def get_child_class(cls) -> type:
         try:
```

### Comparing `django-cml2-1.0.0.3/cml/views.py` & `django-cml2-1.0.0.4/cml/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from __future__ import absolute_import
-import logging
 import typing
 import os
 import shutil
 import datetime
 from django.core.files.uploadedfile import SimpleUploadedFile
 from django.conf import settings
 from django.db import transaction
 from django.http import (HttpRequest, HttpResponse)
 from django.utils import timezone
 from django.views.decorators.csrf import csrf_exempt
 from django.views.generic import View
+from . import logger
 from . import (auth, utils, items)
 from .models import Exchange, ExchangeState
 
 
-logger = logging.getLogger(__name__)
-
-
 # Test configuration of delegate. If delegate was not configured,
 utils.AbstractUserDelegate.get_child_class()
 
 RESPONSE_SUCCESS = 'success'
 RESPONSE_PROGRESS = 'progress'
 RESPONSE_ERROR = 'failure'
 
@@ -83,25 +80,29 @@
 
 class HttpRequestAuth(HttpRequest):
     user: any = None
     session: any = None
 
 
 class ProtocolSession(object):
-    def __init__(self, pv: 'ProtocolView', user=None, create=True):
+    def __init__(self, pv: 'ProtocolView', user=None, create=True, operation='init', filename=''):
+        self._pv = pv
         self.user = user
         self.create = create
-        self._pv = pv
+        self.operation = operation
+        self.filename = filename
         self._rec = None
 
     def close(self):
         self._rec.state = ExchangeState.DONE
 
-    def set_filename(self, filename):
+    def set_operation(self, operation, filename):
+        self._rec.operation = operation
         self._rec.file_name = filename
+        self._rec.save()
 
     def __enter__(self):
         """
         get or create `_rec`
         """
         with transaction.atomic():
             if self.create:
@@ -208,14 +209,15 @@
             ('sale', 'file'): self.api_file,
             ('sale', 'query'): self.api_query,
             ('sale', 'success'): self.api_success,
         }
 
         self.user_delegate = utils.AbstractUserDelegate.get_child_instance()
         self._check_cml_upload_root(items.FileRef.base_path)
+        self.operation = None
 
         self.c_up = 0
         self.c_up_xml = 0
         self.c_up_img = 0
 
         self.c_imp_classifier = 0
         self.c_imp_catalogue = 0
@@ -265,14 +267,16 @@
     # @auth.logged_in_or_basicauth()
     def dispatch(self, request: HttpRequestAuth, *args, **kwargs) -> HttpResponse:
         get_kwargs = request.GET.dict()
         logger.debug(f'user="{request.user}" {request.method} ({get_kwargs})')
 
         p_type = request.GET.get('type')
         p_mode = request.GET.get('mode')
+        self.operation = f'{p_type}_{p_mode}'
+
         api_method = self.routes_map.get((p_type, p_mode))
         if not api_method:
             msg = f'Unknown GET sequence: {get_kwargs}'
             logger.info(msg)
             return response_error(msg)
 
         try:
@@ -308,14 +312,16 @@
         if request.method != 'POST':
             msg = f'Bad request method: {request.method}'
             logger.info(msg)
             return response_error(msg)
 
         with self.session(request) as cur:
             filename = self._get_param_filename(request)
+            cur.set_operation(self.operation, filename)
+
             fref = items.FileRef(filename)
             folder_path = fref.full_path.parent
 
             temp_file = SimpleUploadedFile(filename, request.read())
             try:
                 if not os.path.exists(folder_path):
                     os.makedirs(folder_path)
@@ -323,15 +329,14 @@
                 f = open(fref.full_path, 'wb')
                 for chunk in temp_file.chunks():
                     f.write(chunk)
             except Exception as e:
                 logger.error(f'Cannot write to file. msg: {e}')
                 return response_error('Cannot write to buffer file')
 
-            cur.set_filename(filename)
             logger.info(f'File loaded: {fref.path}')
 
             self.c_up += 1
             if fref.path.suffix == '.xml':
                 self.c_up_xml += 1
             if fref.is_image_type():
                 self.c_up_img += 1
@@ -342,22 +347,22 @@
 
             return response_success()
 
     # Processing import received file
     def api_import(self, request: HttpRequestAuth):
         with self.session(request) as cur:
             filename = self._get_param_filename(request)
-            fref = items.FileRef(filename)
+            cur.set_operation(self.operation, filename)
 
+            fref = items.FileRef(filename)
             if not fref.full_path.exists():
                 msg = f'File not found: {fref.path}'
                 logger.info(msg)
                 return response_error(msg)
 
-            cur.set_filename(filename)
             pack = items.Packet.parse(fref.full_path)
             self.import_pack(pack)
 
             if settings.CML_DELETE_FILES_AFTER_IMPORT:
                 try:
                     shutil.rmtree(items.FileRef.base_path)
                 except OSError as e:
@@ -365,19 +370,20 @@
 
             logger.info(f'Import completed. filename: {filename}')
             cur.close()
             return response_success()
 
     def api_query(self, request: HttpRequestAuth):
         with self.session(request, is_init=True) as cur:
+            cur.set_operation(self.operation, 'query')
+
             pack = items.Packet()
             pack.docs = self.user_delegate.export_orders()
 
             data = pack.compose()
-            cur.set_filename('query')
             self.c_exp_doc += 1
 
             logger.info(f'sale_success(user={request.user}): OK')
             return HttpResponse(data, content_type='text/xml')
 
     def api_success(self, request: HttpRequestAuth):
         with self.session(request) as cur:
```

### Comparing `django-cml2-1.0.0.3/cml/xml.py` & `django-cml2-1.0.0.4/cml/xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # -*- coding: utf-8 -
-import logging
 import typing
 from io import BytesIO
 from lxml import etree
 
 
-logger = logging.getLogger(__name__)
-
-
 class XmlImportException(Exception):
     pass
 
 
 class XmlElement(object):
     """
     It's analogue of etree.Element().__class__.
```

### Comparing `django-cml2-1.0.0.3/django_cml2.egg-info/PKG-INFO` & `django-cml2-1.0.0.4/django_cml2.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-cml2
-Version: 1.0.0.3
+Version: 1.0.0.4
 Summary: Application for data exchange in CommerceML 2 standard. This is a new version with new architecture
 Home-page: https://github.com/sergey-gru/django-cml2
 Author: Sergey Grunenko
 Author-email: grunenko.serg@gmail.com
 License: BSD License
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -24,15 +23,15 @@
 
 ===
 CML
 ===
 
 CML is a reusable Django app for data exchange in CommerceML 2 standard.
 
-This packet is avaliable here: https://pypi.org/project/django-cml2
+This packet is available here: https://pypi.org/project/django-cml2
 
 
 Requirements
 ------------
 
 - Python 3.3, 3.4, 3.5, 3.6
 - Django 3.2
@@ -40,17 +39,21 @@
 Quick start
 -----------
 
 1. Install using pip::
 
     pip install django-cml2
 
-   or clone the repo and add to your `PYTHONPATH`::
+   or clone the repo and add to your virtual environment `venv`::
+
+    # cd <your_project>
+    # source venv/bin/activate
 
     git clone https://github.com/sergey-gru/django-cml2.git
+    pip install --editable django-cml2
 
 
 2. Add 'cml' to your `settings.py` like this::
 
     INSTALLED_APPS = [
         ...
         'cml',
@@ -76,12 +79,39 @@
 
     CML_USER_DELEGATE = 'cml_delegate'
     # CML_USER_DELEGATE = 'app.cml_delegate'
 
 7. Modify methods to stack new cml packet with your django models.
 
 
-Release notes
-----------------
-- 1.0.0 This version was created based on https://github.com/ArtemiusUA/django-cml
+8. Add logger settings to your `settings.py`::
 
+    LOGGING = {
+        'version': 1,
+        ...
 
+        'handlers': {
+            'console': {...},
+            'log_debug': {...},
+            'log_info': {...},
+        },
+
+        'loggers': {
+            ...
+
+            # Logging important change process
+            'cml.views': {
+                'handlers': ['console', 'log_debug', 'log_info'] if DEBUG else ['log_info'],
+                'level': 'DEBUG',
+                'propagate': False,
+            },
+            'cml.utils': {
+                'handlers': ['console', 'log_debug', 'log_info'] if DEBUG else ['log_info'],
+                'level': 'INFO',
+                'propagate': False,
+            },
+        }
+    }
+
+Release notes
+----------------
+- 1.0.0 This version was forked from https://github.com/ArtemiusUA/django-cml
```

### Comparing `django-cml2-1.0.0.3/django_cml2.egg-info/SOURCES.txt` & `django-cml2-1.0.0.4/django_cml2.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,18 +10,26 @@
 cml/items.py
 cml/models.py
 cml/urls.py
 cml/utils.py
 cml/views.py
 cml/xml.py
 cml/management/__init__.py
+cml/management/__pycache__/__init__.cpython-311.pyc
 cml/management/commands/__init__.py
 cml/management/commands/cml_init.py
 cml/migrations/0001_initial.py
 cml/migrations/0002_reorganize_fields.py
+cml/migrations/0003_add_operation.py
 cml/migrations/__init__.py
+cml/migrations/__pycache__/0001_initial.cpython-311.pyc
+cml/migrations/__pycache__/0002_reorganize_fields.cpython-311.pyc
+cml/migrations/__pycache__/0003_add_operation.cpython-311.pyc
+cml/migrations/__pycache__/__init__.cpython-311.pyc
 cml/templates/cml/cml_delegate.py
 django_cml2.egg-info/PKG-INFO
 django_cml2.egg-info/SOURCES.txt
 django_cml2.egg-info/dependency_links.txt
 django_cml2.egg-info/requires.txt
-django_cml2.egg-info/top_level.txt
+django_cml2.egg-info/top_level.txt
+tests/test_utils.py
+tests/tests.py
```

### Comparing `django-cml2-1.0.0.3/setup.py` & `django-cml2-1.0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-cml2',
-    version='1.0.0.3',
+    version='1.0.0.4',
     description='Application for data exchange in CommerceML 2 standard. This is a new version with new architecture',
     long_description=README,
     author='Sergey Grunenko',
     author_email='grunenko.serg@gmail.com',
 
     url='https://github.com/sergey-gru/django-cml2',
     license='BSD License',
```

