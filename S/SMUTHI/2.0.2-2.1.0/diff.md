# Comparing `tmp/SMUTHI-2.0.2.tar.gz` & `tmp/SMUTHI-2.1.0-cp38-cp38-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SMUTHI-2.0.2.tar", last modified: Thu Nov 17 16:55:31 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

