# Comparing `tmp/for-django-projects-1.0.2.tar.gz` & `tmp/for-django-projects-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "for-django-projects-1.0.2.tar", last modified: Thu May  4 17:17:40 2023, max compression
+gzip compressed data, was "for-django-projects-1.0.3.tar", last modified: Thu May  4 17:23:47 2023, max compression
```

## Comparing `for-django-projects-1.0.2.tar` & `for-django-projects-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.598404 for-django-projects-1.0.2/
--rw-rw-rw-   0        0        0     1010 2023-05-04 17:17:40.598404 for-django-projects-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-05-04 17:16:18.000000 for-django-projects-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.566758 for-django-projects-1.0.2/for_django_projects/
--rw-rw-rw-   0        0        0        0 2023-05-04 17:11:49.000000 for-django-projects-1.0.2/for_django_projects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.582387 for-django-projects-1.0.2/for_django_projects/alertas/
--rw-rw-rw-   0        0        0     1152 2022-11-22 19:35:13.000000 for-django-projects-1.0.2/for_django_projects/alertas/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.596398 for-django-projects-1.0.2/for_django_projects/form_utils/
--rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/__init__.py
--rw-rw-rw-   0        0        0      511 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/admin.py
--rw-rw-rw-   0        0        0     2457 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/fields.py
--rw-rw-rw-   0        0        0    10772 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/forms.py
--rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/models.py
--rw-rw-rw-   0        0        0      375 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.596398 for-django-projects-1.0.2/for_django_projects/form_utils/templatetags/
--rw-rw-rw-   0        0        0      118 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/templatetags/__init__.py
--rw-rw-rw-   0        0        0     3499 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/templatetags/form_utils.py
--rw-rw-rw-   0        0        0      555 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/utils.py
--rw-rw-rw-   0        0        0     4405 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.598404 for-django-projects-1.0.2/for_django_projects/pwa/
--rw-rw-rw-   0        0        0       41 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/pwa/__init__.py
--rw-rw-rw-   0        0        0     4617 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/pwa/app_settings.py
--rw-rw-rw-   0        0        0       86 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/pwa/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.598404 for-django-projects-1.0.2/for_django_projects/pwa/templatetags/
--rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/pwa/templatetags/__init__.py
--rw-rw-rw-   0        0        0      732 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/pwa/templatetags/pwa.py
--rw-rw-rw-   0        0        0      358 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/pwa/urls.py
--rw-rw-rw-   0        0        0      616 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/pwa/views.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.598404 for-django-projects-1.0.2/for_django_projects/utils/
--rw-rw-rw-   0        0        0        0 2023-05-03 20:33:09.000000 for-django-projects-1.0.2/for_django_projects/utils/__init__.py
--rw-rw-rw-   0        0        0    24053 2023-05-04 14:09:27.000000 for-django-projects-1.0.2/for_django_projects/utils/custom_models.py
--rw-rw-rw-   0        0        0     3267 2023-05-04 14:09:27.000000 for-django-projects-1.0.2/for_django_projects/utils/decoradores.py
--rw-rw-rw-   0        0        0    18609 2023-05-04 14:15:47.000000 for-django-projects-1.0.2/for_django_projects/utils/funciones.py
--rw-rw-rw-   0        0        0     4732 2023-05-04 14:32:38.000000 for-django-projects-1.0.2/for_django_projects/utils/funciones_adicionales.py
--rw-rw-rw-   0        0        0     3117 2023-03-30 15:00:29.000000 for-django-projects-1.0.2/for_django_projects/utils/models_utils.py
--rw-rw-rw-   0        0        0     4058 2023-05-02 21:53:32.000000 for-django-projects-1.0.2/for_django_projects/utils/validadores.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.582387 for-django-projects-1.0.2/for_django_projects.egg-info/
--rw-rw-rw-   0        0        0     1010 2023-05-04 17:17:40.000000 for-django-projects-1.0.2/for_django_projects.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1309 2023-05-04 17:17:40.000000 for-django-projects-1.0.2/for_django_projects.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 17:17:40.000000 for-django-projects-1.0.2/for_django_projects.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-05-04 17:17:40.000000 for-django-projects-1.0.2/for_django_projects.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-04 17:17:40.000000 for-django-projects-1.0.2/for_django_projects.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 17:17:40.598404 for-django-projects-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      919 2023-05-04 17:17:37.000000 for-django-projects-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.169842 for-django-projects-1.0.3/
+-rw-rw-rw-   0        0        0     1010 2023-05-04 17:23:47.169842 for-django-projects-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-05-04 17:16:18.000000 for-django-projects-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.127312 for-django-projects-1.0.3/for_django_projects/
+-rw-rw-rw-   0        0        0        0 2023-05-04 17:11:49.000000 for-django-projects-1.0.3/for_django_projects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.150369 for-django-projects-1.0.3/for_django_projects/alertas/
+-rw-rw-rw-   0        0        0     1152 2022-11-22 19:35:13.000000 for-django-projects-1.0.3/for_django_projects/alertas/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.157685 for-django-projects-1.0.3/for_django_projects/form_utils/
+-rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/__init__.py
+-rw-rw-rw-   0        0        0      511 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/admin.py
+-rw-rw-rw-   0        0        0     2457 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/fields.py
+-rw-rw-rw-   0        0        0    10772 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/forms.py
+-rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/models.py
+-rw-rw-rw-   0        0        0      375 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.159646 for-django-projects-1.0.3/for_django_projects/form_utils/templatetags/
+-rw-rw-rw-   0        0        0      118 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     3499 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/templatetags/form_utils.py
+-rw-rw-rw-   0        0        0      555 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/utils.py
+-rw-rw-rw-   0        0        0     4405 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.162648 for-django-projects-1.0.3/for_django_projects/pwa/
+-rw-rw-rw-   0        0        0       41 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/pwa/__init__.py
+-rw-rw-rw-   0        0        0     4617 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/pwa/app_settings.py
+-rw-rw-rw-   0        0        0       86 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/pwa/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.163653 for-django-projects-1.0.3/for_django_projects/pwa/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/pwa/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      732 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/pwa/templatetags/pwa.py
+-rw-rw-rw-   0        0        0      358 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/pwa/urls.py
+-rw-rw-rw-   0        0        0      616 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/pwa/views.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.168841 for-django-projects-1.0.3/for_django_projects/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-03 20:33:09.000000 for-django-projects-1.0.3/for_django_projects/utils/__init__.py
+-rw-rw-rw-   0        0        0    24113 2023-05-04 17:23:25.000000 for-django-projects-1.0.3/for_django_projects/utils/custom_models.py
+-rw-rw-rw-   0        0        0     3012 2023-05-04 17:23:25.000000 for-django-projects-1.0.3/for_django_projects/utils/decoradores.py
+-rw-rw-rw-   0        0        0    18629 2023-05-04 17:23:25.000000 for-django-projects-1.0.3/for_django_projects/utils/funciones.py
+-rw-rw-rw-   0        0        0     4732 2023-05-04 14:32:38.000000 for-django-projects-1.0.3/for_django_projects/utils/funciones_adicionales.py
+-rw-rw-rw-   0        0        0     3137 2023-05-04 17:23:25.000000 for-django-projects-1.0.3/for_django_projects/utils/models_utils.py
+-rw-rw-rw-   0        0        0     4058 2023-05-02 21:53:32.000000 for-django-projects-1.0.3/for_django_projects/utils/validadores.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.149357 for-django-projects-1.0.3/for_django_projects.egg-info/
+-rw-rw-rw-   0        0        0     1010 2023-05-04 17:23:47.000000 for-django-projects-1.0.3/for_django_projects.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1309 2023-05-04 17:23:47.000000 for-django-projects-1.0.3/for_django_projects.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 17:23:47.000000 for-django-projects-1.0.3/for_django_projects.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-05-04 17:23:47.000000 for-django-projects-1.0.3/for_django_projects.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-04 17:23:47.000000 for-django-projects-1.0.3/for_django_projects.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 17:23:47.169842 for-django-projects-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      919 2023-05-04 17:23:25.000000 for-django-projects-1.0.3/setup.py
```

### Comparing `for-django-projects-1.0.2/PKG-INFO` & `for-django-projects-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: for-django-projects
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package of libraries for Django projects
 Home-page: https://github.com/jasmanysanchez/for-django-projects
 Author: Jasmany Sanchez Mendez
 Author-email: jasmanysanchez97@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `for-django-projects-1.0.2/README.md` & `for-django-projects-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.2/for_django_projects/alertas/__init__.py` & `for-django-projects-1.0.3/for_django_projects/alertas/__init__.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.2/for_django_projects/form_utils/fields.py` & `for-django-projects-1.0.3/for_django_projects/form_utils/fields.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.2/for_django_projects/form_utils/forms.py` & `for-django-projects-1.0.3/for_django_projects/form_utils/forms.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.2/for_django_projects/form_utils/templatetags/form_utils.py` & `for-django-projects-1.0.3/for_django_projects/form_utils/templatetags/form_utils.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.2/for_django_projects/form_utils/utils.py` & `for-django-projects-1.0.3/for_django_projects/form_utils/utils.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.2/for_django_projects/form_utils/widgets.py` & `for-django-projects-1.0.3/for_django_projects/form_utils/widgets.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.2/for_django_projects/pwa/app_settings.py` & `for-django-projects-1.0.3/for_django_projects/pwa/app_settings.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.2/for_django_projects/pwa/templatetags/pwa.py` & `for-django-projects-1.0.3/for_django_projects/pwa/templatetags/pwa.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.2/for_django_projects/pwa/views.py` & `for-django-projects-1.0.3/for_django_projects/pwa/views.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.2/for_django_projects/utils/custom_models.py` & `for-django-projects-1.0.3/for_django_projects/utils/custom_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from django.forms.widgets import DateTimeBaseInput
 from django.template.loader import render_to_string
 from django.utils.html import strip_tags
 from django.utils.safestring import mark_safe
 from django_select2.forms import ModelSelect2Widget, Select2Widget, Select2MultipleWidget, ModelSelect2MultipleWidget
 
 from django.conf import settings
-from form_utils.forms import BetterModelForm, BetterForm
-from utils.funciones_adicionales import customgetattr
+from for_django_projects.form_utils.forms import BetterModelForm, BetterForm
+from for_django_projects.utils.funciones_adicionales import customgetattr
 
 
 class CustomValueDb(Value):
     def __init__(self, value, output_field=None):
         from django.db.models import IntegerField, CharField, FloatField, DecimalField, BooleanField, DateField, DateTimeField
         type_value = type(value).__name__.lower()
         if not output_field:
@@ -167,15 +167,15 @@
     def fecha_hora_registro(self):
         return self.fecha_registro
 
     class Meta:
         abstract = True
 
 def filter_queryset(self, request, term, queryset=None, **dependent_fields):
-    from django.db.models import Q;import django;from utils.funciones import criterioBusquedaDinamico
+    from django.db.models import Q;import django;from for_django_projects.utils.funciones import criterioBusquedaDinamico
     if django.VERSION < (4, 0):
         from django.contrib.admin.utils import (
             lookup_needs_distinct as lookup_spawns_duplicates,
         )
     else:
         from django.contrib.admin.utils import lookup_spawns_duplicates
     if queryset is None:
```

### Comparing `for-django-projects-1.0.2/for_django_projects/utils/decoradores.py` & `for-django-projects-1.0.3/for_django_projects/utils/decoradores.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import re
 from django.contrib import messages
 from django.db import transaction, IntegrityError
 from django.http import JsonResponse
 from django.shortcuts import redirect
 from django.conf import settings
-from utils.funciones import redirectAfterPostGet
+from for_django_projects.utils.funciones import redirectAfterPostGet
 
 
 def custom_atomic_request(func):
-    from utils.custom_models import FormError
-    from utils.funciones_adicionales import salva_logs_request
+    from for_django_projects.utils.custom_models import FormError
     import sys
     def validate_request(*args, **kwargs):
         res_json = []
         request = args[0]
         has_except = False
         error_message = ""
         if request.method == "POST":
@@ -44,17 +43,14 @@
                     {
                         'error': has_except,
                         "message": error_message
                     }
                 )
                 val_func = JsonResponse(res_json, safe=False)
             except Exception as ex:
-                salva_logs_request(request, __file__, request.method,
-                                   action, type(ex).__name__,
-                                   'Error on line {}'.format(sys.exc_info()[-1].tb_lineno), ex)
                 res_json.append({'error': True,
                                  "message": "Intente Nuevamente"
                                  })
                 val_func = JsonResponse(res_json, safe=False)
                 has_except = True
                 error_message = "Intente Nuevamente"
         elif request.method == "GET":
```

### Comparing `for-django-projects-1.0.2/for_django_projects/utils/funciones.py` & `for-django-projects-1.0.3/for_django_projects/utils/funciones.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     for f in filtros:
         if c.endswith(f):
             return False
     return True
 def criterioBusquedaDinamico(criterio: str, campos: list, isPostgres=True):
     '''Si el modelo no proviene de una base de datos postgres set isPostgres=False'''
     from django.db.models import Q
-    from utils.funciones_adicionales import remover_espacios_de_mas
+    from for_django_projects.utils.funciones_adicionales import remover_espacios_de_mas
     filtros = Q()
     criterio_list = remover_espacios_de_mas(criterio).split("+")
     # for c in campos:
     #     filtros = filtros | formarCondicion(c, criterio)
     if len(criterio_list) <= 1:
         cri = criterio.strip()
         for c in campos:
```

### Comparing `for-django-projects-1.0.2/for_django_projects/utils/funciones_adicionales.py` & `for-django-projects-1.0.3/for_django_projects/utils/funciones_adicionales.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.2/for_django_projects/utils/models_utils.py` & `for-django-projects-1.0.3/for_django_projects/utils/models_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     def get_filename(self, instance, filename):
         from django.utils.text import slugify
         filename = default_storage.get_valid_name(os.path.basename(filename))
         filename = force_str(filename)
         filename = unicodedata.normalize('NFKD', filename).encode('ascii', 'ignore').decode('ascii')
         extension = os.path.splitext(filename)[1][1:]
-        from utils.funciones_adicionales import customgetattr
+        from for_django_projects.utils.funciones_adicionales import customgetattr
         concatenar = ""
         for x in self.campos_concatenar:
             concatenar += str(customgetattr(instance, x) or "") + " "
         return os.path.normpath("%s-%s.%s" % (slugify(self.nombreArchivo + concatenar).upper(), datetime.datetime.now().strftime('%d-%m-%Y-%H-%M-%S-%f'), extension.lower()))
 
     def generate_filename(self, instance, filename):
         return os.path.join(self.upload_to, self.get_filename(instance, filename))
```

### Comparing `for-django-projects-1.0.2/for_django_projects/utils/validadores.py` & `for-django-projects-1.0.3/for_django_projects/utils/validadores.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.2/for_django_projects.egg-info/PKG-INFO` & `for-django-projects-1.0.3/for_django_projects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: for-django-projects
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package of libraries for Django projects
 Home-page: https://github.com/jasmanysanchez/for-django-projects
 Author: Jasmany Sanchez Mendez
 Author-email: jasmanysanchez97@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `for-django-projects-1.0.2/for_django_projects.egg-info/SOURCES.txt` & `for-django-projects-1.0.3/for_django_projects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.2/setup.py` & `for-django-projects-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="for-django-projects",
-    version="1.0.2",
+    version="1.0.3",
     author="Jasmany Sanchez Mendez",
     author_email="jasmanysanchez97@gmail.com",
     description="Package of libraries for Django projects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jasmanysanchez/for-django-projects",
     packages=setuptools.find_packages(),
```

