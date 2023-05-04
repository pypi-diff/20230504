# Comparing `tmp/document_merge_service-6.1.0.tar.gz` & `tmp/document_merge_service-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_merge_service-6.1.0.tar", max compression
+gzip compressed data, was "document_merge_service-6.1.1.tar", max compression
```

## Comparing `document_merge_service-6.1.0.tar` & `document_merge_service-6.1.1.tar`

### file list

```diff
@@ -1,68 +1,67 @@
--rw-r--r--   0        0        0    10652 2023-01-27 09:04:38.057199 document_merge_service-6.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-01-27 09:04:38.057199 document_merge_service-6.1.0/LICENSE
--rw-r--r--   0        0        0     2261 2023-01-27 09:04:38.057199 document_merge_service-6.1.0/README.md
--rw-r--r--   0        0        0        0 2023-01-27 09:04:38.061199 document_merge_service-6.1.0/document_merge_service/__init__.py
--rw-r--r--   0        0        0        0 2023-01-27 09:04:38.061199 document_merge_service-6.1.0/document_merge_service/api/__init__.py
--rw-r--r--   0        0        0      405 2023-01-27 09:04:38.061199 document_merge_service-6.1.0/document_merge_service/api/apps.py
--rw-r--r--   0        0        0     3159 2023-01-27 09:04:38.061199 document_merge_service-6.1.0/document_merge_service/api/authentication.py
--rw-r--r--   0        0        0      504 2023-01-27 09:04:38.061199 document_merge_service-6.1.0/document_merge_service/api/data/__init__.py
--rw-r--r--   0        0        0      559 2023-01-27 09:04:38.061199 document_merge_service-6.1.0/document_merge_service/api/data/black.png
--rw-r--r--   0        0        0     9125 2023-01-27 09:04:38.061199 document_merge_service-6.1.0/document_merge_service/api/data/docx-mailmerge-syntax.docx
--rw-r--r--   0        0        0    11489 2023-01-27 09:04:38.061199 document_merge_service-6.1.0/document_merge_service/api/data/docx-mailmerge.docx
--rw-r--r--   0        0        0     5735 2023-01-27 09:04:38.061199 document_merge_service-6.1.0/document_merge_service/api/data/docx-template-filters.docx
--rw-r--r--   0        0        0     6087 2023-01-27 09:04:38.061199 document_merge_service-6.1.0/document_merge_service/api/data/docx-template-loopcontrols.docx
--rw-r--r--   0        0        0     5952 2023-01-27 09:04:38.061199 document_merge_service-6.1.0/document_merge_service/api/data/docx-template-placeholdercheck.docx
--rw-r--r--   0        0        0     5091 2023-01-27 09:04:38.061199 document_merge_service-6.1.0/document_merge_service/api/data/docx-template-syntax.docx
--rw-r--r--   0        0        0     5490 2023-01-27 09:04:38.061199 document_merge_service-6.1.0/document_merge_service/api/data/docx-template.docx
--rw-r--r--   0        0        0  1127936 2023-01-27 09:04:38.065199 document_merge_service-6.1.0/document_merge_service/api/data/loadtest/1.doc
--rw-r--r--   0        0        0   175922 2023-01-27 09:04:38.065199 document_merge_service-6.1.0/document_merge_service/api/data/loadtest/2.docx
--rw-r--r--   0        0        0   163307 2023-01-27 09:04:38.065199 document_merge_service-6.1.0/document_merge_service/api/data/loadtest/3.docx
--rw-r--r--   0        0        0   141498 2023-01-27 09:04:38.065199 document_merge_service-6.1.0/document_merge_service/api/data/loadtest/4.docx
--rw-r--r--   0        0        0       22 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/data/test.txt
--rw-r--r--   0        0        0        5 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/data/xlsx-not-valid.xlsx
--rw-r--r--   0        0        0     6424 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/data/xlsx-structure.xlsx
--rw-r--r--   0        0        0     6432 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/data/xlsx-syntax.xlsx
--rw-r--r--   0        0        0     4750 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/data/xlsx-template.xlsx
--rw-r--r--   0        0        0     9585 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/engines.py
--rw-r--r--   0        0        0      389 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/factories.py
--rw-r--r--   0        0        0     2841 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/filters.py
--rw-r--r--   0        0        0     2546 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/jinja.py
--rw-r--r--   0        0        0        0 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/management/__init__.py
--rw-r--r--   0        0        0        0 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/management/commands/__init__.py
--rw-r--r--   0        0        0     1582 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/management/commands/clean_dangling_files.py
--rw-r--r--   0        0        0     1249 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      489 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/migrations/0002_template_group.py
--rw-r--r--   0        0        0      375 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/migrations/0003_template_meta.py
--rw-r--r--   0        0        0      145 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/migrations/0004_cleanup_files.py
--rw-r--r--   0        0        0     1005 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py
--rw-r--r--   0        0        0      328 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/migrations/0006_remove_template_group.py
--rw-r--r--   0        0        0        0 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/migrations/__init__.py
--rw-r--r--   0        0        0     1876 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/models.py
--rw-r--r--   0        0        0      231 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/pagination.py
--rw-r--r--   0        0        0      289 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/permissions.py
--rw-r--r--   0        0        0     4651 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/serializers.py
--rw-r--r--   0        0        0        0 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/tests/snapshots/__init__.py
--rw-r--r--   0        0        0    29399 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/tests/snapshots/snap_test_template.py
--rw-r--r--   0        0        0     2270 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/tests/test_authentication.py
--rw-r--r--   0        0        0      942 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/tests/test_clean_dangling_files.py
--rw-r--r--   0        0        0     1821 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/tests/test_excel.py
--rw-r--r--   0        0        0     1372 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/tests/test_filters.py
--rw-r--r--   0        0        0     1300 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/tests/test_jinja.py
--rw-r--r--   0        0        0      749 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/tests/test_pagination.py
--rw-r--r--   0        0        0    25635 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/tests/test_template.py
--rw-r--r--   0        0        0     3425 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/tests/test_unoconv.py
--rw-r--r--   0        0        0     6947 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/unoconv.py
--rw-r--r--   0        0        0      356 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/urls.py
--rw-r--r--   0        0        0     3570 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/api/views.py
--rw-r--r--   0        0        0     2794 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/conftest.py
--rw-r--r--   0        0        0      789 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/sentry.py
--rw-r--r--   0        0        0     8039 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/settings.py
--rw-r--r--   0        0        0        0 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/tests/__init__.py
--rw-r--r--   0        0        0      386 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/tests/test_sentry.py
--rw-r--r--   0        0        0      615 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/tests/test_settings.py
--rw-r--r--   0        0        0      225 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/urls.py
--rw-r--r--   0        0        0      412 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/document_merge_service/wsgi.py
--rw-r--r--   0        0        0     3461 2023-01-27 09:04:38.069199 document_merge_service-6.1.0/pyproject.toml
--rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 document_merge_service-6.1.0/setup.py
--rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 document_merge_service-6.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10867 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/LICENSE
+-rw-r--r--   0        0        0     2261 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/document_merge_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/document_merge_service/api/__init__.py
+-rw-r--r--   0        0        0      405 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/document_merge_service/api/apps.py
+-rw-r--r--   0        0        0     3159 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/document_merge_service/api/authentication.py
+-rw-r--r--   0        0        0      504 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/document_merge_service/api/data/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/document_merge_service/api/data/black.png
+-rw-r--r--   0        0        0     9125 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/document_merge_service/api/data/docx-mailmerge-syntax.docx
+-rw-r--r--   0        0        0    11489 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/document_merge_service/api/data/docx-mailmerge.docx
+-rw-r--r--   0        0        0     5735 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/document_merge_service/api/data/docx-template-filters.docx
+-rw-r--r--   0        0        0     6087 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/document_merge_service/api/data/docx-template-loopcontrols.docx
+-rw-r--r--   0        0        0     5952 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/document_merge_service/api/data/docx-template-placeholdercheck.docx
+-rw-r--r--   0        0        0     5091 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/document_merge_service/api/data/docx-template-syntax.docx
+-rw-r--r--   0        0        0     5490 2023-05-04 06:11:41.874065 document_merge_service-6.1.1/document_merge_service/api/data/docx-template.docx
+-rw-r--r--   0        0        0  1127936 2023-05-04 06:11:41.878065 document_merge_service-6.1.1/document_merge_service/api/data/loadtest/1.doc
+-rw-r--r--   0        0        0   175922 2023-05-04 06:11:41.878065 document_merge_service-6.1.1/document_merge_service/api/data/loadtest/2.docx
+-rw-r--r--   0        0        0   163307 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/data/loadtest/3.docx
+-rw-r--r--   0        0        0   141498 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/data/loadtest/4.docx
+-rw-r--r--   0        0        0       22 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/data/test.txt
+-rw-r--r--   0        0        0        5 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/data/xlsx-not-valid.xlsx
+-rw-r--r--   0        0        0     6467 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/data/xlsx-structure.xlsx
+-rw-r--r--   0        0        0     6432 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/data/xlsx-syntax.xlsx
+-rw-r--r--   0        0        0     4750 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/data/xlsx-template.xlsx
+-rw-r--r--   0        0        0     9774 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/engines.py
+-rw-r--r--   0        0        0      389 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/factories.py
+-rw-r--r--   0        0        0     2841 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/filters.py
+-rw-r--r--   0        0        0     2546 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/jinja.py
+-rw-r--r--   0        0        0        0 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/management/commands/__init__.py
+-rw-r--r--   0        0        0     1582 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/management/commands/clean_dangling_files.py
+-rw-r--r--   0        0        0     1249 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      489 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/migrations/0002_template_group.py
+-rw-r--r--   0        0        0      375 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/migrations/0003_template_meta.py
+-rw-r--r--   0        0        0      145 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/migrations/0004_cleanup_files.py
+-rw-r--r--   0        0        0     1005 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/migrations/0005_xlsx_template_engine.py
+-rw-r--r--   0        0        0      328 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/migrations/0006_remove_template_group.py
+-rw-r--r--   0        0        0        0 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/migrations/__init__.py
+-rw-r--r--   0        0        0     1876 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/models.py
+-rw-r--r--   0        0        0      231 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/pagination.py
+-rw-r--r--   0        0        0      289 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/permissions.py
+-rw-r--r--   0        0        0     4651 2023-05-04 06:11:41.882065 document_merge_service-6.1.1/document_merge_service/api/serializers.py
+-rw-r--r--   0        0        0        0 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/api/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/api/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0    29399 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/api/tests/snapshots/snap_test_template.py
+-rw-r--r--   0        0        0     2270 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/api/tests/test_authentication.py
+-rw-r--r--   0        0        0      942 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/api/tests/test_clean_dangling_files.py
+-rw-r--r--   0        0        0     1963 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/api/tests/test_excel.py
+-rw-r--r--   0        0        0     1372 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/api/tests/test_filters.py
+-rw-r--r--   0        0        0     1300 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/api/tests/test_jinja.py
+-rw-r--r--   0        0        0      749 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/api/tests/test_pagination.py
+-rw-r--r--   0        0        0    25635 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/api/tests/test_template.py
+-rw-r--r--   0        0        0     3425 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/api/tests/test_unoconv.py
+-rw-r--r--   0        0        0     6947 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/api/unoconv.py
+-rw-r--r--   0        0        0      356 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/api/urls.py
+-rw-r--r--   0        0        0     3570 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/api/views.py
+-rw-r--r--   0        0        0     2794 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/conftest.py
+-rw-r--r--   0        0        0      789 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/sentry.py
+-rw-r--r--   0        0        0     8039 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/settings.py
+-rw-r--r--   0        0        0        0 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/tests/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/tests/test_sentry.py
+-rw-r--r--   0        0        0      615 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/tests/test_settings.py
+-rw-r--r--   0        0        0      225 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/urls.py
+-rw-r--r--   0        0        0      412 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/document_merge_service/wsgi.py
+-rw-r--r--   0        0        0     3496 2023-05-04 06:11:41.886065 document_merge_service-6.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 document_merge_service-6.1.1/PKG-INFO
```

### Comparing `document_merge_service-6.1.0/CHANGELOG.md` & `document_merge_service-6.1.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 # Changelog
+## 6.1.1 (03 May 2023)
+### Fix
+* **excel:** Set `sheet_name` and `tpl_name` to load the correct sheet
+([`13a2a07`](https://github.com/adfinis/document-merge-service/commit/13a2a073aa1a7f65cbf7c794210f460db1a2509e))
 ## 6.1.0 (27 January 2023)
 ### Feature
 * **filters:** Add template meta filter ([`2daf8ec`](https://github.com/Yelinz/document-merge-service/commit/2daf8ec736a9ff5ee424548ef9eef53362e284e0))
 * Add sentry integration ([`abe37f1`](https://github.com/Yelinz/document-merge-service/commit/abe37f1417554119299acb8aa852892bae823490))
 
 ### Fix
 * **auth:** Add userinfo to authenticated user ([`21ae809`](https://github.com/Yelinz/document-merge-service/commit/21ae809dd6e08d1b5823373637ef17805640d73a))
```

### Comparing `document_merge_service-6.1.0/LICENSE` & `document_merge_service-6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/README.md` & `document_merge_service-6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/authentication.py` & `document_merge_service-6.1.1/document_merge_service/api/authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/data/black.png` & `document_merge_service-6.1.1/document_merge_service/api/data/black.png`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/data/docx-mailmerge-syntax.docx` & `document_merge_service-6.1.1/document_merge_service/api/data/docx-mailmerge-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/data/docx-mailmerge.docx` & `document_merge_service-6.1.1/document_merge_service/api/data/docx-mailmerge.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/data/docx-template-filters.docx` & `document_merge_service-6.1.1/document_merge_service/api/data/docx-template-filters.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/data/docx-template-loopcontrols.docx` & `document_merge_service-6.1.1/document_merge_service/api/data/docx-template-loopcontrols.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/data/docx-template-placeholdercheck.docx` & `document_merge_service-6.1.1/document_merge_service/api/data/docx-template-placeholdercheck.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/data/docx-template-syntax.docx` & `document_merge_service-6.1.1/document_merge_service/api/data/docx-template-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/data/docx-template.docx` & `document_merge_service-6.1.1/document_merge_service/api/data/docx-template.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/data/loadtest/1.doc` & `document_merge_service-6.1.1/document_merge_service/api/data/loadtest/1.doc`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/data/loadtest/2.docx` & `document_merge_service-6.1.1/document_merge_service/api/data/loadtest/2.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/data/loadtest/3.docx` & `document_merge_service-6.1.1/document_merge_service/api/data/loadtest/3.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/data/loadtest/4.docx` & `document_merge_service-6.1.1/document_merge_service/api/data/loadtest/4.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/data/xlsx-syntax.xlsx` & `document_merge_service-6.1.1/document_merge_service/api/data/xlsx-syntax.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/data/xlsx-template.xlsx` & `document_merge_service-6.1.1/document_merge_service/api/data/xlsx-template.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/engines.py` & `document_merge_service-6.1.1/document_merge_service/api/engines.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,16 +264,22 @@
         self._current_data = data
 
         writer.jinja_env.filters.update(get_jinja_filters())
         if is_test_merge:
             writer.jinja_env.undefined = self._undefined_factory
         writer.jinja_env.globals.update(dir=dir, getattr=getattr)
 
-        data = [data] * len(writer.sheet_resource_map.sheet_state_list)
-        writer.render_book(payloads=data)
+        payloads = []
+        sheets = writer.sheet_resource_map.sheet_state_list
+        for sheet in sheets:
+            new = dict(data)
+            new["sheet_name"] = sheet.name
+            new["tpl_name"] = sheet.name
+            payloads.append(new)
+        writer.render_book(payloads=payloads)
         writer.save(buf)
         return buf
 
     def _undefined_factory(self, name):
         # For test merges, we set a custom "undefined" factory that
         # doesn't really do undefined, but just fetches the right value
         # from our magic placeholder structure
```

### Comparing `document_merge_service-6.1.0/document_merge_service/api/filters.py` & `document_merge_service-6.1.1/document_merge_service/api/filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/jinja.py` & `document_merge_service-6.1.1/document_merge_service/api/jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/management/commands/clean_dangling_files.py` & `document_merge_service-6.1.1/document_merge_service/api/management/commands/clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/migrations/0001_initial.py` & `document_merge_service-6.1.1/document_merge_service/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py` & `document_merge_service-6.1.1/document_merge_service/api/migrations/0005_xlsx_template_engine.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/models.py` & `document_merge_service-6.1.1/document_merge_service/api/models.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/serializers.py` & `document_merge_service-6.1.1/document_merge_service/api/serializers.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/tests/snapshots/snap_test_template.py` & `document_merge_service-6.1.1/document_merge_service/api/tests/snapshots/snap_test_template.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/tests/test_authentication.py` & `document_merge_service-6.1.1/document_merge_service/api/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/tests/test_clean_dangling_files.py` & `document_merge_service-6.1.1/document_merge_service/api/tests/test_clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/tests/test_excel.py` & `document_merge_service-6.1.1/document_merge_service/api/tests/test_excel.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,25 +15,29 @@
     "key2": [
         "mixed",
         "list",
         {"subkey2": "xdata2"},
     ],
 }
 
+_expect_name = ["test", "another"]
+
 
 def test_render():
     tmpl = django_file("xlsx-structure.xlsx")
     engine = XlsxTemplateEngine(tmpl)
     buf = io.BytesIO()
     engine.merge(_structure, buf)
     buf.seek(0)
     doc = openpyxl.load_workbook(buf)
-    for ws in doc.worksheets:
+    for i, ws in enumerate(doc.worksheets):
+        assert ws.title == _expect_name[i]
         assert ws["A1"].value == "xdata0"
         assert ws["A2"].value == "xdata1"
+        assert ws["A3"].value == _expect_name[i]
         assert ws["A5"].value == "Item: mixed"
         assert ws["A6"].value == "Item: list"
         assert ws["A7"].value == "Subitem: xdata2"
 
 
 @pytest.mark.parametrize(
     "available, expect_success",
```

### Comparing `document_merge_service-6.1.0/document_merge_service/api/tests/test_filters.py` & `document_merge_service-6.1.1/document_merge_service/api/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/tests/test_jinja.py` & `document_merge_service-6.1.1/document_merge_service/api/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/tests/test_pagination.py` & `document_merge_service-6.1.1/document_merge_service/api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/tests/test_template.py` & `document_merge_service-6.1.1/document_merge_service/api/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/tests/test_unoconv.py` & `document_merge_service-6.1.1/document_merge_service/api/tests/test_unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/unoconv.py` & `document_merge_service-6.1.1/document_merge_service/api/unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/api/views.py` & `document_merge_service-6.1.1/document_merge_service/api/views.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/conftest.py` & `document_merge_service-6.1.1/document_merge_service/conftest.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/sentry.py` & `document_merge_service-6.1.1/document_merge_service/sentry.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/settings.py` & `document_merge_service-6.1.1/document_merge_service/settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/document_merge_service/tests/test_settings.py` & `document_merge_service-6.1.1/document_merge_service/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.0/pyproject.toml` & `document_merge_service-6.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "document-merge-service"
-version = "6.1.0"
+version = "6.1.1"
 description = "Merge Document Template Service"
 license = "GPL-3.0-or-later"
 authors = ["Adfinis AG <info@adfinis.com>"]
 homepage = "https://github.com/adfinis/document-merge-service"
 repository = "https://github.com/adfinis/document-merge-service"
 documentation = "https://github.com/adfinis/document-merge-service/blob/main/README.md"
 readme = "README.md"
@@ -91,15 +91,16 @@
 line_length = 88
 
 [tool.pytest.ini_options]
 addopts = "--reuse-db --randomly-seed=1521188766 --randomly-dont-reorganize"
 DJANGO_SETTINGS_MODULE = "document_merge_service.settings"
 filterwarnings = """
     error::DeprecationWarning
-    error::PendingDeprecationWarning"""
+    error::PendingDeprecationWarning
+    ignore:invalid escape sequence"""
 env = """
     ADMINS=Test Example <test@example.com>,Test2 <test2@example.com>
     OIDC_USERINFO_ENDPOINT=mock://document-merge-service.github.com/openid/userinfo
     OIDC_BEARER_TOKEN_REVALIDATION_TIME=60"""
 
 [tool.coverage.run]
 source = ["."]
```

### Comparing `document_merge_service-6.1.0/PKG-INFO` & `document_merge_service-6.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document-merge-service
-Version: 6.1.0
+Version: 6.1.1
 Summary: Merge Document Template Service
 Home-page: https://github.com/adfinis/document-merge-service
 License: GPL-3.0-or-later
 Author: Adfinis AG
 Author-email: info@adfinis.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

