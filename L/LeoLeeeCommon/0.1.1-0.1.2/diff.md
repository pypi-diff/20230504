# Comparing `tmp/LeoLeeeCommon-0.1.1.tar.gz` & `tmp/LeoLeeeCommon-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LeoLeeeCommon-0.1.1.tar", last modified: Thu May  4 14:22:28 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

