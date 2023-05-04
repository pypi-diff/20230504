# Comparing `tmp/pastell-admin-0.1.16.tar.gz` & `tmp/pastell-admin-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pastell-admin-0.1.16.tar", last modified: Wed Apr 12 14:49:28 2023, max compression
+gzip compressed data, was "pastell-admin-0.1.17.tar", last modified: Thu May  4 08:11:01 2023, max compression
```

## Comparing `pastell-admin-0.1.16.tar` & `pastell-admin-0.1.17.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:49:28.608570 pastell-admin-0.1.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-04-12 14:49:28.608570 pastell-admin-0.1.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:49:28.608570 pastell-admin-0.1.16/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:49:28.604570 pastell-admin-0.1.16/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:49:28.608570 pastell-admin-0.1.16/src/pastell_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-04-12 14:49:28.000000 pastell-admin-0.1.16/src/pastell_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-12 14:49:28.000000 pastell-admin-0.1.16/src/pastell_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:49:28.000000 pastell-admin-0.1.16/src/pastell_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-12 14:49:28.000000 pastell-admin-0.1.16/src/pastell_admin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 14:49:28.000000 pastell-admin-0.1.16/src/pastell_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 14:49:28.000000 pastell-admin-0.1.16/src/pastell_admin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:49:28.608570 pastell-admin-0.1.16/src/pastelladmin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:49:28.608570 pastell-admin-0.1.16/src/pastelladmin/api/
--rw-r--r--   0 runner    (1001) docker     (123)    19924 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/delete_any.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2181 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_associations.py
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_connector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1990 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_connector_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_docs_delete_from_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_find.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3213 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_matrice_roles.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2540 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_org.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:49:28.608570 pastell-admin-0.1.16/src/pastelladmin/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/shared/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/src/pastell_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-05-04 08:11:01.000000 pastell-admin-0.1.17/src/pastell_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-04 08:11:01.000000 pastell-admin-0.1.17/src/pastell_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:11:01.000000 pastell-admin-0.1.17/src/pastell_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 08:11:01.000000 pastell-admin-0.1.17/src/pastell_admin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 08:11:01.000000 pastell-admin-0.1.17/src/pastell_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 08:11:01.000000 pastell-admin-0.1.17/src/pastell_admin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/src/pastelladmin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/src/pastelladmin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    19924 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/delete_any.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2181 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_associations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15496 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_connector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1990 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_connector_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_docs_delete_from_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_find.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3213 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_matrice_roles.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2540 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/pastell_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:01.847042 pastell-admin-0.1.17/src/pastelladmin/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-04 08:10:52.000000 pastell-admin-0.1.17/src/pastelladmin/shared/configuration.py
```

### Comparing `pastell-admin-0.1.16/LICENSE` & `pastell-admin-0.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.16/PKG-INFO` & `pastell-admin-0.1.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastell-admin
-Version: 0.1.16
+Version: 0.1.17
 Author-email: Sebastien Pelhate <sebastien.pelhate@megalis.bretagne.bzh>, Yann Guenneugues <yann.guenneugues@sib.fr>
 Project-URL: Homepage, https://github.com/megalis-bretagne/scripts-pastell
 Project-URL: Bug Tracker, https://github.com/megalis-bretagne/scripts-pastell/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,22 +17,22 @@
 
 
 # Installation
 
 Pour la version stable :
 
 ```
-pip install pastell-admin==0.1.16
+pip install pastell-admin==0.1.17
 ```
 
 Pour la version de dev :
 
 ```
 pip install requests
-pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.16
+pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.17
 ```
 # Développement
 
 ```
 git clone git@github.com:megalis-bretagne/scripts-pastell.git
 cd scripts-pastell
 python3 -m venv .venv
@@ -181,15 +181,15 @@
 
 ### Paramètres
 
  - `--env` : pour sélectionner l'environnement d'éxécution (**preprod** ou **prod**)
  - `--source` : fichier json contenant la définition du connecteur ou la liste des connecteurs à supprimer ``[{"id_e":"", "id_ce"},]``
  - `--org` : précise l'id_e de l'entité cocernée par la création du connecteur
  - `--recursive` : précise si les entités filles sont également concernées. A associer avec --org=
- - `--flux` : type de dossier (flux). Requis pour les actions de dissociation et de suppression sans fichier source
+ - `--flux` : type de dossier (flux) Liste séparée par des vigules. Requis pour les actions de dissociation et de suppression sans fichier source
  - `--action` : Requis. A choisir parmis [create, update, append, dissociate, delete, status]
  - `--libelle` :  Libellé du connecteur. Requis pour les actions de statut, de dissociation et de suppression sans fichier source
  - `--type` : type de connecteur (eg. GED). Requis pour les actions de dissociation et de suppression sans fichier source
  - `--id_connector` : id_connecteur (eg. depot-pastell). Requis pour les actions de dissociation et de suppression sans fichier source
  - `--details` : A utiliser avec l'action status. Option pour afficher les id_e des entités concernées.
  - `--scheduler` : Pour lancer un connecteur de purge en asynchrone.
```

### Comparing `pastell-admin-0.1.16/README.md` & `pastell-admin-0.1.17/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 
 # Installation
 
 Pour la version stable :
 
 ```
-pip install pastell-admin==0.1.16
+pip install pastell-admin==0.1.17
 ```
 
 Pour la version de dev :
 
 ```
 pip install requests
-pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.16
+pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.17
 ```
 # Développement
 
 ```
 git clone git@github.com:megalis-bretagne/scripts-pastell.git
 cd scripts-pastell
 python3 -m venv .venv
@@ -167,15 +167,15 @@
 
 ### Paramètres
 
  - `--env` : pour sélectionner l'environnement d'éxécution (**preprod** ou **prod**)
  - `--source` : fichier json contenant la définition du connecteur ou la liste des connecteurs à supprimer ``[{"id_e":"", "id_ce"},]``
  - `--org` : précise l'id_e de l'entité cocernée par la création du connecteur
  - `--recursive` : précise si les entités filles sont également concernées. A associer avec --org=
- - `--flux` : type de dossier (flux). Requis pour les actions de dissociation et de suppression sans fichier source
+ - `--flux` : type de dossier (flux) Liste séparée par des vigules. Requis pour les actions de dissociation et de suppression sans fichier source
  - `--action` : Requis. A choisir parmis [create, update, append, dissociate, delete, status]
  - `--libelle` :  Libellé du connecteur. Requis pour les actions de statut, de dissociation et de suppression sans fichier source
  - `--type` : type de connecteur (eg. GED). Requis pour les actions de dissociation et de suppression sans fichier source
  - `--id_connector` : id_connecteur (eg. depot-pastell). Requis pour les actions de dissociation et de suppression sans fichier source
  - `--details` : A utiliser avec l'action status. Option pour afficher les id_e des entités concernées.
  - `--scheduler` : Pour lancer un connecteur de purge en asynchrone.
```

### Comparing `pastell-admin-0.1.16/pyproject.toml` & `pastell-admin-0.1.17/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pastell-admin"
-version = "0.1.16"
+version = "0.1.17"
 authors = [
   { name="Sebastien Pelhate", email="sebastien.pelhate@megalis.bretagne.bzh"}, {name ="Yann Guenneugues" ,email="yann.guenneugues@sib.fr"  }
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pastell-admin-0.1.16/src/pastell_admin.egg-info/PKG-INFO` & `pastell-admin-0.1.17/src/pastell_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastell-admin
-Version: 0.1.16
+Version: 0.1.17
 Author-email: Sebastien Pelhate <sebastien.pelhate@megalis.bretagne.bzh>, Yann Guenneugues <yann.guenneugues@sib.fr>
 Project-URL: Homepage, https://github.com/megalis-bretagne/scripts-pastell
 Project-URL: Bug Tracker, https://github.com/megalis-bretagne/scripts-pastell/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,22 +17,22 @@
 
 
 # Installation
 
 Pour la version stable :
 
 ```
-pip install pastell-admin==0.1.16
+pip install pastell-admin==0.1.17
 ```
 
 Pour la version de dev :
 
 ```
 pip install requests
-pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.16
+pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.17
 ```
 # Développement
 
 ```
 git clone git@github.com:megalis-bretagne/scripts-pastell.git
 cd scripts-pastell
 python3 -m venv .venv
@@ -181,15 +181,15 @@
 
 ### Paramètres
 
  - `--env` : pour sélectionner l'environnement d'éxécution (**preprod** ou **prod**)
  - `--source` : fichier json contenant la définition du connecteur ou la liste des connecteurs à supprimer ``[{"id_e":"", "id_ce"},]``
  - `--org` : précise l'id_e de l'entité cocernée par la création du connecteur
  - `--recursive` : précise si les entités filles sont également concernées. A associer avec --org=
- - `--flux` : type de dossier (flux). Requis pour les actions de dissociation et de suppression sans fichier source
+ - `--flux` : type de dossier (flux) Liste séparée par des vigules. Requis pour les actions de dissociation et de suppression sans fichier source
  - `--action` : Requis. A choisir parmis [create, update, append, dissociate, delete, status]
  - `--libelle` :  Libellé du connecteur. Requis pour les actions de statut, de dissociation et de suppression sans fichier source
  - `--type` : type de connecteur (eg. GED). Requis pour les actions de dissociation et de suppression sans fichier source
  - `--id_connector` : id_connecteur (eg. depot-pastell). Requis pour les actions de dissociation et de suppression sans fichier source
  - `--details` : A utiliser avec l'action status. Option pour afficher les id_e des entités concernées.
  - `--scheduler` : Pour lancer un connecteur de purge en asynchrone.
```

### Comparing `pastell-admin-0.1.16/src/pastell_admin.egg-info/SOURCES.txt` & `pastell-admin-0.1.17/src/pastell_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.16/src/pastelladmin/api/client.py` & `pastell-admin-0.1.17/src/pastelladmin/api/client.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.16/src/pastelladmin/delete_any.py` & `pastell-admin-0.1.17/src/pastelladmin/delete_any.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.16/src/pastelladmin/pastell_associations.py` & `pastell-admin-0.1.17/src/pastelladmin/pastell_associations.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.16/src/pastelladmin/pastell_connector.py` & `pastell-admin-0.1.17/src/pastelladmin/pastell_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
   result = o.copy()
   for key, val in o.items():
     variable = re.findall('{{(.*?)}}', val)
     if variable and os.getenv(variable[0]):
       result[key] = os.getenv(variable[0])
   return result
 
-def taskConnectorFor(session, scope, action, connector_template, delete_list, flux_associe, lib_connector, type_connector, id_connector, details, recursive, scheduler, file):
+def taskConnectorFor(session, scope, action, connector_template, delete_list, flux_associes, lib_connector, type_connector, id_connector, details, recursive, scheduler, file):
   global connector
   if scope == 'all':
     # Get all entities from Pastell API
     request = Entity(session).getAll()
     if request.success:
       entities = request.result
     else:
@@ -130,32 +130,34 @@
         if action in ['append', 'update']:
           print(f"info : entité : {id_e} : mise à jour du connecteur : {id_ce}")
           if type_connector == "transformation":
             parameters = {'file_name': 'definition.json'}
           else:
             parameters = variables_substitution(connector_template["parameters"])
           result = Connector(session).update(id_e, id_ce, parameters, file)
-          if result and flux_associe:
-            Association(session).create(id_e, flux_associe, id_ce, type_connector)
+          if result and flux_associes:
+            for flux in flux_associes:
+              Association(session).create(id_e, flux, id_ce, type_connector)
           if result.success and scheduler:
             Connector(session).action(id_e, id_ce, "purge-async")
 
         elif action == 'dissociate':
           #Dissociate only with the flux specified
-          deleteAssociations(session, id_e, id_ce, flux_associe)
+          for flux in flux_associes:
+            deleteAssociations(session, id_e, id_ce, flux)
         elif action == 'delete':
           deleteConnector(session, id_e, id_ce)
         elif action == 'create':
           # Does not occurs because entities are filtered for this connector
           print(f"warning : le connecteur existe déjà : {id_ce} pour l'entité : {id_e}")
       else:
         if action in ['create', 'append']:
           #Only create connector if does not exists yet
           print(f"info : création du connecteur pour l'entité : {id_e}")
-          createConnecteur(session, id_e, connector_template, flux_associe, lib_connector, type_connector, scheduler, file)
+          createConnecteur(session, id_e, connector_template, flux_associes, lib_connector, type_connector, scheduler, file)
         elif action in ['delete', 'update']:
           # Does not occurs because entities are filtered for this connector
           print(f"warning: Aucun connecteur de type {type_connector}:{id_connector} et libellé {lib_connector} trouvé pour l'entité ({id_e})")
 
 
 def deleteConnector(session, id_e, id_ce):
   #delete associations for this connector
@@ -176,15 +178,15 @@
     if flux:
       print(f"info : désassociation du connecteur {id_ce} avec le flux {association['flux']}")
     else:
       print(f"info: désassociation du connecteur {id_ce} avec tous les flux")
     Association(session).delete(id_e, association["id_fe"])
 
 
-def createConnecteur(session, id_e, connector_template, flux_associe, lib_connector, type_connector, scheduler, file):
+def createConnecteur(session, id_e, connector_template, flux_associes, lib_connector, type_connector, scheduler, file):
   definition = variables_substitution(connector_template["definition"])
   if type_connector == "transformation":
     parameters = {'file_name': 'definition.json'}
   else:
     parameters = variables_substitution(connector_template["parameters"])
   #Etape 1 Creation du connecteur sans sa configuration pour l'IDE sélectionnée
   request = Connector(session).create(id_e, definition)
@@ -192,16 +194,17 @@
     id_ce = request.result
   else:
     print(f"error : {request.result}")
 
   if id_ce:
     # ETAPE 2: configuration du connecteur précédemment créé avec injection des paramètres
     request = Connector(session).update(id_e, id_ce, parameters, file)
-    if request.success and flux_associe:
-      Association(session).create(id_e, flux_associe, id_ce, type_connector)
+    if request.success and flux_associes:
+      for flux in flux_associes:
+        Association(session).create(id_e, flux, id_ce, type_connector)
     if request.success and scheduler:
       Connector(session).action(id_e, id_ce, "purge-async")
 
   else:
     print(f"error : Création du connecteur {lib_connector} KO erreur:{request.result}")
 
 def script_wrapper():
@@ -216,25 +219,25 @@
   parser.add_argument("-t", "--type", type=str, help="type de connecteur (eg. GED)")
   parser.add_argument("-i", "--id_connector", type=str, help="id_connecteur (eg. depot-pastell)")
   parser.add_argument("-d", "--details", action="store_true", help="A utiliser avec l'action status. Pour afficher les id_e des entités concernées")
   parser.add_argument("-r", "--recursive", action="store_true", help="Sélection de l'environnement")
   parser.add_argument("-c", "--scheduler", action="store_true", help="Launch connecteur with existing asynchrone scheduler")
   args = parser.parse_args()
 
-  connector(env=args.env, action=args.action, org=args.org, flux_associe=args.flux, source=args.source,
+  connector(env=args.env, action=args.action, org=args.org, flux_associes=args.flux, source=args.source,
     type_connector=args.type, id_connector=args.id_connector, lib_connector=args.libelle,
     details=args.details, recursive=args.recursive, scheduler=args.scheduler)
 
   xend = datetime.now()
   delta = xend - xstart
   msg = f"info : script exécuté en {delta.seconds // 60} minutes et {delta.seconds % 60} secondes"
   print(msg)
 
 
-def connector(env, action, org=None, flux_associe=None, source=None, type_connector=None, id_connector=None, lib_connector=None, details=None, recursive=None, scheduler=None):
+def connector(env, action, org=None, flux_associes=None, source=None, type_connector=None, id_connector=None, lib_connector=None, details=None, recursive=None, scheduler=None):
   #Get parameters from config file ~/.pastell-admin
   config = getConfiguration()
 
   delete_list = None
   connector_template = None
   file_transformation = None
 
@@ -242,14 +245,18 @@
   for var, value in config[env].items():
     if var not in ('server', 'login', 'password'):
       os.environ[var] = value
 
   #Check for mandatory parameters
   assert action in ['status', 'create', 'append', 'update', 'delete', 'dissociate']
   #if create or append then source is mandatory
+  if flux_associes:
+      flux_associes = flux_associes.split(",")
+  else:
+    flux_associes = []
   if action in ['create', 'append', 'update']:
     assert source != None
     # Opening JSON file
     f = open(source)
     # returns JSON object as dictionary
     connector_template = json.load(f)
     # Récupération des propriétés du connecteur & substitution des variables
@@ -274,15 +281,15 @@
     if source:
       f = open(source)
       # returns JSON object as dictionary
       delete_list = json.load(f)
       # Chek if All items in delete_list contains keys id_ce and id_e
       assert all(key in item.keys() for item in delete_list for key in ["id_ce", "id_e"])
   elif action == 'dissociate':
-    assert (lib_connector and type_connector and id_connector and flux_associe)
+    assert (lib_connector and type_connector and id_connector and len(flux_associes)>0)
   elif action == 'status':
     assert (lib_connector)
 
 
   server = config[env]['server']
   user = config[env]['login']
   pwd = config[env]['password']
@@ -291,15 +298,15 @@
   #Check if session is valid
   if not session.valid:
     exit()
   if action in ['status', 'create', 'append', 'dissociate', 'delete', 'update']:
     scope = 'all'
     if org:
       scope = org
-    taskConnectorFor(session, scope, action, connector_template, delete_list, flux_associe, lib_connector, type_connector, id_connector, details, recursive, scheduler, file=file_transformation)
+    taskConnectorFor(session, scope, action, connector_template, delete_list, flux_associes, lib_connector, type_connector, id_connector, details, recursive, scheduler, file=file_transformation)
     if file_transformation and tmpfile:
       tmpfile.close()
 
 if __name__ == '__main__':
   script_wrapper()
```

### Comparing `pastell-admin-0.1.16/src/pastelladmin/pastell_connector_instances.py` & `pastell-admin-0.1.17/src/pastelladmin/pastell_connector_instances.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.16/src/pastelladmin/pastell_docs_delete_from_list.py` & `pastell-admin-0.1.17/src/pastelladmin/pastell_docs_delete_from_list.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.16/src/pastelladmin/pastell_find.py` & `pastell-admin-0.1.17/src/pastelladmin/pastell_find.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.16/src/pastelladmin/pastell_matrice_roles.py` & `pastell-admin-0.1.17/src/pastelladmin/pastell_matrice_roles.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.16/src/pastelladmin/pastell_org.py` & `pastell-admin-0.1.17/src/pastelladmin/pastell_org.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.16/src/pastelladmin/pastell_stats.py` & `pastell-admin-0.1.17/src/pastelladmin/pastell_stats.py`

 * *Files identical despite different names*

