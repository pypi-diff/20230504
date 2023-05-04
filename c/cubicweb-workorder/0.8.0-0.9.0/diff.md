# Comparing `tmp/cubicweb-workorder-0.8.0.tar.gz` & `tmp/cubicweb-workorder-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-workorder-0.8.0.tar", last modified: Sat Jul 17 08:04:38 2010, max compression, from Unix
+gzip compressed data, was "cubicweb-workorder-0.9.0.tar", last modified: Sun Oct 17 19:37:23 2010, max compression, from Unix
```

## Comparing `cubicweb-workorder-0.8.0.tar` & `cubicweb-workorder-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-07-17 08:04:38.000000 cubicweb-workorder-0.8.0/
--rw-rw-r--   0 syt       (1004) syt       (1004)     4417 2010-07-16 15:51:58.000000 cubicweb-workorder-0.8.0/entities.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     5628 2010-06-07 11:15:34.000000 cubicweb-workorder-0.8.0/setup.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1376 2010-06-07 11:15:34.000000 cubicweb-workorder-0.8.0/views.py
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-07-17 08:04:38.000000 cubicweb-workorder-0.8.0/i18n/
--rw-rw-r--   0 syt       (1004) syt       (1004)     3772 2010-07-16 15:51:50.000000 cubicweb-workorder-0.8.0/i18n/fr.po
--rw-rw-r--   0 syt       (1004) syt       (1004)     3116 2010-06-07 11:15:34.000000 cubicweb-workorder-0.8.0/i18n/en.po
--rw-rw-r--   0 syt       (1004) syt       (1004)     1521 2010-07-16 15:51:58.000000 cubicweb-workorder-0.8.0/__pkginfo__.py
--rw-rw-r--   0 syt       (1004) syt       (1004)      387 2010-07-17 08:04:38.000000 cubicweb-workorder-0.8.0/PKG-INFO
--rw-rw-r--   0 syt       (1004) syt       (1004)      335 2008-10-28 14:23:23.000000 cubicweb-workorder-0.8.0/MANIFEST.in
--rw-rw-r--   0 syt       (1004) syt       (1004)      143 2010-01-27 12:33:55.000000 cubicweb-workorder-0.8.0/__init__.py
--rw-rw-r--   0 syt       (1004) syt       (1004)       45 2008-10-28 14:23:23.000000 cubicweb-workorder-0.8.0/sobjects.py
--rw-rw-r--   0 syt       (1004) syt       (1004)       96 2010-06-07 11:15:34.000000 cubicweb-workorder-0.8.0/README
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-07-17 08:04:38.000000 cubicweb-workorder-0.8.0/test/
--rw-rw-r--   0 syt       (1004) syt       (1004)     1148 2008-10-28 14:23:23.000000 cubicweb-workorder-0.8.0/test/pytestconf.py
--rw-rw-r--   0 syt       (1004) syt       (1004)      372 2009-06-24 11:42:42.000000 cubicweb-workorder-0.8.0/test/test_workorder.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1106 2008-10-28 14:23:23.000000 cubicweb-workorder-0.8.0/test/realdb_test_workorder.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1216 2010-07-16 15:51:58.000000 cubicweb-workorder-0.8.0/hooks.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1453 2010-06-07 11:15:34.000000 cubicweb-workorder-0.8.0/schema.py
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-07-17 08:04:38.000000 cubicweb-workorder-0.8.0/cubicweb_workorder.egg-info/
--rw-rw-r--   0 syt       (1004) syt       (1004)       17 2010-07-17 08:04:37.000000 cubicweb-workorder-0.8.0/cubicweb_workorder.egg-info/requires.txt
--rw-rw-r--   0 syt       (1004) syt       (1004)       10 2010-07-17 08:04:37.000000 cubicweb-workorder-0.8.0/cubicweb_workorder.egg-info/top_level.txt
--rw-rw-r--   0 syt       (1004) syt       (1004)        1 2010-07-17 08:04:37.000000 cubicweb-workorder-0.8.0/cubicweb_workorder.egg-info/dependency_links.txt
--rw-rw-r--   0 syt       (1004) syt       (1004)      601 2010-07-17 08:04:37.000000 cubicweb-workorder-0.8.0/cubicweb_workorder.egg-info/SOURCES.txt
--rw-rw-r--   0 syt       (1004) syt       (1004)      387 2010-07-17 08:04:37.000000 cubicweb-workorder-0.8.0/cubicweb_workorder.egg-info/PKG-INFO
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-07-17 08:04:38.000000 cubicweb-workorder-0.8.0/migration/
--rw-rw-r--   0 syt       (1004) syt       (1004)     1144 2009-08-18 14:21:56.000000 cubicweb-workorder-0.8.0/migration/0.6.0_Any.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1254 2010-01-27 12:33:55.000000 cubicweb-workorder-0.8.0/migration/postcreate.py
--rw-rw-r--   0 syt       (1004) syt       (1004)       33 2010-06-07 11:15:34.000000 cubicweb-workorder-0.8.0/migration/0.6.2_Any.py
--rw-rw-r--   0 syt       (1004) syt       (1004)       59 2010-07-17 08:04:38.000000 cubicweb-workorder-0.8.0/setup.cfg
+drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-10-17 19:37:23.000000 cubicweb-workorder-0.9.0/
+-rw-rw-r--   0 syt       (1004) syt       (1004)     2924 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/entities.py
+-rw-rw-r--   0 syt       (1004) syt       (1004)     5628 2010-06-07 11:15:34.000000 cubicweb-workorder-0.9.0/setup.py
+-rw-rw-r--   0 syt       (1004) syt       (1004)     1212 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/views.py
+drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-10-17 19:37:23.000000 cubicweb-workorder-0.9.0/i18n/
+-rw-rw-r--   0 syt       (1004) syt       (1004)     3604 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/i18n/fr.po
+-rw-rw-r--   0 syt       (1004) syt       (1004)     2927 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/i18n/en.po
+-rw-rw-r--   0 syt       (1004) syt       (1004)     1522 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/__pkginfo__.py
+-rw-rw-r--   0 syt       (1004) syt       (1004)      387 2010-10-17 19:37:23.000000 cubicweb-workorder-0.9.0/PKG-INFO
+-rw-rw-r--   0 syt       (1004) syt       (1004)      335 2008-10-28 14:23:23.000000 cubicweb-workorder-0.9.0/MANIFEST.in
+-rw-rw-r--   0 syt       (1004) syt       (1004)      143 2010-01-27 12:33:55.000000 cubicweb-workorder-0.9.0/__init__.py
+-rw-rw-r--   0 syt       (1004) syt       (1004)       45 2008-10-28 14:23:23.000000 cubicweb-workorder-0.9.0/sobjects.py
+-rw-rw-r--   0 syt       (1004) syt       (1004)       96 2010-06-07 11:15:34.000000 cubicweb-workorder-0.9.0/README
+drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-10-17 19:37:23.000000 cubicweb-workorder-0.9.0/test/
+-rw-rw-r--   0 syt       (1004) syt       (1004)     1148 2008-10-28 14:23:23.000000 cubicweb-workorder-0.9.0/test/pytestconf.py
+-rw-rw-r--   0 syt       (1004) syt       (1004)      372 2009-06-24 11:42:42.000000 cubicweb-workorder-0.9.0/test/test_workorder.py
+-rw-rw-r--   0 syt       (1004) syt       (1004)     1106 2008-10-28 14:23:23.000000 cubicweb-workorder-0.9.0/test/realdb_test_workorder.py
+-rw-rw-r--   0 syt       (1004) syt       (1004)     2216 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/hooks.py
+-rw-rw-r--   0 syt       (1004) syt       (1004)     1225 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/schema.py
+drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-10-17 19:37:23.000000 cubicweb-workorder-0.9.0/cubicweb_workorder.egg-info/
+-rw-rw-r--   0 syt       (1004) syt       (1004)       18 2010-10-17 19:37:22.000000 cubicweb-workorder-0.9.0/cubicweb_workorder.egg-info/requires.txt
+-rw-rw-r--   0 syt       (1004) syt       (1004)       10 2010-10-17 19:37:22.000000 cubicweb-workorder-0.9.0/cubicweb_workorder.egg-info/top_level.txt
+-rw-rw-r--   0 syt       (1004) syt       (1004)        1 2010-10-17 19:37:22.000000 cubicweb-workorder-0.9.0/cubicweb_workorder.egg-info/dependency_links.txt
+-rw-rw-r--   0 syt       (1004) syt       (1004)      624 2010-10-17 19:37:22.000000 cubicweb-workorder-0.9.0/cubicweb_workorder.egg-info/SOURCES.txt
+-rw-rw-r--   0 syt       (1004) syt       (1004)      387 2010-10-17 19:37:22.000000 cubicweb-workorder-0.9.0/cubicweb_workorder.egg-info/PKG-INFO
+drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-10-17 19:37:23.000000 cubicweb-workorder-0.9.0/migration/
+-rw-rw-r--   0 syt       (1004) syt       (1004)     1144 2009-08-18 14:21:56.000000 cubicweb-workorder-0.9.0/migration/0.6.0_Any.py
+-rw-rw-r--   0 syt       (1004) syt       (1004)     1254 2010-01-27 12:33:55.000000 cubicweb-workorder-0.9.0/migration/postcreate.py
+-rw-rw-r--   0 syt       (1004) syt       (1004)      176 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/migration/0.9.0_Any.py
+-rw-rw-r--   0 syt       (1004) syt       (1004)       33 2010-06-07 11:15:34.000000 cubicweb-workorder-0.9.0/migration/0.6.2_Any.py
+-rw-rw-r--   0 syt       (1004) syt       (1004)       59 2010-10-17 19:37:23.000000 cubicweb-workorder-0.9.0/setup.cfg
```

### Comparing `cubicweb-workorder-0.8.0/setup.py` & `cubicweb-workorder-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-workorder-0.8.0/views.py` & `cubicweb-workorder-0.9.0/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 """template-specific forms/views/actions/components"""
 
+from cubicweb.selectors import is_instance
 from cubicweb.web import uicfg
+from cubicweb.web.views.ibreadcrumbs import IBreadCrumbsAdapter
+
+class WorkOrderIBreadCrumbsAdapter(IBreadCrumbsAdapter):
+    __select__ = is_instance('WorkOrder')
+
+    def parent_entity(self):
+        return self.entity.order
+
+_pvs = uicfg.primaryview_section
+_pvdc = uicfg.primaryview_display_ctrl
+_afs = uicfg.autoform_section
 
 # Order
-uicfg.primaryview_section.tag_subject_of(('Order', 'split_into', '*'),
-                                         'relations')
-uicfg.primaryview_section.tag_attribute(('Order', 'budget'), 'hidden')
-uicfg.primaryview_section.tag_attribute(('Order', 'progress_target'), 'hidden')
-uicfg.primaryview_section.tag_attribute(('Order', 'progress_done'), 'hidden')
-uicfg.primaryview_section.tag_attribute(('Order', 'progress_todo'), 'hidden')
-uicfg.primaryview_display_ctrl.tag_subject_of(('Order', 'split_into', '*'),
-                                              {'vid': 'ic_progress_table_view'})
-
-uicfg.autoform_section.tag_attribute(('Order', 'budget'), 'main', 'hidden')
-uicfg.autoform_section.tag_attribute(('Order', 'progress_target'), 'main', 'hidden')
-uicfg.autoform_section.tag_attribute(('Order', 'progress_todo'), 'main', 'hidden')
-uicfg.autoform_section.tag_attribute(('Order', 'progress_done'), 'main', 'hidden')
-uicfg.autoform_section.tag_subject_of(('Order', 'split_into', '*'), 'main', 'inlined')
+_pvs.tag_subject_of(('Order', 'split_into', '*'), 'relations')
+_pvs.tag_attribute(('Order', 'budget'), 'hidden')
+_pvs.tag_attribute(('Order', 'progress_done'), 'hidden')
+_pvs.tag_attribute(('Order', 'progress_todo'), 'hidden')
+_pvdc.tag_subject_of(('Order', 'split_into', '*'),
+                     {'vid': 'ic_progress_table_view'})
+
+_afs.tag_attribute(('Order', 'budget'), 'main', 'hidden')
+_afs.tag_attribute(('Order', 'progress_todo'), 'main', 'hidden')
+_afs.tag_attribute(('Order', 'progress_done'), 'main', 'hidden')
+_afs.tag_subject_of(('Order', 'split_into', '*'), 'main', 'inlined')
 
 # WorkOrder
-uicfg.autoform_section.tag_attribute(('WorkOrder', 'progress_target'), 'main', 'hidden')
-uicfg.autoform_section.tag_attribute(('WorkOrder', 'progress_todo'), 'main', 'hidden')
-uicfg.autoform_section.tag_attribute(('WorkOrder', 'progress_done'), 'main', 'hidden')
+_afs.tag_attribute(('WorkOrder', 'progress_todo'), 'main', 'hidden')
+_afs.tag_attribute(('WorkOrder', 'progress_done'), 'main', 'hidden')
```

### Comparing `cubicweb-workorder-0.8.0/i18n/fr.po` & `cubicweb-workorder-0.9.0/i18n/fr.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: 2.0\n"
 "POT-Creation-Date: 2006-01-12 17:35+CET\n"
 "PO-Revision-Date: 2008-02-15 12:55+0100\n"
 "Last-Translator: Logilab\n"
 "Language-Team: French <devel@logilab.fr.org>\n"
+"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "New Order"
@@ -28,18 +29,18 @@
 
 msgid "This Order"
 msgstr "Cette commande"
 
 msgid "This WorkOrder"
 msgstr "Ce lot"
 
-msgctxt "inlined:Order.split_into.subject"
 msgid "WorkOrder"
 msgstr "Lot"
 
+msgctxt "inlined:Order.split_into.subject"
 msgid "WorkOrder"
 msgstr "Lot"
 
 msgid "WorkOrder_plural"
 msgstr "Lots"
 
 # add related box generated message
@@ -61,19 +62,19 @@
 msgctxt "WorkOrder"
 msgid "begin_date"
 msgstr "date de début"
 
 msgid "budget"
 msgstr "budget"
 
-msgctxt "WorkOrder"
+msgctxt "Order"
 msgid "budget"
 msgstr "budget"
 
-msgctxt "Order"
+msgctxt "WorkOrder"
 msgid "budget"
 msgstr "budget"
 
 msgid "cancel"
 msgstr "annuler"
 
 msgid "canceled"
@@ -136,41 +137,30 @@
 
 msgid "planned"
 msgstr "prévu"
 
 msgid "progress_done"
 msgstr "progrès: fait"
 
-msgctxt "WorkOrder"
-msgid "progress_done"
-msgstr "progrès: fait"
-
 msgctxt "Order"
 msgid "progress_done"
 msgstr "progrès: fait"
 
-msgid "progress_target"
-msgstr "progrès: cible"
-
 msgctxt "WorkOrder"
-msgid "progress_target"
-msgstr "progrès: cible"
-
-msgctxt "Order"
-msgid "progress_target"
+msgid "progress_done"
 msgstr "progrès: fait"
 
 msgid "progress_todo"
 msgstr "progrès: restant"
 
-msgctxt "WorkOrder"
+msgctxt "Order"
 msgid "progress_todo"
 msgstr "progrès: restant"
 
-msgctxt "Order"
+msgctxt "WorkOrder"
 msgid "progress_todo"
 msgstr "progrès: restant"
 
 msgid "receive"
 msgstr "reçu"
 
 msgid "send"
@@ -182,29 +172,29 @@
 msgid "split_into"
 msgstr "divisé en"
 
 msgctxt "Order"
 msgid "split_into"
 msgstr "divisé en"
 
-msgctxt "WorkOrder"
 msgid "split_into_object"
 msgstr "fait partie de"
 
+msgctxt "WorkOrder"
 msgid "split_into_object"
 msgstr "fait partie de"
 
 msgid "start"
 msgstr "commencer"
 
-msgctxt "WorkOrder"
+msgctxt "Order"
 msgid "title"
 msgstr "titre"
 
-msgctxt "Order"
+msgctxt "WorkOrder"
 msgid "title"
 msgstr "titre"
 
 msgid "validated"
 msgstr "validé"
 
 msgid "warrant"
```

### Comparing `cubicweb-workorder-0.8.0/i18n/en.po` & `cubicweb-workorder-0.9.0/i18n/en.po`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
 msgid "This Order"
 msgstr "This order"
 
 msgid "This WorkOrder"
 msgstr "This work-order"
 
-msgctxt "inlined:Order.split_into.subject"
 msgid "WorkOrder"
 msgstr "Work-order"
 
+msgctxt "inlined:Order.split_into.subject"
 msgid "WorkOrder"
 msgstr "Work-order"
 
 msgid "WorkOrder_plural"
 msgstr "Work orders"
 
 # add related box generated message
@@ -55,19 +55,19 @@
 msgctxt "WorkOrder"
 msgid "begin_date"
 msgstr "begin date"
 
 msgid "budget"
 msgstr ""
 
-msgctxt "WorkOrder"
+msgctxt "Order"
 msgid "budget"
 msgstr ""
 
-msgctxt "Order"
+msgctxt "WorkOrder"
 msgid "budget"
 msgstr ""
 
 msgid "cancel"
 msgstr ""
 
 msgid "canceled"
@@ -130,41 +130,30 @@
 
 msgid "planned"
 msgstr ""
 
 msgid "progress_done"
 msgstr "progress: done"
 
-msgctxt "WorkOrder"
-msgid "progress_done"
-msgstr "progress: done"
-
 msgctxt "Order"
 msgid "progress_done"
 msgstr "progress: done"
 
-msgid "progress_target"
-msgstr "progress: target"
-
 msgctxt "WorkOrder"
-msgid "progress_target"
-msgstr "progress: target"
-
-msgctxt "Order"
-msgid "progress_target"
-msgstr "progress: target"
+msgid "progress_done"
+msgstr "progress: done"
 
 msgid "progress_todo"
 msgstr "progress: todo"
 
-msgctxt "WorkOrder"
+msgctxt "Order"
 msgid "progress_todo"
 msgstr "progress: todo"
 
-msgctxt "Order"
+msgctxt "WorkOrder"
 msgid "progress_todo"
 msgstr "progress: todo"
 
 msgid "receive"
 msgstr ""
 
 msgid "send"
@@ -176,29 +165,29 @@
 msgid "split_into"
 msgstr "split into"
 
 msgctxt "Order"
 msgid "split_into"
 msgstr "split into"
 
-msgctxt "WorkOrder"
 msgid "split_into_object"
 msgstr "part of"
 
+msgctxt "WorkOrder"
 msgid "split_into_object"
 msgstr "part of"
 
 msgid "start"
 msgstr ""
 
-msgctxt "WorkOrder"
+msgctxt "Order"
 msgid "title"
 msgstr "title"
 
-msgctxt "Order"
+msgctxt "WorkOrder"
 msgid "title"
 msgstr "title"
 
 msgid "validated"
 msgstr ""
 
 msgid "warrant"
```

### Comparing `cubicweb-workorder-0.8.0/__pkginfo__.py` & `cubicweb-workorder-0.9.0/__pkginfo__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # pylint: disable-msg=W0622
 """cubicweb-workorder application packaging information"""
 
 modname = 'workorder'
 distname = 'cubicweb-%s' % modname
 
-numversion = (0, 8, 0)
+numversion = (0, 9, 0)
 version = '.'.join(str(num) for num in numversion)
 
 license = 'LGPL'
 description = 'workorder component for the CubicWeb framework'
 web = 'http://www.cubicweb.org/project/%s' % distname
 author = 'Logilab'
 author_email = 'contact@logilab.fr'
 classifiers = [
            'Environment :: Web Environment',
            'Framework :: CubicWeb',
            'Programming Language :: Python',
            'Programming Language :: JavaScript',
 ]
 
-__depends__ = {'cubicweb': '>= 3.9.0'}
+__depends__ = {'cubicweb': '>= 3.10.0'}
 
 
 # packaging ###
 
 from os import listdir as _listdir
 from os.path import join, isdir
 from glob import glob
```

### Comparing `cubicweb-workorder-0.8.0/test/pytestconf.py` & `cubicweb-workorder-0.9.0/test/pytestconf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-workorder-0.8.0/test/realdb_test_workorder.py` & `cubicweb-workorder-0.9.0/test/realdb_test_workorder.py`

 * *Files identical despite different names*

### Comparing `cubicweb-workorder-0.8.0/schema.py` & `cubicweb-workorder-0.9.0/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 from yams.buildobjs import (EntityType, SubjectRelation, ObjectRelation,
-                            String, Date, Float)
-try:
-    from yams.buildobjs import RichString
-except ImportError:
-    from cubicweb.schema import RichString
-
+                            String, Date, Float, RichString)
 from cubicweb.schema import RQLConstraint, WorkflowableEntityType
 
 _ = unicode
 
 class Order(WorkflowableEntityType):
     title = String(required=True, fulltextindexed=True, maxsize=128, unique=True)
     date = Date(description=_('date order was placed on'))
     split_into = SubjectRelation('WorkOrder', cardinality='*1', composite='subject')
 
     # computed attributes
     budget = Float(description=_('computed attribute'))
-    progress_target = Float(description=_('computed attribute'))
     progress_done = Float(description=_('computed attribute'))
     progress_todo = Float(description=_('computed attribute'))
 
+
 class WorkOrder(WorkflowableEntityType):
     title = String(required=True, fulltextindexed=True, indexed=True, maxsize=128)
     description = RichString(fulltextindexed=True)
     budget = Float(description=_('amount that should not be overspent'))
     begin_date = Date(description=_('date work order will begin on'))
     end_date = Date(description=_('date work order will end on'))
 
     # computed attributes
-    progress_target = Float(description=_('computed attribute'))
     progress_done = Float(description=_('computed attribute'))
     progress_todo = Float(description=_('computed attribute'))
```

### Comparing `cubicweb-workorder-0.8.0/cubicweb_workorder.egg-info/SOURCES.txt` & `cubicweb-workorder-0.9.0/cubicweb_workorder.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 cubicweb_workorder.egg-info/dependency_links.txt
 cubicweb_workorder.egg-info/requires.txt
 cubicweb_workorder.egg-info/top_level.txt
 i18n/en.po
 i18n/fr.po
 migration/0.6.0_Any.py
 migration/0.6.2_Any.py
+migration/0.9.0_Any.py
 migration/postcreate.py
 test/test_workorder.py
```

### Comparing `cubicweb-workorder-0.8.0/migration/0.6.0_Any.py` & `cubicweb-workorder-0.9.0/migration/0.6.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-workorder-0.8.0/migration/postcreate.py` & `cubicweb-workorder-0.9.0/migration/postcreate.py`

 * *Files identical despite different names*

