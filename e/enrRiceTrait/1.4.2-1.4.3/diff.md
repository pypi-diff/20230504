# Comparing `tmp/enrRiceTrait-1.4.2.tar.gz` & `tmp/enrRiceTrait-1.4.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enrRiceTrait-1.4.2.tar", last modified: Thu May  4 14:51:06 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

