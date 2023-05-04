# Comparing `tmp/JoBase-2.6.tar.gz` & `tmp/JoBase-2.7-cp37-cp37m-musllinux_1_1_s390x.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JoBase-2.6.tar", last modified: Fri Feb 17 17:36:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

