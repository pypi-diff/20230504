# Comparing `tmp/django-transactional-mail-0.3.0.tar.gz` & `tmp/django-transactional-mail-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-transactional-mail-0.3.0.tar", last modified: Fri Feb  3 20:40:51 2023, max compression
+gzip compressed data, was "django-transactional-mail-0.3.1.tar", last modified: Thu May  4 18:12:40 2023, max compression
```

## Comparing `django-transactional-mail-0.3.0.tar` & `django-transactional-mail-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-02-03 20:40:51.376124 django-transactional-mail-0.3.0/
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1066 2019-12-26 19:13:31.000000 django-transactional-mail-0.3.0/LICENSE
--rw-rw----   0 vinay     (1000) vinay     (1000)       49 2021-03-08 05:06:12.000000 django-transactional-mail-0.3.0/MANIFEST.in
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1247 2023-02-03 20:40:51.376124 django-transactional-mail-0.3.0/PKG-INFO
--rw-rw----   0 vinay     (1000) vinay     (1000)      585 2021-03-24 14:11:46.000000 django-transactional-mail-0.3.0/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-02-03 20:40:51.376124 django-transactional-mail-0.3.0/django_transactional_mail.egg-info/
--rw-rw----   0 vinay     (1000) vinay     (1000)     1247 2023-02-03 20:40:51.000000 django-transactional-mail-0.3.0/django_transactional_mail.egg-info/PKG-INFO
--rw-rw----   0 vinay     (1000) vinay     (1000)      942 2023-02-03 20:40:51.000000 django-transactional-mail-0.3.0/django_transactional_mail.egg-info/SOURCES.txt
--rw-rw----   0 vinay     (1000) vinay     (1000)        1 2023-02-03 20:40:51.000000 django-transactional-mail-0.3.0/django_transactional_mail.egg-info/dependency_links.txt
--rw-rw----   0 vinay     (1000) vinay     (1000)       89 2023-02-03 20:40:51.000000 django-transactional-mail-0.3.0/django_transactional_mail.egg-info/requires.txt
--rw-rw----   0 vinay     (1000) vinay     (1000)       19 2023-02-03 20:40:51.000000 django-transactional-mail-0.3.0/django_transactional_mail.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-02-03 20:40:51.376124 django-transactional-mail-0.3.0/setup.cfg
--rw-rw----   0 vinay     (1000) vinay     (1000)     1195 2023-02-03 20:39:34.000000 django-transactional-mail-0.3.0/setup.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-02-03 20:40:51.376124 django-transactional-mail-0.3.0/transactional_mail/
--rw-r--r--   0 vinay     (1000) vinay     (1000)       70 2019-07-19 16:36:07.000000 django-transactional-mail-0.3.0/transactional_mail/__init__.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)     3530 2021-08-06 15:42:11.000000 django-transactional-mail-0.3.0/transactional_mail/admin.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      292 2019-07-19 16:33:34.000000 django-transactional-mail-0.3.0/transactional_mail/apps.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)     3306 2023-02-03 20:39:19.000000 django-transactional-mail-0.3.0/transactional_mail/emails.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-02-03 20:40:51.376124 django-transactional-mail-0.3.0/transactional_mail/migrations/
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1141 2019-07-19 14:51:33.000000 django-transactional-mail-0.3.0/transactional_mail/migrations/0001_initial.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      601 2019-07-19 14:51:26.000000 django-transactional-mail-0.3.0/transactional_mail/migrations/0002_auto_20180313_2251.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      507 2019-12-30 20:06:41.000000 django-transactional-mail-0.3.0/transactional_mail/migrations/0003_registeredemailtype.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-06-05 15:44:10.000000 django-transactional-mail-0.3.0/transactional_mail/migrations/__init__.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)      538 2019-12-26 20:20:30.000000 django-transactional-mail-0.3.0/transactional_mail/models.py
--rw-rw----   0 vinay     (1000) vinay     (1000)     1343 2021-03-08 03:59:54.000000 django-transactional-mail-0.3.0/transactional_mail/registry.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-02-03 20:40:51.372123 django-transactional-mail-0.3.0/transactional_mail/templates/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-02-03 20:40:51.372123 django-transactional-mail-0.3.0/transactional_mail/templates/admin/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-02-03 20:40:51.376124 django-transactional-mail-0.3.0/transactional_mail/templates/admin/transactional_mail/
--rw-r--r--   0 vinay     (1000) vinay     (1000)      836 2019-12-26 21:38:35.000000 django-transactional-mail-0.3.0/transactional_mail/templates/admin/transactional_mail/preview_table.html
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-02-03 20:40:51.376124 django-transactional-mail-0.3.0/transactional_mail/templates/admin/transactional_mail/registeredemailtype/
--rw-r--r--   0 vinay     (1000) vinay     (1000)      936 2021-03-31 13:33:56.000000 django-transactional-mail-0.3.0/transactional_mail/templates/admin/transactional_mail/registeredemailtype/change_list.html
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-02-03 20:40:51.376124 django-transactional-mail-0.3.0/transactional_mail/templatetags/
--rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-06-05 15:44:10.000000 django-transactional-mail-0.3.0/transactional_mail/templatetags/__init__.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1030 2020-01-16 22:13:47.000000 django-transactional-mail-0.3.0/transactional_mail/templatetags/email_tags.py
--rw-r--r--   0 vinay     (1000) vinay     (1000)       60 2019-06-05 15:44:10.000000 django-transactional-mail-0.3.0/transactional_mail/tests.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-04 18:12:40.480503 django-transactional-mail-0.3.1/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1066 2019-12-26 19:13:31.000000 django-transactional-mail-0.3.1/LICENSE
+-rw-rw----   0 vinay     (1000) vinay     (1000)       49 2021-03-08 05:06:12.000000 django-transactional-mail-0.3.1/MANIFEST.in
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1247 2023-05-04 18:12:40.476503 django-transactional-mail-0.3.1/PKG-INFO
+-rw-rw----   0 vinay     (1000) vinay     (1000)      585 2021-03-24 14:11:46.000000 django-transactional-mail-0.3.1/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-04 18:12:40.476503 django-transactional-mail-0.3.1/django_transactional_mail.egg-info/
+-rw-rw----   0 vinay     (1000) vinay     (1000)     1247 2023-05-04 18:12:40.000000 django-transactional-mail-0.3.1/django_transactional_mail.egg-info/PKG-INFO
+-rw-rw----   0 vinay     (1000) vinay     (1000)      942 2023-05-04 18:12:40.000000 django-transactional-mail-0.3.1/django_transactional_mail.egg-info/SOURCES.txt
+-rw-rw----   0 vinay     (1000) vinay     (1000)        1 2023-05-04 18:12:40.000000 django-transactional-mail-0.3.1/django_transactional_mail.egg-info/dependency_links.txt
+-rw-rw----   0 vinay     (1000) vinay     (1000)       89 2023-05-04 18:12:40.000000 django-transactional-mail-0.3.1/django_transactional_mail.egg-info/requires.txt
+-rw-rw----   0 vinay     (1000) vinay     (1000)       19 2023-05-04 18:12:40.000000 django-transactional-mail-0.3.1/django_transactional_mail.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-05-04 18:12:40.480503 django-transactional-mail-0.3.1/setup.cfg
+-rw-rw----   0 vinay     (1000) vinay     (1000)     1195 2023-05-04 18:12:01.000000 django-transactional-mail-0.3.1/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-04 18:12:40.476503 django-transactional-mail-0.3.1/transactional_mail/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       70 2019-07-19 16:36:07.000000 django-transactional-mail-0.3.1/transactional_mail/__init__.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     3530 2021-08-06 15:42:11.000000 django-transactional-mail-0.3.1/transactional_mail/admin.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      292 2019-07-19 16:33:34.000000 django-transactional-mail-0.3.1/transactional_mail/apps.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     3400 2023-05-04 18:11:26.000000 django-transactional-mail-0.3.1/transactional_mail/emails.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-04 18:12:40.476503 django-transactional-mail-0.3.1/transactional_mail/migrations/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1141 2019-07-19 14:51:33.000000 django-transactional-mail-0.3.1/transactional_mail/migrations/0001_initial.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      601 2019-07-19 14:51:26.000000 django-transactional-mail-0.3.1/transactional_mail/migrations/0002_auto_20180313_2251.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      507 2019-12-30 20:06:41.000000 django-transactional-mail-0.3.1/transactional_mail/migrations/0003_registeredemailtype.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-06-05 15:44:10.000000 django-transactional-mail-0.3.1/transactional_mail/migrations/__init__.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      538 2019-12-26 20:20:30.000000 django-transactional-mail-0.3.1/transactional_mail/models.py
+-rw-rw----   0 vinay     (1000) vinay     (1000)     1343 2021-03-08 03:59:54.000000 django-transactional-mail-0.3.1/transactional_mail/registry.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-04 18:12:40.476503 django-transactional-mail-0.3.1/transactional_mail/templates/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-04 18:12:40.476503 django-transactional-mail-0.3.1/transactional_mail/templates/admin/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-04 18:12:40.476503 django-transactional-mail-0.3.1/transactional_mail/templates/admin/transactional_mail/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      836 2019-12-26 21:38:35.000000 django-transactional-mail-0.3.1/transactional_mail/templates/admin/transactional_mail/preview_table.html
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-04 18:12:40.476503 django-transactional-mail-0.3.1/transactional_mail/templates/admin/transactional_mail/registeredemailtype/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      936 2021-03-31 13:33:56.000000 django-transactional-mail-0.3.1/transactional_mail/templates/admin/transactional_mail/registeredemailtype/change_list.html
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-04 18:12:40.476503 django-transactional-mail-0.3.1/transactional_mail/templatetags/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        0 2019-06-05 15:44:10.000000 django-transactional-mail-0.3.1/transactional_mail/templatetags/__init__.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1030 2020-01-16 22:13:47.000000 django-transactional-mail-0.3.1/transactional_mail/templatetags/email_tags.py
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       60 2019-06-05 15:44:10.000000 django-transactional-mail-0.3.1/transactional_mail/tests.py
```

### Comparing `django-transactional-mail-0.3.0/LICENSE` & `django-transactional-mail-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-transactional-mail-0.3.0/PKG-INFO` & `django-transactional-mail-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-transactional-mail
-Version: 0.3.0
+Version: 0.3.1
 Summary: Transactional emails in Django projects made easy
 Home-page: https://github.com/vinaypai/django-transactional-mail/
 Author: Vinay Pai
 Author-email: vinay@vinaypai.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-transactional-mail-0.3.0/README.md` & `django-transactional-mail-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django-transactional-mail-0.3.0/django_transactional_mail.egg-info/PKG-INFO` & `django-transactional-mail-0.3.1/django_transactional_mail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-transactional-mail
-Version: 0.3.0
+Version: 0.3.1
 Summary: Transactional emails in Django projects made easy
 Home-page: https://github.com/vinaypai/django-transactional-mail/
 Author: Vinay Pai
 Author-email: vinay@vinaypai.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-transactional-mail-0.3.0/django_transactional_mail.egg-info/SOURCES.txt` & `django-transactional-mail-0.3.1/django_transactional_mail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-transactional-mail-0.3.0/setup.py` & `django-transactional-mail-0.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # python3 -m twine upload dist/*
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='django-transactional-mail',
-    version='0.3.0',
+    version='0.3.1',
     author='Vinay Pai',
     author_email='vinay@vinaypai.com',
     description='Transactional emails in Django projects made easy',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/vinaypai/django-transactional-mail/',
     packages=setuptools.find_packages(include=['transactional_mail', 'transactional_mail.*']),
```

### Comparing `django-transactional-mail-0.3.0/transactional_mail/admin.py` & `django-transactional-mail-0.3.1/transactional_mail/admin.py`

 * *Files identical despite different names*

### Comparing `django-transactional-mail-0.3.0/transactional_mail/emails.py` & `django-transactional-mail-0.3.1/transactional_mail/emails.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .models import SentMail
 
 class Email:
     template = None
     from_email = settings.DEFAULT_FROM_EMAIL
     user = None
 
-    def __init__(self, to_email, extra_ctx={}):
+    def __init__(self, to_email: str, extra_ctx: dict={}):
         if self.template is None:
             raise ProgrammingError("Email subclasses must set template")
 
         self.to_email = to_email
 
         ctx = {
             'BASE_URL': settings.BASE_URL, **extra_ctx
@@ -104,15 +104,16 @@
         else:
             user = request.user
 
         return cls(user)
 
 class AdminEmail(Email):
     def __init__(self, ctx):
-        super().__init__(ctx, None)
+        email = settings.ADMINS[0][1] if settings.ADMINS else 'admin@example.com'
+        super().__init__(email, ctx)
 
     def send(self):
         mail_admins(
             self.subject,
             self.plain,
             html_message=self.html
         )
```

### Comparing `django-transactional-mail-0.3.0/transactional_mail/migrations/0001_initial.py` & `django-transactional-mail-0.3.1/transactional_mail/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-transactional-mail-0.3.0/transactional_mail/migrations/0002_auto_20180313_2251.py` & `django-transactional-mail-0.3.1/transactional_mail/migrations/0002_auto_20180313_2251.py`

 * *Files identical despite different names*

### Comparing `django-transactional-mail-0.3.0/transactional_mail/models.py` & `django-transactional-mail-0.3.1/transactional_mail/models.py`

 * *Files identical despite different names*

### Comparing `django-transactional-mail-0.3.0/transactional_mail/registry.py` & `django-transactional-mail-0.3.1/transactional_mail/registry.py`

 * *Files identical despite different names*

### Comparing `django-transactional-mail-0.3.0/transactional_mail/templates/admin/transactional_mail/preview_table.html` & `django-transactional-mail-0.3.1/transactional_mail/templates/admin/transactional_mail/preview_table.html`

 * *Files identical despite different names*

### Comparing `django-transactional-mail-0.3.0/transactional_mail/templates/admin/transactional_mail/registeredemailtype/change_list.html` & `django-transactional-mail-0.3.1/transactional_mail/templates/admin/transactional_mail/registeredemailtype/change_list.html`

 * *Files identical despite different names*

### Comparing `django-transactional-mail-0.3.0/transactional_mail/templatetags/email_tags.py` & `django-transactional-mail-0.3.1/transactional_mail/templatetags/email_tags.py`

 * *Files identical despite different names*

