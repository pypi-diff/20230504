# Comparing `tmp/ai-django-core-7.0.0.tar.gz` & `tmp/ai-django-core-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-django-core-7.0.0.tar", last modified: Tue Mar 28 10:56:44 2023, max compression
+gzip compressed data, was "ai-django-core-7.0.1.tar", last modified: Thu May  4 13:25:36 2023, max compression
```

## Comparing `ai-django-core-7.0.0.tar` & `ai-django-core-7.0.1.tar`

### file list

```diff
@@ -1,216 +1,216 @@
--rw-r--r--   0        0        0       82 2020-11-10 13:14:44.154401 ai-django-core-7.0.0/.coveragerc
--rw-r--r--   0        0        0      288 2021-01-14 07:24:43.398405 ai-django-core-7.0.0/.editorconfig
--rw-r--r--   0        0        0     1736 2023-03-28 10:54:28.055319 ai-django-core-7.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      440 2021-03-04 09:38:08.535097 ai-django-core-7.0.0/.gitignore
--rw-r--r--   0        0        0     3941 2023-02-21 14:56:53.431540 ai-django-core-7.0.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      904 2023-03-28 10:21:30.616476 ai-django-core-7.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      462 2021-10-22 07:56:33.382491 ai-django-core-7.0.0/.readthedocs.yml
--rw-r--r--   0        0        0    18602 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/CHANGES.md
--rw-r--r--   0        0        0      962 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/Dockerfile
--rw-r--r--   0        0        0     1104 2020-11-13 14:09:23.939844 ai-django-core-7.0.0/LICENSE.md
--rw-r--r--   0        0        0      133 2021-05-12 15:25:03.940857 ai-django-core-7.0.0/MANIFEST.in
--rw-r--r--   0        0        0     4514 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/README.md
--rw-r--r--   0        0        0       94 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/ai_django_core/__init__.py
--rw-r--r--   0        0        0        0 2021-04-09 06:37:42.469103 ai-django-core-7.0.0/ai_django_core/admin/__init__.py
--rw-r--r--   0        0        0        0 2021-04-09 06:37:42.470102 ai-django-core-7.0.0/ai_django_core/admin/model_admins/__init__.py
--rw-r--r--   0        0        0     1644 2022-05-24 06:35:41.773628 ai-django-core-7.0.0/ai_django_core/admin/model_admins/classes.py
--rw-r--r--   0        0        0      824 2022-05-24 06:35:41.774630 ai-django-core-7.0.0/ai_django_core/admin/model_admins/inlines.py
--rw-r--r--   0        0        0     4623 2022-05-24 06:35:41.775628 ai-django-core-7.0.0/ai_django_core/admin/model_admins/mixins.py
--rw-r--r--   0        0        0        0 2021-04-09 06:37:42.475273 ai-django-core-7.0.0/ai_django_core/admin/views/__init__.py
--rw-r--r--   0        0        0     1100 2022-05-24 06:35:41.776629 ai-django-core-7.0.0/ai_django_core/admin/views/forms.py
--rw-r--r--   0        0        0     2427 2022-05-24 06:35:41.777629 ai-django-core-7.0.0/ai_django_core/admin/views/mixins.py
--rw-r--r--   0        0        0      205 2023-03-28 10:19:53.622405 ai-django-core-7.0.0/ai_django_core/apps.py
--rw-r--r--   0        0        0      942 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/ai_django_core/context_manager.py
--rw-r--r--   0        0        0      147 2020-11-10 13:14:44.158402 ai-django-core-7.0.0/ai_django_core/context_processors.py
--rw-r--r--   0        0        0        0 2020-11-10 13:14:44.160402 ai-django-core-7.0.0/ai_django_core/drf/__init__.py
--rw-r--r--   0        0        0     1031 2021-04-20 12:41:00.456568 ai-django-core-7.0.0/ai_django_core/drf/fields.py
--rw-r--r--   0        0        0     1143 2022-05-24 06:35:41.778630 ai-django-core-7.0.0/ai_django_core/drf/serializers.py
--rw-r--r--   0        0        0     3226 2022-05-24 06:35:41.779630 ai-django-core-7.0.0/ai_django_core/drf/tests.py
--rw-r--r--   0        0        0        0 2022-01-28 16:15:47.090253 ai-django-core-7.0.0/ai_django_core/gitlab/__init__.py
--rw-r--r--   0        0        0     9623 2023-01-18 08:31:21.694327 ai-django-core-7.0.0/ai_django_core/gitlab/coverage.py
--rw-r--r--   0        0        0        0 2020-11-13 14:09:23.941890 ai-django-core-7.0.0/ai_django_core/graphql/__init__.py
--rw-r--r--   0        0        0        0 2020-11-13 14:09:23.942857 ai-django-core-7.0.0/ai_django_core/graphql/forms/__init__.py
--rw-r--r--   0        0        0     1687 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/ai_django_core/graphql/forms/mutations.py
--rw-r--r--   0        0        0        0 2020-11-13 14:09:23.943809 ai-django-core-7.0.0/ai_django_core/graphql/schemes/__init__.py
--rw-r--r--   0        0        0     2065 2022-05-24 06:35:41.781666 ai-django-core-7.0.0/ai_django_core/graphql/schemes/mutations.py
--rw-r--r--   0        0        0        0 2022-02-04 10:38:34.206745 ai-django-core-7.0.0/ai_django_core/graphql/sentry/__init__.py
--rw-r--r--   0        0        0      419 2022-02-04 10:38:34.206745 ai-django-core-7.0.0/ai_django_core/graphql/sentry/utils.py
--rw-r--r--   0        0        0     1342 2022-05-24 06:35:41.782630 ai-django-core-7.0.0/ai_django_core/graphql/sentry/views.py
--rw-r--r--   0        0        0        0 2020-11-13 14:09:23.943809 ai-django-core-7.0.0/ai_django_core/graphql/tests/__init__.py
--rw-r--r--   0        0        0     2144 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/ai_django_core/graphql/tests/base_test.py
--rw-r--r--   0        0        0     2011 2022-08-15 14:15:09.435312 ai-django-core-7.0.0/ai_django_core/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3041 2022-08-15 14:15:09.435312 ai-django-core-7.0.0/ai_django_core/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-11-10 13:14:44.162402 ai-django-core-7.0.0/ai_django_core/mail/__init__.py
--rw-r--r--   0        0        0        0 2020-11-10 13:14:44.162402 ai-django-core-7.0.0/ai_django_core/mail/backends/__init__.py
--rw-r--r--   0        0        0     3225 2022-09-08 14:02:33.496300 ai-django-core-7.0.0/ai_django_core/mail/backends/whitelist_smtp.py
--rw-r--r--   0        0        0      120 2021-04-21 06:46:28.573328 ai-django-core-7.0.0/ai_django_core/mail/errors.py
--rw-r--r--   0        0        0        0 2020-11-10 13:14:44.163402 ai-django-core-7.0.0/ai_django_core/mail/services/__init__.py
--rw-r--r--   0        0        0    11273 2022-09-19 13:29:54.389265 ai-django-core-7.0.0/ai_django_core/mail/services/base.py
--rw-r--r--   0        0        0    10121 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/ai_django_core/mail/services/tests.py
--rw-r--r--   0        0        0        0 2023-03-28 10:19:53.622405 ai-django-core-7.0.0/ai_django_core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 10:19:53.622405 ai-django-core-7.0.0/ai_django_core/management/commands/__init__.py
--rw-r--r--   0        0        0      302 2023-03-28 10:19:53.622405 ai-django-core-7.0.0/ai_django_core/management/commands/validate_test_structure.py
--rw-r--r--   0        0        0     2550 2022-05-24 06:35:41.788665 ai-django-core-7.0.0/ai_django_core/managers.py
--rw-r--r--   0        0        0        0 2020-11-10 13:14:44.164402 ai-django-core-7.0.0/ai_django_core/middleware/__init__.py
--rw-r--r--   0        0        0     1050 2022-05-24 06:35:41.789666 ai-django-core-7.0.0/ai_django_core/middleware/current_user.py
--rw-r--r--   0        0        0       31 2020-11-10 13:14:44.165401 ai-django-core-7.0.0/ai_django_core/mixins/__init__.py
--rw-r--r--   0        0        0     1958 2022-05-24 06:35:41.790664 ai-django-core-7.0.0/ai_django_core/mixins/bleacher.py
--rw-r--r--   0        0        0     1378 2022-12-19 13:01:29.209174 ai-django-core-7.0.0/ai_django_core/mixins/models.py
--rw-r--r--   0        0        0      246 2022-05-24 06:35:41.790664 ai-django-core-7.0.0/ai_django_core/mixins/validation.py
--rw-r--r--   0        0        0     2591 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/ai_django_core/models.py
--rw-r--r--   0        0        0        0 2022-11-28 15:32:07.384273 ai-django-core-7.0.0/ai_django_core/selectors/__init__.py
--rw-r--r--   0        0        0      362 2022-11-28 15:32:07.385402 ai-django-core-7.0.0/ai_django_core/selectors/base.py
--rw-r--r--   0        0        0     1060 2022-11-28 15:32:07.385402 ai-django-core-7.0.0/ai_django_core/selectors/permission.py
--rw-r--r--   0        0        0        0 2021-12-10 10:03:32.599005 ai-django-core-7.0.0/ai_django_core/sentry/__init__.py
--rw-r--r--   0        0        0      668 2021-12-10 10:03:32.599005 ai-django-core-7.0.0/ai_django_core/sentry/helpers.py
--rw-r--r--   0        0        0        0 2020-11-10 13:14:44.167401 ai-django-core-7.0.0/ai_django_core/services/__init__.py
--rw-r--r--   0        0        0     3223 2021-11-25 10:47:00.939956 ai-django-core-7.0.0/ai_django_core/services/custom_scrubber.py
--rw-r--r--   0        0        0       31 2020-11-10 13:14:44.167401 ai-django-core-7.0.0/ai_django_core/templatetags/__init__.py
--rw-r--r--   0        0        0      244 2020-11-10 13:14:44.168401 ai-django-core-7.0.0/ai_django_core/templatetags/ai_date_tags.py
--rw-r--r--   0        0        0      675 2022-09-08 14:02:33.497415 ai-django-core-7.0.0/ai_django_core/templatetags/ai_email_tags.py
--rw-r--r--   0        0        0      807 2022-09-08 14:02:33.497415 ai-django-core-7.0.0/ai_django_core/templatetags/ai_file_tags.py
--rw-r--r--   0        0        0      194 2020-11-10 13:14:44.168401 ai-django-core-7.0.0/ai_django_core/templatetags/ai_helper_tags.py
--rw-r--r--   0        0        0     1375 2020-11-10 13:14:44.170401 ai-django-core-7.0.0/ai_django_core/templatetags/ai_number_tags.py
--rw-r--r--   0        0        0      384 2020-11-10 13:14:44.170401 ai-django-core-7.0.0/ai_django_core/templatetags/ai_object_tags.py
--rw-r--r--   0        0        0      654 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/ai_django_core/templatetags/ai_string_tags.py
--rw-r--r--   0        0        0        0 2020-11-10 13:14:44.170401 ai-django-core-7.0.0/ai_django_core/tests/__init__.py
--rw-r--r--   0        0        0       60 2022-06-29 09:26:02.622257 ai-django-core-7.0.0/ai_django_core/tests/errors.py
--rw-r--r--   0        0        0     5145 2023-02-13 15:51:14.621663 ai-django-core-7.0.0/ai_django_core/tests/mixins.py
--rw-r--r--   0        0        0        0 2023-03-28 10:19:53.622405 ai-django-core-7.0.0/ai_django_core/tests/structure_validator/__init__.py
--rw-r--r--   0        0        0      397 2023-03-28 10:19:53.622405 ai-django-core-7.0.0/ai_django_core/tests/structure_validator/settings.py
--rw-r--r--   0        0        0     4633 2023-03-28 10:19:53.622405 ai-django-core-7.0.0/ai_django_core/tests/structure_validator/test_structure_validator.py
--rw-r--r--   0        0        0      261 2020-11-10 13:14:44.171401 ai-django-core-7.0.0/ai_django_core/utils/__init__.py
--rw-r--r--   0        0        0      127 2021-01-14 07:24:43.398405 ai-django-core-7.0.0/ai_django_core/utils/cache.py
--rw-r--r--   0        0        0     5971 2023-03-28 10:54:28.065329 ai-django-core-7.0.0/ai_django_core/utils/date.py
--rw-r--r--   0        0        0     1468 2021-01-14 07:24:43.398405 ai-django-core-7.0.0/ai_django_core/utils/file.py
--rw-r--r--   0        0        0      343 2021-01-14 07:24:43.398405 ai-django-core-7.0.0/ai_django_core/utils/log_whodid.py
--rw-r--r--   0        0        0      574 2021-01-14 07:24:43.398405 ai-django-core-7.0.0/ai_django_core/utils/math.py
--rw-r--r--   0        0        0      935 2021-01-14 07:24:43.398405 ai-django-core-7.0.0/ai_django_core/utils/model.py
--rw-r--r--   0        0        0     3970 2022-09-08 14:02:33.505424 ai-django-core-7.0.0/ai_django_core/utils/named_tuple.py
--rw-r--r--   0        0        0     3803 2022-09-19 13:29:54.389265 ai-django-core-7.0.0/ai_django_core/utils/string.py
--rw-r--r--   0        0        0        0 2021-04-20 12:41:00.463080 ai-django-core-7.0.0/ai_django_core/view_layer/__init__.py
--rw-r--r--   0        0        0      750 2021-05-12 15:06:00.458891 ai-django-core-7.0.0/ai_django_core/view_layer/form_mixins.py
--rw-r--r--   0        0        0      485 2021-04-20 12:41:00.463080 ai-django-core-7.0.0/ai_django_core/view_layer/formset_mixins.py
--rw-r--r--   0        0        0     2998 2022-01-24 10:00:35.394971 ai-django-core-7.0.0/ai_django_core/view_layer/formset_view_mixin.py
--rw-r--r--   0        0        0     1585 2023-03-28 10:54:28.065329 ai-django-core-7.0.0/ai_django_core/view_layer/htmx_mixins.py
--rw-r--r--   0        0        0     2110 2022-06-29 09:26:02.622257 ai-django-core-7.0.0/ai_django_core/view_layer/mixins.py
--rw-r--r--   0        0        0        0 2022-06-29 09:26:02.630352 ai-django-core-7.0.0/ai_django_core/view_layer/tests/__init__.py
--rw-r--r--   0        0        0     4120 2022-11-18 09:22:48.279440 ai-django-core-7.0.0/ai_django_core/view_layer/tests/mixins.py
--rw-r--r--   0        0        0     1882 2023-02-21 14:56:53.431540 ai-django-core-7.0.0/ai_django_core/view_layer/views.py
--rw-r--r--   0        0        0      654 2020-11-10 13:14:44.174401 ai-django-core-7.0.0/docs/Makefile
--rw-r--r--   0        0        0     2837 2023-03-28 10:19:53.622405 ai-django-core-7.0.0/docs/conf.py
--rw-r--r--   0        0        0     6729 2021-10-18 07:39:32.497063 ai-django-core-7.0.0/docs/features/admin.md
--rw-r--r--   0        0        0       35 2023-01-11 09:52:17.805374 ai-django-core-7.0.0/docs/features/changelog.rst
--rw-r--r--   0        0        0     2313 2021-01-14 07:24:43.398405 ai-django-core-7.0.0/docs/features/context_manager.md
--rw-r--r--   0        0        0      548 2021-01-14 07:24:43.398405 ai-django-core-7.0.0/docs/features/context_processors.md
--rw-r--r--   0        0        0     7273 2021-11-18 10:21:13.237257 ai-django-core-7.0.0/docs/features/database_anonymisation.md
--rw-r--r--   0        0        0     6807 2021-04-20 12:41:00.463080 ai-django-core-7.0.0/docs/features/djangorestframework.md
--rw-r--r--   0        0        0     2552 2023-01-18 08:31:21.694327 ai-django-core-7.0.0/docs/features/gitlab.md
--rw-r--r--   0        0        0     6565 2022-02-28 07:50:22.449644 ai-django-core-7.0.0/docs/features/graphql.md
--rw-r--r--   0        0        0    10664 2022-02-28 08:19:55.459314 ai-django-core-7.0.0/docs/features/mail.md
--rw-r--r--   0        0        0     5891 2022-11-28 15:32:07.388913 ai-django-core-7.0.0/docs/features/managers.md
--rw-r--r--   0        0        0     5951 2022-12-19 13:01:29.209174 ai-django-core-7.0.0/docs/features/mixins.md
--rw-r--r--   0        0        0     1551 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/docs/features/models.md
--rw-r--r--   0        0        0     4451 2022-11-28 15:32:07.388913 ai-django-core-7.0.0/docs/features/selectors.md
--rw-r--r--   0        0        0     1077 2021-12-10 11:08:53.244274 ai-django-core-7.0.0/docs/features/sentry.md
--rw-r--r--   0        0        0     4977 2021-11-09 07:08:13.635599 ai-django-core-7.0.0/docs/features/services.md
--rw-r--r--   0        0        0     1564 2021-03-17 07:25:04.039629 ai-django-core-7.0.0/docs/features/setup.md
--rw-r--r--   0        0        0    10391 2023-03-28 10:19:53.638030 ai-django-core-7.0.0/docs/features/tests.md
--rw-r--r--   0        0        0      232 2021-11-09 07:08:13.635599 ai-django-core-7.0.0/docs/features/utils.rst
--rw-r--r--   0        0        0      526 2021-01-14 07:24:43.414029 ai-django-core-7.0.0/docs/features/utils/cache.md
--rw-r--r--   0        0        0     7404 2022-12-01 13:52:47.823951 ai-django-core-7.0.0/docs/features/utils/date.md
--rw-r--r--   0        0        0      737 2021-01-14 07:24:43.414029 ai-django-core-7.0.0/docs/features/utils/math.md
--rw-r--r--   0        0        0     1100 2021-01-14 07:24:43.414029 ai-django-core-7.0.0/docs/features/utils/model.md
--rw-r--r--   0        0        0     2405 2021-11-09 07:08:13.635599 ai-django-core-7.0.0/docs/features/utils/named_tuple.md
--rw-r--r--   0        0        0     5847 2021-11-09 07:08:13.635599 ai-django-core-7.0.0/docs/features/utils/string.md
--rw-r--r--   0        0        0    15052 2023-02-21 14:56:53.431540 ai-django-core-7.0.0/docs/features/view-layer.md
--rw-r--r--   0        0        0     1152 2022-11-28 15:32:07.390913 ai-django-core-7.0.0/docs/index.rst
--rwxr-xr-x   0        0        0      795 2020-11-10 13:14:44.177401 ai-django-core-7.0.0/docs/make.bat
--rw-r--r--   0        0        0      677 2020-11-10 13:14:44.177401 ai-django-core-7.0.0/manage.py
--rw-r--r--   0        0        0     3912 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/pyproject.toml
--rw-r--r--   0        0        0       56 2020-11-10 13:14:44.177401 ai-django-core-7.0.0/pytest.ini
--rw-r--r--   0        0        0      190 2022-02-28 08:20:33.491214 ai-django-core-7.0.0/scripts/publish_and_update_mirror.ps1
--rw-r--r--   0        0        0      302 2022-02-28 08:20:33.492601 ai-django-core-7.0.0/scripts/update-mirror.ps1
--rw-r--r--   0        0        0     1769 2022-08-15 14:15:09.445355 ai-django-core-7.0.0/settings.py
--rw-r--r--   0        0        0       69 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/setup.cfg
--rw-r--r--   0        0        0        0 2020-11-10 13:14:44.179401 ai-django-core-7.0.0/testapp/__init__.py
--rw-r--r--   0        0        0        0 2021-03-16 07:23:55.271552 ai-django-core-7.0.0/testapp/api/__init__.py
--rw-r--r--   0        0        0      287 2021-03-16 07:23:55.271552 ai-django-core-7.0.0/testapp/api/serializers.py
--rw-r--r--   0        0        0      257 2021-03-16 07:23:55.271552 ai-django-core-7.0.0/testapp/api/urls.py
--rw-r--r--   0        0        0      524 2021-03-16 07:23:55.271552 ai-django-core-7.0.0/testapp/api/views.py
--rw-r--r--   0        0        0      219 2023-03-28 10:19:53.638030 ai-django-core-7.0.0/testapp/forms.py
--rw-r--r--   0        0        0       97 2022-11-28 15:32:07.391937 ai-django-core-7.0.0/testapp/managers.py
--rw-r--r--   0        0        0      829 2023-02-06 12:05:23.340506 ai-django-core-7.0.0/testapp/migrations/0001_initial.py
--rw-r--r--   0        0        0     2529 2023-02-06 12:05:23.340506 ai-django-core-7.0.0/testapp/migrations/0002_auto_210407.py
--rw-r--r--   0        0        0     2194 2022-05-24 06:35:41.804729 ai-django-core-7.0.0/testapp/migrations/0003_modelwithfktoself.py
--rw-r--r--   0        0        0     1866 2023-02-06 12:05:23.340506 ai-django-core-7.0.0/testapp/migrations/0004_auto_20210511_1343.py
--rw-r--r--   0        0        0      613 2023-02-06 12:05:23.348513 ai-django-core-7.0.0/testapp/migrations/0005_modelwithcleanmixin.py
--rw-r--r--   0        0        0      680 2023-02-06 12:05:23.348513 ai-django-core-7.0.0/testapp/migrations/0006_modelwithselector.py
--rw-r--r--   0        0        0      692 2023-02-06 12:05:23.348513 ai-django-core-7.0.0/testapp/migrations/0007_modelwithsavewithoutsignals.py
--rw-r--r--   0        0        0        0 2020-11-10 13:14:44.179401 ai-django-core-7.0.0/testapp/migrations/__init__.py
--rw-r--r--   0        0        0     3359 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/testapp/models.py
--rw-r--r--   0        0        0      161 2022-11-28 15:32:07.394913 ai-django-core-7.0.0/testapp/selectors.py
--rw-r--r--   0        0        0     1449 2022-08-15 14:15:09.445355 ai-django-core-7.0.0/testapp/templates/403.html
--rw-r--r--   0        0        0      145 2021-03-04 09:32:10.641680 ai-django-core-7.0.0/testapp/templates/test_email.html
--rw-r--r--   0        0        0      148 2021-03-04 09:32:10.641680 ai-django-core-7.0.0/testapp/templates/test_email.txt
--rw-r--r--   0        0        0        0 2023-03-28 10:19:53.638030 ai-django-core-7.0.0/testapp/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 10:19:53.638030 ai-django-core-7.0.0/testapp/tests/missing_init/test_ok.py
--rw-r--r--   0        0        0        0 2023-03-28 10:19:53.638030 ai-django-core-7.0.0/testapp/tests/subdirectory/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 10:19:53.638030 ai-django-core-7.0.0/testapp/tests/subdirectory/missing_test_prefix.py
--rw-r--r--   0        0        0        0 2023-03-28 10:19:53.638030 ai-django-core-7.0.0/testapp/tests/subdirectory/test_ok.py
--rw-r--r--   0        0        0      382 2022-05-24 06:35:41.808921 ai-django-core-7.0.0/testapp/urls.py
--rw-r--r--   0        0        0      490 2022-09-29 17:20:33.983485 ai-django-core-7.0.0/testapp/views.py
--rw-r--r--   0        0        0        0 2020-11-10 13:14:44.180402 ai-django-core-7.0.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2021-04-09 06:37:42.495289 ai-django-core-7.0.0/tests/admin/__init__.py
--rw-r--r--   0        0        0        0 2021-04-09 06:37:42.496229 ai-django-core-7.0.0/tests/admin/model_admin_mixins/__init__.py
--rw-r--r--   0        0        0     2605 2023-03-28 10:19:53.638030 ai-django-core-7.0.0/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py
--rw-r--r--   0        0        0     1898 2022-05-24 06:35:41.810332 ai-django-core-7.0.0/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py
--rw-r--r--   0        0        0     1681 2022-05-24 06:35:41.811338 ai-django-core-7.0.0/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py
--rw-r--r--   0        0        0     1182 2022-05-24 06:35:41.811338 ai-django-core-7.0.0/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py
--rw-r--r--   0        0        0     3869 2022-08-12 15:34:54.695254 ai-django-core-7.0.0/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py
--rw-r--r--   0        0        0     1489 2022-05-24 06:35:41.813338 ai-django-core-7.0.0/tests/admin/model_admin_mixins/test_fetch_object_mixin.py
--rw-r--r--   0        0        0     1907 2022-05-24 06:35:41.814334 ai-django-core-7.0.0/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py
--rw-r--r--   0        0        0        0 2023-03-28 10:19:53.638030 ai-django-core-7.0.0/tests/ambient_toolbox/__init__.py
--rw-r--r--   0        0        0     7498 2023-03-28 10:54:28.065329 ai-django-core-7.0.0/tests/ambient_toolbox/test_test_structure_validator.py
--rw-r--r--   0        0        0        0 2021-04-20 12:41:00.463080 ai-django-core-7.0.0/tests/drf/__init__.py
--rw-r--r--   0        0        0     2578 2022-05-24 06:35:41.815386 ai-django-core-7.0.0/tests/drf/test_fields.py
--rw-r--r--   0        0        0       28 2021-04-20 12:41:00.463080 ai-django-core-7.0.0/tests/files/testfile.txt
--rw-r--r--   0        0        0        0 2022-05-24 06:35:41.816336 ai-django-core-7.0.0/tests/mixins/__init__.py
--rw-r--r--   0        0        0      364 2022-05-24 06:35:41.816336 ai-django-core-7.0.0/tests/mixins/validation.py
--rw-r--r--   0        0        0        0 2022-11-28 15:32:07.395419 ai-django-core-7.0.0/tests/selectors/__init__.py
--rw-r--r--   0        0        0      498 2022-11-28 15:32:07.395419 ai-django-core-7.0.0/tests/selectors/test_base.py
--rw-r--r--   0        0        0     1630 2022-11-28 15:32:07.396425 ai-django-core-7.0.0/tests/selectors/test_permission.py
--rw-r--r--   0        0        0      552 2022-05-24 06:35:41.817336 ai-django-core-7.0.0/tests/test_admin_forms.py
--rw-r--r--   0        0        0     1610 2022-05-24 06:35:41.817336 ai-django-core-7.0.0/tests/test_admin_inlines.py
--rw-r--r--   0        0        0     2649 2022-05-24 06:35:41.818336 ai-django-core-7.0.0/tests/test_admin_model_admins_classes.py
--rw-r--r--   0        0        0     2886 2022-05-24 06:35:41.819334 ai-django-core-7.0.0/tests/test_admin_view_mixins.py
--rw-r--r--   0        0        0     2217 2022-05-24 06:35:41.820371 ai-django-core-7.0.0/tests/test_context_manager.py
--rw-r--r--   0        0        0     9590 2023-01-11 09:41:19.392472 ai-django-core-7.0.0/tests/test_email_test_service.py
--rw-r--r--   0        0        0      821 2020-11-10 13:14:44.181402 ai-django-core-7.0.0/tests/test_log_whodid.py
--rw-r--r--   0        0        0    15502 2022-05-24 06:35:41.822374 ai-django-core-7.0.0/tests/test_mail_services.py
--rw-r--r--   0        0        0     1169 2022-05-24 06:35:41.822374 ai-django-core-7.0.0/tests/test_managers.py
--rw-r--r--   0        0        0     1627 2022-05-24 06:35:41.823344 ai-django-core-7.0.0/tests/test_math.py
--rw-r--r--   0        0        0     2592 2022-02-21 09:30:03.598830 ai-django-core-7.0.0/tests/test_middleware.py
--rw-r--r--   0        0        0     1200 2022-12-19 13:01:29.209174 ai-django-core-7.0.0/tests/test_mixins_models.py
--rw-r--r--   0        0        0     1669 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/tests/test_models.py
--rw-r--r--   0        0        0     1779 2022-05-24 06:35:41.824334 ai-django-core-7.0.0/tests/test_rest_api_mixins.py
--rw-r--r--   0        0        0      663 2022-05-24 06:35:41.825335 ai-django-core-7.0.0/tests/test_scrubbing_service.py
--rw-r--r--   0        0        0     1196 2022-05-24 06:35:41.826335 ai-django-core-7.0.0/tests/test_sentry_helper.py
--rw-r--r--   0        0        0      288 2022-05-24 06:35:41.827372 ai-django-core-7.0.0/tests/test_utils_cache.py
--rw-r--r--   0        0        0    12740 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/tests/test_utils_date.py
--rw-r--r--   0        0        0     1593 2022-05-24 06:35:41.829339 ai-django-core-7.0.0/tests/test_utils_file.py
--rw-r--r--   0        0        0      932 2022-05-24 06:35:41.830340 ai-django-core-7.0.0/tests/test_utils_model.py
--rw-r--r--   0        0        0     3806 2022-05-24 06:35:41.831465 ai-django-core-7.0.0/tests/test_utils_named_tuple.py
--rw-r--r--   0        0        0     5342 2022-05-24 06:35:41.831465 ai-django-core-7.0.0/tests/test_utils_string.py
--rw-r--r--   0        0        0        0 2021-04-09 06:37:42.510051 ai-django-core-7.0.0/tests/tests/__init__.py
--rw-r--r--   0        0        0        0 2021-04-09 06:37:42.511052 ai-django-core-7.0.0/tests/tests/mixins/__init__.py
--rw-r--r--   0        0        0      371 2022-10-12 09:19:16.027824 ai-django-core-7.0.0/tests/tests/mixins/models.py
--rw-r--r--   0        0        0      816 2023-02-13 15:51:14.621663 ai-django-core-7.0.0/tests/tests/mixins/test_django_message_framework.py
--rw-r--r--   0        0        0     2482 2022-05-24 06:35:41.833465 ai-django-core-7.0.0/tests/tests/mixins/test_request_provider_mixin.py
--rw-r--r--   0        0        0     2055 2022-05-24 06:35:41.834526 ai-django-core-7.0.0/tests/tests/test_mail_backends.py
--rw-r--r--   0        0        0        0 2021-04-20 12:41:00.463080 ai-django-core-7.0.0/tests/view_layer/__init__.py
--rw-r--r--   0        0        0     1890 2023-03-28 10:21:30.627841 ai-django-core-7.0.0/tests/view_layer/test_formset_mixins.py
--rw-r--r--   0        0        0     1562 2023-02-21 14:56:53.431540 ai-django-core-7.0.0/tests/view_layer/test_htmx_response_mixin.py
--rw-r--r--   0        0        0     3455 2022-06-29 11:57:30.358496 ai-django-core-7.0.0/tests/view_layer/test_meta_mixins.py
--rw-r--r--   0        0        0     1323 2022-09-29 17:20:33.992372 ai-django-core-7.0.0/tests/view_layer/test_views.py
--rw-r--r--   0        0        0     6713 1970-01-01 00:00:00.000000 ai-django-core-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0       82 2020-04-24 09:15:50.688102 ai-django-core-7.0.1/.coveragerc
+-rw-r--r--   0        0        0      288 2021-01-14 07:19:48.798830 ai-django-core-7.0.1/.editorconfig
+-rw-r--r--   0        0        0     1736 2023-03-28 10:54:55.241821 ai-django-core-7.0.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      400 2021-03-04 09:37:37.670469 ai-django-core-7.0.1/.gitignore
+-rw-r--r--   0        0        0     3941 2023-02-21 14:56:14.192364 ai-django-core-7.0.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      904 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      443 2023-05-02 10:10:53.230359 ai-django-core-7.0.1/.readthedocs.yml
+-rw-r--r--   0        0        0    18390 2023-05-04 13:24:40.338660 ai-django-core-7.0.1/CHANGES.md
+-rw-r--r--   0        0        0      962 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/Dockerfile
+-rw-r--r--   0        0        0     1104 2020-11-11 13:34:13.878022 ai-django-core-7.0.1/LICENSE.md
+-rw-r--r--   0        0        0      129 2021-05-12 15:21:27.853419 ai-django-core-7.0.1/MANIFEST.in
+-rw-r--r--   0        0        0     4710 2023-05-04 13:15:53.544078 ai-django-core-7.0.1/README.md
+-rw-r--r--   0        0        0       91 2023-05-04 13:24:40.338660 ai-django-core-7.0.1/ai_django_core/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-08 14:39:10.018823 ai-django-core-7.0.1/ai_django_core/admin/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-08 14:39:10.018823 ai-django-core-7.0.1/ai_django_core/admin/model_admins/__init__.py
+-rw-r--r--   0        0        0     1644 2022-05-24 06:31:55.191175 ai-django-core-7.0.1/ai_django_core/admin/model_admins/classes.py
+-rw-r--r--   0        0        0      824 2022-05-24 06:31:55.192174 ai-django-core-7.0.1/ai_django_core/admin/model_admins/inlines.py
+-rw-r--r--   0        0        0     4623 2022-05-24 06:31:55.194174 ai-django-core-7.0.1/ai_django_core/admin/model_admins/mixins.py
+-rw-r--r--   0        0        0        0 2021-04-08 14:39:10.030331 ai-django-core-7.0.1/ai_django_core/admin/views/__init__.py
+-rw-r--r--   0        0        0     1100 2022-05-24 06:31:55.195173 ai-django-core-7.0.1/ai_django_core/admin/views/forms.py
+-rw-r--r--   0        0        0     2427 2022-05-24 06:31:55.196174 ai-django-core-7.0.1/ai_django_core/admin/views/mixins.py
+-rw-r--r--   0        0        0      205 2023-03-16 14:29:23.656927 ai-django-core-7.0.1/ai_django_core/apps.py
+-rw-r--r--   0        0        0      942 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/ai_django_core/context_manager.py
+-rw-r--r--   0        0        0      147 2022-05-19 13:07:18.117710 ai-django-core-7.0.1/ai_django_core/context_processors.py
+-rw-r--r--   0        0        0        0 2020-10-30 08:58:27.570199 ai-django-core-7.0.1/ai_django_core/drf/__init__.py
+-rw-r--r--   0        0        0     1031 2022-05-19 13:07:18.117710 ai-django-core-7.0.1/ai_django_core/drf/fields.py
+-rw-r--r--   0        0        0     1143 2022-05-24 06:31:55.197177 ai-django-core-7.0.1/ai_django_core/drf/serializers.py
+-rw-r--r--   0        0        0     3226 2022-05-24 06:31:55.198174 ai-django-core-7.0.1/ai_django_core/drf/tests.py
+-rw-r--r--   0        0        0        0 2022-01-28 15:09:22.800090 ai-django-core-7.0.1/ai_django_core/gitlab/__init__.py
+-rw-r--r--   0        0        0     9623 2023-01-18 08:29:41.824417 ai-django-core-7.0.1/ai_django_core/gitlab/coverage.py
+-rw-r--r--   0        0        0        0 2020-11-11 13:34:13.878022 ai-django-core-7.0.1/ai_django_core/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2020-11-11 13:34:13.879027 ai-django-core-7.0.1/ai_django_core/graphql/forms/__init__.py
+-rw-r--r--   0        0        0     1687 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/ai_django_core/graphql/forms/mutations.py
+-rw-r--r--   0        0        0        0 2020-11-11 13:34:13.880023 ai-django-core-7.0.1/ai_django_core/graphql/schemes/__init__.py
+-rw-r--r--   0        0        0     2065 2022-05-24 06:31:55.201402 ai-django-core-7.0.1/ai_django_core/graphql/schemes/mutations.py
+-rw-r--r--   0        0        0        0 2022-02-04 10:36:09.232865 ai-django-core-7.0.1/ai_django_core/graphql/sentry/__init__.py
+-rw-r--r--   0        0        0      419 2022-05-19 13:07:18.117710 ai-django-core-7.0.1/ai_django_core/graphql/sentry/utils.py
+-rw-r--r--   0        0        0     1342 2022-05-24 06:31:55.202177 ai-django-core-7.0.1/ai_django_core/graphql/sentry/views.py
+-rw-r--r--   0        0        0        0 2020-11-11 13:34:13.880023 ai-django-core-7.0.1/ai_django_core/graphql/tests/__init__.py
+-rw-r--r--   0        0        0     2144 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/ai_django_core/graphql/tests/base_test.py
+-rw-r--r--   0        0        0     2011 2022-09-29 17:01:08.183567 ai-django-core-7.0.1/ai_django_core/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2948 2022-09-29 17:01:08.186898 ai-django-core-7.0.1/ai_django_core/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-10-14 11:54:26.324037 ai-django-core-7.0.1/ai_django_core/mail/__init__.py
+-rw-r--r--   0        0        0        0 2020-10-14 11:54:26.326832 ai-django-core-7.0.1/ai_django_core/mail/backends/__init__.py
+-rw-r--r--   0        0        0     3148 2022-09-29 17:01:08.190635 ai-django-core-7.0.1/ai_django_core/mail/backends/whitelist_smtp.py
+-rw-r--r--   0        0        0      120 2021-04-21 06:44:18.414056 ai-django-core-7.0.1/ai_django_core/mail/errors.py
+-rw-r--r--   0        0        0        0 2020-10-14 11:54:26.326832 ai-django-core-7.0.1/ai_django_core/mail/services/__init__.py
+-rw-r--r--   0        0        0    11273 2022-09-19 13:21:41.288357 ai-django-core-7.0.1/ai_django_core/mail/services/base.py
+-rw-r--r--   0        0        0    10121 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/ai_django_core/mail/services/tests.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.656927 ai-django-core-7.0.1/ai_django_core/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.657928 ai-django-core-7.0.1/ai_django_core/management/commands/__init__.py
+-rw-r--r--   0        0        0      302 2023-03-16 14:29:23.658434 ai-django-core-7.0.1/ai_django_core/management/commands/validate_test_structure.py
+-rw-r--r--   0        0        0     2550 2022-05-24 06:31:55.208172 ai-django-core-7.0.1/ai_django_core/managers.py
+-rw-r--r--   0        0        0        0 2020-10-14 11:54:26.328426 ai-django-core-7.0.1/ai_django_core/middleware/__init__.py
+-rw-r--r--   0        0        0     1050 2022-05-24 06:31:55.209173 ai-django-core-7.0.1/ai_django_core/middleware/current_user.py
+-rw-r--r--   0        0        0       31 2022-05-19 13:07:18.127538 ai-django-core-7.0.1/ai_django_core/mixins/__init__.py
+-rw-r--r--   0        0        0     1958 2022-05-24 06:31:55.210172 ai-django-core-7.0.1/ai_django_core/mixins/bleacher.py
+-rw-r--r--   0        0        0     1378 2023-02-13 12:03:20.486464 ai-django-core-7.0.1/ai_django_core/mixins/models.py
+-rw-r--r--   0        0        0      246 2022-05-24 06:31:55.211171 ai-django-core-7.0.1/ai_django_core/mixins/validation.py
+-rw-r--r--   0        0        0     2591 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/ai_django_core/models.py
+-rw-r--r--   0        0        0        0 2022-11-28 15:41:36.586624 ai-django-core-7.0.1/ai_django_core/selectors/__init__.py
+-rw-r--r--   0        0        0      362 2022-11-28 15:41:36.587626 ai-django-core-7.0.1/ai_django_core/selectors/base.py
+-rw-r--r--   0        0        0     1060 2022-11-28 15:41:36.588627 ai-django-core-7.0.1/ai_django_core/selectors/permission.py
+-rw-r--r--   0        0        0        0 2021-12-10 09:34:59.322678 ai-django-core-7.0.1/ai_django_core/sentry/__init__.py
+-rw-r--r--   0        0        0      668 2022-05-19 13:07:18.127538 ai-django-core-7.0.1/ai_django_core/sentry/helpers.py
+-rw-r--r--   0        0        0        0 2020-10-14 11:54:26.334428 ai-django-core-7.0.1/ai_django_core/services/__init__.py
+-rw-r--r--   0        0        0     3223 2022-05-19 13:07:18.132547 ai-django-core-7.0.1/ai_django_core/services/custom_scrubber.py
+-rw-r--r--   0        0        0       31 2022-05-19 13:07:18.132547 ai-django-core-7.0.1/ai_django_core/templatetags/__init__.py
+-rw-r--r--   0        0        0      244 2020-10-14 11:54:26.435582 ai-django-core-7.0.1/ai_django_core/templatetags/ai_date_tags.py
+-rw-r--r--   0        0        0      647 2022-09-29 17:01:08.196796 ai-django-core-7.0.1/ai_django_core/templatetags/ai_email_tags.py
+-rw-r--r--   0        0        0      771 2022-09-29 17:01:08.197793 ai-django-core-7.0.1/ai_django_core/templatetags/ai_file_tags.py
+-rw-r--r--   0        0        0      194 2020-10-14 11:54:26.432584 ai-django-core-7.0.1/ai_django_core/templatetags/ai_helper_tags.py
+-rw-r--r--   0        0        0     1375 2022-05-19 13:07:18.132547 ai-django-core-7.0.1/ai_django_core/templatetags/ai_number_tags.py
+-rw-r--r--   0        0        0      384 2022-05-19 13:07:18.132547 ai-django-core-7.0.1/ai_django_core/templatetags/ai_object_tags.py
+-rw-r--r--   0        0        0      654 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/ai_django_core/templatetags/ai_string_tags.py
+-rw-r--r--   0        0        0        0 2020-10-29 09:10:12.146622 ai-django-core-7.0.1/ai_django_core/tests/__init__.py
+-rw-r--r--   0        0        0       60 2022-06-29 09:25:01.899799 ai-django-core-7.0.1/ai_django_core/tests/errors.py
+-rw-r--r--   0        0        0     5006 2023-02-13 12:01:53.840473 ai-django-core-7.0.1/ai_django_core/tests/mixins.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.659442 ai-django-core-7.0.1/ai_django_core/tests/structure_validator/__init__.py
+-rw-r--r--   0        0        0      397 2023-03-16 14:29:23.660441 ai-django-core-7.0.1/ai_django_core/tests/structure_validator/settings.py
+-rw-r--r--   0        0        0     4633 2023-03-16 14:29:23.660441 ai-django-core-7.0.1/ai_django_core/tests/structure_validator/test_structure_validator.py
+-rw-r--r--   0        0        0      261 2020-10-29 08:14:58.246710 ai-django-core-7.0.1/ai_django_core/utils/__init__.py
+-rw-r--r--   0        0        0      127 2021-01-14 07:19:48.798830 ai-django-core-7.0.1/ai_django_core/utils/cache.py
+-rw-r--r--   0        0        0     5971 2023-03-28 10:54:55.241821 ai-django-core-7.0.1/ai_django_core/utils/date.py
+-rw-r--r--   0        0        0     1468 2022-05-19 13:07:18.137589 ai-django-core-7.0.1/ai_django_core/utils/file.py
+-rw-r--r--   0        0        0      343 2022-05-19 13:07:18.137589 ai-django-core-7.0.1/ai_django_core/utils/log_whodid.py
+-rw-r--r--   0        0        0      574 2021-01-14 07:19:48.798830 ai-django-core-7.0.1/ai_django_core/utils/math.py
+-rw-r--r--   0        0        0      935 2022-05-19 13:07:18.137589 ai-django-core-7.0.1/ai_django_core/utils/model.py
+-rw-r--r--   0        0        0     3850 2023-03-16 11:00:21.086080 ai-django-core-7.0.1/ai_django_core/utils/named_tuple.py
+-rw-r--r--   0        0        0     3694 2022-09-29 17:01:08.210953 ai-django-core-7.0.1/ai_django_core/utils/string.py
+-rw-r--r--   0        0        0        0 2021-04-20 12:33:32.484731 ai-django-core-7.0.1/ai_django_core/view_layer/__init__.py
+-rw-r--r--   0        0        0      750 2022-05-19 13:07:18.137589 ai-django-core-7.0.1/ai_django_core/view_layer/form_mixins.py
+-rw-r--r--   0        0        0      485 2022-05-19 13:07:18.142596 ai-django-core-7.0.1/ai_django_core/view_layer/formset_mixins.py
+-rw-r--r--   0        0        0     2998 2022-05-19 13:07:18.142596 ai-django-core-7.0.1/ai_django_core/view_layer/formset_view_mixin.py
+-rw-r--r--   0        0        0     1585 2023-03-28 10:54:55.241821 ai-django-core-7.0.1/ai_django_core/view_layer/htmx_mixins.py
+-rw-r--r--   0        0        0     2110 2022-06-29 09:25:01.903801 ai-django-core-7.0.1/ai_django_core/view_layer/mixins.py
+-rw-r--r--   0        0        0        0 2022-06-29 09:25:01.903801 ai-django-core-7.0.1/ai_django_core/view_layer/tests/__init__.py
+-rw-r--r--   0        0        0     4120 2022-11-18 09:21:47.406961 ai-django-core-7.0.1/ai_django_core/view_layer/tests/mixins.py
+-rw-r--r--   0        0        0     1882 2023-02-21 14:56:14.199514 ai-django-core-7.0.1/ai_django_core/view_layer/views.py
+-rw-r--r--   0        0        0      654 2020-10-29 08:14:58.247751 ai-django-core-7.0.1/docs/Makefile
+-rw-r--r--   0        0        0     2837 2023-03-16 14:29:23.662561 ai-django-core-7.0.1/docs/conf.py
+-rw-r--r--   0        0        0     6729 2021-10-18 07:37:49.515098 ai-django-core-7.0.1/docs/features/admin.md
+-rw-r--r--   0        0        0       33 2023-01-11 09:49:34.733879 ai-django-core-7.0.1/docs/features/changelog.rst
+-rw-r--r--   0        0        0     2313 2021-01-14 07:19:48.814455 ai-django-core-7.0.1/docs/features/context_manager.md
+-rw-r--r--   0        0        0      548 2021-01-14 07:19:48.814455 ai-django-core-7.0.1/docs/features/context_processors.md
+-rw-r--r--   0        0        0     7273 2021-11-18 10:19:55.448850 ai-django-core-7.0.1/docs/features/database_anonymisation.md
+-rw-r--r--   0        0        0     6807 2021-04-20 12:33:32.500344 ai-django-core-7.0.1/docs/features/djangorestframework.md
+-rw-r--r--   0        0        0     2552 2023-01-18 08:29:41.824417 ai-django-core-7.0.1/docs/features/gitlab.md
+-rw-r--r--   0        0        0     6339 2022-02-28 07:49:19.065009 ai-django-core-7.0.1/docs/features/graphql.md
+-rw-r--r--   0        0        0    10426 2022-02-28 08:13:29.331040 ai-django-core-7.0.1/docs/features/mail.md
+-rw-r--r--   0        0        0     5891 2022-11-28 15:41:36.593627 ai-django-core-7.0.1/docs/features/managers.md
+-rw-r--r--   0        0        0     5951 2022-12-19 12:58:18.633582 ai-django-core-7.0.1/docs/features/mixins.md
+-rw-r--r--   0        0        0     1551 2023-03-28 09:35:16.410380 ai-django-core-7.0.1/docs/features/models.md
+-rw-r--r--   0        0        0     4451 2022-11-28 15:41:36.594720 ai-django-core-7.0.1/docs/features/selectors.md
+-rw-r--r--   0        0        0     1045 2021-12-10 11:03:41.492786 ai-django-core-7.0.1/docs/features/sentry.md
+-rw-r--r--   0        0        0     4977 2021-11-09 07:06:36.578897 ai-django-core-7.0.1/docs/features/services.md
+-rw-r--r--   0        0        0     1502 2021-03-17 07:16:57.205815 ai-django-core-7.0.1/docs/features/setup.md
+-rw-r--r--   0        0        0    10391 2023-03-16 14:29:23.663545 ai-django-core-7.0.1/docs/features/tests.md
+-rw-r--r--   0        0        0      232 2022-06-30 10:27:42.711391 ai-django-core-7.0.1/docs/features/utils.rst
+-rw-r--r--   0        0        0      526 2021-01-14 07:19:48.814455 ai-django-core-7.0.1/docs/features/utils/cache.md
+-rw-r--r--   0        0        0     7404 2022-12-01 13:50:38.529789 ai-django-core-7.0.1/docs/features/utils/date.md
+-rw-r--r--   0        0        0      737 2021-01-14 07:19:48.814455 ai-django-core-7.0.1/docs/features/utils/math.md
+-rw-r--r--   0        0        0     1100 2021-01-14 07:19:48.814455 ai-django-core-7.0.1/docs/features/utils/model.md
+-rw-r--r--   0        0        0     2405 2021-11-09 07:06:36.594530 ai-django-core-7.0.1/docs/features/utils/named_tuple.md
+-rw-r--r--   0        0        0     5847 2021-11-09 07:06:36.594530 ai-django-core-7.0.1/docs/features/utils/string.md
+-rw-r--r--   0        0        0    15052 2023-02-21 14:56:14.200514 ai-django-core-7.0.1/docs/features/view-layer.md
+-rw-r--r--   0        0        0     1152 2022-11-28 15:41:36.595725 ai-django-core-7.0.1/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2020-10-29 08:14:58.263559 ai-django-core-7.0.1/docs/make.bat
+-rw-r--r--   0        0        0      677 2022-05-19 13:07:18.142596 ai-django-core-7.0.1/manage.py
+-rw-r--r--   0        0        0     3912 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/pyproject.toml
+-rw-r--r--   0        0        0       56 2020-10-30 08:58:27.573230 ai-django-core-7.0.1/pytest.ini
+-rw-r--r--   0        0        0      184 2022-02-28 08:20:10.689851 ai-django-core-7.0.1/scripts/publish_and_update_mirror.ps1
+-rw-r--r--   0        0        0      302 2023-03-16 14:36:30.853296 ai-django-core-7.0.1/scripts/update-mirror.ps1
+-rw-r--r--   0        0        0     1703 2022-09-29 17:01:08.221675 ai-django-core-7.0.1/settings.py
+-rw-r--r--   0        0        0       69 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/setup.cfg
+-rw-r--r--   0        0        0        0 2020-10-30 08:58:27.574229 ai-django-core-7.0.1/testapp/__init__.py
+-rw-r--r--   0        0        0        0 2021-03-16 07:21:28.693546 ai-django-core-7.0.1/testapp/api/__init__.py
+-rw-r--r--   0        0        0      287 2022-05-19 13:07:18.142596 ai-django-core-7.0.1/testapp/api/serializers.py
+-rw-r--r--   0        0        0      257 2022-05-19 13:07:18.142596 ai-django-core-7.0.1/testapp/api/urls.py
+-rw-r--r--   0        0        0      524 2021-03-16 07:21:28.693546 ai-django-core-7.0.1/testapp/api/views.py
+-rw-r--r--   0        0        0      219 2023-03-16 14:29:23.663545 ai-django-core-7.0.1/testapp/forms.py
+-rw-r--r--   0        0        0       97 2022-11-28 15:41:36.595725 ai-django-core-7.0.1/testapp/managers.py
+-rw-r--r--   0        0        0      829 2023-02-06 12:03:54.198766 ai-django-core-7.0.1/testapp/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2529 2023-02-06 12:03:54.242881 ai-django-core-7.0.1/testapp/migrations/0002_auto_210407.py
+-rw-r--r--   0        0        0     2194 2022-05-24 06:31:55.228545 ai-django-core-7.0.1/testapp/migrations/0003_modelwithfktoself.py
+-rw-r--r--   0        0        0     1866 2023-02-06 12:03:54.226798 ai-django-core-7.0.1/testapp/migrations/0004_auto_20210511_1343.py
+-rw-r--r--   0        0        0      613 2023-02-06 12:03:54.191159 ai-django-core-7.0.1/testapp/migrations/0005_modelwithcleanmixin.py
+-rw-r--r--   0        0        0      680 2023-02-06 12:03:54.198766 ai-django-core-7.0.1/testapp/migrations/0006_modelwithselector.py
+-rw-r--r--   0        0        0      692 2023-02-06 12:03:54.198766 ai-django-core-7.0.1/testapp/migrations/0007_modelwithsavewithoutsignals.py
+-rw-r--r--   0        0        0        0 2020-10-30 08:58:27.575702 ai-django-core-7.0.1/testapp/migrations/__init__.py
+-rw-r--r--   0        0        0     3359 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/testapp/models.py
+-rw-r--r--   0        0        0      161 2022-11-28 15:41:36.598713 ai-django-core-7.0.1/testapp/selectors.py
+-rw-r--r--   0        0        0     1390 2022-09-29 17:01:08.223215 ai-django-core-7.0.1/testapp/templates/403.html
+-rw-r--r--   0        0        0      145 2021-03-04 09:15:39.283083 ai-django-core-7.0.1/testapp/templates/test_email.html
+-rw-r--r--   0        0        0      148 2021-03-04 09:15:39.283083 ai-django-core-7.0.1/testapp/templates/test_email.txt
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.665545 ai-django-core-7.0.1/testapp/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.665545 ai-django-core-7.0.1/testapp/tests/missing_init/test_ok.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.665545 ai-django-core-7.0.1/testapp/tests/subdirectory/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.666607 ai-django-core-7.0.1/testapp/tests/subdirectory/missing_test_prefix.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.666607 ai-django-core-7.0.1/testapp/tests/subdirectory/test_ok.py
+-rw-r--r--   0        0        0      382 2022-05-24 06:31:55.232545 ai-django-core-7.0.1/testapp/urls.py
+-rw-r--r--   0        0        0      490 2022-09-29 17:18:59.613421 ai-django-core-7.0.1/testapp/views.py
+-rw-r--r--   0        0        0        0 2020-10-30 08:58:27.576702 ai-django-core-7.0.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-08 14:39:10.030331 ai-django-core-7.0.1/tests/admin/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-08 14:39:10.030331 ai-django-core-7.0.1/tests/admin/model_admin_mixins/__init__.py
+-rw-r--r--   0        0        0     2605 2023-03-16 14:29:23.667647 ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py
+-rw-r--r--   0        0        0     1898 2022-05-24 06:31:55.235544 ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py
+-rw-r--r--   0        0        0     1681 2022-05-24 06:31:55.236545 ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py
+-rw-r--r--   0        0        0     1182 2022-05-24 06:31:55.237545 ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py
+-rw-r--r--   0        0        0     3790 2022-09-29 17:01:08.225217 ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py
+-rw-r--r--   0        0        0     1489 2022-05-24 06:31:55.239544 ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_fetch_object_mixin.py
+-rw-r--r--   0        0        0     1907 2022-05-24 06:31:55.240547 ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.667647 ai-django-core-7.0.1/tests/ambient_toolbox/__init__.py
+-rw-r--r--   0        0        0     7498 2023-04-28 13:00:07.370054 ai-django-core-7.0.1/tests/ambient_toolbox/test_test_structure_validator.py
+-rw-r--r--   0        0        0        0 2021-04-20 12:33:32.500344 ai-django-core-7.0.1/tests/drf/__init__.py
+-rw-r--r--   0        0        0     2578 2022-05-24 06:31:55.241566 ai-django-core-7.0.1/tests/drf/test_fields.py
+-rw-r--r--   0        0        0       28 2021-04-20 12:33:32.500344 ai-django-core-7.0.1/tests/files/testfile.txt
+-rw-r--r--   0        0        0        0 2022-05-24 06:31:55.242545 ai-django-core-7.0.1/tests/mixins/__init__.py
+-rw-r--r--   0        0        0      364 2022-05-24 06:31:55.243544 ai-django-core-7.0.1/tests/mixins/validation.py
+-rw-r--r--   0        0        0        0 2022-11-28 15:41:36.598713 ai-django-core-7.0.1/tests/selectors/__init__.py
+-rw-r--r--   0        0        0      498 2022-11-28 15:41:36.599713 ai-django-core-7.0.1/tests/selectors/test_base.py
+-rw-r--r--   0        0        0     1630 2022-11-28 15:41:36.599713 ai-django-core-7.0.1/tests/selectors/test_permission.py
+-rw-r--r--   0        0        0      552 2022-05-24 06:31:55.244544 ai-django-core-7.0.1/tests/test_admin_forms.py
+-rw-r--r--   0        0        0     1610 2022-05-24 06:31:55.245548 ai-django-core-7.0.1/tests/test_admin_inlines.py
+-rw-r--r--   0        0        0     2649 2022-05-24 06:31:55.247546 ai-django-core-7.0.1/tests/test_admin_model_admins_classes.py
+-rw-r--r--   0        0        0     2886 2022-05-24 06:31:55.248546 ai-django-core-7.0.1/tests/test_admin_view_mixins.py
+-rw-r--r--   0        0        0     2217 2022-05-24 06:31:55.249546 ai-django-core-7.0.1/tests/test_context_manager.py
+-rw-r--r--   0        0        0     9342 2023-01-11 09:40:21.960817 ai-django-core-7.0.1/tests/test_email_test_service.py
+-rw-r--r--   0        0        0      821 2020-10-30 08:58:27.625804 ai-django-core-7.0.1/tests/test_log_whodid.py
+-rw-r--r--   0        0        0    15502 2022-05-24 06:31:55.250546 ai-django-core-7.0.1/tests/test_mail_services.py
+-rw-r--r--   0        0        0     1169 2022-05-24 06:31:55.251544 ai-django-core-7.0.1/tests/test_managers.py
+-rw-r--r--   0        0        0     1627 2022-05-24 06:31:55.252553 ai-django-core-7.0.1/tests/test_math.py
+-rw-r--r--   0        0        0     2592 2022-05-19 13:07:18.157715 ai-django-core-7.0.1/tests/test_middleware.py
+-rw-r--r--   0        0        0     1200 2022-12-19 12:58:18.636566 ai-django-core-7.0.1/tests/test_mixins_models.py
+-rw-r--r--   0        0        0     1669 2023-03-28 09:35:16.411383 ai-django-core-7.0.1/tests/test_models.py
+-rw-r--r--   0        0        0     1779 2022-05-24 06:31:55.254447 ai-django-core-7.0.1/tests/test_rest_api_mixins.py
+-rw-r--r--   0        0        0      663 2022-05-24 06:31:55.255429 ai-django-core-7.0.1/tests/test_scrubbing_service.py
+-rw-r--r--   0        0        0     1196 2022-05-24 06:31:55.256430 ai-django-core-7.0.1/tests/test_sentry_helper.py
+-rw-r--r--   0        0        0      288 2022-05-24 06:31:55.257429 ai-django-core-7.0.1/tests/test_utils_cache.py
+-rw-r--r--   0        0        0    12740 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/tests/test_utils_date.py
+-rw-r--r--   0        0        0     1593 2022-05-24 06:31:55.259430 ai-django-core-7.0.1/tests/test_utils_file.py
+-rw-r--r--   0        0        0      932 2022-05-24 06:31:55.260430 ai-django-core-7.0.1/tests/test_utils_model.py
+-rw-r--r--   0        0        0     3806 2022-05-24 06:31:55.261429 ai-django-core-7.0.1/tests/test_utils_named_tuple.py
+-rw-r--r--   0        0        0     5342 2022-05-24 06:31:55.262430 ai-django-core-7.0.1/tests/test_utils_string.py
+-rw-r--r--   0        0        0        0 2021-04-08 14:39:10.030331 ai-django-core-7.0.1/tests/tests/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-08 14:39:10.045967 ai-django-core-7.0.1/tests/tests/mixins/__init__.py
+-rw-r--r--   0        0        0      371 2022-10-12 09:20:31.364313 ai-django-core-7.0.1/tests/tests/mixins/models.py
+-rw-r--r--   0        0        0      796 2023-02-13 15:49:17.040360 ai-django-core-7.0.1/tests/tests/mixins/test_django_message_framework.py
+-rw-r--r--   0        0        0     2482 2022-05-24 06:31:55.263431 ai-django-core-7.0.1/tests/tests/mixins/test_request_provider_mixin.py
+-rw-r--r--   0        0        0     2055 2022-05-24 06:31:55.264429 ai-django-core-7.0.1/tests/tests/test_mail_backends.py
+-rw-r--r--   0        0        0        0 2021-04-20 12:33:32.500344 ai-django-core-7.0.1/tests/view_layer/__init__.py
+-rw-r--r--   0        0        0     1890 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/tests/view_layer/test_formset_mixins.py
+-rw-r--r--   0        0        0     1562 2023-02-21 14:56:14.201551 ai-django-core-7.0.1/tests/view_layer/test_htmx_response_mixin.py
+-rw-r--r--   0        0        0     3369 2022-06-29 11:55:51.396586 ai-django-core-7.0.1/tests/view_layer/test_meta_mixins.py
+-rw-r--r--   0        0        0     1323 2022-09-29 17:18:59.613421 ai-django-core-7.0.1/tests/view_layer/test_views.py
+-rw-r--r--   0        0        0     7044 1970-01-01 00:00:00.000000 ai-django-core-7.0.1/PKG-INFO
```

### Comparing `ai-django-core-7.0.0/.github/workflows/ci.yml` & `ai-django-core-7.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/.gitlab-ci.yml` & `ai-django-core-7.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/.pre-commit-config.yaml` & `ai-django-core-7.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/CHANGES.md` & `ai-django-core-7.0.1/CHANGES.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,475 +1,479 @@
-# Changelog
-
-* **7.0.0** (2023-03-28)
-  * *Breaking change:* Dropped Python 3.7 support due to end of lifetime
-  * Added `ALWAYS_UPDATE_FIELDS` flag to `CommonInfo` model
-  * Added `ruff` linter and replaced `flake8` and `isort` with it
-
-* **6.12.0** (2023-03-16)
-  * Added `validate_test_structure` management command for validating project test structure
-  * Fixed syntax error in docs
-  * Fixed typo in docstring of `concat` method
-  * Improved code in test app
-
-* **6.11.0** (2023-02-19)
-  * Added `HtmxResponseMixin` for Django views
-  * Added missing `object` class attribute to `ToggleView`
-  * Updated local lint, build and test suite to Python 3.11
-  * Updated readme file for contribution
-
-* **6.10.1** (2023-02-13)
-  * Updated bug in documentation
-
-* **6.10.0** (2023-02-13)
-  * Added test mixin `DjangoMessagingFrameworkTestMixin`
-  * Added python 3.11 to test matrix and supported versions
-
-* **6.9.2** (2023-02-06)
-  * Updated `pre-commit` packages
-
-* **6.9.1** (2023-01-25)
-  * Set version border for dependency "bleach" because of breaking changes
-
-* **6.9.0** (2023-01-18)
-  * Added "GITLAB_CI_DISABLE_COVERAGE" flag to coverage script for Gitlab pipeline
-  * Fixed typo in the docs
-
-* **6.8.4** (2023-01-11)
-  * Moved changelog to "CHANGES.md" to make Dependabot understand/find it
-
-* **6.8.3** (2023-01-11)
-  * Fixed bug with filtering in EmailTestService for subject passing a gettext_lazy object (second occurrence)
-
-* **6.8.2** (2023-01-11)
-  * Fixed bug with filtering in EmailTestService for subject passing a gettext_lazy object
-
-* **6.8.1** (2022-12-20)
-  * Fixed broken init file
-
-* **6.8.0** (2022-12-19)
-  * Added `SaveWithoutSignalsMixin` model mixin
-
-* **6.7.0** (2022-11-25)
-  * Added `Selector` base class
-  * Added `AbstractUserSpecificSelectorMixin` and `GloballyVisibleSelector` helpers for selector pattern
-  * Added documentation for new selector pattern
-  * Added `django-upgrade` to linting
-  * Added date helper `get_first_and_last_of_month`
-  * Updated linting tools `black` & `pyupgrade`
-  * Added `pyupgrade` and `django-upgrade` to pipeline
-
-* **6.6.3** (2022-11-18)
-  * Fixed `BaseViewPermissionTestMixin` to work with custom user models
-
-* **6.6.2** (2022-10-12)
-  * Updated documentation of mixin `PermissionModelMixin` in regard to a caveat with default permissions
-
-* **6.6.1** (2022-10-12)
-  * Bugfix in documentation of mixin `PermissionModelMixin`
-
-* **6.6.0** (2022-10-12)
-  * Added model mixin `PermissionModelMixin` to provide a neat way of handling non-(database)-model-related permissions
-  * Improved mixin documentation
-  * Updated GitHub Actions
-
-* **6.5.0** (2022-09-29)
-  * Added view mixin `UserInFormKwargsMixin` to pass the user to a form in a `FormView`, `CreateView` or `UpdateView`
-
-* **6.4.0** (2022-09-29)
-  * Models inheriting from `CommonInfo` will automatically save the four CommonInfo fields in addition to the fields
-    selected when using `update_fields` in the models save method.
-
-* **6.3.2** (2022-09-29)
-  * Updated gitlab-ci for showing tests in MR
-
-* **6.3.1** (2022-09-19)
-  * Updated GitHub test matrix OS
-
-* **6.3.0** (2022-09-19)
-  * Integrated `flake8-bugbear` and `pyupgrade` including required code adjustments
-  * Improved security vulnerability scanning
-  * Updated local build and test suite to Python 3.10
-  * Added `flake8-bugbear` to Quality Assurance measures
-  * Added `pyupgrade` to Quality Assurance measures
-
-* **6.2.3** (2022-08-15)
-  * Fixed some translations
-
-* **6.2.2** (2022-08-12)
-  * Added Django 4.1 to test matrix and compatible versions
-
-* **6.2.1** (2022-08-12)
-  * Improved detecting of permission mismatches in view test mixin `BaseViewPermissionTestMixin`
-
-* **6.2.0** (2022-07-13)
-  * Added test case for `BaseViewPermissionTestMixin` to ensure that defined permissions exist in the database
-
-* **6.1.3** (2022-06-30)
-  * Clarified docs for `GloballyVisibleQuerySet`
-
-* **6.1.2** (2022-06-30)
-  * Extended docs for `BaseViewPermissionTestMixin` with limitation when using a caching wrapper
-
-* **6.1.1** (2022-06-29)
-  * Fixed unittest for django<3.2
-
-* **6.1.0** (2022-06-29)
-  * Added `DjangoPermissionRequiredMixin` for Django views and supporting test mixin `BaseViewPermissionTestMixin`
-  * Increased minimal required bugfix version for Django 2.2
-  * Updated Readme file
-
-* **6.0.0** (2022-05-19)
-  * *Breaking change:* Removed `ffmpeg` helper methods `generate_video_thumbnail()` and `get_video_length()`
-  * Added `CleanOnSaveMixin`
-  * black and isort linting integrated
-  * Added pre-commit hooks for linting
-
-* **5.14.1** (2022-04-06)
-  * Dropped support for deprecated Python 3.6
-
-* **5.14.0** (2022-04-06)
-  * `EmailTestService` can now filter for subjects using regular expressions
-
-* **5.13.7** (2022-03-14)
-  * Fixed typo in coverage validator
-
-* **5.13.6** (2022-03-11)
-  * Improved console logging for coverage validator
-
-* **5.13.5** (2022-02-28)
-  * Improved motivation in class-based email docs
-
-* **5.13.4** (2022-02-28)
-  * Added Script for updating mirror
-  * Fixed typo in documentation
-
-* **5.13.3** (2022-02-23)
-  * Added GitHub action matrix for running tests on django/python combinations
-  * Updated Ambient email addresses to new domain
-  * Removed django <4.0 restriction
-  * Fixed tests for django 4.0
-
-* **5.13.2** (2022-02-21)
-  * `CurrentUserMiddleware` bugfix, cleaning up user variable for single-threaded tests after request processing
-  * Fixed version typo in changelog
-
-* **5.13.1** (2022-02-04)
-  * GraphQL docs bugfix
-
-* **5.13.0** (2022-02-03)
-  * Added a view which allows logging errors to Sentry normally while using Graphene.
-
-* **5.12.1** (2022-01-31)
-  * Fixed bug in Gitlab code coverage compare service documentation
-
-* **5.12.0** (2022-01-28)
-  * Added Gitlab code coverage compare service `CoverageService` with documentation
-
-* **5.11.1** (2022-01-24)
-  * Added docs for `ToggleView`
-  * Fixed some typos in `Readme.md` and `changelog.md`
-
-* **5.11.0** (2022-01-24)
-  * Added generic `ToggleView`
-  * Updated some docstrings in `formset_view_mixin`
-
-* **5.10.1** (2021-12-10)
-  * Added docs about GDPR-compliant use of sentry with user data
-  * Fixed some versions to make Sphinx build work again
-
-* **5.10.0** (2021-12-10)
-  * Added helper method for sentry to GDPR-compliant remove sensitive user data from event
-  * Updated type hints in `BaseEmailServiceFactory` init method
-  * Improved docs for method `get_start_and_end_date_from_calendar_week`
-
-* **5.9.1** (2021-11-25)
-  * Fixed typo in custom scrubber class logging
-  * Rewrote permission manager docs and added better best practice
-  * Update in email testing docs
-
-* **5.9.0** (2021-11-18)
-    * Added default truncate of django session table to `AbstractScrubbingService`
-
-* **5.8.0** (2021-11-11)
-    * Added `url` parameter to `RequestProviderMixin`
-
-* **5.7.4** (2021-11-08)
-    * Added missing documentation about semantic database anonymisation
-    * Added missing documentation about string utils
-    * Added missing documentation about `get_namedtuple_choices()` helper
-    * Added missing documentation about `CrispyLayoutFormMixin`
-    * Added missing documentation about `ClassBasedViewTestMixin`
-
-* **5.7.3** (2021-10-22)
-    * Added missing documentation about email testing
-    * Updated Readme file
-
-* **5.7.2** (2021-10-21)
-    * Fixed `flit` configuration
-
-* **5.7.1** (2021-10-21)
-    * Setup `flit` for release management
-
-* **5.7.0** (2021-10-15)
-    * Added admin mixin `DeactivatableChangeViewAdminMixin`
-    * Added `response` parameter to testing middlewares
-
-* **5.6.0** (2021-09-01)
-    * Extracted embedded form valid logic to separate method with super call in `_FormsetMixin`
-    * Added documentation about `FormsetCreateViewMixin` and `FormsetUpdateViewMixin`
-
-* **5.5.2** (2021-08-24)
-    * Added documentation about `BleacherMixin`
-
-* **5.5.1** (2021-08-24)
-    * Added explicit declaration of bleacher field list attribute `BLEACH_FIELD_LIST` in `BleacherMixin`
-
-* **5.5.0** (2021-08-02)
-    * Added validation for user object in `RequestProviderMixin`
-    * Added link to changelog in setup.py
-    * Moved minimum django version to 2.2
-
-* **5.4.0** (2021-06-28)
-    * Added `__len__` and `__iter__` to EmailTestService
-    * EmailTestService uses EmailTestServiceMail instances, which wrap the underlying Django mail objects, and provide
-      additional assertion functions
-
-* **5.3.0** (2021-06-16)
-    * Added `method` kwarg to `RequestProviderMixin.get_request()`
-
-* **5.2.2** (2021-05-27)
-    * Fixed a bug in `BaseEmailService` where txt part was rendered sometimes with weird line breaks
-    * Added Bugtracker link to `setup.py`
-
-* **5.2.1** (2021-05-12)
-    * Translation files were missing in wheel
-    * Bugfix in docs
-
-* **5.2.0** (2021-05-11)
-    * Changed all translatable texts to English base version
-    * Added German translation file for current translatable
-    * Updated RequestProviderMixin.get_request() type hinting
-    * Added documentation for database anonymisation / django-scrubber wrapper
-
-* **5.1.1** (2021-04-21)
-    * Extended email attachment functionality to be able to define filename and mimetype
-
-* **5.1.0** (2021-04-20)
-    * *Breaking change:* Fixed typo in `WhitelistEmailBackend.whitify_mail_adresses` method name. Method is now
-      called `whitify_mail_addresses`
-    * Moved assignment of `WhitelistEmailBackend` settings var to static methods to be able to overwrite them if needed
-    * Added documentation about `WhitelistEmailBackend`
-    * Added some type hinting to `WhitelistEmailBackend`
-    * Added formset mixin `CountChildrenFormsetMixin`
-    * Added djangorestframework field `RecursiveField`
-    * Added `get_attachments()` method to `BaseEmailService` and extended constructor to accept a
-      variable `attachment_list`
-
-* **5.0.0** (2021-03-26)
-    * *Breaking change:* Moved `ReadOnlyAdmin` and `EditableOnlyAdmin` to package `model_admins.classes`
-      and `ReadOnlyTabularInline` to package `model_admins.inlines` to enable better structuring of new admin components
-    * Fixed some inconsistencies within `ReadOnlyAdmin`, `EditableOnlyAdmin` and `ReadOnlyTabularInline` classes
-    * Added `admin.views` package containing a base crispy form, and a mixin to turn any regular django view into a nice
-      and cozy django admin view
-    * Added an abundance of `model_admins.mixins`: `AdminCreateFormMixin`, `AdminNoInlinesForCreateMixin`
-      ,`AdminRequestInFormMixin`, `FetchParentObjectInlineMixin`, `FetchObjectMixin`, `CommonInfoAdminMixin`
-    * Added `RequestProviderMixin` to easily create a dummy request in unittests
-    * Added support for django 3.2 and dropped support for 2.0, 2.1 and 3.0
-    * Added support for Python 3.9 and dropped support for 3.5
-    * Updated test python version to 3.9
-
-* **4.2.1** (2021-03-17)
-    * Added some links to setup.py for pypi
-    * Added some documentation for setting up the toolbox
-
-* **4.2.0** (2021-03-12)
-    * Added ``GloballyVisibleQuerySet`` including tests and documentation
-    * Added ``BaseViewSetTestMixin`` for the djangorestframework plugin
-    * Fixed some typos in the documentation
-
-* **4.1.2** (2021-03-05)
-    * Added kwargs parameter to init-method of `BaseEmailServiceFactory`
-
-* **4.1.1** (2021-03-04)
-    * Fixed a bug in the documentation
-
-* **4.1.0** (2021-02-25)
-    * Added class `BaseEmailService` for easier email creation and factory `BaseEmailServiceFactory`
-      for multiple (mostly personalised) emails
-    * Added `html2text` as a dependency to be able to automatically process the text part of an email from the html
-      template
-
-* **4.0.2** (2021-02-24)
-    * Fixed a bug in ``EmailTestService.assert_body_contains()`` method to make it work for emails NOT having an HTML
-      part
-
-* **4.0.1** (2021-01-29)
-    * Optimised code of function `test_get_value_from_tuple_by_key_found()`
-    * Added unittests for named tuple functions
-
-* **4.0.0** (2020-11-10)
-    * *Breaking change:* Moved view mixin ``RequestInFormKwargsMixin`` from ``mixin.forms`` to proper place
-      ``mixin.views``
-    * *Breaking change:* Removed string helper function ``restore_windows1252controls()``, ``number_to_text()`` and
-      ``replace_link_pattern()``
-    * *Breaking change:* Removed choice converter function ``get_name_by_value()`` in favour
-      of ``get_value_from_tuple_by_key()``
-    * *Breaking change:* Removed date converter function ``get_seconds()`` because Python 3.6 already provides
-      a `total_seconds()` method
-    * *Breaking change:* Removed date converter function ``get_current_datetime()`` because django already provides
-      the `timezone.now()` method
-    * *Breaking change:* Removed date converter function ``diff_month()`` in favour of ``date_month_delta()``
-    * *Breaking change:* Merged ``converter`` package in ``utils`` package
-    * *Breaking change:* Moved view-layer-based helpers to extra requirement ``view-layer``: `_FormsetMixin`,
-      `FormsetUpdateViewMixin`, `FormsetCreateViewMixin`, `CrispyLayoutFormMixin`, `CustomPermissionMixin`
-      , `RequestInFormKwargsMixin`
-    * Simplified code of function ``float_to_string()``
-    * Added type hinting to lots of helper functions
-    * Updated and restructured documentation
-    * Added security check for dependencies in local pipeline
-    * Removed some old python 2.7 syntax
-
-* **3.5.2** (2021-01-07)
-    * Bugfix with args and kwargs in ``ReadOnlyTabularInline``
-
-* **3.5.1** (2020-11-19)
-    * Bugfix with args and kwargs in ``ClassBasedViewTestMixin``
-
-* **3.5.0** (2020-11-10)
-    * Merged package ``graphene-django-ai`` into this package and enabled graphql-specific installation
-      with `pip install ai_django_core[graphql]`
-    * Added some files for readthedocs.io and updated Readme
-
-* **3.4.0** (2020-10-30)
-    * Moved tests out of package scope
-    * Updated test python version to 3.8
-    * Added tests for context manager ``TempDisconnectSignal`` with test setup
-
-* **3.3.0** (2020-10-30)
-    * Merged package ``ai-drf-core`` into this package and enabled djangorestframework-specific installation
-      with `pip install ai_django_core[drf]`
-    * Added ``BaseModelSerializer`` and ``CommonInfoSerializer``
-    * Incremented dependencies django and bleach to previous versions latest bugfix release
-
-* **3.2.0** (2020-10-16)
-    * Added ``AbstractPermissionMixin``, ``AbstractUserSpecificQuerySet`` and ``AbstractUserSpecificManager`` abstract
-      managers
-    * Removed deprecated `antivir` package
-    * Added Sphinx documentation setup to package
-
-* **3.1.0** (2020-10-14)
-    * Added context manager ``TempDisconnectSignal`` to nicely disable model signals temporarily
-    * Moved dev dependencies to ``extras_require`` in the setup file
-
-* **3.0.2** (2020-10-15)
-    * Imports all utils into the modules scope
-    * Re-translated some docstrings into English
-    * Added tests for the `log_whodid` util function
-
-* **3.0.1** (2020-10-12)
-    * Added missing ``__init__.py`` file to package mail.services
-
-* **3.0.0** (2020-09-09)
-    * *Breaking change:*  Renamed package from `ai` to `ai_django_core` to clarify dependencies for usages
-    * Finished code linting
-    * Removed unused imports in antivirus util package
-
-* **2.3.0** (2020-08-07)
-    * Changed `ugettext_lazy` to `gettext_lazy` to tackle django 4.0 deprecation warnings
-
-* **2.2.1** (2020-07-01)
-    * Removed misleading inheritance of mixin `ClassBasedViewTestMixin` from `TestCase`
-
-* **2.2.0** (2020-07-01)
-    * Added response class `CustomPermissionMixin`
-
-* **2.1.2** (2020-04-30)
-    * Extended pypi documentation with classifiers
-
-* **2.1.1** (2020-04-24)
-    * Refactors open calls to use context managers
-    * Refactors the test setup
-    * Configures coverage
-    * Adds a coverage report to the CI
-
-* **2.1.0** (2020-04-20)
-    * Removed password generator method `generate_password`
-    * Renamed math method `round_up_to_decimal` to `round_up_decimal`
-    * Added math method `round_to_decimal`
-    * Updated metadata in setup.cfg
-
-* **2.0.0** (2020-04-09)
-    * Dropped Python 2.x support
-    * Removed explicit dependency to package `mock` and using implicit one via unittest
-    * Improved linting
-
-* **1.2.14** (2020-04-06)
-    * Fixed a bug with session setup in `ClassBasedViewTestMixin`
-
-* **1.2.13** (2020-04-02)
-    * Added ``DELETE`` method for testing mixing `ClassBasedViewTestMixin`
-
-* **1.2.12** (2020-02-14)
-    * Added CBV testing mixing `ClassBasedViewTestMixin`
-
-* **1.2.11** (2020-01-28)
-    * Bugfix in documentation
-
-* **1.2.10** (2020-01-28)
-    * Improved documentation
-
-* **1.2.9** (2020-01-02)
-    * Extended and improved class `AbstractScrubbingService`
-
-* **1.2.8** (2019-12-13)
-    * Added custom scrubber class `AbstractScrubbingService` to provide a helper for adding custom scrubbing logic for
-      data anonymisation
-
-* **1.2.7** (2019-07-11)
-    * Added email testing class `EmailTestService` to provide a wrapper for better email unittests
-
-* **1.2.6** (2019-07-02)
-    * Added helper class `tz_today()` to provide an easy getter for a timezone-aware today
-
-* **1.2.5** (2019-06-25)
-    * Added helper class `DateHelper` to provide constants to use in django's ORM lookup `__week_day`
-
-* **1.2.4** (2019-05-20)
-    * More refactoring on `CurrentUserMiddleware` to make it easier to override internal functions
-
-* **1.2.3** (2019-05-20)
-    * Moved `get_current_user` function inside `CurrentUserMiddleware` as a static method to enable devs to override it
-
-* **1.2.2** (2019-04-05)
-    * Updated deployment documentation
-    * Added markdown support to Readme file
-
-* **1.2.1** (2019-03-25)
-    * Fixed bug causing `CommonInfo` middleware to not set `lastmodified_by` on object creation
-
-* **1.2.0** (2019-03-19)
-    * Added `CommonInfo` middleware
-
-* **1.1.8**
-    * Readonly admin classes
-    * Date util functions
-    * Clear cache helper
-
-* **1.1.7**
-    * Settings for whitelist email services added
-    * Formset mixins added
-
-* **1.1.6**
-    * Modifications to antivirus field
-
-* **1.1.5**
-    * Updated setup.py with newer information
-
-* **1.1.4**
-    * Bleacher mixin bugfix
-
-* **1.1.3**
-    * Bleacher mixin added
-
-* **< 1.1.3**
-    * Ancient history :)
+# Changelog
+
+* **7.0.1** (2023-05-04)
+  * **This package was superseded by** [ambient-toolbox](https://pypi.org/project/ambient-toolbox/). Please install the successor package.
+
+* **7.0.0** (2023-03-28)
+  * *Breaking change:* Dropped Python 3.7 support due to end of lifetime
+  * Added `ALWAYS_UPDATE_FIELDS` flag to `CommonInfo` model
+  * Added `ruff` linter and replaced `flake8` and `isort` with it
+  * Excluded not officially supported Python versions for certain Django releases for test matrix
+
+* **6.12.0** (2023-03-16)
+  * Added `validate_test_structure` management command for validating project test structure
+  * Fixed syntax error in docs
+  * Fixed typo in docstring of `concat` method
+  * Improved code in test app
+
+* **6.11.0** (2023-02-19)
+  * Added `HtmxResponseMixin` for Django views
+  * Added missing `object` class attribute to `ToggleView`
+  * Updated local lint, build and test suite to Python 3.11
+  * Updated readme file for contribution
+
+* **6.10.1** (2023-02-13)
+  * Updated bug in documentation
+
+* **6.10.0** (2023-02-13)
+  * Added test mixin `DjangoMessagingFrameworkTestMixin`
+  * Added python 3.11 to test matrix and supported versions
+
+* **6.9.2** (2023-02-06)
+  * Updated `pre-commit` packages
+
+* **6.9.1** (2023-01-25)
+  * Set version border for dependency "bleach" because of breaking changes
+
+* **6.9.0** (2023-01-18)
+  * Added "GITLAB_CI_DISABLE_COVERAGE" flag to coverage script for Gitlab pipeline
+  * Fixed typo in the docs
+
+* **6.8.4** (2023-01-11)
+  * Moved changelog to "CHANGES.md" to make Dependabot understand/find it
+
+* **6.8.3** (2023-01-11)
+  * Fixed bug with filtering in EmailTestService for subject passing a gettext_lazy object (second occurrence)
+
+* **6.8.2** (2023-01-11)
+  * Fixed bug with filtering in EmailTestService for subject passing a gettext_lazy object
+
+* **6.8.1** (2022-12-20)
+  * Fixed broken init file
+
+* **6.8.0** (2022-12-19)
+  * Added `SaveWithoutSignalsMixin` model mixin
+
+* **6.7.0** (2022-11-25)
+  * Added `Selector` base class
+  * Added `AbstractUserSpecificSelectorMixin` and `GloballyVisibleSelector` helpers for selector pattern
+  * Added documentation for new selector pattern
+  * Added `django-upgrade` to linting
+  * Added date helper `get_first_and_last_of_month`
+  * Updated linting tools `black` & `pyupgrade`
+  * Added `pyupgrade` and `django-upgrade` to pipeline
+
+* **6.6.3** (2022-11-18)
+  * Fixed `BaseViewPermissionTestMixin` to work with custom user models
+
+* **6.6.2** (2022-10-12)
+  * Updated documentation of mixin `PermissionModelMixin` in regard to a caveat with default permissions
+
+* **6.6.1** (2022-10-12)
+  * Bugfix in documentation of mixin `PermissionModelMixin`
+
+* **6.6.0** (2022-10-12)
+  * Added model mixin `PermissionModelMixin` to provide a neat way of handling non-(database)-model-related permissions
+  * Improved mixin documentation
+  * Updated GitHub Actions
+
+* **6.5.0** (2022-09-29)
+  * Added view mixin `UserInFormKwargsMixin` to pass the user to a form in a `FormView`, `CreateView` or `UpdateView`
+
+* **6.4.0** (2022-09-29)
+  * Models inheriting from `CommonInfo` will automatically save the four CommonInfo fields in addition to the fields
+    selected when using `update_fields` in the models save method.
+
+* **6.3.2** (2022-09-29)
+  * Updated gitlab-ci for showing tests in MR
+
+* **6.3.1** (2022-09-19)
+  * Updated GitHub test matrix OS
+
+* **6.3.0** (2022-09-19)
+  * Integrated `flake8-bugbear` and `pyupgrade` including required code adjustments
+  * Improved security vulnerability scanning
+  * Updated local build and test suite to Python 3.10
+  * Added `flake8-bugbear` to Quality Assurance measures
+  * Added `pyupgrade` to Quality Assurance measures
+
+* **6.2.3** (2022-08-15)
+  * Fixed some translations
+
+* **6.2.2** (2022-08-12)
+  * Added Django 4.1 to test matrix and compatible versions
+
+* **6.2.1** (2022-08-12)
+  * Improved detecting of permission mismatches in view test mixin `BaseViewPermissionTestMixin`
+
+* **6.2.0** (2022-07-13)
+  * Added test case for `BaseViewPermissionTestMixin` to ensure that defined permissions exist in the database
+
+* **6.1.3** (2022-06-30)
+  * Clarified docs for `GloballyVisibleQuerySet`
+
+* **6.1.2** (2022-06-30)
+  * Extended docs for `BaseViewPermissionTestMixin` with limitation when using a caching wrapper
+
+* **6.1.1** (2022-06-29)
+  * Fixed unittest for django<3.2
+
+* **6.1.0** (2022-06-29)
+  * Added `DjangoPermissionRequiredMixin` for Django views and supporting test mixin `BaseViewPermissionTestMixin`
+  * Increased minimal required bugfix version for Django 2.2
+  * Updated Readme file
+
+* **6.0.0** (2022-05-19)
+  * *Breaking change:* Removed `ffmpeg` helper methods `generate_video_thumbnail()` and `get_video_length()`
+  * Added `CleanOnSaveMixin`
+  * black and isort linting integrated
+  * Added pre-commit hooks for linting
+
+* **5.14.1** (2022-04-06)
+  * Dropped support for deprecated Python 3.6
+
+* **5.14.0** (2022-04-06)
+  * `EmailTestService` can now filter for subjects using regular expressions
+
+* **5.13.7** (2022-03-14)
+  * Fixed typo in coverage validator
+
+* **5.13.6** (2022-03-11)
+  * Improved console logging for coverage validator
+
+* **5.13.5** (2022-02-28)
+  * Improved motivation in class-based email docs
+
+* **5.13.4** (2022-02-28)
+  * Added Script for updating mirror
+  * Fixed typo in documentation
+
+* **5.13.3** (2022-02-23)
+  * Added GitHub action matrix for running tests on django/python combinations
+  * Updated Ambient email addresses to new domain
+  * Removed django <4.0 restriction
+  * Fixed tests for django 4.0
+
+* **5.13.2** (2022-02-21)
+  * `CurrentUserMiddleware` bugfix, cleaning up user variable for single-threaded tests after request processing
+  * Fixed version typo in changelog
+
+* **5.13.1** (2022-02-04)
+  * GraphQL docs bugfix
+
+* **5.13.0** (2022-02-03)
+  * Added a view which allows logging errors to Sentry normally while using Graphene.
+
+* **5.12.1** (2022-01-31)
+  * Fixed bug in Gitlab code coverage compare service documentation
+
+* **5.12.0** (2022-01-28)
+  * Added Gitlab code coverage compare service `CoverageService` with documentation
+
+* **5.11.1** (2022-01-24)
+  * Added docs for `ToggleView`
+  * Fixed some typos in `Readme.md` and `changelog.md`
+
+* **5.11.0** (2022-01-24)
+  * Added generic `ToggleView`
+  * Updated some docstrings in `formset_view_mixin`
+
+* **5.10.1** (2021-12-10)
+  * Added docs about GDPR-compliant use of sentry with user data
+  * Fixed some versions to make Sphinx build work again
+
+* **5.10.0** (2021-12-10)
+  * Added helper method for sentry to GDPR-compliant remove sensitive user data from event
+  * Updated type hints in `BaseEmailServiceFactory` init method
+  * Improved docs for method `get_start_and_end_date_from_calendar_week`
+
+* **5.9.1** (2021-11-25)
+  * Fixed typo in custom scrubber class logging
+  * Rewrote permission manager docs and added better best practice
+  * Update in email testing docs
+
+* **5.9.0** (2021-11-18)
+    * Added default truncate of django session table to `AbstractScrubbingService`
+
+* **5.8.0** (2021-11-11)
+    * Added `url` parameter to `RequestProviderMixin`
+
+* **5.7.4** (2021-11-08)
+    * Added missing documentation about semantic database anonymisation
+    * Added missing documentation about string utils
+    * Added missing documentation about `get_namedtuple_choices()` helper
+    * Added missing documentation about `CrispyLayoutFormMixin`
+    * Added missing documentation about `ClassBasedViewTestMixin`
+
+* **5.7.3** (2021-10-22)
+    * Added missing documentation about email testing
+    * Updated Readme file
+
+* **5.7.2** (2021-10-21)
+    * Fixed `flit` configuration
+
+* **5.7.1** (2021-10-21)
+    * Setup `flit` for release management
+
+* **5.7.0** (2021-10-15)
+    * Added admin mixin `DeactivatableChangeViewAdminMixin`
+    * Added `response` parameter to testing middlewares
+
+* **5.6.0** (2021-09-01)
+    * Extracted embedded form valid logic to separate method with super call in `_FormsetMixin`
+    * Added documentation about `FormsetCreateViewMixin` and `FormsetUpdateViewMixin`
+
+* **5.5.2** (2021-08-24)
+    * Added documentation about `BleacherMixin`
+
+* **5.5.1** (2021-08-24)
+    * Added explicit declaration of bleacher field list attribute `BLEACH_FIELD_LIST` in `BleacherMixin`
+
+* **5.5.0** (2021-08-02)
+    * Added validation for user object in `RequestProviderMixin`
+    * Added link to changelog in setup.py
+    * Moved minimum django version to 2.2
+
+* **5.4.0** (2021-06-28)
+    * Added `__len__` and `__iter__` to EmailTestService
+    * EmailTestService uses EmailTestServiceMail instances, which wrap the underlying Django mail objects, and provide
+      additional assertion functions
+
+* **5.3.0** (2021-06-16)
+    * Added `method` kwarg to `RequestProviderMixin.get_request()`
+
+* **5.2.2** (2021-05-27)
+    * Fixed a bug in `BaseEmailService` where txt part was rendered sometimes with weird line breaks
+    * Added Bugtracker link to `setup.py`
+
+* **5.2.1** (2021-05-12)
+    * Translation files were missing in wheel
+    * Bugfix in docs
+
+* **5.2.0** (2021-05-11)
+    * Changed all translatable texts to English base version
+    * Added German translation file for current translatable
+    * Updated RequestProviderMixin.get_request() type hinting
+    * Added documentation for database anonymisation / django-scrubber wrapper
+
+* **5.1.1** (2021-04-21)
+    * Extended email attachment functionality to be able to define filename and mimetype
+
+* **5.1.0** (2021-04-20)
+    * *Breaking change:* Fixed typo in `WhitelistEmailBackend.whitify_mail_adresses` method name. Method is now
+      called `whitify_mail_addresses`
+    * Moved assignment of `WhitelistEmailBackend` settings var to static methods to be able to overwrite them if needed
+    * Added documentation about `WhitelistEmailBackend`
+    * Added some type hinting to `WhitelistEmailBackend`
+    * Added formset mixin `CountChildrenFormsetMixin`
+    * Added djangorestframework field `RecursiveField`
+    * Added `get_attachments()` method to `BaseEmailService` and extended constructor to accept a
+      variable `attachment_list`
+
+* **5.0.0** (2021-03-26)
+    * *Breaking change:* Moved `ReadOnlyAdmin` and `EditableOnlyAdmin` to package `model_admins.classes`
+      and `ReadOnlyTabularInline` to package `model_admins.inlines` to enable better structuring of new admin components
+    * Fixed some inconsistencies within `ReadOnlyAdmin`, `EditableOnlyAdmin` and `ReadOnlyTabularInline` classes
+    * Added `admin.views` package containing a base crispy form, and a mixin to turn any regular django view into a nice
+      and cozy django admin view
+    * Added an abundance of `model_admins.mixins`: `AdminCreateFormMixin`, `AdminNoInlinesForCreateMixin`
+      ,`AdminRequestInFormMixin`, `FetchParentObjectInlineMixin`, `FetchObjectMixin`, `CommonInfoAdminMixin`
+    * Added `RequestProviderMixin` to easily create a dummy request in unittests
+    * Added support for django 3.2 and dropped support for 2.0, 2.1 and 3.0
+    * Added support for Python 3.9 and dropped support for 3.5
+    * Updated test python version to 3.9
+
+* **4.2.1** (2021-03-17)
+    * Added some links to setup.py for pypi
+    * Added some documentation for setting up the toolbox
+
+* **4.2.0** (2021-03-12)
+    * Added ``GloballyVisibleQuerySet`` including tests and documentation
+    * Added ``BaseViewSetTestMixin`` for the djangorestframework plugin
+    * Fixed some typos in the documentation
+
+* **4.1.2** (2021-03-05)
+    * Added kwargs parameter to init-method of `BaseEmailServiceFactory`
+
+* **4.1.1** (2021-03-04)
+    * Fixed a bug in the documentation
+
+* **4.1.0** (2021-02-25)
+    * Added class `BaseEmailService` for easier email creation and factory `BaseEmailServiceFactory`
+      for multiple (mostly personalised) emails
+    * Added `html2text` as a dependency to be able to automatically process the text part of an email from the html
+      template
+
+* **4.0.2** (2021-02-24)
+    * Fixed a bug in ``EmailTestService.assert_body_contains()`` method to make it work for emails NOT having an HTML
+      part
+
+* **4.0.1** (2021-01-29)
+    * Optimised code of function `test_get_value_from_tuple_by_key_found()`
+    * Added unittests for named tuple functions
+
+* **4.0.0** (2020-11-10)
+    * *Breaking change:* Moved view mixin ``RequestInFormKwargsMixin`` from ``mixin.forms`` to proper place
+      ``mixin.views``
+    * *Breaking change:* Removed string helper function ``restore_windows1252controls()``, ``number_to_text()`` and
+      ``replace_link_pattern()``
+    * *Breaking change:* Removed choice converter function ``get_name_by_value()`` in favour
+      of ``get_value_from_tuple_by_key()``
+    * *Breaking change:* Removed date converter function ``get_seconds()`` because Python 3.6 already provides
+      a `total_seconds()` method
+    * *Breaking change:* Removed date converter function ``get_current_datetime()`` because django already provides
+      the `timezone.now()` method
+    * *Breaking change:* Removed date converter function ``diff_month()`` in favour of ``date_month_delta()``
+    * *Breaking change:* Merged ``converter`` package in ``utils`` package
+    * *Breaking change:* Moved view-layer-based helpers to extra requirement ``view-layer``: `_FormsetMixin`,
+      `FormsetUpdateViewMixin`, `FormsetCreateViewMixin`, `CrispyLayoutFormMixin`, `CustomPermissionMixin`
+      , `RequestInFormKwargsMixin`
+    * Simplified code of function ``float_to_string()``
+    * Added type hinting to lots of helper functions
+    * Updated and restructured documentation
+    * Added security check for dependencies in local pipeline
+    * Removed some old python 2.7 syntax
+
+* **3.5.2** (2021-01-07)
+    * Bugfix with args and kwargs in ``ReadOnlyTabularInline``
+
+* **3.5.1** (2020-11-19)
+    * Bugfix with args and kwargs in ``ClassBasedViewTestMixin``
+
+* **3.5.0** (2020-11-10)
+    * Merged package ``graphene-django-ai`` into this package and enabled graphql-specific installation
+      with `pip install ai_django_core[graphql]`
+    * Added some files for readthedocs.io and updated Readme
+
+* **3.4.0** (2020-10-30)
+    * Moved tests out of package scope
+    * Updated test python version to 3.8
+    * Added tests for context manager ``TempDisconnectSignal`` with test setup
+
+* **3.3.0** (2020-10-30)
+    * Merged package ``ai-drf-core`` into this package and enabled djangorestframework-specific installation
+      with `pip install ai_django_core[drf]`
+    * Added ``BaseModelSerializer`` and ``CommonInfoSerializer``
+    * Incremented dependencies django and bleach to previous versions latest bugfix release
+
+* **3.2.0** (2020-10-16)
+    * Added ``AbstractPermissionMixin``, ``AbstractUserSpecificQuerySet`` and ``AbstractUserSpecificManager`` abstract
+      managers
+    * Removed deprecated `antivir` package
+    * Added Sphinx documentation setup to package
+
+* **3.1.0** (2020-10-14)
+    * Added context manager ``TempDisconnectSignal`` to nicely disable model signals temporarily
+    * Moved dev dependencies to ``extras_require`` in the setup file
+
+* **3.0.2** (2020-10-15)
+    * Imports all utils into the modules scope
+    * Re-translated some docstrings into English
+    * Added tests for the `log_whodid` util function
+
+* **3.0.1** (2020-10-12)
+    * Added missing ``__init__.py`` file to package mail.services
+
+* **3.0.0** (2020-09-09)
+    * *Breaking change:*  Renamed package from `ai` to `ai_django_core` to clarify dependencies for usages
+    * Finished code linting
+    * Removed unused imports in antivirus util package
+
+* **2.3.0** (2020-08-07)
+    * Changed `ugettext_lazy` to `gettext_lazy` to tackle django 4.0 deprecation warnings
+
+* **2.2.1** (2020-07-01)
+    * Removed misleading inheritance of mixin `ClassBasedViewTestMixin` from `TestCase`
+
+* **2.2.0** (2020-07-01)
+    * Added response class `CustomPermissionMixin`
+
+* **2.1.2** (2020-04-30)
+    * Extended pypi documentation with classifiers
+
+* **2.1.1** (2020-04-24)
+    * Refactors open calls to use context managers
+    * Refactors the test setup
+    * Configures coverage
+    * Adds a coverage report to the CI
+
+* **2.1.0** (2020-04-20)
+    * Removed password generator method `generate_password`
+    * Renamed math method `round_up_to_decimal` to `round_up_decimal`
+    * Added math method `round_to_decimal`
+    * Updated metadata in setup.cfg
+
+* **2.0.0** (2020-04-09)
+    * Dropped Python 2.x support
+    * Removed explicit dependency to package `mock` and using implicit one via unittest
+    * Improved linting
+
+* **1.2.14** (2020-04-06)
+    * Fixed a bug with session setup in `ClassBasedViewTestMixin`
+
+* **1.2.13** (2020-04-02)
+    * Added ``DELETE`` method for testing mixing `ClassBasedViewTestMixin`
+
+* **1.2.12** (2020-02-14)
+    * Added CBV testing mixing `ClassBasedViewTestMixin`
+
+* **1.2.11** (2020-01-28)
+    * Bugfix in documentation
+
+* **1.2.10** (2020-01-28)
+    * Improved documentation
+
+* **1.2.9** (2020-01-02)
+    * Extended and improved class `AbstractScrubbingService`
+
+* **1.2.8** (2019-12-13)
+    * Added custom scrubber class `AbstractScrubbingService` to provide a helper for adding custom scrubbing logic for
+      data anonymisation
+
+* **1.2.7** (2019-07-11)
+    * Added email testing class `EmailTestService` to provide a wrapper for better email unittests
+
+* **1.2.6** (2019-07-02)
+    * Added helper class `tz_today()` to provide an easy getter for a timezone-aware today
+
+* **1.2.5** (2019-06-25)
+    * Added helper class `DateHelper` to provide constants to use in django's ORM lookup `__week_day`
+
+* **1.2.4** (2019-05-20)
+    * More refactoring on `CurrentUserMiddleware` to make it easier to override internal functions
+
+* **1.2.3** (2019-05-20)
+    * Moved `get_current_user` function inside `CurrentUserMiddleware` as a static method to enable devs to override it
+
+* **1.2.2** (2019-04-05)
+    * Updated deployment documentation
+    * Added markdown support to Readme file
+
+* **1.2.1** (2019-03-25)
+    * Fixed bug causing `CommonInfo` middleware to not set `lastmodified_by` on object creation
+
+* **1.2.0** (2019-03-19)
+    * Added `CommonInfo` middleware
+
+* **1.1.8**
+    * Readonly admin classes
+    * Date util functions
+    * Clear cache helper
+
+* **1.1.7**
+    * Settings for whitelist email services added
+    * Formset mixins added
+
+* **1.1.6**
+    * Modifications to antivirus field
+
+* **1.1.5**
+    * Updated setup.py with newer information
+
+* **1.1.4**
+    * Bleacher mixin bugfix
+
+* **1.1.3**
+    * Bleacher mixin added
+
+* **< 1.1.3**
+    * Ancient history :)
```

### Comparing `ai-django-core-7.0.0/Dockerfile` & `ai-django-core-7.0.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/LICENSE.md` & `ai-django-core-7.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/README.md` & `ai-django-core-7.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,135 +1,143 @@
-[![pypi](https://img.shields.io/pypi/v/ai-django-core.svg)](https://pypi.python.org/pypi/ai-django-core/)
-[![Downloads](https://pepy.tech/badge/ai-django-core)](https://pepy.tech/project/ai-django-core)
-[![Documentation Status](https://readthedocs.org/projects/ai-django-core/badge/?version=latest)](https://ai-django-core.readthedocs.io/en/latest/?badge=latest)
-
-# Overview
-
-This package contains various useful helper functions. You can read up on all the fancy things at
-[readthedocs.io](https://ai-django-core.readthedocs.io/en/latest/index.html).
-
-# Installation
-
-- Install the package via pip:
-
-  `pip install ai-django-core`
-
-  or via pipenv:
-
-  `pipenv install ai-django-core`
-
-- Add module to `INSTALLED_APPS` within the main django `settings.py`:
-
-    ````
-    INSTALLED_APPS = (
-        ...
-        'ai_django_core',
-    )
-     ````
-
-# Contribute
-
-## Setup package for development
-
-- Create a Python 3.11 virtualenv
-- Activate the virtualenv (take care that you need `Scripts/activate.ps1` for Windows users instead of
-  `Scripts/activate`)
-- Install dependencies with `pip install .[dev,docs,view-layer,drf,graphql]`
-
-## Add functionality
-
-- Clone the project locally
-- Create a new branch for your feature
-- Change the dependency in your requirements.txt to a local (editable) one that points to your local file system:
-  `-e /Users/workspace/ai-django-core` or via pip  `pip install -e /Users/workspace/ai-django-core`
-- Ensure the code passes the tests
-- Create a pull request
-
-## Run tests
-
-- Check coverage
-  ````
-  pytest --cov=.
-  ````
-
-- Run tests
-  ````
-  pytest
-  ````
-
-## Git hooks (via pre-commit)
-
-We use pre-push hooks to ensure that only linted code reaches our remote repository and pipelines aren't triggered in
-vain.
-
-To enable the configured pre-push hooks, you need to [install](https://pre-commit.com/) pre-commit and run once:
-
-    pre-commit install -t pre-push -t pre-commit --install-hooks
-
-This will permanently install the git hooks for both, frontend and backend, in your local
-[`.git/hooks`](./.git/hooks) folder.
-The hooks are configured in the [`.pre-commit-config.yaml`](.pre-commit-config.yaml).
-
-You can check whether hooks work as intended using the [run](https://pre-commit.com/#pre-commit-run) command:
-
-    pre-commit run [hook-id] [options]
-
-Example: run single hook
-
-    pre-commit run ruff --all-files --hook-stage push
-
-Example: run all hooks of pre-push stage
-
-    pre-commit run --all-files --hook-stage push
-
-## Update documentation
-
-- To generate new auto-docs for new modules run: `sphinx-apidoc -o ./docs/modules/ ./ai_django_core/` (in the current
-  set up an auto doc for the antivirus module is not supported due to installation and import problems. Since it might
-  be removed in the future, that should be fine for now).
-- To build the documentation run: `sphinx-build docs/ docs/_build/html/` or go into the **docs** folder and
-  run: `make html`. Open `docs/_build/html/index.html` to see the documentation.
-
-## Translation files
-
-If you have added custom text, make sure to wrap it in `_()` where `_` is
-gettext_lazy (`from django.utils.translation import gettext_lazy as _`).
-
-How to create translation file:
-
-* Navigate to `ai_django_core/ai_django_core` (the inner directory!)
-* `python manage.py makemessages -l de`
-* Have a look at the new/changed files within `ai_django_core/ai_django_core/locale`
-
-How to compile translation files:
-
-* Navigate to `ai_django_core/ai_django_core` (the inner directory!)
-* `python manage.py compilemessages`
-* Have a look at the new/changed files within `ai_django_core/ai_django_core/locale`
-
-## Publish to ReadTheDocs.io
-
-- Fetch the latest changes in GitHub mirror and push them
-- Trigger new build at ReadTheDocs.io (follow instructions in admin panel at RTD) if the GitHub webhook is not yet set
-  up.
-
-## Publish to PyPi
-
-- Update documentation about new/changed functionality
-
-- Update the `Changelog`
-
-- Increment version in main `__init__.py`
-
-- Create pull request / merge to master
-
-- This project uses the flit package to publish to PyPI. Thus publishing should be as easy as running:
-  ```
-  flit publish
-  ```
-
-  To publish to TestPyPI use the following ensure that you have set up your .pypirc as
-  shown [here](https://flit.readthedocs.io/en/latest/upload.html#using-pypirc) and use the following command:
-
-  ```
-  flit publish --repository testpypi
-  ```
+[![pypi](https://img.shields.io/pypi/v/ai-django-core.svg)](https://pypi.python.org/pypi/ai-django-core/)
+[![Downloads](https://pepy.tech/badge/ai-django-core)](https://pepy.tech/project/ai-django-core)
+[![Documentation Status](https://readthedocs.org/projects/ai-django-core/badge/?version=latest)](https://ai-django-core.readthedocs.io/en/latest/?badge=latest)
+
+# Disclaimer: Package was superseded by ambient-toolbox!
+
+This package was renamed, moved and deprecated under the old name. The successor is the "**Ambient Toolbox**".
+* [PyPI](https://pypi.org/project/ambient-toolbox/)
+* [Migration docs](https://github.com/ambient-innovation/ambient-toolbox#migration-from-ai_django_core)
+
+---
+
+# Overview
+
+This package contains various useful helper functions. You can read up on all the fancy things at
+[readthedocs.io](https://ai-django-core.readthedocs.io/en/latest/index.html).
+
+# Installation
+
+- Install the package via pip:
+
+  `pip install ai-django-core`
+
+  or via pipenv:
+
+  `pipenv install ai-django-core`
+
+- Add module to `INSTALLED_APPS` within the main django `settings.py`:
+
+    ````
+    INSTALLED_APPS = (
+        ...
+        'ai_django_core',
+    )
+     ````
+
+# Contribute
+
+## Setup package for development
+
+- Create a Python 3.11 virtualenv
+- Activate the virtualenv (take care that you need `Scripts/activate.ps1` for Windows users instead of
+  `Scripts/activate`)
+- Install dependencies with `pip install .[dev,docs,view-layer,drf,graphql]`
+
+## Add functionality
+
+- Clone the project locally
+- Create a new branch for your feature
+- Change the dependency in your requirements.txt to a local (editable) one that points to your local file system:
+  `-e /Users/workspace/ai-django-core` or via pip  `pip install -e /Users/workspace/ai-django-core`
+- Ensure the code passes the tests
+- Create a pull request
+
+## Run tests
+
+- Check coverage
+  ````
+  pytest --cov=.
+  ````
+
+- Run tests
+  ````
+  pytest
+  ````
+
+## Git hooks (via pre-commit)
+
+We use pre-push hooks to ensure that only linted code reaches our remote repository and pipelines aren't triggered in
+vain.
+
+To enable the configured pre-push hooks, you need to [install](https://pre-commit.com/) pre-commit and run once:
+
+    pre-commit install -t pre-push -t pre-commit --install-hooks
+
+This will permanently install the git hooks for both, frontend and backend, in your local
+[`.git/hooks`](./.git/hooks) folder.
+The hooks are configured in the [`.pre-commit-config.yaml`](.pre-commit-config.yaml).
+
+You can check whether hooks work as intended using the [run](https://pre-commit.com/#pre-commit-run) command:
+
+    pre-commit run [hook-id] [options]
+
+Example: run single hook
+
+    pre-commit run ruff --all-files --hook-stage push
+
+Example: run all hooks of pre-push stage
+
+    pre-commit run --all-files --hook-stage push
+
+## Update documentation
+
+- To generate new auto-docs for new modules run: `sphinx-apidoc -o ./docs/modules/ ./ai_django_core/` (in the current
+  set up an auto doc for the antivirus module is not supported due to installation and import problems. Since it might
+  be removed in the future, that should be fine for now).
+- To build the documentation run: `sphinx-build docs/ docs/_build/html/` or go into the **docs** folder and
+  run: `make html`. Open `docs/_build/html/index.html` to see the documentation.
+
+## Translation files
+
+If you have added custom text, make sure to wrap it in `_()` where `_` is
+gettext_lazy (`from django.utils.translation import gettext_lazy as _`).
+
+How to create translation file:
+
+* Navigate to `ai_django_core/ai_django_core` (the inner directory!)
+* `python manage.py makemessages -l de`
+* Have a look at the new/changed files within `ai_django_core/ai_django_core/locale`
+
+How to compile translation files:
+
+* Navigate to `ai_django_core/ai_django_core` (the inner directory!)
+* `python manage.py compilemessages`
+* Have a look at the new/changed files within `ai_django_core/ai_django_core/locale`
+
+## Publish to ReadTheDocs.io
+
+- Fetch the latest changes in GitHub mirror and push them
+- Trigger new build at ReadTheDocs.io (follow instructions in admin panel at RTD) if the GitHub webhook is not yet set
+  up.
+
+## Publish to PyPi
+
+- Update documentation about new/changed functionality
+
+- Update the `Changelog`
+
+- Increment version in main `__init__.py`
+
+- Create pull request / merge to master
+
+- This project uses the flit package to publish to PyPI. Thus publishing should be as easy as running:
+  ```
+  flit publish
+  ```
+
+  To publish to TestPyPI use the following ensure that you have set up your .pypirc as
+  shown [here](https://flit.readthedocs.io/en/latest/upload.html#using-pypirc) and use the following command:
+
+  ```
+  flit publish --repository testpypi
+  ```
```

### Comparing `ai-django-core-7.0.0/ai_django_core/admin/model_admins/classes.py` & `ai-django-core-7.0.1/ai_django_core/admin/model_admins/classes.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/admin/model_admins/inlines.py` & `ai-django-core-7.0.1/ai_django_core/admin/model_admins/inlines.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/admin/model_admins/mixins.py` & `ai-django-core-7.0.1/ai_django_core/admin/model_admins/mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/admin/views/forms.py` & `ai-django-core-7.0.1/ai_django_core/admin/views/forms.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/admin/views/mixins.py` & `ai-django-core-7.0.1/ai_django_core/admin/views/mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/context_manager.py` & `ai-django-core-7.0.1/ai_django_core/context_manager.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/drf/fields.py` & `ai-django-core-7.0.1/ai_django_core/drf/fields.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/drf/serializers.py` & `ai-django-core-7.0.1/ai_django_core/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/drf/tests.py` & `ai-django-core-7.0.1/ai_django_core/drf/tests.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/gitlab/coverage.py` & `ai-django-core-7.0.1/ai_django_core/gitlab/coverage.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/graphql/forms/mutations.py` & `ai-django-core-7.0.1/ai_django_core/graphql/forms/mutations.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/graphql/schemes/mutations.py` & `ai-django-core-7.0.1/ai_django_core/graphql/schemes/mutations.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/graphql/sentry/views.py` & `ai-django-core-7.0.1/ai_django_core/graphql/sentry/views.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/graphql/tests/base_test.py` & `ai-django-core-7.0.1/ai_django_core/graphql/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/locale/de/LC_MESSAGES/django.mo` & `ai-django-core-7.0.1/ai_django_core/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/locale/de/LC_MESSAGES/django.po` & `ai-django-core-7.0.1/ai_django_core/locale/de/LC_MESSAGES/django.po`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-# Translations for ai-django-core package
-# Copyright (C) 2021 Ambient Innovation: GmbH
-# This file is distributed under the same license as the PACKAGE package.
-# Ronny Vedrilla, 2021
-#
-#, fuzzy
-msgid ""
-msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
-"Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-08-15 16:12+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-
-#: .\ai_django_core\admin\views\forms.py:12
-msgid "No title defined"
-msgstr "Kein Titel gesetzt"
-
-#: .\ai_django_core\admin\views\forms.py:13
-#: .\ai_django_core\view_layer\form_mixins.py:16
-msgid "Save"
-msgstr "Speichern"
-
-#: .\ai_django_core\mail\services\base.py:42
-msgid "Email factory requires a mail service class."
-msgstr "E-Mailfactory benötigt eine Mailservice-Klasse."
-
-#: .\ai_django_core\mail\services\base.py:44
-msgid "Email factory requires a target mail address."
-msgstr "E-Mailfactory benötigt eine Ziel-Mailadresse."
-
-#: .\ai_django_core\mail\services\base.py:212
-msgid "Missing or mislabeled data provided for email attachment."
-msgstr "Fehlende oder falsch deklarierte Daten für E-Mailanhänge übergeben."
-
-#: .\ai_django_core\mail\services\base.py:269
-msgid "Email service requires a subject."
-msgstr "E-Mailservice benötigt einen Betreff."
-
-#: .\ai_django_core\mail\services\base.py:271
-msgid "Email service requires a template."
-msgstr "E-Mailservice benötigt ein Template."
-
-#: .\ai_django_core\mail\services\base.py:273
-msgid "Email service requires a target mail address."
-msgstr "E-Mailservice benötigt eine Ziel-Mailadresse."
-
-#: .\ai_django_core\models.py:10
-msgid "Created at"
-msgstr "Erstellt am"
-
-#: .\ai_django_core\models.py:25
-msgid "Created by"
-msgstr "Erstellt von"
-
-#: .\ai_django_core\models.py:31
-msgid "Last modified at"
-msgstr "Zuletzt geändert am"
-
-#: .\ai_django_core\models.py:34
-msgid "Last modified by"
-msgstr "Zuletzt geändert von"
-
-#: .\ai_django_core\tests\mixins.py:92
-msgid "Please pass a user object to RequestProviderMixin."
-msgstr "Bitte ein User-Objekt an RequestProviderMixin übergeben."
-
-#: .\ai_django_core\utils\date.py:74
-msgid "Seconds must be positive."
-msgstr "Sekunden müssen eine positive Zahl sein."
-
-#: .\ai_django_core\view_layer\mixins.py:20
-msgid ""
-"Class-based view using DjangoPermissionRequiredMixin without defining a "
-"permission list."
-msgstr ""
-"Klassen-basierter View verwendet DjangoPermissionRequiredMixin ohne "
-"definierte Berechtigungen."
-
-#: .\ai_django_core\view_layer\tests\mixins.py:31
-msgid "BaseViewPermissionTestMixin used without setting a \"view_class\"."
-msgstr ""
-"BaseViewPermissionTestMixin verwendet ohne eine View-Klasse gesetzt zu haben."
-
-#: .\testapp\templates\403.html:53
-msgid "Error 403"
-msgstr "Fehler 403"
+# Translations for ai-django-core package
+# Copyright (C) 2021 Ambient Innovation: GmbH
+# This file is distributed under the same license as the PACKAGE package.
+# Ronny Vedrilla, 2021
+#
+#, fuzzy
+msgid ""
+msgstr ""
+"Project-Id-Version: PACKAGE VERSION\n"
+"Report-Msgid-Bugs-To: \n"
+"POT-Creation-Date: 2022-08-15 16:12+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
+"MIME-Version: 1.0\n"
+"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: .\ai_django_core\admin\views\forms.py:12
+msgid "No title defined"
+msgstr "Kein Titel gesetzt"
+
+#: .\ai_django_core\admin\views\forms.py:13
+#: .\ai_django_core\view_layer\form_mixins.py:16
+msgid "Save"
+msgstr "Speichern"
+
+#: .\ai_django_core\mail\services\base.py:42
+msgid "Email factory requires a mail service class."
+msgstr "E-Mailfactory benötigt eine Mailservice-Klasse."
+
+#: .\ai_django_core\mail\services\base.py:44
+msgid "Email factory requires a target mail address."
+msgstr "E-Mailfactory benötigt eine Ziel-Mailadresse."
+
+#: .\ai_django_core\mail\services\base.py:212
+msgid "Missing or mislabeled data provided for email attachment."
+msgstr "Fehlende oder falsch deklarierte Daten für E-Mailanhänge übergeben."
+
+#: .\ai_django_core\mail\services\base.py:269
+msgid "Email service requires a subject."
+msgstr "E-Mailservice benötigt einen Betreff."
+
+#: .\ai_django_core\mail\services\base.py:271
+msgid "Email service requires a template."
+msgstr "E-Mailservice benötigt ein Template."
+
+#: .\ai_django_core\mail\services\base.py:273
+msgid "Email service requires a target mail address."
+msgstr "E-Mailservice benötigt eine Ziel-Mailadresse."
+
+#: .\ai_django_core\models.py:10
+msgid "Created at"
+msgstr "Erstellt am"
+
+#: .\ai_django_core\models.py:25
+msgid "Created by"
+msgstr "Erstellt von"
+
+#: .\ai_django_core\models.py:31
+msgid "Last modified at"
+msgstr "Zuletzt geändert am"
+
+#: .\ai_django_core\models.py:34
+msgid "Last modified by"
+msgstr "Zuletzt geändert von"
+
+#: .\ai_django_core\tests\mixins.py:92
+msgid "Please pass a user object to RequestProviderMixin."
+msgstr "Bitte ein User-Objekt an RequestProviderMixin übergeben."
+
+#: .\ai_django_core\utils\date.py:74
+msgid "Seconds must be positive."
+msgstr "Sekunden müssen eine positive Zahl sein."
+
+#: .\ai_django_core\view_layer\mixins.py:20
+msgid ""
+"Class-based view using DjangoPermissionRequiredMixin without defining a "
+"permission list."
+msgstr ""
+"Klassen-basierter View verwendet DjangoPermissionRequiredMixin ohne "
+"definierte Berechtigungen."
+
+#: .\ai_django_core\view_layer\tests\mixins.py:31
+msgid "BaseViewPermissionTestMixin used without setting a \"view_class\"."
+msgstr ""
+"BaseViewPermissionTestMixin verwendet ohne eine View-Klasse gesetzt zu haben."
+
+#: .\testapp\templates\403.html:53
+msgid "Error 403"
+msgstr "Fehler 403"
```

### Comparing `ai-django-core-7.0.0/ai_django_core/mail/backends/whitelist_smtp.py` & `ai-django-core-7.0.1/ai_django_core/mail/backends/whitelist_smtp.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-import re
-
-from django.conf import settings
-from django.core.mail.backends.smtp import EmailBackend as SMTPEmailBackend
-
-
-class WhitelistEmailBackend(SMTPEmailBackend):
-    """
-    Via the following settings it is possible to configure if mails are sent to all domains.
-    If not, you can configure a redirect to an inbox via CATCHALL.
-
-    EMAIL_BACKEND = 'ai_django_core.mail.backends.whitelist_smtp.WhitelistEmailBackend'
-    EMAIL_BACKEND_DOMAIN_WHITELIST = ['ambient.digital']
-    EMAIL_BACKEND_REDIRECT_ADDRESS = '%s@testuser.ambient.digital'
-
-    If `EMAIL_BACKEND_REDIRECT_ADDRESS` is set, a mail to `john.doe@example.com` will be redirected to
-    `john.doe_example.com@testuser.ambient.digital`
-    """
-
-    @staticmethod
-    def get_domain_whitelist() -> list:
-        """
-        Getter for configuration variable from the settings.
-        Will return a list of domains: ['ambient.digital', 'ambient.digital']
-        """
-        return getattr(settings, 'EMAIL_BACKEND_DOMAIN_WHITELIST', [])
-
-    @staticmethod
-    def get_email_regex():
-        """
-        Getter for configuration variable from the settings.
-        Will return a RegEX to match email whitelisted domains.
-        """
-        return r'^[\w\-\.]+@(%s)$' % '|'.join(x for x in WhitelistEmailBackend.get_domain_whitelist()).replace(
-            '.', r'\.'
-        )
-
-    @staticmethod
-    def get_backend_redirect_address() -> str:
-        """
-        Getter for configuration variable from the settings.
-        Will return a string with a placeholder for redirecting non-whitelisted domains.
-        """
-        return settings.EMAIL_BACKEND_REDIRECT_ADDRESS
-
-    @staticmethod
-    def whitify_mail_addresses(mail_address_list: list) -> list:
-        """
-        Check for every recipient in the list if its domain is included in the whitelist.
-        If not, and we have a redirect address configured, we change the original mail address to something new,
-        according to our configuration.
-        """
-        allowed_recipients = []
-        for to in mail_address_list:
-            if re.search(WhitelistEmailBackend.get_email_regex(), to):
-                allowed_recipients.append(to)
-            elif WhitelistEmailBackend.get_backend_redirect_address():
-                # Send not allowed emails to the configured redirect address (with CATCHALL)
-                allowed_recipients.append(WhitelistEmailBackend.get_backend_redirect_address() % to.replace('@', '_'))
-        return allowed_recipients
-
-    def _process_recipients(self, email_messages):
-        """
-        Helper method to wrap custom logic of this backend. Required to make it testable.
-        """
-        for email in email_messages:
-            allowed_recipients = self.whitify_mail_addresses(email.to)
-            email.to = allowed_recipients
-        return email_messages
-
-    def send_messages(self, email_messages):
-        """
-        Checks if email-recipients are in allowed domains and cancels if not.
-        Uses regular smtp-sending afterwards.
-        """
-        email_messages = self._process_recipients(email_messages)
-        super().send_messages(email_messages)
+import re
+
+from django.conf import settings
+from django.core.mail.backends.smtp import EmailBackend as SMTPEmailBackend
+
+
+class WhitelistEmailBackend(SMTPEmailBackend):
+    """
+    Via the following settings it is possible to configure if mails are sent to all domains.
+    If not, you can configure a redirect to an inbox via CATCHALL.
+
+    EMAIL_BACKEND = 'ai_django_core.mail.backends.whitelist_smtp.WhitelistEmailBackend'
+    EMAIL_BACKEND_DOMAIN_WHITELIST = ['ambient.digital']
+    EMAIL_BACKEND_REDIRECT_ADDRESS = '%s@testuser.ambient.digital'
+
+    If `EMAIL_BACKEND_REDIRECT_ADDRESS` is set, a mail to `john.doe@example.com` will be redirected to
+    `john.doe_example.com@testuser.ambient.digital`
+    """
+
+    @staticmethod
+    def get_domain_whitelist() -> list:
+        """
+        Getter for configuration variable from the settings.
+        Will return a list of domains: ['ambient.digital', 'ambient.digital']
+        """
+        return getattr(settings, 'EMAIL_BACKEND_DOMAIN_WHITELIST', [])
+
+    @staticmethod
+    def get_email_regex():
+        """
+        Getter for configuration variable from the settings.
+        Will return a RegEX to match email whitelisted domains.
+        """
+        return r'^[\w\-\.]+@(%s)$' % '|'.join(x for x in WhitelistEmailBackend.get_domain_whitelist()).replace(
+            '.', r'\.'
+        )
+
+    @staticmethod
+    def get_backend_redirect_address() -> str:
+        """
+        Getter for configuration variable from the settings.
+        Will return a string with a placeholder for redirecting non-whitelisted domains.
+        """
+        return settings.EMAIL_BACKEND_REDIRECT_ADDRESS
+
+    @staticmethod
+    def whitify_mail_addresses(mail_address_list: list) -> list:
+        """
+        Check for every recipient in the list if its domain is included in the whitelist.
+        If not, and we have a redirect address configured, we change the original mail address to something new,
+        according to our configuration.
+        """
+        allowed_recipients = []
+        for to in mail_address_list:
+            if re.search(WhitelistEmailBackend.get_email_regex(), to):
+                allowed_recipients.append(to)
+            elif WhitelistEmailBackend.get_backend_redirect_address():
+                # Send not allowed emails to the configured redirect address (with CATCHALL)
+                allowed_recipients.append(WhitelistEmailBackend.get_backend_redirect_address() % to.replace('@', '_'))
+        return allowed_recipients
+
+    def _process_recipients(self, email_messages):
+        """
+        Helper method to wrap custom logic of this backend. Required to make it testable.
+        """
+        for email in email_messages:
+            allowed_recipients = self.whitify_mail_addresses(email.to)
+            email.to = allowed_recipients
+        return email_messages
+
+    def send_messages(self, email_messages):
+        """
+        Checks if email-recipients are in allowed domains and cancels if not.
+        Uses regular smtp-sending afterwards.
+        """
+        email_messages = self._process_recipients(email_messages)
+        super().send_messages(email_messages)
```

### Comparing `ai-django-core-7.0.0/ai_django_core/mail/services/base.py` & `ai-django-core-7.0.1/ai_django_core/mail/services/base.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/mail/services/tests.py` & `ai-django-core-7.0.1/ai_django_core/mail/services/tests.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/managers.py` & `ai-django-core-7.0.1/ai_django_core/managers.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/middleware/current_user.py` & `ai-django-core-7.0.1/ai_django_core/middleware/current_user.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/mixins/bleacher.py` & `ai-django-core-7.0.1/ai_django_core/mixins/bleacher.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/mixins/models.py` & `ai-django-core-7.0.1/ai_django_core/mixins/models.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/models.py` & `ai-django-core-7.0.1/ai_django_core/models.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/selectors/permission.py` & `ai-django-core-7.0.1/ai_django_core/selectors/permission.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/sentry/helpers.py` & `ai-django-core-7.0.1/ai_django_core/sentry/helpers.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/services/custom_scrubber.py` & `ai-django-core-7.0.1/ai_django_core/services/custom_scrubber.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/templatetags/ai_email_tags.py` & `ai-django-core-7.0.1/ai_django_core/templatetags/ai_email_tags.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 00000000: 6672 6f6d 2064 6a61 6e67 6f20 696d 706f  from django impo
-00000010: 7274 2074 656d 706c 6174 650d 0a66 726f  rt template..fro
-00000020: 6d20 646a 616e 676f 2e74 656d 706c 6174  m django.templat
-00000030: 652e 6465 6661 756c 7466 696c 7465 7273  e.defaultfilters
-00000040: 2069 6d70 6f72 7420 7374 7269 6e67 6669   import stringfi
-00000050: 6c74 6572 0d0a 6672 6f6d 2064 6a61 6e67  lter..from djang
-00000060: 6f2e 7574 696c 732e 7361 6665 7374 7269  o.utils.safestri
-00000070: 6e67 2069 6d70 6f72 7420 6d61 726b 5f73  ng import mark_s
-00000080: 6166 650d 0a0d 0a72 6567 6973 7465 7220  afe....register 
-00000090: 3d20 7465 6d70 6c61 7465 2e4c 6962 7261  = template.Libra
-000000a0: 7279 2829 0d0a 0d0a 0d0a 6465 6620 6f62  ry()......def ob
-000000b0: 6675 7363 6174 655f 7374 7269 6e67 2876  fuscate_string(v
-000000c0: 616c 7565 293a 0d0a 2020 2020 7265 7475  alue):..    retu
-000000d0: 726e 2027 272e 6a6f 696e 285b 6627 2623  rn ''.join([f'&#
-000000e0: 7b73 7472 286f 7264 2863 6861 7229 293a  {str(ord(char)):
-000000f0: 737d 3b27 2066 6f72 2063 6861 7220 696e  s};' for char in
-00000100: 2076 616c 7565 5d29 0d0a 0d0a 0d0a 4072   value])......@r
-00000110: 6567 6973 7465 722e 6669 6c74 6572 0d0a  egister.filter..
-00000120: 4073 7472 696e 6766 696c 7465 720d 0a64  @stringfilter..d
-00000130: 6566 206f 6266 7573 6361 7465 2876 616c  ef obfuscate(val
-00000140: 7565 293a 0d0a 2020 2020 7265 7475 726e  ue):..    return
-00000150: 206d 6172 6b5f 7361 6665 286f 6266 7573   mark_safe(obfus
-00000160: 6361 7465 5f73 7472 696e 6728 7661 6c75  cate_string(valu
-00000170: 6529 290d 0a0d 0a0d 0a40 7265 6769 7374  e))......@regist
-00000180: 6572 2e66 696c 7465 720d 0a40 7374 7269  er.filter..@stri
-00000190: 6e67 6669 6c74 6572 0d0a 6465 6620 6f62  ngfilter..def ob
-000001a0: 6675 7363 6174 655f 6d61 696c 746f 2876  fuscate_mailto(v
-000001b0: 616c 7565 2c20 7465 7874 3d46 616c 7365  alue, text=False
-000001c0: 293a 0d0a 2020 2020 6d61 696c 203d 206f  ):..    mail = o
-000001d0: 6266 7573 6361 7465 5f73 7472 696e 6728  bfuscate_string(
-000001e0: 7661 6c75 6529 0d0a 0d0a 2020 2020 6966  value)....    if
-000001f0: 2074 6578 743a 0d0a 2020 2020 2020 2020   text:..        
-00000200: 6c69 6e6b 5f74 6578 7420 3d20 7465 7874  link_text = text
-00000210: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
-00000220: 2020 2020 206c 696e 6b5f 7465 7874 203d       link_text =
-00000230: 206d 6169 6c0d 0a0d 0a20 2020 2072 6574   mail....    ret
-00000240: 7572 6e20 6d61 726b 5f73 6166 6528 273c  urn mark_safe('<
-00000250: 6120 6872 6566 3d22 7b3a 737d 7b3a 737d  a href="{:s}{:s}
-00000260: 223e 7b3a 737d 3c2f 613e 272e 666f 726d  ">{:s}</a>'.form
-00000270: 6174 286f 6266 7573 6361 7465 5f73 7472  at(obfuscate_str
-00000280: 696e 6728 276d 6169 6c74 6f3a 2729 2c20  ing('mailto:'), 
-00000290: 6d61 696c 2c20 6c69 6e6b 5f74 6578 7429  mail, link_text)
-000002a0: 290d 0a                                  )..
+00000010: 7274 2074 656d 706c 6174 650a 6672 6f6d  rt template.from
+00000020: 2064 6a61 6e67 6f2e 7465 6d70 6c61 7465   django.template
+00000030: 2e64 6566 6175 6c74 6669 6c74 6572 7320  .defaultfilters 
+00000040: 696d 706f 7274 2073 7472 696e 6766 696c  import stringfil
+00000050: 7465 720a 6672 6f6d 2064 6a61 6e67 6f2e  ter.from django.
+00000060: 7574 696c 732e 7361 6665 7374 7269 6e67  utils.safestring
+00000070: 2069 6d70 6f72 7420 6d61 726b 5f73 6166   import mark_saf
+00000080: 650a 0a72 6567 6973 7465 7220 3d20 7465  e..register = te
+00000090: 6d70 6c61 7465 2e4c 6962 7261 7279 2829  mplate.Library()
+000000a0: 0a0a 0a64 6566 206f 6266 7573 6361 7465  ...def obfuscate
+000000b0: 5f73 7472 696e 6728 7661 6c75 6529 3a0a  _string(value):.
+000000c0: 2020 2020 7265 7475 726e 2027 272e 6a6f      return ''.jo
+000000d0: 696e 285b 6627 2623 7b73 7472 286f 7264  in([f'&#{str(ord
+000000e0: 2863 6861 7229 293a 737d 3b27 2066 6f72  (char)):s};' for
+000000f0: 2063 6861 7220 696e 2076 616c 7565 5d29   char in value])
+00000100: 0a0a 0a40 7265 6769 7374 6572 2e66 696c  ...@register.fil
+00000110: 7465 720a 4073 7472 696e 6766 696c 7465  ter.@stringfilte
+00000120: 720a 6465 6620 6f62 6675 7363 6174 6528  r.def obfuscate(
+00000130: 7661 6c75 6529 3a0a 2020 2020 7265 7475  value):.    retu
+00000140: 726e 206d 6172 6b5f 7361 6665 286f 6266  rn mark_safe(obf
+00000150: 7573 6361 7465 5f73 7472 696e 6728 7661  uscate_string(va
+00000160: 6c75 6529 290a 0a0a 4072 6567 6973 7465  lue))...@registe
+00000170: 722e 6669 6c74 6572 0a40 7374 7269 6e67  r.filter.@string
+00000180: 6669 6c74 6572 0a64 6566 206f 6266 7573  filter.def obfus
+00000190: 6361 7465 5f6d 6169 6c74 6f28 7661 6c75  cate_mailto(valu
+000001a0: 652c 2074 6578 743d 4661 6c73 6529 3a0a  e, text=False):.
+000001b0: 2020 2020 6d61 696c 203d 206f 6266 7573      mail = obfus
+000001c0: 6361 7465 5f73 7472 696e 6728 7661 6c75  cate_string(valu
+000001d0: 6529 0a0a 2020 2020 6966 2074 6578 743a  e)..    if text:
+000001e0: 0a20 2020 2020 2020 206c 696e 6b5f 7465  .        link_te
+000001f0: 7874 203d 2074 6578 740a 2020 2020 656c  xt = text.    el
+00000200: 7365 3a0a 2020 2020 2020 2020 6c69 6e6b  se:.        link
+00000210: 5f74 6578 7420 3d20 6d61 696c 0a0a 2020  _text = mail..  
+00000220: 2020 7265 7475 726e 206d 6172 6b5f 7361    return mark_sa
+00000230: 6665 2827 3c61 2068 7265 663d 227b 3a73  fe('<a href="{:s
+00000240: 7d7b 3a73 7d22 3e7b 3a73 7d3c 2f61 3e27  }{:s}">{:s}</a>'
+00000250: 2e66 6f72 6d61 7428 6f62 6675 7363 6174  .format(obfuscat
+00000260: 655f 7374 7269 6e67 2827 6d61 696c 746f  e_string('mailto
+00000270: 3a27 292c 206d 6169 6c2c 206c 696e 6b5f  :'), mail, link_
+00000280: 7465 7874 2929 0a                        text)).
```

### Comparing `ai-django-core-7.0.0/ai_django_core/templatetags/ai_file_tags.py` & `ai-django-core-7.0.1/ai_django_core/templatetags/ai_file_tags.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import os
-
-from django import template
-from django.conf import settings
-
-register = template.Library()
-
-
-@register.filter
-def filename(value, max_length=25):
-    """
-    Shortens the filename to maxlength 25 without loosing the file extension
-
-    :param value:
-    :param max_length:
-    :return filename with a max length of 25
-    """
-    name = os.path.basename(value.url)
-    if len(name) > max_length:
-        ext = name.split('.')[-1]
-        name = f"{name[:max_length]}[..].{ext}"
-    return name
-
-
-@register.filter
-def filesize(value):
-    """
-    Returns the filesize of the filename given in value
-
-    :param value:
-    :return filesize:
-    """
-    try:
-        return os.path.getsize(f"{settings.MEDIA_ROOT}{value}")
-    except Exception:
-        return 0
+import os
+
+from django import template
+from django.conf import settings
+
+register = template.Library()
+
+
+@register.filter
+def filename(value, max_length=25):
+    """
+    Shortens the filename to maxlength 25 without loosing the file extension
+
+    :param value:
+    :param max_length:
+    :return filename with a max length of 25
+    """
+    name = os.path.basename(value.url)
+    if len(name) > max_length:
+        ext = name.split('.')[-1]
+        name = f"{name[:max_length]}[..].{ext}"
+    return name
+
+
+@register.filter
+def filesize(value):
+    """
+    Returns the filesize of the filename given in value
+
+    :param value:
+    :return filesize:
+    """
+    try:
+        return os.path.getsize(f"{settings.MEDIA_ROOT}{value}")
+    except Exception:
+        return 0
```

### Comparing `ai-django-core-7.0.0/ai_django_core/templatetags/ai_number_tags.py` & `ai-django-core-7.0.1/ai_django_core/templatetags/ai_number_tags.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/templatetags/ai_string_tags.py` & `ai-django-core-7.0.1/ai_django_core/templatetags/ai_string_tags.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/tests/mixins.py` & `ai-django-core-7.0.1/ai_django_core/tests/mixins.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-from typing import Optional, Union
-
-from django.contrib.auth.base_user import AbstractBaseUser
-from django.contrib.auth.models import AnonymousUser
-from django.contrib.messages import get_messages
-from django.contrib.messages.middleware import MessageMiddleware
-from django.contrib.messages.storage.fallback import FallbackStorage
-from django.contrib.sessions.middleware import SessionMiddleware
-from django.core.handlers.wsgi import WSGIRequest
-from django.http import HttpResponse
-from django.test import RequestFactory
-from django.utils.translation import gettext_lazy as _
-
-
-class ClassBasedViewTestMixin:
-    """
-    Helper mixin for easy testing of Django views
-    """
-
-    factory_class = RequestFactory
-    view_class = None
-
-    @staticmethod
-    def _authentication(request, user):
-        request.user = user if user else AnonymousUser()
-
-    def _get_response(self, method, user, data, url_params=None, *args, **kwargs):
-        """Returns response."""
-
-        # Catch case that URL does not get any params passed to
-        if not url_params:
-            url_params = {}
-
-        # Create request
-        factory = self.factory_class()
-        req_kwargs = {}
-        if data:
-            req_kwargs.update({'data': data})
-        request = getattr(factory, method)('/', **req_kwargs)
-
-        # Annotate a request object with a session
-        middleware = SessionMiddleware(get_response=HttpResponse(status=200))
-        middleware.process_request(request)
-        request.session.save()
-
-        # Authenticate user
-        self._authentication(request, user)
-
-        # Setup messages
-        messages = FallbackStorage(request)
-        request._messages = messages
-
-        # Call view
-        return self.view_class.as_view()(request, *args, **url_params)
-
-    def get(self, user=None, data=None, url_params=None, *args, **kwargs):
-        """Returns response for a GET request."""
-        return self._get_response('get', user, data, url_params, *args, **kwargs)
-
-    def post(self, user=None, data=None, url_params=None, *args, **kwargs):
-        """Returns response for a POST request."""
-        return self._get_response('post', user, data, url_params, *args, **kwargs)
-
-    def delete(self, user=None, data=None, url_params=None, *args, **kwargs):
-        """Returns response for a DELETE request."""
-        return self._get_response('delete', user, data, url_params, *args, **kwargs)
-
-
-class RequestProviderMixin:
-    """
-    Mixin that provides a method which returns a django request.
-    Supposed to be used in unittests that require a request object.
-    Also adds the message middleware so django messages can be tested.
-    """
-
-    @staticmethod
-    def get_request(
-        user: Union[AbstractBaseUser, AnonymousUser, None] = None, method: str = 'GET', url: Optional[str] = None
-    ):
-        """
-        Creates and returns a django request.
-        """
-        # Determine URL
-        url = url if url else '/'
-
-        # Create test request
-        factory = RequestFactory()
-        request = factory.get(url)
-
-        # Set user object if it is of a valid type
-        if user is None or isinstance(user, AbstractBaseUser) or isinstance(user, AnonymousUser):
-            request.user = user
-        else:
-            raise ValueError(_('Please pass a user object to RequestProviderMixin.'))
-
-        # Annotate a request object with a session
-        session_middleware = SessionMiddleware(get_response=HttpResponse(status=200))
-        session_middleware.process_request(request)
-        request.session.save()
-
-        # Annotate a request object with messages
-        message_middleware = MessageMiddleware(get_response=HttpResponse(status=200))
-        message_middleware.process_request(request)
-        request.session.save()
-
-        # Set request method
-        request.method = method
-
-        return request
-
-
-class DjangoMessagingFrameworkTestMixin:
-    """
-    Mixin to enable test cases to easily check for messages in the request.
-    This test is made for the Django Messaging Framework.
-    """
-
-    def assert_full_message_in_request(self, request: WSGIRequest, message: str) -> None:
-        messages = list(get_messages(request))
-
-        self.assertGreater(len(messages), 0, "The request doesn't contain any messages.")
-        message_found = False
-        for request_message in messages:
-            if str(request_message) == message:
-                message_found = True
-
-        self.assertTrue(message_found, f"Message {message!r} not found in request.")
-
-    def assert_partial_message_in_request(self, request: WSGIRequest, message: str) -> None:
-        messages = list(get_messages(request))
-
-        self.assertGreater(len(messages), 0, "The request doesn't contain any messages.")
-
-        message_found = False
-        for request_message in messages:
-            if message in str(request_message):
-                message_found = True
-
-        self.assertTrue(message_found, f"Message part {message!r} not found in request.")
+from typing import Optional, Union
+
+from django.contrib.auth.base_user import AbstractBaseUser
+from django.contrib.auth.models import AnonymousUser
+from django.contrib.messages import get_messages
+from django.contrib.messages.middleware import MessageMiddleware
+from django.contrib.messages.storage.fallback import FallbackStorage
+from django.contrib.sessions.middleware import SessionMiddleware
+from django.core.handlers.wsgi import WSGIRequest
+from django.http import HttpResponse
+from django.test import RequestFactory
+from django.utils.translation import gettext_lazy as _
+
+
+class ClassBasedViewTestMixin:
+    """
+    Helper mixin for easy testing of Django views
+    """
+
+    factory_class = RequestFactory
+    view_class = None
+
+    @staticmethod
+    def _authentication(request, user):
+        request.user = user if user else AnonymousUser()
+
+    def _get_response(self, method, user, data, url_params=None, *args, **kwargs):
+        """Returns response."""
+
+        # Catch case that URL does not get any params passed to
+        if not url_params:
+            url_params = {}
+
+        # Create request
+        factory = self.factory_class()
+        req_kwargs = {}
+        if data:
+            req_kwargs.update({'data': data})
+        request = getattr(factory, method)('/', **req_kwargs)
+
+        # Annotate a request object with a session
+        middleware = SessionMiddleware(get_response=HttpResponse(status=200))
+        middleware.process_request(request)
+        request.session.save()
+
+        # Authenticate user
+        self._authentication(request, user)
+
+        # Setup messages
+        messages = FallbackStorage(request)
+        request._messages = messages
+
+        # Call view
+        return self.view_class.as_view()(request, *args, **url_params)
+
+    def get(self, user=None, data=None, url_params=None, *args, **kwargs):
+        """Returns response for a GET request."""
+        return self._get_response('get', user, data, url_params, *args, **kwargs)
+
+    def post(self, user=None, data=None, url_params=None, *args, **kwargs):
+        """Returns response for a POST request."""
+        return self._get_response('post', user, data, url_params, *args, **kwargs)
+
+    def delete(self, user=None, data=None, url_params=None, *args, **kwargs):
+        """Returns response for a DELETE request."""
+        return self._get_response('delete', user, data, url_params, *args, **kwargs)
+
+
+class RequestProviderMixin:
+    """
+    Mixin that provides a method which returns a django request.
+    Supposed to be used in unittests that require a request object.
+    Also adds the message middleware so django messages can be tested.
+    """
+
+    @staticmethod
+    def get_request(
+        user: Union[AbstractBaseUser, AnonymousUser, None] = None, method: str = 'GET', url: Optional[str] = None
+    ):
+        """
+        Creates and returns a django request.
+        """
+        # Determine URL
+        url = url if url else '/'
+
+        # Create test request
+        factory = RequestFactory()
+        request = factory.get(url)
+
+        # Set user object if it is of a valid type
+        if user is None or isinstance(user, AbstractBaseUser) or isinstance(user, AnonymousUser):
+            request.user = user
+        else:
+            raise ValueError(_('Please pass a user object to RequestProviderMixin.'))
+
+        # Annotate a request object with a session
+        session_middleware = SessionMiddleware(get_response=HttpResponse(status=200))
+        session_middleware.process_request(request)
+        request.session.save()
+
+        # Annotate a request object with messages
+        message_middleware = MessageMiddleware(get_response=HttpResponse(status=200))
+        message_middleware.process_request(request)
+        request.session.save()
+
+        # Set request method
+        request.method = method
+
+        return request
+
+
+class DjangoMessagingFrameworkTestMixin:
+    """
+    Mixin to enable test cases to easily check for messages in the request.
+    This test is made for the Django Messaging Framework.
+    """
+
+    def assert_full_message_in_request(self, request: WSGIRequest, message: str) -> None:
+        messages = list(get_messages(request))
+
+        self.assertGreater(len(messages), 0, "The request doesn't contain any messages.")
+        message_found = False
+        for request_message in messages:
+            if str(request_message) == message:
+                message_found = True
+
+        self.assertTrue(message_found, f"Message {message!r} not found in request.")
+
+    def assert_partial_message_in_request(self, request: WSGIRequest, message: str) -> None:
+        messages = list(get_messages(request))
+
+        self.assertGreater(len(messages), 0, "The request doesn't contain any messages.")
+
+        message_found = False
+        for request_message in messages:
+            if message in str(request_message):
+                message_found = True
+
+        self.assertTrue(message_found, f"Message part {message!r} not found in request.")
```

### Comparing `ai-django-core-7.0.0/ai_django_core/tests/structure_validator/test_structure_validator.py` & `ai-django-core-7.0.1/ai_django_core/tests/structure_validator/test_structure_validator.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/utils/date.py` & `ai-django-core-7.0.1/ai_django_core/utils/date.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/utils/file.py` & `ai-django-core-7.0.1/ai_django_core/utils/file.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/utils/math.py` & `ai-django-core-7.0.1/ai_django_core/utils/math.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/utils/model.py` & `ai-django-core-7.0.1/ai_django_core/utils/model.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/utils/named_tuple.py` & `ai-django-core-7.0.1/ai_django_core/utils/named_tuple.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-from collections import OrderedDict, namedtuple
-from typing import Any
-
-
-def get_namedtuple_choices(name, choices_tuple):
-    """
-    Made by Ross Crawford-d'Heureuse.
-
-    Factory function for quickly making a namedtuple suitable for use in a
-    Django model as a choices attribute on a field. It will preserve order.
-
-    Usage::
-
-        class MyModel(models.Model):
-            COLORS = get_namedtuple_choices('COLORS', (
-                (0, 'black', 'Black'),
-                (1, 'white', 'White'),
-            ))
-            colors = models.PositiveIntegerField(choices=COLORS)
-
-        >>> MyModel.COLORS.black
-        0
-        >>> MyModel.COLORS.get_choices()
-        [(0, 'Black'), (1, 'White')]
-
-        class OtherModel(models.Model):
-            GRADES = get_namedtuple_choices('GRADES', (
-                ('FR', 'fr', 'Freshman'),
-                ('SR', 'sr', 'Senior'),
-            ))
-            grade = models.CharField(max_length=2, choices=GRADES)
-
-        >>> OtherModel.GRADES.fr
-        'FR'
-        >>> OtherModel.GRADES.get_choices()
-        [('fr', 'Freshman'), ('sr', 'Senior')]
-    """
-
-    class Choices(namedtuple(name, [name for val, name, desc in choices_tuple])):
-        __slots__ = ()
-        _choices = tuple(desc for val, name, desc in choices_tuple)
-
-        def get_choices(self):
-            return list(zip(tuple(self), self._choices))
-
-        def get_choices_dict(self):
-            """
-            Return an ordered dict of key and their values
-            must be ordered correctly as there are items that depend on the key
-            order
-            """
-            choices = OrderedDict()
-            for k, v in self.get_choices():
-                choices[k] = v
-            return choices
-
-        def get_all(self):
-            yield from choices_tuple
-
-        def get_choices_tuple(self):
-            return choices_tuple
-
-        def get_values(self):
-            values = []
-            for val, _name, _desc in choices_tuple:
-                if isinstance(val, type([])):
-                    values.extend(val)
-                else:
-                    values.append(val)
-            return values
-
-        def get_value_by_name(self, input_name):
-            for val, _name, _desc in choices_tuple:
-                if _name == input_name:
-                    return val
-            return False
-
-        def get_desc_by_value(self, input_value):
-            for val, _name, _desc in choices_tuple:
-                if val == input_value:
-                    return _desc
-            return False
-
-        def get_name_by_value(self, input_value):
-            for val, _name, _desc in choices_tuple:
-                if val == input_value:
-                    return _name
-            return False
-
-        def is_valid(self, selection):
-            for val, _name, _desc in choices_tuple:
-                if val == selection or _name == selection or _desc == selection:
-                    return True
-            return False
-
-    return Choices._make([val for val, name, desc in choices_tuple])
-
-
-def get_value_from_tuple_by_key(choices: tuple, key) -> Any:
-    """
-    Fetches the tuple value by a given key
-    Useful for getting the name of a key from a model choice tuple of tuples.
-    Usage: project_type_a_name = get_value_from_tuple_by_key(PROJECT_TYPE_CHOICES, PROJECT_TYPE_A)
-    """
-    try:
-        return dict(choices)[key]
-    except KeyError:
-        return '-'
-
-
-def get_key_from_tuple_by_value(choices: tuple, value) -> Any:
-    """
-    Fetches the tuple key by a given value
-    Useful for getting the key of a value from a model choice tuple of tuples.
-    Usage: project_type_a_name = get_value_from_tuple_by_key(PROJECT_TYPE_CHOICES, 'Budget-Project')
-    """
-    try:
-        return [x[0] for x in choices if x[1] == value][0]
-    except IndexError:
-        return '-'
+from collections import OrderedDict, namedtuple
+from typing import Any
+
+
+def get_namedtuple_choices(name, choices_tuple):
+    """
+    Made by Ross Crawford-d'Heureuse.
+
+    Factory function for quickly making a namedtuple suitable for use in a
+    Django model as a choices attribute on a field. It will preserve order.
+
+    Usage::
+
+        class MyModel(models.Model):
+            COLORS = get_namedtuple_choices('COLORS', (
+                (0, 'black', 'Black'),
+                (1, 'white', 'White'),
+            ))
+            colors = models.PositiveIntegerField(choices=COLORS)
+
+        >>> MyModel.COLORS.black
+        0
+        >>> MyModel.COLORS.get_choices()
+        [(0, 'Black'), (1, 'White')]
+
+        class OtherModel(models.Model):
+            GRADES = get_namedtuple_choices('GRADES', (
+                ('FR', 'fr', 'Freshman'),
+                ('SR', 'sr', 'Senior'),
+            ))
+            grade = models.CharField(max_length=2, choices=GRADES)
+
+        >>> OtherModel.GRADES.fr
+        'FR'
+        >>> OtherModel.GRADES.get_choices()
+        [('fr', 'Freshman'), ('sr', 'Senior')]
+    """
+
+    class Choices(namedtuple(name, [name for val, name, desc in choices_tuple])):
+        __slots__ = ()
+        _choices = tuple(desc for val, name, desc in choices_tuple)
+
+        def get_choices(self):
+            return list(zip(tuple(self), self._choices))
+
+        def get_choices_dict(self):
+            """
+            Return an ordered dict of key and their values
+            must be ordered correctly as there are items that depend on the key
+            order
+            """
+            choices = OrderedDict()
+            for k, v in self.get_choices():
+                choices[k] = v
+            return choices
+
+        def get_all(self):
+            yield from choices_tuple
+
+        def get_choices_tuple(self):
+            return choices_tuple
+
+        def get_values(self):
+            values = []
+            for val, _name, _desc in choices_tuple:
+                if isinstance(val, type([])):
+                    values.extend(val)
+                else:
+                    values.append(val)
+            return values
+
+        def get_value_by_name(self, input_name):
+            for val, _name, _desc in choices_tuple:
+                if _name == input_name:
+                    return val
+            return False
+
+        def get_desc_by_value(self, input_value):
+            for val, _name, _desc in choices_tuple:
+                if val == input_value:
+                    return _desc
+            return False
+
+        def get_name_by_value(self, input_value):
+            for val, _name, _desc in choices_tuple:
+                if val == input_value:
+                    return _name
+            return False
+
+        def is_valid(self, selection):
+            for val, _name, _desc in choices_tuple:
+                if val == selection or _name == selection or _desc == selection:
+                    return True
+            return False
+
+    return Choices._make([val for val, name, desc in choices_tuple])
+
+
+def get_value_from_tuple_by_key(choices: tuple, key) -> Any:
+    """
+    Fetches the tuple value by a given key
+    Useful for getting the name of a key from a model choice tuple of tuples.
+    Usage: project_type_a_name = get_value_from_tuple_by_key(PROJECT_TYPE_CHOICES, PROJECT_TYPE_A)
+    """
+    try:
+        return dict(choices)[key]
+    except KeyError:
+        return '-'
+
+
+def get_key_from_tuple_by_value(choices: tuple, value) -> Any:
+    """
+    Fetches the tuple key by a given value
+    Useful for getting the key of a value from a model choice tuple of tuples.
+    Usage: project_type_a_name = get_value_from_tuple_by_key(PROJECT_TYPE_CHOICES, 'Budget-Project')
+    """
+    try:
+        return [x[0] for x in choices if x[1] == value][0]
+    except IndexError:
+        return '-'
```

### Comparing `ai-django-core-7.0.0/ai_django_core/utils/string.py` & `ai-django-core-7.0.1/ai_django_core/utils/string.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-import datetime
-import os
-from typing import Optional, Union
-
-from django.contrib.humanize.templatetags.humanize import intcomma
-from django.template.defaultfilters import floatformat, slugify
-from django.utils.encoding import smart_str
-
-from ai_django_core.utils import datetime_format
-
-
-def distinct(not_distinct_list: list) -> list:
-    """
-    Returns a list with no duplicate elements
-    """
-    return list(set(not_distinct_list))
-
-
-def slugify_file_name(file_name: str, length: int = 40) -> str:
-    """
-    Slugify the given file name
-    """
-    name, ext = os.path.splitext(file_name)
-    name = smart_str(slugify(name).replace('-', '_'))
-    ext = smart_str(slugify(ext))
-    result = '{}{}{}'.format(name[:length], "." if ext else "", ext)
-    return result
-
-
-def smart_truncate(text: str, max_length: int = 100, suffix: str = '...') -> str:
-    """
-    Returns a string of at most `max_length` characters, cutting
-    only at word-boundaries. If the string was truncated, `suffix`
-    will be appended.
-    In comparison to Djangos default filter `truncatechars` this method does NOT break words and you
-    can choose a custom suffix.
-    """
-    if text is None:
-        return ''
-
-    # Return the string itself if length is smaller or equal to the limit
-    if len(text) <= max_length:
-        return text
-
-    # Cut the string
-    value = text[:max_length]
-
-    # Break into words and remove the last
-    words = value.split(' ')[:-1]
-
-    # Join the words and return
-    return ' '.join(words) + suffix
-
-
-def float_to_string(value: Optional[float], replacement: str = "0,00") -> str:
-    """
-    Converts a float to a properly, German-formatted string value
-    # todo name is misleading, should contain "de"
-    # todo thousand separator would be nice
-    If the passed object is None, it will return `replacement`.
-    """
-    return ("%.2f" % value).replace('.', ',') if value is not None else replacement
-
-
-def date_to_string(value: Optional[datetime.date], replacement: str = "-", str_format: str = "%d.%m.%Y") -> str:
-    """
-    Converts a given date "value" to a string formatted with `str_format`.
-    If the passed "value" is None, it will return `replacement`.
-    """
-    return value.strftime(str_format) if value is not None else replacement
-
-
-def datetime_to_string(
-    value: Optional[datetime.datetime], replacement: str = "-", str_format: str = "%d.%m.%Y %H:%M"
-) -> str:
-    """
-    Converts a given datetime "value" to a string formatted with `str_format`.
-    If the passed "value" is None, it will return `replacement`.
-    """
-    return datetime_format(value, str_format) if value is not None else replacement
-
-
-def number_to_string(value: Optional[Union[int, float]], decimal_digits: int = 0, replacement: str = "-") -> str:
-    """
-    Converts a given int or float number to a string. Decimal places can be configured via `decimal_digits`.
-    If the passed "value" is None, it will return `replacement`.
-    Attention: Will not localise the return value!
-    """
-    return intcomma(floatformat(value, decimal_digits)) if value is not None else replacement
-
-
-def string_or_none_to_string(value: Optional[any], replacement: str = "-") -> str:
-    """
-    Converts a given "value" to a string.
-    If the passed "value" is None, it will return `replacement`.
-    """
-    return value if value is not None else replacement
-
-
-def encode_to_xml(text: str) -> str:
-    """
-    Encodes ampersand, greater and lower characters in a given string to HTML-entities.
-    """
-    text_str = str(text)
-    text_str = text_str.replace('&', '&amp;')
-    text_str = text_str.replace('<', '&lt;')
-    text_str = text_str.replace('>', '&gt;')
-
-    return text_str
+import datetime
+import os
+from typing import Optional, Union
+
+from django.contrib.humanize.templatetags.humanize import intcomma
+from django.template.defaultfilters import floatformat, slugify
+from django.utils.encoding import smart_str
+
+from ai_django_core.utils import datetime_format
+
+
+def distinct(not_distinct_list: list) -> list:
+    """
+    Returns a list with no duplicate elements
+    """
+    return list(set(not_distinct_list))
+
+
+def slugify_file_name(file_name: str, length: int = 40) -> str:
+    """
+    Slugify the given file name
+    """
+    name, ext = os.path.splitext(file_name)
+    name = smart_str(slugify(name).replace('-', '_'))
+    ext = smart_str(slugify(ext))
+    result = '{}{}{}'.format(name[:length], "." if ext else "", ext)
+    return result
+
+
+def smart_truncate(text: str, max_length: int = 100, suffix: str = '...') -> str:
+    """
+    Returns a string of at most `max_length` characters, cutting
+    only at word-boundaries. If the string was truncated, `suffix`
+    will be appended.
+    In comparison to Djangos default filter `truncatechars` this method does NOT break words and you
+    can choose a custom suffix.
+    """
+    if text is None:
+        return ''
+
+    # Return the string itself if length is smaller or equal to the limit
+    if len(text) <= max_length:
+        return text
+
+    # Cut the string
+    value = text[:max_length]
+
+    # Break into words and remove the last
+    words = value.split(' ')[:-1]
+
+    # Join the words and return
+    return ' '.join(words) + suffix
+
+
+def float_to_string(value: Optional[float], replacement: str = "0,00") -> str:
+    """
+    Converts a float to a properly, German-formatted string value
+    # todo name is misleading, should contain "de"
+    # todo thousand separator would be nice
+    If the passed object is None, it will return `replacement`.
+    """
+    return ("%.2f" % value).replace('.', ',') if value is not None else replacement
+
+
+def date_to_string(value: Optional[datetime.date], replacement: str = "-", str_format: str = "%d.%m.%Y") -> str:
+    """
+    Converts a given date "value" to a string formatted with `str_format`.
+    If the passed "value" is None, it will return `replacement`.
+    """
+    return value.strftime(str_format) if value is not None else replacement
+
+
+def datetime_to_string(
+    value: Optional[datetime.datetime], replacement: str = "-", str_format: str = "%d.%m.%Y %H:%M"
+) -> str:
+    """
+    Converts a given datetime "value" to a string formatted with `str_format`.
+    If the passed "value" is None, it will return `replacement`.
+    """
+    return datetime_format(value, str_format) if value is not None else replacement
+
+
+def number_to_string(value: Optional[Union[int, float]], decimal_digits: int = 0, replacement: str = "-") -> str:
+    """
+    Converts a given int or float number to a string. Decimal places can be configured via `decimal_digits`.
+    If the passed "value" is None, it will return `replacement`.
+    Attention: Will not localise the return value!
+    """
+    return intcomma(floatformat(value, decimal_digits)) if value is not None else replacement
+
+
+def string_or_none_to_string(value: Optional[any], replacement: str = "-") -> str:
+    """
+    Converts a given "value" to a string.
+    If the passed "value" is None, it will return `replacement`.
+    """
+    return value if value is not None else replacement
+
+
+def encode_to_xml(text: str) -> str:
+    """
+    Encodes ampersand, greater and lower characters in a given string to HTML-entities.
+    """
+    text_str = str(text)
+    text_str = text_str.replace('&', '&amp;')
+    text_str = text_str.replace('<', '&lt;')
+    text_str = text_str.replace('>', '&gt;')
+
+    return text_str
```

### Comparing `ai-django-core-7.0.0/ai_django_core/view_layer/form_mixins.py` & `ai-django-core-7.0.1/ai_django_core/view_layer/form_mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/view_layer/formset_view_mixin.py` & `ai-django-core-7.0.1/ai_django_core/view_layer/formset_view_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/view_layer/htmx_mixins.py` & `ai-django-core-7.0.1/ai_django_core/view_layer/htmx_mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/view_layer/mixins.py` & `ai-django-core-7.0.1/ai_django_core/view_layer/mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/view_layer/tests/mixins.py` & `ai-django-core-7.0.1/ai_django_core/view_layer/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/ai_django_core/view_layer/views.py` & `ai-django-core-7.0.1/ai_django_core/view_layer/views.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/Makefile` & `ai-django-core-7.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/conf.py` & `ai-django-core-7.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/admin.md` & `ai-django-core-7.0.1/docs/features/admin.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/context_manager.md` & `ai-django-core-7.0.1/docs/features/context_manager.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/context_processors.md` & `ai-django-core-7.0.1/docs/features/context_processors.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/database_anonymisation.md` & `ai-django-core-7.0.1/docs/features/database_anonymisation.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/djangorestframework.md` & `ai-django-core-7.0.1/docs/features/djangorestframework.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/gitlab.md` & `ai-django-core-7.0.1/docs/features/gitlab.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/graphql.md` & `ai-django-core-7.0.1/docs/features/graphql.md`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,226 +1,226 @@
-# Graphene extension
-// todo Needs to be rewritten
-
-## GraphQL based on django ModelForms
-
-Here is a simple Django model in `my_app/models.py`:
-
-```python
-from django.db import models
-
-class User(models.Model):
-    first_name = models.CharField(max_length=100)
-    last_name = models.CharField(max_length=100)
-```
-
-Now we create a `ModelForm` in `my_app/forms.py`:
-
-```
-from django import forms
-from .models import User
-
-class UserForm(forms.ModelForm):
-    class Meta:
-        model = User
-        fields = ('first_name', 'last_name')
-```
-
- We need to create an `ObjectType` which we derive from our model.
- Lives in `my_apps/schemes/schematypes.py`:
-
-```
-from graphene_django import DjangoObjectType
-from ..models import User
-
-class UserType(DjangoObjectType):
-    class Meta:
-        model = User
-```
-
- Here's the mutation in `my_app/schema/mutations.py`.
- It takes a `ModelForm` (or a non-model form) to derive the validation rules from:
-
- ```
-import graphene
-from graphene_django_ai.forms.mutations import LoginRequiredDjangoModelFormMutation
-from .schematypes import UserType
-from ..forms import UserForm
-
-
-class UserCreateUpdateMutation(LoginRequiredDjangoModelFormMutation):
-    space = graphene.Field(UserType)
-
-    class Meta:
-        form_class = UserForm
-
-
-# Register new mutation
-class UserMutation(graphene.ObjectType):
-    spaces = UserCreateUpdateMutation.Field(description='Create and update users')
- ```
-
- If you register now your `UserMutation` in your schema you have a working model-based and DRY API
- endpoint. Congratulations!
-
-## DeleteMutation for django-model objects
-
-If you want to delete an object you can easily use the `DeleteMutation` like this:
-
-```python
-from graphene_django_ai.schemes.mutations import DeleteMutation
-from my_app.models import MyModel
-
-class MyModelDeleteMutation(DeleteMutation):
-    class Meta:
-        model = MyModel
-```
-
-If you are using `django-graphql-jwt` authentication you can ensure only logged in access to your delete endpoint like this:
-
-```python
-from graphene_django_ai.schemes.mutations import LoginRequiredDeleteMutation
-from my_app.models import MyModel
-
-class MyModelDeleteMutation(LoginRequiredDeleteMutation):
-    class Meta:
-        model = MyModel
-```
-
-If you need to customize the **validation** or the **base queryset** you can override methods like this:
-
-```python
-from graphene_django_ai.schemes.mutations import LoginRequiredDeleteMutation
-from graphql import GraphQLError
-from my_app.models import MyModel
-
-class MyModelDeleteMutation(LoginRequiredDeleteMutation):
-    class Meta:
-        model = MyModel
-
-    def validate(self, request):
-        if not request.user.is_superuser:
-            raise GraphQLError("This is only allowed for superusers!")
-
-    def get_queryset(self, request):
-        return self.model.objects.filter(created_by=request.user)
-```
-
-## JWT secure mutations
-
-If you derive your mutation from `LoginRequiredDjangoModelFormMutation` you don't have to manually take
-care about securing the login with the decorators.
-
-```python
-from graphene_django_ai.forms.mutations import LoginRequiredDjangoModelFormMutation
-class MyMutation(LoginRequiredDjangoModelFormMutation):
-    ...
-```
-
-## Testing GraphQL calls
-
-If you want to unittest your API calls derive your test case from the class `GraphQLTestCase`.
-
-Usage:
-
-```python
-import json
-
-from graphene_django.tests.base_test import GraphQLTestCase
-from my_project.config.schema import schema
-
-class MyFancyTestCase(GraphQLTestCase):
-
-    # Here you need to inject your test case's schema
-    GRAPHQL_SCHEMA = schema
-
-    def test_some_query(self):
-        response = self.query(
-            '''
-            query {
-                myModel {
-                    id
-                    name
-                }
-            }
-            ''',
-            op_name='myModel'
-        )
-        content = json.loads(response.content)
-        # This validates the status code and if you get errors
-        self.assertResponseNoErrors(response)
-
-        # Add some more asserts if you like
-        ...
-
-    def test_some_mutation(self):
-        response = self.query(
-            '''
-            mutation myMutation($input: MyMutationInput!) {
-                myMutation(input: $input) {
-                    my-model {
-                        id
-                        name
-                    }
-                }
-            }
-            ''',
-            op_name='myMutation',
-            input_data={'my_field': 'foo', 'other_field': 'bar'}
-        )
-        # This validates the status code and if you get errors
-        self.assertResponseNoErrors(response)
-
-        # Add some more asserts if you like
-        ...
-
-    def test_failing_call(self):
-
-       response = self.query(
-           '''
-           mutation myMutation($input: MyMutationInput!) {
-               myMutation(input: $badInput) {
-                   my-model {
-                       id
-                       name
-                   }
-               }
-           }
-           ''',
-           op_name='myMutation',
-           input_data={'my_field': 'foo', 'other_field': 'bar'}
-       )
-       # This assert tests if the call raised some errors
-       # For example if you want to test if invalid input is handled correctly by your endpoint
-       self.assertResponseHasErrors(response)
-
-       # Add some more asserts if you like
-       ...
-
-```
-
-## GraphQL with Sentry
-
-In some cases you might want to include Sentry while using a GraphQL API. This will probably lead to issues
-while using Graphene. This happens because Sentry sends the errors to Sentry as a string and not as error
-objects. Because of that all errors are combined and cannot be analyzed. You can use `SentryGraphQLView` for this case.
-
-> **Note**: You must use the following versions of libraries to use this feature!
-> * sentry_sdk >= 0.13.0
-> * graphene_django >=2.9.1, <3.0
-
-Usage:
-
-```python
-# urls.py
-from django.urls import path
-from django.views.decorators.csrf import csrf_exempt
-from ai_django_core.graphql.views import SentryGraphQLView
-from ai_django_core.graphql.utils import ignore_graphene_logger
-
-ignore_graphene_logger()    # <-- add this line at global level
-
-# change this line:
-path("graphql", csrf_exempt(GraphQLView.as_view(graphiql=True))),
-# to this:
-path("graphql", csrf_exempt(SentryGraphQLView.as_view(graphiql=True))),
-```
+# Graphene extension
+// todo Needs to be rewritten
+
+## GraphQL based on django ModelForms
+
+Here is a simple Django model in `my_app/models.py`:
+
+```python
+from django.db import models
+
+class User(models.Model):
+    first_name = models.CharField(max_length=100)
+    last_name = models.CharField(max_length=100)
+```
+
+Now we create a `ModelForm` in `my_app/forms.py`:
+
+```
+from django import forms
+from .models import User
+
+class UserForm(forms.ModelForm):
+    class Meta:
+        model = User
+        fields = ('first_name', 'last_name')
+```
+
+ We need to create an `ObjectType` which we derive from our model.
+ Lives in `my_apps/schemes/schematypes.py`:
+
+```
+from graphene_django import DjangoObjectType
+from ..models import User
+
+class UserType(DjangoObjectType):
+    class Meta:
+        model = User
+```
+
+ Here's the mutation in `my_app/schema/mutations.py`.
+ It takes a `ModelForm` (or a non-model form) to derive the validation rules from:
+
+ ```
+import graphene
+from graphene_django_ai.forms.mutations import LoginRequiredDjangoModelFormMutation
+from .schematypes import UserType
+from ..forms import UserForm
+
+
+class UserCreateUpdateMutation(LoginRequiredDjangoModelFormMutation):
+    space = graphene.Field(UserType)
+
+    class Meta:
+        form_class = UserForm
+
+
+# Register new mutation
+class UserMutation(graphene.ObjectType):
+    spaces = UserCreateUpdateMutation.Field(description='Create and update users')
+ ```
+
+ If you register now your `UserMutation` in your schema you have a working model-based and DRY API
+ endpoint. Congratulations!
+
+## DeleteMutation for django-model objects
+
+If you want to delete an object you can easily use the `DeleteMutation` like this:
+
+```python
+from graphene_django_ai.schemes.mutations import DeleteMutation
+from my_app.models import MyModel
+
+class MyModelDeleteMutation(DeleteMutation):
+    class Meta:
+        model = MyModel
+```
+
+If you are using `django-graphql-jwt` authentication you can ensure only logged in access to your delete endpoint like this:
+
+```python
+from graphene_django_ai.schemes.mutations import LoginRequiredDeleteMutation
+from my_app.models import MyModel
+
+class MyModelDeleteMutation(LoginRequiredDeleteMutation):
+    class Meta:
+        model = MyModel
+```
+
+If you need to customize the **validation** or the **base queryset** you can override methods like this:
+
+```python
+from graphene_django_ai.schemes.mutations import LoginRequiredDeleteMutation
+from graphql import GraphQLError
+from my_app.models import MyModel
+
+class MyModelDeleteMutation(LoginRequiredDeleteMutation):
+    class Meta:
+        model = MyModel
+
+    def validate(self, request):
+        if not request.user.is_superuser:
+            raise GraphQLError("This is only allowed for superusers!")
+
+    def get_queryset(self, request):
+        return self.model.objects.filter(created_by=request.user)
+```
+
+## JWT secure mutations
+
+If you derive your mutation from `LoginRequiredDjangoModelFormMutation` you don't have to manually take
+care about securing the login with the decorators.
+
+```python
+from graphene_django_ai.forms.mutations import LoginRequiredDjangoModelFormMutation
+class MyMutation(LoginRequiredDjangoModelFormMutation):
+    ...
+```
+
+## Testing GraphQL calls
+
+If you want to unittest your API calls derive your test case from the class `GraphQLTestCase`.
+
+Usage:
+
+```python
+import json
+
+from graphene_django.tests.base_test import GraphQLTestCase
+from my_project.config.schema import schema
+
+class MyFancyTestCase(GraphQLTestCase):
+
+    # Here you need to inject your test case's schema
+    GRAPHQL_SCHEMA = schema
+
+    def test_some_query(self):
+        response = self.query(
+            '''
+            query {
+                myModel {
+                    id
+                    name
+                }
+            }
+            ''',
+            op_name='myModel'
+        )
+        content = json.loads(response.content)
+        # This validates the status code and if you get errors
+        self.assertResponseNoErrors(response)
+
+        # Add some more asserts if you like
+        ...
+
+    def test_some_mutation(self):
+        response = self.query(
+            '''
+            mutation myMutation($input: MyMutationInput!) {
+                myMutation(input: $input) {
+                    my-model {
+                        id
+                        name
+                    }
+                }
+            }
+            ''',
+            op_name='myMutation',
+            input_data={'my_field': 'foo', 'other_field': 'bar'}
+        )
+        # This validates the status code and if you get errors
+        self.assertResponseNoErrors(response)
+
+        # Add some more asserts if you like
+        ...
+
+    def test_failing_call(self):
+
+       response = self.query(
+           '''
+           mutation myMutation($input: MyMutationInput!) {
+               myMutation(input: $badInput) {
+                   my-model {
+                       id
+                       name
+                   }
+               }
+           }
+           ''',
+           op_name='myMutation',
+           input_data={'my_field': 'foo', 'other_field': 'bar'}
+       )
+       # This assert tests if the call raised some errors
+       # For example if you want to test if invalid input is handled correctly by your endpoint
+       self.assertResponseHasErrors(response)
+
+       # Add some more asserts if you like
+       ...
+
+```
+
+## GraphQL with Sentry
+
+In some cases you might want to include Sentry while using a GraphQL API. This will probably lead to issues
+while using Graphene. This happens because Sentry sends the errors to Sentry as a string and not as error
+objects. Because of that all errors are combined and cannot be analyzed. You can use `SentryGraphQLView` for this case.
+
+> **Note**: You must use the following versions of libraries to use this feature!
+> * sentry_sdk >= 0.13.0
+> * graphene_django >=2.9.1, <3.0
+
+Usage:
+
+```python
+# urls.py
+from django.urls import path
+from django.views.decorators.csrf import csrf_exempt
+from ai_django_core.graphql.views import SentryGraphQLView
+from ai_django_core.graphql.utils import ignore_graphene_logger
+
+ignore_graphene_logger()    # <-- add this line at global level
+
+# change this line:
+path("graphql", csrf_exempt(GraphQLView.as_view(graphiql=True))),
+# to this:
+path("graphql", csrf_exempt(SentryGraphQLView.as_view(graphiql=True))),
+```
```

### Comparing `ai-django-core-7.0.0/docs/features/mail.md` & `ai-django-core-7.0.1/docs/features/mail.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,238 +1,238 @@
-# Mailing
-
-## Backends
-
-### WhitelistEmailBackend
-
-In some cases it is useful to debug and test email functionality on local or test environments. Additionally, your
-project could contain logic, that triggers emails in the background, so it is very important, that you don't send emails
-to other domains, e.g. 'xyz@test.de' or to other test users with another domain, by accident.
-
-This email backend can be used as Django EMAIL_BACKEND to restrict outgoing emails to a set of allowed domains. You can
-define an email address (must be a catchall inbox), where the restricted emails should be redirected to.
-
-Example:
-
-    EMAIL_BACKEND = 'ai_django_core.mail.backends.whitelist_smtp.WhitelistEmailBackend'
-    EMAIL_BACKEND_DOMAIN_WHITELIST = ['ambient.digital']
-    EMAIL_BACKEND_REDIRECT_ADDRESS = '%s@testuser.ambient.digital'
-
-If EMAIL_BACKEND_REDIRECT_ADDRESS is configured, an email to 'albertus.magnus@example.com' will be redirected to:
-albertus.magnus_example.com@testuser.ambient.digital
-
-## Class-based Emails
-
-This package contains an approach called "class-based emails". Similar to class-based views in django (in comparison to
-function-based ones), you can now implement your email as a class and use all the benefits of object-orientated
-programming like fiddling around with functions and all the non-DRY repetition of code you'll usually end up with.
-
-USPs:
-
-* Better structure and advantages of object-orientated programming over handling multiple functions!
-* Quick and fast creation of new emails - only worry about the things you have to think about!
-* No code redundancy for setting up the default mail configuration - all wrapped in the class!
-* The text part of the email can be automatically rendered from the HTML part - no redundant templates anymore!
-* Built-in (and extendable) sanity checks as a validation for forgotten variables!
-* Clean and easy solution for email attachments
-
-There are two scenarios covered by this package:
-
-* **Single mail**: Create a single email through a class to utilise benefits of object-orientation.
-* **Similar mails**: Create a bunch of similar emails with a factory class, for example if you want to send the same
-  content but with a personal salutation to a number of people.
-
-### Create a single email
-
-Imagine you want to send a single email to a given user or to the system admins. Instead of having to deal with how to
-end an email and worry about if the ``to`` field requires a list or string of emails... look at this example:
-
-````
-from ai_django_core.mail.services.base import BaseEmailService
-
-class MyFancyClassBasedMail(BaseEmailService):
-    """
-    Send an email to my admins to inform them about something important.
-    """
-    subject = _('Heads up, admins!')
-    template_name = 'email/my_fancy_class_based_email.html'
-
-    def get_context_data(self):
-        data = super().get_context_data()
-        data['my_variable'] = ...
-        return data
-````
-
-This is a simple example of how to create an email. We pass or set the recipients in the `__init__()` method and can add
-more data in the `get_context_data()` - or just provide the context on creation as a parameter.
-
-One big advantage is that you can create your own base class which handles all the context data you need to have for
-your base email template. Imagine you have an unsubscribe link or a logo in the base template. In the "old world"
-you have to think to pass these variables every time. Now, just wrap it up in a base class and that's it!
-
-And that is how you would send the email:
-
-````
-from django.conf import settings
-
-email_service = MyFancyClassBasedMail(settings.MY_ADMIN_EMAIL_ADDRESS)
-email_service.process()
-````
-
-Optionally you can set the class attribute ``template_txt_name`` to define a plain text template. If not set, the HTML
-part will be used to render the plain text body.
-
-#### Configuration
-
-You can set a subject prefix, so that all your emails look more similar when setting the constant ``SUBJECT_PREFIX``.
-
-If you wish to define a custom "from" email, you can do so via the ``FROM_EMAIL`` constant. Take care:
-If you do not set it, the ``DEFAULT_FROM_EMAIL`` variable from the django settings is used.
-
-#### Public method overview
-
-* `__init__(recipient_email_list: Union[list, str] = None, context_data: dict = None)`
-  Takes a list of recipient email addresses or just a single email address as a string and optionally some context data.
-  `recipient_email_list` might be none, because you could set the variable statically in the class definition.
-
-
-* ``get_context_data()``
-  Similar to django CBVs known method, you can extend here the ``context_data`` provided in the `__init__()`.
-
-
-* ``get_subject()``
-  This method combines the constant ``SUBJECT_PREFIX`` with the variable `subject`. Can be overwritten, if required.
-
-
-* ``get_from_email()``
-  Returns the email address the mail should be sent from. Will take the django settings variable ``DEFAULT_FROM_EMAIL``
-  if the constant ``FROM_EMAIL`` in the class is not set.
-
-
-* ``get_reply_to_email()``
-  Returns the content of constant ``REPLY_TO_ADDRESS``. If this constant is not set, there will be no "reply-to" data in
-  the email.
-
-
-* ``get_cc_to_email()``
-  Returns the content of class variable ``cc_email_list_``. Any email address returned by this method will be used in
-  the "CC" field of the generated email. This variable can be set anywhere within the class
-  (preferably in the `__init__` method) or this method can be overwritten for custom behaviour.
-
-
-* ``get_bcc_to_email()``
-  Returns the content of class variable ``bcc_email_list_``. Any email address returned by this method will be used in
-  the "CC" field of the generated email. This variable can be set anywhere within the class
-  (preferably in the `__init__` method) or this method can be overwritten for custom behaviour.
-
-
-* ``get_translation()``
-  Tries to parse the language from the django settings variable ``LANGUAGE_CODE``. Can be overwritten to set a language
-  manually. Needs to return either `None` or a two-character language code like `en` or `de`. If this method returns
-  `None`, translation will be deactivated. Translations are needed for localised values like getting the current month
-  from a date (in the correct language).
-
-* ``get_attachments()``
-  This method returns a list of paths to a locally-stored file. Can automatically be filled by passing the kwarg
-  `attachment_list` in the constructor. Each file of the given list will be attached to the newly created email.
-
-* ``has_errors()``
-  If ``is_valid()`` is called with the keyword argument `raise_exception=False`, the configuration errors are not raised
-  but stored internally. This method checks if any errors occurred. If you need the explicit errors, you can fetch them
-  via the ``errors`` property.
-
-
-* ``process()``
-  Executes the actual sending. Not recommended to change.
-
-### Create multiple similar emails
-
-Imagine you want to inform a couple of users about something that happened in your system, for example a successful
-transaction or a report generated by your application. You would have a very similar mail body except for the salutation
-or one or two minor differences. Handling this with the single email class from above feels a little off.
-
-That is why this package provides a mail factory! This factory is a wrapper for creating similar emails and providing
-the email class shown above with recipient-specific content.
-
-Look at this example:
-
-``````
-class MyFancyMail(BaseEmailService):
-    subject = _('I am a great email!')
-    template_name = 'email/my_fancy_email.html'
-
-
-class MyFancyMailFactory(BaseEmailServiceFactory):
-    service_class = MyFancyMail
-
-    def __init__(self, action_id: int, recipient_email_list: list = None):
-        super().__init__(recipient_email_list)
-        self.action = Action.objects.filter(id=action_id).first()
-
-    def get_recipient_list(self) -> list:
-        return self.action.fetch_recipients_for_this_action()
-
-    def get_email_from_recipient(self, recipient) -> str:
-        if isinstance(recipient, User):
-            return recipient.email
-        return recipient
-
-    def is_valid(self):
-        if not self.action:
-            raise EmailServiceConfigError('No action provided.')
-
-        return super().is_valid()
-
-    def get_context_data(self):
-        context = super().get_context_data()
-        context.update({
-            'action': self.action,
-        })
-        return context
-``````
-
-This is only one of many (!) possibilities to handle a case like described above. We pass a custom action id to the
-factory and fetch the given action (this might be a project, a report, a record...) and set it to a class attribute.
-
-The ``get_recipient_list()`` method fetches the recipients based on the action we are looking at right now.
-
-Because we might get mixed results (mostly not, but just to show what is possible), we overwrite the method
-``get_email_from_recipient()`` to be able to handle simple email addresses as a string or user objects. If you pass only
-strings, overwriting this method can be omitted.
-
-We add a sanity check in the ``is_valid()`` method to be sure that nobody tries to create emails like this without an
-action being set.
-
-Finally, we add the action to the context data ``get_context_data()`` so the `MyFancyMail()` class can use it.
-
-Now for every recipient an instance of ``MyFancyMail()`` will be created. Now it is no problem, handling the salutation
-or any other recipient-specific content within the "real" mail class. Only make sure that the factory provides all the
-required data.
-
-### Attachments
-
-If you want to attach a number of files to your emails, you can do this in two ways.
-
-The simple way is passing an absolute file path to the constructor of the service:
-
-````
-email_service = MyMailService(
-  ...
-  attachment_list=[my_file_1, my_file_2]
-)
-````
-
-If you want to customise the filename or even pass a mimetype, you can do as follows:
-
-````
-email_service = MyMailService(
-  ...
-  attachment_list=[{'filename': 'my_fancy_file.json', 'file': file_content, 'mimetype': 'application/json'}]
-)
-````
-
-Please note that here the file content, not the file path, needs to be passed to the attachment list. If anything goes
-sideways, the service will throw an `EmailServiceAttachmentError` exception.
-
-## Testing emails
-
-If you are curious about how to properly test your emails, have a look at the testing section.
+# Mailing
+
+## Backends
+
+### WhitelistEmailBackend
+
+In some cases it is useful to debug and test email functionality on local or test environments. Additionally, your
+project could contain logic, that triggers emails in the background, so it is very important, that you don't send emails
+to other domains, e.g. 'xyz@test.de' or to other test users with another domain, by accident.
+
+This email backend can be used as Django EMAIL_BACKEND to restrict outgoing emails to a set of allowed domains. You can
+define an email address (must be a catchall inbox), where the restricted emails should be redirected to.
+
+Example:
+
+    EMAIL_BACKEND = 'ai_django_core.mail.backends.whitelist_smtp.WhitelistEmailBackend'
+    EMAIL_BACKEND_DOMAIN_WHITELIST = ['ambient.digital']
+    EMAIL_BACKEND_REDIRECT_ADDRESS = '%s@testuser.ambient.digital'
+
+If EMAIL_BACKEND_REDIRECT_ADDRESS is configured, an email to 'albertus.magnus@example.com' will be redirected to:
+albertus.magnus_example.com@testuser.ambient.digital
+
+## Class-based Emails
+
+This package contains an approach called "class-based emails". Similar to class-based views in django (in comparison to
+function-based ones), you can now implement your email as a class and use all the benefits of object-orientated
+programming like fiddling around with functions and all the non-DRY repetition of code you'll usually end up with.
+
+USPs:
+
+* Better structure and advantages of object-orientated programming over handling multiple functions!
+* Quick and fast creation of new emails - only worry about the things you have to think about!
+* No code redundancy for setting up the default mail configuration - all wrapped in the class!
+* The text part of the email can be automatically rendered from the HTML part - no redundant templates anymore!
+* Built-in (and extendable) sanity checks as a validation for forgotten variables!
+* Clean and easy solution for email attachments
+
+There are two scenarios covered by this package:
+
+* **Single mail**: Create a single email through a class to utilise benefits of object-orientation.
+* **Similar mails**: Create a bunch of similar emails with a factory class, for example if you want to send the same
+  content but with a personal salutation to a number of people.
+
+### Create a single email
+
+Imagine you want to send a single email to a given user or to the system admins. Instead of having to deal with how to
+end an email and worry about if the ``to`` field requires a list or string of emails... look at this example:
+
+````
+from ai_django_core.mail.services.base import BaseEmailService
+
+class MyFancyClassBasedMail(BaseEmailService):
+    """
+    Send an email to my admins to inform them about something important.
+    """
+    subject = _('Heads up, admins!')
+    template_name = 'email/my_fancy_class_based_email.html'
+
+    def get_context_data(self):
+        data = super().get_context_data()
+        data['my_variable'] = ...
+        return data
+````
+
+This is a simple example of how to create an email. We pass or set the recipients in the `__init__()` method and can add
+more data in the `get_context_data()` - or just provide the context on creation as a parameter.
+
+One big advantage is that you can create your own base class which handles all the context data you need to have for
+your base email template. Imagine you have an unsubscribe link or a logo in the base template. In the "old world"
+you have to think to pass these variables every time. Now, just wrap it up in a base class and that's it!
+
+And that is how you would send the email:
+
+````
+from django.conf import settings
+
+email_service = MyFancyClassBasedMail(settings.MY_ADMIN_EMAIL_ADDRESS)
+email_service.process()
+````
+
+Optionally you can set the class attribute ``template_txt_name`` to define a plain text template. If not set, the HTML
+part will be used to render the plain text body.
+
+#### Configuration
+
+You can set a subject prefix, so that all your emails look more similar when setting the constant ``SUBJECT_PREFIX``.
+
+If you wish to define a custom "from" email, you can do so via the ``FROM_EMAIL`` constant. Take care:
+If you do not set it, the ``DEFAULT_FROM_EMAIL`` variable from the django settings is used.
+
+#### Public method overview
+
+* `__init__(recipient_email_list: Union[list, str] = None, context_data: dict = None)`
+  Takes a list of recipient email addresses or just a single email address as a string and optionally some context data.
+  `recipient_email_list` might be none, because you could set the variable statically in the class definition.
+
+
+* ``get_context_data()``
+  Similar to django CBVs known method, you can extend here the ``context_data`` provided in the `__init__()`.
+
+
+* ``get_subject()``
+  This method combines the constant ``SUBJECT_PREFIX`` with the variable `subject`. Can be overwritten, if required.
+
+
+* ``get_from_email()``
+  Returns the email address the mail should be sent from. Will take the django settings variable ``DEFAULT_FROM_EMAIL``
+  if the constant ``FROM_EMAIL`` in the class is not set.
+
+
+* ``get_reply_to_email()``
+  Returns the content of constant ``REPLY_TO_ADDRESS``. If this constant is not set, there will be no "reply-to" data in
+  the email.
+
+
+* ``get_cc_to_email()``
+  Returns the content of class variable ``cc_email_list_``. Any email address returned by this method will be used in
+  the "CC" field of the generated email. This variable can be set anywhere within the class
+  (preferably in the `__init__` method) or this method can be overwritten for custom behaviour.
+
+
+* ``get_bcc_to_email()``
+  Returns the content of class variable ``bcc_email_list_``. Any email address returned by this method will be used in
+  the "CC" field of the generated email. This variable can be set anywhere within the class
+  (preferably in the `__init__` method) or this method can be overwritten for custom behaviour.
+
+
+* ``get_translation()``
+  Tries to parse the language from the django settings variable ``LANGUAGE_CODE``. Can be overwritten to set a language
+  manually. Needs to return either `None` or a two-character language code like `en` or `de`. If this method returns
+  `None`, translation will be deactivated. Translations are needed for localised values like getting the current month
+  from a date (in the correct language).
+
+* ``get_attachments()``
+  This method returns a list of paths to a locally-stored file. Can automatically be filled by passing the kwarg
+  `attachment_list` in the constructor. Each file of the given list will be attached to the newly created email.
+
+* ``has_errors()``
+  If ``is_valid()`` is called with the keyword argument `raise_exception=False`, the configuration errors are not raised
+  but stored internally. This method checks if any errors occurred. If you need the explicit errors, you can fetch them
+  via the ``errors`` property.
+
+
+* ``process()``
+  Executes the actual sending. Not recommended to change.
+
+### Create multiple similar emails
+
+Imagine you want to inform a couple of users about something that happened in your system, for example a successful
+transaction or a report generated by your application. You would have a very similar mail body except for the salutation
+or one or two minor differences. Handling this with the single email class from above feels a little off.
+
+That is why this package provides a mail factory! This factory is a wrapper for creating similar emails and providing
+the email class shown above with recipient-specific content.
+
+Look at this example:
+
+``````
+class MyFancyMail(BaseEmailService):
+    subject = _('I am a great email!')
+    template_name = 'email/my_fancy_email.html'
+
+
+class MyFancyMailFactory(BaseEmailServiceFactory):
+    service_class = MyFancyMail
+
+    def __init__(self, action_id: int, recipient_email_list: list = None):
+        super().__init__(recipient_email_list)
+        self.action = Action.objects.filter(id=action_id).first()
+
+    def get_recipient_list(self) -> list:
+        return self.action.fetch_recipients_for_this_action()
+
+    def get_email_from_recipient(self, recipient) -> str:
+        if isinstance(recipient, User):
+            return recipient.email
+        return recipient
+
+    def is_valid(self):
+        if not self.action:
+            raise EmailServiceConfigError('No action provided.')
+
+        return super().is_valid()
+
+    def get_context_data(self):
+        context = super().get_context_data()
+        context.update({
+            'action': self.action,
+        })
+        return context
+``````
+
+This is only one of many (!) possibilities to handle a case like described above. We pass a custom action id to the
+factory and fetch the given action (this might be a project, a report, a record...) and set it to a class attribute.
+
+The ``get_recipient_list()`` method fetches the recipients based on the action we are looking at right now.
+
+Because we might get mixed results (mostly not, but just to show what is possible), we overwrite the method
+``get_email_from_recipient()`` to be able to handle simple email addresses as a string or user objects. If you pass only
+strings, overwriting this method can be omitted.
+
+We add a sanity check in the ``is_valid()`` method to be sure that nobody tries to create emails like this without an
+action being set.
+
+Finally, we add the action to the context data ``get_context_data()`` so the `MyFancyMail()` class can use it.
+
+Now for every recipient an instance of ``MyFancyMail()`` will be created. Now it is no problem, handling the salutation
+or any other recipient-specific content within the "real" mail class. Only make sure that the factory provides all the
+required data.
+
+### Attachments
+
+If you want to attach a number of files to your emails, you can do this in two ways.
+
+The simple way is passing an absolute file path to the constructor of the service:
+
+````
+email_service = MyMailService(
+  ...
+  attachment_list=[my_file_1, my_file_2]
+)
+````
+
+If you want to customise the filename or even pass a mimetype, you can do as follows:
+
+````
+email_service = MyMailService(
+  ...
+  attachment_list=[{'filename': 'my_fancy_file.json', 'file': file_content, 'mimetype': 'application/json'}]
+)
+````
+
+Please note that here the file content, not the file path, needs to be passed to the attachment list. If anything goes
+sideways, the service will throw an `EmailServiceAttachmentError` exception.
+
+## Testing emails
+
+If you are curious about how to properly test your emails, have a look at the testing section.
```

### Comparing `ai-django-core-7.0.0/docs/features/managers.md` & `ai-django-core-7.0.1/docs/features/managers.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/mixins.md` & `ai-django-core-7.0.1/docs/features/mixins.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/models.md` & `ai-django-core-7.0.1/docs/features/models.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/selectors.md` & `ai-django-core-7.0.1/docs/features/selectors.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/services.md` & `ai-django-core-7.0.1/docs/features/services.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/setup.md` & `ai-django-core-7.0.1/docs/features/setup.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-# Setup
-
-## Default installation
-
-Setting up and getting started with this toolbox is very simple. At first make sure you are installing the latest
-version of `ai-django-core`:
-
-* Installation via pip:
-
-  `pip install -U ai-django-core`
-
-* Installation via pipenv:
-
-  `pipenv install ai-django-core`
-
-Afterwards, include the package in your ``INSTALLED_APPS`` within your main
-[django settings file](https://docs.djangoproject.com/en/dev/ref/settings/#std:setting-INSTALLED_APPS):
-
-````
-INSTALLED_APPS = (
-    ...
-    'ai_django_core',
-)
- ````
-
-## Installing the djangorestframework extension
-
-If you wish to use the extensions for [djangorestframework](https://www.django-rest-framework.org/), simply install the
-toolbox with the desired extension:
-
-* Installation via pip:
-
-  `pip install -U ai-django-core[drf]`
-
-* Installation via pipenv:
-
-  `pipenv install ai-django-core[drf]`
-
-## Installing the GraphQL extension
-
-If you wish to use the extensions for [django-graphene](https://pypi.org/project/graphene-django/), simply install the
-toolbox with the desired extension:
-
-* Installation via pip:
-
-  `pip install -U ai-django-core[graphql]`
-
-* Installation via pipenv:
-
-  `pipenv install ai-django-core[graphql]`
-
-# Installing multiple extensions
-
-In the case that you want to install more than one extension, just chain the extension with a comma:
-
-* Installation via pip:
-
-  `pip install -U ai-django-core[drf,graphql]`
-
-* Installation via pipenv:
-
-  `pipenv install ai-django-core[drf,graphql]`
+# Setup
+
+## Default installation
+
+Setting up and getting started with this toolbox is very simple. At first make sure you are installing the latest
+version of `ai-django-core`:
+
+* Installation via pip:
+
+  `pip install -U ai-django-core`
+
+* Installation via pipenv:
+
+  `pipenv install ai-django-core`
+
+Afterwards, include the package in your ``INSTALLED_APPS`` within your main
+[django settings file](https://docs.djangoproject.com/en/dev/ref/settings/#std:setting-INSTALLED_APPS):
+
+````
+INSTALLED_APPS = (
+    ...
+    'ai_django_core',
+)
+ ````
+
+## Installing the djangorestframework extension
+
+If you wish to use the extensions for [djangorestframework](https://www.django-rest-framework.org/), simply install the
+toolbox with the desired extension:
+
+* Installation via pip:
+
+  `pip install -U ai-django-core[drf]`
+
+* Installation via pipenv:
+
+  `pipenv install ai-django-core[drf]`
+
+## Installing the GraphQL extension
+
+If you wish to use the extensions for [django-graphene](https://pypi.org/project/graphene-django/), simply install the
+toolbox with the desired extension:
+
+* Installation via pip:
+
+  `pip install -U ai-django-core[graphql]`
+
+* Installation via pipenv:
+
+  `pipenv install ai-django-core[graphql]`
+
+# Installing multiple extensions
+
+In the case that you want to install more than one extension, just chain the extension with a comma:
+
+* Installation via pip:
+
+  `pip install -U ai-django-core[drf,graphql]`
+
+* Installation via pipenv:
+
+  `pipenv install ai-django-core[drf,graphql]`
```

### Comparing `ai-django-core-7.0.0/docs/features/tests.md` & `ai-django-core-7.0.1/docs/features/tests.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/utils/cache.md` & `ai-django-core-7.0.1/docs/features/utils/cache.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/utils/date.md` & `ai-django-core-7.0.1/docs/features/utils/date.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/utils/math.md` & `ai-django-core-7.0.1/docs/features/utils/math.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/utils/model.md` & `ai-django-core-7.0.1/docs/features/utils/model.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/utils/named_tuple.md` & `ai-django-core-7.0.1/docs/features/utils/named_tuple.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/utils/string.md` & `ai-django-core-7.0.1/docs/features/utils/string.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/features/view-layer.md` & `ai-django-core-7.0.1/docs/features/view-layer.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/index.rst` & `ai-django-core-7.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/docs/make.bat` & `ai-django-core-7.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/manage.py` & `ai-django-core-7.0.1/manage.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/pyproject.toml` & `ai-django-core-7.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/settings.py` & `ai-django-core-7.0.1/settings.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from pathlib import Path
-
-BASE_PATH = Path(__file__).resolve(strict=True).parent
-
-INSTALLED_APPS = (
-    'django.contrib.admin',
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.messages',
-    'django.contrib.staticfiles',
-    'testapp',
-)
-
-DEBUG = False
-
-ALLOWED_HOSTS = ['localhost:8000']
-
-SECRET_KEY = 'ASDFjklö123456890'
-
-# Routing
-ROOT_URLCONF = 'testapp.urls'
-
-DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
-
-DATABASES = {
-    'default': {
-        'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': 'db.sqlite',
-    }
-}
-
-TEMPLATES = [
-    {
-        'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'DIRS': ['templates'],
-        'APP_DIRS': True,
-        'OPTIONS': {
-            'context_processors': [
-                'django.template.context_processors.debug',
-                'django.template.context_processors.request',
-                'django.contrib.auth.context_processors.auth',
-                'django.contrib.messages.context_processors.messages',
-            ],
-            'debug': True,
-        },
-    },
-]
-
-MIDDLEWARE = (
-    'django.middleware.security.SecurityMiddleware',
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.middleware.common.CommonMiddleware',
-    'django.middleware.csrf.CsrfViewMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
-    'django.middleware.clickjacking.XFrameOptionsMiddleware',
-)
-
-# Mail backend
-EMAIL_BACKEND_DOMAIN_WHITELIST = ''
-EMAIL_BACKEND_REDIRECT_ADDRESS = ''
-
-TIME_ZONE = 'UTC'
-
-LOCALE_PATHS = [str(BASE_PATH) + '/ai_django_core/locale']
+from pathlib import Path
+
+BASE_PATH = Path(__file__).resolve(strict=True).parent
+
+INSTALLED_APPS = (
+    'django.contrib.admin',
+    'django.contrib.auth',
+    'django.contrib.contenttypes',
+    'django.contrib.sessions',
+    'django.contrib.messages',
+    'django.contrib.staticfiles',
+    'testapp',
+)
+
+DEBUG = False
+
+ALLOWED_HOSTS = ['localhost:8000']
+
+SECRET_KEY = 'ASDFjklö123456890'
+
+# Routing
+ROOT_URLCONF = 'testapp.urls'
+
+DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
+
+DATABASES = {
+    'default': {
+        'ENGINE': 'django.db.backends.sqlite3',
+        'NAME': 'db.sqlite',
+    }
+}
+
+TEMPLATES = [
+    {
+        'BACKEND': 'django.template.backends.django.DjangoTemplates',
+        'DIRS': ['templates'],
+        'APP_DIRS': True,
+        'OPTIONS': {
+            'context_processors': [
+                'django.template.context_processors.debug',
+                'django.template.context_processors.request',
+                'django.contrib.auth.context_processors.auth',
+                'django.contrib.messages.context_processors.messages',
+            ],
+            'debug': True,
+        },
+    },
+]
+
+MIDDLEWARE = (
+    'django.middleware.security.SecurityMiddleware',
+    'django.contrib.sessions.middleware.SessionMiddleware',
+    'django.middleware.common.CommonMiddleware',
+    'django.middleware.csrf.CsrfViewMiddleware',
+    'django.contrib.auth.middleware.AuthenticationMiddleware',
+    'django.contrib.messages.middleware.MessageMiddleware',
+    'django.middleware.clickjacking.XFrameOptionsMiddleware',
+)
+
+# Mail backend
+EMAIL_BACKEND_DOMAIN_WHITELIST = ''
+EMAIL_BACKEND_REDIRECT_ADDRESS = ''
+
+TIME_ZONE = 'UTC'
+
+LOCALE_PATHS = [str(BASE_PATH) + '/ai_django_core/locale']
```

### Comparing `ai-django-core-7.0.0/testapp/api/views.py` & `ai-django-core-7.0.1/testapp/api/views.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/testapp/migrations/0001_initial.py` & `ai-django-core-7.0.1/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/testapp/migrations/0002_auto_210407.py` & `ai-django-core-7.0.1/testapp/migrations/0002_auto_210407.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/testapp/migrations/0003_modelwithfktoself.py` & `ai-django-core-7.0.1/testapp/migrations/0003_modelwithfktoself.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/testapp/migrations/0004_auto_20210511_1343.py` & `ai-django-core-7.0.1/testapp/migrations/0004_auto_20210511_1343.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/testapp/migrations/0005_modelwithcleanmixin.py` & `ai-django-core-7.0.1/testapp/migrations/0005_modelwithcleanmixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/testapp/migrations/0006_modelwithselector.py` & `ai-django-core-7.0.1/testapp/migrations/0006_modelwithselector.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/testapp/migrations/0007_modelwithsavewithoutsignals.py` & `ai-django-core-7.0.1/testapp/migrations/0007_modelwithsavewithoutsignals.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/testapp/models.py` & `ai-django-core-7.0.1/testapp/models.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/testapp/templates/403.html` & `ai-django-core-7.0.1/testapp/templates/403.html`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-{% load i18n static %}
-
-<!DOCTYPE html>
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
-<head>
-    <meta content="text/html; charset=utf-8" http-equiv="Content-Type">
-    <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0">
-
-    <title>403 - Forbidden</title>
-    <style type="text/css">
-        html, body {
-            height: 100%;
-            margin: 0;
-            padding: 0;
-            font-family: Helvetica, sans-serif;
-            color: #595959;
-            font-size: 1.2em;
-        }
-
-        h1 {
-            display: none;
-        }
-
-        .container {
-            position: relative;
-            height: 100%;
-            width: 100%;
-        }
-
-        .image-container {
-            position: absolute;
-            top: 50%;
-            left: 50%;
-            transform: translate(-50%, -50%);
-        }
-
-        .image-container > p {
-            position: absolute;
-            width: auto;
-            white-space: nowrap;
-        }
-
-        .image-container > p.error-msg {
-            left: 19em;
-            bottom: 5em;
-        }
-    </style>
-</head>
-
-<body>
-{% block body %}
-    <div class="container">
-        <h1>{% trans "Error 403" %}</h1>
-        <div class="image-container">
-            <p class="error-msg">You don't have access to this page.</p>
-        </div>
-    </div>
-{% endblock %}
-</body>
+{% load i18n static %}
+
+<!DOCTYPE html>
+<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
+<head>
+    <meta content="text/html; charset=utf-8" http-equiv="Content-Type">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0">
+
+    <title>403 - Forbidden</title>
+    <style type="text/css">
+        html, body {
+            height: 100%;
+            margin: 0;
+            padding: 0;
+            font-family: Helvetica, sans-serif;
+            color: #595959;
+            font-size: 1.2em;
+        }
+
+        h1 {
+            display: none;
+        }
+
+        .container {
+            position: relative;
+            height: 100%;
+            width: 100%;
+        }
+
+        .image-container {
+            position: absolute;
+            top: 50%;
+            left: 50%;
+            transform: translate(-50%, -50%);
+        }
+
+        .image-container > p {
+            position: absolute;
+            width: auto;
+            white-space: nowrap;
+        }
+
+        .image-container > p.error-msg {
+            left: 19em;
+            bottom: 5em;
+        }
+    </style>
+</head>
+
+<body>
+{% block body %}
+    <div class="container">
+        <h1>{% trans "Error 403" %}</h1>
+        <div class="image-container">
+            <p class="error-msg">You don't have access to this page.</p>
+        </div>
+    </div>
+{% endblock %}
+</body>
```

### Comparing `ai-django-core-7.0.0/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py` & `ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py` & `ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py` & `ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py` & `ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py` & `ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-from unittest import mock
-
-from django.contrib import admin
-from django.contrib.auth.models import User
-from django.http import HttpResponseRedirect
-from django.test import TestCase
-
-from ai_django_core.admin.model_admins.mixins import DeactivatableChangeViewAdminMixin
-from ai_django_core.tests.mixins import RequestProviderMixin
-
-
-class TestAdmin(DeactivatableChangeViewAdminMixin, admin.ModelAdmin):
-    pass
-
-
-class DeactivatableChangeViewAdminMixinTest(RequestProviderMixin, TestCase):
-    @classmethod
-    def setUpTestData(cls):
-        super().setUpTestData()
-
-        # Use random model for this meta test
-        cls.user = User.objects.create(username="test_user", is_superuser=False)
-        cls.super_user = User.objects.create(username="super_user", is_superuser=True)
-
-    def test_can_see_change_view_positive_flag(self):
-        admin_cls = TestAdmin(admin_site=None, model=User)
-        self.assertTrue(admin_cls.can_see_change_view(request=self.get_request()))
-
-    def test_can_see_change_view_negative_flag(self):
-        admin_cls = TestAdmin(admin_site=None, model=User)
-        admin_cls.enable_change_view = False
-        self.assertFalse(admin_cls.can_see_change_view(request=self.get_request()))
-
-    def test_get_list_display_links_can_see_method_called(self):
-        admin_cls = TestAdmin(admin_site=None, model=User)
-        with mock.patch.object(admin_cls, 'can_see_change_view', return_value=True) as mock_method:
-            admin_cls.get_list_display_links(request=self.get_request(user=self.user), list_display=('first_name',))
-
-        mock_method.assert_called_once()
-
-    def test_get_list_display_links_can_see_method_positive_flag(self):
-        admin_cls = TestAdmin(admin_site=None, model=User)
-        field_tuple = ('first_name',)
-        self.assertEqual(
-            list(field_tuple),
-            admin_cls.get_list_display_links(request=self.get_request(user=self.user), list_display=field_tuple),
-        )
-
-    def test_get_list_display_links_can_see_method_negative_flag(self):
-        admin_cls = TestAdmin(admin_site=None, model=User)
-        admin_cls.enable_change_view = False
-        self.assertIsNone(
-            admin_cls.get_list_display_links(request=self.get_request(user=self.user), list_display=('first_name',))
-        )
-
-    def test_change_view_can_see_method_called_because_of_positive_flag(self):
-        admin_cls = TestAdmin(admin_site=None, model=User)
-        with mock.patch.object(admin_cls, 'can_see_change_view', return_value=True) as mocked_can_see_method:
-            with mock.patch('django.contrib.admin.ModelAdmin.change_view') as mocked_base_change_view:
-                admin_cls.change_view(request=self.get_request(user=self.super_user), object_id=str(self.user.id))
-
-        mocked_can_see_method.assert_called_once()
-        mocked_base_change_view.assert_called_once()
-
-    def test_change_view_can_see_method_not_called_because_of_negative_flag(self):
-        admin_cls = TestAdmin(admin_site=None, model=User)
-        with mock.patch.object(admin_cls, 'can_see_change_view', return_value=False) as mocked_can_see_method:
-            with mock.patch('django.contrib.admin.ModelAdmin.change_view') as mocked_base_change_view:
-                admin_cls.change_view(request=self.get_request(user=self.super_user), object_id=str(self.user.id))
-
-        mocked_can_see_method.assert_called_once()
-        mocked_base_change_view.assert_not_called()
-
-    def test_change_view_can_see_method_not_called_but_redirect(self):
-        admin_cls = TestAdmin(admin_site=None, model=User)
-        admin_cls.enable_change_view = False
-        result = admin_cls.change_view(request=self.get_request(user=self.super_user), object_id=str(self.user.id))
-
-        self.assertIsInstance(result, HttpResponseRedirect)
+from unittest import mock
+
+from django.contrib import admin
+from django.contrib.auth.models import User
+from django.http import HttpResponseRedirect
+from django.test import TestCase
+
+from ai_django_core.admin.model_admins.mixins import DeactivatableChangeViewAdminMixin
+from ai_django_core.tests.mixins import RequestProviderMixin
+
+
+class TestAdmin(DeactivatableChangeViewAdminMixin, admin.ModelAdmin):
+    pass
+
+
+class DeactivatableChangeViewAdminMixinTest(RequestProviderMixin, TestCase):
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+
+        # Use random model for this meta test
+        cls.user = User.objects.create(username="test_user", is_superuser=False)
+        cls.super_user = User.objects.create(username="super_user", is_superuser=True)
+
+    def test_can_see_change_view_positive_flag(self):
+        admin_cls = TestAdmin(admin_site=None, model=User)
+        self.assertTrue(admin_cls.can_see_change_view(request=self.get_request()))
+
+    def test_can_see_change_view_negative_flag(self):
+        admin_cls = TestAdmin(admin_site=None, model=User)
+        admin_cls.enable_change_view = False
+        self.assertFalse(admin_cls.can_see_change_view(request=self.get_request()))
+
+    def test_get_list_display_links_can_see_method_called(self):
+        admin_cls = TestAdmin(admin_site=None, model=User)
+        with mock.patch.object(admin_cls, 'can_see_change_view', return_value=True) as mock_method:
+            admin_cls.get_list_display_links(request=self.get_request(user=self.user), list_display=('first_name',))
+
+        mock_method.assert_called_once()
+
+    def test_get_list_display_links_can_see_method_positive_flag(self):
+        admin_cls = TestAdmin(admin_site=None, model=User)
+        field_tuple = ('first_name',)
+        self.assertEqual(
+            list(field_tuple),
+            admin_cls.get_list_display_links(request=self.get_request(user=self.user), list_display=field_tuple),
+        )
+
+    def test_get_list_display_links_can_see_method_negative_flag(self):
+        admin_cls = TestAdmin(admin_site=None, model=User)
+        admin_cls.enable_change_view = False
+        self.assertIsNone(
+            admin_cls.get_list_display_links(request=self.get_request(user=self.user), list_display=('first_name',))
+        )
+
+    def test_change_view_can_see_method_called_because_of_positive_flag(self):
+        admin_cls = TestAdmin(admin_site=None, model=User)
+        with mock.patch.object(admin_cls, 'can_see_change_view', return_value=True) as mocked_can_see_method:
+            with mock.patch('django.contrib.admin.ModelAdmin.change_view') as mocked_base_change_view:
+                admin_cls.change_view(request=self.get_request(user=self.super_user), object_id=str(self.user.id))
+
+        mocked_can_see_method.assert_called_once()
+        mocked_base_change_view.assert_called_once()
+
+    def test_change_view_can_see_method_not_called_because_of_negative_flag(self):
+        admin_cls = TestAdmin(admin_site=None, model=User)
+        with mock.patch.object(admin_cls, 'can_see_change_view', return_value=False) as mocked_can_see_method:
+            with mock.patch('django.contrib.admin.ModelAdmin.change_view') as mocked_base_change_view:
+                admin_cls.change_view(request=self.get_request(user=self.super_user), object_id=str(self.user.id))
+
+        mocked_can_see_method.assert_called_once()
+        mocked_base_change_view.assert_not_called()
+
+    def test_change_view_can_see_method_not_called_but_redirect(self):
+        admin_cls = TestAdmin(admin_site=None, model=User)
+        admin_cls.enable_change_view = False
+        result = admin_cls.change_view(request=self.get_request(user=self.super_user), object_id=str(self.user.id))
+
+        self.assertIsInstance(result, HttpResponseRedirect)
```

### Comparing `ai-django-core-7.0.0/tests/admin/model_admin_mixins/test_fetch_object_mixin.py` & `ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_fetch_object_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py` & `ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/ambient_toolbox/test_test_structure_validator.py` & `ai-django-core-7.0.1/tests/ambient_toolbox/test_test_structure_validator.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/drf/test_fields.py` & `ai-django-core-7.0.1/tests/drf/test_fields.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/selectors/test_permission.py` & `ai-django-core-7.0.1/tests/selectors/test_permission.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_admin_forms.py` & `ai-django-core-7.0.1/tests/test_admin_forms.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_admin_inlines.py` & `ai-django-core-7.0.1/tests/test_admin_inlines.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_admin_model_admins_classes.py` & `ai-django-core-7.0.1/tests/test_admin_model_admins_classes.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_admin_view_mixins.py` & `ai-django-core-7.0.1/tests/test_admin_view_mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_context_manager.py` & `ai-django-core-7.0.1/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_email_test_service.py` & `ai-django-core-7.0.1/tests/test_email_test_service.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,248 +1,248 @@
-import re
-
-from django.core import mail
-from django.core.mail import EmailMultiAlternatives
-from django.test import TestCase
-from django.utils.translation import gettext_lazy as _
-
-from ai_django_core.mail.services.tests import EmailTestService, EmailTestServiceMail, EmailTestServiceQuerySet
-
-
-class EmailTestServiceTest(TestCase):
-    @classmethod
-    def setUpClass(cls):
-        super().setUpClass()
-
-        # Mail data
-        cls.subject = 'Super great email (definitely not spam!)'
-        cls.to = 'spam@world.com'
-        cls.cc = 'spam-copy@world.com'
-        cls.bcc = 'spam-secret@world.com'
-        cls.content_part = 'body part'
-        cls.text_content = 'I\'m the %s.' % cls.content_part
-        cls.html_content = '<html>I\'m the %s.</html>' % cls.content_part
-
-        cls.other_mail_subject = 'Other mail subject'
-
-        # Initialize django outbox
-        mail.outbox = []
-
-        # Instances
-        cls.ets = EmailTestService()
-
-    def setUp(self):
-        super().setUp()
-
-        # Create email per test case
-        email = EmailMultiAlternatives(self.subject, self.text_content, to=[self.to], cc=[self.cc], bcc=[self.bcc])
-        email.attach_alternative(self.html_content, "text/html")
-        mail.outbox.append(email)
-
-        # Create second email per test case
-        email = EmailMultiAlternatives(
-            self.other_mail_subject, self.text_content, to=['to@world.com'], cc=['cc@world.com'], bcc=['bcc@world.com']
-        )
-        email.attach_alternative(self.html_content, "text/html")
-        mail.outbox.append(email)
-
-    def tearDown(self) -> None:
-        super().tearDown()
-        # Emtpy mailbox for next test
-        mail.outbox = []
-
-    def test_outbox_is_updated(self):
-        self.assertEqual(self.ets.all().count(), 2)
-        # Create third mail
-        email = EmailMultiAlternatives(
-            self.other_mail_subject, self.text_content, to=['to@world.com'], cc=['cc@world.com'], bcc=['bcc@world.com']
-        )
-        email.attach_alternative(self.html_content, "text/html")
-        mail.outbox.append(email)
-        self.assertEqual(self.ets.all().count(), 3)
-
-    def test_ensure_outbox_is_loaded(self):
-        ets = EmailTestService()
-        self.assertEqual(ets._outbox, None)
-        ets._ensure_outbox_is_loaded()
-        self.assertIsInstance(ets._outbox, list)
-
-    def test_reload(self):
-        ets = EmailTestService()
-        self.assertEqual(ets._outbox, None)
-        ets.reload()
-        self.assertIsInstance(ets._outbox, list)
-
-    def test_filter_no_params(self):
-        self.assertRaises(ValueError, self.ets.filter)
-
-    def test_filter_to_valid(self):
-        qs = self.ets.filter(to=self.to)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_cc_valid(self):
-        qs = self.ets.filter(cc=self.cc)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_bcc_valid(self):
-        qs = self.ets.filter(bcc=self.bcc)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_subject_valid(self):
-        qs = self.ets.filter(subject=self.subject)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_to_invalid(self):
-        qs = self.ets.filter(to='not-my@mail.com')
-        self.assertEqual(qs.count(), 0)
-
-    def test_filter_cc_invalid(self):
-        qs = self.ets.filter(cc='not-my@mail.com')
-        self.assertEqual(qs.count(), 0)
-
-    def test_filter_bcc_invalid(self):
-        qs = self.ets.filter(bcc='not-my@mail.com')
-        self.assertEqual(qs.count(), 0)
-
-    def test_filter_subject_invalid(self):
-        qs = self.ets.filter(subject='Not my subject')
-        self.assertEqual(qs.count(), 0)
-
-    def test_filter_to_cc_valid(self):
-        qs = self.ets.filter(to=self.to, cc=self.cc)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_to_cc_bcc_valid(self):
-        qs = self.ets.filter(to=self.to, cc=self.cc, bcc=self.bcc)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_to_cc_bcc_subject_valid(self):
-        qs = self.ets.filter(to=self.to, cc=self.cc, bcc=self.bcc, subject=self.subject)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_to_cc_bcc_subject_invalid(self):
-        qs = self.ets.filter(to=self.to, cc=self.cc, bcc=self.bcc, subject='Not my subject')
-        self.assertEqual(qs.count(), 0)
-
-    def test_filter_subject_regular(self):
-        qs = self.ets.filter(subject=self.subject)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_subject_regex_invalid(self):
-        qs = self.ets.filter(subject=re.compile('Not my subject'))
-        self.assertEqual(qs.count(), 0)
-
-    def test_filter_subject_translatable(self):
-        qs = self.ets.filter(subject=_(self.subject))
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_subject_regex_valid_single(self):
-        qs = self.ets.filter(subject=re.compile('definitely not'))
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_subject_regex_valid_multiple(self):
-        qs = self.ets.filter(subject=re.compile('other|spam', flags=re.IGNORECASE))
-        self.assertEqual(qs.count(), 2)
-
-    def test_all(self):
-        # Assertion
-        self.assertEqual(self.ets.all().count(), 2)
-
-    def test_validate_lookup_cache_contains_one_element_true(self):
-        # Assertion (we have two mails so it's not equal to 1)
-        self.assertEqual(self.ets.all().count(), 2)
-        self.assertRaises(RuntimeError, self.ets.all()._validate_lookup_cache_contains_one_element)
-
-    def test_validate_lookup_cache_contains_one_element_false(self):
-        self.assertEqual(self.ets.filter(subject=self.subject).count(), 1)
-        self.assertEqual(self.ets.filter(subject=self.subject)._validate_lookup_cache_contains_one_element(), None)
-
-    def test_ensure_matching_list_was_populated_false(self):
-        self.assertRaises(RuntimeError, EmailTestServiceQuerySet()._ensure_matching_list_was_populated)
-
-    def test_ensure_matching_list_was_populated_true(self):
-        self.assertEqual(self.ets.all()._ensure_matching_list_was_populated(), None)
-
-    def test_get_html_content(self):
-        self.assertEqual(self.ets.filter(subject=self.subject)._get_html_content(), self.html_content)
-
-    def test_get_txt_content(self):
-        self.assertEqual(self.ets.filter(subject=self.subject)._get_txt_content(), self.text_content)
-
-    def test_one_true(self):
-        self.assertEqual(self.ets.filter(subject=self.subject).one(), True)
-
-    def test_one_false(self):
-        self.assertEqual(self.ets.all().one(), False)
-
-    def test_count(self):
-        self.assertEqual(self.ets.all().count(), 2)
-        self.assertEqual(self.ets.filter(subject=self.subject).count(), 1)
-        self.assertEqual(self.ets.filter(subject='Not my subject').count(), 0)
-
-    def test_first(self):
-        self.assertEqual(self.ets.all().first().subject, self.subject)
-
-    def test_last(self):
-        self.assertEqual(self.ets.all().last().subject, self.other_mail_subject)
-
-    def test_assert_one_true(self):
-        self.ets.filter(subject=self.subject).assert_one()
-
-    def test_assert_one_false(self):
-        with self.assertRaises(AssertionError):
-            self.ets.all().assert_one()
-
-    def test_assert_quantity_true(self):
-        self.ets.filter(subject=self.subject).assert_quantity(1)
-
-    def test_assert_quantity_false(self):
-        with self.assertRaises(AssertionError):
-            self.ets.filter(subject=self.subject).assert_quantity(0)
-
-    def test_assert_subject_true(self):
-        self.ets.filter(subject=self.subject).assert_subject(self.subject)
-
-    def test_assert_subject_false(self):
-        with self.assertRaises(AssertionError):
-            self.ets.filter(subject=self.subject).assert_subject(self.other_mail_subject)
-
-    def test_assert_body_contains_true(self):
-        self.ets.filter(subject=self.subject).assert_body_contains(self.content_part)
-
-    def test_assert_body_contains_false(self):
-        with self.assertRaises(AssertionError):
-            self.ets.filter(subject=self.subject).assert_body_contains('Not in here!')
-
-    def test_assert_body_contains_not_true(self):
-        self.ets.filter(subject=self.subject).assert_body_contains_not('Not in here!')
-
-    def test_assert_body_contains_not_false(self):
-        with self.assertRaises(AssertionError):
-            self.ets.filter(subject=self.subject).assert_body_contains_not(self.content_part)
-
-    def test_assert_body_contains_no_html_part(self):
-        subject = 'No html email'
-        email = EmailMultiAlternatives(subject, self.text_content, to=[self.to], cc=[self.cc], bcc=[self.bcc])
-        mail.outbox.append(email)
-
-        self.ets.filter(subject=subject).assert_body_contains(self.content_part)
-
-    def test_can_get_mail_via_item(self):
-        mail_qs = self.ets.all()
-        self.assertIsInstance(mail_qs[0], EmailTestServiceMail)
-
-    def test_can_get_first_email_via_brackets_operator(self):
-        mail_qs = self.ets.all()
-        self.assertEqual(mail_qs[0], mail_qs.first())
-
-    def test_can_get_last_email_via_brackets_operator(self):
-        mail_qs = self.ets.all()
-        self.assertEqual(mail_qs[-1], mail_qs.last())
-
-    def test_can_use_len_operator(self):
-        mail_qs = self.ets.all()
-        self.assertEqual(len(mail_qs), 2)
-
-    def test_assert_to_contains(self):
-        email = self.ets.all()[0]
-        email.assert_to_contains(self.to)
+import re
+
+from django.core import mail
+from django.core.mail import EmailMultiAlternatives
+from django.test import TestCase
+from django.utils.translation import gettext_lazy as _
+
+from ai_django_core.mail.services.tests import EmailTestService, EmailTestServiceMail, EmailTestServiceQuerySet
+
+
+class EmailTestServiceTest(TestCase):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+        # Mail data
+        cls.subject = 'Super great email (definitely not spam!)'
+        cls.to = 'spam@world.com'
+        cls.cc = 'spam-copy@world.com'
+        cls.bcc = 'spam-secret@world.com'
+        cls.content_part = 'body part'
+        cls.text_content = 'I\'m the %s.' % cls.content_part
+        cls.html_content = '<html>I\'m the %s.</html>' % cls.content_part
+
+        cls.other_mail_subject = 'Other mail subject'
+
+        # Initialize django outbox
+        mail.outbox = []
+
+        # Instances
+        cls.ets = EmailTestService()
+
+    def setUp(self):
+        super().setUp()
+
+        # Create email per test case
+        email = EmailMultiAlternatives(self.subject, self.text_content, to=[self.to], cc=[self.cc], bcc=[self.bcc])
+        email.attach_alternative(self.html_content, "text/html")
+        mail.outbox.append(email)
+
+        # Create second email per test case
+        email = EmailMultiAlternatives(
+            self.other_mail_subject, self.text_content, to=['to@world.com'], cc=['cc@world.com'], bcc=['bcc@world.com']
+        )
+        email.attach_alternative(self.html_content, "text/html")
+        mail.outbox.append(email)
+
+    def tearDown(self) -> None:
+        super().tearDown()
+        # Emtpy mailbox for next test
+        mail.outbox = []
+
+    def test_outbox_is_updated(self):
+        self.assertEqual(self.ets.all().count(), 2)
+        # Create third mail
+        email = EmailMultiAlternatives(
+            self.other_mail_subject, self.text_content, to=['to@world.com'], cc=['cc@world.com'], bcc=['bcc@world.com']
+        )
+        email.attach_alternative(self.html_content, "text/html")
+        mail.outbox.append(email)
+        self.assertEqual(self.ets.all().count(), 3)
+
+    def test_ensure_outbox_is_loaded(self):
+        ets = EmailTestService()
+        self.assertEqual(ets._outbox, None)
+        ets._ensure_outbox_is_loaded()
+        self.assertIsInstance(ets._outbox, list)
+
+    def test_reload(self):
+        ets = EmailTestService()
+        self.assertEqual(ets._outbox, None)
+        ets.reload()
+        self.assertIsInstance(ets._outbox, list)
+
+    def test_filter_no_params(self):
+        self.assertRaises(ValueError, self.ets.filter)
+
+    def test_filter_to_valid(self):
+        qs = self.ets.filter(to=self.to)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_cc_valid(self):
+        qs = self.ets.filter(cc=self.cc)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_bcc_valid(self):
+        qs = self.ets.filter(bcc=self.bcc)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_subject_valid(self):
+        qs = self.ets.filter(subject=self.subject)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_to_invalid(self):
+        qs = self.ets.filter(to='not-my@mail.com')
+        self.assertEqual(qs.count(), 0)
+
+    def test_filter_cc_invalid(self):
+        qs = self.ets.filter(cc='not-my@mail.com')
+        self.assertEqual(qs.count(), 0)
+
+    def test_filter_bcc_invalid(self):
+        qs = self.ets.filter(bcc='not-my@mail.com')
+        self.assertEqual(qs.count(), 0)
+
+    def test_filter_subject_invalid(self):
+        qs = self.ets.filter(subject='Not my subject')
+        self.assertEqual(qs.count(), 0)
+
+    def test_filter_to_cc_valid(self):
+        qs = self.ets.filter(to=self.to, cc=self.cc)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_to_cc_bcc_valid(self):
+        qs = self.ets.filter(to=self.to, cc=self.cc, bcc=self.bcc)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_to_cc_bcc_subject_valid(self):
+        qs = self.ets.filter(to=self.to, cc=self.cc, bcc=self.bcc, subject=self.subject)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_to_cc_bcc_subject_invalid(self):
+        qs = self.ets.filter(to=self.to, cc=self.cc, bcc=self.bcc, subject='Not my subject')
+        self.assertEqual(qs.count(), 0)
+
+    def test_filter_subject_regular(self):
+        qs = self.ets.filter(subject=self.subject)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_subject_regex_invalid(self):
+        qs = self.ets.filter(subject=re.compile('Not my subject'))
+        self.assertEqual(qs.count(), 0)
+
+    def test_filter_subject_translatable(self):
+        qs = self.ets.filter(subject=_(self.subject))
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_subject_regex_valid_single(self):
+        qs = self.ets.filter(subject=re.compile('definitely not'))
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_subject_regex_valid_multiple(self):
+        qs = self.ets.filter(subject=re.compile('other|spam', flags=re.IGNORECASE))
+        self.assertEqual(qs.count(), 2)
+
+    def test_all(self):
+        # Assertion
+        self.assertEqual(self.ets.all().count(), 2)
+
+    def test_validate_lookup_cache_contains_one_element_true(self):
+        # Assertion (we have two mails so it's not equal to 1)
+        self.assertEqual(self.ets.all().count(), 2)
+        self.assertRaises(RuntimeError, self.ets.all()._validate_lookup_cache_contains_one_element)
+
+    def test_validate_lookup_cache_contains_one_element_false(self):
+        self.assertEqual(self.ets.filter(subject=self.subject).count(), 1)
+        self.assertEqual(self.ets.filter(subject=self.subject)._validate_lookup_cache_contains_one_element(), None)
+
+    def test_ensure_matching_list_was_populated_false(self):
+        self.assertRaises(RuntimeError, EmailTestServiceQuerySet()._ensure_matching_list_was_populated)
+
+    def test_ensure_matching_list_was_populated_true(self):
+        self.assertEqual(self.ets.all()._ensure_matching_list_was_populated(), None)
+
+    def test_get_html_content(self):
+        self.assertEqual(self.ets.filter(subject=self.subject)._get_html_content(), self.html_content)
+
+    def test_get_txt_content(self):
+        self.assertEqual(self.ets.filter(subject=self.subject)._get_txt_content(), self.text_content)
+
+    def test_one_true(self):
+        self.assertEqual(self.ets.filter(subject=self.subject).one(), True)
+
+    def test_one_false(self):
+        self.assertEqual(self.ets.all().one(), False)
+
+    def test_count(self):
+        self.assertEqual(self.ets.all().count(), 2)
+        self.assertEqual(self.ets.filter(subject=self.subject).count(), 1)
+        self.assertEqual(self.ets.filter(subject='Not my subject').count(), 0)
+
+    def test_first(self):
+        self.assertEqual(self.ets.all().first().subject, self.subject)
+
+    def test_last(self):
+        self.assertEqual(self.ets.all().last().subject, self.other_mail_subject)
+
+    def test_assert_one_true(self):
+        self.ets.filter(subject=self.subject).assert_one()
+
+    def test_assert_one_false(self):
+        with self.assertRaises(AssertionError):
+            self.ets.all().assert_one()
+
+    def test_assert_quantity_true(self):
+        self.ets.filter(subject=self.subject).assert_quantity(1)
+
+    def test_assert_quantity_false(self):
+        with self.assertRaises(AssertionError):
+            self.ets.filter(subject=self.subject).assert_quantity(0)
+
+    def test_assert_subject_true(self):
+        self.ets.filter(subject=self.subject).assert_subject(self.subject)
+
+    def test_assert_subject_false(self):
+        with self.assertRaises(AssertionError):
+            self.ets.filter(subject=self.subject).assert_subject(self.other_mail_subject)
+
+    def test_assert_body_contains_true(self):
+        self.ets.filter(subject=self.subject).assert_body_contains(self.content_part)
+
+    def test_assert_body_contains_false(self):
+        with self.assertRaises(AssertionError):
+            self.ets.filter(subject=self.subject).assert_body_contains('Not in here!')
+
+    def test_assert_body_contains_not_true(self):
+        self.ets.filter(subject=self.subject).assert_body_contains_not('Not in here!')
+
+    def test_assert_body_contains_not_false(self):
+        with self.assertRaises(AssertionError):
+            self.ets.filter(subject=self.subject).assert_body_contains_not(self.content_part)
+
+    def test_assert_body_contains_no_html_part(self):
+        subject = 'No html email'
+        email = EmailMultiAlternatives(subject, self.text_content, to=[self.to], cc=[self.cc], bcc=[self.bcc])
+        mail.outbox.append(email)
+
+        self.ets.filter(subject=subject).assert_body_contains(self.content_part)
+
+    def test_can_get_mail_via_item(self):
+        mail_qs = self.ets.all()
+        self.assertIsInstance(mail_qs[0], EmailTestServiceMail)
+
+    def test_can_get_first_email_via_brackets_operator(self):
+        mail_qs = self.ets.all()
+        self.assertEqual(mail_qs[0], mail_qs.first())
+
+    def test_can_get_last_email_via_brackets_operator(self):
+        mail_qs = self.ets.all()
+        self.assertEqual(mail_qs[-1], mail_qs.last())
+
+    def test_can_use_len_operator(self):
+        mail_qs = self.ets.all()
+        self.assertEqual(len(mail_qs), 2)
+
+    def test_assert_to_contains(self):
+        email = self.ets.all()[0]
+        email.assert_to_contains(self.to)
```

### Comparing `ai-django-core-7.0.0/tests/test_log_whodid.py` & `ai-django-core-7.0.1/tests/test_log_whodid.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_mail_services.py` & `ai-django-core-7.0.1/tests/test_mail_services.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_managers.py` & `ai-django-core-7.0.1/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_math.py` & `ai-django-core-7.0.1/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_middleware.py` & `ai-django-core-7.0.1/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_mixins_models.py` & `ai-django-core-7.0.1/tests/test_mixins_models.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_models.py` & `ai-django-core-7.0.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_rest_api_mixins.py` & `ai-django-core-7.0.1/tests/test_rest_api_mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_scrubbing_service.py` & `ai-django-core-7.0.1/tests/test_scrubbing_service.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_sentry_helper.py` & `ai-django-core-7.0.1/tests/test_sentry_helper.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_utils_date.py` & `ai-django-core-7.0.1/tests/test_utils_date.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_utils_file.py` & `ai-django-core-7.0.1/tests/test_utils_file.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_utils_model.py` & `ai-django-core-7.0.1/tests/test_utils_model.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_utils_named_tuple.py` & `ai-django-core-7.0.1/tests/test_utils_named_tuple.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/test_utils_string.py` & `ai-django-core-7.0.1/tests/test_utils_string.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/tests/mixins/test_request_provider_mixin.py` & `ai-django-core-7.0.1/tests/tests/mixins/test_request_provider_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/tests/test_mail_backends.py` & `ai-django-core-7.0.1/tests/tests/test_mail_backends.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/view_layer/test_formset_mixins.py` & `ai-django-core-7.0.1/tests/view_layer/test_formset_mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/view_layer/test_htmx_response_mixin.py` & `ai-django-core-7.0.1/tests/view_layer/test_htmx_response_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/tests/view_layer/test_meta_mixins.py` & `ai-django-core-7.0.1/tests/view_layer/test_meta_mixins.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from django.contrib.auth.models import AnonymousUser, Permission, User
-from django.http import HttpResponse
-from django.test import TestCase
-from django.views import generic
-
-from ai_django_core.tests.mixins import RequestProviderMixin
-from ai_django_core.view_layer.mixins import DjangoPermissionRequiredMixin
-
-
-class MetaDjangoPermissionRequiredMixinTest(RequestProviderMixin, TestCase):
-    class TestViewNoPerms(DjangoPermissionRequiredMixin, generic.View):
-        pass
-
-    class TestViewSinglePerm(DjangoPermissionRequiredMixin, generic.View):
-        permission_list = ['auth.change_user']
-
-        def get(self, *args, **kwargs):
-            return HttpResponse(status=200)
-
-    class TestViewMultiplePerms(DjangoPermissionRequiredMixin, generic.View):
-        permission_list = ['auth.change_user', 'auth.add_user']
-
-        def get_login_url(self):
-            return 'login/'
-
-    @classmethod
-    def setUpTestData(cls):
-        super().setUpTestData()
-
-        cls.permission = Permission.objects.get_by_natural_key(app_label='auth', codename='change_user', model='user')
-
-    def setUp(self) -> None:
-        super().setUp()
-        self.user = User.objects.create(username='test_user', email='test.user@ai-django-core.com')
-
-    def test_get_login_url(self):
-        self.assertEqual(self.TestViewMultiplePerms().get_login_url(), 'login/')
-
-    def test_permissions_are_set_validation(self):
-        with self.assertRaises(RuntimeError):
-            self.TestViewNoPerms()
-
-    def test_has_permissions_correct_permission(self):
-        self.user.user_permissions.add(self.permission)
-
-        self.assertTrue(self.TestViewSinglePerm().has_permissions(self.user))
-
-    def test_has_permissions_missing_permission(self):
-        self.assertFalse(self.TestViewSinglePerm().has_permissions(self.user))
-
-    def test_has_permissions_multiple_permissions_one_missing(self):
-        self.user.user_permissions.add(self.permission)
-
-        self.assertFalse(self.TestViewMultiplePerms().has_permissions(self.user))
-
-    def test_passes_login_barrier_no_login_required(self):
-        view = self.TestViewSinglePerm()
-        view.login_required = False
-
-        self.assertTrue(view.passes_login_barrier(self.user))
-
-    def test_passes_login_barrier_user_logged_in(self):
-        self.assertTrue(self.TestViewSinglePerm().passes_login_barrier(self.user))
-
-    def test_passes_login_barrier_user_not_logged_in(self):
-        self.assertFalse(self.TestViewSinglePerm().passes_login_barrier(AnonymousUser()))
-
-    def test_has_permissions_is_superuser_is_not_blocked(self):
-        self.user.is_superuser = True
-        self.assertTrue(self.TestViewSinglePerm().has_permissions(self.user))
-
-    def test_has_permissions_django_superuser_is_always_allowed(self):
-        self.user.is_superuser = True
-        self.assertTrue(self.TestViewSinglePerm().has_permissions(self.user))
-
-    def test_dispatch_lockout_on_missing_permissions(self):
-        response = self.TestViewSinglePerm().dispatch(request=self.get_request(self.user))
-
-        self.assertEqual(response.status_code, 403)
-
-    def test_dispatch_working_on_having_permissions(self):
-        self.user.user_permissions.add(self.permission)
-        view = self.TestViewSinglePerm()
-        response = view.dispatch(request=self.get_request(self.user))
-
-        self.assertEqual(response.status_code, 200)
+from django.contrib.auth.models import AnonymousUser, Permission, User
+from django.http import HttpResponse
+from django.test import TestCase
+from django.views import generic
+
+from ai_django_core.tests.mixins import RequestProviderMixin
+from ai_django_core.view_layer.mixins import DjangoPermissionRequiredMixin
+
+
+class MetaDjangoPermissionRequiredMixinTest(RequestProviderMixin, TestCase):
+    class TestViewNoPerms(DjangoPermissionRequiredMixin, generic.View):
+        pass
+
+    class TestViewSinglePerm(DjangoPermissionRequiredMixin, generic.View):
+        permission_list = ['auth.change_user']
+
+        def get(self, *args, **kwargs):
+            return HttpResponse(status=200)
+
+    class TestViewMultiplePerms(DjangoPermissionRequiredMixin, generic.View):
+        permission_list = ['auth.change_user', 'auth.add_user']
+
+        def get_login_url(self):
+            return 'login/'
+
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+
+        cls.permission = Permission.objects.get_by_natural_key(app_label='auth', codename='change_user', model='user')
+
+    def setUp(self) -> None:
+        super().setUp()
+        self.user = User.objects.create(username='test_user', email='test.user@ai-django-core.com')
+
+    def test_get_login_url(self):
+        self.assertEqual(self.TestViewMultiplePerms().get_login_url(), 'login/')
+
+    def test_permissions_are_set_validation(self):
+        with self.assertRaises(RuntimeError):
+            self.TestViewNoPerms()
+
+    def test_has_permissions_correct_permission(self):
+        self.user.user_permissions.add(self.permission)
+
+        self.assertTrue(self.TestViewSinglePerm().has_permissions(self.user))
+
+    def test_has_permissions_missing_permission(self):
+        self.assertFalse(self.TestViewSinglePerm().has_permissions(self.user))
+
+    def test_has_permissions_multiple_permissions_one_missing(self):
+        self.user.user_permissions.add(self.permission)
+
+        self.assertFalse(self.TestViewMultiplePerms().has_permissions(self.user))
+
+    def test_passes_login_barrier_no_login_required(self):
+        view = self.TestViewSinglePerm()
+        view.login_required = False
+
+        self.assertTrue(view.passes_login_barrier(self.user))
+
+    def test_passes_login_barrier_user_logged_in(self):
+        self.assertTrue(self.TestViewSinglePerm().passes_login_barrier(self.user))
+
+    def test_passes_login_barrier_user_not_logged_in(self):
+        self.assertFalse(self.TestViewSinglePerm().passes_login_barrier(AnonymousUser()))
+
+    def test_has_permissions_is_superuser_is_not_blocked(self):
+        self.user.is_superuser = True
+        self.assertTrue(self.TestViewSinglePerm().has_permissions(self.user))
+
+    def test_has_permissions_django_superuser_is_always_allowed(self):
+        self.user.is_superuser = True
+        self.assertTrue(self.TestViewSinglePerm().has_permissions(self.user))
+
+    def test_dispatch_lockout_on_missing_permissions(self):
+        response = self.TestViewSinglePerm().dispatch(request=self.get_request(self.user))
+
+        self.assertEqual(response.status_code, 403)
+
+    def test_dispatch_working_on_having_permissions(self):
+        self.user.user_permissions.add(self.permission)
+        view = self.TestViewSinglePerm()
+        response = view.dispatch(request=self.get_request(self.user))
+
+        self.assertEqual(response.status_code, 200)
```

### Comparing `ai-django-core-7.0.0/tests/view_layer/test_views.py` & `ai-django-core-7.0.1/tests/view_layer/test_views.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.0/PKG-INFO` & `ai-django-core-7.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-django-core
-Version: 7.0.0
+Version: 7.0.1
 Summary: Ambient toolbox - Lots of helper functions and useful widgets
 Author-email: "Ambient Innovation: GmbH" <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
@@ -51,14 +51,22 @@
 Provides-Extra: graphql
 Provides-Extra: view-layer
 
 [![pypi](https://img.shields.io/pypi/v/ai-django-core.svg)](https://pypi.python.org/pypi/ai-django-core/)
 [![Downloads](https://pepy.tech/badge/ai-django-core)](https://pepy.tech/project/ai-django-core)
 [![Documentation Status](https://readthedocs.org/projects/ai-django-core/badge/?version=latest)](https://ai-django-core.readthedocs.io/en/latest/?badge=latest)
 
+# Disclaimer: Package was superseded by ambient-toolbox!
+
+This package was renamed, moved and deprecated under the old name. The successor is the "**Ambient Toolbox**".
+* [PyPI](https://pypi.org/project/ambient-toolbox/)
+* [Migration docs](https://github.com/ambient-innovation/ambient-toolbox#migration-from-ai_django_core)
+
+---
+
 # Overview
 
 This package contains various useful helper functions. You can read up on all the fancy things at
 [readthedocs.io](https://ai-django-core.readthedocs.io/en/latest/index.html).
 
 # Installation
```

