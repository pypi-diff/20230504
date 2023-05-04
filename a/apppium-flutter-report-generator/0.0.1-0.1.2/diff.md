# Comparing `tmp/apppium_flutter_report_generator-0.0.1-py3-none-any.whl.zip` & `tmp/apppium_flutter_report_generator-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4985 bytes, number of entries: 9
+Zip file size: 4986 bytes, number of entries: 9
 -rw-r--r--  2.0 fat      335 b- defN 20-Feb-02 00:00 setup.py
 -rw-r--r--  2.0 fat       96 b- defN 20-Feb-02 00:00 src/__init__.py
 -rw-r--r--  2.0 fat     3453 b- defN 20-Feb-02 00:00 src/group_and_test.py
 -rw-r--r--  2.0 fat      507 b- defN 20-Feb-02 00:00 src/logger.py
 -rw-r--r--  2.0 fat     2296 b- defN 20-Feb-02 00:00 src/report_generator.py
-?rw-r--r--  2.0 fat      665 b- defN 20-Feb-02 00:00 apppium_flutter_report_generator-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 apppium_flutter_report_generator-0.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1096 b- defN 20-Feb-02 00:00 apppium_flutter_report_generator-0.0.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat      763 b- defN 20-Feb-02 00:00 apppium_flutter_report_generator-0.0.1.dist-info/RECORD
-9 files, 9298 bytes uncompressed, 3657 bytes compressed:  60.7%
+?rw-r--r--  2.0 fat      665 b- defN 20-Feb-02 00:00 apppium_flutter_report_generator-0.1.2.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 apppium_flutter_report_generator-0.1.2.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1096 b- defN 20-Feb-02 00:00 apppium_flutter_report_generator-0.1.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat      763 b- defN 20-Feb-02 00:00 apppium_flutter_report_generator-0.1.2.dist-info/RECORD
+9 files, 9298 bytes uncompressed, 3658 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: src/logger.py
 Comment: 
 
 Filename: src/report_generator.py
 Comment: 
 
-Filename: apppium_flutter_report_generator-0.0.1.dist-info/METADATA
+Filename: apppium_flutter_report_generator-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: apppium_flutter_report_generator-0.0.1.dist-info/WHEEL
+Filename: apppium_flutter_report_generator-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: apppium_flutter_report_generator-0.0.1.dist-info/licenses/LICENSE
+Filename: apppium_flutter_report_generator-0.1.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: apppium_flutter_report_generator-0.0.1.dist-info/RECORD
+Filename: apppium_flutter_report_generator-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## setup.py

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(
    name='apppium_flutter_report_generator',
-   version='0.0.1',
+   version='0.1.2',
    description='A package for generating Appium Flutter Report.',
    author='Aaradhya Gopal Nepal',
    author_email='aradhya.1441@gmail.com',
    packages=['apppium_flutter_report_generator'],
    install_requires=['wheel'],
 )
```

## Comparing `apppium_flutter_report_generator-0.0.1.dist-info/METADATA` & `apppium_flutter_report_generator-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apppium_flutter_report_generator
-Version: 0.0.1
+Version: 0.1.2
 Summary: A package for generating Appium Flutter Report.
 Project-URL: Homepage, https://github.com/AradhyaNepal/AppiumFlutterReport/tree/main/PythonReportGenerator
 Project-URL: Bug Tracker, https://github.com/AradhyaNepal/AppiumFlutterReport/issues
 Author-email: Aaradhya Gopal Nepal <aradhya.1441@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `apppium_flutter_report_generator-0.0.1.dist-info/licenses/LICENSE` & `apppium_flutter_report_generator-0.1.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `apppium_flutter_report_generator-0.0.1.dist-info/RECORD` & `apppium_flutter_report_generator-0.1.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-setup.py,sha256=TwiIgvkjfwIQxKy-FYtt7LiV2KcN8OcfGvpBiF6eZow,335
+setup.py,sha256=0Sp3OWBnmmwgOvN7Lc1VcvcFB1shKex3MoRe7uoTpVg,335
 src/__init__.py,sha256=sERwxqWEsUcpThoOcy12EuKVsBmFmZgCqbnU3gx6__k,96
 src/group_and_test.py,sha256=B3_ivBLzrN9bDFwqdsVPAut3XWN20Kz0c5baMmW4Vc4,3453
 src/logger.py,sha256=UeX1Rnt8dkxfz2tEtZkl6sNdYVVEoHHxp_nuJYA1dCk,507
 src/report_generator.py,sha256=s1ifSVP_gZARxS4MKEltr8f7B_4s3ZsonA9UaXk1ftc,2296
-apppium_flutter_report_generator-0.0.1.dist-info/METADATA,sha256=EGgL3KbRzzaf3BRHiq8aF8zusazJK1UKISoGkmQIpNU,665
-apppium_flutter_report_generator-0.0.1.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
-apppium_flutter_report_generator-0.0.1.dist-info/licenses/LICENSE,sha256=0OdJe5iNQkEvzmrwalMse3qe1rGiX68PuIRlNU-IhsY,1096
-apppium_flutter_report_generator-0.0.1.dist-info/RECORD,,
+apppium_flutter_report_generator-0.1.2.dist-info/METADATA,sha256=7gs8t0k0JTbNWqrc9dLQPQpRrv0g_uC4vE1ZxA91-HY,665
+apppium_flutter_report_generator-0.1.2.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+apppium_flutter_report_generator-0.1.2.dist-info/licenses/LICENSE,sha256=0OdJe5iNQkEvzmrwalMse3qe1rGiX68PuIRlNU-IhsY,1096
+apppium_flutter_report_generator-0.1.2.dist-info/RECORD,,
```

