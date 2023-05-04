# Comparing `tmp/rxnplot-0.9.1.tar.gz` & `tmp/rxnplot-0.9.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rxnplot-0.9.1.tar", last modified: Sun Jan 29 18:29:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

