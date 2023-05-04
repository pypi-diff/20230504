# Comparing `tmp/lsms-0.4.4-py2.py3-none-any.whl.zip` & `tmp/lsms-0.4.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7304 bytes, number of entries: 9
--rw-rw----  2.0 unx      121 b- defN 23-Apr-20 02:21 lsms/__init__.py
+Zip file size: 7306 bytes, number of entries: 9
+-rw-rw----  2.0 unx      121 b- defN 23-May-04 17:01 lsms/__init__.py
 -rw-rw----  2.0 unx      838 b- defN 23-Apr-20 02:21 lsms/dta_concordance.py
--rw-rw----  2.0 unx      633 b- defN 23-Apr-20 02:21 lsms/from_dta.py
+-rw-rw----  2.0 unx      637 b- defN 23-May-04 15:41 lsms/from_dta.py
 -rw-rw----  2.0 unx    21813 b- defN 23-Apr-20 02:21 lsms/tools.py
--rw-rw----  2.0 unx      282 b- defN 23-Apr-20 02:21 lsms-0.4.4.dist-info/LICENSE.txt
--rw-rw----  2.0 unx      396 b- defN 23-Apr-20 02:21 lsms-0.4.4.dist-info/METADATA
--rw-rw----  2.0 unx      110 b- defN 23-Apr-20 02:21 lsms-0.4.4.dist-info/WHEEL
--rw-rw----  2.0 unx        5 b- defN 23-Apr-20 02:21 lsms-0.4.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      667 b- defN 23-Apr-20 02:21 lsms-0.4.4.dist-info/RECORD
-9 files, 24865 bytes uncompressed, 6166 bytes compressed:  75.2%
+-rw-rw----  2.0 unx      282 b- defN 23-May-04 17:02 lsms-0.4.5.dist-info/LICENSE.txt
+-rw-rw----  2.0 unx      396 b- defN 23-May-04 17:02 lsms-0.4.5.dist-info/METADATA
+-rw-rw----  2.0 unx      110 b- defN 23-May-04 17:02 lsms-0.4.5.dist-info/WHEEL
+-rw-rw----  2.0 unx        5 b- defN 23-May-04 17:02 lsms-0.4.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      667 b- defN 23-May-04 17:02 lsms-0.4.5.dist-info/RECORD
+9 files, 24869 bytes uncompressed, 6168 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: lsms/from_dta.py
 Comment: 
 
 Filename: lsms/tools.py
 Comment: 
 
-Filename: lsms-0.4.4.dist-info/LICENSE.txt
+Filename: lsms-0.4.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: lsms-0.4.4.dist-info/METADATA
+Filename: lsms-0.4.5.dist-info/METADATA
 Comment: 
 
-Filename: lsms-0.4.4.dist-info/WHEEL
+Filename: lsms-0.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: lsms-0.4.4.dist-info/top_level.txt
+Filename: lsms-0.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: lsms-0.4.4.dist-info/RECORD
+Filename: lsms-0.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lsms/__init__.py

```diff
@@ -1,5 +1,5 @@
 from . import tools
 from . dta_concordance import dta_concordance
 from . from_dta import from_dta
 
-__version__ = '0.4.4'
+__version__ = '0.4.5'
```

## lsms/from_dta.py

```diff
@@ -10,12 +10,12 @@
     var_to_label = dict(zip(sr.varlist,sr.lbllist))    
 
     if convert_categoricals:
         for var in sr.varlist: # Check mapping for each variable with values
             if len(var_to_label[var]):
                 try:
                     code2label = values[var_to_label[var]]
-                    df[var] = df[var].map(code2label)
+                    df[var] = df[var].replace(code2label)
                 except KeyError:
                     print('Issue with categorical mapping: %s' % var)
 
     return df
```

## Comparing `lsms-0.4.4.dist-info/RECORD` & `lsms-0.4.5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-lsms/__init__.py,sha256=dw5tDmXoDpZDcS8JbIbimsUnKmLihVBA5gDfcGxcc6c,121
+lsms/__init__.py,sha256=Q79FmxXfdedie_STmaLwPhbaOvaP8iUgVEmx5ohhIcY,121
 lsms/dta_concordance.py,sha256=MIruKRn1IqVgXdUGf4X4MJ65Pmw-POwctVTpKohozDg,838
-lsms/from_dta.py,sha256=QQgP8ftl-DOM1llg3gcGTJmyFJgOGWIfiKhIvst2aDg,633
+lsms/from_dta.py,sha256=eUVfoG7QoFymXTFcQluAVWUM5cWwIhRO4Jv5iNZY258,637
 lsms/tools.py,sha256=BW-7yrz4249mJB5Dr0GRi7vUj_ohurfZXmNU05_DPCY,21813
-lsms-0.4.4.dist-info/LICENSE.txt,sha256=qImFXcRJwxIHS80FE7uOx6FhmLY8apd4Y12aR54QU7w,282
-lsms-0.4.4.dist-info/METADATA,sha256=uWkZYZUn3coMS957iZZqw8m3gkn6JhJYJB7ZYInFMO8,396
-lsms-0.4.4.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-lsms-0.4.4.dist-info/top_level.txt,sha256=kOSV2CMw4OoSMw9rYGFItmsQDWDXpO3GzeVBTj020lc,5
-lsms-0.4.4.dist-info/RECORD,,
+lsms-0.4.5.dist-info/LICENSE.txt,sha256=qImFXcRJwxIHS80FE7uOx6FhmLY8apd4Y12aR54QU7w,282
+lsms-0.4.5.dist-info/METADATA,sha256=mwS3r2PiBOnrARV2s0sAVDwTB8mDoGXIt16Q6tCKgoE,396
+lsms-0.4.5.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+lsms-0.4.5.dist-info/top_level.txt,sha256=kOSV2CMw4OoSMw9rYGFItmsQDWDXpO3GzeVBTj020lc,5
+lsms-0.4.5.dist-info/RECORD,,
```

