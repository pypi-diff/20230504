# Comparing `tmp/rfrenchseti_cspyce-0.0.0.tar.gz` & `tmp/rfrenchseti_cspyce-2.0.10.dev0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfrenchseti_cspyce-0.0.0.tar", last modified: Wed May  3 23:51:23 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

