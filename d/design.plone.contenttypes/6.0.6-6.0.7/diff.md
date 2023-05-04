# Comparing `tmp/design.plone.contenttypes-6.0.6.tar.gz` & `tmp/design.plone.contenttypes-6.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.contenttypes-6.0.6.tar", last modified: Fri Apr 28 06:57:41 2023, max compression
+gzip compressed data, was "design.plone.contenttypes-6.0.7.tar", last modified: Thu May  4 08:01:57 2023, max compression
```

## Comparing `design.plone.contenttypes-6.0.6.tar` & `design.plone.contenttypes-6.0.7.tar`

### file list

```diff
@@ -1,360 +1,360 @@
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.254011 design.plone.contenttypes-6.0.6/
--rw-r--r--   0 lucabel    (501) staff       (20)    16812 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/CHANGES.rst
--rw-r--r--   0 lucabel    (501) staff       (20)       67 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/CONTRIBUTORS.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      585 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/DEVELOP.rst
--rw-r--r--   0 lucabel    (501) staff       (20)    18092 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/LICENSE.GPL
--rw-r--r--   0 lucabel    (501) staff       (20)      665 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/LICENSE.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      158 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/MANIFEST.in
--rw-r--r--   0 lucabel    (501) staff       (20)    33576 2023-04-28 06:57:41.254164 design.plone.contenttypes-6.0.6/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)    15519 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/README.md
--rw-r--r--   0 lucabel    (501) staff       (20)       27 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/constraints.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      105 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/constraints_plone60.txt
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.170636 design.plone.contenttypes-6.0.6/docs/
--rw-r--r--   0 lucabel    (501) staff       (20)     7993 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/docs/conf.py
--rw-r--r--   0 lucabel    (501) staff       (20)       98 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/docs/index.rst
--rw-r--r--   0 lucabel    (501) staff       (20)       50 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/requirements.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      383 2023-04-28 06:57:41.254807 design.plone.contenttypes-6.0.6/setup.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2892 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/setup.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.158628 design.plone.contenttypes-6.0.6/src/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.170910 design.plone.contenttypes-6.0.6/src/design/
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.173591 design.plone.contenttypes-6.0.6/src/design/plone/
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.175800 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/
--rw-r--r--   0 lucabel    (501) staff       (20)      668 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.177140 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/adapters/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/adapters/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      828 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/adapters/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      421 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/adapters/interfaces.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1755 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/adapters/searchabletext_indexers.py
--rw-r--r--   0 lucabel    (501) staff       (20)      231 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/adapters/servizi_correlati.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.183386 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1354 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/additional_help_infos.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2403 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/address.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7942 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/argomenti.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11450 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     6669 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/contatti.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1629 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/dataset_correlati.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2679 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/descrizione_estesa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6334 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/evento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1657 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/geolocation.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2388 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/info_testata.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2733 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/luoghi_correlati.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6580 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1606 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/multi_file.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4559 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/news_additional_fields.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1827 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/servizi_correlati.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1357 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/show_modified.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1688 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/strutture_correlate.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10532 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/trasparenza.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1164 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/update_note.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.184188 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1342 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.185601 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3813 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/change_news_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5162 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/check_servizi.py
--rw-r--r--   0 lucabel    (501) staff       (20)      787 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2796 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/move_news_items.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.186539 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/templates/
--rw-r--r--   0 lucabel    (501) staff       (20)     3360 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     6876 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/templates/check_servizi.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     4760 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.187089 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/overrides/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/overrides/.gitkeep
--rw-r--r--   0 lucabel    (501) staff       (20)      993 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.160381 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/static/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.187395 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/static/js/
--rw-r--r--   0 lucabel    (501) staff       (20)      262 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/static/js/move_content.js
--rw-r--r--   0 lucabel    (501) staff       (20)      469 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/trasparenza.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2770 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.192177 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      315 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)      238 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/dataset.py
--rw-r--r--   0 lucabel    (501) staff       (20)      246 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      283 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/documento_personale.py
--rw-r--r--   0 lucabel    (501) staff       (20)      210 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/evento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      242 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/incarico.py
--rw-r--r--   0 lucabel    (501) staff       (20)      215 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)      275 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/messaggio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      229 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)      271 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      238 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)      238 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)      272 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)      279 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/ricevuta_pagamento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      242 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      283 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/content/unita_organizzativa.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.193287 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/controlpanels/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/controlpanels/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      737 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/controlpanels/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1382 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3441 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/controlpanels/settings.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.197533 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      540 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)      276 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/common.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2964 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      618 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/document.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1265 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3024 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/evento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1660 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/incarico.py
--rw-r--r--   0 lucabel    (501) staff       (20)      848 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1268 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/notizie_e_comunicati_stampa.py
--rw-r--r--   0 lucabel    (501) staff       (20)      969 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1886 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)      631 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1053 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1078 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/unita_organizzativa.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.200738 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      458 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)      989 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/common.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1605 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      411 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/events.py
--rw-r--r--   0 lucabel    (501) staff       (20)      921 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/news.py
--rw-r--r--   0 lucabel    (501) staff       (20)      621 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      829 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)      741 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)      327 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      445 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/uo.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.205489 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/
--rw-r--r--   0 lucabel    (501) staff       (20)      419 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6263 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)      699 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)      857 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/dataset.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8681 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4702 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/documento_personale.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5442 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/incarico.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1483 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/messaggio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      205 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2600 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4773 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1781 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2522 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1838 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py
--rw-r--r--   0 lucabel    (501) staff       (20)    18282 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8198 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/unita_organizzativa.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.207225 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/
--rw-r--r--   0 lucabel    (501) staff       (20)      611 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/README.rst
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.161823 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/__pycache__/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.207515 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)    83688 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po
--rw-r--r--   0 lucabel    (501) staff       (20)    83643 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.162139 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/en/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.207929 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/en/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)    83808 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.162456 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/it/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.209078 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/it/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)     1243 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po
--rw-r--r--   0 lucabel    (501) staff       (20)    84783 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po
--rw-r--r--   0 lucabel    (501) staff       (20)     7287 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/plone.pot
--rw-r--r--   0 lucabel    (501) staff       (20)     1597 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/update.py
--rwxr-xr-x   0 lucabel    (501) staff       (20)      512 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/update.sh
--rw-r--r--   0 lucabel    (501) staff       (20)      712 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/overrides.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.210266 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/patches/
--rw-r--r--   0 lucabel    (501) staff       (20)      516 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/patches/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3700 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/patches/baseserializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)      483 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/patches/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      319 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/patches/patches.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2751 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/permissions.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.164355 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.163090 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.218040 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/
--rw-r--r--   0 lucabel    (501) staff       (20)      314 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     3401 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      331 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     4370 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      286 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2870 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      372 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     8078 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      300 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2156 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      313 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)    13733 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      398 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     5133 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      292 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     1042 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      303 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2196 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      265 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)    15346 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      322 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     1015 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      355 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     3138 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      342 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2275 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      344 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2275 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.221077 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/
--rw-r--r--   0 lucabel    (501) staff       (20)      193 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2681 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/catalog.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1040 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/controlpanel.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1219 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/diff_tool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      519 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/metadata.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.221776 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/registry/
--rw-r--r--   0 lucabel    (501) staff       (20)    19192 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/registry/criteria.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      618 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/registry/settings.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1139 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/repositorytool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     4491 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/rolemap.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.227566 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/
--rw-r--r--   0 lucabel    (501) staff       (20)     1155 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Bando.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      503 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Bando_Folder_Deepening.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3563 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3327 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Dataset.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      921 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Document.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3747 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Documento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3321 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2500 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Event.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3427 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Incarico.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      432 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Link.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3199 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2855 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Modulo.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1007 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/News_Item.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3456 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3430 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Persona.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3178 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Pratica.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3342 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3149 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3784 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Servizio.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3775 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2212 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Venue.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1194 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.227809 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/fix_syndication/
--rw-r--r--   0 lucabel    (501) staff       (20)      524 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.228300 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/to_3000/
--rw-r--r--   0 lucabel    (501) staff       (20)      377 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/to_3000/controlpanel.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      275 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/to_3000/registry.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.228554 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/uninstall/
--rw-r--r--   0 lucabel    (501) staff       (20)      128 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.229689 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      663 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      504 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/converters.py
--rw-r--r--   0 lucabel    (501) staff       (20)      702 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/correlati.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.232011 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      760 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     5795 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6300 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/dxfields.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5743 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/news.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1658 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5844 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5999 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6016 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/venue.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.236101 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1254 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2086 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1921 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2102 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3377 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/dxcontent.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6505 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/dxfields.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1452 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2190 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3771 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1763 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2401 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/relationfield.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1705 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)    13976 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/summary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5886 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3814 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/venue.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.236868 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      564 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.237671 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/content/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/content/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      664 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/content/add.py
--rw-r--r--   0 lucabel    (501) staff       (20)      368 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/content/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      653 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/controlpanel.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.238440 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/modulistica_items/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/modulistica_items/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      605 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2915 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.239243 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/scadenziario/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/scadenziario/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1200 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)    10380 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/scadenziario/post.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.240131 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/trasparenza/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/trasparenza/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      884 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     3351 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/trasparenza/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.240949 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/types/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/types/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      404 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/types/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)    10630 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/types/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.241654 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/types/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/types/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3804 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/types/adapters.py
--rw-r--r--   0 lucabel    (501) staff       (20)      394 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/types/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1628 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/schema_overrides.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2315 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/setuphandlers.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3921 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/testing.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.249706 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11218 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/example.pdf
--rw-r--r--   0 lucabel    (501) staff       (20)    10503 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/example.png
--rw-r--r--   0 lucabel    (501) staff       (20)     1997 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_argomenti.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2330 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_base_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1564 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3169 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_behavior_luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2563 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_behavior_show_modified.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1755 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_behavior_update_note.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1893 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_change_news_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1679 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1462 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1342 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_document.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6365 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1294 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_documento_personale.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4924 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_event.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7744 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)      982 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8019 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_news.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1296 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5271 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11188 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10788 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2164 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_filefield_view_mode_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2526 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_move_news_items_view.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6638 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1381 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3533 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_setup.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11257 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_summary_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4714 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6351 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_vocabularies.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.251237 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/upgrades/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/upgrades/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)    21941 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/upgrades/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     5033 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/upgrades/draftjs_converter.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11792 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/upgrades/to_7001.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5975 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/upgrades/to_7002.py
--rw-r--r--   0 lucabel    (501) staff       (20)    50684 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/upgrades/upgrades.py
--rw-r--r--   0 lucabel    (501) staff       (20)      862 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/utils.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.253796 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1308 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1573 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1824 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1466 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1895 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1704 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/mockup.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2223 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/people_vocabulary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1533 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5199 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-04-28 06:57:41.173322 design.plone.contenttypes-6.0.6/src/design.plone.contenttypes.egg-info/
--rw-r--r--   0 lucabel    (501) staff       (20)    33576 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design.plone.contenttypes.egg-info/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)    18446 2023-04-28 06:57:41.000000 design.plone.contenttypes-6.0.6/src/design.plone.contenttypes.egg-info/SOURCES.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design.plone.contenttypes.egg-info/dependency_links.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      130 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design.plone.contenttypes.egg-info/entry_points.txt
--rw-r--r--   0 lucabel    (501) staff       (20)       20 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design.plone.contenttypes.egg-info/namespace_packages.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design.plone.contenttypes.egg-info/not-zip-safe
--rw-r--r--   0 lucabel    (501) staff       (20)      411 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design.plone.contenttypes.egg-info/requires.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        7 2023-04-28 06:57:40.000000 design.plone.contenttypes-6.0.6/src/design.plone.contenttypes.egg-info/top_level.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.647090 design.plone.contenttypes-6.0.7/
+-rw-r--r--   0 lucabel    (501) staff       (20)    16931 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/CHANGES.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       67 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/CONTRIBUTORS.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      585 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/DEVELOP.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)    18092 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/LICENSE.GPL
+-rw-r--r--   0 lucabel    (501) staff       (20)      665 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/LICENSE.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      158 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/MANIFEST.in
+-rw-r--r--   0 lucabel    (501) staff       (20)    33695 2023-05-04 08:01:57.647246 design.plone.contenttypes-6.0.7/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)    15519 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/README.md
+-rw-r--r--   0 lucabel    (501) staff       (20)       27 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/constraints.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      105 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/constraints_plone60.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.546646 design.plone.contenttypes-6.0.7/docs/
+-rw-r--r--   0 lucabel    (501) staff       (20)     7993 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/docs/conf.py
+-rw-r--r--   0 lucabel    (501) staff       (20)       98 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/docs/index.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       50 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/requirements.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      383 2023-05-04 08:01:57.647840 design.plone.contenttypes-6.0.7/setup.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2892 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/setup.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.532739 design.plone.contenttypes-6.0.7/src/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.546988 design.plone.contenttypes-6.0.7/src/design/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.550208 design.plone.contenttypes-6.0.7/src/design/plone/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.552983 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/
+-rw-r--r--   0 lucabel    (501) staff       (20)      668 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.554536 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/adapters/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/adapters/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      828 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/adapters/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      421 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/adapters/interfaces.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1755 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/adapters/searchabletext_indexers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      231 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/adapters/servizi_correlati.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.562425 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1354 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/additional_help_infos.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2403 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/address.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7942 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/argomenti.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11450 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     6669 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/contatti.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1629 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/dataset_correlati.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2679 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/descrizione_estesa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6334 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/evento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1657 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/geolocation.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2388 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/info_testata.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2733 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/luoghi_correlati.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6580 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1606 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/multi_file.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4559 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/news_additional_fields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1827 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/servizi_correlati.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1357 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/show_modified.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1688 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/strutture_correlate.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    10532 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/trasparenza.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1164 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/update_note.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.563510 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1342 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.565050 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3813 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/change_news_type.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5720 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/check_servizi.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      787 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2796 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/move_news_items.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.566267 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/templates/
+-rw-r--r--   0 lucabel    (501) staff       (20)     3360 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     7637 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/templates/check_servizi.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     4760 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.566840 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/overrides/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/overrides/.gitkeep
+-rw-r--r--   0 lucabel    (501) staff       (20)      993 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.535893 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/static/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.567168 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/static/js/
+-rw-r--r--   0 lucabel    (501) staff       (20)      262 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/static/js/move_content.js
+-rw-r--r--   0 lucabel    (501) staff       (20)      469 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/trasparenza.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2770 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.574953 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      315 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      238 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/dataset.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      246 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      283 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/documento_personale.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      210 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/evento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      242 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/incarico.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      215 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      275 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/messaggio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      229 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      271 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      238 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      238 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      272 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      279 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/ricevuta_pagamento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      242 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      283 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/content/unita_organizzativa.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.576252 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/controlpanels/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/controlpanels/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      737 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/controlpanels/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1382 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3441 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/controlpanels/settings.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.583289 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      540 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      276 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/common.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2964 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      618 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/document.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1265 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3024 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/evento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1660 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/incarico.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      848 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1268 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/notizie_e_comunicati_stampa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      969 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1886 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      631 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1053 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1078 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/unita_organizzativa.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.586960 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      458 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      989 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/common.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1605 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      411 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/events.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      921 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/news.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      621 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      829 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      741 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      327 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      445 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/uo.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.591860 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/
+-rw-r--r--   0 lucabel    (501) staff       (20)      419 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6263 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      699 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      857 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/dataset.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8681 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4702 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/documento_personale.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5442 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/incarico.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1483 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/messaggio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      205 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2600 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4773 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1781 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2522 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1838 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    18283 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8198 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/unita_organizzativa.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.593392 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/
+-rw-r--r--   0 lucabel    (501) staff       (20)      611 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/README.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.537323 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/__pycache__/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.593644 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)    83688 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po
+-rw-r--r--   0 lucabel    (501) staff       (20)    83643 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.537631 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/en/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.594116 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/en/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)    83808 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.537940 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/it/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.595285 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/it/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1243 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po
+-rw-r--r--   0 lucabel    (501) staff       (20)    84783 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po
+-rw-r--r--   0 lucabel    (501) staff       (20)     7287 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/plone.pot
+-rw-r--r--   0 lucabel    (501) staff       (20)     1597 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/update.py
+-rwxr-xr-x   0 lucabel    (501) staff       (20)      512 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/update.sh
+-rw-r--r--   0 lucabel    (501) staff       (20)      712 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/overrides.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.596464 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/patches/
+-rw-r--r--   0 lucabel    (501) staff       (20)      516 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/patches/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3700 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/patches/baseserializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      483 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/patches/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      319 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/patches/patches.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2751 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/permissions.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.539662 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.538563 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.604505 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/
+-rw-r--r--   0 lucabel    (501) staff       (20)      314 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     3401 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      331 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     4370 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      286 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2870 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      372 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     8078 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      300 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2156 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      313 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)    13733 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      398 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     5133 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      292 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     1042 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      303 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2196 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      265 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)    15346 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      322 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     1015 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      355 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     3138 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      342 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2275 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      344 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2275 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.606619 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/
+-rw-r--r--   0 lucabel    (501) staff       (20)      193 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2681 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/catalog.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1040 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/controlpanel.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1219 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/diff_tool.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      519 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/metadata.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.607178 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/registry/
+-rw-r--r--   0 lucabel    (501) staff       (20)    19192 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/registry/criteria.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      618 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/registry/settings.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1139 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/repositorytool.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     4491 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/rolemap.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.614670 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1155 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Bando.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      503 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Bando_Folder_Deepening.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3563 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3327 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Dataset.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      921 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Document.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3747 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Documento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3321 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2500 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Event.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3427 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Incarico.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      432 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Link.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3199 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2855 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Modulo.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1007 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/News_Item.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3456 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3430 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Persona.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3178 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Pratica.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3342 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3149 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3784 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Servizio.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3775 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2212 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Venue.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1194 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.615047 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/fix_syndication/
+-rw-r--r--   0 lucabel    (501) staff       (20)      524 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.615763 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/to_3000/
+-rw-r--r--   0 lucabel    (501) staff       (20)      377 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/to_3000/controlpanel.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      275 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/to_3000/registry.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.616063 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/uninstall/
+-rw-r--r--   0 lucabel    (501) staff       (20)      128 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.617145 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      663 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      504 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/converters.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      702 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/correlati.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.620156 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      760 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     5795 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6300 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/dxfields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5743 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/news.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1658 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5844 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5999 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6016 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/venue.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.624890 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1254 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2086 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1921 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2102 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3377 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/dxcontent.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6505 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/dxfields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1452 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2190 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3771 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1763 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2401 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/relationfield.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1705 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    13976 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/summary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5886 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3814 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/venue.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.625871 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      564 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.626688 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/content/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/content/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      664 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/content/add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      368 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/content/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      653 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/controlpanel.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.627566 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/modulistica_items/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/modulistica_items/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      605 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2915 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.628676 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/scadenziario/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/scadenziario/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1200 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)    10380 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/scadenziario/post.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.629530 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/trasparenza/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/trasparenza/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      884 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3351 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/trasparenza/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.630579 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/types/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      404 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/types/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)    10630 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/types/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.631523 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/types/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3804 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/types/adapters.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      394 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/types/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1628 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/schema_overrides.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2315 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/setuphandlers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3921 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/testing.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.641691 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11218 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/example.pdf
+-rw-r--r--   0 lucabel    (501) staff       (20)    10503 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/example.png
+-rw-r--r--   0 lucabel    (501) staff       (20)     1997 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_argomenti.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2330 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_base_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1564 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3169 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_behavior_luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2563 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_behavior_show_modified.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1755 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_behavior_update_note.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1893 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_change_news_type.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1679 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1462 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1342 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_document.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6365 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1294 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_documento_personale.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4924 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_event.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7744 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      982 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8019 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_news.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1296 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5271 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11188 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    10788 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2164 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_filefield_view_mode_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2526 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_move_news_items_view.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6638 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1381 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3533 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_setup.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11257 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_summary_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4714 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6351 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_vocabularies.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.643694 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/upgrades/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/upgrades/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    21941 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/upgrades/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     5033 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/upgrades/draftjs_converter.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11792 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/upgrades/to_7001.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5975 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/upgrades/to_7002.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    50684 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/upgrades/upgrades.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      862 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/utils.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.646843 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1308 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1573 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1824 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1466 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1895 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1704 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/mockup.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2223 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/people_vocabulary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1533 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5199 2023-05-04 08:01:56.000000 design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-05-04 08:01:57.549897 design.plone.contenttypes-6.0.7/src/design.plone.contenttypes.egg-info/
+-rw-r--r--   0 lucabel    (501) staff       (20)    33695 2023-05-04 08:01:57.000000 design.plone.contenttypes-6.0.7/src/design.plone.contenttypes.egg-info/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)    18446 2023-05-04 08:01:57.000000 design.plone.contenttypes-6.0.7/src/design.plone.contenttypes.egg-info/SOURCES.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-05-04 08:01:57.000000 design.plone.contenttypes-6.0.7/src/design.plone.contenttypes.egg-info/dependency_links.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      130 2023-05-04 08:01:57.000000 design.plone.contenttypes-6.0.7/src/design.plone.contenttypes.egg-info/entry_points.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       20 2023-05-04 08:01:57.000000 design.plone.contenttypes-6.0.7/src/design.plone.contenttypes.egg-info/namespace_packages.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-05-04 08:01:57.000000 design.plone.contenttypes-6.0.7/src/design.plone.contenttypes.egg-info/not-zip-safe
+-rw-r--r--   0 lucabel    (501) staff       (20)      411 2023-05-04 08:01:57.000000 design.plone.contenttypes-6.0.7/src/design.plone.contenttypes.egg-info/requires.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        7 2023-05-04 08:01:57.000000 design.plone.contenttypes-6.0.7/src/design.plone.contenttypes.egg-info/top_level.txt
```

### Comparing `design.plone.contenttypes-6.0.6/CHANGES.rst` & `design.plone.contenttypes-6.0.7/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+6.0.7 (2023-05-04)
+------------------
+
+- Fix check_servizi view and made optional canale_fisico in Servizio
+  [lucabel]
 
 6.0.6 (2023-04-28)
 ------------------
 
 - Added images serialization to the summary serializer of the UO content type;
   If both the image and preview image are present, the 'image_field' attribute
   is forced to contain 'preview_image'.
@@ -19,15 +24,14 @@
   UO summary serializer
   [lucabel]
 - Re-add FileFieldViewModeSerializer accidentally deleted.
   [cekk]
 - Fix broken tests.
   [cekk]
 
-
 6.0.4 (2023-04-19)
 ------------------
 
 - Remove redturtle.prenotazioni integration.
   [cekk]
 - Fix syndication.
   [lucabel]
```

### Comparing `design.plone.contenttypes-6.0.6/DEVELOP.rst` & `design.plone.contenttypes-6.0.7/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/LICENSE.GPL` & `design.plone.contenttypes-6.0.7/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/LICENSE.rst` & `design.plone.contenttypes-6.0.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/PKG-INFO` & `design.plone.contenttypes-6.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.contenttypes
-Version: 6.0.6
+Version: 6.0.7
 Summary: DesignItalia contenty types
 Home-page: https://github.com/collective/design.plone.contenttypes
 Author: RedTurtle
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.contenttypes
 Project-URL: Source, https://github.com/RedTurtle/design.plone.contenttypes
@@ -484,14 +484,19 @@
 
 - RedTurtle, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
+6.0.7 (2023-05-04)
+------------------
+
+- Fix check_servizi view and made optional canale_fisico in Servizio
+  [lucabel]
 
 6.0.6 (2023-04-28)
 ------------------
 
 - Added images serialization to the summary serializer of the UO content type;
   If both the image and preview image are present, the 'image_field' attribute
   is forced to contain 'preview_image'.
@@ -506,15 +511,14 @@
   UO summary serializer
   [lucabel]
 - Re-add FileFieldViewModeSerializer accidentally deleted.
   [cekk]
 - Fix broken tests.
   [cekk]
 
-
 6.0.4 (2023-04-19)
 ------------------
 
 - Remove redturtle.prenotazioni integration.
   [cekk]
 - Fix syndication.
   [lucabel]
```

### Comparing `design.plone.contenttypes-6.0.6/README.md` & `design.plone.contenttypes-6.0.7/README.md`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/docs/conf.py` & `design.plone.contenttypes-6.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/setup.py` & `design.plone.contenttypes-6.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.contenttypes",
-    version="6.0.6",
+    version="6.0.7",
     description="DesignItalia contenty types",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
```

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/__init__.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/adapters/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/adapters/searchabletext_indexers.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/adapters/searchabletext_indexers.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/additional_help_infos.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/additional_help_infos.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/address.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/address.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/argomenti.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/argomenti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/contatti.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/contatti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/dataset_correlati.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/dataset_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/descrizione_estesa.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/descrizione_estesa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/evento.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/evento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/geolocation.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/geolocation.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/info_testata.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/info_testata.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/luoghi_correlati.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/luoghi_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/luogo.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/multi_file.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/multi_file.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/news_additional_fields.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/news_additional_fields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/servizi_correlati.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/servizi_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/show_modified.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/show_modified.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/strutture_correlate.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/strutture_correlate.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/trasparenza.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/trasparenza.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/behaviors/update_note.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/behaviors/update_note.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/change_news_type.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/change_news_type.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/check_servizi.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/check_servizi.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,28 +33,42 @@
 
 class CheckServizi(BrowserView):
     cds = None
 
     def is_anonymous(self):
         return api.user.is_anonymous()
 
+    def get_canale_accesso_info(self, servizio):
+        canale_fisico = getattr(servizio, "canale_fisico", None)
+        canale_digitale = text_in_block(getattr(servizio, "canale_digitale", None))
+        canale_digitale_link = getattr(servizio, "canale_digitale_link", None)
+        if canale_digitale and canale_digitale_link and canale_fisico:
+            return "D e F"
+        elif canale_digitale and canale_digitale_link:
+            return "D"
+        elif canale_fisico:
+            return "F"
+        # elif canale_digitale or canale_digitale_link:
+        #     return "&frac12;D"
+        return None
+
     def information_dict(self, servizio):
         return {
             "title": getattr(servizio, "title"),
             "description": getattr(servizio, "description", None),
             "condizioni_di_servizio": getattr(servizio, "condizioni_di_servizio", None),
             "tassonomia_argomenti": getattr(servizio, "tassonomia_argomenti", None),
             "a_chi_si_rivolge": text_in_block(
                 getattr(servizio, "a_chi_si_rivolge", None)
             ),
             "come_si_fa": text_in_block(getattr(servizio, "come_si_fa", None)),
             "cosa_si_ottiene": text_in_block(
                 getattr(servizio, "cosa_si_ottiene", None)
             ),
-            "canale_fisico": getattr(servizio, "canale_fisico", None),
+            "canale_accesso": self.get_canale_accesso_info(servizio),
             "cosa_serve": text_in_block(getattr(servizio, "cosa_serve", None)),
             "tempi_e_scadenze": text_in_block(
                 getattr(servizio, "tempi_e_scadenze", None)
             ),
             "ufficio_responsabile": getattr(servizio, "ufficio_responsabile", None),
         }
 
@@ -109,27 +123,25 @@
                         "a_chi_si_rivolge": information_dict.get("a_chi_si_rivolge")
                         and FLAG
                         or "",
                         "come_si_fa": information_dict.get("come_si_fa") and FLAG or "",
                         "cosa_si_ottiene": information_dict.get("cosa_si_ottiene")
                         and FLAG
                         or "",
-                        "canale_fisico": information_dict.get("canale_fisico")
-                        and FLAG
-                        or "",
+                        "canale_accesso": information_dict.get("canale_accesso") or "",
                         "cosa_serve": information_dict.get("cosa_serve") and FLAG or "",
                         "tempi_e_scadenze": information_dict.get("tempi_e_scadenze")
                         and FLAG
                         or "",
                         "ufficio_responsabile": information_dict.get(
                             "ufficio_responsabile"
                         )
                         and FLAG
                         or "",
                     },
                 }
             )
+
         results = dict(sorted(results.items()))
         for key in results:
             results[key]["children"].sort(key=lambda x: x["title"])
-
         return results
```

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/move_news_items.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/move_news_items.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/templates/check_servizi.pt` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/templates/check_servizi.pt`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 >
 
   <body>
     <metal:block fill-slot="javascript_head_slot">
 
     </metal:block>
     <metal:block fill-slot="style_slot">
-<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" integrity="sha512-iecdLmaskl7CVkqkXNQ/ZH/XLlvWZOJyj7Yy7tcenmpD1ypASozpmT/E0iPtmFIB46ZmdtAc9eNBvH0H/ZpiBw==" crossorigin="anonymous" referrerpolicy="no-referrer" />
+      <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" integrity="sha512-iecdLmaskl7CVkqkXNQ/ZH/XLlvWZOJyj7Yy7tcenmpD1ypASozpmT/E0iPtmFIB46ZmdtAc9eNBvH0H/ZpiBw==" crossorigin="anonymous" referrerpolicy="no-referrer" />
       <style>
        li.categoria{margin-bottom:2em}
        #content-header,
        #mainnavigation-wrapper,
        #above-content-wrapper{display:none}
        .container{margin-top:2em}
 
@@ -83,14 +83,23 @@
              tal:condition="servizi"
           >
                La lista seguente elenca tutti quei servizi per i quali non sono
                ancora stati aggiunti i campi che AGID indica come obbligatori.
                Ogni redattore pu&ograve; vedere in questa lista tutti i servizi e,
                cliccando su ognuno, andare alla vista di dettaglio del servizio,
             editarlo e compilare tutti i campi obbligatori.</p>
+            <p class="lead"
+             tal:condition="servizi">Per quanto riguarda la colonna <strong>canale di accesso</strong>,
+            nei servizi, abbiamo canale fisico e canale digitale. Il canale digitale,
+            è calcolato su due campi: uno testuale descrittivo e uno contenente il link per
+            l'accesso. È obbligatorio compilare o il canale fisico oppure i due campi relativi al canale
+            digitale per seguire le direttive indicate da AGID.
+            Nella tabella sotto si troverà scritto "D" nel caso nel servizio siano compilati
+            i due campi del canale digitale, "F" nel caso sia compilato il canale fisico e
+            "D e F" nel caso siano compilati tutti i campi relativi al canale di accesso.</p>
 
         <div class="forms">
           <div tal:condition="view/cds">
             <form action="${context/absolute_url}/@@check_servizi">
               <input type="Submit" value="Cerca senza condizioni di servizio" />
             </form>
           </div>
@@ -128,15 +137,15 @@
                       <th class="service_title"><span>Titolo</span></th>
                       <th><span>Descrizione</span></th>
                       <th tal:condition="view/cds"><span>Condizioni di servizio</span></th>
                       <th><span>Argomenti</span></th>
                       <th><span>A chi &egrave; rivolto</span></th>
                       <th><span>Come fare per</span></th>
                       <th><span>Cosa si ottiene</span></th>
-                      <th><span>Canale fisico</span></th>
+                      <th><span>Canale di accesso</span></th>
                       <th><span>Cosa serve</span></th>
                       <th><span>Tempi e scadenze</span></th>
                       <th><span>Unit&agrave; org. responsabile</span></th>
                       <tr>
                       </tr></tr></thead>
                   <tbody>
                     <tr tal:repeat="servizio python:servizi[categoria]['children']">
@@ -145,15 +154,15 @@
                         >${servizio/title}</a></td>
                       <td><span tal:content="structure servizio/data/description"></span></td>
                       <td tal:condition="view/cds"><span tal:content="servizio/data/condizioni_di_servizio"></span></td>
                       <td><span tal:content="structure servizio/data/tassonomia_argomenti"></span></td>
                       <td><span tal:content="structure servizio/data/a_chi_si_rivolge"></span></td>
                       <td><span tal:content="structure servizio/data/come_si_fa"></span></td>
                       <td><span tal:content="structure servizio/data/cosa_si_ottiene"></span></td>
-                      <td><span tal:content="structure servizio/data/canale_fisico"></span></td>
+                      <td><span tal:content="servizio/data/canale_accesso"></span></td>
                       <td><span tal:content="structure servizio/data/cosa_serve"></span></td>
                       <td><span tal:content="structure servizio/data/tempi_e_scadenze"></span></td>
                       <td><span tal:content="structure servizio/data/ufficio_responsabile"></span></td>
                     </tr>
                   </tbody>
                 </table>
               </tal:block>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -4,18 +4,26 @@
 Non hai i permessi per vedere questo elenco di informazioni. Se pensi che
 questo non sia corretto verifica di essere autenticato oppure rivolgiti agli
 amministratori del sito.
 La lista seguente elenca tutti quei servizi per i quali non sono ancora stati
 aggiunti i campi che AGID indica come obbligatori. Ogni redattore può vedere in
 questa lista tutti i servizi e, cliccando su ognuno, andare alla vista di
 dettaglio del servizio, editarlo e compilare tutti i campi obbligatori.
+Per quanto riguarda la colonna canale di accesso, nei servizi, abbiamo canale
+fisico e canale digitale. Il canale digitale, Ã¨ calcolato su due campi: uno
+testuale descrittivo e uno contenente il link per l'accesso. Ã obbligatorio
+compilare o il canale fisico oppure i due campi relativi al canale digitale per
+seguire le direttive indicate da AGID. Nella tabella sotto si troverÃ  scritto
+"D" nel caso nel servizio siano compilati i due campi del canale digitale, "F"
+nel caso sia compilato il canale fisico e "D e F" nel caso siano compilati
+tutti i campi relativi al canale di accesso.
 [Cerca senza condizioni di servizio]
  [Cerca con condizioni di servizio]
     * ***** ${categoria} *****
           o ** ${servizio/title} **
-                             Condizioni           A chi è Come Cosa si Canale Cosa  Tempi e  Unità org.
-      Titolo     Descrizione di         Argomenti rivolto  fare ottiene fisico serve scadenze responsabile
-                             servizio                      per
+                             Condizioni           A chi è Come Cosa si Canale  Cosa  Tempi e  Unità org.
+      Titolo     Descrizione di         Argomenti rivolto  fare ottiene di      serve scadenze responsabile
+                             servizio                      per          accesso
       $
       {servizio/
       title}
```

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/controlpanels/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/controlpanels/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/controlpanels/settings.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/controlpanels/settings.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/bando.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/document.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/document.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/documento.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/evento.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/evento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/incarico.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/incarico.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/luogo.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/notizie_e_comunicati_stampa.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/notizie_e_comunicati_stampa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/pagina_argomento.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/persona.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/pratica.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/servizio.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/events/unita_organizzativa.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/events/unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/common.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/common.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/news.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/news.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/pagina_argomento.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/persona.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/indexers/punto_di_contatto.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/indexers/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/bando.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/cartella_modulistica.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/dataset.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/dataset.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/documento.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/documento_personale.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/documento_personale.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/incarico.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/incarico.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/messaggio.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/messaggio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/pagina_argomento.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/persona.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/pratica.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/punto_di_contatto.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/servizio.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/servizio.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from collective.volto.blocksfield.field import BlocksField
 from collective.z3cform.datagridfield.datagridfield import DataGridFieldFactory
 from collective.z3cform.datagridfield.row import DictRow
 from design.plone.contenttypes import _
 from design.plone.contenttypes.interfaces import IDesignPloneContentType
 from plone.app.dexterity import textindexer
 from plone.app.z3cform.widget import DateFieldWidget
-from plone.app.z3cform.widget import RelatedItemsFieldWidget
 from plone.app.z3cform.widget import LinkFieldWidget
+from plone.app.z3cform.widget import RelatedItemsFieldWidget
 from plone.autoform import directives as form
 from plone.namedfile import field
 from plone.supermodel import model
 from z3c.relationfield.schema import RelationChoice
 from z3c.relationfield.schema import RelationList
 from zope import schema
 
@@ -173,15 +173,15 @@
     # vocabolario dalle unita' organizzative presenti a catalogo?
     canale_fisico = RelationList(
         title=_("canale_fisico", default="Canale fisico"),
         description=_(
             "canale_fisico_help",
             default="Unità organizzative per la fruizione del servizio",
         ),
-        required=True,
+        required=False,
         default=[],
         value_type=RelationChoice(
             title=_("Canale fisico"),
             vocabulary="plone.app.vocabularies.Catalog",
         ),
     )
```

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/interfaces/unita_organizzativa.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/interfaces/unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/README.rst` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/update.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/locales/update.sh` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/locales/update.sh`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/overrides.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/overrides.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/patches/__init__.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/patches/baseserializer.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/patches/baseserializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/permissions.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/permissions.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/catalog.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/controlpanel.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/diff_tool.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/diff_tool.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/metadata.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/registry/criteria.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/registry/criteria.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/registry/settings.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/registry/settings.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/repositorytool.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/repositorytool.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/rolemap.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Bando.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Bando.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Dataset.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Dataset.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Document.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Document.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Documento.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Documento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Event.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Event.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Incarico.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Incarico.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Modulo.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Modulo.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/News_Item.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/News_Item.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Persona.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Persona.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Pratica.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Pratica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Servizio.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Servizio.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types/Venue.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types/Venue.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/default/types.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/correlati.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/documento.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/dxfields.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/dxfields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/news.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/news.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/persona.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/servizio.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/deserializers/venue.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/deserializers/venue.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/bando.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/documento.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/dxcontent.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/dxcontent.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/dxfields.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/dxfields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/modulo.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/modulo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/persona.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/relationfield.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/relationfield.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/servizio.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/summary.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/summary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/serializers/venue.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/serializers/venue.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/content/add.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/content/add.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/controlpanel.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/controlpanel.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/scadenziario/post.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/scadenziario/post.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/trasparenza/get.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/trasparenza/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/services/types/get.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/services/types/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/restapi/types/adapters.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/restapi/types/adapters.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/schema_overrides.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/schema_overrides.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/setuphandlers.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/testing.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/example.pdf` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/example.pdf`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/example.png` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/example.png`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_argomenti.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_argomenti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_base_serializer.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_base_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_behavior_luogo.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_behavior_luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_behavior_show_modified.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_behavior_show_modified.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_behavior_update_note.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_behavior_update_note.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_change_news_type.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_change_news_type.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_bando.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_document.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_document.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_documento.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_documento_personale.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_documento_personale.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_event.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_event.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_luogo.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_modulo.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_modulo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_news.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_news.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_persona.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_servizio.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_filefield_view_mode_serializer.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_filefield_view_mode_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_move_news_items_view.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_move_news_items_view.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_setup.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_summary_serializer.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_summary_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/tests/test_vocabularies.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/upgrades/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/upgrades/draftjs_converter.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/upgrades/draftjs_converter.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/upgrades/to_7001.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/upgrades/to_7001.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/upgrades/to_7002.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/upgrades/to_7002.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/upgrades/upgrades.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/utils.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/utils.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/configure.zcml` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/mockup.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/mockup.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/people_vocabulary.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/people_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py` & `design.plone.contenttypes-6.0.7/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.0.6/src/design.plone.contenttypes.egg-info/PKG-INFO` & `design.plone.contenttypes-6.0.7/src/design.plone.contenttypes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.contenttypes
-Version: 6.0.6
+Version: 6.0.7
 Summary: DesignItalia contenty types
 Home-page: https://github.com/collective/design.plone.contenttypes
 Author: RedTurtle
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.contenttypes
 Project-URL: Source, https://github.com/RedTurtle/design.plone.contenttypes
@@ -484,14 +484,19 @@
 
 - RedTurtle, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
+6.0.7 (2023-05-04)
+------------------
+
+- Fix check_servizi view and made optional canale_fisico in Servizio
+  [lucabel]
 
 6.0.6 (2023-04-28)
 ------------------
 
 - Added images serialization to the summary serializer of the UO content type;
   If both the image and preview image are present, the 'image_field' attribute
   is forced to contain 'preview_image'.
@@ -506,15 +511,14 @@
   UO summary serializer
   [lucabel]
 - Re-add FileFieldViewModeSerializer accidentally deleted.
   [cekk]
 - Fix broken tests.
   [cekk]
 
-
 6.0.4 (2023-04-19)
 ------------------
 
 - Remove redturtle.prenotazioni integration.
   [cekk]
 - Fix syndication.
   [lucabel]
```

### Comparing `design.plone.contenttypes-6.0.6/src/design.plone.contenttypes.egg-info/SOURCES.txt` & `design.plone.contenttypes-6.0.7/src/design.plone.contenttypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

