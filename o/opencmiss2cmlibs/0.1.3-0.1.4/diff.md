# Comparing `tmp/opencmiss2cmlibs-0.1.3.tar.gz` & `tmp/opencmiss2cmlibs-0.1.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencmiss2cmlibs-0.1.3.tar", last modified: Wed May  3 23:31:21 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

