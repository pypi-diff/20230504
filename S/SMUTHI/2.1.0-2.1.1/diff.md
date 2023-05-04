# Comparing `tmp/SMUTHI-2.1.0.tar.gz` & `tmp/SMUTHI-2.1.1-cp36-cp36m-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SMUTHI-2.1.0.tar", last modified: Thu May  4 09:55:53 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

