# Comparing `tmp/hsmm_mvpy-0.0.8b0.tar.gz` & `tmp/hsmm_mvpy-0.1.0a0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsmm_mvpy-0.0.8b0.tar", last modified: Wed Nov  2 10:46:50 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

