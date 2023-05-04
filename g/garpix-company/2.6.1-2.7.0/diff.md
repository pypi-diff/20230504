# Comparing `tmp/garpix_company-2.6.1.tar.gz` & `tmp/garpix_company-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_company-2.6.1.tar", last modified: Thu Apr 27 15:15:25 2023, max compression
+gzip compressed data, was "garpix_company-2.7.0.tar", last modified: Thu May  4 14:33:26 2023, max compression
```

## Comparing `garpix_company-2.6.1.tar` & `garpix_company-2.7.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.439727 garpix_company-2.6.1/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2023-04-27 15:15:25.000000 garpix_company-2.6.1/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3807 2023-04-27 15:15:25.439570 garpix_company-2.6.1/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.434204 garpix_company-2.6.1/garpix_company/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2301 2023-04-27 15:15:01.000000 garpix_company-2.6.1/garpix_company/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3237 2023-01-24 14:45:59.000000 garpix_company-2.6.1/garpix_company/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.435221 garpix_company-2.6.1/garpix_company/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/admin/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      352 2023-01-30 05:54:06.000000 garpix_company-2.6.1/garpix_company/admin/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-02-02 10:50:50.000000 garpix_company-2.6.1/garpix_company/admin/company_invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      137 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/apps.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      550 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/helpers.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.435527 garpix_company-2.6.1/garpix_company/managers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/managers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/managers/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      254 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/managers/invite.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.435643 garpix_company-2.6.1/garpix_company/migrations/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/migrations/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.435736 garpix_company-2.6.1/garpix_company/mixins/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/mixins/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.435953 garpix_company-2.6.1/garpix_company/mixins/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       53 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/mixins/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-02-02 07:19:24.000000 garpix_company-2.6.1/garpix_company/mixins/views/company_mixin.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.436602 garpix_company-2.6.1/garpix_company/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      177 2022-12-09 15:26:30.000000 garpix_company-2.6.1/garpix_company/models/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5711 2023-02-10 15:45:53.000000 garpix_company-2.6.1/garpix_company/models/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4306 2023-02-14 14:37:52.000000 garpix_company-2.6.1/garpix_company/models/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3371 2023-02-10 15:45:53.000000 garpix_company-2.6.1/garpix_company/models/user_company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1943 2023-01-30 05:54:06.000000 garpix_company-2.6.1/garpix_company/models/user_role.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.437480 garpix_company-2.6.1/garpix_company/permissions/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      130 2023-02-10 15:45:53.000000 garpix_company-2.6.1/garpix_company/permissions/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      985 2023-02-10 15:45:53.000000 garpix_company-2.6.1/garpix_company/permissions/company_admin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      656 2023-02-02 07:34:38.000000 garpix_company-2.6.1/garpix_company/permissions/company_owner.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      441 2023-02-10 15:45:53.000000 garpix_company-2.6.1/garpix_company/permissions/company_user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      420 2022-12-09 14:51:29.000000 garpix_company-2.6.1/garpix_company/permissions/invite_receiver.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.438384 garpix_company-2.6.1/garpix_company/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      266 2023-01-30 05:54:06.000000 garpix_company-2.6.1/garpix_company/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2841 2023-04-27 15:14:15.000000 garpix_company-2.6.1/garpix_company/serializers/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5570 2023-04-27 15:13:08.000000 garpix_company-2.6.1/garpix_company/serializers/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2023-01-30 05:54:06.000000 garpix_company-2.6.1/garpix_company/serializers/role.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-01-20 07:56:37.000000 garpix_company-2.6.1/garpix_company/serializers/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      801 2023-02-10 15:21:14.000000 garpix_company-2.6.1/garpix_company/serializers/user_company.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.438696 garpix_company-2.6.1/garpix_company/services/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-01-30 05:54:06.000000 garpix_company-2.6.1/garpix_company/services/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      609 2023-01-30 05:54:06.000000 garpix_company-2.6.1/garpix_company/services/role_service.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      580 2023-01-30 08:58:28.000000 garpix_company-2.6.1/garpix_company/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-04-27 15:15:01.000000 garpix_company-2.6.1/garpix_company/setup.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/tests.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      733 2023-02-10 15:45:53.000000 garpix_company-2.6.1/garpix_company/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.439368 garpix_company-2.6.1/garpix_company/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      124 2023-01-19 14:51:26.000000 garpix_company-2.6.1/garpix_company/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5459 2023-02-10 15:45:53.000000 garpix_company-2.6.1/garpix_company/views/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2127 2023-02-06 10:05:38.000000 garpix_company-2.6.1/garpix_company/views/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3536 2023-02-06 08:24:58.000000 garpix_company-2.6.1/garpix_company/views/user_company.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.434874 garpix_company-2.6.1/garpix_company.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3807 2023-04-27 15:15:25.000000 garpix_company-2.6.1/garpix_company.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1721 2023-04-27 15:15:25.000000 garpix_company-2.6.1/garpix_company.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-27 15:15:25.000000 garpix_company-2.6.1/garpix_company.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-27 15:15:25.000000 garpix_company-2.6.1/garpix_company.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2023-04-27 15:15:25.000000 garpix_company-2.6.1/garpix_company.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       15 2023-04-27 15:15:25.000000 garpix_company-2.6.1/garpix_company.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-04-27 15:15:25.439777 garpix_company-2.6.1/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-04-27 15:15:25.000000 garpix_company-2.6.1/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.997221 garpix_company-2.7.0/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2023-05-04 14:33:26.000000 garpix_company-2.7.0/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3893 2023-05-04 14:33:26.997074 garpix_company-2.7.0/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.992749 garpix_company-2.7.0/garpix_company/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2441 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3323 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.993768 garpix_company-2.7.0/garpix_company/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/admin/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      403 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/admin/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-02-02 10:50:50.000000 garpix_company-2.7.0/garpix_company/admin/company_invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      137 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      550 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/helpers.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.994070 garpix_company-2.7.0/garpix_company/managers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/managers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/managers/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      254 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/managers/invite.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.994191 garpix_company-2.7.0/garpix_company/migrations/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/migrations/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.994289 garpix_company-2.7.0/garpix_company/mixins/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/mixins/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.994493 garpix_company-2.7.0/garpix_company/mixins/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       53 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/mixins/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-02-02 07:19:24.000000 garpix_company-2.7.0/garpix_company/mixins/views/company_mixin.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.995044 garpix_company-2.7.0/garpix_company/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      222 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/models/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6003 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/models/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4356 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/models/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4095 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/models/user_company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1943 2023-01-30 05:54:06.000000 garpix_company-2.7.0/garpix_company/models/user_role.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.995609 garpix_company-2.7.0/garpix_company/permissions/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      130 2023-02-10 15:45:53.000000 garpix_company-2.7.0/garpix_company/permissions/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1035 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/permissions/company_admin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      656 2023-02-02 07:34:38.000000 garpix_company-2.7.0/garpix_company/permissions/company_owner.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      441 2023-02-10 15:45:53.000000 garpix_company-2.7.0/garpix_company/permissions/company_user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      420 2022-12-09 14:51:29.000000 garpix_company-2.7.0/garpix_company/permissions/invite_receiver.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.996259 garpix_company-2.7.0/garpix_company/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      266 2023-01-30 05:54:06.000000 garpix_company-2.7.0/garpix_company/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3137 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/serializers/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5620 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/serializers/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2023-01-30 05:54:06.000000 garpix_company-2.7.0/garpix_company/serializers/role.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-01-20 07:56:37.000000 garpix_company-2.7.0/garpix_company/serializers/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      851 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/serializers/user_company.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.996457 garpix_company-2.7.0/garpix_company/services/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-01-30 05:54:06.000000 garpix_company-2.7.0/garpix_company/services/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      609 2023-01-30 05:54:06.000000 garpix_company-2.7.0/garpix_company/services/role_service.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      580 2023-01-30 08:58:28.000000 garpix_company-2.7.0/garpix_company/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/setup.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/tests.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      733 2023-02-10 15:45:53.000000 garpix_company-2.7.0/garpix_company/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.996908 garpix_company-2.7.0/garpix_company/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      124 2023-01-19 14:51:26.000000 garpix_company-2.7.0/garpix_company/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5446 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/views/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2127 2023-02-06 10:05:38.000000 garpix_company-2.7.0/garpix_company/views/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3588 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/views/user_company.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.993419 garpix_company-2.7.0/garpix_company.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3893 2023-05-04 14:33:26.000000 garpix_company-2.7.0/garpix_company.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1721 2023-05-04 14:33:26.000000 garpix_company-2.7.0/garpix_company.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-04 14:33:26.000000 garpix_company-2.7.0/garpix_company.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-04 14:33:26.000000 garpix_company-2.7.0/garpix_company.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2023-05-04 14:33:26.000000 garpix_company-2.7.0/garpix_company.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       15 2023-05-04 14:33:26.000000 garpix_company-2.7.0/garpix_company.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-04 14:33:26.997263 garpix_company-2.7.0/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-04 14:33:26.000000 garpix_company-2.7.0/setup.py
```

### Comparing `garpix_company-2.6.1/PKG-INFO` & `garpix_company-2.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_company
-Version: 2.6.1
+Version: 2.7.0
 Home-page: https://github.com/garpixcms/garpix_company
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -81,21 +81,22 @@
 
 class UserCompanyRole(AbstractUserCompanyRole):
     pass
 
 
 ```
 
-Add `GARPIX_COMPANY_MODEL` and `GARPIX_COMPANY_ROLE_MODEL` to `settings.py`:
+Add `GARPIX_COMPANY_MODEL`, `GARPIX_USER_COMPANY_MODEL` and `GARPIX_COMPANY_ROLE_MODEL` to `settings.py`:
 
 ```python
 # settings.py
 
 GARPIX_COMPANY_MODEL = 'app.Company'
 GARPIX_COMPANY_ROLE_MODEL = 'app.UserCompanyRole'
+GARPIX_USER_COMPANY_MODEL = 'garpix_company.UserCompany'
 
 ```
 
 Use `CompanyAdmin` as base in your admin panel:
 ```python
 from django.contrib import admin
```

### Comparing `garpix_company-2.6.1/garpix_company/CHANGELOG.md` & `garpix_company-2.7.0/garpix_company/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+### 2.7.0 (04.05.2023)
+
+- `GARPIX_USER_COMPANY_MODEL` setting added
+- `role` and `stay_in_company` fields added to `change_owner` endpoint
+
 ### 2.6.1 (27.04.2023)
 
 - Invite user bug fixed
 
 ### 2.6.0 (14.02.2023)
 
 - Decline previous invites for the invite to same person
```

### Comparing `garpix_company-2.6.1/garpix_company/CONTRIBUTING.md` & `garpix_company-2.7.0/garpix_company/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.1/garpix_company/README.md` & `garpix_company-2.7.0/garpix_company/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -64,21 +64,22 @@
 
 class UserCompanyRole(AbstractUserCompanyRole):
     pass
 
 
 ```
 
-Add `GARPIX_COMPANY_MODEL` and `GARPIX_COMPANY_ROLE_MODEL` to `settings.py`:
+Add `GARPIX_COMPANY_MODEL`, `GARPIX_USER_COMPANY_MODEL` and `GARPIX_COMPANY_ROLE_MODEL` to `settings.py`:
 
 ```python
 # settings.py
 
 GARPIX_COMPANY_MODEL = 'app.Company'
 GARPIX_COMPANY_ROLE_MODEL = 'app.UserCompanyRole'
+GARPIX_USER_COMPANY_MODEL = 'garpix_company.UserCompany'
 
 ```
 
 Use `CompanyAdmin` as base in your admin panel:
 ```python
 from django.contrib import admin
```

### Comparing `garpix_company-2.6.1/garpix_company/helpers.py` & `garpix_company-2.7.0/garpix_company/helpers.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.1/garpix_company/models/company.py` & `garpix_company-2.7.0/garpix_company/models/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,29 +77,37 @@
     def delete(self, using=None, keep_parents=False):
         self.comp_deleted()
         self.save()
 
     def hard_delete(self):
         super().delete()
 
-    def change_owner(self, new_owner_id, current_user):
+    def change_owner(self, data, current_user):
         from .user_company import UserCompany
         company_role_service = UserCompanyRoleService()
+
+        new_owner_id = data.get('new_owner')
         if self.owner != current_user:
             return False, _('Действие доступно только для владельца компании')
         try:
             user_company = UserCompany.objects.get(company=self, pk=int(new_owner_id))
             if self.owner == user_company.user:
                 return False, _('Пользователь с указанным id уже является владельцем компании')
             if user_company.is_blocked:
                 return False, _('Нельзя сделать владельцем заблокированного пользователя')
             admin_role = company_role_service.get_admin_role()
             owner_role = company_role_service.get_owner_role()
 
-            UserCompany.objects.filter(company=self, user=current_user).update(role=admin_role)
+            new_role = data.get('role', admin_role)
+            stay_in_company = data.get('stay_in_company', True)
+
+            if stay_in_company:
+                UserCompany.objects.filter(company=self, user=current_user).update(role=new_role)
+            else:
+                UserCompany.objects.filter(company=self, user=current_user).delete()
             user_company.role = owner_role
             user_company.save()
             return True, None
         except UserCompany.DoesNotExist:
             return False, _('Пользователь с указанным id не является сотрудником компании')
 
     @classmethod
```

### Comparing `garpix_company-2.6.1/garpix_company/models/invite.py` & `garpix_company-2.7.0/garpix_company/models/invite.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 from django_fsm import FSMField, transition, can_proceed
 from garpix_notify.models import Notify
 from garpix_utils.string import get_random_string
 
 from garpix_company.helpers import CHOICES_INVITE_STATUS_ENUM
 from garpix_company.managers.invite import CreatedInviteManager
 from garpix_company.models.company import get_company_model
-from garpix_company.models.user_company import UserCompany
+from garpix_company.models.user_company import get_user_company_model
 
 User = get_user_model()
+UserCompany = get_user_company_model()
 
 
 class InviteToCompany(models.Model):
     CHOICES_INVITE_STATUS = CHOICES_INVITE_STATUS_ENUM
 
     company = models.ForeignKey(settings.GARPIX_COMPANY_MODEL, on_delete=models.CASCADE, verbose_name=_('Компания'))
     email = models.EmailField(null=True, blank=True, verbose_name=_('E-mail инвайта'))
```

### Comparing `garpix_company-2.6.1/garpix_company/models/user_company.py` & `garpix_company-2.7.0/garpix_company/models/user_company.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from django.conf import settings
 from django.contrib.auth import get_user_model
+from django.core.exceptions import ImproperlyConfigured
 from django.db import models
 from django.db.models import Manager
 from django.utils.translation import ugettext_lazy as _
-
+from django.apps import apps as django_apps
 from garpix_company.models.user_role import get_company_role_model
 
 User = get_user_model()
 
 
 class ActiveManager(Manager):
 
     def get_queryset(self):
         return super().get_queryset().filter(is_blocked=False)
 
 
-class UserCompany(models.Model):
+class AbstractUserCompany(models.Model):
     """
     Модель участников. Связка между компанией и пользователем.
     """
     user = models.ForeignKey(User, on_delete=models.CASCADE, related_name='user_companies', verbose_name=_('Пользователь'))
     company = models.ForeignKey(settings.GARPIX_COMPANY_MODEL, related_name='user_companies', on_delete=models.CASCADE)
     created_at = models.DateTimeField(auto_now_add=True, verbose_name=_("Дата/время создания"))
     is_blocked = models.BooleanField(default=False, verbose_name=_("Заблокирован администратором компании"))
@@ -29,14 +30,15 @@
     objects = Manager()
     active_objects = ActiveManager()
 
     class Meta:
         unique_together = ("user", "company")
         verbose_name = _('Пользователь компании')
         verbose_name_plural = _('Пользователи компании')
+        abstract = True
 
     def block(self):
         """
         Заблокировать участника в компании
         :return: (bool, str)
         """
         if self.company.owner == self.user:
@@ -75,7 +77,25 @@
         if role == CompanyRole.get_owner_role():
             return False, _('Нельзя сделать пользователя владельцем. Воспользуйтесь функционалом смены владельца')
         if role == CompanyRole.get_admin_role() and self.is_blocked:
             return False, _('Нельзя сделать администратором заблокированного пользователя')
         self.role = role
         self.save()
         return True, None
+
+
+class UserCompany(AbstractUserCompany):
+    pass
+
+
+def get_user_company_model():
+    """
+    Return the UserCompany model that is active in this project.
+    """
+    try:
+        return django_apps.get_model(settings.GARPIX_USER_COMPANY_MODEL, require_ready=False)
+    except ValueError:
+        raise ImproperlyConfigured("GARPIX_USER_COMPANY_MODEL must be of the form 'app_label.model_name'")
+    except LookupError:
+        raise ImproperlyConfigured(
+            "GARPIX_USER_COMPANY_MODEL refers to model '%s' that has not been installed" % settings.GARPIX_USER_COMPANY_MODEL
+        )
```

### Comparing `garpix_company-2.6.1/garpix_company/models/user_role.py` & `garpix_company-2.7.0/garpix_company/models/user_role.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.1/garpix_company/permissions/company_admin.py` & `garpix_company-2.7.0/garpix_company/permissions/company_admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from rest_framework import permissions
 
-from garpix_company.models import get_company_model, UserCompany, InviteToCompany
+from garpix_company.models import get_company_model, get_user_company_model, InviteToCompany
 from garpix_company.services.role_service import UserCompanyRoleService
 
 Company = get_company_model()
+UserCompany = get_user_company_model()
 
 
 class CompanyAdminOnly(permissions.BasePermission):
     """
     Доступ только для администратора компании
     """
```

### Comparing `garpix_company-2.6.1/garpix_company/permissions/company_owner.py` & `garpix_company-2.7.0/garpix_company/permissions/company_owner.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.1/garpix_company/serializers/company.py` & `garpix_company-2.7.0/garpix_company/serializers/company.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from django.db import transaction
 from rest_framework import serializers
 from rest_framework.exceptions import ValidationError
 
 from garpix_company.models.company import get_company_model
-from garpix_company.models.user_company import UserCompany
+from garpix_company.models.user_company import get_user_company_model
 from django.utils.translation import ugettext_lazy as _
 
 from garpix_company.models.user_role import get_company_role_model
 from garpix_company.services.role_service import UserCompanyRoleService
 
 Company = get_company_model()
 CompanyRole = get_company_role_model()
+UserCompany = get_user_company_model()
 
 
 class ExtraFieldsCompanySerializerMixin(serializers.Serializer):
 
     def get_field_names(self, declared_fields, info):
         expanded_fields = super().get_field_names(declared_fields, info)
 
@@ -75,9 +76,17 @@
         model = Company
         fields = (
             'title', 'full_title', 'inn', 'ogrn', 'kpp', 'bank_title',
             'bic', 'schet', 'korschet', 'ur_address', 'fact_address'
         )
 
 
-class ChangeOwnerCompanySerializer(serializers.Serializer):
+class ChangeOwnerCompanySerializer(serializers.ModelSerializer):
     new_owner = serializers.IntegerField()
+    stay_in_company = serializers.BooleanField(required=False)
+
+    class Meta:
+        model = UserCompany
+        fields = ('new_owner', 'role', 'stay_in_company')
+        extra_kwargs = {
+            'role': {'required': False}
+        }
```

### Comparing `garpix_company-2.6.1/garpix_company/serializers/invite.py` & `garpix_company-2.7.0/garpix_company/serializers/invite.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 from django.contrib.auth import get_user_model
 from django.db import transaction
 from django.utils.module_loading import import_string
 from garpix_utils.string import get_random_string
 from rest_framework import serializers
 from rest_framework.exceptions import ValidationError
 
-from garpix_company.models import UserCompany
+from garpix_company.models import get_user_company_model
 from garpix_company.models.company import get_company_model
 from garpix_company.models.invite import InviteToCompany
 from django.utils.translation import ugettext_lazy as _
 from garpix_company.models.user_role import get_company_role_model
 
 
 RoleSerializer = import_string(getattr(settings, 'GARPIX_COMPANY_ROLE_SERIALIZER', 'garpix_company.serializers.role.GarpixCompanyRoleSerializer'))
+UserCompany = get_user_company_model()
 
 
 class InviteToCompanySerializer(serializers.ModelSerializer):
 
     class Meta:
         model = InviteToCompany
         fields = ('email', 'user', 'role')
```

### Comparing `garpix_company-2.6.1/garpix_company/serializers/user_company.py` & `garpix_company-2.7.0/garpix_company/serializers/user_company.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from django.conf import settings
 from django.utils.module_loading import import_string
 from rest_framework import serializers
 
-from garpix_company.models.user_company import UserCompany
+from garpix_company.models.user_company import get_user_company_model
 
 
 UserSerializer = import_string(getattr(settings, 'GARPIX_COMPANY_USER_SERIALIZER', 'garpix_company.serializers.GarpixCompanyUserSerializer'))
 RoleSerializer = import_string(getattr(settings, 'GARPIX_COMPANY_ROLE_SERIALIZER', 'garpix_company.serializers.role.GarpixCompanyRoleSerializer'))
+UserCompany = get_user_company_model()
 
 
 class UserCompanySerializer(serializers.ModelSerializer):
 
     user = UserSerializer()
     role = RoleSerializer()
```

### Comparing `garpix_company-2.6.1/garpix_company/services/role_service.py` & `garpix_company-2.7.0/garpix_company/services/role_service.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.1/garpix_company/settings.py` & `garpix_company-2.7.0/garpix_company/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.1/garpix_company/setup.py` & `garpix_company-2.7.0/garpix_company/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_company')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_company',
-    version='2.6.1',
+    version='2.7.0',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_company',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

### Comparing `garpix_company-2.6.1/garpix_company/urls.py` & `garpix_company-2.7.0/garpix_company/urls.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.1/garpix_company/views/company.py` & `garpix_company-2.7.0/garpix_company/views/company.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     @action(detail=True, methods=['POST'])
     def change_owner(self, request, pk):
         company = self.get_object()
         self.check_object_permissions(request, company)
         serializer = ChangeOwnerCompanySerializer(data=request.data, context={"request": request})
         serializer.is_valid(raise_exception=True)
-        result, message = company.change_owner(serializer.data['new_owner'], request.user)
+        result, message = company.change_owner(serializer.data, request.user)
         if result:
             return Response({'status': _('Владелец успешно изменен')}, status=status.HTTP_200_OK)
         return Response({"non_field_error": [message]}, status=status.HTTP_400_BAD_REQUEST)
 
     @action(methods=['post'], detail=True)
     def invite(self, request, pk):
         company = self.get_object()
```

### Comparing `garpix_company-2.6.1/garpix_company/views/invite.py` & `garpix_company-2.7.0/garpix_company/views/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.1/garpix_company/views/user_company.py` & `garpix_company-2.7.0/garpix_company/views/user_company.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 from rest_framework import status, mixins, filters
 from rest_framework.decorators import action
 from rest_framework.response import Response
 from rest_framework.viewsets import GenericViewSet
 from django_filters.rest_framework import DjangoFilterBackend
 from garpix_company.mixins.views import GarpixCompanyViewSetMixin
 from garpix_company.models import get_company_model
-from garpix_company.models.user_company import UserCompany
+from garpix_company.models.user_company import get_user_company_model
 from garpix_company.permissions import CompanyAdminOnly, CompanyOwnerOnly
 from garpix_company.serializers.user_company import UserCompanySerializer, ChangeUserRoleSerializer
 from django.utils.translation import ugettext_lazy as _
 
 
+UserCompany = get_user_company_model()
+
+
 class UserCompanyViewSet(GarpixCompanyViewSetMixin,
                          mixins.RetrieveModelMixin,
                          mixins.DestroyModelMixin,
                          mixins.ListModelMixin,
                          GenericViewSet):
     permission_classes = [CompanyAdminOnly | CompanyOwnerOnly]
     queryset = UserCompany.objects.all()
```

### Comparing `garpix_company-2.6.1/garpix_company.egg-info/PKG-INFO` & `garpix_company-2.7.0/garpix_company.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-company
-Version: 2.6.1
+Version: 2.7.0
 Home-page: https://github.com/garpixcms/garpix_company
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -81,21 +81,22 @@
 
 class UserCompanyRole(AbstractUserCompanyRole):
     pass
 
 
 ```
 
-Add `GARPIX_COMPANY_MODEL` and `GARPIX_COMPANY_ROLE_MODEL` to `settings.py`:
+Add `GARPIX_COMPANY_MODEL`, `GARPIX_USER_COMPANY_MODEL` and `GARPIX_COMPANY_ROLE_MODEL` to `settings.py`:
 
 ```python
 # settings.py
 
 GARPIX_COMPANY_MODEL = 'app.Company'
 GARPIX_COMPANY_ROLE_MODEL = 'app.UserCompanyRole'
+GARPIX_USER_COMPANY_MODEL = 'garpix_company.UserCompany'
 
 ```
 
 Use `CompanyAdmin` as base in your admin panel:
 ```python
 from django.contrib import admin
```

### Comparing `garpix_company-2.6.1/garpix_company.egg-info/SOURCES.txt` & `garpix_company-2.7.0/garpix_company.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.1/setup.py` & `garpix_company-2.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_company')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_company',
-    version='2.6.1',
+    version='2.7.0',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_company',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

