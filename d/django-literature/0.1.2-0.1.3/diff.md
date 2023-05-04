# Comparing `tmp/django_literature-0.1.2.tar.gz` & `tmp/django_literature-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_literature-0.1.2.tar", max compression
+gzip compressed data, was "django_literature-0.1.3.tar", max compression
```

## Comparing `django_literature-0.1.2.tar` & `django_literature-0.1.3.tar`

### file list

```diff
@@ -1,50 +1,54 @@
--rw-r--r--   0        0        0     1089 2023-04-25 14:17:45.323626 django_literature-0.1.2/LICENSE
--rw-r--r--   0        0        0     1736 2023-04-25 14:17:45.323626 django_literature-0.1.2/README.rst
--rw-r--r--   0        0        0       22 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/__init__.py
--rw-r--r--   0        0        0     6237 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/admin.py
--rw-r--r--   0        0        0        0 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/api/__init__.py
--rw-r--r--   0        0        0      398 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/api/serialize.py
--rw-r--r--   0        0        0      249 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/api/urls.py
--rw-r--r--   0        0        0      370 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/api/views.py
--rw-r--r--   0        0        0      250 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/apps.py
--rw-r--r--   0        0        0     2514 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/choices.py
--rw-r--r--   0        0        0      724 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/conf.py
--rw-r--r--   0        0        0    36126 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/csl_map.py
--rw-r--r--   0        0        0     1332 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/drf.py
--rw-r--r--   0        0        0      192 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/exceptions.py
--rw-r--r--   0        0        0      761 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/fields.py
--rw-r--r--   0        0        0     5189 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/forms.py
--rw-r--r--   0        0        0     2906 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/formset.py
--rw-r--r--   0        0        0     4159 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/managers.py
--rw-r--r--   0        0        0    13989 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/migrations/0001_initial.py
--rw-r--r--   0        0        0      655 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/migrations/0002_alter_literature_published.py
--rw-r--r--   0        0        0      478 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/migrations/0003_literature_csl.py
--rw-r--r--   0        0        0     2871 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/migrations/0004_remove_literature_doi_remove_literature_isbn_and_more.py
--rw-r--r--   0        0        0      577 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/migrations/0005_remove_literature_pid_remove_literature_pid_type_and_more.py
--rw-r--r--   0        0        0        0 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/migrations/__init__.py
--rw-r--r--   0        0        0     8632 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/models.py
--rw-r--r--   0        0        0     6071 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/base.html
--rw-r--r--   0        0        0     2370 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/admin/change_list.html
--rw-r--r--   0        0        0     2085 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/admin/search.html
--rw-r--r--   0        0        0      615 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/author_detail.html
--rw-r--r--   0        0        0     1349 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/author_list.html
--rw-r--r--   0        0        0       73 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/bibliography.html
--rw-r--r--   0        0        0      665 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/citation/bootstrap.html
--rw-r--r--   0        0        0      465 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/citation/plain_text.html
--rw-r--r--   0        0        0      332 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/literature_detail.html
--rw-r--r--   0        0        0     1591 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/literature_form.html
--rw-r--r--   0        0        0      788 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/literature_form1.html
--rw-r--r--   0        0        0      186 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/literature_list.html
--rw-r--r--   0        0        0      301 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/widgets/identifier.html
--rw-r--r--   0        0        0     1128 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/widgets/pdf_viewer.html
--rw-r--r--   0        0        0     1120 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/widgets/postgres_array_widget.html
--rw-r--r--   0        0        0      348 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/widgets/preview.html
--rw-r--r--   0        0        0        0 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templatetags/__init__.py
--rw-r--r--   0        0        0      568 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templatetags/literature.py
--rw-r--r--   0        0        0     1296 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/test.py
--rw-r--r--   0        0        0      429 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/urls.py
--rw-r--r--   0        0        0     1241 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/utils.py
--rw-r--r--   0        0        0     3040 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/views.py
--rw-r--r--   0        0        0      538 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/widgets.py
--rw-r--r--   0        0        0     3936 2023-04-25 14:18:11.520056 django_literature-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3080 1970-01-01 00:00:00.000000 django_literature-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-04 11:45:36.141295 django_literature-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2343 2023-05-04 11:45:36.141295 django_literature-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/__init__.py
+-rw-r--r--   0        0        0     6237 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/admin.py
+-rw-r--r--   0        0        0        0 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/api/__init__.py
+-rw-r--r--   0        0        0      398 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/api/serialize.py
+-rw-r--r--   0        0        0      249 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/api/urls.py
+-rw-r--r--   0        0        0      370 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/api/views.py
+-rw-r--r--   0        0        0      250 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/apps.py
+-rw-r--r--   0        0        0     2514 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/choices.py
+-rw-r--r--   0        0        0      724 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/conf.py
+-rw-r--r--   0        0        0    36128 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/csl_map.py
+-rw-r--r--   0        0        0      985 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/drf.py
+-rw-r--r--   0        0        0      761 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/fields.py
+-rw-r--r--   0        0        0     4965 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/forms.py
+-rw-r--r--   0        0        0     2576 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/formset.py
+-rw-r--r--   0        0        0     1932 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/managers.py
+-rw-r--r--   0        0        0    13989 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/migrations/0001_initial.py
+-rw-r--r--   0        0        0      655 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/migrations/0002_alter_literature_published.py
+-rw-r--r--   0        0        0      478 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/migrations/0003_literature_csl.py
+-rw-r--r--   0        0        0     2871 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/migrations/0004_remove_literature_doi_remove_literature_isbn_and_more.py
+-rw-r--r--   0        0        0      577 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/migrations/0005_remove_literature_pid_remove_literature_pid_type_and_more.py
+-rw-r--r--   0        0        0        0 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/migrations/__init__.py
+-rw-r--r--   0        0        0     8578 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/models.py
+-rw-r--r--   0        0        0     4667 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/static/literature/icons/icons.svg
+-rw-r--r--   0        0        0     1513 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/static/literature/icons/three-dots.svg
+-rw-r--r--   0        0        0     3106 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/static/literature/js/admin/change_list.js
+-rw-r--r--   0        0        0     3111 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/static/literature/js/datatablesHyperlink.js
+-rw-r--r--   0        0        0     1715 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/static/literature/js/main copy.js
+-rw-r--r--   0        0        0     2012 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/static/literature/js/main.js
+-rw-r--r--   0        0        0     6071 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/base.html
+-rw-r--r--   0        0        0     2370 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/admin/change_list.html
+-rw-r--r--   0        0        0     2085 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/admin/search.html
+-rw-r--r--   0        0        0      615 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/author_detail.html
+-rw-r--r--   0        0        0     1349 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/author_list.html
+-rw-r--r--   0        0        0       73 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/bibliography.html
+-rw-r--r--   0        0        0      665 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/citation/bootstrap.html
+-rw-r--r--   0        0        0      465 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/citation/plain_text.html
+-rw-r--r--   0        0        0      332 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/literature_detail.html
+-rw-r--r--   0        0        0     1591 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/literature_form.html
+-rw-r--r--   0        0        0      788 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/literature_form1.html
+-rw-r--r--   0        0        0      186 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/literature_list.html
+-rw-r--r--   0        0        0      301 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/widgets/identifier.html
+-rw-r--r--   0        0        0     1128 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/widgets/pdf_viewer.html
+-rw-r--r--   0        0        0     1120 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/widgets/postgres_array_widget.html
+-rw-r--r--   0        0        0      348 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/widgets/preview.html
+-rw-r--r--   0        0        0        0 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templatetags/__init__.py
+-rw-r--r--   0        0        0      568 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templatetags/literature.py
+-rw-r--r--   0        0        0      429 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/urls.py
+-rw-r--r--   0        0        0     1241 2023-05-04 11:45:36.149295 django_literature-0.1.3/literature/utils.py
+-rw-r--r--   0        0        0     3040 2023-05-04 11:45:36.149295 django_literature-0.1.3/literature/views.py
+-rw-r--r--   0        0        0      828 2023-05-04 11:45:36.149295 django_literature-0.1.3/literature/widgets.py
+-rw-r--r--   0        0        0     3947 2023-05-04 11:46:06.313609 django_literature-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 django_literature-0.1.3/PKG-INFO
```

### Comparing `django_literature-0.1.2/LICENSE` & `django_literature-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/admin.py` & `django_literature-0.1.3/literature/admin.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/choices.py` & `django_literature-0.1.3/literature/choices.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/conf.py` & `django_literature-0.1.3/literature/conf.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/csl_map.py` & `django_literature-0.1.3/literature/csl_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 # typeMaps = {}
 # for el in tree.findall(".//typeMap"):
 #     typeMaps[el.get("cslType")] = [ZOTERO_FIELD_MAP.get(field.get('value'), field.get('value')) for field in el.findall("field")]
 
 # pprint.pprint(typeMaps)
 
-"""The module level attributes here were generated from the csl-typeMap.xml file at github.com/citation-style-language/schema and tweaked to suit the needs of this application."""
+# """The module level attributes here were generated from the csl-typeMap.xml file at github.com/citation-style-language/schema and tweaked to suit the needs of this application."""
 
 CSL_TYPES = {
     "article": [
         "title",
         "abstract",
         "genre",
         "repository",
```

### Comparing `django_literature-0.1.2/literature/fields.py` & `django_literature-0.1.3/literature/fields.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/forms.py` & `django_literature-0.1.3/literature/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,17 +154,7 @@
     help_text = "I'm a form designed to edit a literature object"
 
     default_renderer = bootstrap.FormRenderer()
     # literature = LiteratureForm()
     required = LiteratureRequired()
     extra = LiteratureExtra()
     supps = SuppMatCollection()
-
-
-# class AuthorForm(ModelForm):
-#     class Meta:
-#         model = Author
-#         fields = ['phone_number']
-
-# class LiteratureCollection(FormCollection):
-#     literature = LiteratureForm()
-#     authors = AuthorForm()
```

### Comparing `django_literature-0.1.2/literature/formset.py` & `django_literature-0.1.3/literature/formset.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,44 +6,38 @@
 from formset.fieldset import Fieldset
 from formset.renderers import bootstrap
 from formset.richtext.widgets import RichTextarea
 from formset.widgets import (
     Selectize,
 )
 
-# from django.forms import fields
 from .choices import TypeChoices
 from .csl_map import CSL_FIELDS, CSL_TYPES
 
-# def show_if(field):
-# return {"show-if": " || ".join([f".type == '{x}'" for x in CSLMap[field]])}
-
 
 class CSLMixin:
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.csl_fields = CSL_FIELDS
-        self.csl_types = CSL_TYPES
         self.update_fields()
         self.update_field_visibility()
 
     def update_fields(self):
         for field in self.Meta.fields:
-            attrs = self.csl_fields[field]
+            attrs = CSL_FIELDS[field]
             if attrs["type"] == "standard":
                 self.fields[field] = forms.CharField(
                     label=attrs["name"],
                     help_text=_(attrs["description"]),
                     required=False,
                     widget=self.Meta.widgets.get(field, None),
                 )
                 self.fields[field].widget.attrs.update({"show-if": ""})
 
     def update_field_visibility(self):
-        for csl_type, fields in self.csl_types.items():
+        for csl_type, fields in CSL_TYPES.items():
             for field_name in fields:
                 if field_name in self.fields:
                     if not self.fields[field_name].widget.attrs["show-if"]:
                         self.fields[field_name].widget.attrs["show-if"] += f"literature.type == '{csl_type}'"
                     else:
                         self.fields[field_name].widget.attrs["show-if"] += f" || literature.type == '{csl_type}'"
 
@@ -67,17 +61,14 @@
         widgets = {
             # "pdf": PDFFileInput(),
             "abstract": RichTextarea(),
             # "published": DateInput,
             # "authors": DualSortableSelector,  # or DualSelector
         }
 
-    # def show_if(field):
-    #     return {"show-if": " || ".join([f".type == '{x}'" for x in CSLMap[field]])}
-
 
 class LiteratureFormCollection(FormCollection):
     # legend = "I'm the literature form"
     # help_text = "I'm a form designed to edit a literature object"
 
     default_renderer = bootstrap.FormRenderer(field_css_classes="mb-3")
```

### Comparing `django_literature-0.1.2/literature/migrations/0001_initial.py` & `django_literature-0.1.3/literature/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/migrations/0002_alter_literature_published.py` & `django_literature-0.1.3/literature/migrations/0002_alter_literature_published.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/migrations/0004_remove_literature_doi_remove_literature_isbn_and_more.py` & `django_literature-0.1.3/literature/migrations/0004_remove_literature_doi_remove_literature_isbn_and_more.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/migrations/0005_remove_literature_pid_remove_literature_pid_type_and_more.py` & `django_literature-0.1.3/literature/migrations/0005_remove_literature_pid_remove_literature_pid_type_and_more.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/models.py` & `django_literature-0.1.3/literature/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from django.utils.translation import gettext as _
 from model_utils import FieldTracker
 from model_utils.models import TimeStampedModel
 from sortedm2m.fields import SortedManyToManyField
 from taggit.managers import TaggableManager
 
 from .choices import IdentifierTypes, TypeChoices
-from .managers import AuthorManager, LiteratureManager
+from .managers import AuthorManager
 from .utils import pdf_file_renamer
 
 
 class LiteratureAuthor(models.Model):
     """An intermediate table for the Work-Author m2m relationship.
     `SortedManyToManyField` automatically creates this table, however, there is no access via querysets. Defining here instead allows us to have access to the intermediate table in order to query author position.
     """
@@ -106,16 +106,14 @@
     def __str__(self):
         return f"{self.get_type_display()} <{self.ID}>"
 
 
 class Literature(TimeStampedModel):
     """Model for storing literature data"""
 
-    objects = LiteratureManager()
-
     # ARTICLE TYPE
     type = models.CharField(_("type"), choices=TypeChoices.choices, max_length=255)  # noqa: A003
 
     # THE FOLLOWING FIELDS ARE DEFINED HERE AS THEY MAY BENEFIT FROM INDEXING
     abstract = models.TextField(_("abstract"), blank=True, null=True)
     container_title = models.CharField(
         _("container title"),
```

### Comparing `django_literature-0.1.2/literature/templates/base.html` & `django_literature-0.1.3/literature/templates/base.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/templates/literature/admin/change_list.html` & `django_literature-0.1.3/literature/templates/literature/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/templates/literature/admin/search.html` & `django_literature-0.1.3/literature/templates/literature/admin/search.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/templates/literature/author_detail.html` & `django_literature-0.1.3/literature/templates/literature/author_detail.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/templates/literature/author_list.html` & `django_literature-0.1.3/literature/templates/literature/author_list.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/templates/literature/citation/bootstrap.html` & `django_literature-0.1.3/literature/templates/literature/citation/bootstrap.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/templates/literature/literature_form.html` & `django_literature-0.1.3/literature/templates/literature/literature_form.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/templates/literature/literature_form1.html` & `django_literature-0.1.3/literature/templates/literature/literature_form1.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/templates/literature/widgets/pdf_viewer.html` & `django_literature-0.1.3/literature/templates/literature/widgets/pdf_viewer.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/templates/literature/widgets/postgres_array_widget.html` & `django_literature-0.1.3/literature/templates/literature/widgets/postgres_array_widget.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/templatetags/literature.py` & `django_literature-0.1.3/literature/templatetags/literature.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/utils.py` & `django_literature-0.1.3/literature/utils.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/literature/views.py` & `django_literature-0.1.3/literature/views.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.2/pyproject.toml` & `django_literature-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "django-literature"
-version = "0.1.2"
+version = "0.1.3"
 description = "A scientific literature management tool for Django"
 authors = ["Sam Jennings <samuel.scott.jennings@gmail.com>"]
 license = "MIT"
-readme = "README.rst"
+readme = "README.md"
 packages = [{include = "literature"}]
 homepage = "https://github.com/SSJenny90/django-literature"
 keywords = ["django", "literature", "publications", "scientific", "research"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: Django :: 3.2",
     "Intended Audience :: Developers",
@@ -187,12 +187,12 @@
     3.10: py310
     3.11: py311
     
 [testenv]
 passenv = PYTHON_VERSION
 allowlist_externals = poetry
 commands =
-    poetry install -v
+    poetry install --without docs
     pytest --doctest-modules tests --cov --cov-config=pyproject.toml --cov-report=xml
     mypy
 """
```

### Comparing `django_literature-0.1.2/PKG-INFO` & `django_literature-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,121 +1,71 @@
-Metadata-Version: 2.1
-Name: django-literature
-Version: 0.1.2
-Summary: A scientific literature management tool for Django
-Home-page: https://github.com/SSJenny90/django-literature
-License: MIT
-Keywords: django,literature,publications,scientific,research
-Author: Sam Jennings
-Author-email: samuel.scott.jennings@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: Django :: 3.2
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: django (>=3.2)
-Requires-Dist: django-appconf (>=1.0.5,<2.0.0)
-Requires-Dist: django-formset (>=0.13.4,<0.14.0)
-Requires-Dist: django-model-utils (>=4.3.1,<5.0.0)
-Requires-Dist: django-sortedm2m (>=3.1.1,<4.0.0)
-Requires-Dist: django-taggit (>=3.1.0,<4.0.0)
-Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
-Requires-Dist: drf-schema-adapter (>=3.0.6,<4.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Description-Content-Type: text/x-rst
-
-=============================
-Django Literature
-=============================
+# Django Literature 
 
-.. image:: https://badge.fury.io/py/django-literature.svg
-    :target: https://badge.fury.io/py/django-literature
-
-.. image:: https://travis-ci.org/SSJenny90/django-literature.svg?branch=master
-    :target: https://travis-ci.org/SSJenny90/django-literature
-
-.. image:: https://codecov.io/gh/SSJenny90/django-literature/branch/main/graph/badge.svg?token=0Q18CLIKZE 
- :target: https://codecov.io/gh/SSJenny90/django-literature
+[![Github Build](https://github.com/SSJenny90/django-literature/actions/workflows/build.yml/badge.svg)](https://github.com/SSJenny90/django-literature/actions/workflows/build.yml)
+[![Github Docs](https://github.com/SSJenny90/django-literature/actions/workflows/docs.yml/badge.svg)](https://github.com/SSJenny90/django-literature/actions/workflows/docs.yml)
+[![CodeCov](https://codecov.io/gh/SSJenny90/django-literature/branch/main/graph/badge.svg?token=0Q18CLIKZE)](https://codecov.io/gh/SSJenny90/django-literature)
+![GitHub](https://img.shields.io/github/license/SSJenny90/django-literature)
+![GitHub last commit](https://img.shields.io/github/last-commit/SSJenny90/django-literature)
+![PyPI](https://img.shields.io/pypi/v/django-literature)
+<!-- [![RTD](https://readthedocs.org/projects/django-literature/badge/?version=latest)](https://django-literature.readthedocs.io/en/latest/readme.html) -->
+<!-- [![Documentation](https://github.com/SSJenny90/django-literature/actions/workflows/build-docs.yml/badge.svg)](https://github.com/SSJenny90/django-literature/actions/workflows/build-docs.yml) -->
+<!-- [![PR](https://img.shields.io/github/issues-pr/SSJenny90/django-literature)](https://github.com/SSJenny90/django-literature/pulls)
+[![Issues](https://img.shields.io/github/issues-raw/SSJenny90/django-literature)](https://github.com/SSJenny90/django-literature/pulls) -->
+<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/django-literature) -->
+<!-- ![PyPI - Status](https://img.shields.io/pypi/status/django-literature) -->
 
 A scientific literature management app for Django
 
 Documentation
 -------------
 
-The full documentation is at https://django-literature.readthedocs.io.
+The full documentation is at https://ssjenny90.github.io/django-literature/
 
 Quickstart
 ----------
 
 Install Django Literature::
 
     pip install django-literature
 
 Add it to your `INSTALLED_APPS`:
 
-.. code-block:: python
 
     INSTALLED_APPS = (
         ...
-        'literature.apps.LiteratureConfig',
+        'literature',
         ...
     )
 
 Add Django Literature's URL patterns:
 
-.. code-block:: python
-
-    from literature import urls as literature_urls
-
-
     urlpatterns = [
         ...
-        url(r'^', include(literature_urls)),
+        path('', include("literature.urls")),
         ...
     ]
 
 Features
 --------
 
 * TODO
 
 Running Tests
 -------------
 
 Does the code actually work?
 
-::
-
     source <YOURVIRTUALENV>/bin/activate
     (myenv) $ pip install tox
     (myenv) $ tox
 
 
 Development commands
 ---------------------
 
-::
-
     pip install -r requirements_dev.txt
     invoke -l
 
 
 Credits
 -------
 
-Tools used in rendering this package:
-
-*  Cookiecutter_
-*  `cookiecutter-djangopackage`_
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
-
```

