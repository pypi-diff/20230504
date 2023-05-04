# Comparing `tmp/django_sqlite_backup-0.0.1-py3-none-any.whl.zip` & `tmp/django_sqlite_backup-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,15 @@
-Zip file size: 4301 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 17:16 django_sqlite_backup/__init__.py
--rw-r--r--  2.0 unx      170 b- defN 23-Apr-14 17:16 django_sqlite_backup/apps.py
--rw-r--r--  2.0 unx       32 b- defN 23-Apr-14 17:16 django_sqlite_backup/aws.py
--rw-r--r--  2.0 unx      121 b- defN 23-Apr-14 17:16 django_sqlite_backup/urls.py
--rw-r--r--  2.0 unx       30 b- defN 23-Apr-14 17:16 django_sqlite_backup/views.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Apr-14 17:18 django_sqlite_backup-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2657 b- defN 23-Apr-14 17:18 django_sqlite_backup-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 17:18 django_sqlite_backup-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Apr-14 17:18 django_sqlite_backup-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      871 b- defN 23-Apr-14 17:18 django_sqlite_backup-0.0.1.dist-info/RECORD
-10 files, 5064 bytes uncompressed, 2783 bytes compressed:  45.0%
+Zip file size: 7315 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-May-04 10:38 django_sqlite_backup/__init__.py
+-rw-r--r--  2.0 unx      450 b- defN 23-May-04 10:38 django_sqlite_backup/apps.py
+-rw-r--r--  2.0 unx     1644 b- defN 23-May-04 10:38 django_sqlite_backup/aws.py
+-rw-r--r--  2.0 unx      779 b- defN 23-May-04 10:38 django_sqlite_backup/backup.py
+-rw-r--r--  2.0 unx      496 b- defN 23-May-04 10:38 django_sqlite_backup/decorators.py
+-rw-r--r--  2.0 unx      740 b- defN 23-May-04 10:38 django_sqlite_backup/restore.py
+-rw-r--r--  2.0 unx      150 b- defN 23-May-04 10:38 django_sqlite_backup/urls.py
+-rw-r--r--  2.0 unx      403 b- defN 23-May-04 10:38 django_sqlite_backup/views.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-04 10:38 django_sqlite_backup-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4514 b- defN 23-May-04 10:38 django_sqlite_backup-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 10:38 django_sqlite_backup-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-May-04 10:38 django_sqlite_backup-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1137 b- defN 23-May-04 10:38 django_sqlite_backup-0.0.2.dist-info/RECORD
+13 files, 11496 bytes uncompressed, 5379 bytes compressed:  53.2%
```

## zipnote {}

```diff
@@ -3,29 +3,38 @@
 
 Filename: django_sqlite_backup/apps.py
 Comment: 
 
 Filename: django_sqlite_backup/aws.py
 Comment: 
 
+Filename: django_sqlite_backup/backup.py
+Comment: 
+
+Filename: django_sqlite_backup/decorators.py
+Comment: 
+
+Filename: django_sqlite_backup/restore.py
+Comment: 
+
 Filename: django_sqlite_backup/urls.py
 Comment: 
 
 Filename: django_sqlite_backup/views.py
 Comment: 
 
-Filename: django_sqlite_backup-0.0.1.dist-info/LICENSE
+Filename: django_sqlite_backup-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: django_sqlite_backup-0.0.1.dist-info/METADATA
+Filename: django_sqlite_backup-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: django_sqlite_backup-0.0.1.dist-info/WHEEL
+Filename: django_sqlite_backup-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: django_sqlite_backup-0.0.1.dist-info/top_level.txt
+Filename: django_sqlite_backup-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: django_sqlite_backup-0.0.1.dist-info/RECORD
+Filename: django_sqlite_backup-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_sqlite_backup/apps.py

```diff
@@ -1,6 +1,12 @@
 from django.apps import AppConfig
+from django.conf import ImproperlyConfigured
+from django.conf import settings
 
 
 class DjangoSqliteBackupConfig(AppConfig):
     default_auto_field = "django.db.models.BigAutoField"
     name = "django_sqlite_backup"
+
+    def ready(self) -> None:
+        if settings.DATABASES["default"]["ENGINE"] != "django.db.backends.sqlite3":
+            raise ImproperlyConfigured("'default' database must be a SQLite database.")
```

## django_sqlite_backup/aws.py

```diff
@@ -1,2 +1,58 @@
+from datetime import datetime
+from typing import Any
+
+import boto3
+from django.conf import ImproperlyConfigured
+from django.conf import settings
+
+
 class AwsSqliteBackup:
-    pass
+    def __init__(self) -> None:
+        self.s3 = boto3.client("s3")
+
+    def get_database_name(self) -> str:
+        return str(settings.DATABASES["default"]["NAME"])
+
+    def _read_db(self) -> Any:
+        with open(self.get_database_name()) as f:
+            return f.read()
+
+    def backup_db(self) -> None:
+        bucket_name = settings.SQLITE_BACKUP.get("BUCKET_NAME")
+        db_name = self.get_database_name().split("/")[-1]
+
+        if bucket_name is None:
+            raise ImproperlyConfigured("`BUCKET_NAME` is not defined")
+
+        full_bucket_name = f"sqlite_backup/{datetime.now().strftime('%Y-%m-%d')}/{db_name}"
+
+        self.s3.put_object(
+            Bucket=bucket_name,
+            Key=full_bucket_name,
+            Body=self._read_db(),
+        )
+
+
+class AwsRestoreDb:
+    def __init__(self) -> None:
+        self.s3 = boto3.client("s3")
+
+    def get_database_name(self) -> str:
+        return str(settings.DATABASES["default"]["NAME"])
+
+    def restore_db(self, date_str: str) -> None:
+        bucket_name = settings.SQLITE_BACKUP.get("BUCKET_NAME")
+
+        if bucket_name is None:
+            raise ImproperlyConfigured("`BUCKET_NAME` is not defined")
+
+        db_name = self.get_database_name()
+        key = f"sqlite_backup/{date_str}/{db_name}"
+
+        response = self.s3.get_object(
+            Bucket=bucket_name,
+            Key=key,
+        )
+
+        with open(db_name, "w") as f:
+            f.write(response.get("Body").read().decode())
```

## django_sqlite_backup/urls.py

```diff
@@ -1,7 +1,7 @@
-from django.url import path
+from django.urls import path
 
 from django_sqlite_backup import views
 
 urlpatterns = [
-    path("backup", views.backup),
+    path("backup/", views.backup_view, name="sqlite-backup"),
 ]
```

## django_sqlite_backup/views.py

```diff
@@ -1,2 +1,13 @@
-def backup(request):
-    pass
+from django.http import HttpRequest
+from django.http import JsonResponse
+from django.views.decorators.http import require_http_methods
+
+from django_sqlite_backup import backup
+from django_sqlite_backup.decorators import login_required
+
+
+@login_required
+@require_http_methods(["POST"])
+def backup_view(request: HttpRequest) -> JsonResponse:
+    backup.do_backup()
+    return JsonResponse({}, status=204)
```

## Comparing `django_sqlite_backup-0.0.1.dist-info/LICENSE` & `django_sqlite_backup-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_sqlite_backup-0.0.1.dist-info/RECORD` & `django_sqlite_backup-0.0.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 django_sqlite_backup/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-django_sqlite_backup/apps.py,sha256=nQDMbXfnJqVeONtw_5GsedP0ANKigeXCiaQpHYn1hbM,170
-django_sqlite_backup/aws.py,sha256=0xDG9MaTpzer9IEmW0g1itQkU0fRQPOSDgg8scO1V6w,32
-django_sqlite_backup/urls.py,sha256=jzjhGr9AEQuPajJDAYkyfr_Q7uE9EjKZzim1pD4qnPE,121
-django_sqlite_backup/views.py,sha256=dH0cwDOGwtXItWlkEWlArkC9qP8sKQ36jvGGPYNwglI,30
-django_sqlite_backup-0.0.1.dist-info/LICENSE,sha256=bwE4PTk0_zgY2rrrldsrBocfua-bkc_IUxH1pr1rCFA,1070
-django_sqlite_backup-0.0.1.dist-info/METADATA,sha256=fkXUN9-grlPls2U9GcAH5QY7bdT9xf2lhBl4cZ9Q0-E,2657
-django_sqlite_backup-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-django_sqlite_backup-0.0.1.dist-info/top_level.txt,sha256=hpNLepZbcHqSqEC92LAtpsd7uaey2g64SD0C0NWEDqM,21
-django_sqlite_backup-0.0.1.dist-info/RECORD,,
+django_sqlite_backup/apps.py,sha256=hr_VWttIN8RVXzXXG2Vo-SjuNgCFDE5POwycNww-ixo,450
+django_sqlite_backup/aws.py,sha256=64FLQTLZV9Am8TaITgj0xkCnAbifpbEyEyZVls4alX0,1644
+django_sqlite_backup/backup.py,sha256=8-4QRYIWJOMYM0Deuub6P5nWiBKjW4w2Gvh-UjttcNg,779
+django_sqlite_backup/decorators.py,sha256=bXvyTazsw0xkkOJ3zNtt8tOv1GmXsmB1lbUMnzW9Mbg,496
+django_sqlite_backup/restore.py,sha256=BJTGqd0zqeTWRbk1c98OqNRweYNmOoDdUC1dsuCkKWc,740
+django_sqlite_backup/urls.py,sha256=ve4fRC0VSPi235hDc9_n973ii_jrIpeE4tPrJTBSNCA,150
+django_sqlite_backup/views.py,sha256=9evoRFbHv4dFHhMD0ntXQH4VyDfWFKNGTFUdTfoIK1Y,403
+django_sqlite_backup-0.0.2.dist-info/LICENSE,sha256=bwE4PTk0_zgY2rrrldsrBocfua-bkc_IUxH1pr1rCFA,1070
+django_sqlite_backup-0.0.2.dist-info/METADATA,sha256=LUXaqUFe76p8jc_-pbHeqrRl83ACKRElWakYqvv-t5g,4514
+django_sqlite_backup-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+django_sqlite_backup-0.0.2.dist-info/top_level.txt,sha256=hpNLepZbcHqSqEC92LAtpsd7uaey2g64SD0C0NWEDqM,21
+django_sqlite_backup-0.0.2.dist-info/RECORD,,
```

