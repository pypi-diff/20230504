# Comparing `tmp/vsdenoise-2.1.3.tar.gz` & `tmp/vsdenoise-2.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsdenoise-2.1.3.tar", last modified: Sun Mar 26 17:40:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

