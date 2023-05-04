# Comparing `tmp/cloudshell-rest-api-8.2.4.0.tar.gz` & `tmp/cloudshell-rest-api-9.0.0.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudshell-rest-api-8.2.4.0.tar", last modified: Sun Nov  3 12:55:15 2019, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

