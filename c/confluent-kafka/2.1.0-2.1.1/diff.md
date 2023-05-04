# Comparing `tmp/confluent-kafka-2.1.0.tar.gz` & `tmp/confluent_kafka-2.1.1-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/confluent-kafka-2.1.0.tar", last modified: Thu Apr  6 09:49:45 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

