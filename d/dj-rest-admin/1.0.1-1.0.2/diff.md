# Comparing `tmp/dj-rest-admin-1.0.1.tar.gz` & `tmp/dj-rest-admin-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-rest-admin-1.0.1.tar", last modified: Wed Apr 26 22:17:02 2023, max compression
+gzip compressed data, was "dj-rest-admin-1.0.2.tar", last modified: Thu May  4 20:53:33 2023, max compression
```

## Comparing `dj-rest-admin-1.0.1.tar` & `dj-rest-admin-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2023-04-26 22:17:02.993834 dj-rest-admin-1.0.1/
--rw-r--r--   0 dario     (1000) dario     (1000)     1069 2023-04-26 22:07:35.000000 dj-rest-admin-1.0.1/LICENSE
--rw-r--r--   0 dario     (1000) dario     (1000)     6027 2023-04-26 22:17:02.993834 dj-rest-admin-1.0.1/PKG-INFO
--rw-r--r--   0 dario     (1000) dario     (1000)     4099 2023-04-26 21:53:39.000000 dj-rest-admin-1.0.1/README.md
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2023-04-26 22:17:02.993834 dj-rest-admin-1.0.1/dj_rest_admin/
--rw-r--r--   0 dario     (1000) dario     (1000)      370 2023-04-26 21:49:32.000000 dj-rest-admin-1.0.1/dj_rest_admin/__init__.py
--rw-r--r--   0 dario     (1000) dario     (1000)      248 2023-04-26 21:49:32.000000 dj-rest-admin-1.0.1/dj_rest_admin/apps.py
--rw-r--r--   0 dario     (1000) dario     (1000)     1094 2023-04-26 21:49:32.000000 dj-rest-admin-1.0.1/dj_rest_admin/decorators.py
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2023-04-26 22:17:02.993834 dj-rest-admin-1.0.1/dj_rest_admin/migrations/
--rw-r--r--   0 dario     (1000) dario     (1000)        0 2023-04-26 21:49:32.000000 dj-rest-admin-1.0.1/dj_rest_admin/migrations/__init__.py
--rw-r--r--   0 dario     (1000) dario     (1000)      449 2023-04-26 21:49:32.000000 dj-rest-admin-1.0.1/dj_rest_admin/restmodeladmin.py
--rw-r--r--   0 dario     (1000) dario     (1000)     5434 2023-04-26 21:49:32.000000 dj-rest-admin-1.0.1/dj_rest_admin/sites.py
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2023-04-26 22:17:02.993834 dj-rest-admin-1.0.1/dj_rest_admin.egg-info/
--rw-r--r--   0 dario     (1000) dario     (1000)     6027 2023-04-26 22:17:02.000000 dj-rest-admin-1.0.1/dj_rest_admin.egg-info/PKG-INFO
--rw-r--r--   0 dario     (1000) dario     (1000)      399 2023-04-26 22:17:02.000000 dj-rest-admin-1.0.1/dj_rest_admin.egg-info/SOURCES.txt
--rw-r--r--   0 dario     (1000) dario     (1000)        1 2023-04-26 22:17:02.000000 dj-rest-admin-1.0.1/dj_rest_admin.egg-info/dependency_links.txt
--rw-r--r--   0 dario     (1000) dario     (1000)       91 2023-04-26 22:17:02.000000 dj-rest-admin-1.0.1/dj_rest_admin.egg-info/requires.txt
--rw-r--r--   0 dario     (1000) dario     (1000)       14 2023-04-26 22:17:02.000000 dj-rest-admin-1.0.1/dj_rest_admin.egg-info/top_level.txt
--rw-r--r--   0 dario     (1000) dario     (1000)     1114 2023-04-26 22:15:09.000000 dj-rest-admin-1.0.1/pyproject.toml
--rw-r--r--   0 dario     (1000) dario     (1000)       38 2023-04-26 22:17:02.993834 dj-rest-admin-1.0.1/setup.cfg
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2023-04-26 22:17:02.993834 dj-rest-admin-1.0.1/tests/
--rw-r--r--   0 dario     (1000) dario     (1000)    10205 2023-04-26 21:49:32.000000 dj-rest-admin-1.0.1/tests/tests.py
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2023-05-04 20:53:33.370230 dj-rest-admin-1.0.2/
+-rw-r--r--   0 dario     (1000) dario     (1000)     1069 2023-04-26 22:07:35.000000 dj-rest-admin-1.0.2/LICENSE
+-rw-r--r--   0 dario     (1000) dario     (1000)     6027 2023-05-04 20:53:33.370230 dj-rest-admin-1.0.2/PKG-INFO
+-rw-r--r--   0 dario     (1000) dario     (1000)     4099 2023-04-26 21:53:39.000000 dj-rest-admin-1.0.2/README.md
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2023-05-04 20:53:33.370230 dj-rest-admin-1.0.2/dj_rest_admin/
+-rw-r--r--   0 dario     (1000) dario     (1000)      370 2023-04-26 22:42:48.000000 dj-rest-admin-1.0.2/dj_rest_admin/__init__.py
+-rw-r--r--   0 dario     (1000) dario     (1000)      248 2023-04-26 22:42:44.000000 dj-rest-admin-1.0.2/dj_rest_admin/apps.py
+-rw-r--r--   0 dario     (1000) dario     (1000)     1120 2023-04-26 22:42:40.000000 dj-rest-admin-1.0.2/dj_rest_admin/decorators.py
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2023-05-04 20:53:33.370230 dj-rest-admin-1.0.2/dj_rest_admin/migrations/
+-rw-r--r--   0 dario     (1000) dario     (1000)        0 2023-04-26 21:49:32.000000 dj-rest-admin-1.0.2/dj_rest_admin/migrations/__init__.py
+-rw-r--r--   0 dario     (1000) dario     (1000)      442 2023-04-26 22:42:35.000000 dj-rest-admin-1.0.2/dj_rest_admin/restmodeladmin.py
+-rw-r--r--   0 dario     (1000) dario     (1000)     6089 2023-04-26 22:42:03.000000 dj-rest-admin-1.0.2/dj_rest_admin/sites.py
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2023-05-04 20:53:33.370230 dj-rest-admin-1.0.2/dj_rest_admin.egg-info/
+-rw-r--r--   0 dario     (1000) dario     (1000)     6027 2023-05-04 20:53:33.000000 dj-rest-admin-1.0.2/dj_rest_admin.egg-info/PKG-INFO
+-rw-r--r--   0 dario     (1000) dario     (1000)      399 2023-05-04 20:53:33.000000 dj-rest-admin-1.0.2/dj_rest_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 dario     (1000) dario     (1000)        1 2023-05-04 20:53:33.000000 dj-rest-admin-1.0.2/dj_rest_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 dario     (1000) dario     (1000)       91 2023-05-04 20:53:33.000000 dj-rest-admin-1.0.2/dj_rest_admin.egg-info/requires.txt
+-rw-r--r--   0 dario     (1000) dario     (1000)       14 2023-05-04 20:53:33.000000 dj-rest-admin-1.0.2/dj_rest_admin.egg-info/top_level.txt
+-rw-r--r--   0 dario     (1000) dario     (1000)     1148 2023-05-04 20:53:13.000000 dj-rest-admin-1.0.2/pyproject.toml
+-rw-r--r--   0 dario     (1000) dario     (1000)       38 2023-05-04 20:53:33.370230 dj-rest-admin-1.0.2/setup.cfg
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2023-05-04 20:53:33.370230 dj-rest-admin-1.0.2/tests/
+-rw-r--r--   0 dario     (1000) dario     (1000)    10205 2023-04-26 21:49:32.000000 dj-rest-admin-1.0.2/tests/tests.py
```

### Comparing `dj-rest-admin-1.0.1/LICENSE` & `dj-rest-admin-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-rest-admin-1.0.1/PKG-INFO` & `dj-rest-admin-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-rest-admin
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package to generate CRUD endpoints for registered models with the Django-REST Framework.
 Author-email: Dario Fragas <dariofg98@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Dario Fragas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dj-rest-admin-1.0.1/README.md` & `dj-rest-admin-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dj-rest-admin-1.0.1/dj_rest_admin/decorators.py` & `dj-rest-admin-1.0.2/dj_rest_admin/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,31 @@
     @register(Author)
     class AuthorAdmin(admin.ModelAdmin):
         pass
 
     The `site` kwarg is an admin site to use instead of the default admin site.
     """
     from rest_framework.serializers import ModelSerializer
+
     from .restmodeladmin import RestModelAdmin
     from .sites import AdminSite
     from .sites import site as default_site
-    
 
     def _model_admin_wrapper(admin_class):
         if not models:
             raise ValueError("At least one model must be passed to register.")
 
         admin_site = site or default_site
 
         if not isinstance(admin_site, AdminSite):
             raise ValueError("site must subclass AdminSite")
 
         if not issubclass(admin_class, (RestModelAdmin, ModelSerializer)):
-            raise ValueError("Wrapped class must subclass RestModelAdmin or ModelSerializer.")
+            raise ValueError(
+                "Wrapped class must subclass RestModelAdmin or ModelSerializer."
+            )
 
         admin_site.register(models, serializer_or_modeladmin=admin_class)
 
         return admin_class
 
     return _model_admin_wrapper
```

### Comparing `dj-rest-admin-1.0.1/dj_rest_admin/sites.py` & `dj-rest-admin-1.0.2/dj_rest_admin/sites.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from django.db.models.base import ModelBase
+from typing import List, Type, Union
+
 from django.core.exceptions import ImproperlyConfigured
-from rest_framework import serializers, viewsets, routers, permissions
-from rest_framework.settings import api_settings
-from rest_framework.permissions import BasePermission
+from django.db.models.base import ModelBase
+from rest_framework import permissions, routers, serializers, viewsets
 from rest_framework.documentation import include_docs_urls
-from typing import Type, List, Union
+from rest_framework.permissions import BasePermission
+from rest_framework.settings import api_settings
 
 from .restmodeladmin import RestModelAdmin
 
 
 class AlreadyRegistered(Exception):
     pass
 
@@ -18,86 +19,128 @@
 
 
 class AdminModel:
     pass
 
 
 class AdminSite:
-
     def __init__(self):
         self._registry = {}
         self.admin_router = routers.DefaultRouter()
 
-    def register(self, model_or_iterable, serializer_or_modeladmin: Union[serializers.ModelSerializer, RestModelAdmin] = None,
-                 permission_classes: List[Type[BasePermission]] = None, pagination_class=None):
+    def register(
+        self,
+        model_or_iterable,
+        serializer_or_modeladmin: Union[
+            serializers.ModelSerializer, RestModelAdmin
+        ] = None,
+        permission_classes: List[Type[BasePermission]] = None,
+        pagination_class=None,
+    ):
         """
-        Register Models to the AdminSite. Generates a serializer or uses the one passed.
+        Register Models to the AdminSite.
+        Generates a serializer or uses the one passed.
         """
 
         if isinstance(model_or_iterable, ModelBase):
             model_or_iterable = [model_or_iterable]
         for model in model_or_iterable:
             if model._meta.abstract:
                 raise ImproperlyConfigured(
-                    f"The model {model.__name__} is abstract. It cannot be registered with admin")
+                    f"The model {model.__name__} is abstract. "
+                    "It cannot be registered with admin"
+                )
 
             if model in self._registry:
-                raise AlreadyRegistered(f"The model {model.__name__} has already been registered")
+                raise AlreadyRegistered(
+                    f"The model {model.__name__} has already been registered"
+                )
             model_name = model.__name__
-            
-            if serializer_or_modeladmin and issubclass(serializer_or_modeladmin, serializers.ModelSerializer):
+
+            if serializer_or_modeladmin and issubclass(
+                serializer_or_modeladmin, serializers.ModelSerializer
+            ):
                 serializer_class = serializer_or_modeladmin
-            elif serializer_or_modeladmin and issubclass(serializer_or_modeladmin, RestModelAdmin):
+            elif serializer_or_modeladmin and issubclass(
+                serializer_or_modeladmin, RestModelAdmin
+            ):
                 self._register_restmodel_admin(model, serializer_or_modeladmin)
                 continue
             else:
-                serializer_class = type(f"{model_name}Serializer", (serializers.ModelSerializer,), {
-                    'Meta': type('Meta', (object,), {
-                        'model': model,
-                        'fields': '__all__'
-                    })
-                })
-
-            generated_viewset_permission_class = permission_classes or [permissions.IsAdminUser]
-            generated_viewset_pagination_class = pagination_class or api_settings.DEFAULT_PAGINATION_CLASS
-
-            viewset = type(f"{model_name}ViewSet", (viewsets.ModelViewSet,), {
-                'queryset': model.objects.all(),
-                'permission_classes': generated_viewset_permission_class,
-                'pagination_class': generated_viewset_pagination_class,
-                'serializer_class': serializer_class,
-            })
+                serializer_class = type(
+                    f"{model_name}Serializer",
+                    (serializers.ModelSerializer,),
+                    {
+                        "Meta": type(
+                            "Meta", (object,), {"model": model, "fields": "__all__"}
+                        )
+                    },
+                )
+
+            generated_viewset_permission_class = permission_classes or [
+                permissions.IsAdminUser
+            ]
+            generated_viewset_pagination_class = (
+                pagination_class or api_settings.DEFAULT_PAGINATION_CLASS
+            )
+
+            viewset = type(
+                f"{model_name}ViewSet",
+                (viewsets.ModelViewSet,),
+                {
+                    "queryset": model.objects.all(),
+                    "permission_classes": generated_viewset_permission_class,
+                    "pagination_class": generated_viewset_pagination_class,
+                    "serializer_class": serializer_class,
+                },
+            )
             self._registry[model] = viewset
             #
-            self.admin_router.register(f"{model._meta.app_label}/{model_name}", viewset, f"admin_{model_name}")
-    
+            self.admin_router.register(
+                f"{model._meta.app_label}/{model_name}", viewset, f"admin_{model_name}"
+            )
+
     def _register_restmodel_admin(self, model, restmodeladmin):
         """Register RestModelAdmin"""
 
         self._setup_default_modeladmin(model, restmodeladmin)
 
         self._registry[model] = restmodeladmin
         #
-        self.admin_router.register(f"{model._meta.app_label}/{model.__name__}", restmodeladmin, f"admin_{model.__name__}")
+
+        self.admin_router.register(
+            f"{model._meta.app_label}/{model.__name__}".lower(),
+            restmodeladmin,
+            f"admin_{model.__name__}",
+        )
 
     def _setup_default_modeladmin(self, model, restmodeladmin):
         """Check for required attributes and set defaults if not given"""
-        
+
         # No queryset or get_queryset defined
-        if restmodeladmin.queryset is None and not 'get_queryset' in restmodeladmin.__dict__:
+        if (
+            restmodeladmin.queryset is None
+            and "get_queryset" not in restmodeladmin.__dict__
+        ):
             restmodeladmin.queryset = model.objects.all()
-        
+
         # No serializer class or get_serializer_class defined
-        if restmodeladmin.serializer_class is None and not 'get_serializer_class' in restmodeladmin.__dict__:
-            restmodeladmin.serializer_class = type(f"{model.__name__}Serializer", (serializers.ModelSerializer,), {
-                'Meta': type('Meta', (object,), {
-                    'model': model,
-                    'fields': '__all__'
-                })
-            })
+        if (
+            restmodeladmin.serializer_class is None
+            and "get_serializer_class" not in restmodeladmin.__dict__
+        ):
+            restmodeladmin.serializer_class = type(
+                f"{model.__name__}Serializer",
+                (serializers.ModelSerializer,),
+                {
+                    "Meta": type(
+                        "Meta", (object,), {"model": model, "fields": "__all__"}
+                    )
+                },
+            )
 
     def get_registry(self):
         return self._registry
 
     # def get_urls(self):
     #     url_patterns = []
     #     for model, admin_site in self._registry.items():
@@ -115,25 +158,32 @@
         """
         Check If a model is registered
         """
         return model in self._registry
 
     def unregister(self, model):
         """
-        Check if the model is in our registry first, Then delete the viewset object from the router registry,
+        Check if the model is in our registry first,
+        Then delete the viewset object from the router registry,
         Then delete from our registry
         """
         model_name = model.__name__
         if model not in self._registry:
             raise NotRegistered(f"The model {model_name} has not been registered")
         viewset = self._registry[model]
-        self.admin_router.registry.remove((f"{model._meta.app_label}/{model_name}", viewset, f"admin_{model_name}"))
+        self.admin_router.registry.remove(
+            (f"{model._meta.app_label}/{model_name}", viewset, f"admin_{model_name}")
+        )
         del self._registry[model]
 
     @property
     def docs(self):
         urls = self.urls
-        return include_docs_urls(title="RestAdmin Endpoints Documentation", public=True, patterns=urls[0],
-                                 permission_classes=[permissions.IsAdminUser])
+        return include_docs_urls(
+            title="RestAdmin Endpoints Documentation",
+            public=True,
+            patterns=urls[0],
+            permission_classes=[permissions.IsAdminUser],
+        )
 
 
 site = AdminSite()
```

### Comparing `dj-rest-admin-1.0.1/dj_rest_admin.egg-info/PKG-INFO` & `dj-rest-admin-1.0.2/dj_rest_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-rest-admin
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package to generate CRUD endpoints for registered models with the Django-REST Framework.
 Author-email: Dario Fragas <dariofg98@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Dario Fragas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dj-rest-admin-1.0.1/tests/tests.py` & `dj-rest-admin-1.0.2/tests/tests.py`

 * *Files identical despite different names*

