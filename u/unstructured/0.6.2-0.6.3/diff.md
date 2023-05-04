# Comparing `tmp/unstructured-0.6.2.tar.gz` & `tmp/unstructured-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.6.2.tar", last modified: Wed Apr 26 20:32:28 2023, max compression
+gzip compressed data, was "unstructured-0.6.3.tar", last modified: Thu May  4 20:26:31 2023, max compression
```

## Comparing `unstructured-0.6.2.tar` & `unstructured-0.6.3.tar`

### file list

```diff
@@ -1,105 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.080474 unstructured-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-26 20:32:16.000000 unstructured-0.6.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-04-26 20:32:28.080474 unstructured-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-04-26 20:32:16.000000 unstructured-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-26 20:32:28.080474 unstructured-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-26 20:32:16.000000 unstructured-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.068474 unstructured-0.6.2/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.068474 unstructured-0.6.2/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-26 20:32:16.000000 unstructured-0.6.2/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 20:32:16.000000 unstructured-0.6.2/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-26 20:32:16.000000 unstructured-0.6.2/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-26 20:32:16.000000 unstructured-0.6.2/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.068474 unstructured-0.6.2/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.068474 unstructured-0.6.2/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.068474 unstructured-0.6.2/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.072474 unstructured-0.6.2/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.072474 unstructured-0.6.2/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.072474 unstructured-0.6.2/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.072474 unstructured-0.6.2/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27999 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.072474 unstructured-0.6.2/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.076474 unstructured-0.6.2/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.080474 unstructured-0.6.2/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/text_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.080474 unstructured-0.6.2/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.068474 unstructured-0.6.2/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-04-26 20:32:27.000000 unstructured-0.6.2/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-26 20:32:28.000000 unstructured-0.6.2/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:32:27.000000 unstructured-0.6.2/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-26 20:32:27.000000 unstructured-0.6.2/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-26 20:32:27.000000 unstructured-0.6.2/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 20:32:27.000000 unstructured-0.6.2/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.823834 unstructured-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-04 20:26:22.000000 unstructured-0.6.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21094 2023-05-04 20:26:31.823834 unstructured-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16837 2023-05-04 20:26:22.000000 unstructured-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-04 20:26:31.823834 unstructured-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-04 20:26:22.000000 unstructured-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.807834 unstructured-0.6.3/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.807834 unstructured-0.6.3/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-04 20:26:22.000000 unstructured-0.6.3/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-04 20:26:22.000000 unstructured-0.6.3/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-04 20:26:22.000000 unstructured-0.6.3/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-04 20:26:22.000000 unstructured-0.6.3/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.811833 unstructured-0.6.3/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.811833 unstructured-0.6.3/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.811833 unstructured-0.6.3/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.811833 unstructured-0.6.3/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.811833 unstructured-0.6.3/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.811833 unstructured-0.6.3/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.815834 unstructured-0.6.3/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27999 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.815834 unstructured-0.6.3/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.819834 unstructured-0.6.3/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.819834 unstructured-0.6.3/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/text_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.819834 unstructured-0.6.3/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.811833 unstructured-0.6.3/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21094 2023-05-04 20:26:31.000000 unstructured-0.6.3/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-04 20:26:31.000000 unstructured-0.6.3/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:26:31.000000 unstructured-0.6.3/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 20:26:31.000000 unstructured-0.6.3/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-04 20:26:31.000000 unstructured-0.6.3/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 20:26:31.000000 unstructured-0.6.3/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.6.2/LICENSE.md` & `unstructured-0.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/PKG-INFO` & `unstructured-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.2
+Version: 0.6.3
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -17,14 +17,16 @@
         
           <a href="https://github.com/Unstructured-IO/unstructured/blob/main/LICENSE.md">![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/unstructured.svg)</a>
           <a href="https://pypi.python.org/pypi/unstructured/">![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/pyversions/unstructured.svg)</a>
           <a href="https://GitHub.com/unstructured-io/unstructured/graphs/contributors">![https://GitHub.com/unstructured-io/unstructured.js/graphs/contributors](https://img.shields.io/github/contributors/unstructured-io/unstructured)</a>
           <a href="https://github.com/Unstructured-IO/unstructured/blob/main/CODE_OF_CONDUCT.md">![code_of_conduct.md](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg) </a>
           <a href="https://GitHub.com/unstructured-io/unstructured/releases">![https://GitHub.com/unstructured-io/unstructured.js/releases](https://img.shields.io/github/release/unstructured-io/unstructured)</a>
           <a href="https://pypi.python.org/pypi/unstructured/">![https://github.com/Naereen/badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)</a>
+          [![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/project/unstructured)
+          [![Downloads](https://static.pepy.tech/badge/unstructured/month)](https://pepy.tech/project/unstructured)
         
         </div>
         
         <div>
           <p align="center">
           <a
           href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
@@ -36,15 +38,15 @@
         </div>
         <h2 align="center">
           <p>Announcement!!!</p>
         </h2>
         <div align="center">
           <p>We're excited to announce the public release of the unstructured.io hosted API! Now you can leverage Unstructured with a simple API call to render clean text in JSON format out of your images, documents, powerpoints, and more.</p>
         
-        <p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. You’ll also find instructions there about how to host your own version of the API. Unstructured data just got easier! 
+        <p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. You’ll also find instructions there about how to host your own version of the API. Unstructured data just got easier!
         We'd love to hear your feedback, let us know how it goes in our <a
           href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
            community slack</a>. And stay tuned for improvements to both quality and performance over the coming months!
         <p><img src="easy.gif"></p></p>
         </div>
         
         <h3 align="center">
@@ -183,15 +185,16 @@
         you can also uninstall the hooks with `pre-commit uninstall`.
         
         ## :clap: Quick Tour
         
         You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
         
         The following examples show how to get started with the `unstructured` library.
-        You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**, **PPT**, **PPTX**, **JPG**,
+        You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
+        **ODT**, **PPT**, **PPTX**, **JPG**,
         and **PNG** documents with one line of code!
         <br></br>
         See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
         of the features in the library.
         
         ### Document Parsing
```

#### html2text {}

```diff
@@ -1,22 +1,25 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.2 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.3 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
     img.shields.io/pypi/pyversions/unstructured.svg) ![https://GitHub.com/
  unstructured-io/unstructured.js/graphs/contributors](https://img.shields.io/
 github/contributors/unstructured-io/unstructured) ![code_of_conduct.md](https:/
     /img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg) ![https://
  GitHub.com/unstructured-io/unstructured.js/releases](https://img.shields.io/
   github/release/unstructured-io/unstructured) ![https://github.com/Naereen/
 badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)
+[![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/
+      project/unstructured) [![Downloads](https://static.pepy.tech/badge/
+         unstructured/month)](https://pepy.tech/project/unstructured)
      [https://img.shields.io/badge/JOIN_US_ON_SLACK-4A154B?style=for-the-
    badge&logo=slack&logoColor=white] [https://img.shields.io/badge/LinkedIn-
            0077B5?style=for-the-badge&logo=linkedin&logoColor=white]
                           ***** Announcement!!! *****
 We're excited to announce the public release of the unstructured.io hosted API!
  Now you can leverage Unstructured with a simple API call to render clean text
      in JSON format out of your images, documents, powerpoints, and more.
@@ -109,15 +112,16 @@
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
 show how to get started with the `unstructured` library. You can parse **TXT**,
 **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-**PPT**, **PPTX**, **JPG**, and **PNG** documents with one line of code!
+**ODT**, **PPT**, **PPTX**, **JPG**, and **PNG** documents with one line of
+code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
```

### Comparing `unstructured-0.6.2/README.md` & `unstructured-0.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
   <a href="https://github.com/Unstructured-IO/unstructured/blob/main/LICENSE.md">![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/unstructured.svg)</a>
   <a href="https://pypi.python.org/pypi/unstructured/">![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/pyversions/unstructured.svg)</a>
   <a href="https://GitHub.com/unstructured-io/unstructured/graphs/contributors">![https://GitHub.com/unstructured-io/unstructured.js/graphs/contributors](https://img.shields.io/github/contributors/unstructured-io/unstructured)</a>
   <a href="https://github.com/Unstructured-IO/unstructured/blob/main/CODE_OF_CONDUCT.md">![code_of_conduct.md](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg) </a>
   <a href="https://GitHub.com/unstructured-io/unstructured/releases">![https://GitHub.com/unstructured-io/unstructured.js/releases](https://img.shields.io/github/release/unstructured-io/unstructured)</a>
   <a href="https://pypi.python.org/pypi/unstructured/">![https://github.com/Naereen/badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)</a>
+  [![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/project/unstructured)
+  [![Downloads](https://static.pepy.tech/badge/unstructured/month)](https://pepy.tech/project/unstructured)
 
 </div>
 
 <div>
   <p align="center">
   <a
   href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
@@ -28,15 +30,15 @@
 </div>
 <h2 align="center">
   <p>Announcement!!!</p>
 </h2>
 <div align="center">
   <p>We're excited to announce the public release of the unstructured.io hosted API! Now you can leverage Unstructured with a simple API call to render clean text in JSON format out of your images, documents, powerpoints, and more.</p>
 
-<p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. You’ll also find instructions there about how to host your own version of the API. Unstructured data just got easier! 
+<p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. You’ll also find instructions there about how to host your own version of the API. Unstructured data just got easier!
 We'd love to hear your feedback, let us know how it goes in our <a
   href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
    community slack</a>. And stay tuned for improvements to both quality and performance over the coming months!
 <p><img src="easy.gif"></p></p>
 </div>
 
 <h3 align="center">
@@ -175,15 +177,16 @@
 you can also uninstall the hooks with `pre-commit uninstall`.
 
 ## :clap: Quick Tour
 
 You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
 
 The following examples show how to get started with the `unstructured` library.
-You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**, **PPT**, **PPTX**, **JPG**,
+You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
+**ODT**, **PPT**, **PPTX**, **JPG**,
 and **PNG** documents with one line of code!
 <br></br>
 See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
 of the features in the library.
 
 ### Document Parsing
```

#### html2text {}

```diff
@@ -5,14 +5,17 @@
     img.shields.io/pypi/pyversions/unstructured.svg) ![https://GitHub.com/
  unstructured-io/unstructured.js/graphs/contributors](https://img.shields.io/
 github/contributors/unstructured-io/unstructured) ![code_of_conduct.md](https:/
     /img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg) ![https://
  GitHub.com/unstructured-io/unstructured.js/releases](https://img.shields.io/
   github/release/unstructured-io/unstructured) ![https://github.com/Naereen/
 badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)
+[![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/
+      project/unstructured) [![Downloads](https://static.pepy.tech/badge/
+         unstructured/month)](https://pepy.tech/project/unstructured)
      [https://img.shields.io/badge/JOIN_US_ON_SLACK-4A154B?style=for-the-
    badge&logo=slack&logoColor=white] [https://img.shields.io/badge/LinkedIn-
            0077B5?style=for-the-badge&logo=linkedin&logoColor=white]
                           ***** Announcement!!! *****
 We're excited to announce the public release of the unstructured.io hosted API!
  Now you can leverage Unstructured with a simple API call to render clean text
      in JSON format out of your images, documents, powerpoints, and more.
@@ -105,15 +108,16 @@
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
 show how to get started with the `unstructured` library. You can parse **TXT**,
 **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-**PPT**, **PPTX**, **JPG**, and **PNG** documents with one line of code!
+**ODT**, **PPT**, **PPTX**, **JPG**, and **PNG** documents with one line of
+code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
```

### Comparing `unstructured-0.6.2/setup.py` & `unstructured-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     install_requires=[
         "argilla",
         "lxml",
         "msg_parser",
         "nltk",
         "openpyxl",
         "pandas",
+        "pdfminer.six",
         "pillow",
         "pypandoc",
         "python-docx",
         "python-pptx",
         "python-magic",
         "markdown",
         "requests",
```

### Comparing `unstructured-0.6.2/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.6.3/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.6.3/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/test_unstructured/test_utils.py` & `unstructured-0.6.3/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/cleaners/core.py` & `unstructured-0.6.3/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/cleaners/extract.py` & `unstructured-0.6.3/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/cleaners/translate.py` & `unstructured-0.6.3/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/documents/base.py` & `unstructured-0.6.3/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/documents/elements.py` & `unstructured-0.6.3/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/documents/email_elements.py` & `unstructured-0.6.3/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/documents/html.py` & `unstructured-0.6.3/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/documents/xml.py` & `unstructured-0.6.3/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/file_utils/exploration.py` & `unstructured-0.6.3/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/file_utils/file_conversion.py` & `unstructured-0.6.3/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/file_utils/filetype.py` & `unstructured-0.6.3/unstructured/file_utils/filetype.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
 ]
 
 DOC_MIME_TYPES = [
     "application/msword",
 ]
 
+ODT_MIME_TYPES = [
+    "application/vnd.oasis.opendocument.text",
+]
+
 XLSX_MIME_TYPES = [
     "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
 ]
 
 XLS_MIME_TYPES = [
     "application/vnd.ms-excel",
 ]
@@ -110,14 +114,17 @@
     XML = 51
     MD = 52
     EPUB = 53
 
     # Compressed Types
     ZIP = 60
 
+    # Open Office Types
+    ODT = 70
+
     # NOTE(robinson) - This is to support sorting for pandas groupby functions
     def __lt__(self, other):
         return self.name < other.name
 
 
 STR_TO_FILETYPE = {
     "application/pdf": FileType.PDF,
@@ -131,14 +138,15 @@
     "application/epub+zip": FileType.EPUB,
     "text/html": FileType.HTML,
     "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet": FileType.XLSX,
     "application/vnd.ms-excel": FileType.XLS,
     "application/vnd.openxmlformats-officedocument.presentationml.presentation": FileType.PPTX,
     "application/vnd.ms-powerpoint": FileType.PPT,
     "application/xml": FileType.XML,
+    "application/vnd.oasis.opendocument.text": FileType.ODT,
 }
 
 
 EXT_TO_FILETYPE = {
     ".pdf": FileType.PDF,
     ".docx": FileType.DOCX,
     ".jpg": FileType.JPG,
@@ -156,14 +164,15 @@
     ".zip": FileType.ZIP,
     ".xls": FileType.XLS,
     ".ppt": FileType.PPT,
     ".rtf": FileType.RTF,
     ".json": FileType.JSON,
     ".epub": FileType.EPUB,
     ".msg": FileType.MSG,
+    ".odt": FileType.ODT,
     None: FileType.UNK,
 }
 
 
 def detect_filetype(
     filename: Optional[str] = None,
     content_type: Optional[str] = None,
@@ -217,14 +226,17 @@
 
     elif mime_type in DOCX_MIME_TYPES:
         return FileType.DOCX
 
     elif mime_type in DOC_MIME_TYPES:
         return FileType.DOC
 
+    elif mime_type in ODT_MIME_TYPES:
+        return FileType.ODT
+
     elif mime_type in MSG_MIME_TYPES:
         return FileType.MSG
 
     elif mime_type == "image/jpeg":
         return FileType.JPG
 
     elif mime_type == "image/png":
```

### Comparing `unstructured-0.6.2/unstructured/file_utils/metadata.py` & `unstructured-0.6.3/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/connector/azure.py` & `unstructured-0.6.3/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/connector/biomed.py` & `unstructured-0.6.3/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/connector/fsspec.py` & `unstructured-0.6.3/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/connector/git.py` & `unstructured-0.6.3/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/connector/github.py` & `unstructured-0.6.3/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/connector/gitlab.py` & `unstructured-0.6.3/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/connector/google_drive.py` & `unstructured-0.6.3/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/connector/local.py` & `unstructured-0.6.3/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/connector/reddit.py` & `unstructured-0.6.3/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/connector/s3.py` & `unstructured-0.6.3/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/connector/slack.py` & `unstructured-0.6.3/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.6.3/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.6.3/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/interfaces.py` & `unstructured-0.6.3/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/ingest/main.py` & `unstructured-0.6.3/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/nlp/english-words.txt` & `unstructured-0.6.3/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/nlp/english_words.py` & `unstructured-0.6.3/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/nlp/patterns.py` & `unstructured-0.6.3/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/nlp/tokenize.py` & `unstructured-0.6.3/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/partition/__init__.py` & `unstructured-0.6.3/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/partition/api.py` & `unstructured-0.6.3/unstructured/partition/image.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,83 +1,76 @@
-from typing import (
-    IO,
-    List,
-    Optional,
-)
+from typing import List, Optional
 
-import requests
+import pytesseract
+from PIL import Image
 
 from unstructured.documents.elements import Element
 from unstructured.partition.common import exactly_one
-from unstructured.partition.json import partition_json
+from unstructured.partition.pdf import partition_pdf_or_image
+from unstructured.partition.text import partition_text
 
+VALID_STRATEGIES = ["hi_res", "ocr_only"]
 
-def partition_via_api(
-    filename: Optional[str] = None,
-    content_type: Optional[str] = None,
-    file: Optional[IO] = None,
-    file_filename: Optional[str] = None,
+
+def partition_image(
+    filename: str = "",
+    file: Optional[bytes] = None,
+    url: Optional[str] = None,
+    template: Optional[str] = None,
+    token: Optional[str] = None,
+    include_page_breaks: bool = False,
+    ocr_languages: str = "eng",
     strategy: str = "hi_res",
-    api_url: str = "https://api.unstructured.io/general/v0/general",
-    api_key: str = "",
 ) -> List[Element]:
-    """Partitions a document using the Unstructured REST API. This is equivalent to
-    running the document through partition.
-
-    See https://api.unstructured.io/general/docs for the hosted API documentation or
-    https://github.com/Unstructured-IO/unstructured-api for instructions on how to run
-    the API locally as a container.
+    """Parses an image into a list of interpreted elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
-    content_type
-        A string defining the file content in MIME type
     file
-        A file-like object using "rb" mode --> open(filename, "rb").
-    file_filename
-        When file is not None, the filename (string) to store in element metadata. E.g. "foo.txt"
+        A file-like object as bytes --> open(filename, "rb").
+    template
+        A string defining the model to be used. Default None uses default model ("layout/image" url
+        if using the API).
+    url
+        A string endpoint to self-host an inference API, if desired. If None, local inference will
+        be used.
+    token
+        A string defining the authentication token for a self-host url, if applicable.
+    ocr_languages
+        The languages to use for the Tesseract agent. To use a language, you'll first need
+        to install the appropriate Tesseract language pack.
     strategy
-        The strategy to use for partitioning the PDF. Uses a layout detection model if set
-        to 'hi_res', otherwise partition_pdf simply extracts the text from the document
-        and processes it.
-    api_url
-        The URL for the Unstructured API. Defaults to the hosted Unstructured API.
-    api_key
-        The API key to pass to the Unstructured API.
+        The strategy to use for partitioning the PDF. Valid strategies are "hi_res" and
+        "ocr_only". When using the "hi_res" strategy, the function  ses a layout detection
+        model if to identify document elements. When using the "ocr_only strategy",
+        partition_image simply extracts the text from the document and processes it.
     """
     exactly_one(filename=filename, file=file)
 
-    headers = {
-        "ACCEPT": "application/json",
-        "UNSTRUCTURED-API-KEY": api_key,
-    }
-
-    data = {
-        "strategy": strategy,
-    }
-
-    if filename is not None:
-        with open(filename, "rb") as f:
-            files = [
-                ("files", (filename, f, content_type)),
-            ]
-            response = requests.post(
-                api_url,
-                headers=headers,
-                data=data,
-                files=files,  # type: ignore
-            )
-    elif file is not None:
-        _filename = file_filename or ""
-        files = [
-            ("files", (_filename, file, content_type)),  # type: ignore
-        ]
-        response = requests.post(api_url, headers=headers, data=data, files=files)  # type: ignore
+    if strategy == "hi_res":
+        if template is None:
+            template = "layout/image"
+        return partition_pdf_or_image(
+            filename=filename,
+            file=file,
+            url=url,
+            template=template,
+            token=token,
+            include_page_breaks=include_page_breaks,
+            ocr_languages=ocr_languages,
+        )
+
+    elif strategy == "ocr_only":
+        if file is not None:
+            image = Image.open(file)
+            text = pytesseract.image_to_string(image, config=f"-l '{ocr_languages}'")
+        else:
+            text = pytesseract.image_to_string(filename, config=f"-l '{ocr_languages}'")
+        return partition_text(text=text)
 
-    if response.status_code == 200:
-        return partition_json(text=response.text)
     else:
         raise ValueError(
-            f"Receive unexpected status code {response.status_code} from the API.",
+            f"{strategy} is not a valid strategy for partition_image. "
+            f"Choose one of {VALID_STRATEGIES}.",
         )
```

### Comparing `unstructured-0.6.2/unstructured/partition/auto.py` & `unstructured-0.6.3/unstructured/partition/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from unstructured.partition.email import partition_email
 from unstructured.partition.epub import partition_epub
 from unstructured.partition.html import partition_html
 from unstructured.partition.image import partition_image
 from unstructured.partition.json import partition_json
 from unstructured.partition.md import partition_md
 from unstructured.partition.msg import partition_msg
+from unstructured.partition.odt import partition_odt
 from unstructured.partition.pdf import partition_pdf
 from unstructured.partition.ppt import partition_ppt
 from unstructured.partition.pptx import partition_pptx
 from unstructured.partition.rtf import partition_rtf
 from unstructured.partition.text import partition_text
 
 
@@ -102,14 +103,16 @@
     if file is not None:
         file.seek(0)
 
     if filetype == FileType.DOC:
         elements = partition_doc(filename=filename, file=file)
     elif filetype == FileType.DOCX:
         elements = partition_docx(filename=filename, file=file)
+    elif filetype == FileType.ODT:
+        elements = partition_odt(filename=filename, file=file)
     elif filetype == FileType.EML:
         elements = partition_email(filename=filename, file=file, encoding=encoding)
     elif filetype == FileType.MSG:
         elements = partition_msg(filename=filename, file=file)
     elif filetype == FileType.HTML:
         elements = partition_html(
             filename=filename,
```

### Comparing `unstructured-0.6.2/unstructured/partition/common.py` & `unstructured-0.6.3/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/partition/doc.py` & `unstructured-0.6.3/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/partition/docx.py` & `unstructured-0.6.3/unstructured/partition/docx.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import os
+import tempfile
 from typing import IO, List, Optional
 
 import docx
+import pypandoc
 
 from unstructured.cleaners.core import clean_bullets
 from unstructured.documents.elements import (
     Address,
     Element,
     ElementMetadata,
     ListItem,
@@ -128,7 +131,50 @@
         return None
     elif is_possible_narrative_text(text):
         return NarrativeText(text)
     elif is_possible_title(text):
         return Title(text)
     else:
         return Text(text)
+
+
+def convert_and_partition_docx(
+    source_format: str,
+    filename: Optional[str] = None,
+    file: Optional[IO] = None,
+) -> List[Element]:
+    """Converts a document to DOCX and then partitions it using partition_html. Works with
+    any file format support by pandoc.
+
+    Parameters
+    ----------
+    source_format
+        The format of the source document, .e.g. odt
+    filename
+        A string defining the target filename path.
+    file
+        A file-like object using "rb" mode --> open(filename, "rb").
+    """
+    if filename is None:
+        filename = ""
+    exactly_one(filename=filename, file=file)
+
+    if len(filename) > 0:
+        _, filename_no_path = os.path.split(os.path.abspath(filename))
+        base_filename, _ = os.path.splitext(filename_no_path)
+        if not os.path.exists(filename):
+            raise ValueError(f"The file {filename} does not exist.")
+    elif file is not None:
+        tmp = tempfile.NamedTemporaryFile(delete=False)
+        tmp.write(file.read())
+        tmp.close()
+        filename = tmp.name
+        _, filename_no_path = os.path.split(os.path.abspath(tmp.name))
+
+    base_filename, _ = os.path.splitext(filename_no_path)
+
+    with tempfile.TemporaryDirectory() as tmpdir:
+        docx_filename = os.path.join(tmpdir, f"{base_filename}.docx")
+        pypandoc.convert_file(filename, "docx", format=source_format, outputfile=docx_filename)
+        elements = partition_docx(filename=docx_filename, metadata_filename=filename)
+
+    return elements
```

### Comparing `unstructured-0.6.2/unstructured/partition/email.py` & `unstructured-0.6.3/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/partition/epub.py` & `unstructured-0.6.3/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/partition/html.py` & `unstructured-0.6.3/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/partition/json.py` & `unstructured-0.6.3/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/partition/md.py` & `unstructured-0.6.3/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/partition/msg.py` & `unstructured-0.6.3/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/partition/pdf.py` & `unstructured-0.6.3/unstructured/partition/pdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import re
 import warnings
-from io import StringIO
 from typing import BinaryIO, List, Optional, cast
 
+from pdfminer.high_level import extract_pages
 from pdfminer.pdfpage import PDFPage, PDFTextExtractionNotAllowed
 from pdfminer.utils import open_filename
 
+from unstructured.cleaners.core import clean_extra_whitespace
 from unstructured.documents.elements import Element, ElementMetadata, PageBreak
 from unstructured.logger import logger
+from unstructured.nlp.patterns import PARAGRAPH_PATTERN
 from unstructured.partition import _partition_via_api
 from unstructured.partition.common import (
     add_element_metadata,
     document_to_element_list,
     exactly_one,
 )
 from unstructured.partition.text import partition_text
@@ -281,39 +284,37 @@
 def _process_pdfminer_pages(
     fp: BinaryIO,
     filename: str = "",
     encoding: str = "utf-8",
     include_page_breaks: bool = False,
 ):
     """Uses PDF miner to split a document into pages and process them."""
-    from pdfminer.converter import TextConverter
-    from pdfminer.layout import LAParams
-    from pdfminer.pdfinterp import PDFPageInterpreter, PDFResourceManager
-
-    rsrcmgr = PDFResourceManager(caching=False)
-    laparams = LAParams()
-
     elements: List[Element] = []
 
-    for i, page in enumerate(PDFPage.get_pages(fp, check_extractable=True)):
+    for i, page in enumerate(extract_pages(fp)):  # type: ignore
         metadata = ElementMetadata(filename=filename, page_number=i + 1)
-        with StringIO() as output_string:
-            device = TextConverter(
-                rsrcmgr,
-                output_string,
-                codec=encoding,
-                laparams=laparams,
-            )
-            interpreter = PDFPageInterpreter(rsrcmgr, device)
-            interpreter.process_page(page)
-            text = output_string.getvalue()
-            _elements = partition_text(text=text)
-            for element in _elements:
-                element.metadata = metadata
-                elements.append(element)
+
+        text_segments = []
+        for obj in page:
+            # NOTE(robinson) - "Figure" is an example of an object type that does
+            # not have a get_text method
+            if not hasattr(obj, "get_text"):
+                continue
+            _text = obj.get_text()
+            _text = re.sub(PARAGRAPH_PATTERN, " ", _text)
+            _text = clean_extra_whitespace(_text)
+            if _text.strip():
+                text_segments.append(_text)
+
+        text = "\n\n".join(text_segments)
+
+        _elements = partition_text(text=text)
+        for element in _elements:
+            element.metadata = metadata
+            elements.append(element)
 
         if include_page_breaks:
             elements.append(PageBreak())
 
     return elements
```

### Comparing `unstructured-0.6.2/unstructured/partition/ppt.py` & `unstructured-0.6.3/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/partition/pptx.py` & `unstructured-0.6.3/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/partition/rtf.py` & `unstructured-0.6.3/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/partition/text.py` & `unstructured-0.6.3/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/partition/text_type.py` & `unstructured-0.6.3/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/staging/argilla.py` & `unstructured-0.6.3/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/staging/base.py` & `unstructured-0.6.3/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/staging/datasaur.py` & `unstructured-0.6.3/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/staging/huggingface.py` & `unstructured-0.6.3/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/staging/label_box.py` & `unstructured-0.6.3/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/staging/label_studio.py` & `unstructured-0.6.3/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/staging/prodigy.py` & `unstructured-0.6.3/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured/utils.py` & `unstructured-0.6.3/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.2/unstructured.egg-info/PKG-INFO` & `unstructured-0.6.3/unstructured.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.2
+Version: 0.6.3
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -17,14 +17,16 @@
         
           <a href="https://github.com/Unstructured-IO/unstructured/blob/main/LICENSE.md">![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/unstructured.svg)</a>
           <a href="https://pypi.python.org/pypi/unstructured/">![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/pyversions/unstructured.svg)</a>
           <a href="https://GitHub.com/unstructured-io/unstructured/graphs/contributors">![https://GitHub.com/unstructured-io/unstructured.js/graphs/contributors](https://img.shields.io/github/contributors/unstructured-io/unstructured)</a>
           <a href="https://github.com/Unstructured-IO/unstructured/blob/main/CODE_OF_CONDUCT.md">![code_of_conduct.md](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg) </a>
           <a href="https://GitHub.com/unstructured-io/unstructured/releases">![https://GitHub.com/unstructured-io/unstructured.js/releases](https://img.shields.io/github/release/unstructured-io/unstructured)</a>
           <a href="https://pypi.python.org/pypi/unstructured/">![https://github.com/Naereen/badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)</a>
+          [![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/project/unstructured)
+          [![Downloads](https://static.pepy.tech/badge/unstructured/month)](https://pepy.tech/project/unstructured)
         
         </div>
         
         <div>
           <p align="center">
           <a
           href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
@@ -36,15 +38,15 @@
         </div>
         <h2 align="center">
           <p>Announcement!!!</p>
         </h2>
         <div align="center">
           <p>We're excited to announce the public release of the unstructured.io hosted API! Now you can leverage Unstructured with a simple API call to render clean text in JSON format out of your images, documents, powerpoints, and more.</p>
         
-        <p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. You’ll also find instructions there about how to host your own version of the API. Unstructured data just got easier! 
+        <p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. You’ll also find instructions there about how to host your own version of the API. Unstructured data just got easier!
         We'd love to hear your feedback, let us know how it goes in our <a
           href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
            community slack</a>. And stay tuned for improvements to both quality and performance over the coming months!
         <p><img src="easy.gif"></p></p>
         </div>
         
         <h3 align="center">
@@ -183,15 +185,16 @@
         you can also uninstall the hooks with `pre-commit uninstall`.
         
         ## :clap: Quick Tour
         
         You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
         
         The following examples show how to get started with the `unstructured` library.
-        You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**, **PPT**, **PPTX**, **JPG**,
+        You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
+        **ODT**, **PPT**, **PPTX**, **JPG**,
         and **PNG** documents with one line of code!
         <br></br>
         See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
         of the features in the library.
         
         ### Document Parsing
```

#### html2text {}

```diff
@@ -1,22 +1,25 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.2 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.3 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
     img.shields.io/pypi/pyversions/unstructured.svg) ![https://GitHub.com/
  unstructured-io/unstructured.js/graphs/contributors](https://img.shields.io/
 github/contributors/unstructured-io/unstructured) ![code_of_conduct.md](https:/
     /img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg) ![https://
  GitHub.com/unstructured-io/unstructured.js/releases](https://img.shields.io/
   github/release/unstructured-io/unstructured) ![https://github.com/Naereen/
 badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)
+[![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/
+      project/unstructured) [![Downloads](https://static.pepy.tech/badge/
+         unstructured/month)](https://pepy.tech/project/unstructured)
      [https://img.shields.io/badge/JOIN_US_ON_SLACK-4A154B?style=for-the-
    badge&logo=slack&logoColor=white] [https://img.shields.io/badge/LinkedIn-
            0077B5?style=for-the-badge&logo=linkedin&logoColor=white]
                           ***** Announcement!!! *****
 We're excited to announce the public release of the unstructured.io hosted API!
  Now you can leverage Unstructured with a simple API call to render clean text
      in JSON format out of your images, documents, powerpoints, and more.
@@ -109,15 +112,16 @@
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
 show how to get started with the `unstructured` library. You can parse **TXT**,
 **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-**PPT**, **PPTX**, **JPG**, and **PNG** documents with one line of code!
+**ODT**, **PPT**, **PPTX**, **JPG**, and **PNG** documents with one line of
+code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
```

### Comparing `unstructured-0.6.2/unstructured.egg-info/SOURCES.txt` & `unstructured-0.6.3/unstructured.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -69,21 +69,23 @@
 unstructured/partition/email.py
 unstructured/partition/epub.py
 unstructured/partition/html.py
 unstructured/partition/image.py
 unstructured/partition/json.py
 unstructured/partition/md.py
 unstructured/partition/msg.py
+unstructured/partition/odt.py
 unstructured/partition/pdf.py
 unstructured/partition/ppt.py
 unstructured/partition/pptx.py
 unstructured/partition/rtf.py
 unstructured/partition/text.py
 unstructured/partition/text_type.py
 unstructured/staging/__init__.py
 unstructured/staging/argilla.py
 unstructured/staging/base.py
+unstructured/staging/baseplate.py
 unstructured/staging/datasaur.py
 unstructured/staging/huggingface.py
 unstructured/staging/label_box.py
 unstructured/staging/label_studio.py
 unstructured/staging/prodigy.py
```

