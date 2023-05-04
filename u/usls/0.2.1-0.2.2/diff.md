# Comparing `tmp/usls-0.2.1-py3-none-any.whl.zip` & `tmp/usls-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 60625 bytes, number of entries: 23
--rwxrwxrwx  2.0 unx      171 b- defN 23-May-04 03:58 usls/__init__.py
+Zip file size: 60667 bytes, number of entries: 23
+-rwxrwxrwx  2.0 unx      171 b- defN 23-May-04 09:29 usls/__init__.py
 -rwxrwxrwx  2.0 unx    11563 b- defN 23-May-04 03:02 usls/cli.py
 -rwxrwxrwx  2.0 unx     2629 b- defN 23-May-04 03:02 usls/run.py
 -rwxrwxrwx  2.0 unx      309 b- defN 23-May-04 03:02 usls/src/__init__.py
 -rwxrwxrwx  2.0 unx     2171 b- defN 23-May-04 03:02 usls/src/class_modify.py
 -rwxrwxrwx  2.0 unx     6028 b- defN 23-May-04 03:02 usls/src/cleanup.py
 -rwxrwxrwx  2.0 unx     5530 b- defN 23-May-04 03:02 usls/src/deduplicate.py
 -rwxrwxrwx  2.0 unx     1739 b- defN 23-May-04 03:02 usls/src/dir_combine.py
@@ -11,15 +11,15 @@
 -rwxrwxrwx  2.0 unx     3204 b- defN 23-May-04 03:02 usls/src/label_combine.py
 -rwxrwxrwx  2.0 unx    18138 b- defN 23-May-04 03:02 usls/src/labelling_cls.py
 -rwxrwxrwx  2.0 unx    39435 b- defN 23-May-04 03:02 usls/src/labelling_det.py
 -rwxrwxrwx  2.0 unx    40829 b- defN 23-May-04 03:02 usls/src/labelling_det_2.py
 -rwxrwxrwx  2.0 unx     2555 b- defN 23-May-04 03:08 usls/src/rename.py
 -rwxrwxrwx  2.0 unx     3470 b- defN 23-May-04 03:02 usls/src/spider.py
 -rwxrwxrwx  2.0 unx     5906 b- defN 23-May-04 03:02 usls/src/utils.py
--rwxrwxrwx  2.0 unx     9386 b- defN 23-May-04 03:02 usls/src/video_tools.py
--rwxrwxrwx  2.0 unx    35149 b- defN 23-May-04 03:59 usls-0.2.1.dist-info/LICENSE
--rwxrwxrwx  2.0 unx      540 b- defN 23-May-04 03:59 usls-0.2.1.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-May-04 03:59 usls-0.2.1.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       34 b- defN 23-May-04 03:59 usls-0.2.1.dist-info/entry_points.txt
--rwxrwxrwx  2.0 unx        5 b- defN 23-May-04 03:59 usls-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1774 b- defN 23-May-04 03:59 usls-0.2.1.dist-info/RECORD
-23 files, 194602 bytes uncompressed, 57811 bytes compressed:  70.3%
+-rwxrwxrwx  2.0 unx     9413 b- defN 23-May-04 09:28 usls/src/video_tools.py
+-rwxrwxrwx  2.0 unx    35149 b- defN 23-May-04 09:29 usls-0.2.2.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx      540 b- defN 23-May-04 09:29 usls-0.2.2.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-May-04 09:29 usls-0.2.2.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       34 b- defN 23-May-04 09:29 usls-0.2.2.dist-info/entry_points.txt
+-rwxrwxrwx  2.0 unx        5 b- defN 23-May-04 09:29 usls-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1774 b- defN 23-May-04 09:29 usls-0.2.2.dist-info/RECORD
+23 files, 194629 bytes uncompressed, 57853 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -45,26 +45,26 @@
 
 Filename: usls/src/utils.py
 Comment: 
 
 Filename: usls/src/video_tools.py
 Comment: 
 
-Filename: usls-0.2.1.dist-info/LICENSE
+Filename: usls-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: usls-0.2.1.dist-info/METADATA
+Filename: usls-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: usls-0.2.1.dist-info/WHEEL
+Filename: usls-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: usls-0.2.1.dist-info/entry_points.txt
+Filename: usls-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: usls-0.2.1.dist-info/top_level.txt
+Filename: usls-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: usls-0.2.1.dist-info/RECORD
+Filename: usls-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## usls/__init__.py

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*- 
 
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 
 from usls.cli import cli
 from usls.run import run
 
 
 __all__ = [
 	'__version__',
```

## usls/src/video_tools.py

```diff
@@ -22,22 +22,25 @@
         fourcc='mp4v',
         record=False,
         output_dir=None,
     ):
     # video play & record
 
     # check file
-    if not Path(source).is_file():
-        raise TypeError(f"{source} is not a valid file.")
-        sys.exit()
-
-    # check format
-    if not Path(source).suffix in VIDEO_FORMAT:
-        raise TypeError(f"{source} is supported video format: {VIDEO_FORMAT}.")
-        sys.exit()
+    if Path(source).is_file():
+        # raise TypeError(f"{source} is not a valid file.")
+        # sys.exit()
+        
+        # check format
+        if not Path(source).suffix in VIDEO_FORMAT:
+            raise TypeError(f"{source} is supported video format: {VIDEO_FORMAT}.")
+            sys.exit()
+
+
+
 
     CONSOLE.log(f"Source: {Path(source).resolve()}")
 
 
     # flip and rotate
     if flip:
         if flip == 'ud':
```

## Comparing `usls-0.2.1.dist-info/LICENSE` & `usls-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `usls-0.2.1.dist-info/METADATA` & `usls-0.2.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usls
-Version: 0.2.1
+Version: 0.2.2
 Summary: Useless CV toolkits
 Home-page: https://github.com/jamjamjon/usls
 Author: jamjamjon
 License: GPL-3.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `usls-0.2.1.dist-info/RECORD` & `usls-0.2.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-usls/__init__.py,sha256=MvMdXXuE1o8ecodvP1_ClMaOpSy0asz5HlW4dp-tYdc,171
+usls/__init__.py,sha256=FYNOzxUOUHny8bwF4C-bx7ihDE6pZM90MPcpcKjfBMA,171
 usls/cli.py,sha256=VZce68IJqqpJDz7jTXxda1a3KVKOopeDTYUjCSnT8S8,11563
 usls/run.py,sha256=bSl-x3wSxrGIh9I2QwoTESi_e2WyI8QN9ruE_7bl1Zk,2629
 usls/src/__init__.py,sha256=taQDSBFDUilwiGM8wY4BJ1rZL90B8Ahvc-UpHy5d5pE,309
 usls/src/class_modify.py,sha256=MVwj18Z47GV67EfLv77wEKMfRLT2DgOmckQPFQQkU2I,2171
 usls/src/cleanup.py,sha256=ABQiSHOxgLS9zr4-0vCbPe1hrJAeEfatxLEgBpjlU60,6028
 usls/src/deduplicate.py,sha256=7Uaq4QScnOVPVMWRZiG1eBXorg9oF6SWjJklsL6rc_w,5530
 usls/src/dir_combine.py,sha256=xatoOY54X8oMTvH3HJflgTfJdIBOG3gdTJyLOEQEmVc,1739
@@ -10,14 +10,14 @@
 usls/src/label_combine.py,sha256=T99nvA4fcHt94cCV9zZVPJvmgj_Lus-5H3lowCbp9So,3204
 usls/src/labelling_cls.py,sha256=yFW_zeBBFr_HS6fu5mqUpPq9-z0F_txAhUGpg-RchRQ,18138
 usls/src/labelling_det.py,sha256=VnoxsLxSl3DokJcKx6VNp4Fa9uUXYVbeFRkJ-9OsnJE,39435
 usls/src/labelling_det_2.py,sha256=jfiW3F7NifoV64QylkRi5yYmeWJW6HMUkJchEzCjAJ4,40829
 usls/src/rename.py,sha256=IxH2LsZEfitXtHEd7PiSlNx4JyLsblJQuIGOOGLyvu4,2555
 usls/src/spider.py,sha256=g70JjlPX5H2qOjMrmdHspaW9lki9kVIprEBtV49lD8M,3470
 usls/src/utils.py,sha256=JoP0kWsWOX7m1k8MZ0PgSCG4lIkAGNzDsLQAiHi1Brg,5906
-usls/src/video_tools.py,sha256=hR2UdXOWdZfh732YHyUCHnHBuR5dSQ7Hu2M3LYmMaZY,9386
-usls-0.2.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-usls-0.2.1.dist-info/METADATA,sha256=nh2pJ2tegX8rbzlfrPYrRTp3u8bAJPhQDfwwm91Yb8A,540
-usls-0.2.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-usls-0.2.1.dist-info/entry_points.txt,sha256=NtT7OjVpekraB5xlzXzTbTQ9q8VOKMUrByrtciZMJms,34
-usls-0.2.1.dist-info/top_level.txt,sha256=oS7b-J2DgqOuJIQaKnSyirCC_Rt6yeQCLkbNqh2H_DM,5
-usls-0.2.1.dist-info/RECORD,,
+usls/src/video_tools.py,sha256=SOohb0jHwU-0hg7l53jiOJ8m368hoLELez5IH65n2Yg,9413
+usls-0.2.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+usls-0.2.2.dist-info/METADATA,sha256=a2ym4LyYT0SH97aNs0aRqp1DyoakTEbje_Fp3rVthnM,540
+usls-0.2.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+usls-0.2.2.dist-info/entry_points.txt,sha256=NtT7OjVpekraB5xlzXzTbTQ9q8VOKMUrByrtciZMJms,34
+usls-0.2.2.dist-info/top_level.txt,sha256=oS7b-J2DgqOuJIQaKnSyirCC_Rt6yeQCLkbNqh2H_DM,5
+usls-0.2.2.dist-info/RECORD,,
```

