# Comparing `tmp/vepar-2.4.tar.gz` & `tmp/vepar-2.5-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vepar-2.4.tar", last modified: Sat Mar 12 18:25:52 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

