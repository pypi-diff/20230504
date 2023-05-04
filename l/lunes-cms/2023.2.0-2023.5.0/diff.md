# Comparing `tmp/lunes-cms-2023.2.0.tar.gz` & `tmp/lunes-cms-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunes-cms-2023.2.0.tar", last modified: Wed Feb 22 19:49:06 2023, max compression
+gzip compressed data, was "lunes-cms-2023.5.0.tar", last modified: Thu May  4 08:27:27 2023, max compression
```

## Comparing `lunes-cms-2023.2.0.tar` & `lunes-cms-2023.5.0.tar`

### file list

```diff
@@ -1,163 +1,164 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.911553 lunes-cms-2023.2.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11359 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3025 2023-02-22 19:49:06.911553 lunes-cms-2023.2.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1485 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.891553 lunes-cms-2023.2.0/lunes_cms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.895553 lunes-cms-2023.2.0/lunes_cms/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/apps.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/permissions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.895553 lunes-cms-2023.2.0/lunes_cms/api/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/templates/swagger_ui.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      409 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4970 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.895553 lunes-cms-2023.2.0/lunes_cms/api/v1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.895553 lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      424 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/alternative_word_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/discipline_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/document_image_list_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/document_image_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      824 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/document_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      812 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/fallback_icon_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1462 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/feedback_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1180 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/group_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/sponsor_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      543 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/training_set_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2011 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/urls.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.895553 lunes-cms-2023.2.0/lunes_cms/api/v1/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/views/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1870 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/views/discipline_filtered_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1708 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/views/discipline_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1130 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/views/document_by_id_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1623 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/views/document_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/views/feedback_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1412 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/views/group_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/views/sponsors_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1377 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/views/training_set_by_id_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1592 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/views/training_set_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1859 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/api/v1/views/word_viewset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.895553 lunes-cms-2023.2.0/lunes_cms/cms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      128 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/admin.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.899553 lunes-cms-2023.2.0/lunes_cms/cms/admins/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/admins/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/admins/alternative_word_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5565 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/admins/discipline_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7099 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/admins/document_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1151 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/admins/document_image_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2059 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/admins/feedback_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      313 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/admins/group_api_key_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1109 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/admins/sponsor_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10568 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/admins/training_set_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/apps.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2854 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/forms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8869 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/list_filter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.899553 lunes-cms-2023.2.0/lunes_cms/cms/migrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12781 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/migrations/0001_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1787 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/migrations/0002_modify_group_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/migrations/0003_remove_documentimage_name.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2813 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/migrations/0004_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1431 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/migrations/0005_auto_create_id.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3244 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/migrations/0006_convert_group_api_key.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2476 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/migrations/0007_document_created_by_link.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      801 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1375 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/migrations/0009_sponsor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/migrations/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.899553 lunes-cms-2023.2.0/lunes_cms/cms/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/models/alternative_word.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/models/content_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/models/discipline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3570 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/models/document.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3885 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/models/document_image.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2891 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/models/feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/models/group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4574 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/models/group_api_key.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      926 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/models/sponsor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/models/static.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3260 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/models/training_set.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.891553 lunes-cms-2023.2.0/lunes_cms/cms/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.899553 lunes-cms-2023.2.0/lunes_cms/cms/templates/admin/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      965 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/templates/admin/base.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3954 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/templates/admin/delete_confirmation.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3905 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/templates/admin/delete_selected_confirmation.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/templates/admin/object_delete_summary.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1519 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4543 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1363 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/validators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      902 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/cms/widgets.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.903553 lunes-cms-2023.2.0/lunes_cms/core/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/core/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/core/context_processors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/core/logging_formatter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17930 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/core/settings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1853 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/core/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1272 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/core/wsgi.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.903553 lunes-cms-2023.2.0/lunes_cms/help/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/help/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      320 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/help/apps.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.903553 lunes-cms-2023.2.0/lunes_cms/help/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5609 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/help/templates/public_upload.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/help/urls.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.903553 lunes-cms-2023.2.0/lunes_cms/help/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/help/views/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2128 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/help/views/public_upload.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.891553 lunes-cms-2023.2.0/lunes_cms/locale/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.891553 lunes-cms-2023.2.0/lunes_cms/locale/de/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.903553 lunes-cms-2023.2.0/lunes_cms/locale/de/LC_MESSAGES/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9750 2023-02-22 19:48:55.000000 lunes-cms-2023.2.0/lunes_cms/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2023-02-22 19:48:55.000000 lunes-cms-2023.2.0/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      983 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/lunes-cms-cli
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.891553 lunes-cms-2023.2.0/lunes_cms/static/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.891553 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.907553 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    64548 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)   151749 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)    48488 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108539 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4897 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    76483 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4021 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32461 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)   192348 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)   492048 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)   155758 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)   625953 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.907553 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   222911 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   402249 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)    78635 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   311949 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)   131637 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   250568 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.js.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)    58072 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   190253 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.min.js.map
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.907553 lunes-cms-2023.2.0/lunes_cms/static/css/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3988 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/css/corporate_identity.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      807 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/css/feedback.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1384 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/css/overlay.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.907553 lunes-cms-2023.2.0/lunes_cms/static/guidelines/
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1447497 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/guidelines/fotoguide.pdf
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.911553 lunes-cms-2023.2.0/lunes_cms/static/images/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/images/fallback-icon.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/images/logo-lunes-dark.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3181 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/images/logo-lunes.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      933 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/images/logo.svg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.911553 lunes-cms-2023.2.0/lunes_cms/static/js/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/js/corporate_identity.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1430 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/js/image_preview.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    97163 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/js/jquery.min.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/js/manytomany_overlay.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4545 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/lunes_cms/static/js/overlay.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-22 19:49:06.891553 lunes-cms-2023.2.0/lunes_cms.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3025 2023-02-22 19:49:06.000000 lunes-cms-2023.2.0/lunes_cms.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5285 2023-02-22 19:49:06.000000 lunes-cms-2023.2.0/lunes_cms.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-22 19:49:06.000000 lunes-cms-2023.2.0/lunes_cms.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      548 2023-02-22 19:49:06.000000 lunes-cms-2023.2.0/lunes_cms.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-02-22 19:49:06.000000 lunes-cms-2023.2.0/lunes_cms.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2407 2023-02-22 19:49:06.915553 lunes-cms-2023.2.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      187 2023-02-22 19:49:03.000000 lunes-cms-2023.2.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.077775 lunes-cms-2023.5.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11359 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3025 2023-05-04 08:27:27.077775 lunes-cms-2023.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1485 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.049775 lunes-cms-2023.5.0/lunes_cms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.049775 lunes-cms-2023.5.0/lunes_cms/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/apps.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/permissions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.049775 lunes-cms-2023.5.0/lunes_cms/api/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/templates/swagger_ui.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      409 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4970 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.053775 lunes-cms-2023.5.0/lunes_cms/api/v1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.053775 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      424 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/alternative_word_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/discipline_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/document_image_list_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/document_image_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      824 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/document_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      812 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/fallback_icon_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1462 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/feedback_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1180 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/group_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/sponsor_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      543 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/training_set_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2011 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/urls.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.057775 lunes-cms-2023.5.0/lunes_cms/api/v1/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1870 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/discipline_filtered_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1708 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/discipline_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1130 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/document_by_id_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1623 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/document_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/feedback_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1412 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/group_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/sponsors_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1377 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/training_set_by_id_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1592 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/training_set_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1859 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/api/v1/views/word_viewset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.057775 lunes-cms-2023.5.0/lunes_cms/cms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      128 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admin.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.065775 lunes-cms-2023.5.0/lunes_cms/cms/admins/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/alternative_word_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5565 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/discipline_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7099 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/document_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1151 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/document_image_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2059 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/feedback_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      313 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/group_api_key_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1124 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/sponsor_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10568 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/admins/training_set_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/apps.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2854 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/forms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8869 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/list_filter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/cms/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12781 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0001_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1787 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0002_modify_group_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0003_remove_documentimage_name.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2813 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0004_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1431 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0005_auto_create_id.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3244 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0006_convert_group_api_key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2476 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0007_document_created_by_link.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      801 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1375 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0009_sponsor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/0010_sponsor_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/migrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/cms/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/alternative_word.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/content_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/discipline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3570 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/document.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3885 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/document_image.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2891 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4574 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/group_api_key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/sponsor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/static.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3260 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/models/training_set.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.045775 lunes-cms-2023.5.0/lunes_cms/cms/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      965 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3954 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/delete_confirmation.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3905 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/delete_selected_confirmation.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/object_delete_summary.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1519 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4543 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1363 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/validators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      902 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/cms/widgets.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/core/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/core/context_processors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/core/logging_formatter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17930 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/core/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1853 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/core/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1272 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/core/wsgi.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/help/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/help/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      320 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/help/apps.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/help/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5609 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/help/templates/public_upload.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/help/urls.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/help/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/help/views/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2128 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/help/views/public_upload.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.045775 lunes-cms-2023.5.0/lunes_cms/locale/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.045775 lunes-cms-2023.5.0/lunes_cms/locale/de/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.069775 lunes-cms-2023.5.0/lunes_cms/locale/de/LC_MESSAGES/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9782 2023-05-04 08:27:15.000000 lunes-cms-2023.5.0/lunes_cms/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2023-05-04 08:27:15.000000 lunes-cms-2023.5.0/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      983 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/lunes-cms-cli
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.049775 lunes-cms-2023.5.0/lunes_cms/static/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.049775 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.073775 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    64548 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   151749 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    48488 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   108539 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4897 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    76483 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4021 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32461 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   192348 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   492048 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   155758 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   625953 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.077775 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   222911 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   402249 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    78635 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   311949 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   131637 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   250568 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    58072 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   190253 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.min.js.map
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.077775 lunes-cms-2023.5.0/lunes_cms/static/css/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3988 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/css/corporate_identity.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      807 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/css/feedback.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1384 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/css/overlay.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.077775 lunes-cms-2023.5.0/lunes_cms/static/guidelines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1447497 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/guidelines/fotoguide.pdf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.077775 lunes-cms-2023.5.0/lunes_cms/static/images/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/images/fallback-icon.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/images/logo-lunes-dark.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3181 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/images/logo-lunes.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      933 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/images/logo.svg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.077775 lunes-cms-2023.5.0/lunes_cms/static/js/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/js/corporate_identity.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1430 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/js/image_preview.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    97163 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/js/jquery.min.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/js/manytomany_overlay.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4545 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/lunes_cms/static/js/overlay.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:27:27.049775 lunes-cms-2023.5.0/lunes_cms.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3025 2023-05-04 08:27:27.000000 lunes-cms-2023.5.0/lunes_cms.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5330 2023-05-04 08:27:27.000000 lunes-cms-2023.5.0/lunes_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-04 08:27:27.000000 lunes-cms-2023.5.0/lunes_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      548 2023-05-04 08:27:27.000000 lunes-cms-2023.5.0/lunes_cms.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-05-04 08:27:27.000000 lunes-cms-2023.5.0/lunes_cms.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2407 2023-05-04 08:27:27.081776 lunes-cms-2023.5.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      187 2023-05-04 08:27:22.000000 lunes-cms-2023.5.0/setup.py
```

### Comparing `lunes-cms-2023.2.0/LICENSE.txt` & `lunes-cms-2023.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/MANIFEST.in` & `lunes-cms-2023.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/PKG-INFO` & `lunes-cms-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunes-cms
-Version: 2023.2.0
+Version: 2023.5.0
 Summary: Content Management System for the Lunes Vocabulary Trainer App
 Home-page: https://lunes.app/
 Author: Tür an Tür – Digitalfabrik gGmbH
 Author-email: tech@integreat-app.de
 License: Apache License 2.0
 Project-URL: Documentation, https://lunes-cms.rtfd.io
 Project-URL: Issues, https://github.com/digitalfabrik/lunes-cms/issues
```

### Comparing `lunes-cms-2023.2.0/README.md` & `lunes-cms-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/permissions.py` & `lunes-cms-2023.5.0/lunes_cms/api/permissions.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/utils.py` & `lunes-cms-2023.5.0/lunes_cms/api/utils.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/__init__.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/discipline_serializer.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/discipline_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/document_image_list_serializer.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/document_image_list_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/document_image_serializer.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/document_image_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/document_serializer.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/document_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/fallback_icon_serializer.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/fallback_icon_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/feedback_serializer.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/feedback_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/group_serializer.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/group_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/serializers/training_set_serializer.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/serializers/training_set_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/urls.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/views/discipline_filtered_viewset.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/views/discipline_filtered_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/views/discipline_viewset.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/views/discipline_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/views/document_by_id_viewset.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/views/document_by_id_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/views/document_viewset.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/views/document_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/views/group_viewset.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/views/group_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/views/sponsors_viewset.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/views/sponsors_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/views/training_set_by_id_viewset.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/views/training_set_by_id_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/views/training_set_viewset.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/views/training_set_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/api/v1/views/word_viewset.py` & `lunes-cms-2023.5.0/lunes_cms/api/v1/views/word_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/admin.py` & `lunes-cms-2023.5.0/lunes_cms/cms/admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/admins/discipline_admin.py` & `lunes-cms-2023.5.0/lunes_cms/cms/admins/discipline_admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/admins/document_admin.py` & `lunes-cms-2023.5.0/lunes_cms/cms/admins/document_admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/admins/document_image_admin.py` & `lunes-cms-2023.5.0/lunes_cms/cms/admins/document_image_admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/admins/feedback_admin.py` & `lunes-cms-2023.5.0/lunes_cms/cms/admins/feedback_admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/admins/sponsor_admin.py` & `lunes-cms-2023.5.0/lunes_cms/cms/admins/sponsor_admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 class SponsorAdmin(admin.ModelAdmin):
     """
     Admin interface that is used to edit sponsor objects in the CMS.
     """
 
     fields = [
         "name",
+        "url",
         "logo",
         "image_tag",
     ]
     readonly_fields = ["image_tag"]
     list_display = [
         "name",
         "has_logo",
```

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/admins/training_set_admin.py` & `lunes-cms-2023.5.0/lunes_cms/cms/admins/training_set_admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/forms.py` & `lunes-cms-2023.5.0/lunes_cms/cms/forms.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/list_filter.py` & `lunes-cms-2023.5.0/lunes_cms/cms/list_filter.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/migrations/0001_initial.py` & `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/migrations/0002_modify_group_model.py` & `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0002_modify_group_model.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/migrations/0004_feedback.py` & `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0004_feedback.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/migrations/0005_auto_create_id.py` & `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0005_auto_create_id.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/migrations/0006_convert_group_api_key.py` & `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0006_convert_group_api_key.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/migrations/0007_document_created_by_link.py` & `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0007_document_created_by_link.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py` & `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/migrations/0009_sponsor.py` & `lunes-cms-2023.5.0/lunes_cms/cms/migrations/0009_sponsor.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/models/__init__.py` & `lunes-cms-2023.5.0/lunes_cms/cms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/models/alternative_word.py` & `lunes-cms-2023.5.0/lunes_cms/cms/models/alternative_word.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/models/discipline.py` & `lunes-cms-2023.5.0/lunes_cms/cms/models/discipline.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/models/document.py` & `lunes-cms-2023.5.0/lunes_cms/cms/models/document.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/models/document_image.py` & `lunes-cms-2023.5.0/lunes_cms/cms/models/document_image.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/models/feedback.py` & `lunes-cms-2023.5.0/lunes_cms/cms/models/feedback.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/models/group_api_key.py` & `lunes-cms-2023.5.0/lunes_cms/cms/models/group_api_key.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/models/sponsor.py` & `lunes-cms-2023.5.0/lunes_cms/cms/models/sponsor.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,18 @@
     """
 
     name = models.CharField(
         verbose_name=_("name"),
         max_length=255,
         blank=False,
     )
-
+    url = models.URLField(
+        blank=True,
+        verbose_name=_("URL"),
+    )
     logo = models.ImageField(
         upload_to=upload_sponsor_logos,
         validators=[validate_multiple_extensions],
         blank=True,
         verbose_name=_("logo"),
     )
```

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/models/static.py` & `lunes-cms-2023.5.0/lunes_cms/cms/models/static.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/models/training_set.py` & `lunes-cms-2023.5.0/lunes_cms/cms/models/training_set.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/templates/admin/base.html` & `lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/templates/admin/delete_confirmation.html` & `lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/templates/admin/delete_selected_confirmation.html` & `lunes-cms-2023.5.0/lunes_cms/cms/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/urls.py` & `lunes-cms-2023.5.0/lunes_cms/cms/urls.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/utils.py` & `lunes-cms-2023.5.0/lunes_cms/cms/utils.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/validators.py` & `lunes-cms-2023.5.0/lunes_cms/cms/validators.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/cms/widgets.py` & `lunes-cms-2023.5.0/lunes_cms/cms/widgets.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/core/context_processors.py` & `lunes-cms-2023.5.0/lunes_cms/core/context_processors.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/core/logging_formatter.py` & `lunes-cms-2023.5.0/lunes_cms/core/logging_formatter.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/core/settings.py` & `lunes-cms-2023.5.0/lunes_cms/core/settings.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/core/urls.py` & `lunes-cms-2023.5.0/lunes_cms/core/urls.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/core/wsgi.py` & `lunes-cms-2023.5.0/lunes_cms/core/wsgi.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/help/templates/public_upload.html` & `lunes-cms-2023.5.0/lunes_cms/help/templates/public_upload.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/help/views/public_upload.py` & `lunes-cms-2023.5.0/lunes_cms/help/views/public_upload.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/locale/de/LC_MESSAGES/django.mo` & `lunes-cms-2023.5.0/lunes_cms/locale/de/LC_MESSAGES/django.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -205,14 +205,17 @@
 msgid ""
 "The user who marked this feedback as read. If the feedback is unread, this "
 "field is empty."
 msgstr ""
 "Der Benutzer, der dieses Feedback als gelesen markiert hat. Wenn das "
 "Feedback ungelesen ist, ist dieses Feld leer."
 
+msgid "URL"
+msgstr "URL"
+
 msgid "Unrelease selected disciplines"
 msgstr "Ausgewählte Modulgruppen zurückhalten"
 
 msgid "Unrelease selected training sets"
 msgstr "Ausgewählte Module zurückhalten"
 
 msgid "Welcome to the vocabulary management of Lunes!"
```

### Comparing `lunes-cms-2023.2.0/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo` & `lunes-cms-2023.5.0/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/lunes-cms-cli` & `lunes-cms-2023.5.0/lunes_cms/lunes-cms-cli`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-grid.css` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-grid.css.map` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-grid.min.css` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-grid.min.css.map` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.css` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.css.map` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.min.css` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.min.css.map` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap.css` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap.css.map` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap.min.css` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/css/bootstrap.min.css.map` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.js` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.js.map` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.min.js` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.min.js.map` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.js` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.js.map` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.min.js` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/bootstrap/js/bootstrap.min.js.map` & `lunes-cms-2023.5.0/lunes_cms/static/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/css/corporate_identity.css` & `lunes-cms-2023.5.0/lunes_cms/static/css/corporate_identity.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/css/feedback.css` & `lunes-cms-2023.5.0/lunes_cms/static/css/feedback.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/css/overlay.css` & `lunes-cms-2023.5.0/lunes_cms/static/css/overlay.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/guidelines/fotoguide.pdf` & `lunes-cms-2023.5.0/lunes_cms/static/guidelines/fotoguide.pdf`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/images/logo-lunes-dark.svg` & `lunes-cms-2023.5.0/lunes_cms/static/images/logo-lunes-dark.svg`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/images/logo-lunes.svg` & `lunes-cms-2023.5.0/lunes_cms/static/images/logo-lunes.svg`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/images/logo.svg` & `lunes-cms-2023.5.0/lunes_cms/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/js/image_preview.js` & `lunes-cms-2023.5.0/lunes_cms/static/js/image_preview.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/js/jquery.min.js` & `lunes-cms-2023.5.0/lunes_cms/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/js/manytomany_overlay.js` & `lunes-cms-2023.5.0/lunes_cms/static/js/manytomany_overlay.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms/static/js/overlay.js` & `lunes-cms-2023.5.0/lunes_cms/static/js/overlay.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.2.0/lunes_cms.egg-info/PKG-INFO` & `lunes-cms-2023.5.0/lunes_cms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunes-cms
-Version: 2023.2.0
+Version: 2023.5.0
 Summary: Content Management System for the Lunes Vocabulary Trainer App
 Home-page: https://lunes.app/
 Author: Tür an Tür – Digitalfabrik gGmbH
 Author-email: tech@integreat-app.de
 License: Apache License 2.0
 Project-URL: Documentation, https://lunes-cms.rtfd.io
 Project-URL: Issues, https://github.com/digitalfabrik/lunes-cms/issues
```

### Comparing `lunes-cms-2023.2.0/lunes_cms.egg-info/SOURCES.txt` & `lunes-cms-2023.5.0/lunes_cms.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 lunes_cms/cms/migrations/0003_remove_documentimage_name.py
 lunes_cms/cms/migrations/0004_feedback.py
 lunes_cms/cms/migrations/0005_auto_create_id.py
 lunes_cms/cms/migrations/0006_convert_group_api_key.py
 lunes_cms/cms/migrations/0007_document_created_by_link.py
 lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py
 lunes_cms/cms/migrations/0009_sponsor.py
+lunes_cms/cms/migrations/0010_sponsor_url.py
 lunes_cms/cms/migrations/__init__.py
 lunes_cms/cms/models/__init__.py
 lunes_cms/cms/models/alternative_word.py
 lunes_cms/cms/models/content_type.py
 lunes_cms/cms/models/discipline.py
 lunes_cms/cms/models/document.py
 lunes_cms/cms/models/document_image.py
```

### Comparing `lunes-cms-2023.2.0/setup.cfg` & `lunes-cms-2023.5.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lunes-cms
-version = 2023.2.0
+version = 2023.5.0
 author = Tür an Tür – Digitalfabrik gGmbH
 author_email = tech@integreat-app.de
 description = Content Management System for the Lunes Vocabulary Trainer App
 url = https://lunes.app/
 project_urls = 
 	Documentation=https://lunes-cms.rtfd.io
 	Issues=https://github.com/digitalfabrik/lunes-cms/issues
@@ -39,51 +39,51 @@
 	vocabulary-trainer
 	visual-vocabulary-trainer
 
 [options]
 packages = 
 	lunes_cms
 install_requires = 
-	django==3.2.16
+	django==3.2.18
 	django-jazzmin==2.6.0
 	django-mptt==0.14.0
 	django-qr-code==3.1.1
 	djangorestframework==3.14.0
-	drf-spectacular==0.25.1
-	ipython==8.7.0
-	pillow==9.4.0
+	drf-spectacular==0.26.2
+	ipython==8.12.0
+	pillow==9.5.0
 	psycopg2==2.9.5
 	pydub==0.25.1
 python_requires = >=3.8
 include_package_data = True
 scripts = lunes_cms/lunes-cms-cli
 
 [options.extras_require]
 dev = 
 	black==23.1.0
 	bumpver==2022.1120
-	pre-commit==3.0.2
+	pre-commit==3.2.2
 	pyjwt==2.6.0
 	pylint-django==2.5.3
 	pylint-runner==0.6.0
 	shellcheck-py==0.9.0.2
 	twine==4.0.2
 doc = 
 	sphinx==5.3.0
-	sphinx-rtd-theme==1.1.1
+	sphinx-rtd-theme==1.2.0
 	sphinx-last-updated-by-git==0.3.4
-	sphinxcontrib-django2==1.6
+	sphinxcontrib-django==2.3
 test = 
 	pytest-circleci-parallelized==0.1.0
 	pytest-cov==4.0.0
 	pytest-django==4.5.2
-	pytest-xdist==3.1.0
+	pytest-xdist==3.2.1
 
 [bumpver]
-current_version = 2023.2.0
+current_version = 2023.5.0
 version_pattern = YYYY.MM.INC0[-TAG]
 commit_message = 
 	Bump version to {new_version}
 	[skip ci]
 commit = True
 tag = False
 push = False
```

