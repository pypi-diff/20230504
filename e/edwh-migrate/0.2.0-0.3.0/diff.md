# Comparing `tmp/edwh_migrate-0.2.0.tar.gz` & `tmp/edwh_migrate-0.3.0.tar.gz`

## Comparing `edwh_migrate-0.2.0.tar` & `edwh_migrate-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/migrations.py
--rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/requirements.txt
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/test.db
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/test.sqlite
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/.idea/.gitignore
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/.idea/migrate.iml
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/.idea/modules.xml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/.idea/vcs.xml
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/src/edwh_migrate/__about__.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/src/edwh_migrate/__init__.py
--rw-r--r--   0        0        0    17266 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/src/edwh_migrate/migrate.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/README.md
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 edwh_migrate-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/migrations.py
+-rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/.gitignore
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/dataSources.local.xml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/dataSources.xml
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/migrate.iml
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/modules.xml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/vcs.xml
+-rw-r--r--   0        0        0    13833 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/workspace.xml
+-rw-r--r--   0        0        0    47176 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/dataSources/21da014d-6e3f-42ea-8c44-aedba5c52d26.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/src/edwh_migrate/__about__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/src/edwh_migrate/__init__.py
+-rw-r--r--   0        0        0    17991 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/src/edwh_migrate/migrate.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/tests/test_basics.py
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/tests/sqlite_empty/empty_sqlite.db
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/tests/sqlite_empty/just_implemented_features.db
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/tests/sqlite_empty/just_implemented_features.sql
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/README.md
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/PKG-INFO
```

### Comparing `edwh_migrate-0.2.0/migrations.py` & `edwh_migrate-0.3.0/migrations.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.2.0/requirements.txt` & `edwh_migrate-0.3.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.2.0/.idea/jupyter-settings.xml` & `edwh_migrate-0.3.0/.idea/jupyter-settings.xml`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.2.0/src/edwh_migrate/__init__.py` & `edwh_migrate-0.3.0/src/edwh_migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.2.0/src/edwh_migrate/migrate.py` & `edwh_migrate-0.3.0/src/edwh_migrate/migrate.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,16 +12,19 @@
    - public.item
    forget and fail...
 
 """
 import contextlib
 import datetime
 import os
+import pathlib
+import sqlite3
 import sys
 import time
+import typing
 import urllib
 import urllib.parse
 from collections import OrderedDict
 from functools import wraps
 from pathlib import Path
 
 import plumbum
@@ -52,106 +55,154 @@
     pass
 
 class MigrationFailed(Exception):
     pass
 
 
 def setup_db(
-        migrate=False,
-        migrate_enabled=False,
-        appname=" ".join(sys.argv),
-        long_running=False,
-        dal_class=None,
+        migrate: bool = False,
+        migrate_enabled: bool = False,
+        appname: str = " ".join(sys.argv),
+        long_running: bool | int = False,
+        dal_class: type = None,
 ):
+    '''
+
+    Connect to the database and return a DAL object.
+
+    When using postgres, the application name is set to the appname argument, long lasting connections are enabled
+    when using long_running, to avoid PGPOOL closing the connection during unpacking of a larger backup file.
+
+    This function will also search for the ewh_implemented_features table, which is used to keep track of which migrations
+    have been attempted and applied.
+
+    If this table is not found, an DatabaseNotYetInitialized exception is raised. This is handled in the
+    activate_migrations function to allow for the database to be restored from a backup before continuing.
+
+    While migrating, functions registered with the @migration(requires=...) decorator applied, will reconnect using
+    `setup_db()` without any arguments.
+
+    :param migrate: migrate is normally turned off, but if you want to run migrations, set this to True
+    :param migrate_enabled: normally migrate is turned off, but if you want to run migrations, set this to True
+    :param appname: name of this application to register on postgres connections, default: " ".join(sys.argv)
+    :param long_running: bool or int to indicate the number of seconds to keep the connection alive using pgpool set_client_idle_limit
+    :param dal_class: optional DAL class, will use DAL if not given
+    :return: database connection
+    '''
     if dal_class is None:
         # default: pydal.DAL
         # (alternative: py4web.core.DAL)
         dal_class = DAL
 
     try:
         uri = os.environ["MIGRATE_URI"]
     except KeyError as e:
         raise InvalidConfigException("$MIGRATE_URI not found in environment.") from e
     is_postgres = uri.startswith('postgres')
-    driver_args = dict(
-        application_name=appname,
-    ) if is_postgres else {}
-    if not long_running and is_postgres:
-        driver_args["keepalives"] = 1
+    driver_args = {}
+    if is_postgres:
+        driver_args['application_name'] = appname
+        if not long_running:
+            driver_args["keepalives"] = 1
+
     db = dal_class(
         uri,
         migrate=migrate,
         migrate_enabled=migrate_enabled,
         driver_args=driver_args,
         pool_size=1,
     )
     if is_postgres and not long_running:
-        db.executesql("PGPOOL SET client_idle_limit = 10;")
-    # https://www.pgpool.net/docs/latest/en/html/sql-pgpool-set.html
-    # make this connection able to live longer, because the functions can take over 30s
-    # to perform the job.
-    # db.executesql("PGPOOL SET client_idle_limit = 3600;")
+        # https://www.pgpool.net/docs/latest/en/html/sql-pgpool-set.html
+        # make this connection able to live longer, because the functions can take over 30s
+        # to perform the job.
+        # db.executesql("PGPOOL SET client_idle_limit = 3600;")
+        with contextlib.suppress(Exception):
+            db.executesql(f"PGPOOL SET client_idle_limit = {long_running if str(long_running).isdigit() else 3600};")
 
     db.define_table(
         "ewh_implemented_features",
         Field("name", unique=True),
         Field("installed", "boolean", default=False),
         Field("last_update_dttm", "datetime", default=datetime.datetime.now()),
     )
     try:
         db(db.ewh_implemented_features).count()
-    except psycopg2.errors.UndefinedTable as e:
+    except (psycopg2.errors.UndefinedTable, sqlite3.OperationalError) as e:
         raise DatabaseNotYetInitialized(
             "ewh_implemented_features is missing.", db
         ) from e
     return db
 
 
-def migration(func: callable = None, requires: list[str] | None = None):
+def migration(func: callable = None, requires: list[callable] | typing.Callable | None = None):
+    """
+    Decorator to register a function as a migration function.
+
+    example:
+
+    @migration
+    def my_migration_function(db):
+        db.executesql("select 1")
+        return True # or False, if the migration failed. On true db.commit() will be performed.
+
+    :param func: function to register as a migration function
+    :param requires: list of function names that need to be applied before this function can be applied.
+
+    """
     if func is None and requires:
-        # requires is opgegeven, dus decorator teruggeven.
+        # requires is given, so return the decorator that will test if the requirements are met before
+        # executing the decorated function, when it's time to really execute the function.
         if callable(requires):
-            # bij een enkelvoudige requirement, alleen een functie, neem de naam van de functie
+            # when a single requirement is given, and it is a function, take the name of the function
             required_names = [requires.__name__]
         else:
-            # als niet callable, dan moet het een list zijn van functies, dus pak alle namen van die functies.
+            # if requires is not callable, then it must be a list of functions, so take the names of those functions.
             required_names = [_.__name__ for _ in requires]
 
         def decorator(decorated: callable):
             @wraps(decorated)
-            def met_requires(*p, **kwp):
+            def with_requires(*p, **kwp):
                 # check requirements
                 db = setup_db()
                 installed = [
                     row.installed
                     for row in db(
-                        db.ewh_implemented_features.name.belongs(required_names)
+                        db.ewh_implemented_features.name.belongs(required_names) &
+                        (db.ewh_implemented_features.installed == True)
                     ).select("installed")
                 ]
-                # check of alle requirements wel gevonden zijn:
+                # check if all requirements are in the list of installed features
                 if len(installed) != len(required_names):
                     db.close()
                     print(decorated.__name__, "REQUIREMENTS NOT MET")
                     raise RequimentsNotMet("requirements not met")
                 if not all(installed):
                     db.close()
                     print(decorated.__name__, "REQUIREMENTS NOT MET")
                     raise RequimentsNotMet("requirements not met")
                 return decorated(*p, **kwp)
 
-            registered_functions[decorated.__name__] = met_requires
-            return met_requires
+            registered_functions[decorated.__name__] = with_requires
+            return with_requires
 
         return decorator
     if func:
         registered_functions[func.__name__] = func
     return func
 
 
-def should_run(db, name):
+def should_run(db: DAL, name: str) -> bool:
+    """
+    Checks if a migration function should be run.
+
+    :param db: database connection
+    :param name: name of the migration function
+    :return: whether the migration function should be run (if not installed) or not (when installed).
+    """
     resultset = db(db.ewh_implemented_features.name == name).select()
     row = resultset.first() if resultset else None
     return row.installed is False if row else True
 
 
 def recover_database_from_backup():
     """
@@ -167,71 +218,36 @@
         possibly downloaded from backblaze, but this code
         is stale.
     Effectively running something like:
         A,B)  7z x -so -p"secret" db.7z | psql -h  127.0.0.1 -U postgres -d backend
           C) cat /data/database_to_restore.sql | psql -h  127.0.0.1 -U postgres -d backend
 
     """
-    print("RECOVER_DATABASE_FROM_BACKEND  started ")
-    prepared_sql_path = "/data/database_to_restore.sql"
-    prepared_sql_path_gz = f"{prepared_sql_path}.gz"
-    prepared_sql_path_xz = f"{prepared_sql_path}.xz"
-    if os.path.exists(prepared_sql_path):
-        print("RECOVER:", prepared_sql_path, "exists. ")
-        # option C
-        unpack = plumbum.local["cat"][prepared_sql_path]
-    elif os.path.exists(prepared_sql_path_xz):
-        print("RECOVER:", prepared_sql_path_xz, "exists. ")
-        # option C
-        unpack = plumbum.local["xzcat"][prepared_sql_path_xz]
-    elif os.path.exists(prepared_sql_path_gz):
-        print("RECOVER:", prepared_sql_path_gz, "exists. ")
-        # option C
-        unpack = plumbum.local["zcat"][prepared_sql_path_gz]
-    else:
-        print("RECOVER:", prepared_sql_path, " not found.")
-        # option A and B
-        raise NotImplementedError(
-            "Recovering from the .7z file is not implemented at the moment. "
-        )
-        # local_backup = "/data/database_to_restore.7z"
-        # if not os.path.exists(local_backup):
-        #     print("RECOVER:", local_backup, "not found. Downloading from B2")
-        #     # option A
-        #     b2_application_key_id = os.environ["B2_APPLICATION_KEY_ID"]
-        #     b2_application_key = os.environ["B2_APPLICATION_KEY"]
-        #     b2_file_id = os.environ["B2_FILE_ID"]
-        #     b2_file_password = os.environ["B2_FILE_PASSWORD"]
-        #     # craft a reference to the executable
-        #     b2 = plumbum.local["b2"]
-        #     # authorize the account
-        #     print("RECOVER: authenticating b2")
-        #     b2(
-        #         "authorize-account",
-        #         b2_application_key_id,
-        #         b2_application_key,
-        #     )
-        #     # download the file, it's not that big (30+mb) at the time of writing.
-        #     # b2 doesn't support outputting to stdout, so an intermediate file is required
-        #     print("RECOVER: downloading backup file to ", local_backup)
-        #     b2("download-file-by-id", b2_file_id, local_backup)
-        #     print("RECOVER: download done")
-        # # option A en B mere gere
-        # # prepare the 7z command
-        # archive_password = base64.b64decode(b2_file_password).decode()
-        # unpack = plumbum.local["7z"][
-        #     "x", "-so", "-p{}".format(archive_password), local_backup
-        # ]
-    # option A, B and C merge here
+    print("RECOVER_DATABASE_FROM_BACKEND started ")
+    prepared_sql_path = pathlib.Path(os.getenv('DATABASE_TO_RESTORE', "/data/database_to_restore.sql"))
+    if not prepared_sql_path.exists():
+        raise FileNotFoundError(prepared_sql_path)
+    extension = prepared_sql_path.suffix.lower()
+
+    cat_command = {
+        '.sql': 'cat',
+        '.xz': 'xzcat',
+        '.gz': 'zcat',
+    }.get(extension, os.getenv('MIGRATE_CAT_COMMAND'))
+    if not cat_command:
+        raise NotImplementedError(f"Extension {extension} not supported for {prepared_sql_path}")
+    unpack = plumbum.local[cat_command][prepared_sql_path]
+
     # unpack is now the command to cat the sql to stdout
-    # whih is piped to psql ot perform the recovery
+    # which is piped to psql to perform the recovery
 
     # parse the db uri to find hostname and port and such to
     # feed to pqsl as commandline arguments
     uri = urllib.parse.urlparse(os.environ["MIGRATE_URI"])
+    is_postgres = uri.scheme.startswith("postgres")
     database = str(uri.path).lstrip("/")
     netloc = str(uri.netloc)
     if "@" in netloc:
         username_password, hostname_port = netloc.split("@")
     else:
         username_password = "postgres"
         hostname_port = netloc
@@ -242,31 +258,35 @@
         password = None
     if ":" in hostname_port:
         hostname, port = hostname_port.split(":")
     else:
         hostname = hostname_port
         port = "5432"
 
-    # prepare the psql command
-    psql = plumbum.local["psql"]["-h", hostname, "-U", username, "-d", database]
-    if password:
-        raise InvalidConfigException(
-            "Postgresql Password NOT SUPPORTED for automatic migrations... "
-        )
-    if port:
-        psql = psql["-p", port]
-
+    if is_postgres:
+        # prepare the psql command
+        psql = plumbum.local["psql"]["-h", hostname, "-U", username, "-d", database]
+        if password:
+            raise InvalidConfigException(
+                "Postgresql Password NOT SUPPORTED for automatic migrations... "
+            )
+        if port:
+            psql = psql["-p", port]
+        sql_consumer = psql
+    else:
+        sqlite_database_path = pathlib.Path(uri.netloc) / pathlib.Path(uri.path.strip('/'))
+        sql_consumer = plumbum.local["sqlite3"][sqlite_database_path]
     # combine both
-    cmd = unpack | psql
+    cmd = unpack | sql_consumer
 
     print("UNPACKING AND INSTALLING DATABASE:", cmd)
     # noinspection PyStatementEffect
     # is plumbum syntax
     cmd() > "/dev/null"
-    print("phew. that took a while")
+    print("Done unpacking and feeding to", cmd)
 
     # os.unlink(local_backup)
 
 
 def activate_migrations():
     """Start the migration process, don't wait for a lock"""
     started = time.time()
@@ -310,58 +330,51 @@
 
     successes = []
     # perform migrations
     for name, function in registered_functions.items():
         print("test:", name)
         if should_run(db, name):
             print("run: ", name)
-            try:
-                # create a new database connection
-                # because there could be tables being defined,
-                # and we want all the functions to be siloed and not
-                # have database schema dependencies and collisions.
-                db_for_this_function = setup_db()
-                result = function(db_for_this_function)
-                successes.append(result)
-                if result:
-                    # commit the change to db
-                    db_for_this_function.commit()
-                    # close this specific cursor, it's not used any longer.
-                    db_for_this_function.close()
-                    print("ran: ", name, "successfully. ")
-                    # alleen bij success opslaan dat er de feature beschikbaar is
-                    db.ewh_implemented_features.update_or_insert(
-                        db.ewh_implemented_features.name == name,
-                        name=name,
-                        installed=True,
-                        last_update_dttm=datetime.datetime.now(),
-                    )
-                    db.commit()
-                else:
-                    print("ran: ", name, " and failed. ")
-                    successes.append(False)
-                    # try a rollback, because we should ignore whatever happend
-                    db_for_this_function.rollback()
-                    # and close because this connection is not used any longer.
-                    db_for_this_function.close()
-
-            except:
-                raise
-            # except:
-            #     print(sys.exc_info())
-            #     # ignore elke error!
-            #     exception_type, exception_value, exception_traceback = sys.exc_info()
-            #     print(f"ERROR: {exception_type}({exception_value} ")
-            #     print(exception_traceback)
-            #     success = False
-            #     successes.append(False)
-            #     raise
+            # create a new database connection
+            # because there could be tables being defined,
+            # and we want all the functions to be siloed and not
+            # have database schema dependencies and collisions.
+            db_for_this_function = setup_db()
+            result = function(db_for_this_function)
+            successes.append(result)
+            if result:
+                # commit the change to db
+                db_for_this_function.commit()
+                # close this specific cursor, it's not used any longer.
+                db_for_this_function.close()
+                print("ran: ", name, "successfully. ")
+                # alleen bij success opslaan dat er de feature beschikbaar is
+                db.ewh_implemented_features.update_or_insert(
+                    db.ewh_implemented_features.name == name,
+                    name=name,
+                    installed=True,
+                    last_update_dttm=datetime.datetime.now(),
+                )
+            else:
+                print("ran: ", name, " and failed. ")
+                successes.append(False)
+                # try a rollback, because we should ignore whatever happend
+                db_for_this_function.rollback()
+                # and close because this connection is not used any longer.
+                db_for_this_function.close()
+                db.ewh_implemented_features.update_or_insert(
+                    db.ewh_implemented_features.name == name,
+                    name=name,
+                    installed=False,
+                    last_update_dttm=datetime.datetime.now(),
+                )
+            db.commit()
         else:
             print("already installed. ")
-    # db(db.ewh_implemented_features.name == 'feature_2').delete()
+
     db.close()
 
     # clean redis whenever possible
     # reads REDIS_MASTER_HOST from the environment
     if redis_host := os.getenv("REDIS_HOST", None):
         r = redis.Redis(redis_host)
         keys = r.keys()
```

### Comparing `edwh_migrate-0.2.0/.gitignore` & `edwh_migrate-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.2.0/LICENSE.txt` & `edwh_migrate-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.2.0/pyproject.toml` & `edwh_migrate-0.3.0/pyproject.toml`

 * *Files identical despite different names*

