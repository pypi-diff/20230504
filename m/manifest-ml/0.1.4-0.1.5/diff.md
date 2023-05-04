# Comparing `tmp/manifest-ml-0.1.4.tar.gz` & `tmp/manifest-ml-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifest-ml-0.1.4.tar", last modified: Mon Apr 24 22:34:12 2023, max compression
+gzip compressed data, was "manifest-ml-0.1.5.tar", last modified: Thu May  4 04:44:00 2023, max compression
```

## Comparing `manifest-ml-0.1.4.tar` & `manifest-ml-0.1.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.988283 manifest-ml-0.1.4/
--rw-r--r--   0 laurelorr   (501) staff       (20)    11357 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/LICENSE
--rw-r--r--   0 laurelorr   (501) staff       (20)    10067 2023-04-24 22:34:12.988099 manifest-ml-0.1.4/PKG-INFO
--rw-r--r--   0 laurelorr   (501) staff       (20)     9379 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/README.md
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.978902 manifest-ml-0.1.4/manifest/
--rw-r--r--   0 laurelorr   (501) staff       (20)      183 2023-03-12 04:05:54.000000 manifest-ml-0.1.4/manifest/__init__.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.979548 manifest-ml-0.1.4/manifest/api/
--rw-r--r--   0 laurelorr   (501) staff       (20)       16 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/api/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     8947 2023-04-16 20:56:11.000000 manifest-ml-0.1.4/manifest/api/app.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.981051 manifest-ml-0.1.4/manifest/api/models/
--rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/api/models/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     4383 2023-04-09 06:56:02.000000 manifest-ml-0.1.4/manifest/api/models/diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    23121 2023-04-09 06:56:02.000000 manifest-ml-0.1.4/manifest/api/models/huggingface.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2798 2023-04-09 06:56:02.000000 manifest-ml-0.1.4/manifest/api/models/model.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3880 2023-04-09 06:56:02.000000 manifest-ml-0.1.4/manifest/api/models/sentence_transformer.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1767 2023-04-17 05:07:52.000000 manifest-ml-0.1.4/manifest/api/response.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.982433 manifest-ml-0.1.4/manifest/caches/
--rw-r--r--   0 laurelorr   (501) staff       (20)       18 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/caches/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3725 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/caches/array_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     4386 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/caches/cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1131 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/caches/noop.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3944 2023-03-12 04:05:54.000000 manifest-ml-0.1.4/manifest/caches/postgres.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1716 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/caches/redis.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5997 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/caches/serializers.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1772 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/caches/sqlite.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.984583 manifest-ml-0.1.4/manifest/clients/
--rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/clients/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3303 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/ai21.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    13421 2023-04-24 18:39:09.000000 manifest-ml-0.1.4/manifest/clients/client.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3461 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/cohere.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2821 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     4510 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/dummy.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3751 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/huggingface.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2336 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/huggingface_embedding.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     4810 2023-04-24 19:18:15.000000 manifest-ml-0.1.4/manifest/clients/openai.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5132 2023-04-09 06:56:02.000000 manifest-ml-0.1.4/manifest/clients/openai_chat.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     6560 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/openai_embedding.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5164 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/toma.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1940 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/toma_diffuser.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.985183 manifest-ml-0.1.4/manifest/connections/
--rw-r--r--   0 laurelorr   (501) staff       (20)       23 2023-04-17 05:07:52.000000 manifest-ml-0.1.4/manifest/connections/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5947 2023-04-17 05:07:52.000000 manifest-ml-0.1.4/manifest/connections/client_pool.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1227 2023-04-17 05:07:52.000000 manifest-ml-0.1.4/manifest/connections/scheduler.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    18277 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/manifest.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3000 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/request.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    10750 2023-04-24 19:16:26.000000 manifest-ml-0.1.4/manifest/response.py
--rw-r--r--   0 laurelorr   (501) staff       (20)       22 2023-04-12 20:16:25.000000 manifest-ml-0.1.4/manifest/version.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.985822 manifest-ml-0.1.4/manifest_ml.egg-info/
--rw-r--r--   0 laurelorr   (501) staff       (20)    10067 2023-04-24 22:34:12.000000 manifest-ml-0.1.4/manifest_ml.egg-info/PKG-INFO
--rw-r--r--   0 laurelorr   (501) staff       (20)     1568 2023-04-24 22:34:12.000000 manifest-ml-0.1.4/manifest_ml.egg-info/SOURCES.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)        1 2023-04-24 22:34:12.000000 manifest-ml-0.1.4/manifest_ml.egg-info/dependency_links.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)     1615 2023-04-24 22:34:12.000000 manifest-ml-0.1.4/manifest_ml.egg-info/requires.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)       17 2023-04-24 22:34:12.000000 manifest-ml-0.1.4/manifest_ml.egg-info/top_level.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)      786 2023-04-09 06:56:02.000000 manifest-ml-0.1.4/pyproject.toml
--rw-r--r--   0 laurelorr   (501) staff       (20)       38 2023-04-24 22:34:12.988327 manifest-ml-0.1.4/setup.cfg
--rw-r--r--   0 laurelorr   (501) staff       (20)     5349 2023-04-12 20:13:43.000000 manifest-ml-0.1.4/setup.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.987443 manifest-ml-0.1.4/tests/
--rw-r--r--   0 laurelorr   (501) staff       (20)     2275 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/tests/test_array_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     8152 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/tests/test_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2446 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/tests/test_client.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2294 2023-04-17 05:07:52.000000 manifest-ml-0.1.4/tests/test_client_pool.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     9132 2023-04-09 06:56:02.000000 manifest-ml-0.1.4/tests/test_huggingface_api.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    36113 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/tests/test_manifest.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1949 2023-03-12 04:05:54.000000 manifest-ml-0.1.4/tests/test_request.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    10431 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/tests/test_response.py
--rw-r--r--   0 laurelorr   (501) staff       (20)      769 2023-04-17 05:07:52.000000 manifest-ml-0.1.4/tests/test_scheduler.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1073 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/tests/test_serializer.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.987870 manifest-ml-0.1.4/web_app/
--rw-r--r--   0 laurelorr   (501) staff       (20)       36 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/web_app/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1737 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/web_app/main.py
--rw-r--r--   0 laurelorr   (501) staff       (20)      721 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/web_app/schemas.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.204735 manifest-ml-0.1.5/
+-rw-r--r--   0 laurelorr   (501) staff       (20)    11357 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/LICENSE
+-rw-r--r--   0 laurelorr   (501) staff       (20)    10682 2023-05-04 04:44:00.204545 manifest-ml-0.1.5/PKG-INFO
+-rw-r--r--   0 laurelorr   (501) staff       (20)     9994 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/README.md
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.195734 manifest-ml-0.1.5/manifest/
+-rw-r--r--   0 laurelorr   (501) staff       (20)      183 2023-03-12 04:05:54.000000 manifest-ml-0.1.5/manifest/__init__.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.196379 manifest-ml-0.1.5/manifest/api/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       16 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/api/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     8947 2023-04-16 20:56:11.000000 manifest-ml-0.1.5/manifest/api/app.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.197708 manifest-ml-0.1.5/manifest/api/models/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/api/models/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4383 2023-04-09 06:56:02.000000 manifest-ml-0.1.5/manifest/api/models/diffuser.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    23121 2023-04-09 06:56:02.000000 manifest-ml-0.1.5/manifest/api/models/huggingface.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2798 2023-04-09 06:56:02.000000 manifest-ml-0.1.5/manifest/api/models/model.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3880 2023-04-09 06:56:02.000000 manifest-ml-0.1.5/manifest/api/models/sentence_transformer.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1767 2023-04-17 05:07:52.000000 manifest-ml-0.1.5/manifest/api/response.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.199231 manifest-ml-0.1.5/manifest/caches/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       18 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/caches/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3725 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/caches/array_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4386 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/caches/cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1131 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/caches/noop.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3944 2023-03-12 04:05:54.000000 manifest-ml-0.1.5/manifest/caches/postgres.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1716 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/caches/redis.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5997 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/caches/serializers.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1772 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/caches/sqlite.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.201139 manifest-ml-0.1.5/manifest/clients/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/manifest/clients/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3303 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/clients/ai21.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    14386 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/clients/client.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3461 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/clients/cohere.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2821 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/clients/diffuser.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5717 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/clients/dummy.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3751 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/clients/huggingface.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2336 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/clients/huggingface_embedding.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4810 2023-04-24 19:18:15.000000 manifest-ml-0.1.5/manifest/clients/openai.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5782 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/clients/openai_chat.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     6560 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/clients/openai_embedding.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5164 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/clients/toma.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1940 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/manifest/clients/toma_diffuser.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.201639 manifest-ml-0.1.5/manifest/connections/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       23 2023-04-17 05:07:52.000000 manifest-ml-0.1.5/manifest/connections/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     6196 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/connections/client_pool.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1227 2023-05-03 06:44:32.000000 manifest-ml-0.1.5/manifest/connections/scheduler.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    22429 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/manifest.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3135 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/request.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    10950 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/manifest/response.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)       22 2023-05-01 03:31:34.000000 manifest-ml-0.1.5/manifest/version.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.202342 manifest-ml-0.1.5/manifest_ml.egg-info/
+-rw-r--r--   0 laurelorr   (501) staff       (20)    10682 2023-05-04 04:43:59.000000 manifest-ml-0.1.5/manifest_ml.egg-info/PKG-INFO
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1568 2023-05-04 04:44:00.000000 manifest-ml-0.1.5/manifest_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)        1 2023-05-04 04:43:59.000000 manifest-ml-0.1.5/manifest_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1615 2023-05-04 04:44:00.000000 manifest-ml-0.1.5/manifest_ml.egg-info/requires.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)       17 2023-05-04 04:44:00.000000 manifest-ml-0.1.5/manifest_ml.egg-info/top_level.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)      786 2023-04-09 06:56:02.000000 manifest-ml-0.1.5/pyproject.toml
+-rw-r--r--   0 laurelorr   (501) staff       (20)       38 2023-05-04 04:44:00.204777 manifest-ml-0.1.5/setup.cfg
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5349 2023-04-12 20:13:43.000000 manifest-ml-0.1.5/setup.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.203918 manifest-ml-0.1.5/tests/
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2275 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/tests/test_array_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     8152 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/tests/test_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2446 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/tests/test_client.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2304 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/tests/test_client_pool.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     9132 2023-04-09 06:56:02.000000 manifest-ml-0.1.5/tests/test_huggingface_api.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    38750 2023-05-04 04:43:35.000000 manifest-ml-0.1.5/tests/test_manifest.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1949 2023-03-12 04:05:54.000000 manifest-ml-0.1.5/tests/test_request.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    10431 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/tests/test_response.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)      769 2023-05-03 06:44:15.000000 manifest-ml-0.1.5/tests/test_scheduler.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1073 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/tests/test_serializer.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-04 04:44:00.204337 manifest-ml-0.1.5/web_app/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       36 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/web_app/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1737 2023-04-24 18:36:42.000000 manifest-ml-0.1.5/web_app/main.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)      721 2023-02-14 19:01:23.000000 manifest-ml-0.1.5/web_app/schemas.py
```

### Comparing `manifest-ml-0.1.4/LICENSE` & `manifest-ml-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/PKG-INFO` & `manifest-ml-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manifest-ml
-Version: 0.1.4
+Version: 0.1.5
 Summary: Manifest for Prompting Foundation Models.
 Home-page: https://github.com/HazyResearch/manifest
 Author: Laurel Orr
 Author-email: laurel.orr@numbersstation.ai
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -27,14 +27,15 @@
 
 
 # Table of Contents
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Manifest](#manifest-components)
 - [Local HuggingFace Models](#local-huggingface-models)
+- [Chat Models](#chat-models)
 - [Embedding Models](#embedding-models)
 - [Road Map](#road-map)
 - [Development](#development)
 - [Cite](#cite)
 
 
 # Install
@@ -99,16 +100,16 @@
 )
 ```
 You can also just set `export COHERE_API_KEY=<COHERE_API_KEY>` and not use `client_connection`.
 
 
 You can see the model details and possible model inputs to `run()` via
 ```python
-print(manifest.client.get_model_params())
-print(manifest.client.get_model_inputs())
+print(manifest.client_pool.get_current_client().get_model_params())
+print(manifest.client_pool.get_current_client().get_model_inputs())
 ```
 
 ## Global Cache
 We support having queries and results stored in a global cache that can be shared across users. We treat inputs and outputs as key value pairs and support SQLite or Redis backends. To start with global caching using SQLite, run
 
 ```python
 manifest = Manifest(
@@ -236,14 +237,26 @@
 python3 -m manifest.api.app \
     --model_type huggingface \
     --model_name_or_path bigscience/bloom \
     --use_bitsandbytes \
     --percent_max_gpu_mem_reduction 0.85
 ```
 
+# Chat Models
+Manifest has specific support for executing against chat models in the more standard "system" / "user" dialogue. To pass in a dialogue history to Manifest, you must use the `run_chat` command with an associated chat model such as `openaichat`.
+
+```python
+manifest = Manifest(client_name="openaichat")
+dialogue = [
+    {"role": "system", "content": "You are a helpful assistant who also responds in rhymes"},
+    {"role": "user", "content": "What is the date?"},
+]
+res = manifest.run_chat(dialogue, max_tokens=100)
+```
+
 # Embedding Models
 Manifest also supports getting embeddings from models and available APIs. We do this all through changing the `client_name` argument. You still use `run` and `abatch_run`.
 
 To use OpenAI's embedding models, simply run
 ```python
 manifest = Manifest(client_name="openaiembedding")
 embedding_as_np = manifest.run("Get me an embedding for a bunny")
```

### Comparing `manifest-ml-0.1.4/README.md` & `manifest-ml-0.1.5/manifest_ml.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,41 @@
+Metadata-Version: 2.1
+Name: manifest-ml
+Version: 0.1.5
+Summary: Manifest for Prompting Foundation Models.
+Home-page: https://github.com/HazyResearch/manifest
+Author: Laurel Orr
+Author-email: laurel.orr@numbersstation.ai
+License: Apache 2.0
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Provides-Extra: api
+Provides-Extra: app
+Provides-Extra: diffusers
+Provides-Extra: gcp
+Provides-Extra: dev
+Provides-Extra: all
+License-File: LICENSE
+
+
 # Manifest
 How to make prompt programming with Foundation Models a little easier.
 
 
 # Table of Contents
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Manifest](#manifest-components)
 - [Local HuggingFace Models](#local-huggingface-models)
+- [Chat Models](#chat-models)
 - [Embedding Models](#embedding-models)
 - [Road Map](#road-map)
 - [Development](#development)
 - [Cite](#cite)
 
 
 # Install
@@ -75,16 +100,16 @@
 )
 ```
 You can also just set `export COHERE_API_KEY=<COHERE_API_KEY>` and not use `client_connection`.
 
 
 You can see the model details and possible model inputs to `run()` via
 ```python
-print(manifest.client.get_model_params())
-print(manifest.client.get_model_inputs())
+print(manifest.client_pool.get_current_client().get_model_params())
+print(manifest.client_pool.get_current_client().get_model_inputs())
 ```
 
 ## Global Cache
 We support having queries and results stored in a global cache that can be shared across users. We treat inputs and outputs as key value pairs and support SQLite or Redis backends. To start with global caching using SQLite, run
 
 ```python
 manifest = Manifest(
@@ -212,14 +237,26 @@
 python3 -m manifest.api.app \
     --model_type huggingface \
     --model_name_or_path bigscience/bloom \
     --use_bitsandbytes \
     --percent_max_gpu_mem_reduction 0.85
 ```
 
+# Chat Models
+Manifest has specific support for executing against chat models in the more standard "system" / "user" dialogue. To pass in a dialogue history to Manifest, you must use the `run_chat` command with an associated chat model such as `openaichat`.
+
+```python
+manifest = Manifest(client_name="openaichat")
+dialogue = [
+    {"role": "system", "content": "You are a helpful assistant who also responds in rhymes"},
+    {"role": "user", "content": "What is the date?"},
+]
+res = manifest.run_chat(dialogue, max_tokens=100)
+```
+
 # Embedding Models
 Manifest also supports getting embeddings from models and available APIs. We do this all through changing the `client_name` argument. You still use `run` and `abatch_run`.
 
 To use OpenAI's embedding models, simply run
 ```python
 manifest = Manifest(client_name="openaiembedding")
 embedding_as_np = manifest.run("Get me an embedding for a bunny")
@@ -262,7 +299,9 @@
   author = {Orr, Laurel},
   title = {Manifest},
   year = {2022},
   publisher = {GitHub},
   howpublished = {\url{https://github.com/HazyResearch/manifest}},
 }
 ```
+
+
```

### Comparing `manifest-ml-0.1.4/manifest/api/app.py` & `manifest-ml-0.1.5/manifest/api/app.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/api/models/diffuser.py` & `manifest-ml-0.1.5/manifest/api/models/diffuser.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/api/models/huggingface.py` & `manifest-ml-0.1.5/manifest/api/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/api/models/model.py` & `manifest-ml-0.1.5/manifest/api/models/model.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/api/models/sentence_transformer.py` & `manifest-ml-0.1.5/manifest/api/models/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/api/response.py` & `manifest-ml-0.1.5/manifest/api/response.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/caches/array_cache.py` & `manifest-ml-0.1.5/manifest/caches/array_cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/caches/cache.py` & `manifest-ml-0.1.5/manifest/caches/cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/caches/noop.py` & `manifest-ml-0.1.5/manifest/caches/noop.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/caches/postgres.py` & `manifest-ml-0.1.5/manifest/caches/postgres.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/caches/redis.py` & `manifest-ml-0.1.5/manifest/caches/redis.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/caches/serializers.py` & `manifest-ml-0.1.5/manifest/caches/serializers.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/caches/sqlite.py` & `manifest-ml-0.1.5/manifest/caches/sqlite.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/clients/ai21.py` & `manifest-ml-0.1.5/manifest/clients/ai21.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/clients/client.py` & `manifest-ml-0.1.5/manifest/clients/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import aiohttp
 import requests
 from tenacity import RetryCallState, retry, stop_after_attempt, wait_random_exponential
 
 from manifest.request import (
     DEFAULT_REQUEST_KEYS,
     NOT_CACHE_KEYS,
+    LMChatRequest,
     LMScoreRequest,
     Request,
 )
 from manifest.response import (
     RESPONSE_CONSTRUCTORS,
     ArrayModelChoice,
     LMModelChoice,
@@ -304,15 +305,15 @@
             ) as res:
                 res.raise_for_status()
                 res_json = await res.json(content_type=None)
                 return self.validate_response(res_json, request_params)
 
     def run_request(self, request: Request) -> Response:
         """
-        Get request string function.
+        Run request.
 
         Args:
             request: request.
 
         Returns:
             response.
         """
@@ -338,15 +339,15 @@
             request=request,
             usages=Usages(usages=usages) if usages else None,
             **RESPONSE_CONSTRUCTORS[self.REQUEST_CLS],  # type: ignore
         )
 
     async def arun_batch_request(self, request: Request) -> Response:
         """
-        Get async request string function.
+        Run async request.
 
         Args:
             request: request.
 
         Returns:
             response.
         """
@@ -392,24 +393,55 @@
             self.get_model_choices(final_response_dict),
             cached=False,
             request=request,
             usages=final_usages,
             **RESPONSE_CONSTRUCTORS[self.REQUEST_CLS],  # type: ignore
         )
 
-    def get_score_prompt_request(
+    def run_chat_request(
+        self,
+        request: LMChatRequest,
+    ) -> Response:
+        """
+        Get the response from chat model.
+
+        Args:
+            request: request.
+
+        Returns:
+            response.
+        """
+        request_params = self.get_request_params(request)
+        # Take the default keys we need and drop the rest as they
+        # are not part of the model request.
+        retry_timeout = request_params.pop("client_timeout")
+        for key in DEFAULT_REQUEST_KEYS:
+            request_params.pop(key, None)
+        response_dict = self._run_completion(request_params, retry_timeout)
+        usages = None
+        if "usage" in response_dict:
+            usages = [Usage(**usage) for usage in response_dict["usage"]]
+
+        return Response(
+            response=self.get_model_choices(response_dict),
+            cached=False,
+            request=request,
+            usages=Usages(usages=usages) if usages else None,
+            **RESPONSE_CONSTRUCTORS[LMChatRequest],  # type: ignore
+        )
+
+    def run_score_prompt_request(
         self,
         request: LMScoreRequest,
     ) -> Response:
         """
         Get the logit score of the prompt via a forward pass of the model.
 
         Args:
             request: request.
 
         Returns:
-            request function that takes no input.
-            request parameters as dict.
+            response.
         """
         raise NotImplementedError(
             f"{self.__class__.__name__} does not support prompt scoring request."
         )
```

### Comparing `manifest-ml-0.1.4/manifest/clients/cohere.py` & `manifest-ml-0.1.5/manifest/clients/cohere.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/clients/diffuser.py` & `manifest-ml-0.1.5/manifest/clients/diffuser.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/clients/huggingface.py` & `manifest-ml-0.1.5/manifest/clients/huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         Returns:
             model params.
         """
         res = requests.post(self.host + "/params").json()
         res["client_name"] = self.NAME
         return res
 
-    def get_score_prompt_request(
+    def run_score_prompt_request(
         self,
         request: LMScoreRequest,
     ) -> Response:
         """
         Get the logit score of the prompt via a forward pass of the model.
 
         Args:
```

### Comparing `manifest-ml-0.1.4/manifest/clients/huggingface_embedding.py` & `manifest-ml-0.1.5/manifest/clients/huggingface_embedding.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/clients/openai.py` & `manifest-ml-0.1.5/manifest/clients/openai.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/clients/openai_chat.py` & `manifest-ml-0.1.5/manifest/clients/openai_chat.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,18 +88,31 @@
         Returns:
             formatted request params.
         """
         # Format for chat model
         request_params = copy.deepcopy(request_params)
         prompt = request_params.pop("prompt")
         if isinstance(prompt, str):
-            prompt_list = [prompt]
-        else:
+            messages = [{"role": "user", "content": prompt}]
+        elif isinstance(prompt, list) and isinstance(prompt[0], str):
             prompt_list = prompt
-        messages = [{"role": "user", "content": prompt} for prompt in prompt_list]
+            messages = [{"role": "user", "content": prompt} for prompt in prompt_list]
+        elif isinstance(prompt, list) and isinstance(prompt[0], dict):
+            for pmt_dict in prompt:
+                if "role" not in pmt_dict or "content" not in pmt_dict:
+                    raise ValueError(
+                        "Prompt must be list of dicts with 'role' and 'content' "
+                        f"keys. Got {prompt}."
+                    )
+            messages = prompt
+        else:
+            raise ValueError(
+                "Prompt must be string, list of strings, or list of dicts."
+                f"Got {prompt}"
+            )
         request_params["messages"] = messages
         return request_params
 
     def _format_request_from_chat(self, response_dict: Dict[str, Any]) -> Dict:
         """Format response for standard response from chat.
 
         Args:
```

### Comparing `manifest-ml-0.1.4/manifest/clients/openai_embedding.py` & `manifest-ml-0.1.5/manifest/clients/openai_embedding.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/clients/toma.py` & `manifest-ml-0.1.5/manifest/clients/toma.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/clients/toma_diffuser.py` & `manifest-ml-0.1.5/manifest/clients/toma_diffuser.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/connections/client_pool.py` & `manifest-ml-0.1.5/manifest/connections/client_pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,20 +154,28 @@
         self.client_pool_metrics = [Timing() for _ in self.client_pool]
 
     def close(self) -> None:
         """Close."""
         for client in self.client_pool:
             client.close()
 
-    def get_client(self) -> Client:
+    def num_clients(self) -> int:
+        """Get number of clients."""
+        return len(self.client_pool)
+
+    def get_next_client(self) -> Client:
         """Get client."""
         client_int = self.scheduler.get_client()
         self.current_client_id = client_int
         return self.client_pool[client_int]
 
+    def get_current_client(self) -> Client:
+        """Get current client."""
+        return self.client_pool[self.current_client_id]
+
     def start_timer(self) -> None:
         """Start timer."""
         self.client_pool_metrics[self.current_client_id].start = time.time()
 
     def end_timer(self) -> None:
         """End timer."""
         self.client_pool_metrics[self.current_client_id].end = time.time()
```

### Comparing `manifest-ml-0.1.4/manifest/connections/scheduler.py` & `manifest-ml-0.1.5/manifest/connections/scheduler.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest/manifest.py` & `manifest-ml-0.1.5/manifest/manifest.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from manifest.clients.client import Client
 from manifest.clients.huggingface import HuggingFaceClient
 from manifest.connections.client_pool import (
     CLIENT_CONSTRUCTORS,
     ClientConnection,
     ClientConnectionPool,
 )
-from manifest.request import LMScoreRequest, Request
+from manifest.request import LMChatRequest, LMScoreRequest, Request
 from manifest.response import ModelChoices, Response, Usage, Usages
 
 logging.getLogger("openai").setLevel(logging.WARNING)
 logger = logging.getLogger(__name__)
 
 
 CACHE_CONSTRUCTORS = {
@@ -138,55 +138,79 @@
         Returns:
             cached_idx_to_response: dict of cached responses.
             new_request: request object with only prompts to run.
         """
         cached_idx_to_response: Dict[int, Response] = {}
         new_request = copy.deepcopy(request)
         if not overwrite_cache:
-            if isinstance(new_request.prompt, list):
+            if isinstance(new_request.prompt, list) and not isinstance(
+                request, LMChatRequest
+            ):
                 new_request.prompt = []
                 for idx, prompt_str in enumerate(request.prompt):
                     single_request = copy.deepcopy(request)
                     single_request.prompt = prompt_str
                     possible_response = self.cache.get(
                         client.get_cache_key(single_request)
                     )
                     if possible_response:
                         cached_idx_to_response[idx] = possible_response
                     else:
                         new_request.prompt.append(prompt_str)
-            else:
+            # Chat or single string requests are not broken down into
+            # subprompts for caching.
+            elif (isinstance(new_request.prompt, str)) or (
+                isinstance(new_request.prompt, list)
+                and isinstance(request, LMChatRequest)
+            ):
                 possible_response = self.cache.get(client.get_cache_key(new_request))
                 if possible_response:
                     cached_idx_to_response[0] = possible_response
                     new_request.prompt = None
+            else:
+                raise ValueError(
+                    f"Invalid prompt type: {type(new_request.prompt)}"
+                    f" with request type: {type(request)}"
+                )
         return cached_idx_to_response, new_request
 
     def _stitch_responses_and_cache(
         self,
         request: Request,
         client: Client,
         response: Union[Response, None],
         cached_idx_to_response: Dict[int, Response],
     ) -> Response:
         """Stich together the cached and uncached responses."""
         # We stitch the responses (the choices) here from both the new request the
         # cached entries.
         all_model_choices = []
         all_usages = []
-        all_input_prompts = []
+        all_input_prompts: List[Union[str, List[str], List[Dict]]] = []
         response_idx = 0
         number_prompts = len(cached_idx_to_response)
-        single_output = False
+        single_completion_output = False
         if response:
             if isinstance(response.get_request_obj().prompt, str):
-                single_output = True
+                single_completion_output = True
                 number_prompts += 1
-            else:
+            elif isinstance(response.get_request_obj().prompt, list) and not isinstance(
+                request, LMChatRequest
+            ):
                 number_prompts += len(response.get_request_obj().prompt)
+            elif isinstance(response.get_request_obj().prompt, list) and isinstance(
+                request, LMChatRequest
+            ):
+                assert len(cached_idx_to_response) <= 1
+                number_prompts += 1
+            else:
+                raise ValueError(
+                    f"Invalid prompt type: {type(response.get_request_obj().prompt)}"
+                    f" with request type: {type(request)}"
+                )
         response_type = None
         request_type: Type[Request] = None
         for idx in range(number_prompts):
             if idx in cached_idx_to_response:
                 cached_res = cached_idx_to_response[idx]
                 response_type = cached_res._response_type
                 request_type = cached_res._request_type
@@ -206,39 +230,53 @@
                 # the choices list in the response is a flat one.
                 # length is request.n * num_prompts
                 current_choices = response.get_response_obj().choices[
                     response_idx * request.n : (response_idx + 1) * request.n
                 ]
                 all_model_choices.extend(current_choices)
 
-                if isinstance(response.get_request_obj().prompt, list):
-                    prompt = response.get_request_obj().prompt[response_idx]
+                if isinstance(
+                    response.get_request_obj().prompt, list
+                ) and not isinstance(request, LMChatRequest):
+                    prompt: Union[
+                        str, List[str], List[Dict]
+                    ] = response.get_request_obj().prompt[response_idx]
+                # Chat request
+                elif isinstance(response.get_request_obj().prompt, list) and isinstance(
+                    request, LMChatRequest
+                ):
+                    # We will only have response_idx == 0 here as we can only
+                    # support single chat requests.
+                    assert request.n == 1
+                    assert number_prompts <= 1
+                    prompt = response.get_request_obj().prompt
                 else:
                     prompt = str(response.get_request_obj().prompt)
+
                 usages: Optional[List[Usage]] = None
                 if response.get_usage_obj().usages:
                     usages = response.get_usage_obj().usages[
                         response_idx * request.n : (response_idx + 1) * request.n
                     ]
                     all_usages.extend(usages)
                 all_input_prompts.append(prompt)
                 # set cache
                 new_request = copy.deepcopy(request)
-                new_request.prompt = prompt
+                new_request.prompt = prompt  # type: ignore
                 cache_key = client.get_cache_key(new_request)
                 new_response = copy.deepcopy(response)
                 new_response._response.choices = current_choices
                 new_response._usages = Usages(usages=(usages or []))
                 self.cache.set(cache_key, new_response.to_dict(drop_request=True))
                 response_idx += 1
 
         new_request = copy.deepcopy(request)
         new_request.prompt = (
             all_input_prompts  # type: ignore
-            if len(all_input_prompts) > 1 or not single_output
+            if len(all_input_prompts) > 1 or not single_completion_output
             else all_input_prompts[0]
         )
         response_obj = Response(
             response=ModelChoices(choices=all_model_choices),
             cached=len(cached_idx_to_response) > 0,
             request=new_request,
             usages=Usages(usages=all_usages),
@@ -267,15 +305,15 @@
             return_response: whether to return Response object.
 
         Returns:
             response from prompt.
         """
         is_batch = isinstance(prompt, list)
         # Get the client to run
-        client = self.client_pool.get_client()
+        client = self.client_pool.get_next_client()
         stop_token = stop_token if stop_token is not None else self.stop_token
         # Must pass kwargs as dict for client "pop" methods removed used arguments
         request_params = client.get_request(prompt, kwargs)
         # Avoid nested list of results - enforce n = 1 for batch
         if is_batch and request_params.n > 1:
             raise ValueError("Batch mode does not support n > 1.")
         self._validate_kwargs(kwargs, request_params)
@@ -344,18 +382,18 @@
             response from prompt.
         """
         # Split the prompts into chunks
         prompt_chunks: List[Tuple[Client, List[str]]] = []
         if chunk_size > 0:
             for i in range(0, len(prompts), chunk_size):
                 prompt_chunks.append(
-                    (self.client_pool.get_client(), prompts[i : i + chunk_size])
+                    (self.client_pool.get_next_client(), prompts[i : i + chunk_size])
                 )
         else:
-            prompt_chunks = [(self.client_pool.get_client(), prompts)]
+            prompt_chunks = [(self.client_pool.get_next_client(), prompts)]
 
         # Run the chunks
         tasks = []
         for client, chunk in prompt_chunks:
             tasks.append(
                 asyncio.create_task(
                     self._arun_batch_client(
@@ -422,14 +460,75 @@
             request=request_params,
             client=client,
             response=response,
             cached_idx_to_response=cached_idx_to_response,
         )
         return final_response
 
+    def run_chat(
+        self,
+        prompt: List[Dict[str, str]],
+        overwrite_cache: bool = False,
+        return_response: bool = False,
+        **kwargs: Any,
+    ) -> Union[str, Response]:
+        """
+        Run the prompt.
+
+        Args:
+            prompt: prompt dictionary to run.
+            overwrite_cache: whether to overwrite cache.
+            stop_token: stop token for prompt generation.
+                        Default is self.stop_token.
+                        "" for no stop token.
+            return_response: whether to return Response object.
+
+        Returns:
+            response from prompt.
+        """
+        is_batch = False
+        # Get the client to run
+        client = self.client_pool.get_next_client()
+        # Get a request for an empty prompt to handle all kwargs
+        request_params = client.get_request("", kwargs)
+        # Add prompt and cast as chat request
+        request_params_dict = request_params.to_dict()
+        request_params_dict["prompt"] = prompt
+        request_params_as_chat = LMChatRequest(**request_params_dict)
+        # Avoid nested list of results - enforce n = 1 for batch
+        if request_params_as_chat.n > 1:
+            raise ValueError("Chat mode does not support n > 1.")
+        self._validate_kwargs(kwargs, request_params_as_chat)
+
+        cached_idx_to_response, request_params_as_chat = self._split_cached_requests(  # type: ignore # noqa: E501
+            request_params_as_chat, client, overwrite_cache
+        )
+        # If not None value or empty list - run new request
+        if request_params_as_chat.prompt:
+            # Start timing metrics
+            self.client_pool.start_timer()
+            response = client.run_chat_request(request_params_as_chat)
+            self.client_pool.end_timer()
+        else:
+            # Nothing to run
+            response = None
+
+        final_response = self._stitch_responses_and_cache(
+            request=request_params_as_chat,
+            client=client,
+            response=response,
+            cached_idx_to_response=cached_idx_to_response,
+        )
+
+        # Extract text results
+        if return_response:
+            return final_response
+        else:
+            return cast(str, final_response.get_response("", is_batch))
+
     def score_prompt(
         self,
         prompt: Union[str, List[str]],
         overwrite_cache: bool = False,
         **kwargs: Any,
     ) -> Dict:
         """
@@ -440,30 +539,30 @@
         Args:
             prompt: prompt(s) to run.
             overwrite_cache: whether to overwrite cache.
 
         Returns:
             response from prompt.
         """
-        client = self.client_pool.get_client()
+        client = self.client_pool.get_next_client()
         # Must pass kwargs as dict for client "pop" methods removed used arguments
         request_params = client.get_request(prompt, kwargs)
         request_params_as_score = LMScoreRequest(**request_params.to_dict())
 
         if request_params_as_score.n > 1:
             raise ValueError("Sequence scoring does not support n > 1.")
         self._validate_kwargs(kwargs, request_params_as_score)
 
         cached_idx_to_response, request_params_as_score = self._split_cached_requests(  # type: ignore # noqa: E501
             request_params_as_score, client, overwrite_cache
         )
         # If not None value or empty list - run new request
         if request_params_as_score.prompt:
             try:
-                response = cast(HuggingFaceClient, client).get_score_prompt_request(
+                response = cast(HuggingFaceClient, client).run_score_prompt_request(
                     request_params_as_score
                 )
             except AttributeError:
                 raise ValueError("`score_prompt` only supported for HF models.")
         else:
             # Nothing to run
             response = None
```

### Comparing `manifest-ml-0.1.4/manifest/request.py` & `manifest-ml-0.1.5/manifest/request.py`

 * *Files 16% similar despite different names*

```diff
@@ -97,14 +97,20 @@
     # Penalize resence
     presence_penalty: float = 0
 
     # Penalize frequency
     frequency_penalty: float = 0
 
 
+class LMChatRequest(LMRequest):
+    """Language Model Chat Request object."""
+
+    prompt: List[Dict[str, str]] = {}  # type: ignore
+
+
 class LMScoreRequest(LMRequest):
     """Language Model Score Request object."""
 
     pass
 
 
 class EmbeddingRequest(Request):
```

### Comparing `manifest-ml-0.1.4/manifest/response.py` & `manifest-ml-0.1.5/manifest/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 import numpy as np
 from pydantic import BaseModel
 
 from manifest.request import (
     ENGINE_SEP,
     DiffusionRequest,
     EmbeddingRequest,
+    LMChatRequest,
     LMRequest,
     LMScoreRequest,
     Request,
 )
 
 RESPONSE_CONSTRUCTORS: Dict[Type[Request], Dict[str, Union[str, Type[Request]]]] = {
     LMRequest: {"response_type": "text", "request_type": LMRequest},
+    LMChatRequest: {"response_type": "text", "request_type": LMChatRequest},
     LMScoreRequest: {"response_type": "text", "request_type": LMScoreRequest},
     EmbeddingRequest: {"response_type": "array", "request_type": EmbeddingRequest},
     DiffusionRequest: {"response_type": "array", "request_type": DiffusionRequest},
 }
 
 
 class NumpyArrayEncoder(json.JSONEncoder):
@@ -287,14 +289,16 @@
                 "Request dictionary must be provided if "
                 "request is not in response dictionary."
             )
         item_dtype = response_dict["item_dtype"]
         response_type = response_dict["response_type"]
         if response_dict["request_type"] == "LMRequest":
             request_type: Type[Request] = LMRequest
+        elif response_dict["request_type"] == "LMChatRequest":
+            request_type = LMChatRequest
         elif response_dict["request_type"] == "LMScoreRequest":
             request_type = LMScoreRequest
         elif response_dict["request_type"] == "EmbeddingRequest":
             request_type = EmbeddingRequest
         elif response_dict["request_type"] == "DiffusionRequest":
             request_type = DiffusionRequest
         choices: List[Union[LMModelChoice, ArrayModelChoice]] = []
```

### Comparing `manifest-ml-0.1.4/manifest_ml.egg-info/PKG-INFO` & `manifest-ml-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,17 @@
-Metadata-Version: 2.1
-Name: manifest-ml
-Version: 0.1.4
-Summary: Manifest for Prompting Foundation Models.
-Home-page: https://github.com/HazyResearch/manifest
-Author: Laurel Orr
-Author-email: laurel.orr@numbersstation.ai
-License: Apache 2.0
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: api
-Provides-Extra: app
-Provides-Extra: diffusers
-Provides-Extra: gcp
-Provides-Extra: dev
-Provides-Extra: all
-License-File: LICENSE
-
-
 # Manifest
 How to make prompt programming with Foundation Models a little easier.
 
 
 # Table of Contents
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Manifest](#manifest-components)
 - [Local HuggingFace Models](#local-huggingface-models)
+- [Chat Models](#chat-models)
 - [Embedding Models](#embedding-models)
 - [Road Map](#road-map)
 - [Development](#development)
 - [Cite](#cite)
 
 
 # Install
@@ -99,16 +76,16 @@
 )
 ```
 You can also just set `export COHERE_API_KEY=<COHERE_API_KEY>` and not use `client_connection`.
 
 
 You can see the model details and possible model inputs to `run()` via
 ```python
-print(manifest.client.get_model_params())
-print(manifest.client.get_model_inputs())
+print(manifest.client_pool.get_current_client().get_model_params())
+print(manifest.client_pool.get_current_client().get_model_inputs())
 ```
 
 ## Global Cache
 We support having queries and results stored in a global cache that can be shared across users. We treat inputs and outputs as key value pairs and support SQLite or Redis backends. To start with global caching using SQLite, run
 
 ```python
 manifest = Manifest(
@@ -236,14 +213,26 @@
 python3 -m manifest.api.app \
     --model_type huggingface \
     --model_name_or_path bigscience/bloom \
     --use_bitsandbytes \
     --percent_max_gpu_mem_reduction 0.85
 ```
 
+# Chat Models
+Manifest has specific support for executing against chat models in the more standard "system" / "user" dialogue. To pass in a dialogue history to Manifest, you must use the `run_chat` command with an associated chat model such as `openaichat`.
+
+```python
+manifest = Manifest(client_name="openaichat")
+dialogue = [
+    {"role": "system", "content": "You are a helpful assistant who also responds in rhymes"},
+    {"role": "user", "content": "What is the date?"},
+]
+res = manifest.run_chat(dialogue, max_tokens=100)
+```
+
 # Embedding Models
 Manifest also supports getting embeddings from models and available APIs. We do this all through changing the `client_name` argument. You still use `run` and `abatch_run`.
 
 To use OpenAI's embedding models, simply run
 ```python
 manifest = Manifest(client_name="openaiembedding")
 embedding_as_np = manifest.run("Get me an embedding for a bunny")
@@ -286,9 +275,7 @@
   author = {Orr, Laurel},
   title = {Manifest},
   year = {2022},
   publisher = {GitHub},
   howpublished = {\url{https://github.com/HazyResearch/manifest}},
 }
 ```
-
-
```

### Comparing `manifest-ml-0.1.4/manifest_ml.egg-info/SOURCES.txt` & `manifest-ml-0.1.5/manifest_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/manifest_ml.egg-info/requires.txt` & `manifest-ml-0.1.5/manifest_ml.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -5,52 +5,52 @@
 aiohttp>=3.8.0
 sqlitedict>=2.0.0
 tenacity>=8.2.0
 tiktoken>=0.3.0
 xxhash>=3.0.0
 
 [all]
-types-requests>=2.27.29
-accelerate>=0.10.0
-Flask>=2.1.2
+deepspeed>=0.7.0
+pre-commit>=2.14.0
+fastapi>=0.70.0
+sqlalchemy
+uvicorn>=0.18.0
 transformers<4.26.0,>=4.20.0
-types-redis>=4.2.6
-pytest>=7.0.0
-pytest-cov>=3.0.0
 diffusers>=0.6.0
-black>=22.3.0
-flake8>=4.0.0
-torch>=1.8.0
+types-PyYAML>=6.0.7
+types-redis>=4.2.6
 pillow>=9.0.0
+docformatter>=1.4
+types-python-dateutil>=2.8.16
 python-dotenv>=0.20.0
-sqlalchemy
+flake8>=4.0.0
+torch>=1.8.0
 types-protobuf>=3.19.21
-recommonmark>=0.7.1
-sentence_transformers>=2.2.0
-types-xxhash>=3.0.0
-pg8000
-pep8-naming>=0.12.1
-deepspeed>=0.7.0
+sphinx-autobuild
 sphinx-rtd-theme>=0.5.1
 nbsphinx>=0.8.0
-twine
-types-PyYAML>=6.0.7
-types-python-dateutil>=2.8.16
-mypy>=0.950
+black>=22.3.0
+recommonmark>=0.7.1
+types-xxhash>=3.0.0
 types-pillow>=9.0.0
-sphinx-autobuild
-docformatter>=1.4
-autopep8>=1.6.0
-uvicorn>=0.18.0
-fastapi>=0.70.0
+Flask>=2.1.2
 cloud-sql-python-connector[pg8000]>=1.0.0
-pre-commit>=2.14.0
+types-requests>=2.27.29
+sentence_transformers>=2.2.0
 isort>=5.9.3
-types-setuptools>=57.4.17
 flake8-docstrings>=1.6.0
+pytest>=7.0.0
+pep8-naming>=0.12.1
+autopep8>=1.6.0
+pytest-cov>=3.0.0
+accelerate>=0.10.0
+types-setuptools>=57.4.17
+mypy>=0.950
+twine
+pg8000
 
 [api]
 accelerate>=0.10.0
 deepspeed>=0.7.0
 diffusers>=0.6.0
 Flask>=2.1.2
 sentence_transformers>=2.2.0
```

### Comparing `manifest-ml-0.1.4/pyproject.toml` & `manifest-ml-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/setup.py` & `manifest-ml-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/tests/test_array_cache.py` & `manifest-ml-0.1.5/tests/test_array_cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/tests/test_cache.py` & `manifest-ml-0.1.5/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/tests/test_client.py` & `manifest-ml-0.1.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/tests/test_client_pool.py` & `manifest-ml-0.1.5/tests/test_client_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,21 +42,21 @@
 
 def test_timing() -> None:
     """Test timing client."""
     client_connection1 = ClientConnection(client_name="dummy")
     client_connection2 = ClientConnection(client_name="dummy")
     connection_pool = ClientConnectionPool([client_connection1, client_connection2])
 
-    connection_pool.get_client()
+    connection_pool.get_next_client()
     assert connection_pool.current_client_id == 0
     connection_pool.start_timer()
     time.sleep(2)
     connection_pool.end_timer()
 
-    connection_pool.get_client()
+    connection_pool.get_next_client()
     assert connection_pool.current_client_id == 1
     connection_pool.start_timer()
     time.sleep(1)
     connection_pool.end_timer()
 
     timing = connection_pool.client_pool_metrics
     assert timing[0].end - timing[0].start > 1.9
```

### Comparing `manifest-ml-0.1.4/tests/test_huggingface_api.py` & `manifest-ml-0.1.5/tests/test_huggingface_api.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/tests/test_manifest.py` & `manifest-ml-0.1.5/tests/test_manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,28 +39,28 @@
 
     manifest = Manifest(
         client_name="dummy",
         cache_name="sqlite",
         cache_connection=sqlite_cache,
     )
     assert len(manifest.client_pool.client_pool) == 1
-    client = manifest.client_pool.get_client()
+    client = manifest.client_pool.get_next_client()
     assert isinstance(client, DummyClient)
     assert isinstance(manifest.cache, SQLiteCache)
     assert client.n == 1  # type: ignore
     assert manifest.stop_token == ""
 
     manifest = Manifest(
         client_name="dummy",
         cache_name="noop",
         n=3,
         stop_token="\n",
     )
     assert len(manifest.client_pool.client_pool) == 1
-    client = manifest.client_pool.get_client()
+    client = manifest.client_pool.get_next_client()
     assert isinstance(client, DummyClient)
     assert isinstance(manifest.cache, NoopCache)
     assert client.n == 3  # type: ignore
     assert manifest.stop_token == "\n"
 
 
 @pytest.mark.usefixtures("sqlite_cache")
@@ -77,15 +77,15 @@
 
     prompt = "This is a prompt"
     with pytest.raises(ValueError) as exc_info:
         result = manifest.run(prompt, return_response=return_response, bad_input=5)
     assert str(exc_info.value) == "[('bad_input', 5)] arguments are not recognized."
 
     # Allow params in the request object but not in the client to go through
-    assert "top_k" not in manifest.client_pool.get_client().PARAMS
+    assert "top_k" not in manifest.client_pool.get_next_client().PARAMS
     result = manifest.run(prompt, return_response=return_response, top_k=5)
     assert result is not None
 
     prompt = "This is a prompt"
     result = manifest.run(prompt, return_response=return_response)
     if return_response:
         assert isinstance(result, Response)
@@ -388,14 +388,66 @@
 
     assert len(result.get_usage_obj().usages) == len(result.get_response_obj().choices)
     res = result.get_response(stop_token="ll", is_batch=True)
     assert res == ["he", "he"]
 
 
 @pytest.mark.usefixtures("sqlite_cache")
+def test_run_chat(sqlite_cache: str) -> None:
+    """Test manifest run."""
+    manifest = Manifest(
+        client_name="dummy",
+        cache_name="sqlite",
+        cache_connection=sqlite_cache,
+    )
+
+    prompt = [
+        {"role": "system", "content": "Hello."},
+    ]
+    result = manifest.run_chat(prompt, return_response=False)
+    assert result == "Hello."
+    assert (
+        manifest.cache.get(
+            {
+                "prompt": [{"content": "Hello.", "role": "system"}],
+                "engine": "dummy",
+                "num_results": 1,
+                "request_cls": "LMChatRequest",
+            },
+        )
+        is not None
+    )
+
+    prompt = [
+        {"role": "system", "content": "Hello."},
+        {"role": "user", "content": "Goodbye?"},
+    ]
+    result = manifest.run_chat(prompt, return_response=True)
+    assert isinstance(result, Response)
+    result = cast(Response, result)
+    assert len(result.get_usage_obj().usages) == len(result.get_response_obj().choices)
+    res = result.get_response()
+    assert res == "Hello."
+    assert (
+        manifest.cache.get(
+            {
+                "prompt": [
+                    {"role": "system", "content": "Hello."},
+                    {"role": "user", "content": "Goodbye?"},
+                ],
+                "engine": "dummy",
+                "num_results": 1,
+                "request_cls": "LMChatRequest",
+            },
+        )
+        is not None
+    )
+
+
+@pytest.mark.usefixtures("sqlite_cache")
 def test_score_run(sqlite_cache: str) -> None:
     """Test manifest run."""
     manifest = Manifest(
         client_name="dummy",
         cache_name="sqlite",
         cache_connection=sqlite_cache,
     )
@@ -784,14 +836,40 @@
     assert response.get_usage_obj().usages[1].total_tokens == 23
 
     response = cast(
         Response, client.run("Why are there oranges?", return_response=True)
     )
     assert response.is_cached() is True
 
+    chat_dict = [
+        {"role": "system", "content": "You are a helpful assistant."},
+        {"role": "user", "content": "Who won the world series in 2020?"},
+        {
+            "role": "assistant",
+            "content": "The Los Angeles Dodgers won the World Series in 2020.",
+        },
+        {"role": "user", "content": "Where was it played?"},
+    ]
+    res = client.run_chat(chat_dict)
+    assert isinstance(res, str) and len(res) > 0
+    response = cast(Response, client.run_chat(chat_dict, return_response=True))
+    assert response.is_cached() is True
+    assert response.get_usage_obj().usages[0].total_tokens == 67
+    chat_dict = [
+        {"role": "system", "content": "You are a helpful assistanttttt."},
+        {"role": "user", "content": "Who won the world series in 2020?"},
+        {
+            "role": "assistant",
+            "content": "The Los Angeles Dodgers won the World Series in 2020.",
+        },
+        {"role": "user", "content": "Where was it played?"},
+    ]
+    response = cast(Response, client.run_chat(chat_dict, return_response=True))
+    assert response.is_cached() is False
+
 
 @pytest.mark.skipif(not OPENAI_ALIVE, reason="No openai key set")
 @pytest.mark.usefixtures("sqlite_cache")
 def test_openaiembedding(sqlite_cache: str) -> None:
     """Test openaichat client."""
     client = Manifest(
         client_name="openaiembedding",
```

### Comparing `manifest-ml-0.1.4/tests/test_request.py` & `manifest-ml-0.1.5/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/tests/test_response.py` & `manifest-ml-0.1.5/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/tests/test_scheduler.py` & `manifest-ml-0.1.5/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/tests/test_serializer.py` & `manifest-ml-0.1.5/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/web_app/main.py` & `manifest-ml-0.1.5/web_app/main.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.4/web_app/schemas.py` & `manifest-ml-0.1.5/web_app/schemas.py`

 * *Files identical despite different names*

