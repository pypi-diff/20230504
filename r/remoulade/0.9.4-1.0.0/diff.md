# Comparing `tmp/remoulade-0.9.4.tar.gz` & `tmp/remoulade-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/remoulade-0.9.4.tar", last modified: Fri Feb 15 17:21:30 2019, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

