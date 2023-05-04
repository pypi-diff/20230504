# Comparing `tmp/anltk-1.0.3.tar.gz` & `tmp/anltk-1.0.4-cp38-cp38-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anltk-1.0.3.tar", last modified: Mon Mar 27 07:05:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

