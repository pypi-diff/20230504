# Comparing `tmp/Reda_Utils-1.1.0.tar.gz` & `tmp/Reda_Utils-2.0.0-py2-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Reda_Utils-1.1.0.tar", last modified: Mon Sep 26 06:36:03 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

