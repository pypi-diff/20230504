# Comparing `tmp/fittings-2.0.4.tar.gz` & `tmp/fittings-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fittings-2.0.4.tar", last modified: Sat Apr 29 19:02:34 2023, max compression
+gzip compressed data, was "dist/fittings-2.0.5.tar", last modified: Thu May  4 21:07:38 2023, max compression
```

## Comparing `fittings-2.0.4.tar` & `fittings-2.0.5.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/
--rw-r--r--   0 root         (0) root         (0)     5574 2023-04-29 19:02:34.000000 fittings-2.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35065 2023-04-29 19:02:23.000000 fittings-2.0.4/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/auth_hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/cogs/
--rw-rw-rw-   0 root         (0) root         (0)     8423 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/cogs/fittings.py
--rw-rw-rw-   0 root         (0) root         (0)     9979 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/templates/fittings/
--rw-rw-rw-   0 root         (0) root         (0)     2414 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/edit_fit.html
--rw-rw-rw-   0 root         (0) root         (0)    35061 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/view_fit.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/templates/fittings/bundles/
--rw-rw-rw-   0 root         (0) root         (0)      357 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/bundles/multi-select-css.html
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/bundles/jquery.quicksearch-js.html
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/bundles/multi-select-js.html
--rw-rw-rw-   0 root         (0) root         (0)      359 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/bundles/slim-select-css.html
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/bundles/clipboard-js.html
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/bundles/slim-select-js.html
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/view_all_categories.html
--rw-rw-rw-   0 root         (0) root         (0)     3776 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     6546 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/view_doctrine.html
--rw-rw-rw-   0 root         (0) root         (0)     3443 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/view_all_fits.html
--rw-rw-rw-   0 root         (0) root         (0)     5848 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/edit_category.html
--rw-rw-rw-   0 root         (0) root         (0)     6015 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/add_doctrine.html
--rw-rw-rw-   0 root         (0) root         (0)     3702 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/base.html
--rw-rw-rw-   0 root         (0) root         (0)     8300 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/view_category.html
--rw-rw-rw-   0 root         (0) root         (0)     2369 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/add_fit.html
--rw-rw-rw-   0 root         (0) root         (0)     6129 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/create_category.html
--rw-rw-rw-   0 root         (0) root         (0)     6411 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templates/fittings/edit_doctrine.html
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      727 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/management/commands/fittings_preload_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/dt-i18n/
--rw-rw-rw-   0 root         (0) root         (0)     7759 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/dt-i18n/zh.json
--rw-rw-rw-   0 root         (0) root         (0)     8110 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/dt-i18n/it-IT.json
--rw-rw-rw-   0 root         (0) root         (0)     7731 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/dt-i18n/en-GB.json
--rw-rw-rw-   0 root         (0) root         (0)     8452 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/dt-i18n/fr-FR.json
--rw-rw-rw-   0 root         (0) root         (0)    10517 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/dt-i18n/ru.json
--rw-rw-rw-   0 root         (0) root         (0)     8241 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/dt-i18n/es-ES.json
--rw-rw-rw-   0 root         (0) root         (0)     2988 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/dt-i18n/ja.json
--rw-rw-rw-   0 root         (0) root         (0)     7318 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/dt-i18n/uk.json
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/dt-i18n/ko.json
--rw-rw-rw-   0 root         (0) root         (0)     8329 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/dt-i18n/de-DE.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/img/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/
--rw-rw-rw-   0 root         (0) root         (0)     8580 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/7m.png
--rw-rw-rw-   0 root         (0) root         (0)     4956 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/4m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/0l.png
--rw-rw-rw-   0 root         (0) root         (0)     5888 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/5l.png
--rw-rw-rw-   0 root         (0) root         (0)    43642 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/tyrannis.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/h.png
--rw-rw-rw-   0 root         (0) root         (0)     7439 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/6m.png
--rw-rw-rw-   0 root         (0) root         (0)     7399 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/5s.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/r.png
--rw-rw-rw-   0 root         (0) root         (0)     4607 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/3h.png
--rw-rw-rw-   0 root         (0) root         (0)     3541 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/2h.png
--rw-rw-rw-   0 root         (0) root         (0)    16840 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/circle.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/l.png
--rw-rw-rw-   0 root         (0) root         (0)     4886 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/3r.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/m.png
--rw-rw-rw-   0 root         (0) root         (0)     2766 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/2m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/0r.png
--rw-rw-rw-   0 root         (0) root         (0)     3720 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/3m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/0m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/0s.png
--rw-rw-rw-   0 root         (0) root         (0)     6109 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/5h.png
--rw-rw-rw-   0 root         (0) root         (0)     4628 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/4l.png
--rw-rw-rw-   0 root         (0) root         (0)    33523 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/dustwheel.png
--rw-rw-rw-   0 root         (0) root         (0)     8972 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/8l.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/0h.png
--rw-rw-rw-   0 root         (0) root         (0)     9490 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/4s.png
--rw-rw-rw-   0 root         (0) root         (0)     6270 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/5m.png
--rw-rw-rw-   0 root         (0) root         (0)    38343 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/tyrannis_default.png
--rw-rw-rw-   0 root         (0) root         (0)    43560 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/tyrannis_blue.png
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/working.jpg
--rw-rw-rw-   0 root         (0) root         (0)     8067 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/7l.png
--rw-rw-rw-   0 root         (0) root         (0)     2512 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/1r.png
--rw-rw-rw-   0 root         (0) root         (0)     8879 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/noship.png
--rw-rw-rw-   0 root         (0) root         (0)     1976 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/1l.png
--rw-rw-rw-   0 root         (0) root         (0)     5309 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/4h.png
--rw-rw-rw-   0 root         (0) root         (0)     8288 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/7h.png
--rw-rw-rw-   0 root         (0) root         (0)     3523 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/3l.png
--rw-rw-rw-   0 root         (0) root         (0)     7203 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/6h.png
--rw-rw-rw-   0 root         (0) root         (0)     2590 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/1h.png
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/1m.png
--rw-rw-rw-   0 root         (0) root         (0)    42868 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/tyrannis_revelations.png
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/blank.png
--rw-rw-rw-   0 root         (0) root         (0)     2570 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/2l.png
--rw-rw-rw-   0 root         (0) root         (0)     3497 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/2r.png
--rw-rw-rw-   0 root         (0) root         (0)     7014 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/6l.png
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/error.jpg
--rw-rw-rw-   0 root         (0) root         (0)    42833 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/tyrannis_darkred.png
--rw-rw-rw-   0 root         (0) root         (0)     9541 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/8m.png
--rw-rw-rw-   0 root         (0) root         (0)     9276 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/img/pannel/8h.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/ajax/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/clipboard.js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/
--rw-rw-rw-   0 root         (0) root         (0)    10753 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/clipboard.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/multi-select/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/multi-select/0.9.12/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/
--rw-rw-rw-   0 root         (0) root         (0)    19224 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/jquery.multi-select.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/
--rw-rw-rw-   0 root         (0) root         (0)     1902 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/multi-select.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/jquery.quicksearch/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    10904 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/jquery.quicksearch.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/slim-select/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/slim-select/1.26.0/
--rw-rw-rw-   0 root         (0) root         (0)     6240 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.css
--rw-rw-rw-   0 root         (0) root         (0)    35553 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.js
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6647 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/models.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/tests.py
--rw-rw-rw-   0 root         (0) root         (0)    24838 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/views.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0005_unicategory.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      750 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0003_remove_type_description_not_null.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0008_auto_20200605_0736.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0014_serverversion.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0010_auto_20200718_2227.py
--rw-rw-rw-   0 root         (0) root         (0)     6132 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0011_auto_20200815_2022.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0012_typehistory.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0013_alter_doctrine_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0007_auto_20200605_0735.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0004_add_item_category_and_group.py
--rw-rw-rw-   0 root         (0) root         (0)      718 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0009_auto_20200605_2117.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0002_add_dgm_unique_constraints.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/migrations/0006_auto_20200605_0724.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10078 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/locale/ru/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10229 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10085 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/fr_FR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/fr_FR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/locale/fr_FR/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10038 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     6341 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/locale/ja/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    13534 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5900 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    12224 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/ko_KR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/locale/ko_KR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5263 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/locale/ko_KR/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    13034 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templatetags/filters.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      684 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/templatetags/tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1409 2023-04-29 19:02:23.000000 fittings-2.0.4/fittings/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-04-29 19:02:23.000000 fittings-2.0.4/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1645 2023-04-29 19:02:23.000000 fittings-2.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5574 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6120 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 19:02:34.000000 fittings-2.0.4/fittings.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)     4554 2023-04-29 19:02:23.000000 fittings-2.0.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-29 19:02:34.000000 fittings-2.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/
+-rw-r--r--   0 root         (0) root         (0)     5574 2023-05-04 21:07:38.000000 fittings-2.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35065 2023-05-04 21:07:26.000000 fittings-2.0.5/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/auth_hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/cogs/
+-rw-rw-rw-   0 root         (0) root         (0)     8413 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/cogs/fittings.py
+-rw-rw-rw-   0 root         (0) root         (0)     9979 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/templates/fittings/
+-rw-rw-rw-   0 root         (0) root         (0)     2414 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/edit_fit.html
+-rw-rw-rw-   0 root         (0) root         (0)    35061 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/view_fit.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/templates/fittings/bundles/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/bundles/multi-select-css.html
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/bundles/jquery.quicksearch-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/bundles/multi-select-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      359 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/bundles/slim-select-css.html
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/bundles/clipboard-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/bundles/slim-select-js.html
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/view_all_categories.html
+-rw-rw-rw-   0 root         (0) root         (0)     3776 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     6546 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/view_doctrine.html
+-rw-rw-rw-   0 root         (0) root         (0)     3443 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/view_all_fits.html
+-rw-rw-rw-   0 root         (0) root         (0)     5848 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/edit_category.html
+-rw-rw-rw-   0 root         (0) root         (0)     6015 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/add_doctrine.html
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/base.html
+-rw-rw-rw-   0 root         (0) root         (0)     8300 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/view_category.html
+-rw-rw-rw-   0 root         (0) root         (0)     2369 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/add_fit.html
+-rw-rw-rw-   0 root         (0) root         (0)     6129 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/create_category.html
+-rw-rw-rw-   0 root         (0) root         (0)     6411 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templates/fittings/edit_doctrine.html
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      727 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/management/commands/fittings_preload_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/dt-i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     7759 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/dt-i18n/zh.json
+-rw-rw-rw-   0 root         (0) root         (0)     8110 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/dt-i18n/it-IT.json
+-rw-rw-rw-   0 root         (0) root         (0)     7731 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/dt-i18n/en-GB.json
+-rw-rw-rw-   0 root         (0) root         (0)     8452 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/dt-i18n/fr-FR.json
+-rw-rw-rw-   0 root         (0) root         (0)    10517 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/dt-i18n/ru.json
+-rw-rw-rw-   0 root         (0) root         (0)     8241 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/dt-i18n/es-ES.json
+-rw-rw-rw-   0 root         (0) root         (0)     2988 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/dt-i18n/ja.json
+-rw-rw-rw-   0 root         (0) root         (0)     7318 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/dt-i18n/uk.json
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/dt-i18n/ko.json
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/dt-i18n/de-DE.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/img/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/
+-rw-rw-rw-   0 root         (0) root         (0)     8580 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/7m.png
+-rw-rw-rw-   0 root         (0) root         (0)     4956 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/4m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/0l.png
+-rw-rw-rw-   0 root         (0) root         (0)     5888 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/5l.png
+-rw-rw-rw-   0 root         (0) root         (0)    43642 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/tyrannis.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/h.png
+-rw-rw-rw-   0 root         (0) root         (0)     7439 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/6m.png
+-rw-rw-rw-   0 root         (0) root         (0)     7399 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/5s.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/r.png
+-rw-rw-rw-   0 root         (0) root         (0)     4607 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/3h.png
+-rw-rw-rw-   0 root         (0) root         (0)     3541 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/2h.png
+-rw-rw-rw-   0 root         (0) root         (0)    16840 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/circle.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/l.png
+-rw-rw-rw-   0 root         (0) root         (0)     4886 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/3r.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/m.png
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/2m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/0r.png
+-rw-rw-rw-   0 root         (0) root         (0)     3720 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/3m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/0m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/0s.png
+-rw-rw-rw-   0 root         (0) root         (0)     6109 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/5h.png
+-rw-rw-rw-   0 root         (0) root         (0)     4628 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/4l.png
+-rw-rw-rw-   0 root         (0) root         (0)    33523 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/dustwheel.png
+-rw-rw-rw-   0 root         (0) root         (0)     8972 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/8l.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/0h.png
+-rw-rw-rw-   0 root         (0) root         (0)     9490 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/4s.png
+-rw-rw-rw-   0 root         (0) root         (0)     6270 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/5m.png
+-rw-rw-rw-   0 root         (0) root         (0)    38343 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/tyrannis_default.png
+-rw-rw-rw-   0 root         (0) root         (0)    43560 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/tyrannis_blue.png
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/working.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     8067 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/7l.png
+-rw-rw-rw-   0 root         (0) root         (0)     2512 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/1r.png
+-rw-rw-rw-   0 root         (0) root         (0)     8879 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/noship.png
+-rw-rw-rw-   0 root         (0) root         (0)     1976 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/1l.png
+-rw-rw-rw-   0 root         (0) root         (0)     5309 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/4h.png
+-rw-rw-rw-   0 root         (0) root         (0)     8288 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/7h.png
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/3l.png
+-rw-rw-rw-   0 root         (0) root         (0)     7203 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/6h.png
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/1h.png
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/1m.png
+-rw-rw-rw-   0 root         (0) root         (0)    42868 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/tyrannis_revelations.png
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/blank.png
+-rw-rw-rw-   0 root         (0) root         (0)     2570 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/2l.png
+-rw-rw-rw-   0 root         (0) root         (0)     3497 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/2r.png
+-rw-rw-rw-   0 root         (0) root         (0)     7014 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/6l.png
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/error.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    42833 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/tyrannis_darkred.png
+-rw-rw-rw-   0 root         (0) root         (0)     9541 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/8m.png
+-rw-rw-rw-   0 root         (0) root         (0)     9276 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/img/pannel/8h.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/ajax/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/clipboard.js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)    10753 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/clipboard.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/multi-select/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/multi-select/0.9.12/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/
+-rw-rw-rw-   0 root         (0) root         (0)    19224 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/jquery.multi-select.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/multi-select.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/jquery.quicksearch/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)    10904 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/jquery.quicksearch.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/slim-select/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/slim-select/1.26.0/
+-rw-rw-rw-   0 root         (0) root         (0)     6240 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.css
+-rw-rw-rw-   0 root         (0) root         (0)    35553 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.js
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6647 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)    24838 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0005_unicategory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      750 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0003_remove_type_description_not_null.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0008_auto_20200605_0736.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0014_serverversion.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0010_auto_20200718_2227.py
+-rw-rw-rw-   0 root         (0) root         (0)     6132 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0011_auto_20200815_2022.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0012_typehistory.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0013_alter_doctrine_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0007_auto_20200605_0735.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0004_add_item_category_and_group.py
+-rw-rw-rw-   0 root         (0) root         (0)      718 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0009_auto_20200605_2117.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0002_add_dgm_unique_constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/migrations/0006_auto_20200605_0724.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10078 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10229 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10085 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/fr_FR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/fr_FR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10038 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6341 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    13534 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5900 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    12224 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/ko_KR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/locale/ko_KR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5263 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    13034 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templatetags/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      684 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/templatetags/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2023-05-04 21:07:26.000000 fittings-2.0.5/fittings/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-05-04 21:07:26.000000 fittings-2.0.5/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1645 2023-05-04 21:07:26.000000 fittings-2.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:07:38.000000 fittings-2.0.5/fittings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5574 2023-05-04 21:07:37.000000 fittings-2.0.5/fittings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6120 2023-05-04 21:07:37.000000 fittings-2.0.5/fittings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 21:07:37.000000 fittings-2.0.5/fittings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-04 21:07:37.000000 fittings-2.0.5/fittings.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-04 21:07:37.000000 fittings-2.0.5/fittings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 21:07:37.000000 fittings-2.0.5/fittings.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)     4554 2023-05-04 21:07:26.000000 fittings-2.0.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-04 21:07:38.000000 fittings-2.0.5/setup.cfg
```

### Comparing `fittings-2.0.4/PKG-INFO` & `fittings-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fittings
-Version: 2.0.4
+Version: 2.0.5
 Summary: A simple fittings and doctrine management application.
 Home-page: https://gitlab.com/colcrunch/fittings
 Author: Col Crunch
 Author-email: it-team@serin.space
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `fittings-2.0.4/LICENSE` & `fittings-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/auth_hooks.py` & `fittings-2.0.5/fittings/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/cogs/fittings.py` & `fittings-2.0.5/fittings/cogs/fittings.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     async def fit(self, ctx, fit_name):
         """
         Returns fits and ships matching the string given
         """
         await ctx.channel.trigger_typing()
         await ctx.message.add_reaction(chr(0x231B))
 
-        fits = Fitting.objects.filter(Q(name__icontains=fit_name) | Q(ship_type__type_name__icontains=fit_name))
+        fits = Fitting.objects.filter(Q(name__icontains=fit_name) | Q(ship_type__name__icontains=fit_name))
 
         if fits.exists() is True:
             for fit in fits:
                 embed = fitting_details(fit.id)
                 await ctx.reply(embed=embed, mention_author=False)
         else:
             await ctx.reply("No Fits Found", mention_author=False)
@@ -105,15 +105,15 @@
     async def fit_ship(self, ctx, ship_name):
         """
         Returns fittings for a Ship Type
         """
         await ctx.channel.trigger_typing()
         await ctx.message.add_reaction(chr(0x231B))
 
-        fits = Fitting.objects.filter(ship_type__type_name__icontains=ship_name)
+        fits = Fitting.objects.filter(ship_type__name__icontains=ship_name)
 
         if fits.exists() is True:
             for fit in fits:
                 embed = fitting_details(fit.id)
                 await ctx.reply(embed=embed, mention_author=False)
         else:
             await ctx.reply("No Fits Found", mention_author=False)
```

### Comparing `fittings-2.0.4/fittings/tasks.py` & `fittings-2.0.5/fittings/tasks.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templates/fittings/edit_fit.html` & `fittings-2.0.5/fittings/templates/fittings/edit_fit.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templates/fittings/view_fit.html` & `fittings-2.0.5/fittings/templates/fittings/view_fit.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templates/fittings/view_all_categories.html` & `fittings-2.0.5/fittings/templates/fittings/view_all_categories.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templates/fittings/dashboard.html` & `fittings-2.0.5/fittings/templates/fittings/dashboard.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templates/fittings/view_doctrine.html` & `fittings-2.0.5/fittings/templates/fittings/view_doctrine.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templates/fittings/view_all_fits.html` & `fittings-2.0.5/fittings/templates/fittings/view_all_fits.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templates/fittings/edit_category.html` & `fittings-2.0.5/fittings/templates/fittings/edit_category.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templates/fittings/add_doctrine.html` & `fittings-2.0.5/fittings/templates/fittings/add_doctrine.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templates/fittings/base.html` & `fittings-2.0.5/fittings/templates/fittings/base.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templates/fittings/view_category.html` & `fittings-2.0.5/fittings/templates/fittings/view_category.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templates/fittings/add_fit.html` & `fittings-2.0.5/fittings/templates/fittings/add_fit.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templates/fittings/create_category.html` & `fittings-2.0.5/fittings/templates/fittings/create_category.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templates/fittings/edit_doctrine.html` & `fittings-2.0.5/fittings/templates/fittings/edit_doctrine.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/management/commands/fittings_preload_data.py` & `fittings-2.0.5/fittings/management/commands/fittings_preload_data.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/dt-i18n/zh.json` & `fittings-2.0.5/fittings/static/fittings/dt-i18n/zh.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/dt-i18n/it-IT.json` & `fittings-2.0.5/fittings/static/fittings/dt-i18n/it-IT.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/dt-i18n/en-GB.json` & `fittings-2.0.5/fittings/static/fittings/dt-i18n/en-GB.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/dt-i18n/fr-FR.json` & `fittings-2.0.5/fittings/static/fittings/dt-i18n/fr-FR.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/dt-i18n/ru.json` & `fittings-2.0.5/fittings/static/fittings/dt-i18n/ru.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/dt-i18n/es-ES.json` & `fittings-2.0.5/fittings/static/fittings/dt-i18n/es-ES.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/dt-i18n/ja.json` & `fittings-2.0.5/fittings/static/fittings/dt-i18n/ja.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/dt-i18n/uk.json` & `fittings-2.0.5/fittings/static/fittings/dt-i18n/uk.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/dt-i18n/ko.json` & `fittings-2.0.5/fittings/static/fittings/dt-i18n/ko.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/dt-i18n/de-DE.json` & `fittings-2.0.5/fittings/static/fittings/dt-i18n/de-DE.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/7m.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/7m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/4m.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/4m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/0l.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/0l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/5l.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/5l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/tyrannis.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/tyrannis.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/h.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/6m.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/6m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/5s.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/5s.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/r.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/3h.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/3h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/2h.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/2h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/circle.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/circle.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/l.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/3r.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/3r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/m.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/2m.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/2m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/0r.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/0r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/3m.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/3m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/0m.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/0m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/0s.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/0s.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/5h.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/5h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/4l.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/4l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/dustwheel.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/dustwheel.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/8l.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/8l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/0h.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/0h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/4s.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/4s.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/5m.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/5m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/tyrannis_default.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/tyrannis_default.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/tyrannis_blue.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/tyrannis_blue.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/working.jpg` & `fittings-2.0.5/fittings/static/fittings/img/pannel/working.jpg`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/7l.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/7l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/1r.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/1r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/noship.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/noship.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/1l.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/1l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/4h.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/4h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/7h.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/7h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/3l.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/3l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/6h.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/6h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/1h.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/1h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/1m.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/1m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/tyrannis_revelations.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/tyrannis_revelations.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/2l.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/2l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/2r.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/2r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/6l.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/6l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/error.jpg` & `fittings-2.0.5/fittings/static/fittings/img/pannel/error.jpg`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/tyrannis_darkred.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/tyrannis_darkred.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/8m.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/8m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/img/pannel/8h.png` & `fittings-2.0.5/fittings/static/fittings/img/pannel/8h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/clipboard.min.js` & `fittings-2.0.5/fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/jquery.multi-select.js` & `fittings-2.0.5/fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/jquery.multi-select.js`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/multi-select.min.css` & `fittings-2.0.5/fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/multi-select.min.css`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/jquery.quicksearch.min.js` & `fittings-2.0.5/fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/jquery.quicksearch.min.js`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.css` & `fittings-2.0.5/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.css`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.js` & `fittings-2.0.5/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.js`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/models.py` & `fittings-2.0.5/fittings/models.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/admin.py` & `fittings-2.0.5/fittings/admin.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/views.py` & `fittings-2.0.5/fittings/views.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/migrations/0005_unicategory.py` & `fittings-2.0.5/fittings/migrations/0005_unicategory.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py` & `fittings-2.0.5/fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py` & `fittings-2.0.5/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/migrations/0014_serverversion.py` & `fittings-2.0.5/fittings/migrations/0014_serverversion.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/migrations/0001_initial.py` & `fittings-2.0.5/fittings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/migrations/0011_auto_20200815_2022.py` & `fittings-2.0.5/fittings/migrations/0011_auto_20200815_2022.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/migrations/0012_typehistory.py` & `fittings-2.0.5/fittings/migrations/0012_typehistory.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/migrations/0007_auto_20200605_0735.py` & `fittings-2.0.5/fittings/migrations/0007_auto_20200605_0735.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/migrations/0004_add_item_category_and_group.py` & `fittings-2.0.5/fittings/migrations/0004_add_item_category_and_group.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/migrations/0009_auto_20200605_2117.py` & `fittings-2.0.5/fittings/migrations/0009_auto_20200605_2117.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/migrations/0002_add_dgm_unique_constraints.py` & `fittings-2.0.5/fittings/migrations/0002_add_dgm_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/locale/zh_Hans/LC_MESSAGES/django.po` & `fittings-2.0.5/fittings/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/locale/ru/LC_MESSAGES/django.mo` & `fittings-2.0.5/fittings/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/locale/ru/LC_MESSAGES/django.po` & `fittings-2.0.5/fittings/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/locale/es/LC_MESSAGES/django.po` & `fittings-2.0.5/fittings/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/locale/fr_FR/LC_MESSAGES/django.po` & `fittings-2.0.5/fittings/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/locale/ja/LC_MESSAGES/django.mo` & `fittings-2.0.5/fittings/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/locale/ja/LC_MESSAGES/django.po` & `fittings-2.0.5/fittings/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/locale/de/LC_MESSAGES/django.mo` & `fittings-2.0.5/fittings/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/locale/de/LC_MESSAGES/django.po` & `fittings-2.0.5/fittings/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/locale/ko_KR/LC_MESSAGES/django.mo` & `fittings-2.0.5/fittings/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/locale/ko_KR/LC_MESSAGES/django.po` & `fittings-2.0.5/fittings/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templatetags/filters.py` & `fittings-2.0.5/fittings/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/templatetags/tags.py` & `fittings-2.0.5/fittings/templatetags/tags.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings/urls.py` & `fittings-2.0.5/fittings/urls.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/setup.py` & `fittings-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/fittings.egg-info/PKG-INFO` & `fittings-2.0.5/fittings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fittings
-Version: 2.0.4
+Version: 2.0.5
 Summary: A simple fittings and doctrine management application.
 Home-page: https://gitlab.com/colcrunch/fittings
 Author: Col Crunch
 Author-email: it-team@serin.space
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `fittings-2.0.4/fittings.egg-info/SOURCES.txt` & `fittings-2.0.5/fittings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fittings-2.0.4/README.md` & `fittings-2.0.5/README.md`

 * *Files identical despite different names*

