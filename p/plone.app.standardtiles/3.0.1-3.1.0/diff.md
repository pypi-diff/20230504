# Comparing `tmp/plone.app.standardtiles-3.0.1.tar.gz` & `tmp/plone.app.standardtiles-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.standardtiles-3.0.1.tar", last modified: Sat Apr 22 13:58:37 2023, max compression
+gzip compressed data, was "plone.app.standardtiles-3.1.0.tar", last modified: Thu May  4 10:08:12 2023, max compression
```

## Comparing `plone.app.standardtiles-3.0.1.tar` & `plone.app.standardtiles-3.1.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.537007 plone.app.standardtiles-3.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)    10731 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      750 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      178 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    12898 2023-04-22 13:58:37.537156 plone.app.standardtiles-3.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1061 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      289 2023-04-22 13:58:37.537680 plone.app.standardtiles-3.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1994 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.508303 plone.app.standardtiles-3.0.1/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.512329 plone.app.standardtiles-3.0.1/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.514949 plone.app.standardtiles-3.0.1/src/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.523966 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/
--rw-r--r--   0 maurits    (501) staff       (20)      122 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3764 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/attachment.py
--rw-r--r--   0 maurits    (501) staff       (20)    11183 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/common.py
--rw-r--r--   0 maurits    (501) staff       (20)     4184 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5249 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/content.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9084 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/contentlisting.py
--rw-r--r--   0 maurits    (501) staff       (20)     2330 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/discussion.py
--rw-r--r--   0 maurits    (501) staff       (20)      739 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/embed.py
--rw-r--r--   0 maurits    (501) staff       (20)     8463 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/existingcontent.py
--rw-r--r--   0 maurits    (501) staff       (20)     5775 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/field.py
--rw-r--r--   0 maurits    (501) staff       (20)     2182 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/head.py
--rw-r--r--   0 maurits    (501) staff       (20)     1909 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/head.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1426 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/html.py
--rw-r--r--   0 maurits    (501) staff       (20)      587 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     4359 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/layout.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1002 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/linkintegrity.py
--rw-r--r--   0 maurits    (501) staff       (20)     1688 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/media.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1361 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/metadata.py
--rw-r--r--   0 maurits    (501) staff       (20)    11827 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/navigation.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.526970 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3940 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/add.py
--rw-r--r--   0 maurits    (501) staff       (20)     1968 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/assignment.py
--rw-r--r--   0 maurits    (501) staff       (20)     2563 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      317 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/delete.py
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/edit.py
--rw-r--r--   0 maurits    (501) staff       (20)     2282 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/portlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     1799 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/portletmanager.py
--rw-r--r--   0 maurits    (501) staff       (20)     1970 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1720 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.509155 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.527799 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      184 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      207 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/default/portlets.xml
--rw-r--r--   0 maurits    (501) staff       (20)     4557 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/default/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.528537 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      239 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/uninstall/portlets..xml
--rw-r--r--   0 maurits    (501) staff       (20)      146 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/uninstall/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1382 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/rawembed.py
--rw-r--r--   0 maurits    (501) staff       (20)     8427 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/rss.py
--rw-r--r--   0 maurits    (501) staff       (20)      780 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1000 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/sitemap.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.533534 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1761 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/attachment_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2251 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/configlets.pt
--rw-r--r--   0 maurits    (501) staff       (20)      728 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/contentlisting_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      457 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/description.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3905 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/existingcontent_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      762 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/image.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3433 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/listing_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5767 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/login.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1477 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/namedimage.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1501 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/navigation.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2143 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/navigation_recurse.pt
--rw-r--r--   0 maurits    (501) staff       (20)      681 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/navigationlink.pt
--rw-r--r--   0 maurits    (501) staff       (20)      767 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/rawembed.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1689 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/rss.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5336 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/summary_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4803 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/tabular_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      368 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/title.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9747 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/testing.py
--rw-r--r--   0 maurits    (501) staff       (20)      698 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/testing.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.536771 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/
--rw-r--r--   0 maurits    (501) staff       (20)     2921 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/RSS.xml
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      746 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)      969 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/funky_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     7293 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_content.py
--rw-r--r--   0 maurits    (501) staff       (20)    14645 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_existing_content.py
--rw-r--r--   0 maurits    (501) staff       (20)    10897 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_field.py
--rw-r--r--   0 maurits    (501) staff       (20)     6241 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_head.py
--rw-r--r--   0 maurits    (501) staff       (20)    15107 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_layout.py
--rw-r--r--   0 maurits    (501) staff       (20)     7409 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_media.py
--rw-r--r--   0 maurits    (501) staff       (20)     1650 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      272 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)      746 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/upgrades.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1854 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2489 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/viewletmanager.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.514706 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    12898 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3964 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      259 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/top_level.txt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-04 10:08:12.817982 plone.app.standardtiles-3.1.0/
+-rw-r--r--   0 peterm     (501) staff       (20)    10911 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/CHANGES.rst
+-rw-r--r--   0 peterm     (501) staff       (20)    12282 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/LICENSE.GPL
+-rw-r--r--   0 peterm     (501) staff       (20)      750 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/LICENSE.txt
+-rw-r--r--   0 peterm     (501) staff       (20)      178 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/MANIFEST.in
+-rw-r--r--   0 peterm     (501) staff       (20)    13078 2023-05-04 10:08:12.818070 plone.app.standardtiles-3.1.0/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     1061 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/README.rst
+-rw-r--r--   0 peterm     (501) staff       (20)      289 2023-05-04 10:08:12.818306 plone.app.standardtiles-3.1.0/setup.cfg
+-rw-r--r--   0 peterm     (501) staff       (20)     1992 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/setup.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-04 10:08:12.806775 plone.app.standardtiles-3.1.0/src/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-04 10:08:12.808343 plone.app.standardtiles-3.1.0/src/plone/
+-rw-r--r--   0 peterm     (501) staff       (20)       56 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-04 10:08:12.809442 plone.app.standardtiles-3.1.0/src/plone/app/
+-rw-r--r--   0 peterm     (501) staff       (20)       56 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-04 10:08:12.812868 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/
+-rw-r--r--   0 peterm     (501) staff       (20)      122 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     3763 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/attachment.py
+-rw-r--r--   0 peterm     (501) staff       (20)    11182 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/common.py
+-rw-r--r--   0 peterm     (501) staff       (20)     4184 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     5249 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/content.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)    10594 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/contentlisting.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2330 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/discussion.py
+-rw-r--r--   0 peterm     (501) staff       (20)      739 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/embed.py
+-rw-r--r--   0 peterm     (501) staff       (20)     8462 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/existingcontent.py
+-rw-r--r--   0 peterm     (501) staff       (20)     5774 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/field.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2182 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/head.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1909 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/head.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1425 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/html.py
+-rw-r--r--   0 peterm     (501) staff       (20)      587 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/interfaces.py
+-rw-r--r--   0 peterm     (501) staff       (20)     4359 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/layout.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1002 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/linkintegrity.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1688 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/media.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1361 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/metadata.py
+-rw-r--r--   0 peterm     (501) staff       (20)    11827 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/navigation.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-04 10:08:12.814036 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     3940 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/add.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1968 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/assignment.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2563 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)      317 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/delete.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1185 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/edit.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2298 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/portlet.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1799 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/portletmanager.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1970 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/utils.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1720 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/vocabularies.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-04 10:08:12.807193 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/profiles/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-04 10:08:12.814388 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/profiles/default/
+-rw-r--r--   0 peterm     (501) staff       (20)      184 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/profiles/default/metadata.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      207 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/profiles/default/portlets.xml
+-rw-r--r--   0 peterm     (501) staff       (20)     4557 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/profiles/default/registry.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-04 10:08:12.814626 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/profiles/uninstall/
+-rw-r--r--   0 peterm     (501) staff       (20)      239 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/profiles/uninstall/portlets..xml
+-rw-r--r--   0 peterm     (501) staff       (20)      146 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/profiles/uninstall/registry.xml
+-rw-r--r--   0 peterm     (501) staff       (20)     1382 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/rawembed.py
+-rw-r--r--   0 peterm     (501) staff       (20)     8427 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/rss.py
+-rw-r--r--   0 peterm     (501) staff       (20)      780 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/setuphandlers.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1000 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/sitemap.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-04 10:08:12.816616 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/
+-rw-r--r--   0 peterm     (501) staff       (20)     1761 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/attachment_listing.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     2251 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/configlets.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      728 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/contentlisting_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      457 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/description.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     3905 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/existingcontent_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      762 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/image.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     3686 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/listing_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     5767 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/login.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     1477 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/namedimage.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     1501 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/navigation.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     2143 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/navigation_recurse.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      681 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/navigationlink.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      767 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/rawembed.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     1689 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/rss.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     5453 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/summary_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     4940 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/tabular_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      368 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/title.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     9746 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/testing.py
+-rw-r--r--   0 peterm     (501) staff       (20)      698 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/testing.zcml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-04 10:08:12.817872 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/
+-rw-r--r--   0 peterm     (501) staff       (20)     2921 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/RSS.xml
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)      746 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      969 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/funky_display.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     7293 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/test_content.py
+-rw-r--r--   0 peterm     (501) staff       (20)    14645 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/test_existing_content.py
+-rw-r--r--   0 peterm     (501) staff       (20)    10897 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/test_field.py
+-rw-r--r--   0 peterm     (501) staff       (20)     6241 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/test_head.py
+-rw-r--r--   0 peterm     (501) staff       (20)    15107 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/test_layout.py
+-rw-r--r--   0 peterm     (501) staff       (20)     7409 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/test_media.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1647 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/test_setup.py
+-rw-r--r--   0 peterm     (501) staff       (20)      272 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/upgrades.py
+-rw-r--r--   0 peterm     (501) staff       (20)      746 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/upgrades.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1854 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/utils.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2488 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/viewletmanager.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-04 10:08:12.809320 plone.app.standardtiles-3.1.0/src/plone.app.standardtiles.egg-info/
+-rw-r--r--   0 peterm     (501) staff       (20)    13078 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone.app.standardtiles.egg-info/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     3964 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone.app.standardtiles.egg-info/SOURCES.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone.app.standardtiles.egg-info/dependency_links.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       40 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone.app.standardtiles.egg-info/entry_points.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       16 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone.app.standardtiles.egg-info/namespace_packages.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone.app.standardtiles.egg-info/not-zip-safe
+-rw-r--r--   0 peterm     (501) staff       (20)      257 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone.app.standardtiles.egg-info/requires.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        6 2023-05-04 10:08:12.000000 plone.app.standardtiles-3.1.0/src/plone.app.standardtiles.egg-info/top_level.txt
```

### Comparing `plone.app.standardtiles-3.0.1/CHANGES.rst` & `plone.app.standardtiles-3.1.0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,671 +1,682 @@
 00000000: 4368 616e 6765 6c6f 670a 3d3d 3d3d 3d3d  Changelog.======
-00000010: 3d3d 3d0a 0a33 2e30 2e31 2028 3230 3233  ===..3.0.1 (2023
-00000020: 2d30 342d 3232 290a 2d2d 2d2d 2d2d 2d2d  -04-22).--------
-00000030: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2d20 4669  ----------..- Fi
-00000040: 7820 6272 6f6b 656e 2043 4d46 4479 6e61  x broken CMFDyna
-00000050: 6d69 6356 6965 7746 5449 2069 6d70 6f72  micViewFTI impor
-00000060: 742e 0a20 205b 7468 6574 5d0a 0a2d 2046  t..  [thet]..- F
-00000070: 6978 2062 796c 696e 6520 7669 6577 6c65  ix byline viewle
-00000080: 7420 6e61 6d65 0a20 205b 6672 6170 656c  t name.  [frapel
-00000090: 6c5d 0a0a 0a33 2e30 2e30 2028 3230 3232  l]...3.0.0 (2022
-000000a0: 2d31 322d 3035 290a 2d2d 2d2d 2d2d 2d2d  -12-05).--------
-000000b0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2d20 4164  ----------..- Ad
-000000c0: 6465 6420 6c69 6e6b 696e 7465 6772 6974  ded linkintegrit
-000000d0: 7920 666f 7220 6874 6d6c 2061 6e64 2065  y for html and e
-000000e0: 7869 7374 696e 6763 6f6e 7465 6e74 2074  xistingcontent t
-000000f0: 696c 652e 0a20 2043 6f64 6520 6973 2070  ile..  Code is p
-00000100: 6f72 7465 6420 666f 726d 2076 6572 7369  orted form versi
-00000110: 6f6e 2032 2e35 2e30 2c20 616e 6420 6973  on 2.5.0, and is
-00000120: 206f 6e6c 7920 6163 7469 7665 2077 6865   only active whe
-00000130: 6e0a 2020 706c 6f6e 652e 6170 702e 626c  n.  plone.app.bl
-00000140: 6f63 6b73 2076 6572 7369 6f6e 2036 2e30  ocks version 6.0
-00000150: 2e32 206f 7220 6869 6768 6572 2069 7320  .2 or higher is 
-00000160: 7573 6564 2e0a 2020 5b70 6574 7363 686b  used..  [petschk
-00000170: 695d 0a0a 0a33 2e30 2e30 6231 2028 3230  i]...3.0.0b1 (20
-00000180: 3232 2d30 362d 3234 290a 2d2d 2d2d 2d2d  22-06-24).------
-00000190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-000001a0: 2d20 4669 7820 6060 6973 4465 6661 756c  - Fix ``isDefaul
-000001b0: 7450 6167 6560 6020 696d 706f 7274 2077  tPage`` import w
-000001c0: 6869 6368 2077 6173 206d 6f76 6564 2074  hich was moved t
-000001d0: 6f20 6060 706c 6f6e 652e 6261 7365 2e64  o ``plone.base.d
-000001e0: 6566 6175 6c74 7061 6765 6060 0a20 205b  efaultpage``.  [
-000001f0: 7065 7473 6368 6b69 5d0a 0a2d 2043 6c65  petschki]..- Cle
-00000200: 616e 7570 2061 6e64 2066 6978 2045 7869  anup and fix Exi
-00000210: 7374 696e 6743 6f6e 7465 6e74 5469 6c65  stingContentTile
-00000220: 2069 6e20 352e 320a 2020 5b67 6f74 6368   in 5.2.  [gotch
-00000230: 612c 204d 7963 6861 6531 5d0a 0a0a 332e  a, Mychae1]...3.
-00000240: 302e 3061 3220 2832 3032 322d 3034 2d30  0.0a2 (2022-04-0
-00000250: 3129 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  1).-------------
-00000260: 2d2d 2d2d 2d2d 2d0a 0a2d 2046 6978 6564  -------..- Fixed
-00000270: 204b 6579 4572 726f 7220 6060 7265 7375   KeyError ``resu
-00000280: 6c74 7360 6020 696e 2074 6162 756c 6172  lts`` in tabular
-00000290: 2076 6965 772e 2020 5368 6f75 6c64 2068   view.  Should h
-000002a0: 6176 6520 6265 656e 2060 6062 6174 6368  ave been ``batch
-000002b0: 6060 2e0a 2020 4669 7865 7320 6069 7373  ``..  Fixes `iss
-000002c0: 7565 2031 3232 203c 6874 7470 733a 2f2f  ue 122 <https://
-000002d0: 6769 7468 7562 2e63 6f6d 2f70 6c6f 6e65  github.com/plone
-000002e0: 2f70 6c6f 6e65 2e61 7070 2e73 7461 6e64  /plone.app.stand
-000002f0: 6172 6474 696c 6573 2f69 7373 7565 732f  ardtiles/issues/
-00000300: 3132 323e 605f 2e0a 2020 5b6d 6175 7269  122>`_..  [mauri
-00000310: 7473 5d0a 0a0a 332e 302e 3061 3120 2832  ts]...3.0.0a1 (2
-00000320: 3032 322d 3033 2d32 3329 0a2d 2d2d 2d2d  022-03-23).-----
-00000330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00000340: 0a2d 2046 6978 2073 686f 7769 6e67 2070  .- Fix showing p
-00000350: 7269 7661 7465 2063 6f6e 7465 6e74 2077  rivate content w
-00000360: 6869 6c65 2065 6469 7469 6e67 2061 2074  hile editing a t
-00000370: 696c 652e 0a20 2046 6978 6573 2060 6973  ile..  Fixes `is
-00000380: 7375 6520 3130 3020 3c68 7474 7073 3a2f  sue 100 <https:/
-00000390: 2f67 6974 6875 622e 636f 6d2f 706c 6f6e  /github.com/plon
-000003a0: 652f 706c 6f6e 652e 6170 702e 7374 616e  e/plone.app.stan
-000003b0: 6461 7264 7469 6c65 732f 6973 7375 6573  dardtiles/issues
-000003c0: 2f31 3030 3e60 5f2e 0a20 205b 6d61 7572  /100>`_..  [maur
-000003d0: 6974 735d 0a0a 2d20 4669 7820 7465 7374  its]..- Fix test
-000003e0: 7320 746f 2072 6573 7065 6374 2042 5335  s to respect BS5
-000003f0: 204d 6172 6b75 7020 6f66 2050 6c6f 6e65   Markup of Plone
-00000400: 2036 2e0a 2020 5b6a 656e 7365 6e73 5d0a   6..  [jensens].
-00000410: 0a2d 2046 6978 206d 656d 6265 7274 6f6f  .- Fix membertoo
-00000420: 6c73 2074 696c 650a 2020 5b61 6769 7461  ls tile.  [agita
-00000430: 746f 725d 0a0a 2d20 4272 6561 6b69 6e67  tor]..- Breaking
-00000440: 3a20 4472 6f70 2063 6f64 6520 6d61 726b  : Drop code mark
-00000450: 6564 2061 7320 6465 7072 6563 6174 6564  ed as deprecated
-00000460: 2066 6f72 2033 2e30 2e0a 2020 5468 6973   for 3.0..  This
-00000470: 2069 6e63 6c75 6465 7320 6060 706c 6f6e   includes ``plon
-00000480: 652e 6170 702e 7374 616e 6461 7264 7469  e.app.standardti
-00000490: 6c65 732e 696d 6167 6560 602e 0a20 2049  les.image``..  I
-000004a0: 6620 616e 796f 6e65 2066 6f72 2061 6e79  f anyone for any
-000004b0: 2072 6561 736f 6e20 6861 7320 7374 696c   reason has stil
-000004c0: 6c20 7468 6573 6520 6c6f 6e67 2064 6570  l these long dep
-000004d0: 7265 6361 7465 6420 7469 6c65 2061 726f  recated tile aro
-000004e0: 756e 642c 2063 7573 746f 6d20 7570 6772  und, custom upgr
-000004f0: 6164 6573 2061 7265 206e 6565 6465 642e  ades are needed.
-00000500: 0a20 205b 6a65 6e73 656e 735d 0a0a 2d20  .  [jensens]..- 
-00000510: 4d61 6e75 616c 2063 6f64 6520 636c 6561  Manual code clea
-00000520: 6e75 702e 0a20 205b 6a65 6e73 656e 735d  nup..  [jensens]
-00000530: 0a0a 2d20 4272 6561 6b69 6e67 3a20 4472  ..- Breaking: Dr
-00000540: 6f70 2053 7570 706f 7274 2066 6f72 2050  op Support for P
-00000550: 7974 686f 6e20 322e 3720 616e 6420 506c  ython 2.7 and Pl
-00000560: 6f6e 6520 352e 0a20 205b 6a65 6e73 656e  one 5..  [jensen
-00000570: 735d 0a0a 2d20 4869 6465 2075 6e69 6e73  s]..- Hide unins
-00000580: 7461 6c6c 2070 726f 6669 6c65 2066 726f  tall profile fro
-00000590: 6d20 696e 7374 616c 6c20 7669 6577 2e0a  m install view..
-000005a0: 2020 5b6a 656e 7365 6e73 5d0a 0a0a 322e    [jensens]...2.
-000005b0: 342e 3020 2832 3032 312d 3033 2d32 3429  4.0 (2021-03-24)
-000005c0: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
-000005d0: 2d2d 2d0a 0a2d 2043 6f6e 7465 6e74 206c  ---..- Content l
-000005e0: 6973 7469 6e67 3a20 416c 6c6f 7720 746f  isting: Allow to
-000005f0: 2075 7365 2063 6f6c 6c65 6374 696f 6e20   use collection 
-00000600: 7175 6572 7920 7061 7261 6d65 7465 7273  query parameters
-00000610: 2066 726f 6d20 636f 6e74 6578 742e 0a20   from context.. 
-00000620: 2043 6f6e 7465 6e74 206c 6973 7469 6e67   Content listing
-00000630: 3a20 496e 636c 7564 6520 7175 6572 7920  : Include query 
-00000640: 7061 7261 6d65 7465 7273 2066 726f 6d20  parameters from 
-00000650: 7265 7175 6573 742e 0a20 2043 6f6e 7465  request..  Conte
-00000660: 6e74 206c 6973 7469 6e67 3a20 4164 6420  nt listing: Add 
-00000670: 2274 696c 655f 636c 6173 7322 2e0a 2020  "tile_class"..  
-00000680: 4261 7463 6869 6e67 2073 7570 706f 7274  Batching support
-00000690: 0a20 2044 726f 7020 7375 7070 6f72 7420  .  Drop support 
-000006a0: 666f 7220 506c 6f6e 6520 352e 302e 7820  for Plone 5.0.x 
-000006b0: 2d20 6e6f 2067 6574 5f74 6f70 5f72 6571  - no get_top_req
-000006c0: 7565 7374 2061 7661 696c 6162 6c65 0a20  uest available. 
-000006d0: 205b 6167 6974 6174 6f72 5d0a 0a2d 2055   [agitator]..- U
-000006e0: 7067 7261 6465 2074 6573 7473 2074 6f20  pgrade tests to 
-000006f0: 6769 7468 7562 2061 6374 696f 6e73 0a20  github actions. 
-00000700: 205b 646a 6179 5d0a 0a2d 2043 4920 7769   [djay]..- CI wi
-00000710: 7468 2047 6974 6875 6220 6163 7469 6f6e  th Github action
-00000720: 733a 2050 7974 686f 6e20 3220 2f20 5079  s: Python 2 / Py
-00000730: 7468 6f6e 2033 2061 6e64 206f 7320 7665  thon 3 and os ve
-00000740: 7273 696f 6e0a 2020 5b6b 7375 6573 735d  rsion.  [ksuess]
-00000750: 0a0a 2d20 7273 7320 7469 6c65 3a20 6578  ..- rss tile: ex
-00000760: 706f 7365 2070 7562 6c69 7368 6564 2064  pose published d
-00000770: 6174 650a 2020 5b6b 7375 6573 735d 0a0a  ate.  [ksuess]..
-00000780: 2d20 7570 6461 7465 206c 696e 6b20 746f  - update link to
-00000790: 2070 6c6f 6e65 2063 6f72 6564 6576 2064   plone coredev d
-000007a0: 6f63 7320 696e 2072 6561 646d 650a 2020  ocs in readme.  
-000007b0: 5b73 7065 7265 7665 7264 655d 0a0a 2d20  [spereverde]..- 
-000007c0: 636f 7665 7261 6c6c 7320 616e 6420 6769  coveralls and gi
-000007d0: 7468 7562 2061 6374 696f 6e73 2077 6f72  thub actions wor
-000007e0: 6b66 6c6f 770a 2020 5b6b 7375 6573 735d  kflow.  [ksuess]
-000007f0: 0a0a 322e 332e 3220 2832 3031 392d 3132  ..2.3.2 (2019-12
-00000800: 2d30 3529 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  -05).-----------
-00000810: 2d2d 2d2d 2d2d 2d0a 0a2d 2041 6464 6564  -------..- Added
-00000820: 2041 6c74 2061 7474 7269 6275 7465 2074   Alt attribute t
-00000830: 6f20 7375 6d6d 6172 7920 7669 6577 2c20  o summary view, 
-00000840: 6e65 6564 6564 2066 6f72 2061 6363 6573  needed for acces
-00000850: 7369 6269 6c69 7479 0a20 205b 726e 756e  sibility.  [rnun
-00000860: 657a 5d0a 0a2d 2050 7933 2066 6978 2066  ez]..- Py3 fix f
-00000870: 6f72 2065 7869 7374 696e 6763 6f6e 7465  or existingconte
-00000880: 6e74 2074 696c 650a 2020 5b70 6574 7363  nt tile.  [petsc
-00000890: 686b 695d 0a0a 2d20 4164 6420 756e 696e  hki]..- Add unin
-000008a0: 7374 616c 6c20 7072 6f66 696c 652e 0a20  stall profile.. 
-000008b0: 205b 6876 656c 6172 6465 5d0a 0a2d 2052   [hvelarde]..- R
-000008c0: 656d 6f76 6520 696e 7374 616c 6c61 7469  emove installati
-000008d0: 6f6e 206f 6620 706c 6f6e 652e 6170 702e  on of plone.app.
-000008e0: 7769 6467 6574 7320 6465 6661 756c 7420  widgets default 
-000008f0: 7072 6f66 696c 6520 696e 2074 6573 7473  profile in tests
-00000900: 2e0a 2020 496e 2050 6c6f 6e65 2035 2e30  ..  In Plone 5.0
-00000910: 2f35 2e31 2077 6974 6820 706c 6f6e 652e  /5.1 with plone.
-00000920: 6170 702e 7769 6467 6574 7320 3e3d 2032  app.widgets >= 2
-00000930: 2e30 2c20 7468 6520 7072 6f66 696c 6520  .0, the profile 
-00000940: 6973 206f 6e6c 7920 6120 6475 6d6d 7920  is only a dummy 
-00000950: 7072 6f66 696c 6520 666f 7220 4242 422e  profile for BBB.
-00000960: 0a20 2049 6e20 506c 6f6e 6520 352e 3220  .  In Plone 5.2 
-00000970: 6974 2077 696c 6c20 6265 2072 656d 6f76  it will be remov
-00000980: 6564 2e0a 2020 5b6a 656e 7365 6e73 5d0a  ed..  [jensens].
-00000990: 0a2d 2053 686f 7720 6576 656e 7420 6465  .- Show event de
-000009a0: 7461 696c 7320 666f 7220 616c 6c20 636f  tails for all co
-000009b0: 6e74 656e 7420 7479 7065 7320 7768 6963  ntent types whic
-000009c0: 6820 7072 6f76 6964 6573 2073 7461 7274  h provides start
-000009d0: 206f 7220 656e 6420 6669 656c 6473 2e0a   or end fields..
-000009e0: 2020 5b4d 7254 616e 676f 5d0a 0a2d 2046    [MrTango]..- F
-000009f0: 6978 2074 6573 7473 2069 6e20 506c 6f6e  ix tests in Plon
-00000a00: 6520 352e 320a 2020 5b4d 7254 616e 676f  e 5.2.  [MrTango
-00000a10: 5d0a 0a2d 2041 6464 2063 7573 746f 6d5f  ]..- Add custom_
-00000a20: 7669 6577 2061 6c73 6f20 696e 2065 7869  view also in exi
-00000a30: 7374 696e 6763 6f6e 7465 6e74 2074 696c  stingcontent til
-00000a40: 652e 0a20 205b 6365 6b6b 5d0a 0a2d 2046  e..  [cekk]..- F
-00000a50: 6978 2065 7869 7374 696e 6763 6f6e 7465  ix existingconte
-00000a60: 6e74 2074 696c 6520 666f 726d 206c 6162  nt tile form lab
-00000a70: 656c 730a 2020 5b70 6e69 636f 6c6c 695d  els.  [pnicolli]
-00000a80: 0a0a 0a32 2e33 2e31 2028 3230 3138 2d30  ...2.3.1 (2018-0
-00000a90: 362d 3037 290a 2d2d 2d2d 2d2d 2d2d 2d2d  6-07).----------
-00000aa0: 2d2d 2d2d 2d2d 2d2d 0a0a 2d20 4669 7820  --------..- Fix 
-00000ab0: 7465 7374 7320 6172 6f75 6e64 2064 6570  tests around dep
-00000ac0: 7265 6361 7465 6420 7261 7720 6874 6d6c  recated raw html
-00000ad0: 2074 696c 6520 616e 6420 7573 6520 6874   tile and use ht
-00000ae0: 6d6c 7469 6c65 2e0a 2020 5b6a 656e 7365  mltile..  [jense
-00000af0: 6e73 5d0a 0a2d 2046 6978 2023 3837 3a20  ns]..- Fix #87: 
-00000b00: 4578 6973 7469 6e67 2043 6f6e 7465 6e74  Existing Content
-00000b10: 2054 696c 6520 6272 6f6b 656e 2077 6865   Tile broken whe
-00000b20: 6e20 7573 6564 2069 6e20 6d75 6c74 696c  n used in multil
-00000b30: 696e 6775 616c 2073 6974 6573 2e0a 2020  ingual sites..  
-00000b40: 5769 6467 6574 2069 7320 6e6f 7720 7369  Widget is now si
-00000b50: 6d69 6c61 7220 746f 2072 656c 6174 6564  milar to related
-00000b60: 2069 7465 6d73 2062 6568 6176 696f 722e   items behavior.
-00000b70: 0a20 205b 6a65 6e73 656e 735d 0a0a 2d20  .  [jensens]..- 
-00000b80: 4669 7820 5469 6c65 436f 6d6d 656e 7446  Fix TileCommentF
-00000b90: 6f72 6d20 746f 2070 7265 6669 7820 666f  orm to prefix fo
-00000ba0: 726d 7320 7769 7468 206a 7573 7420 2766  rms with just 'f
-00000bb0: 6f72 6d27 2074 6f20 6669 7820 636f 6d70  orm' to fix comp
-00000bc0: 6174 6962 696c 6974 790a 2020 7769 7468  atibility.  with
-00000bd0: 2070 6c6f 6e65 2e61 7070 2e64 6973 6375   plone.app.discu
-00000be0: 7373 696f 6e20 6a61 7661 7363 7269 7074  ssion javascript
-00000bf0: 730a 2020 5b64 6174 616b 7572 7265 5d0a  s.  [datakurre].
-00000c00: 0a0a 322e 332e 3020 2832 3031 382d 3034  ..2.3.0 (2018-04
-00000c10: 2d31 3329 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  -13).-----------
-00000c20: 2d2d 2d2d 2d2d 2d0a 0a4e 6577 2066 6561  -------..New fea
-00000c30: 7475 7265 733a 0a0a 2d20 4d6f 7665 6420  tures:..- Moved 
-00000c40: 6465 7065 6e64 656e 6379 206f 6e20 6060  dependency on ``
-00000c50: 706c 6f6e 652e 666f 726d 7769 6467 6574  plone.formwidget
-00000c60: 2e6d 756c 7469 6669 6c65 6060 2075 7365  .multifile`` use
-00000c70: 6420 666f 7220 6465 7072 6563 6174 6564  d for deprecated
-00000c80: 2041 7474 6163 6865 6d65 6e74 2d54 696c   Attachement-Til
-00000c90: 6520 746f 2061 6e20 6578 7472 6120 6060  e to an extra ``
-00000ca0: 6174 7461 6368 6d65 6e74 6060 2069 6e20  attachment`` in 
-00000cb0: 6060 7365 7475 702e 7079 6060 2e0a 2020  ``setup.py``..  
-00000cc0: 5b6a 656e 7365 6e73 5d0a 0a0a 4275 6720  [jensens]...Bug 
-00000cd0: 6669 7865 733a 0a0a 2d20 4669 7820 7465  fixes:..- Fix te
-00000ce0: 7374 7320 6f66 2042 6f6f 6c65 616e 2077  sts of Boolean w
-00000cf0: 6964 6765 743a 0a20 2052 656d 6f76 6520  idget:.  Remove 
-00000d00: 6368 6563 6b73 206f 6620 696d 706c 656d  checks of implem
-00000d10: 656e 7461 7469 6f6e 2064 6574 6169 6c73  entation details
-00000d20: 206f 6620 7468 6520 7769 6467 6574 2e0a   of the widget..
-00000d30: 2020 5468 6973 2064 6f65 7320 6e6f 7420    This does not 
-00000d40: 6265 6c6f 6e67 2069 6e74 6f20 7468 6973  belong into this
-00000d50: 2074 6573 7473 2e0a 2020 4974 2063 6861   tests..  It cha
-00000d60: 6e67 6564 2062 6574 7765 656e 2035 2e30  nged between 5.0
-00000d70: 2061 6e64 2035 2e31 2061 6674 6572 2073   and 5.1 after s
-00000d80: 6f6d 6520 6669 7865 732e 0a20 205b 6a65  ome fixes..  [je
-00000d90: 6e73 656e 735d 0a0a 2d20 4669 7820 6973  nsens]..- Fix is
-00000da0: 7375 6520 2337 392c 0a20 2077 6865 7265  sue #79,.  where
-00000db0: 2061 2074 6573 7420 6661 696c 6564 2077   a test failed w
-00000dc0: 6974 6820 506c 6f6e 6520 352e 312c 2062  ith Plone 5.1, b
-00000dd0: 6563 6175 7365 2061 2074 696c 6520 696e  ecause a tile in
-00000de0: 2061 2074 6573 7420 6861 6420 6e6f 2060   a test had no `
-00000df0: 605f 5f6e 616d 655f 5f60 602e 0a20 205b  `__name__``..  [
-00000e00: 6a65 6e73 656e 735d 0a0a 2d20 4368 616e  jensens]..- Chan
-00000e10: 6765 6420 7469 746c 6520 6f66 2065 7869  ged title of exi
-00000e20: 7374 696e 6720 636f 6e74 656e 7420 7469  sting content ti
-00000e30: 6c65 2066 726f 6d20 6831 2074 6f20 6832  le from h1 to h2
-00000e40: 0a20 205b 6167 6974 6174 6f72 5d0a 0a2d  .  [agitator]..-
-00000e50: 2046 6978 2069 7373 7565 2077 6865 7265   Fix issue where
-00000e60: 2069 6d61 6765 2066 6965 6c64 2074 696c   image field til
-00000e70: 6520 7465 6d70 6c61 7465 2072 6567 6973  e template regis
-00000e80: 7472 6174 696f 6e20 6469 6420 6e6f 7420  tration did not 
-00000e90: 6170 706c 7920 666f 720a 2020 6669 656c  apply for.  fiel
-00000ea0: 6473 206f 6e20 6e6f 6e2d 6465 6661 756c  ds on non-defaul
-00000eb0: 7420 6669 656c 6473 6574 0a20 205b 6461  t fieldset.  [da
-00000ec0: 7461 6b75 7272 655d 0a0a 2d20 496d 706f  takurre]..- Impo
-00000ed0: 7274 7320 6172 6520 5079 7468 6f6e 3320  rts are Python3 
-00000ee0: 636f 6d70 6174 6962 6c65 0a20 205b 6234  compatible.  [b4
-00000ef0: 6f73 6861 6e79 5d0a 0a2d 2046 6978 2069  oshany]..- Fix i
-00000f00: 7373 7565 2077 6865 7265 2066 6965 6c64  ssue where field
-00000f10: 2074 696c 6520 666f 7220 7469 746c 6520   tile for title 
-00000f20: 616e 6420 6465 7363 7269 7074 696f 6e20  and description 
-00000f30: 6669 656c 6473 2072 656e 6465 7265 640a  fields rendered.
-00000f40: 2020 7769 7468 2064 6f75 626c 6520 3c68    with double <h
-00000f50: 746d 6c3e 3c62 6f64 793e 2d77 7261 7070  tml><body>-wrapp
-00000f60: 696e 670a 2020 5b64 6174 616b 7572 7265  ing.  [datakurre
-00000f70: 5d0a 0a32 2e32 2e30 2028 3230 3137 2d30  ]..2.2.0 (2017-0
-00000f80: 362d 3039 290a 2d2d 2d2d 2d2d 2d2d 2d2d  6-09).----------
-00000f90: 2d2d 2d2d 2d2d 2d2d 0a0a 4e65 7720 6665  --------..New fe
-00000fa0: 6174 7572 6573 3a0a 0a2d 2041 6464 2022  atures:..- Add "
-00000fb0: 7368 6f77 5f69 6d61 6765 222c 2022 7368  show_image", "sh
-00000fc0: 6f77 5f74 6578 7422 2c20 2273 686f 775f  ow_text", "show_
-00000fd0: 636f 6d6d 656e 7473 2220 616e 6420 2274  comments" and "t
-00000fe0: 696c 655f 636c 6173 7322 2061 6464 6974  ile_class" addit
-00000ff0: 696f 6e61 6c0a 2020 6669 656c 6473 2074  ional.  fields t
-00001000: 6f20 6578 6973 7469 6e67 2063 6f6e 7465  o existing conte
-00001010: 6e74 2074 696c 652e 0a20 205b 6365 6b6b  nt tile..  [cekk
-00001020: 5d0a 0a42 7567 2066 6978 6573 3a0a 0a2d  ]..Bug fixes:..-
-00001030: 2046 6978 206e 6f6e 2041 5343 4949 2048   Fix non ASCII H
-00001040: 544d 4c20 7469 6c65 2063 6f6e 7465 6e74  TML tile content
-00001050: 0a20 205b 746f 6d67 726f 7373 5d0a 0a2d  .  [tomgross]..-
-00001060: 2041 6464 2062 6574 7465 7220 6465 7363   Add better desc
-00001070: 7269 7074 696f 6e73 2066 6f72 2074 696c  riptions for til
-00001080: 6573 2e0a 2020 5b63 6775 6172 6469 615d  es..  [cguardia]
-00001090: 0a0a 2d20 4669 7820 6e6f 656d 6265 6420  ..- Fix noembed 
-000010a0: 656e 6470 6f69 6e74 2075 726c 2074 6f20  endpoint url to 
-000010b0: 6765 7420 7661 6c69 6420 4a53 4f4e 2072  get valid JSON r
-000010c0: 6573 706f 6e73 652e 0a20 205b 746d 6173  esponse..  [tmas
-000010d0: 736d 616e 5d0a 0a0a 322e 312e 3020 2832  sman]...2.1.0 (2
-000010e0: 3031 372d 3032 2d32 3429 0a2d 2d2d 2d2d  017-02-24).-----
-000010f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a4e  -------------..N
-00001100: 6577 2066 6561 7475 7265 733a 0a0a 2d20  ew features:..- 
-00001110: 4164 6465 6420 7469 746c 6520 616e 6420  Added title and 
-00001120: 6465 7363 7269 7074 696f 6e20 6669 656c  description fiel
-00001130: 6473 2063 6f6e 7465 6e74 206c 6973 7469  ds content listi
-00001140: 6e67 2074 696c 652c 0a20 2077 696c 6c20  ng tile,.  will 
-00001150: 7368 6f77 2075 7020 6f6e 2074 696c 6520  show up on tile 
-00001160: 6966 2066 696c 6c65 6420 696e 2e0a 2020  if filled in..  
-00001170: 5b61 6769 7461 746f 725d 0a0a 2d20 4164  [agitator]..- Ad
-00001180: 6420 706c 6f6e 652e 6170 702e 7374 616e  d plone.app.stan
-00001190: 6461 7264 7469 6c65 732e 6c65 6164 696d  dardtiles.leadim
-000011a0: 6167 6520 666f 7220 7265 6e64 6572 696e  age for renderin
-000011b0: 6720 6c65 6164 2069 6d61 6765 2066 726f  g lead image fro
-000011c0: 6d0a 2020 6c65 6164 2069 6d61 6765 2062  m.  lead image b
-000011d0: 6568 6176 696f 7220 6469 7265 6374 6c79  ehavior directly
-000011e0: 2028 7769 7468 6f75 7420 7669 6577 6c65   (without viewle
-000011f0: 7420 696e 6469 7265 6374 696f 6e29 0a20  t indirection). 
-00001200: 205b 6461 7461 6b75 7272 655d 0a0a 4275   [datakurre]..Bu
-00001210: 6720 6669 7865 733a 0a0a 2d20 4669 7820  g fixes:..- Fix 
-00001220: 7365 7475 7020 6465 7065 6e64 656e 6369  setup dependenci
-00001230: 6573 3a20 646f 206e 6f74 2064 6570 656e  es: do not depen
-00001240: 6420 6f6e 2070 6c6f 6e65 2e61 7070 2e69  d on plone.app.i
-00001250: 6d61 6769 6e67 2c20 6974 2069 7320 6e6f  maging, it is no
-00001260: 7420 6e65 6564 6564 2e0a 2020 5468 6973  t needed..  This
-00001270: 2072 656d 6f76 6573 2061 6e20 7472 616e   removes an tran
-00001280: 7369 656e 7420 6465 7065 6e64 656e 6379  sient dependency
-00001290: 206f 6e20 4172 6368 6574 7970 6573 2e0a   on Archetypes..
-000012a0: 2020 5b6a 656e 7365 6e73 5d0a 0a2d 2046    [jensens]..- F
-000012b0: 6978 2069 7373 7565 7320 7768 6572 6520  ix issues where 
-000012c0: 7469 6c65 7320 6469 646e 2774 2070 726f  tiles didn't pro
-000012d0: 7065 726c 7920 7265 6e64 6572 2077 6865  perly render whe
-000012e0: 6e20 7472 6176 6572 7365 6420 6672 6f6d  n traversed from
-000012f0: 2061 2076 6965 7720 636f 6e74 6578 740a   a view context.
-00001300: 2020 5b64 6174 616b 7572 7265 5d0a 0a2d    [datakurre]..-
-00001310: 204d 696e 6f72 2063 6c65 616e 7570 2069   Minor cleanup i
-00001320: 6e20 636f 6e74 656e 746c 6973 7469 6e67  n contentlisting
-00001330: 2061 6e64 2065 7869 7374 696e 6763 6f6e   and existingcon
-00001340: 7465 6e74 2e0a 2020 5b6a 656e 7365 6e73  tent..  [jensens
-00001350: 5d0a 0a2d 2046 6978 2062 796c 696e 6520  ]..- Fix byline 
-00001360: 7469 6c65 2074 6f20 6261 7365 206f 6e20  tile to base on 
-00001370: 7265 7370 6563 7469 7665 2050 6c6f 6e65  respective Plone
-00001380: 2035 2076 6965 776c 6574 0a20 2028 6275   5 viewlet.  (bu
-00001390: 7420 6e6f 7465 2074 6861 7420 6974 206f  t note that it o
-000013a0: 6e6c 7920 7265 6e64 6572 7320 666f 7220  nly renders for 
-000013b0: 616e 6f6e 796d 6f75 7320 7573 6572 7320  anonymous users 
-000013c0: 7768 656e 2074 6865 7920 6172 6520 616c  when they are al
-000013d0: 6c6f 7765 640a 2020 746f 2076 6965 7720  lowed.  to view 
-000013e0: 6974 290a 2020 5b64 6174 616b 7572 7265  it).  [datakurre
-000013f0: 5d0a 0a2d 2046 6978 2069 7373 7565 2077  ]..- Fix issue w
-00001400: 6865 7265 2076 6965 776c 6574 6d61 6e61  here viewletmana
-00001410: 6765 7273 2077 6572 6520 7265 6e64 6572  gers were render
-00001420: 6564 2069 6e20 7061 7265 6e74 2063 6f6e  ed in parent con
-00001430: 7465 7874 2069 6e73 7465 6164 206f 660a  text instead of.
-00001440: 2020 6f62 6a65 6374 2063 6f6e 7465 7874    object context
-00001450: 0a20 205b 6461 7461 6b75 7272 655d 0a0a  .  [datakurre]..
-00001460: 2d20 4669 7820 7669 6577 6c65 746d 616e  - Fix viewletman
-00001470: 6167 6572 2061 6e64 2070 6f72 746c 6574  ager and portlet
-00001480: 2074 696c 6573 2074 6f20 7265 6e64 6572   tiles to render
-00001490: 206c 696b 6520 6f6e 2064 6566 6175 6c74   like on default
-000014a0: 2076 6965 7773 206f 6e20 4553 490a 2020   views on ESI.  
-000014b0: 7768 656e 2072 656e 6465 7265 6420 6469  when rendered di
-000014c0: 7265 6374 6c79 2061 6761 696e 7374 2063  rectly against c
-000014d0: 6f6e 7465 6e74 6973 6820 636f 6e74 6578  ontentish contex
-000014e0: 7420 2845 5349 2064 6f65 736e 2774 2068  t (ESI doesn't h
-000014f0: 6176 650a 2020 6b6e 6f77 6c65 6467 6520  ave.  knowledge 
-00001500: 6f66 2070 6172 656e 7420 7265 7175 6573  of parent reques
-00001510: 7420 6c69 6b65 2073 7562 7265 7175 6573  t like subreques
-00001520: 7420 6261 7365 6420 636f 6d70 6f73 6974  t based composit
-00001530: 696f 6e20 6861 7329 0a20 205b 6461 7461  ion has).  [data
-00001540: 6b75 7272 655d 0a0a 2d20 4669 7820 6469  kurre]..- Fix di
-00001550: 7363 7573 7369 6f6e 2074 696c 6520 746f  scussion tile to
-00001560: 2070 726f 7065 726c 7920 706f 7374 2074   properly post t
-00001570: 6f20 7469 6c65 2055 524c 2061 6e64 2072  o tile URL and r
-00001580: 6564 6972 6563 7420 746f 2063 6f6e 7465  edirect to conte
-00001590: 7874 2055 524c 3b0a 2020 4164 6420 6578  xt URL;.  Add ex
-000015a0: 706c 6963 6974 2043 5352 462d 7072 6f74  plicit CSRF-prot
-000015b0: 6563 7469 6f6e 2074 6f20 7375 7070 6f72  ection to suppor
-000015c0: 7420 7265 6e64 6572 696e 6720 6173 2045  t rendering as E
-000015d0: 5349 2074 696c 650a 2020 5b64 6174 616b  SI tile.  [datak
-000015e0: 7572 7265 5d0a 0a0a 322e 302e 3020 2832  urre]...2.0.0 (2
-000015f0: 3031 362d 3132 2d31 3329 0a2d 2d2d 2d2d  016-12-13).-----
-00001600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a42  -------------..B
-00001610: 7265 616b 696e 6720 6368 616e 6765 733a  reaking changes:
-00001620: 0a0a 2d20 5265 6d6f 7665 6420 7375 7070  ..- Removed supp
-00001630: 6f72 7420 666f 7220 506c 6f6e 6520 342e  ort for Plone 4.
-00001640: 332e 2046 6f72 2050 6c6f 6e65 2034 2e33  3. For Plone 4.3
-00001650: 2073 7570 706f 7274 2c20 706c 6561 7365   support, please
-00001660: 2075 7365 0a20 2070 6c6f 6e65 2e61 7070   use.  plone.app
-00001670: 2e73 7461 6e64 6172 6474 696c 6573 203c  .standardtiles <
-00001680: 2032 2e30 2e0a 2020 5b64 6174 616b 7572   2.0..  [datakur
-00001690: 7265 2c20 6a65 6e73 656e 732c 2074 6865  re, jensens, the
-000016a0: 745d 0a0a 2d20 5265 6e61 6d65 2072 6177  t]..- Rename raw
-000016b0: 6874 6d6c 2074 6f20 6874 6d6c 2c20 6465  html to html, de
-000016c0: 7072 6563 6174 6520 7261 7768 746d 6c20  precate rawhtml 
-000016d0: 7469 6c65 2061 6e64 206d 616b 6520 6974  tile and make it
-000016e0: 206e 6f72 6d61 6c0a 2020 7469 6c65 2028   normal.  tile (
-000016f0: 6e6f 7420 7065 7273 6973 7465 6420 696e  not persisted in
-00001700: 746f 2061 6e6e 6f74 6174 696f 6e29 0a20  to annotation). 
-00001710: 205b 7661 6e67 6865 656d 5d0a 0a2d 204d   [vangheem]..- M
-00001720: 6172 6b20 6070 6c6f 6e65 2e61 7070 2e73  ark `plone.app.s
-00001730: 7461 6e64 6172 6474 696c 6573 2e69 6d61  tandardtiles.ima
-00001740: 6765 6020 616e 6420 6070 6c6f 6e65 2e61  ge` and `plone.a
-00001750: 7070 2e73 7461 6e64 6172 6474 696c 6573  pp.standardtiles
-00001760: 2e61 7474 6163 686d 656e 7460 0a20 2061  .attachment`.  a
-00001770: 7320 6465 7072 6563 6174 6564 2e0a 2020  s deprecated..  
-00001780: 5b76 616e 6768 6565 6d5d 0a0a 2d20 5265  [vangheem]..- Re
-00001790: 6d6f 7665 2064 6570 7265 6361 7465 6420  move deprecated 
-000017a0: 736b 6970 2d6c 696e 6b73 2074 696c 652c  skip-links tile,
-000017b0: 2062 6563 6175 7365 2074 6865 7265 2773   because there's
-000017c0: 206e 6f20 7375 6368 2076 6965 776c 6574   no such viewlet
-000017d0: 2066 6561 7475 7265 206f 6e0a 2020 506c   feature on.  Pl
-000017e0: 6f6e 6520 350a 2020 5b64 6174 616b 7572  one 5.  [datakur
-000017f0: 7265 5d0a 0a2d 2044 726f 7020 506c 6f6e  re]..- Drop Plon
-00001800: 6520 3420 6661 6c6c 6261 636b 2066 6f72  e 4 fallback for
-00001810: 206c 616e 6775 6167 6520 7365 6c65 6374   language select
-00001820: 6f72 0a20 205b 6a65 6e73 656e 735d 0a0a  or.  [jensens]..
-00001830: 4e65 7720 6665 6174 7572 6573 3a0a 0a2d  New features:..-
-00001840: 2041 6464 6564 2061 206e 6577 2072 6177   Added a new raw
-00001850: 2065 6d62 6564 2074 696c 650a 2020 5b61   embed tile.  [a
-00001860: 6769 7461 746f 725d 0a0a 2d20 5573 6520  gitator]..- Use 
-00001870: 7361 6665 2068 746d 6c20 7472 616e 7366  safe html transf
-00001880: 6f72 6d20 666f 7220 6874 6d6c 2028 7761  orm for html (wa
-00001890: 7320 7261 7729 2074 696c 6520 6f75 7470  s raw) tile outp
-000018a0: 7574 0a20 205b 7661 6e67 6865 656d 5d0a  ut.  [vangheem].
-000018b0: 0a2d 2042 6520 6162 6c65 2074 6f20 7368  .- Be able to sh
-000018c0: 6f77 2f68 6964 6520 7469 746c 652f 6465  ow/hide title/de
-000018d0: 7363 7269 7074 696f 6e20 7769 7468 2065  scription with e
-000018e0: 7869 7374 696e 6720 636f 6e74 656e 7420  xisting content 
-000018f0: 7469 6c65 0a20 205b 7661 6e67 6865 656d  tile.  [vangheem
-00001900: 5d0a 0a42 7567 2066 6978 6573 3a0a 0a2d  ]..Bug fixes:..-
-00001910: 2046 6978 2065 7869 7374 696e 6720 636f   Fix existing co
-00001920: 6e74 656e 7420 7469 6c65 2074 6f20 776f  ntent tile to wo
-00001930: 726b 2077 6974 6820 636f 6c6c 6563 7469  rk with collecti
-00001940: 6f6e 732e 0a20 2054 6869 7320 6669 7865  ons..  This fixe
-00001950: 7320 6874 7470 733a 2f2f 6769 7468 7562  s https://github
-00001960: 2e63 6f6d 2f70 6c6f 6e65 2f70 6c6f 6e65  .com/plone/plone
-00001970: 2e61 7070 2e6d 6f73 6169 632f 6973 7375  .app.mosaic/issu
-00001980: 6573 2f32 3032 0a20 205b 7661 6e67 6865  es/202.  [vanghe
-00001990: 656d 5d0a 0a2d 2056 616c 6964 6174 6520  em]..- Validate 
-000019a0: 7365 6c65 6374 6564 2063 6f6e 7465 6e74  selected content
-000019b0: 2066 6f72 2065 7869 7374 696e 6720 636f   for existing co
-000019c0: 6e74 656e 7420 6973 206e 6f74 2074 6865  ntent is not the
-000019d0: 2063 7572 7265 6e74 2063 6f6e 7465 7874   current context
-000019e0: 0a20 2074 6865 2074 696c 6520 6973 2062  .  the tile is b
-000019f0: 6569 6e67 2072 656e 6465 7265 6420 6167  eing rendered ag
-00001a00: 6169 6e73 742e 0a20 205b 7661 6e67 6865  ainst..  [vanghe
-00001a10: 656d 5d0a 0a2d 2046 6978 2062 6174 6368  em]..- Fix batch
-00001a20: 696e 6720 7572 6c73 206f 6e20 6578 6973  ing urls on exis
-00001a30: 7469 6e67 2063 6f6e 7465 6e74 2074 696c  ting content til
-00001a40: 6573 0a20 205b 7661 6e67 6865 656d 5d0a  es.  [vangheem].
-00001a50: 0a2d 2057 6865 6e20 6361 6c6c 696e 6720  .- When calling 
-00001a60: 6060 4040 706c 6f6e 652e 6170 702e 7374  ``@@plone.app.st
-00001a70: 616e 6461 7264 7469 6c65 732e 636f 6e74  andardtiles.cont
-00001a80: 656e 746c 6973 7469 6e67 6060 2064 6972  entlisting`` dir
-00001a90: 6563 746c 7920 7769 7468 6f75 740a 2020  ectly without.  
-00001aa0: 6861 7669 6e67 2069 7420 636f 6e66 6967  having it config
-00001ab0: 7572 6564 2076 6961 2061 2066 6f72 6d2c  ured via a form,
-00001ac0: 2067 6574 2074 6865 2060 6071 7565 7279   get the ``query
-00001ad0: 6060 2061 6e64 2060 6073 6f72 745f 6f6e  `` and ``sort_on
-00001ae0: 6060 2076 616c 7565 730a 2020 6672 6f6d  `` values.  from
-00001af0: 2069 7427 7320 6465 6661 756c 7420 6661   it's default fa
-00001b00: 6374 6f72 6965 732e 0a20 205b 7468 6574  ctories..  [thet
-00001b10: 5d0a 0a2d 2043 6861 6e67 6520 696e 6974  ]..- Change init
-00001b20: 6961 6c20 6c69 6d69 7420 666f 7220 6c69  ial limit for li
-00001b30: 7374 696e 6720 7469 6c65 2074 6f20 3130  sting tile to 10
-00001b40: 3020 696e 7374 6561 6420 6f66 2031 3030  0 instead of 100
-00001b50: 300a 2020 5b76 616e 6768 6565 6d5d 0a0a  0.  [vangheem]..
-00001b60: 2d20 4861 6e64 6c65 2075 6e69 636f 6465  - Handle unicode
-00001b70: 2065 7272 6f72 2077 6865 6e20 6170 706c   error when appl
-00001b80: 7969 6e67 2066 696c 7465 7273 206f 6e20  ying filters on 
-00001b90: 6874 6d6c 2028 7761 7320 7261 7729 2074  html (was raw) t
-00001ba0: 696c 650a 2020 5b76 616e 6768 6565 6d5d  ile.  [vangheem]
-00001bb0: 0a0a 2d20 5461 6b65 2070 6572 6d69 7373  ..- Take permiss
-00001bc0: 696f 6e73 2061 6e64 2076 6973 6962 696c  ions and visibil
-00001bd0: 6974 7920 6f66 2076 6965 776c 6574 7320  ity of viewlets 
-00001be0: 696e 2074 696c 6573 2069 6e74 6f20 6163  in tiles into ac
-00001bf0: 636f 756e 742e 0a20 205b 6a65 6e73 656e  count..  [jensen
-00001c00: 735d 0a0a 2d20 5265 706c 6163 6520 6d69  s]..- Replace mi
-00001c10: 736c 6561 6469 6e67 2077 6172 6e69 6e67  sleading warning
-00001c20: 7320 6f6e 206d 6973 7369 6e67 2076 6965  s on missing vie
-00001c30: 776c 6574 2074 696c 6573 2077 6974 6820  wlet tiles with 
-00001c40: 7369 6c65 6e74 0a20 2064 6562 7567 206c  silent.  debug l
-00001c50: 6576 656c 206c 6f67 6769 6e67 0a20 205b  evel logging.  [
-00001c60: 6461 7461 6b75 7272 655d 0a0a 2d20 4669  datakurre]..- Fi
-00001c70: 7820 6973 7375 6520 7768 6572 6520 6c61  x issue where la
-00001c80: 796f 7574 2074 696c 6573 2066 6169 6c65  yout tiles faile
-00001c90: 6420 6f6e 2070 6f72 746c 6574 206d 616e  d on portlet man
-00001ca0: 6167 6572 2063 6f6e 7465 7874 0a20 205b  ager context.  [
-00001cb0: 6461 7461 6b75 7272 652c 2061 6769 7461  datakurre, agita
-00001cc0: 746f 725d 0a0a 2d20 4669 7820 6c6f 636b  tor]..- Fix lock
-00001cd0: 696e 666f 2074 6f20 6e6f 7420 6c6f 6720  info to not log 
-00001ce0: 556e 6175 7468 6f72 697a 6564 2d65 7272  Unauthorized-err
-00001cf0: 6f72 7320 6279 2070 726f 7465 6374 696e  ors by protectin
-00001d00: 6720 6974 7320 7265 6769 7374 7261 7469  g its registrati
-00001d10: 6f6e 0a20 206f 6e6c 7920 7769 7468 207a  on.  only with z
-00001d20: 6f70 6532 2e56 6965 772c 2062 7574 2072  ope2.View, but r
-00001d30: 656e 6465 7220 6974 2065 6d70 7479 2077  ender it empty w
-00001d40: 6974 686f 7574 2063 6d66 2e4d 6f64 6966  ithout cmf.Modif
-00001d50: 7950 6f72 7461 6c43 6f6e 7465 6e74 0a20  yPortalContent. 
-00001d60: 205b 6461 7461 6b75 7272 655d 0a0a 2d20   [datakurre]..- 
-00001d70: 4669 7820 706f 7274 6c65 7420 7469 6c65  Fix portlet tile
-00001d80: 2028 6272 6f6b 656e 2062 7920 7265 6772   (broken by regr
-00001d90: 6573 7369 6f6e 290a 2020 5b64 6174 616b  ession).  [datak
-00001da0: 7572 7265 5d0a 0a2d 2046 6978 2069 7373  urre]..- Fix iss
-00001db0: 7565 2077 6865 7265 2065 7869 7374 696e  ue where existin
-00001dc0: 6720 636f 6e74 656e 7420 6469 6420 6e6f  g content did no
-00001dd0: 7420 7265 6e64 6572 206f 6e20 6564 6974  t render on edit
-00001de0: 2066 6f72 6d20 616e 640a 2020 6c6f 6767   form and.  logg
-00001df0: 6564 2065 7272 6f72 2077 6865 6e20 7461  ed error when ta
-00001e00: 7267 6574 2063 6f6e 7465 6e74 206f 626a  rget content obj
-00001e10: 6563 7420 7761 7320 6465 6c65 7465 640a  ect was deleted.
-00001e20: 2020 5b64 6174 616b 7572 7265 5d0a 0a2d    [datakurre]..-
-00001e30: 2046 6978 2072 6563 7572 7369 6f6e 206c   Fix recursion l
-00001e40: 6f6f 7020 696e 2065 7869 7374 696e 6763  oop in existingc
-00001e50: 6f6e 7465 6e74 2074 696c 6520 2823 3438  ontent tile (#48
-00001e60: 290a 2020 5b74 6f6d 6772 6f73 735d 0a0a  ).  [tomgross]..
-00001e70: 5265 6661 6374 6f72 696e 673a 0a0a 2d20  Refactoring:..- 
-00001e80: 4d6f 7665 2074 696c 6520 7265 6769 7374  Move tile regist
-00001e90: 7261 7469 6f6e 7320 6672 6f6d 2060 606d  rations from ``m
-00001ea0: 6564 6961 2e7a 636d 6c60 6020 746f 206d  edia.zcml`` to m
-00001eb0: 6f72 6520 6170 7072 6f70 7269 6174 6520  ore appropriate 
-00001ec0: 706c 6163 6573 3a0a 2020 2d20 6060 6578  places:.  - ``ex
-00001ed0: 6973 7469 6e67 636f 6e74 656e 7460 602c  istingcontent``,
-00001ee0: 2060 6072 7373 6060 2061 6e64 2060 6072   ``rss`` and ``r
-00001ef0: 6177 6874 6d6c 6060 2074 696c 6573 2069  awhtml`` tiles i
-00001f00: 6e74 6f20 6060 636f 6e74 656e 742e 7a63  nto ``content.zc
-00001f10: 6d6c 6060 2c0a 2020 2d20 6060 6e61 7669  ml``,.  - ``navi
-00001f20: 6761 7469 6f6e 6060 2061 6e64 2060 6073  gation`` and ``s
-00001f30: 6974 656d 6170 6060 2074 696c 6573 2069  itemap`` tiles i
-00001f40: 6e20 746f 2060 606c 6179 6f75 742e 7a63  n to ``layout.zc
-00001f50: 6d6c 6060 2e0a 2020 5b74 6865 745d 0a0a  ml``..  [thet]..
-00001f60: 2d20 486f 7573 656b 6565 7069 6e67 2061  - Housekeeping a
-00001f70: 6e64 206d 696e 6f72 2063 6c65 616e 7570  nd minor cleanup
-00001f80: 2e0a 2020 5b6a 656e 7365 6e73 5d0a 0a2d  ..  [jensens]..-
-00001f90: 204d 6f76 6564 204b 6579 776f 7264 5469   Moved KeywordTi
-00001fa0: 6c65 2061 6e64 2054 6162 6c65 4f66 436f  le and TableOfCo
-00001fb0: 6e74 656e 7473 5469 6c65 2074 6f20 636f  ntentsTile to co
-00001fc0: 6d6d 6f6e 2e70 792e 0a20 205b 6a65 6e73  mmon.py..  [jens
-00001fd0: 656e 735d 0a0a 2d20 5369 6d70 6c69 6679  ens]..- Simplify
-00001fe0: 2062 6173 6963 2076 6965 776c 6574 2070   basic viewlet p
-00001ff0: 726f 7879 2074 696c 6573 2e0a 2020 5b6a  roxy tiles..  [j
-00002000: 656e 7365 6e73 5d0a 0a2d 2045 6e61 626c  ensens]..- Enabl
-00002010: 6520 636f 7665 7261 6c6c 7320 616e 6420  e coveralls and 
-00002020: 636f 6465 2061 6e61 6c79 7369 732e 0a20  code analysis.. 
-00002030: 205b 6766 6f72 6361 6461 5d0a 0a2d 2041   [gforcada]..- A
-00002040: 6461 7074 2074 7261 7669 7320 746f 2061  dapt travis to a
-00002050: 6c6c 206f 7468 6572 206d 6f73 6169 6320  ll other mosaic 
-00002060: 7265 616c 7465 6420 7061 636b 6167 6573  realted packages
-00002070: 2e0a 2020 5b67 666f 7263 6164 615d 0a0a  ..  [gforcada]..
-00002080: 2d20 5265 6d6f 7665 2075 6e75 7365 6420  - Remove unused 
-00002090: 6675 6e63 7469 6f6e 2e0a 2020 5b67 666f  function..  [gfo
-000020a0: 7263 6164 615d 0a0a 0a31 2e30 2028 3230  rcada]...1.0 (20
-000020b0: 3136 2d30 342d 3131 290a 2d2d 2d2d 2d2d  16-04-11).------
-000020c0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2d20 4e6f  ----------..- No
-000020d0: 7468 696e 6720 6368 616e 6765 642e 0a0a  thing changed...
-000020e0: 0a31 2e30 6235 2028 3230 3136 2d30 342d  .1.0b5 (2016-04-
-000020f0: 3036 290a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  06).------------
-00002100: 2d2d 2d2d 2d2d 0a0a 2d20 4164 6420 7265  ------..- Add re
-00002110: 6769 7374 7279 2063 6f6e 6669 6775 7261  gistry configura
-00002120: 7469 6f6e 2074 6f20 7370 6563 6966 7920  tion to specify 
-00002130: 6164 6469 7469 6f6e 616c 2063 6f6e 7465  additional conte
-00002140: 6e74 206c 6973 7469 6e67 2076 6965 7773  nt listing views
-00002150: 0a20 205b 7661 6e67 6865 656d 5d0a 0a2d  .  [vangheem]..-
-00002160: 2041 6464 206c 696d 6974 2074 6f20 636f   Add limit to co
-00002170: 6e74 656e 746c 6973 7469 6e67 0a20 205b  ntentlisting.  [
-00002180: 6d61 7274 696f 725d 0a0a 2d20 4669 7820  martior]..- Fix 
-00002190: 656d 6265 6420 7469 6c65 2074 6f20 7261  embed tile to ra
-000021a0: 6d2e 6361 6368 6520 6f65 6d62 6564 2063  m.cache oembed c
-000021b0: 6f64 6520 6279 2055 524c 0a20 205b 6461  ode by URL.  [da
-000021c0: 7461 6b75 7272 655d 0a0a 2d20 4669 7820  takurre]..- Fix 
-000021d0: 7065 726d 6973 7369 6f6e 2064 6566 696e  permission defin
-000021e0: 6974 696f 6e73 2074 6f20 6e6f 7420 7573  itions to not us
-000021f0: 6520 7075 626c 6963 2070 6572 6d69 7373  e public permiss
-00002200: 696f 6e73 2066 6f72 2061 6464 0a20 205b  ions for add.  [
-00002210: 7661 6e67 6865 656d 5d0a 0a2d 2046 6978  vangheem]..- Fix
-00002220: 2045 7665 6e74 2074 6f20 776f 726b 2077   Event to work w
-00002230: 6974 6820 7375 6d6d 6172 795f 7669 6577  ith summary_view
-00002240: 2063 6f6e 7465 6e74 206c 6973 7469 6e67   content listing
-00002250: 2074 696c 650a 2020 5b76 616e 6768 6565   tile.  [vanghee
-00002260: 6d5d 0a0a 2d20 4669 7820 6c69 7374 696e  m]..- Fix listin
-00002270: 6773 206e 6f74 2069 6e63 6c75 6469 6e67  gs not including
-00002280: 202f 7669 6577 206f 6e20 7572 6c73 0a20   /view on urls. 
-00002290: 205b 7661 6e67 6865 656d 5d0a 0a2d 2041   [vangheem]..- A
-000022a0: 6464 2062 6574 7465 7220 6572 726f 7220  dd better error 
-000022b0: 6861 6e64 6c69 6e67 2069 6e20 7375 6d6d  handling in summ
-000022c0: 6172 795f 7669 6577 0a20 205b 7661 6e67  ary_view.  [vang
-000022d0: 6865 656d 5d0a 0a2d 2046 6978 2067 6574  heem]..- Fix get
-000022e0: 7469 6e67 206c 6561 6420 696d 6167 650a  ting lead image.
-000022f0: 2020 5b76 616e 6768 6565 6d5d 0a0a 2d20    [vangheem]..- 
-00002300: 4669 7820 746f 206e 6f74 2074 7261 6e73  Fix to not trans
-00002310: 666f 726d 2072 6177 6874 6d6c 206f 7574  form rawhtml out
-00002320: 7075 7420 6966 2072 656e 6465 7265 6420  put if rendered 
-00002330: 7769 7468 696e 206d 6f73 6169 6320 6c61  within mosaic la
-00002340: 796f 7574 6564 6974 6f72 0a20 205b 7661  youteditor.  [va
-00002350: 6e67 6865 656d 5d0a 0a0a 312e 3062 3420  ngheem]...1.0b4 
-00002360: 2832 3031 352d 3130 2d30 3429 0a2d 2d2d  (2015-10-04).---
-00002370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00002380: 0a2d 2043 6861 6e67 6520 6e61 7669 6761  .- Change naviga
-00002390: 7469 6f6e 2074 696c 6520 746f 206e 6f74  tion tile to not
-000023a0: 2075 7365 2064 6570 7265 6361 7465 6420   use deprecated 
-000023b0: 6465 6661 756c 7473 2066 726f 6d20 706f  defaults from po
-000023c0: 7274 616c 5f70 726f 7065 7274 6965 730a  rtal_properties.
-000023d0: 2020 5b64 6174 616b 7572 7265 5d0a 0a2d    [datakurre]..-
-000023e0: 2041 6464 2073 6f63 6961 6c74 6167 7320   Add socialtags 
-000023f0: 7469 6c65 0a20 205b 7661 6e67 6865 656d  tile.  [vangheem
-00002400: 5d0a 0a2d 2046 6978 2073 6974 656d 6170  ]..- Fix sitemap
-00002410: 2074 696c 6520 746f 2072 6561 6420 636f   tile to read co
-00002420: 7272 6563 7420 7365 7474 696e 6720 6f6e  rrect setting on
-00002430: 2050 6c6f 6e65 2035 0a20 205b 6461 7461   Plone 5.  [data
-00002440: 6b75 7272 655d 0a0a 0a31 2e30 6233 2028  kurre]...1.0b3 (
-00002450: 3230 3135 2d30 392d 3136 290a 2d2d 2d2d  2015-09-16).----
-00002460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-00002470: 2d20 4669 7820 746f 2061 7070 6c79 206f  - Fix to apply o
-00002480: 7574 7075 7420 6669 6c74 6572 7320 666f  utput filters fo
-00002490: 7220 7261 7768 746d 6c20 7469 6c65 0a20  r rawhtml tile. 
-000024a0: 205b 6461 7461 6b75 7272 655d 0a2d 2046   [datakurre].- F
-000024b0: 6978 2065 6e63 6f64 696e 6720 6973 7375  ix encoding issu
-000024c0: 6520 7768 656e 2072 656e 6465 7269 6e67  e when rendering
-000024d0: 2065 7869 7374 696e 6720 636f 6e74 656e   existing conten
-000024e0: 7420 7469 6c65 0a20 205b 6461 7461 6b75  t tile.  [dataku
-000024f0: 7272 655d 0a0a 312e 3062 3220 2832 3031  rre]..1.0b2 (201
-00002500: 352d 3039 2d31 3629 0a2d 2d2d 2d2d 2d2d  5-09-16).-------
-00002510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a2d 2041  -----------..- A
-00002520: 6464 2060 6070 6c6f 6e65 2e61 7070 2e73  dd ``plone.app.s
-00002530: 7461 6e64 6172 6474 696c 6573 2e72 6177  tandardtiles.raw
-00002540: 6874 6d6c 6060 2074 696c 650a 2020 5b76  html`` tile.  [v
-00002550: 616e 6768 6565 6d5d 0a2d 2043 6861 6e67  angheem].- Chang
-00002560: 6520 696d 6167 6520 7469 6c65 2074 6f20  e image tile to 
-00002570: 7573 6520 7261 6469 6f20 7769 6467 6574  use radio widget
-00002580: 2066 6f72 2069 6d61 6765 2073 6361 6c65   for image scale
-00002590: 2073 656c 6563 7469 6f6e 0a20 205b 6461   selection.  [da
-000025a0: 7461 6b75 7272 655d 0a2d 2046 6978 2064  takurre].- Fix d
-000025b0: 6566 6175 6c74 2076 616c 7565 7320 666f  efault values fo
-000025c0: 7220 7265 6e64 6572 696e 6720 7468 6520  r rendering the 
-000025d0: 636f 6e74 656e 7420 6c69 7374 696e 6720  content listing 
-000025e0: 7469 6c65 0a20 205b 7661 6e67 6865 656d  tile.  [vangheem
-000025f0: 5d0a 0a31 2e30 6231 2028 3230 3135 2d30  ]..1.0b1 (2015-0
-00002600: 362d 3038 290a 2d2d 2d2d 2d2d 2d2d 2d2d  6-08).----------
-00002610: 2d2d 2d2d 2d2d 2d2d 0a0a 2d20 4669 7820  --------..- Fix 
-00002620: 6669 656c 6420 7469 6c65 2062 6163 6b77  field tile backw
-00002630: 6172 6473 2063 6f6d 7061 7469 6269 6c69  ards compatibili
-00002640: 7479 2077 6974 6820 706c 6f6e 652e 6170  ty with plone.ap
-00002650: 702e 626c 6f63 6b73 203c 2032 2e31 2e31  p.blocks < 2.1.1
-00002660: 0a20 205b 6461 7461 6b75 7272 655d 0a0a  .  [datakurre]..
-00002670: 312e 3061 3420 2832 3031 352d 3036 2d30  1.0a4 (2015-06-0
-00002680: 3629 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  6).-------------
-00002690: 2d2d 2d2d 2d0a 0a2d 2052 656d 6f76 6520  -----..- Remove 
-000026a0: 7465 7874 2c20 6361 6c65 6e64 6172 2061  text, calendar a
-000026b0: 6e64 2063 6f6e 6669 676c 6574 7320 7469  nd configlets ti
-000026c0: 6c65 730a 2020 5b64 6174 616b 7572 7265  les.  [datakurre
-000026d0: 5d0a 2d20 4164 6420 7363 7269 7074 732c  ].- Add scripts,
-000026e0: 2073 7479 6c65 7368 6565 7473 2061 6e64   stylesheets and
-000026f0: 2074 6f6f 6c62 6172 2074 696c 6573 2066   toolbar tiles f
-00002700: 6f72 2050 6c6f 6e65 2035 0a20 205b 6461  or Plone 5.  [da
-00002710: 7461 6b75 7272 655d 0a2d 2041 6464 2064  takurre].- Add d
-00002720: 7562 6c69 6e63 6f72 6520 6c61 796f 7574  ublincore layout
-00002730: 2074 696c 650a 2020 5b64 6174 616b 7572   tile.  [datakur
-00002740: 7265 5d0a 2d20 4164 6420 7469 746c 6520  re].- Add title 
-00002750: 6669 656c 6420 666f 7220 696d 6167 6520  field for image 
-00002760: 7469 6c65 0a20 205b 6461 7461 6b75 7272  tile.  [datakurr
-00002770: 655d 0a2d 2052 6566 6163 746f 7220 6d6f  e].- Refactor mo
-00002780: 7374 206c 6179 6f75 7420 7469 6c65 7320  st layout tiles 
-00002790: 746f 2072 652d 7573 6520 7669 6577 6c65  to re-use viewle
-000027a0: 7473 2720 666f 7220 7368 6172 6564 2063  ts' for shared c
-000027b0: 6f64 6562 6173 650a 2020 5b64 6174 616b  odebase.  [datak
-000027c0: 7572 7265 5d0a 2d20 4669 7820 6973 7375  urre].- Fix issu
-000027d0: 6520 7768 6572 6520 6279 6c69 6e65 2074  e where byline t
-000027e0: 696c 6520 7761 7320 6272 6f6b 656e 206f  ile was broken o
-000027f0: 6e20 506c 6f6e 6520 350a 2020 5b64 6174  n Plone 5.  [dat
-00002800: 616b 7572 7265 5d0a 2d20 4669 7820 6973  akurre].- Fix is
-00002810: 7375 6520 7768 6572 6520 6669 656c 6420  sue where field 
-00002820: 7469 6c65 2069 676e 6f72 6564 2077 6964  tile ignored wid
-00002830: 6765 7420 6469 7265 6374 6976 650a 2020  get directive.  
-00002840: 5b64 6174 616b 7572 7265 5d0a 2d20 4669  [datakurre].- Fi
-00002850: 7820 7072 6f66 696c 6520 7665 7273 696f  x profile versio
-00002860: 6e20 286e 6f20 7570 6772 6164 6520 7374  n (no upgrade st
-00002870: 6570 3b20 7570 6772 6164 6520 6279 2072  ep; upgrade by r
-00002880: 6569 6e73 7461 6c6c 290a 2020 5b64 6174  einstall).  [dat
-00002890: 616b 7572 7265 5d0a 0a31 2e30 6133 2028  akurre]..1.0a3 (
-000028a0: 3230 3135 2d30 352d 3237 290a 2d2d 2d2d  2015-05-27).----
-000028b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-000028c0: 2d20 4669 7820 696d 706f 7274 2065 7272  - Fix import err
-000028d0: 6f72 206f 6e20 506c 6f6e 6520 3420 7769  or on Plone 4 wi
-000028e0: 7468 6f75 7420 706c 6f6e 652e 6170 702e  thout plone.app.
-000028f0: 636f 6e74 656e 7474 7970 6573 0a20 205b  contenttypes.  [
-00002900: 6461 7461 6b75 7272 655d 0a0a 312e 3061  datakurre]..1.0a
-00002910: 3220 2832 3031 352d 3035 2d32 3729 0a2d  2 (2015-05-27).-
-00002920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002930: 2d0a 0a2d 2046 6978 2069 6d61 6765 2074  -..- Fix image t
-00002940: 696c 6520 746f 206f 6e6c 7920 7365 7420  ile to only set 
-00002950: 696d 6167 6520 7769 6474 6820 746f 2061  image width to a
-00002960: 6c6c 6f77 2070 726f 706f 7274 696f 6e61  llow proportiona
-00002970: 6c20 7363 616c 696e 6720 7769 7468 696e  l scaling within
-00002980: 0a20 2073 6d61 6c6c 6572 2074 6861 6e20  .  smaller than 
-00002990: 7769 6474 6820 636f 6c75 6d6e 730a 2020  width columns.  
-000029a0: 5b64 6174 616b 7572 7265 5d0a 0a31 2e30  [datakurre]..1.0
-000029b0: 6131 2028 3230 3135 2d30 352d 3235 290a  a1 (2015-05-25).
-000029c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000029d0: 2d2d 0a0a 2d20 4669 7273 7420 616c 7068  --..- First alph
-000029e0: 6120 7265 6c65 6173 652e 0a              a release..
+00000010: 3d3d 3d0a 0a33 2e31 2e30 2028 3230 3233  ===..3.1.0 (2023
+00000020: 2d30 352d 3034 290a 2d2d 2d2d 2d2d 2d2d  -05-04).--------
+00000030: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2d20 4164  ----------..- Ad
+00000040: 6420 6f70 7469 6f6e 2074 6f20 656e 6162  d option to enab
+00000050: 6c65 2074 6865 2045 7665 6e74 6c69 7374  le the Eventlist
+00000060: 696e 6720 7669 6577 2028 7468 6973 2065  ing view (this e
+00000070: 7870 616e 6473 2072 6563 7572 7269 6e67  xpands recurring
+00000080: 2065 7665 6e74 7329 2e0a 2020 4e4f 5445   events)..  NOTE
+00000090: 3a20 5468 6520 6c69 7374 696e 6720 7769  : The listing wi
+000000a0: 6c6c 206f 6e6c 7920 7368 6f77 2045 7665  ll only show Eve
+000000b0: 6e74 2074 7970 6573 2e0a 2020 5b70 6574  nt types..  [pet
+000000c0: 7363 686b 695d 0a0a 0a33 2e30 2e31 2028  schki]...3.0.1 (
+000000d0: 3230 3233 2d30 342d 3232 290a 2d2d 2d2d  2023-04-22).----
+000000e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
+000000f0: 2d20 4669 7820 6272 6f6b 656e 2043 4d46  - Fix broken CMF
+00000100: 4479 6e61 6d69 6356 6965 7746 5449 2069  DynamicViewFTI i
+00000110: 6d70 6f72 742e 0a20 205b 7468 6574 5d0a  mport..  [thet].
+00000120: 0a2d 2046 6978 2062 796c 696e 6520 7669  .- Fix byline vi
+00000130: 6577 6c65 7420 6e61 6d65 0a20 205b 6672  ewlet name.  [fr
+00000140: 6170 656c 6c5d 0a0a 0a33 2e30 2e30 2028  apell]...3.0.0 (
+00000150: 3230 3232 2d31 322d 3035 290a 2d2d 2d2d  2022-12-05).----
+00000160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
+00000170: 2d20 4164 6465 6420 6c69 6e6b 696e 7465  - Added linkinte
+00000180: 6772 6974 7920 666f 7220 6874 6d6c 2061  grity for html a
+00000190: 6e64 2065 7869 7374 696e 6763 6f6e 7465  nd existingconte
+000001a0: 6e74 2074 696c 652e 0a20 2043 6f64 6520  nt tile..  Code 
+000001b0: 6973 2070 6f72 7465 6420 666f 726d 2076  is ported form v
+000001c0: 6572 7369 6f6e 2032 2e35 2e30 2c20 616e  ersion 2.5.0, an
+000001d0: 6420 6973 206f 6e6c 7920 6163 7469 7665  d is only active
+000001e0: 2077 6865 6e0a 2020 706c 6f6e 652e 6170   when.  plone.ap
+000001f0: 702e 626c 6f63 6b73 2076 6572 7369 6f6e  p.blocks version
+00000200: 2036 2e30 2e32 206f 7220 6869 6768 6572   6.0.2 or higher
+00000210: 2069 7320 7573 6564 2e0a 2020 5b70 6574   is used..  [pet
+00000220: 7363 686b 695d 0a0a 0a33 2e30 2e30 6231  schki]...3.0.0b1
+00000230: 2028 3230 3232 2d30 362d 3234 290a 2d2d   (2022-06-24).--
+00000240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000250: 2d2d 0a0a 2d20 4669 7820 6060 6973 4465  --..- Fix ``isDe
+00000260: 6661 756c 7450 6167 6560 6020 696d 706f  faultPage`` impo
+00000270: 7274 2077 6869 6368 2077 6173 206d 6f76  rt which was mov
+00000280: 6564 2074 6f20 6060 706c 6f6e 652e 6261  ed to ``plone.ba
+00000290: 7365 2e64 6566 6175 6c74 7061 6765 6060  se.defaultpage``
+000002a0: 0a20 205b 7065 7473 6368 6b69 5d0a 0a2d  .  [petschki]..-
+000002b0: 2043 6c65 616e 7570 2061 6e64 2066 6978   Cleanup and fix
+000002c0: 2045 7869 7374 696e 6743 6f6e 7465 6e74   ExistingContent
+000002d0: 5469 6c65 2069 6e20 352e 320a 2020 5b67  Tile in 5.2.  [g
+000002e0: 6f74 6368 612c 204d 7963 6861 6531 5d0a  otcha, Mychae1].
+000002f0: 0a0a 332e 302e 3061 3220 2832 3032 322d  ..3.0.0a2 (2022-
+00000300: 3034 2d30 3129 0a2d 2d2d 2d2d 2d2d 2d2d  04-01).---------
+00000310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a2d 2046  -----------..- F
+00000320: 6978 6564 204b 6579 4572 726f 7220 6060  ixed KeyError ``
+00000330: 7265 7375 6c74 7360 6020 696e 2074 6162  results`` in tab
+00000340: 756c 6172 2076 6965 772e 2020 5368 6f75  ular view.  Shou
+00000350: 6c64 2068 6176 6520 6265 656e 2060 6062  ld have been ``b
+00000360: 6174 6368 6060 2e0a 2020 4669 7865 7320  atch``..  Fixes 
+00000370: 6069 7373 7565 2031 3232 203c 6874 7470  `issue 122 <http
+00000380: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00000390: 6c6f 6e65 2f70 6c6f 6e65 2e61 7070 2e73  lone/plone.app.s
+000003a0: 7461 6e64 6172 6474 696c 6573 2f69 7373  tandardtiles/iss
+000003b0: 7565 732f 3132 323e 605f 2e0a 2020 5b6d  ues/122>`_..  [m
+000003c0: 6175 7269 7473 5d0a 0a0a 332e 302e 3061  aurits]...3.0.0a
+000003d0: 3120 2832 3032 322d 3033 2d32 3329 0a2d  1 (2022-03-23).-
+000003e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000003f0: 2d2d 2d0a 0a2d 2046 6978 2073 686f 7769  ---..- Fix showi
+00000400: 6e67 2070 7269 7661 7465 2063 6f6e 7465  ng private conte
+00000410: 6e74 2077 6869 6c65 2065 6469 7469 6e67  nt while editing
+00000420: 2061 2074 696c 652e 0a20 2046 6978 6573   a tile..  Fixes
+00000430: 2060 6973 7375 6520 3130 3020 3c68 7474   `issue 100 <htt
+00000440: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000450: 706c 6f6e 652f 706c 6f6e 652e 6170 702e  plone/plone.app.
+00000460: 7374 616e 6461 7264 7469 6c65 732f 6973  standardtiles/is
+00000470: 7375 6573 2f31 3030 3e60 5f2e 0a20 205b  sues/100>`_..  [
+00000480: 6d61 7572 6974 735d 0a0a 2d20 4669 7820  maurits]..- Fix 
+00000490: 7465 7374 7320 746f 2072 6573 7065 6374  tests to respect
+000004a0: 2042 5335 204d 6172 6b75 7020 6f66 2050   BS5 Markup of P
+000004b0: 6c6f 6e65 2036 2e0a 2020 5b6a 656e 7365  lone 6..  [jense
+000004c0: 6e73 5d0a 0a2d 2046 6978 206d 656d 6265  ns]..- Fix membe
+000004d0: 7274 6f6f 6c73 2074 696c 650a 2020 5b61  rtools tile.  [a
+000004e0: 6769 7461 746f 725d 0a0a 2d20 4272 6561  gitator]..- Brea
+000004f0: 6b69 6e67 3a20 4472 6f70 2063 6f64 6520  king: Drop code 
+00000500: 6d61 726b 6564 2061 7320 6465 7072 6563  marked as deprec
+00000510: 6174 6564 2066 6f72 2033 2e30 2e0a 2020  ated for 3.0..  
+00000520: 5468 6973 2069 6e63 6c75 6465 7320 6060  This includes ``
+00000530: 706c 6f6e 652e 6170 702e 7374 616e 6461  plone.app.standa
+00000540: 7264 7469 6c65 732e 696d 6167 6560 602e  rdtiles.image``.
+00000550: 0a20 2049 6620 616e 796f 6e65 2066 6f72  .  If anyone for
+00000560: 2061 6e79 2072 6561 736f 6e20 6861 7320   any reason has 
+00000570: 7374 696c 6c20 7468 6573 6520 6c6f 6e67  still these long
+00000580: 2064 6570 7265 6361 7465 6420 7469 6c65   deprecated tile
+00000590: 2061 726f 756e 642c 2063 7573 746f 6d20   around, custom 
+000005a0: 7570 6772 6164 6573 2061 7265 206e 6565  upgrades are nee
+000005b0: 6465 642e 0a20 205b 6a65 6e73 656e 735d  ded..  [jensens]
+000005c0: 0a0a 2d20 4d61 6e75 616c 2063 6f64 6520  ..- Manual code 
+000005d0: 636c 6561 6e75 702e 0a20 205b 6a65 6e73  cleanup..  [jens
+000005e0: 656e 735d 0a0a 2d20 4272 6561 6b69 6e67  ens]..- Breaking
+000005f0: 3a20 4472 6f70 2053 7570 706f 7274 2066  : Drop Support f
+00000600: 6f72 2050 7974 686f 6e20 322e 3720 616e  or Python 2.7 an
+00000610: 6420 506c 6f6e 6520 352e 0a20 205b 6a65  d Plone 5..  [je
+00000620: 6e73 656e 735d 0a0a 2d20 4869 6465 2075  nsens]..- Hide u
+00000630: 6e69 6e73 7461 6c6c 2070 726f 6669 6c65  ninstall profile
+00000640: 2066 726f 6d20 696e 7374 616c 6c20 7669   from install vi
+00000650: 6577 2e0a 2020 5b6a 656e 7365 6e73 5d0a  ew..  [jensens].
+00000660: 0a0a 322e 342e 3020 2832 3032 312d 3033  ..2.4.0 (2021-03
+00000670: 2d32 3429 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  -24).-----------
+00000680: 2d2d 2d2d 2d2d 2d0a 0a2d 2043 6f6e 7465  -------..- Conte
+00000690: 6e74 206c 6973 7469 6e67 3a20 416c 6c6f  nt listing: Allo
+000006a0: 7720 746f 2075 7365 2063 6f6c 6c65 6374  w to use collect
+000006b0: 696f 6e20 7175 6572 7920 7061 7261 6d65  ion query parame
+000006c0: 7465 7273 2066 726f 6d20 636f 6e74 6578  ters from contex
+000006d0: 742e 0a20 2043 6f6e 7465 6e74 206c 6973  t..  Content lis
+000006e0: 7469 6e67 3a20 496e 636c 7564 6520 7175  ting: Include qu
+000006f0: 6572 7920 7061 7261 6d65 7465 7273 2066  ery parameters f
+00000700: 726f 6d20 7265 7175 6573 742e 0a20 2043  rom request..  C
+00000710: 6f6e 7465 6e74 206c 6973 7469 6e67 3a20  ontent listing: 
+00000720: 4164 6420 2274 696c 655f 636c 6173 7322  Add "tile_class"
+00000730: 2e0a 2020 4261 7463 6869 6e67 2073 7570  ..  Batching sup
+00000740: 706f 7274 0a20 2044 726f 7020 7375 7070  port.  Drop supp
+00000750: 6f72 7420 666f 7220 506c 6f6e 6520 352e  ort for Plone 5.
+00000760: 302e 7820 2d20 6e6f 2067 6574 5f74 6f70  0.x - no get_top
+00000770: 5f72 6571 7565 7374 2061 7661 696c 6162  _request availab
+00000780: 6c65 0a20 205b 6167 6974 6174 6f72 5d0a  le.  [agitator].
+00000790: 0a2d 2055 7067 7261 6465 2074 6573 7473  .- Upgrade tests
+000007a0: 2074 6f20 6769 7468 7562 2061 6374 696f   to github actio
+000007b0: 6e73 0a20 205b 646a 6179 5d0a 0a2d 2043  ns.  [djay]..- C
+000007c0: 4920 7769 7468 2047 6974 6875 6220 6163  I with Github ac
+000007d0: 7469 6f6e 733a 2050 7974 686f 6e20 3220  tions: Python 2 
+000007e0: 2f20 5079 7468 6f6e 2033 2061 6e64 206f  / Python 3 and o
+000007f0: 7320 7665 7273 696f 6e0a 2020 5b6b 7375  s version.  [ksu
+00000800: 6573 735d 0a0a 2d20 7273 7320 7469 6c65  ess]..- rss tile
+00000810: 3a20 6578 706f 7365 2070 7562 6c69 7368  : expose publish
+00000820: 6564 2064 6174 650a 2020 5b6b 7375 6573  ed date.  [ksues
+00000830: 735d 0a0a 2d20 7570 6461 7465 206c 696e  s]..- update lin
+00000840: 6b20 746f 2070 6c6f 6e65 2063 6f72 6564  k to plone cored
+00000850: 6576 2064 6f63 7320 696e 2072 6561 646d  ev docs in readm
+00000860: 650a 2020 5b73 7065 7265 7665 7264 655d  e.  [spereverde]
+00000870: 0a0a 2d20 636f 7665 7261 6c6c 7320 616e  ..- coveralls an
+00000880: 6420 6769 7468 7562 2061 6374 696f 6e73  d github actions
+00000890: 2077 6f72 6b66 6c6f 770a 2020 5b6b 7375   workflow.  [ksu
+000008a0: 6573 735d 0a0a 322e 332e 3220 2832 3031  ess]..2.3.2 (201
+000008b0: 392d 3132 2d30 3529 0a2d 2d2d 2d2d 2d2d  9-12-05).-------
+000008c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a2d 2041  -----------..- A
+000008d0: 6464 6564 2041 6c74 2061 7474 7269 6275  dded Alt attribu
+000008e0: 7465 2074 6f20 7375 6d6d 6172 7920 7669  te to summary vi
+000008f0: 6577 2c20 6e65 6564 6564 2066 6f72 2061  ew, needed for a
+00000900: 6363 6573 7369 6269 6c69 7479 0a20 205b  ccessibility.  [
+00000910: 726e 756e 657a 5d0a 0a2d 2050 7933 2066  rnunez]..- Py3 f
+00000920: 6978 2066 6f72 2065 7869 7374 696e 6763  ix for existingc
+00000930: 6f6e 7465 6e74 2074 696c 650a 2020 5b70  ontent tile.  [p
+00000940: 6574 7363 686b 695d 0a0a 2d20 4164 6420  etschki]..- Add 
+00000950: 756e 696e 7374 616c 6c20 7072 6f66 696c  uninstall profil
+00000960: 652e 0a20 205b 6876 656c 6172 6465 5d0a  e..  [hvelarde].
+00000970: 0a2d 2052 656d 6f76 6520 696e 7374 616c  .- Remove instal
+00000980: 6c61 7469 6f6e 206f 6620 706c 6f6e 652e  lation of plone.
+00000990: 6170 702e 7769 6467 6574 7320 6465 6661  app.widgets defa
+000009a0: 756c 7420 7072 6f66 696c 6520 696e 2074  ult profile in t
+000009b0: 6573 7473 2e0a 2020 496e 2050 6c6f 6e65  ests..  In Plone
+000009c0: 2035 2e30 2f35 2e31 2077 6974 6820 706c   5.0/5.1 with pl
+000009d0: 6f6e 652e 6170 702e 7769 6467 6574 7320  one.app.widgets 
+000009e0: 3e3d 2032 2e30 2c20 7468 6520 7072 6f66  >= 2.0, the prof
+000009f0: 696c 6520 6973 206f 6e6c 7920 6120 6475  ile is only a du
+00000a00: 6d6d 7920 7072 6f66 696c 6520 666f 7220  mmy profile for 
+00000a10: 4242 422e 0a20 2049 6e20 506c 6f6e 6520  BBB..  In Plone 
+00000a20: 352e 3220 6974 2077 696c 6c20 6265 2072  5.2 it will be r
+00000a30: 656d 6f76 6564 2e0a 2020 5b6a 656e 7365  emoved..  [jense
+00000a40: 6e73 5d0a 0a2d 2053 686f 7720 6576 656e  ns]..- Show even
+00000a50: 7420 6465 7461 696c 7320 666f 7220 616c  t details for al
+00000a60: 6c20 636f 6e74 656e 7420 7479 7065 7320  l content types 
+00000a70: 7768 6963 6820 7072 6f76 6964 6573 2073  which provides s
+00000a80: 7461 7274 206f 7220 656e 6420 6669 656c  tart or end fiel
+00000a90: 6473 2e0a 2020 5b4d 7254 616e 676f 5d0a  ds..  [MrTango].
+00000aa0: 0a2d 2046 6978 2074 6573 7473 2069 6e20  .- Fix tests in 
+00000ab0: 506c 6f6e 6520 352e 320a 2020 5b4d 7254  Plone 5.2.  [MrT
+00000ac0: 616e 676f 5d0a 0a2d 2041 6464 2063 7573  ango]..- Add cus
+00000ad0: 746f 6d5f 7669 6577 2061 6c73 6f20 696e  tom_view also in
+00000ae0: 2065 7869 7374 696e 6763 6f6e 7465 6e74   existingcontent
+00000af0: 2074 696c 652e 0a20 205b 6365 6b6b 5d0a   tile..  [cekk].
+00000b00: 0a2d 2046 6978 2065 7869 7374 696e 6763  .- Fix existingc
+00000b10: 6f6e 7465 6e74 2074 696c 6520 666f 726d  ontent tile form
+00000b20: 206c 6162 656c 730a 2020 5b70 6e69 636f   labels.  [pnico
+00000b30: 6c6c 695d 0a0a 0a32 2e33 2e31 2028 3230  lli]...2.3.1 (20
+00000b40: 3138 2d30 362d 3037 290a 2d2d 2d2d 2d2d  18-06-07).------
+00000b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2d20  ------------..- 
+00000b60: 4669 7820 7465 7374 7320 6172 6f75 6e64  Fix tests around
+00000b70: 2064 6570 7265 6361 7465 6420 7261 7720   deprecated raw 
+00000b80: 6874 6d6c 2074 696c 6520 616e 6420 7573  html tile and us
+00000b90: 6520 6874 6d6c 7469 6c65 2e0a 2020 5b6a  e htmltile..  [j
+00000ba0: 656e 7365 6e73 5d0a 0a2d 2046 6978 2023  ensens]..- Fix #
+00000bb0: 3837 3a20 4578 6973 7469 6e67 2043 6f6e  87: Existing Con
+00000bc0: 7465 6e74 2054 696c 6520 6272 6f6b 656e  tent Tile broken
+00000bd0: 2077 6865 6e20 7573 6564 2069 6e20 6d75   when used in mu
+00000be0: 6c74 696c 696e 6775 616c 2073 6974 6573  ltilingual sites
+00000bf0: 2e0a 2020 5769 6467 6574 2069 7320 6e6f  ..  Widget is no
+00000c00: 7720 7369 6d69 6c61 7220 746f 2072 656c  w similar to rel
+00000c10: 6174 6564 2069 7465 6d73 2062 6568 6176  ated items behav
+00000c20: 696f 722e 0a20 205b 6a65 6e73 656e 735d  ior..  [jensens]
+00000c30: 0a0a 2d20 4669 7820 5469 6c65 436f 6d6d  ..- Fix TileComm
+00000c40: 656e 7446 6f72 6d20 746f 2070 7265 6669  entForm to prefi
+00000c50: 7820 666f 726d 7320 7769 7468 206a 7573  x forms with jus
+00000c60: 7420 2766 6f72 6d27 2074 6f20 6669 7820  t 'form' to fix 
+00000c70: 636f 6d70 6174 6962 696c 6974 790a 2020  compatibility.  
+00000c80: 7769 7468 2070 6c6f 6e65 2e61 7070 2e64  with plone.app.d
+00000c90: 6973 6375 7373 696f 6e20 6a61 7661 7363  iscussion javasc
+00000ca0: 7269 7074 730a 2020 5b64 6174 616b 7572  ripts.  [datakur
+00000cb0: 7265 5d0a 0a0a 322e 332e 3020 2832 3031  re]...2.3.0 (201
+00000cc0: 382d 3034 2d31 3329 0a2d 2d2d 2d2d 2d2d  8-04-13).-------
+00000cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a4e 6577  -----------..New
+00000ce0: 2066 6561 7475 7265 733a 0a0a 2d20 4d6f   features:..- Mo
+00000cf0: 7665 6420 6465 7065 6e64 656e 6379 206f  ved dependency o
+00000d00: 6e20 6060 706c 6f6e 652e 666f 726d 7769  n ``plone.formwi
+00000d10: 6467 6574 2e6d 756c 7469 6669 6c65 6060  dget.multifile``
+00000d20: 2075 7365 6420 666f 7220 6465 7072 6563   used for deprec
+00000d30: 6174 6564 2041 7474 6163 6865 6d65 6e74  ated Attachement
+00000d40: 2d54 696c 6520 746f 2061 6e20 6578 7472  -Tile to an extr
+00000d50: 6120 6060 6174 7461 6368 6d65 6e74 6060  a ``attachment``
+00000d60: 2069 6e20 6060 7365 7475 702e 7079 6060   in ``setup.py``
+00000d70: 2e0a 2020 5b6a 656e 7365 6e73 5d0a 0a0a  ..  [jensens]...
+00000d80: 4275 6720 6669 7865 733a 0a0a 2d20 4669  Bug fixes:..- Fi
+00000d90: 7820 7465 7374 7320 6f66 2042 6f6f 6c65  x tests of Boole
+00000da0: 616e 2077 6964 6765 743a 0a20 2052 656d  an widget:.  Rem
+00000db0: 6f76 6520 6368 6563 6b73 206f 6620 696d  ove checks of im
+00000dc0: 706c 656d 656e 7461 7469 6f6e 2064 6574  plementation det
+00000dd0: 6169 6c73 206f 6620 7468 6520 7769 6467  ails of the widg
+00000de0: 6574 2e0a 2020 5468 6973 2064 6f65 7320  et..  This does 
+00000df0: 6e6f 7420 6265 6c6f 6e67 2069 6e74 6f20  not belong into 
+00000e00: 7468 6973 2074 6573 7473 2e0a 2020 4974  this tests..  It
+00000e10: 2063 6861 6e67 6564 2062 6574 7765 656e   changed between
+00000e20: 2035 2e30 2061 6e64 2035 2e31 2061 6674   5.0 and 5.1 aft
+00000e30: 6572 2073 6f6d 6520 6669 7865 732e 0a20  er some fixes.. 
+00000e40: 205b 6a65 6e73 656e 735d 0a0a 2d20 4669   [jensens]..- Fi
+00000e50: 7820 6973 7375 6520 2337 392c 0a20 2077  x issue #79,.  w
+00000e60: 6865 7265 2061 2074 6573 7420 6661 696c  here a test fail
+00000e70: 6564 2077 6974 6820 506c 6f6e 6520 352e  ed with Plone 5.
+00000e80: 312c 2062 6563 6175 7365 2061 2074 696c  1, because a til
+00000e90: 6520 696e 2061 2074 6573 7420 6861 6420  e in a test had 
+00000ea0: 6e6f 2060 605f 5f6e 616d 655f 5f60 602e  no ``__name__``.
+00000eb0: 0a20 205b 6a65 6e73 656e 735d 0a0a 2d20  .  [jensens]..- 
+00000ec0: 4368 616e 6765 6420 7469 746c 6520 6f66  Changed title of
+00000ed0: 2065 7869 7374 696e 6720 636f 6e74 656e   existing conten
+00000ee0: 7420 7469 6c65 2066 726f 6d20 6831 2074  t tile from h1 t
+00000ef0: 6f20 6832 0a20 205b 6167 6974 6174 6f72  o h2.  [agitator
+00000f00: 5d0a 0a2d 2046 6978 2069 7373 7565 2077  ]..- Fix issue w
+00000f10: 6865 7265 2069 6d61 6765 2066 6965 6c64  here image field
+00000f20: 2074 696c 6520 7465 6d70 6c61 7465 2072   tile template r
+00000f30: 6567 6973 7472 6174 696f 6e20 6469 6420  egistration did 
+00000f40: 6e6f 7420 6170 706c 7920 666f 720a 2020  not apply for.  
+00000f50: 6669 656c 6473 206f 6e20 6e6f 6e2d 6465  fields on non-de
+00000f60: 6661 756c 7420 6669 656c 6473 6574 0a20  fault fieldset. 
+00000f70: 205b 6461 7461 6b75 7272 655d 0a0a 2d20   [datakurre]..- 
+00000f80: 496d 706f 7274 7320 6172 6520 5079 7468  Imports are Pyth
+00000f90: 6f6e 3320 636f 6d70 6174 6962 6c65 0a20  on3 compatible. 
+00000fa0: 205b 6234 6f73 6861 6e79 5d0a 0a2d 2046   [b4oshany]..- F
+00000fb0: 6978 2069 7373 7565 2077 6865 7265 2066  ix issue where f
+00000fc0: 6965 6c64 2074 696c 6520 666f 7220 7469  ield tile for ti
+00000fd0: 746c 6520 616e 6420 6465 7363 7269 7074  tle and descript
+00000fe0: 696f 6e20 6669 656c 6473 2072 656e 6465  ion fields rende
+00000ff0: 7265 640a 2020 7769 7468 2064 6f75 626c  red.  with doubl
+00001000: 6520 3c68 746d 6c3e 3c62 6f64 793e 2d77  e <html><body>-w
+00001010: 7261 7070 696e 670a 2020 5b64 6174 616b  rapping.  [datak
+00001020: 7572 7265 5d0a 0a32 2e32 2e30 2028 3230  urre]..2.2.0 (20
+00001030: 3137 2d30 362d 3039 290a 2d2d 2d2d 2d2d  17-06-09).------
+00001040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 4e65  ------------..Ne
+00001050: 7720 6665 6174 7572 6573 3a0a 0a2d 2041  w features:..- A
+00001060: 6464 2022 7368 6f77 5f69 6d61 6765 222c  dd "show_image",
+00001070: 2022 7368 6f77 5f74 6578 7422 2c20 2273   "show_text", "s
+00001080: 686f 775f 636f 6d6d 656e 7473 2220 616e  how_comments" an
+00001090: 6420 2274 696c 655f 636c 6173 7322 2061  d "tile_class" a
+000010a0: 6464 6974 696f 6e61 6c0a 2020 6669 656c  dditional.  fiel
+000010b0: 6473 2074 6f20 6578 6973 7469 6e67 2063  ds to existing c
+000010c0: 6f6e 7465 6e74 2074 696c 652e 0a20 205b  ontent tile..  [
+000010d0: 6365 6b6b 5d0a 0a42 7567 2066 6978 6573  cekk]..Bug fixes
+000010e0: 3a0a 0a2d 2046 6978 206e 6f6e 2041 5343  :..- Fix non ASC
+000010f0: 4949 2048 544d 4c20 7469 6c65 2063 6f6e  II HTML tile con
+00001100: 7465 6e74 0a20 205b 746f 6d67 726f 7373  tent.  [tomgross
+00001110: 5d0a 0a2d 2041 6464 2062 6574 7465 7220  ]..- Add better 
+00001120: 6465 7363 7269 7074 696f 6e73 2066 6f72  descriptions for
+00001130: 2074 696c 6573 2e0a 2020 5b63 6775 6172   tiles..  [cguar
+00001140: 6469 615d 0a0a 2d20 4669 7820 6e6f 656d  dia]..- Fix noem
+00001150: 6265 6420 656e 6470 6f69 6e74 2075 726c  bed endpoint url
+00001160: 2074 6f20 6765 7420 7661 6c69 6420 4a53   to get valid JS
+00001170: 4f4e 2072 6573 706f 6e73 652e 0a20 205b  ON response..  [
+00001180: 746d 6173 736d 616e 5d0a 0a0a 322e 312e  tmassman]...2.1.
+00001190: 3020 2832 3031 372d 3032 2d32 3429 0a2d  0 (2017-02-24).-
+000011a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000011b0: 2d0a 0a4e 6577 2066 6561 7475 7265 733a  -..New features:
+000011c0: 0a0a 2d20 4164 6465 6420 7469 746c 6520  ..- Added title 
+000011d0: 616e 6420 6465 7363 7269 7074 696f 6e20  and description 
+000011e0: 6669 656c 6473 2063 6f6e 7465 6e74 206c  fields content l
+000011f0: 6973 7469 6e67 2074 696c 652c 0a20 2077  isting tile,.  w
+00001200: 696c 6c20 7368 6f77 2075 7020 6f6e 2074  ill show up on t
+00001210: 696c 6520 6966 2066 696c 6c65 6420 696e  ile if filled in
+00001220: 2e0a 2020 5b61 6769 7461 746f 725d 0a0a  ..  [agitator]..
+00001230: 2d20 4164 6420 706c 6f6e 652e 6170 702e  - Add plone.app.
+00001240: 7374 616e 6461 7264 7469 6c65 732e 6c65  standardtiles.le
+00001250: 6164 696d 6167 6520 666f 7220 7265 6e64  adimage for rend
+00001260: 6572 696e 6720 6c65 6164 2069 6d61 6765  ering lead image
+00001270: 2066 726f 6d0a 2020 6c65 6164 2069 6d61   from.  lead ima
+00001280: 6765 2062 6568 6176 696f 7220 6469 7265  ge behavior dire
+00001290: 6374 6c79 2028 7769 7468 6f75 7420 7669  ctly (without vi
+000012a0: 6577 6c65 7420 696e 6469 7265 6374 696f  ewlet indirectio
+000012b0: 6e29 0a20 205b 6461 7461 6b75 7272 655d  n).  [datakurre]
+000012c0: 0a0a 4275 6720 6669 7865 733a 0a0a 2d20  ..Bug fixes:..- 
+000012d0: 4669 7820 7365 7475 7020 6465 7065 6e64  Fix setup depend
+000012e0: 656e 6369 6573 3a20 646f 206e 6f74 2064  encies: do not d
+000012f0: 6570 656e 6420 6f6e 2070 6c6f 6e65 2e61  epend on plone.a
+00001300: 7070 2e69 6d61 6769 6e67 2c20 6974 2069  pp.imaging, it i
+00001310: 7320 6e6f 7420 6e65 6564 6564 2e0a 2020  s not needed..  
+00001320: 5468 6973 2072 656d 6f76 6573 2061 6e20  This removes an 
+00001330: 7472 616e 7369 656e 7420 6465 7065 6e64  transient depend
+00001340: 656e 6379 206f 6e20 4172 6368 6574 7970  ency on Archetyp
+00001350: 6573 2e0a 2020 5b6a 656e 7365 6e73 5d0a  es..  [jensens].
+00001360: 0a2d 2046 6978 2069 7373 7565 7320 7768  .- Fix issues wh
+00001370: 6572 6520 7469 6c65 7320 6469 646e 2774  ere tiles didn't
+00001380: 2070 726f 7065 726c 7920 7265 6e64 6572   properly render
+00001390: 2077 6865 6e20 7472 6176 6572 7365 6420   when traversed 
+000013a0: 6672 6f6d 2061 2076 6965 7720 636f 6e74  from a view cont
+000013b0: 6578 740a 2020 5b64 6174 616b 7572 7265  ext.  [datakurre
+000013c0: 5d0a 0a2d 204d 696e 6f72 2063 6c65 616e  ]..- Minor clean
+000013d0: 7570 2069 6e20 636f 6e74 656e 746c 6973  up in contentlis
+000013e0: 7469 6e67 2061 6e64 2065 7869 7374 696e  ting and existin
+000013f0: 6763 6f6e 7465 6e74 2e0a 2020 5b6a 656e  gcontent..  [jen
+00001400: 7365 6e73 5d0a 0a2d 2046 6978 2062 796c  sens]..- Fix byl
+00001410: 696e 6520 7469 6c65 2074 6f20 6261 7365  ine tile to base
+00001420: 206f 6e20 7265 7370 6563 7469 7665 2050   on respective P
+00001430: 6c6f 6e65 2035 2076 6965 776c 6574 0a20  lone 5 viewlet. 
+00001440: 2028 6275 7420 6e6f 7465 2074 6861 7420   (but note that 
+00001450: 6974 206f 6e6c 7920 7265 6e64 6572 7320  it only renders 
+00001460: 666f 7220 616e 6f6e 796d 6f75 7320 7573  for anonymous us
+00001470: 6572 7320 7768 656e 2074 6865 7920 6172  ers when they ar
+00001480: 6520 616c 6c6f 7765 640a 2020 746f 2076  e allowed.  to v
+00001490: 6965 7720 6974 290a 2020 5b64 6174 616b  iew it).  [datak
+000014a0: 7572 7265 5d0a 0a2d 2046 6978 2069 7373  urre]..- Fix iss
+000014b0: 7565 2077 6865 7265 2076 6965 776c 6574  ue where viewlet
+000014c0: 6d61 6e61 6765 7273 2077 6572 6520 7265  managers were re
+000014d0: 6e64 6572 6564 2069 6e20 7061 7265 6e74  ndered in parent
+000014e0: 2063 6f6e 7465 7874 2069 6e73 7465 6164   context instead
+000014f0: 206f 660a 2020 6f62 6a65 6374 2063 6f6e   of.  object con
+00001500: 7465 7874 0a20 205b 6461 7461 6b75 7272  text.  [datakurr
+00001510: 655d 0a0a 2d20 4669 7820 7669 6577 6c65  e]..- Fix viewle
+00001520: 746d 616e 6167 6572 2061 6e64 2070 6f72  tmanager and por
+00001530: 746c 6574 2074 696c 6573 2074 6f20 7265  tlet tiles to re
+00001540: 6e64 6572 206c 696b 6520 6f6e 2064 6566  nder like on def
+00001550: 6175 6c74 2076 6965 7773 206f 6e20 4553  ault views on ES
+00001560: 490a 2020 7768 656e 2072 656e 6465 7265  I.  when rendere
+00001570: 6420 6469 7265 6374 6c79 2061 6761 696e  d directly again
+00001580: 7374 2063 6f6e 7465 6e74 6973 6820 636f  st contentish co
+00001590: 6e74 6578 7420 2845 5349 2064 6f65 736e  ntext (ESI doesn
+000015a0: 2774 2068 6176 650a 2020 6b6e 6f77 6c65  't have.  knowle
+000015b0: 6467 6520 6f66 2070 6172 656e 7420 7265  dge of parent re
+000015c0: 7175 6573 7420 6c69 6b65 2073 7562 7265  quest like subre
+000015d0: 7175 6573 7420 6261 7365 6420 636f 6d70  quest based comp
+000015e0: 6f73 6974 696f 6e20 6861 7329 0a20 205b  osition has).  [
+000015f0: 6461 7461 6b75 7272 655d 0a0a 2d20 4669  datakurre]..- Fi
+00001600: 7820 6469 7363 7573 7369 6f6e 2074 696c  x discussion til
+00001610: 6520 746f 2070 726f 7065 726c 7920 706f  e to properly po
+00001620: 7374 2074 6f20 7469 6c65 2055 524c 2061  st to tile URL a
+00001630: 6e64 2072 6564 6972 6563 7420 746f 2063  nd redirect to c
+00001640: 6f6e 7465 7874 2055 524c 3b0a 2020 4164  ontext URL;.  Ad
+00001650: 6420 6578 706c 6963 6974 2043 5352 462d  d explicit CSRF-
+00001660: 7072 6f74 6563 7469 6f6e 2074 6f20 7375  protection to su
+00001670: 7070 6f72 7420 7265 6e64 6572 696e 6720  pport rendering 
+00001680: 6173 2045 5349 2074 696c 650a 2020 5b64  as ESI tile.  [d
+00001690: 6174 616b 7572 7265 5d0a 0a0a 322e 302e  atakurre]...2.0.
+000016a0: 3020 2832 3031 362d 3132 2d31 3329 0a2d  0 (2016-12-13).-
+000016b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016c0: 2d0a 0a42 7265 616b 696e 6720 6368 616e  -..Breaking chan
+000016d0: 6765 733a 0a0a 2d20 5265 6d6f 7665 6420  ges:..- Removed 
+000016e0: 7375 7070 6f72 7420 666f 7220 506c 6f6e  support for Plon
+000016f0: 6520 342e 332e 2046 6f72 2050 6c6f 6e65  e 4.3. For Plone
+00001700: 2034 2e33 2073 7570 706f 7274 2c20 706c   4.3 support, pl
+00001710: 6561 7365 2075 7365 0a20 2070 6c6f 6e65  ease use.  plone
+00001720: 2e61 7070 2e73 7461 6e64 6172 6474 696c  .app.standardtil
+00001730: 6573 203c 2032 2e30 2e0a 2020 5b64 6174  es < 2.0..  [dat
+00001740: 616b 7572 7265 2c20 6a65 6e73 656e 732c  akurre, jensens,
+00001750: 2074 6865 745d 0a0a 2d20 5265 6e61 6d65   thet]..- Rename
+00001760: 2072 6177 6874 6d6c 2074 6f20 6874 6d6c   rawhtml to html
+00001770: 2c20 6465 7072 6563 6174 6520 7261 7768  , deprecate rawh
+00001780: 746d 6c20 7469 6c65 2061 6e64 206d 616b  tml tile and mak
+00001790: 6520 6974 206e 6f72 6d61 6c0a 2020 7469  e it normal.  ti
+000017a0: 6c65 2028 6e6f 7420 7065 7273 6973 7465  le (not persiste
+000017b0: 6420 696e 746f 2061 6e6e 6f74 6174 696f  d into annotatio
+000017c0: 6e29 0a20 205b 7661 6e67 6865 656d 5d0a  n).  [vangheem].
+000017d0: 0a2d 204d 6172 6b20 6070 6c6f 6e65 2e61  .- Mark `plone.a
+000017e0: 7070 2e73 7461 6e64 6172 6474 696c 6573  pp.standardtiles
+000017f0: 2e69 6d61 6765 6020 616e 6420 6070 6c6f  .image` and `plo
+00001800: 6e65 2e61 7070 2e73 7461 6e64 6172 6474  ne.app.standardt
+00001810: 696c 6573 2e61 7474 6163 686d 656e 7460  iles.attachment`
+00001820: 0a20 2061 7320 6465 7072 6563 6174 6564  .  as deprecated
+00001830: 2e0a 2020 5b76 616e 6768 6565 6d5d 0a0a  ..  [vangheem]..
+00001840: 2d20 5265 6d6f 7665 2064 6570 7265 6361  - Remove depreca
+00001850: 7465 6420 736b 6970 2d6c 696e 6b73 2074  ted skip-links t
+00001860: 696c 652c 2062 6563 6175 7365 2074 6865  ile, because the
+00001870: 7265 2773 206e 6f20 7375 6368 2076 6965  re's no such vie
+00001880: 776c 6574 2066 6561 7475 7265 206f 6e0a  wlet feature on.
+00001890: 2020 506c 6f6e 6520 350a 2020 5b64 6174    Plone 5.  [dat
+000018a0: 616b 7572 7265 5d0a 0a2d 2044 726f 7020  akurre]..- Drop 
+000018b0: 506c 6f6e 6520 3420 6661 6c6c 6261 636b  Plone 4 fallback
+000018c0: 2066 6f72 206c 616e 6775 6167 6520 7365   for language se
+000018d0: 6c65 6374 6f72 0a20 205b 6a65 6e73 656e  lector.  [jensen
+000018e0: 735d 0a0a 4e65 7720 6665 6174 7572 6573  s]..New features
+000018f0: 3a0a 0a2d 2041 6464 6564 2061 206e 6577  :..- Added a new
+00001900: 2072 6177 2065 6d62 6564 2074 696c 650a   raw embed tile.
+00001910: 2020 5b61 6769 7461 746f 725d 0a0a 2d20    [agitator]..- 
+00001920: 5573 6520 7361 6665 2068 746d 6c20 7472  Use safe html tr
+00001930: 616e 7366 6f72 6d20 666f 7220 6874 6d6c  ansform for html
+00001940: 2028 7761 7320 7261 7729 2074 696c 6520   (was raw) tile 
+00001950: 6f75 7470 7574 0a20 205b 7661 6e67 6865  output.  [vanghe
+00001960: 656d 5d0a 0a2d 2042 6520 6162 6c65 2074  em]..- Be able t
+00001970: 6f20 7368 6f77 2f68 6964 6520 7469 746c  o show/hide titl
+00001980: 652f 6465 7363 7269 7074 696f 6e20 7769  e/description wi
+00001990: 7468 2065 7869 7374 696e 6720 636f 6e74  th existing cont
+000019a0: 656e 7420 7469 6c65 0a20 205b 7661 6e67  ent tile.  [vang
+000019b0: 6865 656d 5d0a 0a42 7567 2066 6978 6573  heem]..Bug fixes
+000019c0: 3a0a 0a2d 2046 6978 2065 7869 7374 696e  :..- Fix existin
+000019d0: 6720 636f 6e74 656e 7420 7469 6c65 2074  g content tile t
+000019e0: 6f20 776f 726b 2077 6974 6820 636f 6c6c  o work with coll
+000019f0: 6563 7469 6f6e 732e 0a20 2054 6869 7320  ections..  This 
+00001a00: 6669 7865 7320 6874 7470 733a 2f2f 6769  fixes https://gi
+00001a10: 7468 7562 2e63 6f6d 2f70 6c6f 6e65 2f70  thub.com/plone/p
+00001a20: 6c6f 6e65 2e61 7070 2e6d 6f73 6169 632f  lone.app.mosaic/
+00001a30: 6973 7375 6573 2f32 3032 0a20 205b 7661  issues/202.  [va
+00001a40: 6e67 6865 656d 5d0a 0a2d 2056 616c 6964  ngheem]..- Valid
+00001a50: 6174 6520 7365 6c65 6374 6564 2063 6f6e  ate selected con
+00001a60: 7465 6e74 2066 6f72 2065 7869 7374 696e  tent for existin
+00001a70: 6720 636f 6e74 656e 7420 6973 206e 6f74  g content is not
+00001a80: 2074 6865 2063 7572 7265 6e74 2063 6f6e   the current con
+00001a90: 7465 7874 0a20 2074 6865 2074 696c 6520  text.  the tile 
+00001aa0: 6973 2062 6569 6e67 2072 656e 6465 7265  is being rendere
+00001ab0: 6420 6167 6169 6e73 742e 0a20 205b 7661  d against..  [va
+00001ac0: 6e67 6865 656d 5d0a 0a2d 2046 6978 2062  ngheem]..- Fix b
+00001ad0: 6174 6368 696e 6720 7572 6c73 206f 6e20  atching urls on 
+00001ae0: 6578 6973 7469 6e67 2063 6f6e 7465 6e74  existing content
+00001af0: 2074 696c 6573 0a20 205b 7661 6e67 6865   tiles.  [vanghe
+00001b00: 656d 5d0a 0a2d 2057 6865 6e20 6361 6c6c  em]..- When call
+00001b10: 696e 6720 6060 4040 706c 6f6e 652e 6170  ing ``@@plone.ap
+00001b20: 702e 7374 616e 6461 7264 7469 6c65 732e  p.standardtiles.
+00001b30: 636f 6e74 656e 746c 6973 7469 6e67 6060  contentlisting``
+00001b40: 2064 6972 6563 746c 7920 7769 7468 6f75   directly withou
+00001b50: 740a 2020 6861 7669 6e67 2069 7420 636f  t.  having it co
+00001b60: 6e66 6967 7572 6564 2076 6961 2061 2066  nfigured via a f
+00001b70: 6f72 6d2c 2067 6574 2074 6865 2060 6071  orm, get the ``q
+00001b80: 7565 7279 6060 2061 6e64 2060 6073 6f72  uery`` and ``sor
+00001b90: 745f 6f6e 6060 2076 616c 7565 730a 2020  t_on`` values.  
+00001ba0: 6672 6f6d 2069 7427 7320 6465 6661 756c  from it's defaul
+00001bb0: 7420 6661 6374 6f72 6965 732e 0a20 205b  t factories..  [
+00001bc0: 7468 6574 5d0a 0a2d 2043 6861 6e67 6520  thet]..- Change 
+00001bd0: 696e 6974 6961 6c20 6c69 6d69 7420 666f  initial limit fo
+00001be0: 7220 6c69 7374 696e 6720 7469 6c65 2074  r listing tile t
+00001bf0: 6f20 3130 3020 696e 7374 6561 6420 6f66  o 100 instead of
+00001c00: 2031 3030 300a 2020 5b76 616e 6768 6565   1000.  [vanghee
+00001c10: 6d5d 0a0a 2d20 4861 6e64 6c65 2075 6e69  m]..- Handle uni
+00001c20: 636f 6465 2065 7272 6f72 2077 6865 6e20  code error when 
+00001c30: 6170 706c 7969 6e67 2066 696c 7465 7273  applying filters
+00001c40: 206f 6e20 6874 6d6c 2028 7761 7320 7261   on html (was ra
+00001c50: 7729 2074 696c 650a 2020 5b76 616e 6768  w) tile.  [vangh
+00001c60: 6565 6d5d 0a0a 2d20 5461 6b65 2070 6572  eem]..- Take per
+00001c70: 6d69 7373 696f 6e73 2061 6e64 2076 6973  missions and vis
+00001c80: 6962 696c 6974 7920 6f66 2076 6965 776c  ibility of viewl
+00001c90: 6574 7320 696e 2074 696c 6573 2069 6e74  ets in tiles int
+00001ca0: 6f20 6163 636f 756e 742e 0a20 205b 6a65  o account..  [je
+00001cb0: 6e73 656e 735d 0a0a 2d20 5265 706c 6163  nsens]..- Replac
+00001cc0: 6520 6d69 736c 6561 6469 6e67 2077 6172  e misleading war
+00001cd0: 6e69 6e67 7320 6f6e 206d 6973 7369 6e67  nings on missing
+00001ce0: 2076 6965 776c 6574 2074 696c 6573 2077   viewlet tiles w
+00001cf0: 6974 6820 7369 6c65 6e74 0a20 2064 6562  ith silent.  deb
+00001d00: 7567 206c 6576 656c 206c 6f67 6769 6e67  ug level logging
+00001d10: 0a20 205b 6461 7461 6b75 7272 655d 0a0a  .  [datakurre]..
+00001d20: 2d20 4669 7820 6973 7375 6520 7768 6572  - Fix issue wher
+00001d30: 6520 6c61 796f 7574 2074 696c 6573 2066  e layout tiles f
+00001d40: 6169 6c65 6420 6f6e 2070 6f72 746c 6574  ailed on portlet
+00001d50: 206d 616e 6167 6572 2063 6f6e 7465 7874   manager context
+00001d60: 0a20 205b 6461 7461 6b75 7272 652c 2061  .  [datakurre, a
+00001d70: 6769 7461 746f 725d 0a0a 2d20 4669 7820  gitator]..- Fix 
+00001d80: 6c6f 636b 696e 666f 2074 6f20 6e6f 7420  lockinfo to not 
+00001d90: 6c6f 6720 556e 6175 7468 6f72 697a 6564  log Unauthorized
+00001da0: 2d65 7272 6f72 7320 6279 2070 726f 7465  -errors by prote
+00001db0: 6374 696e 6720 6974 7320 7265 6769 7374  cting its regist
+00001dc0: 7261 7469 6f6e 0a20 206f 6e6c 7920 7769  ration.  only wi
+00001dd0: 7468 207a 6f70 6532 2e56 6965 772c 2062  th zope2.View, b
+00001de0: 7574 2072 656e 6465 7220 6974 2065 6d70  ut render it emp
+00001df0: 7479 2077 6974 686f 7574 2063 6d66 2e4d  ty without cmf.M
+00001e00: 6f64 6966 7950 6f72 7461 6c43 6f6e 7465  odifyPortalConte
+00001e10: 6e74 0a20 205b 6461 7461 6b75 7272 655d  nt.  [datakurre]
+00001e20: 0a0a 2d20 4669 7820 706f 7274 6c65 7420  ..- Fix portlet 
+00001e30: 7469 6c65 2028 6272 6f6b 656e 2062 7920  tile (broken by 
+00001e40: 7265 6772 6573 7369 6f6e 290a 2020 5b64  regression).  [d
+00001e50: 6174 616b 7572 7265 5d0a 0a2d 2046 6978  atakurre]..- Fix
+00001e60: 2069 7373 7565 2077 6865 7265 2065 7869   issue where exi
+00001e70: 7374 696e 6720 636f 6e74 656e 7420 6469  sting content di
+00001e80: 6420 6e6f 7420 7265 6e64 6572 206f 6e20  d not render on 
+00001e90: 6564 6974 2066 6f72 6d20 616e 640a 2020  edit form and.  
+00001ea0: 6c6f 6767 6564 2065 7272 6f72 2077 6865  logged error whe
+00001eb0: 6e20 7461 7267 6574 2063 6f6e 7465 6e74  n target content
+00001ec0: 206f 626a 6563 7420 7761 7320 6465 6c65   object was dele
+00001ed0: 7465 640a 2020 5b64 6174 616b 7572 7265  ted.  [datakurre
+00001ee0: 5d0a 0a2d 2046 6978 2072 6563 7572 7369  ]..- Fix recursi
+00001ef0: 6f6e 206c 6f6f 7020 696e 2065 7869 7374  on loop in exist
+00001f00: 696e 6763 6f6e 7465 6e74 2074 696c 6520  ingcontent tile 
+00001f10: 2823 3438 290a 2020 5b74 6f6d 6772 6f73  (#48).  [tomgros
+00001f20: 735d 0a0a 5265 6661 6374 6f72 696e 673a  s]..Refactoring:
+00001f30: 0a0a 2d20 4d6f 7665 2074 696c 6520 7265  ..- Move tile re
+00001f40: 6769 7374 7261 7469 6f6e 7320 6672 6f6d  gistrations from
+00001f50: 2060 606d 6564 6961 2e7a 636d 6c60 6020   ``media.zcml`` 
+00001f60: 746f 206d 6f72 6520 6170 7072 6f70 7269  to more appropri
+00001f70: 6174 6520 706c 6163 6573 3a0a 2020 2d20  ate places:.  - 
+00001f80: 6060 6578 6973 7469 6e67 636f 6e74 656e  ``existingconten
+00001f90: 7460 602c 2060 6072 7373 6060 2061 6e64  t``, ``rss`` and
+00001fa0: 2060 6072 6177 6874 6d6c 6060 2074 696c   ``rawhtml`` til
+00001fb0: 6573 2069 6e74 6f20 6060 636f 6e74 656e  es into ``conten
+00001fc0: 742e 7a63 6d6c 6060 2c0a 2020 2d20 6060  t.zcml``,.  - ``
+00001fd0: 6e61 7669 6761 7469 6f6e 6060 2061 6e64  navigation`` and
+00001fe0: 2060 6073 6974 656d 6170 6060 2074 696c   ``sitemap`` til
+00001ff0: 6573 2069 6e20 746f 2060 606c 6179 6f75  es in to ``layou
+00002000: 742e 7a63 6d6c 6060 2e0a 2020 5b74 6865  t.zcml``..  [the
+00002010: 745d 0a0a 2d20 486f 7573 656b 6565 7069  t]..- Housekeepi
+00002020: 6e67 2061 6e64 206d 696e 6f72 2063 6c65  ng and minor cle
+00002030: 616e 7570 2e0a 2020 5b6a 656e 7365 6e73  anup..  [jensens
+00002040: 5d0a 0a2d 204d 6f76 6564 204b 6579 776f  ]..- Moved Keywo
+00002050: 7264 5469 6c65 2061 6e64 2054 6162 6c65  rdTile and Table
+00002060: 4f66 436f 6e74 656e 7473 5469 6c65 2074  OfContentsTile t
+00002070: 6f20 636f 6d6d 6f6e 2e70 792e 0a20 205b  o common.py..  [
+00002080: 6a65 6e73 656e 735d 0a0a 2d20 5369 6d70  jensens]..- Simp
+00002090: 6c69 6679 2062 6173 6963 2076 6965 776c  lify basic viewl
+000020a0: 6574 2070 726f 7879 2074 696c 6573 2e0a  et proxy tiles..
+000020b0: 2020 5b6a 656e 7365 6e73 5d0a 0a2d 2045    [jensens]..- E
+000020c0: 6e61 626c 6520 636f 7665 7261 6c6c 7320  nable coveralls 
+000020d0: 616e 6420 636f 6465 2061 6e61 6c79 7369  and code analysi
+000020e0: 732e 0a20 205b 6766 6f72 6361 6461 5d0a  s..  [gforcada].
+000020f0: 0a2d 2041 6461 7074 2074 7261 7669 7320  .- Adapt travis 
+00002100: 746f 2061 6c6c 206f 7468 6572 206d 6f73  to all other mos
+00002110: 6169 6320 7265 616c 7465 6420 7061 636b  aic realted pack
+00002120: 6167 6573 2e0a 2020 5b67 666f 7263 6164  ages..  [gforcad
+00002130: 615d 0a0a 2d20 5265 6d6f 7665 2075 6e75  a]..- Remove unu
+00002140: 7365 6420 6675 6e63 7469 6f6e 2e0a 2020  sed function..  
+00002150: 5b67 666f 7263 6164 615d 0a0a 0a31 2e30  [gforcada]...1.0
+00002160: 2028 3230 3136 2d30 342d 3131 290a 2d2d   (2016-04-11).--
+00002170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
+00002180: 2d20 4e6f 7468 696e 6720 6368 616e 6765  - Nothing change
+00002190: 642e 0a0a 0a31 2e30 6235 2028 3230 3136  d....1.0b5 (2016
+000021a0: 2d30 342d 3036 290a 2d2d 2d2d 2d2d 2d2d  -04-06).--------
+000021b0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2d20 4164  ----------..- Ad
+000021c0: 6420 7265 6769 7374 7279 2063 6f6e 6669  d registry confi
+000021d0: 6775 7261 7469 6f6e 2074 6f20 7370 6563  guration to spec
+000021e0: 6966 7920 6164 6469 7469 6f6e 616c 2063  ify additional c
+000021f0: 6f6e 7465 6e74 206c 6973 7469 6e67 2076  ontent listing v
+00002200: 6965 7773 0a20 205b 7661 6e67 6865 656d  iews.  [vangheem
+00002210: 5d0a 0a2d 2041 6464 206c 696d 6974 2074  ]..- Add limit t
+00002220: 6f20 636f 6e74 656e 746c 6973 7469 6e67  o contentlisting
+00002230: 0a20 205b 6d61 7274 696f 725d 0a0a 2d20  .  [martior]..- 
+00002240: 4669 7820 656d 6265 6420 7469 6c65 2074  Fix embed tile t
+00002250: 6f20 7261 6d2e 6361 6368 6520 6f65 6d62  o ram.cache oemb
+00002260: 6564 2063 6f64 6520 6279 2055 524c 0a20  ed code by URL. 
+00002270: 205b 6461 7461 6b75 7272 655d 0a0a 2d20   [datakurre]..- 
+00002280: 4669 7820 7065 726d 6973 7369 6f6e 2064  Fix permission d
+00002290: 6566 696e 6974 696f 6e73 2074 6f20 6e6f  efinitions to no
+000022a0: 7420 7573 6520 7075 626c 6963 2070 6572  t use public per
+000022b0: 6d69 7373 696f 6e73 2066 6f72 2061 6464  missions for add
+000022c0: 0a20 205b 7661 6e67 6865 656d 5d0a 0a2d  .  [vangheem]..-
+000022d0: 2046 6978 2045 7665 6e74 2074 6f20 776f   Fix Event to wo
+000022e0: 726b 2077 6974 6820 7375 6d6d 6172 795f  rk with summary_
+000022f0: 7669 6577 2063 6f6e 7465 6e74 206c 6973  view content lis
+00002300: 7469 6e67 2074 696c 650a 2020 5b76 616e  ting tile.  [van
+00002310: 6768 6565 6d5d 0a0a 2d20 4669 7820 6c69  gheem]..- Fix li
+00002320: 7374 696e 6773 206e 6f74 2069 6e63 6c75  stings not inclu
+00002330: 6469 6e67 202f 7669 6577 206f 6e20 7572  ding /view on ur
+00002340: 6c73 0a20 205b 7661 6e67 6865 656d 5d0a  ls.  [vangheem].
+00002350: 0a2d 2041 6464 2062 6574 7465 7220 6572  .- Add better er
+00002360: 726f 7220 6861 6e64 6c69 6e67 2069 6e20  ror handling in 
+00002370: 7375 6d6d 6172 795f 7669 6577 0a20 205b  summary_view.  [
+00002380: 7661 6e67 6865 656d 5d0a 0a2d 2046 6978  vangheem]..- Fix
+00002390: 2067 6574 7469 6e67 206c 6561 6420 696d   getting lead im
+000023a0: 6167 650a 2020 5b76 616e 6768 6565 6d5d  age.  [vangheem]
+000023b0: 0a0a 2d20 4669 7820 746f 206e 6f74 2074  ..- Fix to not t
+000023c0: 7261 6e73 666f 726d 2072 6177 6874 6d6c  ransform rawhtml
+000023d0: 206f 7574 7075 7420 6966 2072 656e 6465   output if rende
+000023e0: 7265 6420 7769 7468 696e 206d 6f73 6169  red within mosai
+000023f0: 6320 6c61 796f 7574 6564 6974 6f72 0a20  c layouteditor. 
+00002400: 205b 7661 6e67 6865 656d 5d0a 0a0a 312e   [vangheem]...1.
+00002410: 3062 3420 2832 3031 352d 3130 2d30 3429  0b4 (2015-10-04)
+00002420: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
+00002430: 2d2d 2d0a 0a2d 2043 6861 6e67 6520 6e61  ---..- Change na
+00002440: 7669 6761 7469 6f6e 2074 696c 6520 746f  vigation tile to
+00002450: 206e 6f74 2075 7365 2064 6570 7265 6361   not use depreca
+00002460: 7465 6420 6465 6661 756c 7473 2066 726f  ted defaults fro
+00002470: 6d20 706f 7274 616c 5f70 726f 7065 7274  m portal_propert
+00002480: 6965 730a 2020 5b64 6174 616b 7572 7265  ies.  [datakurre
+00002490: 5d0a 0a2d 2041 6464 2073 6f63 6961 6c74  ]..- Add socialt
+000024a0: 6167 7320 7469 6c65 0a20 205b 7661 6e67  ags tile.  [vang
+000024b0: 6865 656d 5d0a 0a2d 2046 6978 2073 6974  heem]..- Fix sit
+000024c0: 656d 6170 2074 696c 6520 746f 2072 6561  emap tile to rea
+000024d0: 6420 636f 7272 6563 7420 7365 7474 696e  d correct settin
+000024e0: 6720 6f6e 2050 6c6f 6e65 2035 0a20 205b  g on Plone 5.  [
+000024f0: 6461 7461 6b75 7272 655d 0a0a 0a31 2e30  datakurre]...1.0
+00002500: 6233 2028 3230 3135 2d30 392d 3136 290a  b3 (2015-09-16).
+00002510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002520: 2d2d 0a0a 2d20 4669 7820 746f 2061 7070  --..- Fix to app
+00002530: 6c79 206f 7574 7075 7420 6669 6c74 6572  ly output filter
+00002540: 7320 666f 7220 7261 7768 746d 6c20 7469  s for rawhtml ti
+00002550: 6c65 0a20 205b 6461 7461 6b75 7272 655d  le.  [datakurre]
+00002560: 0a2d 2046 6978 2065 6e63 6f64 696e 6720  .- Fix encoding 
+00002570: 6973 7375 6520 7768 656e 2072 656e 6465  issue when rende
+00002580: 7269 6e67 2065 7869 7374 696e 6720 636f  ring existing co
+00002590: 6e74 656e 7420 7469 6c65 0a20 205b 6461  ntent tile.  [da
+000025a0: 7461 6b75 7272 655d 0a0a 312e 3062 3220  takurre]..1.0b2 
+000025b0: 2832 3031 352d 3039 2d31 3629 0a2d 2d2d  (2015-09-16).---
+000025c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+000025d0: 0a2d 2041 6464 2060 6070 6c6f 6e65 2e61  .- Add ``plone.a
+000025e0: 7070 2e73 7461 6e64 6172 6474 696c 6573  pp.standardtiles
+000025f0: 2e72 6177 6874 6d6c 6060 2074 696c 650a  .rawhtml`` tile.
+00002600: 2020 5b76 616e 6768 6565 6d5d 0a2d 2043    [vangheem].- C
+00002610: 6861 6e67 6520 696d 6167 6520 7469 6c65  hange image tile
+00002620: 2074 6f20 7573 6520 7261 6469 6f20 7769   to use radio wi
+00002630: 6467 6574 2066 6f72 2069 6d61 6765 2073  dget for image s
+00002640: 6361 6c65 2073 656c 6563 7469 6f6e 0a20  cale selection. 
+00002650: 205b 6461 7461 6b75 7272 655d 0a2d 2046   [datakurre].- F
+00002660: 6978 2064 6566 6175 6c74 2076 616c 7565  ix default value
+00002670: 7320 666f 7220 7265 6e64 6572 696e 6720  s for rendering 
+00002680: 7468 6520 636f 6e74 656e 7420 6c69 7374  the content list
+00002690: 696e 6720 7469 6c65 0a20 205b 7661 6e67  ing tile.  [vang
+000026a0: 6865 656d 5d0a 0a31 2e30 6231 2028 3230  heem]..1.0b1 (20
+000026b0: 3135 2d30 362d 3038 290a 2d2d 2d2d 2d2d  15-06-08).------
+000026c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2d20  ------------..- 
+000026d0: 4669 7820 6669 656c 6420 7469 6c65 2062  Fix field tile b
+000026e0: 6163 6b77 6172 6473 2063 6f6d 7061 7469  ackwards compati
+000026f0: 6269 6c69 7479 2077 6974 6820 706c 6f6e  bility with plon
+00002700: 652e 6170 702e 626c 6f63 6b73 203c 2032  e.app.blocks < 2
+00002710: 2e31 2e31 0a20 205b 6461 7461 6b75 7272  .1.1.  [datakurr
+00002720: 655d 0a0a 312e 3061 3420 2832 3031 352d  e]..1.0a4 (2015-
+00002730: 3036 2d30 3629 0a2d 2d2d 2d2d 2d2d 2d2d  06-06).---------
+00002740: 2d2d 2d2d 2d2d 2d2d 2d0a 0a2d 2052 656d  ---------..- Rem
+00002750: 6f76 6520 7465 7874 2c20 6361 6c65 6e64  ove text, calend
+00002760: 6172 2061 6e64 2063 6f6e 6669 676c 6574  ar and configlet
+00002770: 7320 7469 6c65 730a 2020 5b64 6174 616b  s tiles.  [datak
+00002780: 7572 7265 5d0a 2d20 4164 6420 7363 7269  urre].- Add scri
+00002790: 7074 732c 2073 7479 6c65 7368 6565 7473  pts, stylesheets
+000027a0: 2061 6e64 2074 6f6f 6c62 6172 2074 696c   and toolbar til
+000027b0: 6573 2066 6f72 2050 6c6f 6e65 2035 0a20  es for Plone 5. 
+000027c0: 205b 6461 7461 6b75 7272 655d 0a2d 2041   [datakurre].- A
+000027d0: 6464 2064 7562 6c69 6e63 6f72 6520 6c61  dd dublincore la
+000027e0: 796f 7574 2074 696c 650a 2020 5b64 6174  yout tile.  [dat
+000027f0: 616b 7572 7265 5d0a 2d20 4164 6420 7469  akurre].- Add ti
+00002800: 746c 6520 6669 656c 6420 666f 7220 696d  tle field for im
+00002810: 6167 6520 7469 6c65 0a20 205b 6461 7461  age tile.  [data
+00002820: 6b75 7272 655d 0a2d 2052 6566 6163 746f  kurre].- Refacto
+00002830: 7220 6d6f 7374 206c 6179 6f75 7420 7469  r most layout ti
+00002840: 6c65 7320 746f 2072 652d 7573 6520 7669  les to re-use vi
+00002850: 6577 6c65 7473 2720 666f 7220 7368 6172  ewlets' for shar
+00002860: 6564 2063 6f64 6562 6173 650a 2020 5b64  ed codebase.  [d
+00002870: 6174 616b 7572 7265 5d0a 2d20 4669 7820  atakurre].- Fix 
+00002880: 6973 7375 6520 7768 6572 6520 6279 6c69  issue where byli
+00002890: 6e65 2074 696c 6520 7761 7320 6272 6f6b  ne tile was brok
+000028a0: 656e 206f 6e20 506c 6f6e 6520 350a 2020  en on Plone 5.  
+000028b0: 5b64 6174 616b 7572 7265 5d0a 2d20 4669  [datakurre].- Fi
+000028c0: 7820 6973 7375 6520 7768 6572 6520 6669  x issue where fi
+000028d0: 656c 6420 7469 6c65 2069 676e 6f72 6564  eld tile ignored
+000028e0: 2077 6964 6765 7420 6469 7265 6374 6976   widget directiv
+000028f0: 650a 2020 5b64 6174 616b 7572 7265 5d0a  e.  [datakurre].
+00002900: 2d20 4669 7820 7072 6f66 696c 6520 7665  - Fix profile ve
+00002910: 7273 696f 6e20 286e 6f20 7570 6772 6164  rsion (no upgrad
+00002920: 6520 7374 6570 3b20 7570 6772 6164 6520  e step; upgrade 
+00002930: 6279 2072 6569 6e73 7461 6c6c 290a 2020  by reinstall).  
+00002940: 5b64 6174 616b 7572 7265 5d0a 0a31 2e30  [datakurre]..1.0
+00002950: 6133 2028 3230 3135 2d30 352d 3237 290a  a3 (2015-05-27).
+00002960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002970: 2d2d 0a0a 2d20 4669 7820 696d 706f 7274  --..- Fix import
+00002980: 2065 7272 6f72 206f 6e20 506c 6f6e 6520   error on Plone 
+00002990: 3420 7769 7468 6f75 7420 706c 6f6e 652e  4 without plone.
+000029a0: 6170 702e 636f 6e74 656e 7474 7970 6573  app.contenttypes
+000029b0: 0a20 205b 6461 7461 6b75 7272 655d 0a0a  .  [datakurre]..
+000029c0: 312e 3061 3220 2832 3031 352d 3035 2d32  1.0a2 (2015-05-2
+000029d0: 3729 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  7).-------------
+000029e0: 2d2d 2d2d 2d0a 0a2d 2046 6978 2069 6d61  -----..- Fix ima
+000029f0: 6765 2074 696c 6520 746f 206f 6e6c 7920  ge tile to only 
+00002a00: 7365 7420 696d 6167 6520 7769 6474 6820  set image width 
+00002a10: 746f 2061 6c6c 6f77 2070 726f 706f 7274  to allow proport
+00002a20: 696f 6e61 6c20 7363 616c 696e 6720 7769  ional scaling wi
+00002a30: 7468 696e 0a20 2073 6d61 6c6c 6572 2074  thin.  smaller t
+00002a40: 6861 6e20 7769 6474 6820 636f 6c75 6d6e  han width column
+00002a50: 730a 2020 5b64 6174 616b 7572 7265 5d0a  s.  [datakurre].
+00002a60: 0a31 2e30 6131 2028 3230 3135 2d30 352d  .1.0a1 (2015-05-
+00002a70: 3235 290a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  25).------------
+00002a80: 2d2d 2d2d 2d2d 0a0a 2d20 4669 7273 7420  ------..- First 
+00002a90: 616c 7068 6120 7265 6c65 6173 652e 0a    alpha release..
```

### Comparing `plone.app.standardtiles-3.0.1/LICENSE.GPL` & `plone.app.standardtiles-3.1.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/LICENSE.txt` & `plone.app.standardtiles-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/PKG-INFO` & `plone.app.standardtiles-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.standardtiles
-Version: 3.0.1
+Version: 3.1.0
 Summary: Tiles for plone.app.blocks page composition
 Home-page: https://github.com/plone/plone.app.standardtiles
 Author: Rob Gietema
 Author-email: rob@fourdigits.nl
 License: GPL
 Keywords: tiles content plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,14 +58,22 @@
 -------
 
 The project is licensed under the GPLv2.
 
 Changelog
 =========
 
+3.1.0 (2023-05-04)
+------------------
+
+- Add option to enable the Eventlisting view (this expands recurring events).
+  NOTE: The listing will only show Event types.
+  [petschki]
+
+
 3.0.1 (2023-04-22)
 ------------------
 
 - Fix broken CMFDynamicViewFTI import.
   [thet]
 
 - Fix byline viewlet name
```

### Comparing `plone.app.standardtiles-3.0.1/README.rst` & `plone.app.standardtiles-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/setup.py` & `plone.app.standardtiles-3.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.1"
+version = "3.1.0"
 
 
 setup(
     name="plone.app.standardtiles",
     version=version,
     description="Tiles for plone.app.blocks page composition",
     long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
@@ -35,18 +35,18 @@
     package_dir={"": "src"},
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
         "plone.app.blocks",
-        "plone.app.tiles>=3.1.2",
+        "plone.app.tiles>=4.0.0",
         "plone.subrequest",
         "plone.tiles>=1.8.0",
-        "Products.CMFPlone>=6.0.0a3",
+        "Products.CMFPlone>=6.0.0",
         "requests",
         "setuptools",
     ],
     extras_require={
         "test": [
             "plone.app.testing",
             "plone.app.dexterity",
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/attachment.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from zope.deprecation import deprecated
 from zope.interface import implementer
 from zope.publisher.interfaces import IPublishTraverse
 from zope.publisher.interfaces import NotFound
 
 
 class IAttachmentTile(Schema):
-
     widget(files=MultiFileFieldWidget)
     files = schema.List(
         title=_("Upload files"),
         value_type=NamedBlobFile(title=_("Please upload a file"), required=True),
     )
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/common.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
             )
             return
 
         return viewlet
 
 
 class ProxyViewletTile(BaseViewletTile):
-
     section = "body"
     manager = None
     viewlet = None
 
     def __call__(self):
         alsoProvides(self, IViewView)
         viewlet = self.get_viewlet(self.manager, self.viewlet)
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/configure.zcml` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/content.zcml` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/content.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/contentlisting.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/contentlisting.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,14 +68,26 @@
         description=_(
             "Check this box if you do not want the results changed based on request parameters."
         ),
         required=False,
         default=False,
     )
 
+    event_listing = schema.Bool(
+        title=_(
+            "label_event_listing",
+            default="Show results as event listing",
+        ),
+        description=_(
+            "If enabled only events and their recurring occurrences are shown",
+        ),
+        required=False,
+        default=False,
+    )
+
     sort_on = schema.TextLine(
         title=_("label_sort_on", default="Sort on"),
         description=_("Sort the collection on this index"),
         required=False,
     )
 
     sort_reversed = schema.Bool(
@@ -210,41 +222,81 @@
 
     @property
     def description(self):
         return self.data.get("description")
 
     def contents(self):
         """Search results"""
-        builder = getMultiAdapter(
-            (self.context, self.request), name="querybuilderresults"
-        )
 
         # Include query parameters from request if not set to ignore
         contentFilter = {}
         if not self.ignore_request_params:
             contentFilter = dict(self.request.get("contentFilter", {}))
 
-        accessor = builder(
-            query=self.query,
-            sort_on=self.sort_on or "getObjPositionInParent",
-            sort_order=self.sort_order,
-            limit=self.limit,
-            batch=True,
-            b_start=self.b_start,
-            b_size=self.item_count or 30,
-            brains=False,
-            custom_query=contentFilter,
-        )
+        # This should be an event listing
+        # -> re-use plone.app.event.browser.event_listing logic
+        if self.data.get("event_listing"):
+            # Get results from plone.app.event.browser.event_listing
+            event_listing_view = getMultiAdapter(
+                (self, self.request), name="event_listing"
+            )
+            # Enable contentlisting query lookup
+            event_listing_view.is_collection = True
+            # Mandatory information for batching
+            event_listing_view.b_start = self.b_start
+            event_listing_view.b_size = self.item_count
+            event_listing_view.limit = self.limit
+
+            results = event_listing_view.events()
+        else:
+            results = self.results(
+                b_start=self.b_start,
+                custom_query=contentFilter,
+            )
 
-        accessor.b_start_str = self.b_start_str
+        results.b_start_str = self.b_start_str
 
         view = self.view_template or "listing_view"
         options = dict(original_context=self.context)
         alsoProvides(self.request, IContentListingTileLayer)
-        return getMultiAdapter((accessor, self.request), name=view)(**options)
+        return getMultiAdapter((results, self.request), name=view)(**options)
+
+    # Implementation of ICollection.results
+    def results(
+        self,
+        batch=True,
+        b_start=0,
+        b_size=None,
+        sort_on=None,
+        limit=None,
+        brains=False,
+        custom_query=None,
+    ):
+        if not b_size:
+            b_size = self.item_count
+        if not sort_on:
+            sort_on = self.sort_on
+        if not limit:
+            limit = self.limit
+
+        builder = getMultiAdapter(
+            (self.context, self.request), name="querybuilderresults"
+        )
+
+        return builder(
+            query=self.query,
+            batch=batch,
+            b_start=b_start,
+            b_size=b_size,
+            sort_on=sort_on,
+            sort_order=self.sort_order,
+            limit=limit,
+            brains=brains,
+            custom_query=custom_query,
+        )
 
     @property
     def tile_class(self):
         css_class = "contentlisting-tile"
         additional_classes = self.data.get("tile_class", "")
         if not additional_classes:
             return css_class
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/discussion.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/discussion.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/embed.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/embed.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/existingcontent.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/existingcontent.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     if len(result) != 1:
         return
 
     return result[0]
 
 
 class IExistingContentTile(model.Schema):
-
     content_uid = schema.Choice(
         title=_("Select an existing content"),
         required=True,
         vocabulary="plone.app.vocabularies.Catalog",
     )
     form.widget(
         "content_uid",
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/field.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
     def _wrap_widget(self, render):
         if render.rstrip().endswith("</html>"):
             return render
         return "".join(["<html><body>", render, "</body></html>"])
 
     def updateWidgets(self, prefix=None):
         if self.field is not None:
-
             if self.field in self.fields:
                 self.fields = self.fields.select(self.field)
             else:
                 self.fields = Fields()
 
             for group in self.groups or []:
                 if self.field in group.fields:
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/head.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/head.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/head.zcml` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/head.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/html.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/html.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from plone.tiles.directives import ignore_querystring
 from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone.utils import safe_unicode
 from zope import schema
 
 
 class IHTMLTile(Schema):
-
     ignore_querystring("content")
     primary("content")
     content = schema.Text(
         title=_("HTML"),
         required=True,
     )
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/interfaces.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/layout.zcml` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/layout.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/linkintegrity.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/linkintegrity.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/media.zcml` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/media.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/metadata.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/metadata.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/navigation.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/navigation.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/add.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/add.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/assignment.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/assignment.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/configure.zcml` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/edit.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/edit.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 
         typeName = "plone.app.standardtiles.portlet"
         tile_url = "{}/@@{}/{}?portlet_hash={}".format(
             self.context.absolute_url(), typeName, tileId, portlet_hash
         )
         self.request.form["referer"] = tile_url
         self.request.response.redirect(
-            "{0}?referer={0}".format(url, urllib.parse.quote(tile_url))
+            "{0}?referer={1}".format(url, urllib.parse.quote(tile_url))
         )
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/portlet.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/portlet.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.interface import implementer
 from zope.interface import Interface
 
 
 class IPortletTile(Interface):
-
     form.omitted("portlet_hash")
     portlet_hash = schema.TextLine(title=_("Portlet hash"), required=False)
 
     portlet_type = schema.Choice(
         title=_("Portlet type"),
         vocabulary="standardtiles.available_portlets",
         required=True,
@@ -59,8 +58,8 @@
         renderer.__portlet_metadata__ = info
 
         renderer.update()
         if IDeferredPortletRenderer.providedBy(renderer):
             # if this is a deferred load, prepare now the data
             renderer.deferred_update()
 
-        return f"<html><body>%s</body></html>"
+        return f"<html><body>{renderer.render()}</body></html>"
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/portletmanager.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/portletmanager.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/utils.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/vocabularies.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/portlets/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/default/registry.xml` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/rawembed.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/rawembed.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/rss.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/rss.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/setuphandlers.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/sitemap.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/sitemap.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/attachment_listing.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/attachment_listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/configlets.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/configlets.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/contentlisting_view.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/contentlisting_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/existingcontent_view.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/existingcontent_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/image.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/image.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/listing_view.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/listing_view.pt`

 * *Files 6% similar despite different names*

```diff
@@ -13,47 +13,51 @@
                          show_about python:True;
                          registry original_context/portal_registry;
                          view_types python: registry.get('plone.types_use_view_action_in_listings', [])">
       <tal:listing condition="batch">
         <dl>
           <tal:entry repeat="item batch">
             <dt tal:define="item_has_image python:item.getIcon;
-                            item_url python: item.portal_type in view_types and item.getURL() + '/view' or item.getURL()">
+                            item_url item/getURL|item/absolute_url;
+                            item_type item/portal_type;
+                            item_creator item/Creator|item/creator;
+                            item_modified item/ModificationDate|item/modified;
+                            item_view_url python: item_url + '/view' if item.portal_type in view_types else item_url">
               <span class="summary">
                 <img tal:condition="item_has_image"
-                             tal:attributes="src string:${item/getURL}/@@images/image/tile" />
+                             tal:attributes="src string:${item_url}/@@images/image/tile" />
                 <a href="#"
-                   tal:attributes="href item_url;
+                   tal:attributes="href item_view_url;
                                    class string:${item/ContentTypeClass} ${item/review_state}"
                    tal:content="item/Title|item/getId" />
               </span>
               <span class="documentByLine">
-                <tal:comment condition="python:item.Type() == 'Event'">
+                <tal:comment condition="python:item_type == 'Event'">
                   <!-- Removed special handling for Event type for now.-->
                 </tal:comment>
                 <tal:byline condition="show_about">
                   &mdash;
                   <span class="documentAuthor"
-                        tal:define="author python:pas_member.info(item.Creator())"
+                        tal:define="author python:pas_member.info(item_creator)"
                         i18n:translate="label_by_author">
                     by
                     <a href="#"
                        tal:content="author/name_or_id"
                        tal:omit-tag="not:author"
                        tal:attributes="href string:${original_context/@@plone_portal_state/navigation_root_url}/author/${author/username}"
                        i18n:name="author">
                       Bob Dobalina
                     </a>
                   </span>
-                  <tal:modified condition="python: item.Type() != 'Event'">
+                  <tal:modified condition="python: item_type != 'Event'">
                     &mdash;
                     <tal:mod i18n:translate="">
                       last modified
                     </tal:mod>
-                    <span tal:replace="python:toLocalizedTime(item.ModificationDate())">
+                    <span tal:replace="python:toLocalizedTime(item_modified)">
                       August 16, 2001 at 23:35:59
                     </span>
                   </tal:modified>
                 </tal:byline>
               </span>
             </dt>
             <dd>
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/login.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/login.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/namedimage.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/namedimage.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/navigation.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/navigation.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/navigation_recurse.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/navigation_recurse.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/navigationlink.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/navigationlink.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/rawembed.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/rawembed.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/rss.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/rss.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/summary_view.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/summary_view.pt`

 * *Files 2% similar despite different names*

```diff
@@ -8,37 +8,38 @@
       i18n:domain="plone">
   <body>
     <div tal:define="batch context;
                      original_context nocall:options/original_context|context;
                      registry original_context/portal_registry;
                      view_types python: registry.get('plone.types_use_view_action_in_listings', [])">
       <tal:entry repeat="item batch">
-      <tal:block tal:define="item_url python: item.portal_type in view_types and item.getURL() + '/view' or item.getURL();
-                             item_title_or_id item/title_or_id;
-                             item_type item/Type;
-                             item_creator item/Creator;
+      <tal:block tal:define="item_url item/getURL|item/absolute_url;
+                             item_view_url python: item_url + '/view' if item.portal_type in view_types else item_url;
+                             item_title_or_id item/Title|item/title_or_id;
+                             item_type item/portal_type;
+                             item_creator item/Creator|item/creator;
                              item_description item/Description;
-                             item_modified item/ModificationDate;
+                             item_modified item/ModificationDate|item/modified;
                              item_start item/start;
                              item_end item/end;">
         <div class="tileItem visualIEFloatFix"
              tal:define="item_has_image python:item.getIcon">
           <a href="#"
              class="summary-image"
              tal:condition="item_has_image"
-             tal:attributes="href item_url">
+             tal:attributes="href item_view_url">
             <img tal:condition="item_has_image"
-                 tal:attributes="src string:${item/getURL}/@@images/image/thumb"
+                 tal:attributes="src string:${item_url}/@@images/image/thumb"
                  alt=""/>
           </a>
           <h2 class="tileHeadline"
               metal:define-macro="listitem">
             <a href="#"
                class="summary url"
-               tal:attributes="href item_url"
+               tal:attributes="href item_view_url"
                tal:content="item_title_or_id">
               Item Title
             </a>
           </h2>
           <div class="documentByLine">
             <tal:event condition="python: item_start or item_end">
               <span tal:condition="python: item.location"
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/tabular_view.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/templates/tabular_view.pt`

 * *Files 11% similar despite different names*

```diff
@@ -45,25 +45,26 @@
                                     Modified
                                 </tal:modified>&nbsp;
                             </th>
                         </tr>
                     </thead>
                     <tbody>
                         <tal:results repeat="item batch">
-                            <tal:block tal:define="item_url python: item.portal_type in view_types and item.getURL() + '/view' or item.getURL();
-                                                   item_title_or_id item/title_or_id;
-                                                   item_type item/Type;
+                            <tal:block tal:define="item_url item/getURL|item/absolute_url;
+                                                   item_view_url python: item_url + '/view' if item.portal_type in view_types else item_url;
+                                                   item_title_or_id item/Title|item/title_or_id;
+                                                   item_type item/portal_type;
                                                    item_description item/Description;
-                                                   item_creator item/Creator;
-                                                   item_modified item/ModificationDate">
+                                                   item_creator item/Creator|item/creator;
+                                                   item_modified item/ModificationDate|item/modified">
 
                             <tr tal:define="oddrow repeat/item/odd;"
                                 tal:attributes="class python:oddrow and 'even' or 'odd'" >
                                 <td>
-                                    <a href="#" tal:attributes="href item_url" tal:content="item_title_or_id">
+                                    <a href="#" tal:attributes="href item_view_url" tal:content="item_title_or_id">
                                         Item Title
                                     </a>
                                 </td>
                                 <td tal:condition="view_about">
                                     <tal:name tal:condition="item_creator" tal:define="author python:pas_member.info(item_creator)">
                                         <a href="#"
                                            tal:attributes="href string:author/${author/username}"
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/testing.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 EDITOR_USER_NAME = "editor"
 EDITOR_USER_PASSWORD = "confidential"
 MANAGER_USER_NAME = "manager"
 MANAGER_USER_PASSWORD = "topsecret"
 
 
 class RequestsGetMock:
-
     ok = True
     url = None
 
     def __init__(self, url):
         self.url = url
 
     def json(self):
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/testing.zcml` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/RSS.xml` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/RSS.xml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/funky_display.pt` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/funky_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_content.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_existing_content.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/test_existing_content.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_field.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_head.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/test_head.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_layout.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_media.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/test_media.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_setup.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/tests/test_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,25 @@
 import unittest
 
 
 PROJECTNAME = "plone.app.standardtiles"
 
 
 class InstallTestCase(unittest.TestCase):
-
     layer = PASTANDARDTILES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
 
     def test_installed(self):
         qi = get_installer(self.portal, self.layer["request"])
         self.assertTrue(qi.is_product_installed(PROJECTNAME))
 
 
 class UninstallTestCase(unittest.TestCase):
-
     layer = PASTANDARDTILES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.qi = get_installer(self.portal, self.layer["request"])
         self.qi.uninstall_product(PROJECTNAME)
         self.registry = getUtility(IRegistry)
@@ -40,14 +38,13 @@
         self.fail("TODO: Not Implemented")
 
     def filter_record(self, record):
         """Return a list of record items related with the project."""
         return [v for v in self.registry[record] if v.startswith(PROJECTNAME)]
 
     def test_registry_cleaned(self):
-
         self.assertEqual(self.filter_record("plone.app.tiles"), [])
 
         self.assertNotIn("plone.app.standardtiles.listing_views", self.registry)
 
         record = "plone.app.portlets.PortletManagerBlacklist"
         self.assertEqual(self.filter_record(record), [])
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/upgrades.zcml` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/utils.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/viewletmanager.py` & `plone.app.standardtiles-3.1.0/src/plone/app/standardtiles/viewletmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from zope.interface import Interface
 from zope.viewlet.interfaces import IViewletManager
 
 import Acquisition
 
 
 class IViewletManagerTile(Interface):
-
     manager = schema.TextLine(title=_("Name of the viewlet manager."), required=True)
 
     view = schema.TextLine(title=_("Name of the view"), required=False)
 
     section = schema.Choice(
         title=_("Section of the page"),
         values=("head", "body"),
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/PKG-INFO` & `plone.app.standardtiles-3.1.0/src/plone.app.standardtiles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.standardtiles
-Version: 3.0.1
+Version: 3.1.0
 Summary: Tiles for plone.app.blocks page composition
 Home-page: https://github.com/plone/plone.app.standardtiles
 Author: Rob Gietema
 Author-email: rob@fourdigits.nl
 License: GPL
 Keywords: tiles content plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,14 +58,22 @@
 -------
 
 The project is licensed under the GPLv2.
 
 Changelog
 =========
 
+3.1.0 (2023-05-04)
+------------------
+
+- Add option to enable the Eventlisting view (this expands recurring events).
+  NOTE: The listing will only show Event types.
+  [petschki]
+
+
 3.0.1 (2023-04-22)
 ------------------
 
 - Fix broken CMFDynamicViewFTI import.
   [thet]
 
 - Fix byline viewlet name
```

### Comparing `plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/SOURCES.txt` & `plone.app.standardtiles-3.1.0/src/plone.app.standardtiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

