# Comparing `tmp/django-rest-registration-0.8.0.tar.gz` & `tmp/django-rest-registration-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-rest-registration-0.8.0.tar", last modified: Fri Mar 31 09:49:31 2023, max compression
+gzip compressed data, was "dist/django-rest-registration-0.8.1.tar", last modified: Thu May  4 10:00:56 2023, max compression
```

## Comparing `django-rest-registration-0.8.0.tar` & `django-rest-registration-0.8.1.tar`

### file list

```diff
@@ -1,107 +1,104 @@
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.542078 django-rest-registration-0.8.0/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1088 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/LICENSE
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      161 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/MANIFEST.in
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     5956 2023-03-31 09:49:31.542361 django-rest-registration-0.8.0/PKG-INFO
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4560 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/README.md
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.335662 django-rest-registration-0.8.0/django_rest_registration.egg-info/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     5956 2023-03-31 09:49:31.000000 django-rest-registration-0.8.0/django_rest_registration.egg-info/PKG-INFO
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3365 2023-03-31 09:49:31.000000 django-rest-registration-0.8.0/django_rest_registration.egg-info/SOURCES.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        1 2023-03-31 09:49:31.000000 django-rest-registration-0.8.0/django_rest_registration.egg-info/dependency_links.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       37 2023-03-31 09:49:31.000000 django-rest-registration-0.8.0/django_rest_registration.egg-info/requires.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       18 2023-03-31 09:49:31.000000 django-rest-registration-0.8.0/django_rest_registration.egg-info/top_level.txt
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.414269 django-rest-registration-0.8.0/rest_registration/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      135 2023-03-30 09:35:45.000000 django-rest-registration-0.8.0/rest_registration/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       22 2023-03-31 09:46:27.000000 django-rest-registration-0.8.0/rest_registration/_version.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/admin.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.419103 django-rest-registration-0.8.0/rest_registration/api/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/api/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4738 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/api/serializers.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      946 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/api/urls.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.429967 django-rest-registration-0.8.0/rest_registration/api/views/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      333 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/api/views/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1498 2022-10-04 22:18:47.000000 django-rest-registration-0.8.0/rest_registration/api/views/base.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2099 2022-10-04 22:18:47.000000 django-rest-registration-0.8.0/rest_registration/api/views/change_password.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4012 2022-10-04 22:18:47.000000 django-rest-registration-0.8.0/rest_registration/api/views/login.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1369 2022-10-04 22:18:47.000000 django-rest-registration-0.8.0/rest_registration/api/views/profile.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4584 2022-10-04 22:18:47.000000 django-rest-registration-0.8.0/rest_registration/api/views/register.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4519 2023-03-29 17:45:06.000000 django-rest-registration-0.8.0/rest_registration/api/views/register_email.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4510 2022-10-04 22:18:47.000000 django-rest-registration-0.8.0/rest_registration/api/views/reset_password.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      149 2019-08-01 20:03:57.000000 django-rest-registration-0.8.0/rest_registration/apps.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3054 2023-01-08 23:02:48.000000 django-rest-registration-0.8.0/rest_registration/auth_token_managers.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)    12298 2023-03-29 17:45:06.000000 django-rest-registration-0.8.0/rest_registration/checks.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.430943 django-rest-registration-0.8.0/rest_registration/contrib/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/contrib/__init__.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.439472 django-rest-registration-0.8.0/rest_registration/contrib/verification_redirects/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/contrib/verification_redirects/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/contrib/verification_redirects/admin.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      225 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/contrib/verification_redirects/apps.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.441250 django-rest-registration-0.8.0/rest_registration/contrib/verification_redirects/migrations/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/contrib/verification_redirects/migrations/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/contrib/verification_redirects/models.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      834 2023-03-29 17:45:06.000000 django-rest-registration-0.8.0/rest_registration/contrib/verification_redirects/settings.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      393 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/contrib/verification_redirects/urls.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1975 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/contrib/verification_redirects/views.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1593 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/enums.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3010 2023-03-29 17:45:06.000000 django-rest-registration-0.8.0/rest_registration/exceptions.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.321221 django-rest-registration-0.8.0/rest_registration/locale/
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.320412 django-rest-registration-0.8.0/rest_registration/locale/fr/
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.444723 django-rest-registration-0.8.0/rest_registration/locale/fr/LC_MESSAGES/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2537 2022-12-08 11:12:05.000000 django-rest-registration-0.8.0/rest_registration/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.320932 django-rest-registration-0.8.0/rest_registration/locale/id/
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.447170 django-rest-registration-0.8.0/rest_registration/locale/id/LC_MESSAGES/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3159 2023-03-29 17:45:06.000000 django-rest-registration-0.8.0/rest_registration/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.321476 django-rest-registration-0.8.0/rest_registration/locale/pt_BR/
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.454496 django-rest-registration-0.8.0/rest_registration/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2304 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.455758 django-rest-registration-0.8.0/rest_registration/migrations/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/migrations/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/models.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.460318 django-rest-registration-0.8.0/rest_registration/notifications/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      133 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/notifications/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2426 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/notifications/email.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      204 2019-10-08 08:40:56.000000 django-rest-registration-0.8.0/rest_registration/notifications/enums.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      678 2023-03-29 17:45:06.000000 django-rest-registration-0.8.0/rest_registration/settings.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)    21417 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/settings_fields.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      316 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/signals.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.465502 django-rest-registration-0.8.0/rest_registration/signers/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/signers/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1405 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/signers/register.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      428 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/signers/register_email.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1293 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/signers/reset_password.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.322835 django-rest-registration-0.8.0/rest_registration/templates/
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.323679 django-rest-registration-0.8.0/rest_registration/templates/rest_registration/
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.468683 django-rest-registration-0.8.0/rest_registration/templates/rest_registration/register/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      255 2019-10-08 08:40:56.000000 django-rest-registration-0.8.0/rest_registration/templates/rest_registration/register/body.html
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       84 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/templates/rest_registration/register/body.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       27 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/templates/rest_registration/register/subject.txt
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.507880 django-rest-registration-0.8.0/rest_registration/templates/rest_registration/register_email/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      689 2019-10-08 08:40:56.000000 django-rest-registration-0.8.0/rest_registration/templates/rest_registration/register_email/body.html
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      380 2019-10-08 08:40:56.000000 django-rest-registration-0.8.0/rest_registration/templates/rest_registration/register_email/body.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      102 2019-10-08 08:40:56.000000 django-rest-registration-0.8.0/rest_registration/templates/rest_registration/register_email/subject.txt
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.512962 django-rest-registration-0.8.0/rest_registration/templates/rest_registration/reset_password/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      258 2019-10-08 08:40:56.000000 django-rest-registration-0.8.0/rest_registration/templates/rest_registration/reset_password/body.html
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       85 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/templates/rest_registration/reset_password/body.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       29 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/templates/rest_registration/reset_password/subject.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/tests.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.538136 django-rest-registration-0.8.0/rest_registration/utils/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/utils/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1038 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/utils/auth_backends.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2996 2023-03-29 17:45:06.000000 django-rest-registration-0.8.0/rest_registration/utils/checks.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1581 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/utils/common.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     6751 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/utils/email.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      955 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/utils/functools.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2706 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/utils/html.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1997 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/utils/nested_settings.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      734 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/utils/responses.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3162 2023-03-29 17:45:06.000000 django-rest-registration-0.8.0/rest_registration/utils/signers.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      600 2023-03-29 17:45:06.000000 django-rest-registration-0.8.0/rest_registration/utils/types.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)    11638 2023-03-29 17:45:06.000000 django-rest-registration-0.8.0/rest_registration/utils/users.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4364 2023-03-29 17:45:06.000000 django-rest-registration-0.8.0/rest_registration/utils/validation.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3731 2023-03-29 17:45:06.000000 django-rest-registration-0.8.0/rest_registration/utils/verification.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3520 2022-09-21 08:03:05.000000 django-rest-registration-0.8.0/rest_registration/verification_notifications.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/rest_registration/views.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3145 2023-03-31 09:49:31.544735 django-rest-registration-0.8.0/setup.cfg
--rwxr-xr-x   0 andrzejpragacz   (502) staff       (20)      176 2023-03-30 09:35:45.000000 django-rest-registration-0.8.0/setup.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-03-31 09:49:31.541231 django-rest-registration-0.8.0/tests/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)    15619 2023-03-29 17:45:06.000000 django-rest-registration-0.8.0/tests/test_checks.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      868 2019-06-21 10:41:29.000000 django-rest-registration-0.8.0/tests/test_settings.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.632416 django-rest-registration-0.8.1/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1088 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/LICENSE
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      173 2023-05-04 09:44:58.000000 django-rest-registration-0.8.1/MANIFEST.in
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     5936 2023-05-04 10:00:56.632730 django-rest-registration-0.8.1/PKG-INFO
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4560 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/README.md
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.560482 django-rest-registration-0.8.1/django_rest_registration.egg-info/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     5936 2023-05-04 10:00:56.000000 django-rest-registration-0.8.1/django_rest_registration.egg-info/PKG-INFO
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3321 2023-05-04 10:00:56.000000 django-rest-registration-0.8.1/django_rest_registration.egg-info/SOURCES.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        1 2023-05-04 10:00:56.000000 django-rest-registration-0.8.1/django_rest_registration.egg-info/dependency_links.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       37 2023-05-04 10:00:56.000000 django-rest-registration-0.8.1/django_rest_registration.egg-info/requires.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       18 2023-05-04 10:00:56.000000 django-rest-registration-0.8.1/django_rest_registration.egg-info/top_level.txt
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.577063 django-rest-registration-0.8.1/rest_registration/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      135 2023-03-30 09:35:45.000000 django-rest-registration-0.8.1/rest_registration/__init__.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       22 2023-05-04 10:00:34.000000 django-rest-registration-0.8.1/rest_registration/_version.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/admin.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.580275 django-rest-registration-0.8.1/rest_registration/api/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/api/__init__.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4738 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/api/serializers.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      946 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/api/urls.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.588471 django-rest-registration-0.8.1/rest_registration/api/views/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      333 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/api/views/__init__.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1498 2022-10-04 22:18:47.000000 django-rest-registration-0.8.1/rest_registration/api/views/base.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2099 2022-10-04 22:18:47.000000 django-rest-registration-0.8.1/rest_registration/api/views/change_password.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4012 2022-10-04 22:18:47.000000 django-rest-registration-0.8.1/rest_registration/api/views/login.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1369 2022-10-04 22:18:47.000000 django-rest-registration-0.8.1/rest_registration/api/views/profile.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4685 2023-04-27 22:36:54.000000 django-rest-registration-0.8.1/rest_registration/api/views/register.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4519 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/api/views/register_email.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4510 2022-10-04 22:18:47.000000 django-rest-registration-0.8.1/rest_registration/api/views/reset_password.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      149 2019-08-01 20:03:57.000000 django-rest-registration-0.8.1/rest_registration/apps.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3054 2023-04-28 08:37:06.000000 django-rest-registration-0.8.1/rest_registration/auth_token_managers.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)    12298 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/checks.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.589345 django-rest-registration-0.8.1/rest_registration/contrib/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/contrib/__init__.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.596274 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/__init__.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/admin.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      225 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/apps.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.597141 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/migrations/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/migrations/__init__.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/models.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      834 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/settings.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      393 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/urls.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1975 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/views.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1593 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/enums.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3010 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/exceptions.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.542505 django-rest-registration-0.8.1/rest_registration/locale/
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.541282 django-rest-registration-0.8.1/rest_registration/locale/fr/
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.598172 django-rest-registration-0.8.1/rest_registration/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2537 2022-12-08 11:12:05.000000 django-rest-registration-0.8.1/rest_registration/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.542094 django-rest-registration-0.8.1/rest_registration/locale/id/
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.598971 django-rest-registration-0.8.1/rest_registration/locale/id/LC_MESSAGES/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3159 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.542909 django-rest-registration-0.8.1/rest_registration/locale/pt_BR/
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.599645 django-rest-registration-0.8.1/rest_registration/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2304 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.600594 django-rest-registration-0.8.1/rest_registration/migrations/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/migrations/__init__.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/models.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.602492 django-rest-registration-0.8.1/rest_registration/notifications/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      133 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/notifications/__init__.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2426 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/notifications/email.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      204 2019-10-08 08:40:56.000000 django-rest-registration-0.8.1/rest_registration/notifications/enums.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      678 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/settings.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)    21417 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/settings_fields.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      316 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/signals.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.605583 django-rest-registration-0.8.1/rest_registration/signers/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/signers/__init__.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1405 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/signers/register.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      428 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/signers/register_email.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1293 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/signers/reset_password.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.545236 django-rest-registration-0.8.1/rest_registration/templates/
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.546743 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.608298 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      255 2019-10-08 08:40:56.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register/body.html
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       84 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register/body.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       27 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register/subject.txt
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.610847 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register_email/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      689 2019-10-08 08:40:56.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register_email/body.html
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      380 2019-10-08 08:40:56.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register_email/body.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      102 2019-10-08 08:40:56.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register_email/subject.txt
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.613991 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/reset_password/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      258 2019-10-08 08:40:56.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/reset_password/body.html
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       85 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/reset_password/body.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       29 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/reset_password/subject.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/tests.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.630781 django-rest-registration-0.8.1/rest_registration/utils/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/utils/__init__.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1038 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/utils/auth_backends.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2996 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/utils/checks.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1581 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/utils/common.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     6751 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/utils/email.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      955 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/utils/functools.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2706 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/utils/html.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1997 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/utils/nested_settings.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      734 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/utils/responses.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3162 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/utils/signers.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      600 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/utils/types.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)    11638 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/utils/users.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4364 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/utils/validation.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3731 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/utils/verification.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3520 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/verification_notifications.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/views.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3145 2023-05-04 10:00:56.634470 django-rest-registration-0.8.1/setup.cfg
+-rwxr-xr-x   0 andrzejpragacz   (502) staff       (20)      176 2023-04-27 22:36:38.000000 django-rest-registration-0.8.1/setup.py
```

### Comparing `django-rest-registration-0.8.0/LICENSE` & `django-rest-registration-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/PKG-INFO` & `django-rest-registration-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: django-rest-registration
-Version: 0.8.0
+Version: 0.8.1
 Summary: User registration REST API, based on django-rest-framework
 Home-page: https://github.com/apragacz/django-rest-registration
 Author: Andrzej Pragacz
 Author-email: apragacz@o2.pl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/apragacz/django-rest-registration/issues
 Project-URL: Documentation, https://django-rest-registration.readthedocs.io/
 Project-URL: Source Code, https://github.com/apragacz/django-rest-registration
 Keywords: django,rest,api,auth,rest-framework,registration,register,login,reset-password,register-email,change-email,sign-up,sign-in
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
@@ -148,9 +147,7 @@
 
 You can find all `REST_REGISTRATION` configuration options
 [here](https://django-rest-registration.readthedocs.io/en/latest/detailed_configuration/all_settings.html).
 
 ## Contributing
 
 If you want to contribute, please refer to separate document [CONTRIBUTING.md](CONTRIBUTING.md).
-
-
```

### Comparing `django-rest-registration-0.8.0/README.md` & `django-rest-registration-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/django_rest_registration.egg-info/PKG-INFO` & `django-rest-registration-0.8.1/django_rest_registration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: django-rest-registration
-Version: 0.8.0
+Version: 0.8.1
 Summary: User registration REST API, based on django-rest-framework
 Home-page: https://github.com/apragacz/django-rest-registration
 Author: Andrzej Pragacz
 Author-email: apragacz@o2.pl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/apragacz/django-rest-registration/issues
 Project-URL: Documentation, https://django-rest-registration.readthedocs.io/
 Project-URL: Source Code, https://github.com/apragacz/django-rest-registration
 Keywords: django,rest,api,auth,rest-framework,registration,register,login,reset-password,register-email,change-email,sign-up,sign-in
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
@@ -148,9 +147,7 @@
 
 You can find all `REST_REGISTRATION` configuration options
 [here](https://django-rest-registration.readthedocs.io/en/latest/detailed_configuration/all_settings.html).
 
 ## Contributing
 
 If you want to contribute, please refer to separate document [CONTRIBUTING.md](CONTRIBUTING.md).
-
-
```

### Comparing `django-rest-registration-0.8.0/django_rest_registration.egg-info/SOURCES.txt` & `django-rest-registration-0.8.1/django_rest_registration.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -72,10 +72,8 @@
 rest_registration/utils/html.py
 rest_registration/utils/nested_settings.py
 rest_registration/utils/responses.py
 rest_registration/utils/signers.py
 rest_registration/utils/types.py
 rest_registration/utils/users.py
 rest_registration/utils/validation.py
-rest_registration/utils/verification.py
-tests/test_checks.py
-tests/test_settings.py
+rest_registration/utils/verification.py
```

### Comparing `django-rest-registration-0.8.0/rest_registration/api/serializers.py` & `django-rest-registration-0.8.1/rest_registration/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/api/urls.py` & `django-rest-registration-0.8.1/rest_registration/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/api/views/base.py` & `django-rest-registration-0.8.1/rest_registration/api/views/base.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/api/views/change_password.py` & `django-rest-registration-0.8.1/rest_registration/api/views/change_password.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/api/views/login.py` & `django-rest-registration-0.8.1/rest_registration/api/views/login.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/api/views/profile.py` & `django-rest-registration-0.8.1/rest_registration/api/views/profile.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/api/views/register.py` & `django-rest-registration-0.8.1/rest_registration/api/views/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,17 @@
         )
         signals.user_activated.send(sender=None, user=user, request=request)
         extra_data = None
         if registration_settings.REGISTER_VERIFICATION_AUTO_LOGIN:
             extra_data = perform_login(request, user)
         return get_ok_response(_("User verified successfully"), extra_data=extra_data)
 
+    def get_serializer_class(self) -> Type[Serializer]:
+        return VerifyRegistrationSerializer
+
 
 verify_registration = VerifyRegistrationView.as_view()
 
 
 def process_verify_registration_data(input_data, serializer_context=None):
     if serializer_context is None:
         serializer_context = {}
```

### Comparing `django-rest-registration-0.8.0/rest_registration/api/views/register_email.py` & `django-rest-registration-0.8.1/rest_registration/api/views/register_email.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/api/views/reset_password.py` & `django-rest-registration-0.8.1/rest_registration/api/views/reset_password.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/auth_token_managers.py` & `django-rest-registration-0.8.1/rest_registration/auth_token_managers.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/checks.py` & `django-rest-registration-0.8.1/rest_registration/checks.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/contrib/verification_redirects/settings.py` & `django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/settings.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/contrib/verification_redirects/views.py` & `django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/views.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/enums.py` & `django-rest-registration-0.8.1/rest_registration/enums.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/exceptions.py` & `django-rest-registration-0.8.1/rest_registration/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/locale/fr/LC_MESSAGES/django.po` & `django-rest-registration-0.8.1/rest_registration/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/locale/id/LC_MESSAGES/django.po` & `django-rest-registration-0.8.1/rest_registration/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/locale/pt_BR/LC_MESSAGES/django.po` & `django-rest-registration-0.8.1/rest_registration/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/notifications/email.py` & `django-rest-registration-0.8.1/rest_registration/notifications/email.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/settings.py` & `django-rest-registration-0.8.1/rest_registration/settings.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/settings_fields.py` & `django-rest-registration-0.8.1/rest_registration/settings_fields.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/signers/register.py` & `django-rest-registration-0.8.1/rest_registration/signers/register.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/signers/reset_password.py` & `django-rest-registration-0.8.1/rest_registration/signers/reset_password.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/templates/rest_registration/register_email/body.html` & `django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register_email/body.html`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/utils/auth_backends.py` & `django-rest-registration-0.8.1/rest_registration/utils/auth_backends.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/utils/checks.py` & `django-rest-registration-0.8.1/rest_registration/utils/checks.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/utils/common.py` & `django-rest-registration-0.8.1/rest_registration/utils/common.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/utils/email.py` & `django-rest-registration-0.8.1/rest_registration/utils/email.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/utils/functools.py` & `django-rest-registration-0.8.1/rest_registration/utils/functools.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/utils/html.py` & `django-rest-registration-0.8.1/rest_registration/utils/html.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/utils/nested_settings.py` & `django-rest-registration-0.8.1/rest_registration/utils/nested_settings.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/utils/responses.py` & `django-rest-registration-0.8.1/rest_registration/utils/responses.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/utils/signers.py` & `django-rest-registration-0.8.1/rest_registration/utils/signers.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/utils/types.py` & `django-rest-registration-0.8.1/rest_registration/utils/types.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/utils/users.py` & `django-rest-registration-0.8.1/rest_registration/utils/users.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/utils/validation.py` & `django-rest-registration-0.8.1/rest_registration/utils/validation.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/utils/verification.py` & `django-rest-registration-0.8.1/rest_registration/utils/verification.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/rest_registration/verification_notifications.py` & `django-rest-registration-0.8.1/rest_registration/verification_notifications.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.0/setup.cfg` & `django-rest-registration-0.8.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.0
+current_version = 0.8.1
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)
 serialize = 
 	{major}.{minor}.{patch}
 
 [metadata]
```

