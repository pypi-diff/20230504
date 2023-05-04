# Comparing `tmp/nautobot_firewall_models-1.2.0a2.tar.gz` & `tmp/nautobot_firewall_models-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_firewall_models-1.2.0a2.tar", max compression
+gzip compressed data, was "nautobot_firewall_models-1.2.1.tar", max compression
```

## Comparing `nautobot_firewall_models-1.2.0a2.tar` & `nautobot_firewall_models-1.2.1.tar`

### file list

```diff
@@ -1,180 +1,214 @@
--rw-r--r--   0        0        0      591 2022-12-07 20:34:54.997895 nautobot_firewall_models-1.2.0a2/LICENSE
--rw-r--r--   0        0        0     3715 2022-12-07 20:34:54.997895 nautobot_firewall_models-1.2.0a2/README.md
--rw-r--r--   0        0        0     1109 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/__init__.py
--rw-r--r--   0        0        0       59 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/api/__init__.py
--rw-r--r--   0        0        0     1252 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/api/nested_serializers.py
--rw-r--r--   0        0        0    22366 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/api/serializers.py
--rw-r--r--   0        0        0     1191 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/api/urls.py
--rw-r--r--   0        0        0     4833 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/api/views.py
--rw-r--r--   0        0        0      322 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/choices.py
--rw-r--r--   0        0        0     3487 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/constants.py
--rw-r--r--   0        0        0     1406 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/fields.py
--rw-r--r--   0        0        0     7028 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/filters.py
--rw-r--r--   0        0        0    32915 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/forms.py
--rw-r--r--   0        0        0     1994 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/homepage.py
--rw-r--r--   0        0        0     1938 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/jobs.py
--rw-r--r--   0        0        0        0 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/management/__init__.py
--rw-r--r--   0        0        0        0 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/management/commands/__init__.py
--rw-r--r--   0        0        0      867 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/management/commands/create_test_firewall_data.py
--rw-r--r--   0        0        0    43735 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0001_initial.py
--rw-r--r--   0        0        0     2610 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0002_custom_status.py
--rw-r--r--   0        0        0     5465 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0003_default_status.py
--rw-r--r--   0        0        0      551 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0004_add_description.py
--rw-r--r--   0        0        0     2019 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0005_capircapolicy.py
--rw-r--r--   0        0        0     5153 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0006_renaming_part1.py
--rw-r--r--   0        0        0     2548 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0007_renaming_part2.py
--rw-r--r--   0        0        0      874 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0008_renaming_part3.py
--rw-r--r--   0        0        0      373 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0009_proper_ordering_on_through.py
--rw-r--r--   0        0        0    33458 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0010_nat_policy.py
--rw-r--r--   0        0        0     1950 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0011_custom_status_nat.py
--rw-r--r--   0        0        0      945 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0012_remove_status_m2m_through_models.py
--rw-r--r--   0        0        0     9321 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0013_applications.py
--rw-r--r--   0        0        0     1964 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0014_custom_status_application.py
--rw-r--r--   0        0        0        0 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/__init__.py
--rw-r--r--   0        0        0      460 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/services.yml
--rw-r--r--   0        0        0     2717 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/__init__.py
--rw-r--r--   0        0        0     9303 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/address.py
--rw-r--r--   0        0        0     2201 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/capirca_policy.py
--rw-r--r--   0        0        0    20215 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/nat_policy.py
--rw-r--r--   0        0        0    14330 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/security_policy.py
--rw-r--r--   0        0        0     8207 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/service.py
--rw-r--r--   0        0        0     3288 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/user.py
--rw-r--r--   0        0        0     2413 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/zone.py
--rw-r--r--   0        0        0    10324 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/navigation.py
--rw-r--r--   0        0        0     4575 2022-12-07 20:36:23.606197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/404.html
--rw-r--r--   0        0        0    12581 2022-12-07 20:36:23.618197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/capirca.html
--rw-r--r--   0        0        0    87624 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0   129978 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/theme.css
--rw-r--r--   0        0        0     4597 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/css/theme_extra.css
--rw-r--r--   0        0        0    15635 2022-12-07 20:36:23.618197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/development.html
--rw-r--r--   0        0        0    14248 2022-12-07 20:36:23.618197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/example.html
--rw-r--r--   0        0        0      235 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/extra.css
--rw-r--r--   0        0        0    97434 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/custom-status.png
--rw-r--r--   0        0        0   380271 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/datamodel.png
--rw-r--r--   0        0        0   392814 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/existing-status.png
--rw-r--r--   0        0        0   360700 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/navmenu.png
--rw-r--r--   0        0        0   493383 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/policy.png
--rw-r--r--   0        0        0     1150 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/img/favicon.ico
--rw-r--r--   0        0        0     9818 2022-12-07 20:36:23.618197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/index.html
--rw-r--r--   0        0        0     2731 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/js/html5shiv.min.js
--rw-r--r--   0        0        0    89501 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     5075 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/js/theme.js
--rw-r--r--   0        0        0      195 2022-12-07 20:36:23.542197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/js/theme_extra.js
--rw-r--r--   0        0        0     5974 2022-12-07 20:36:23.622197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/addressobject.html
--rw-r--r--   0        0        0     5593 2022-12-07 20:36:23.622197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/addressobjectgroup.html
--rw-r--r--   0        0        0     5877 2022-12-07 20:36:23.622197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/applicationobject.html
--rw-r--r--   0        0        0     5645 2022-12-07 20:36:23.622197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/applicationobjectgroup.html
--rw-r--r--   0        0        0     5668 2022-12-07 20:36:23.622197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/fqdn.html
--rw-r--r--   0        0        0     5642 2022-12-07 20:36:23.622197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/iprange.html
--rw-r--r--   0        0        0     6147 2022-12-07 20:36:23.626197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/natpolicy.html
--rw-r--r--   0        0        0     5965 2022-12-07 20:36:23.626197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/natpolicydevicem2m.html
--rw-r--r--   0        0        0     6039 2022-12-07 20:36:23.626197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/natpolicydynamicgroupm2m.html
--rw-r--r--   0        0        0     7690 2022-12-07 20:36:23.626197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/natpolicyrule.html
--rw-r--r--   0        0        0     6600 2022-12-07 20:36:23.626197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/policy.html
--rw-r--r--   0        0        0     5917 2022-12-07 20:36:23.626197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/policydevicem2m.html
--rw-r--r--   0        0        0     5997 2022-12-07 20:36:23.626197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/policydynamicgroupm2m.html
--rw-r--r--   0        0        0     6922 2022-12-07 20:36:23.630197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/policyrule.html
--rw-r--r--   0        0        0     6104 2022-12-07 20:36:23.630197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/serviceobject.html
--rw-r--r--   0        0        0     5593 2022-12-07 20:36:23.630197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/serviceobjectgroup.html
--rw-r--r--   0        0        0     5847 2022-12-07 20:36:23.630197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/userobject.html
--rw-r--r--   0        0        0     5554 2022-12-07 20:36:23.630197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/userobjectgroup.html
--rw-r--r--   0        0        0     5540 2022-12-07 20:36:23.630197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models/zone.html
--rw-r--r--   0        0        0    32579 2022-12-07 20:36:23.618197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/models.html
--rw-r--r--   0        0        0       65 2022-12-07 20:36:23.538197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/requirements.txt
--rw-r--r--   0        0        0     5065 2022-12-07 20:36:23.610197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/sitemap.xml
--rw-r--r--   0        0        0      389 2022-12-07 20:36:23.610197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/sitemap.xml.gz
--rw-r--r--   0        0        0     6961 2022-12-07 20:36:23.622197 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/usage.html
--rw-r--r--   0        0        0    10687 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tables.py
--rw-r--r--   0        0        0     2541 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/template_content.py
--rw-r--r--   0        0        0     2216 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/addressobject.html
--rw-r--r--   0        0        0     1156 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/addressobjectgroup.html
--rw-r--r--   0        0        0     1330 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/applicationobject.html
--rw-r--r--   0        0        0      945 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/applicationobjectgroup.html
--rw-r--r--   0        0        0     1275 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/capircapolicy.html
--rw-r--r--   0        0        0     1124 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/capircapolicy_details.html
--rw-r--r--   0        0        0     1134 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/fqdn.html
--rw-r--r--   0        0        0      499 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/capirca_policy.html
--rw-r--r--   0        0        0     1382 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/device_policies.html
--rw-r--r--   0        0        0     1759 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/dynamic_group_device_policies.html
--rw-r--r--   0        0        0     1556 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/dynamic_group_policies.html
--rw-r--r--   0        0        0     1670 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_device_weight.html
--rw-r--r--   0        0        0     1724 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_dynamic_group_weight.html
--rw-r--r--   0        0        0      662 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_expanded_rules.html
--rw-r--r--   0        0        0      726 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_rule_address_object_row.html
--rw-r--r--   0        0        0       85 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_rule_mode_row.html
--rw-r--r--   0        0        0     1318 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/natpolicyrule_tablehead.html
--rw-r--r--   0        0        0     2331 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/natpolicyrule_tablerow.html
--rw-r--r--   0        0        0     1657 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_device_weight.html
--rw-r--r--   0        0        0     1711 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_dynamic_group_weight.html
--rw-r--r--   0        0        0      735 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_expanded_rules.html
--rw-r--r--   0        0        0      306 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_action_row.html
--rw-r--r--   0        0        0      789 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_address_object_row.html
--rw-r--r--   0        0        0      690 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_application_object_row.html
--rw-r--r--   0        0        0      654 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_service_object_row.html
--rw-r--r--   0        0        0      572 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_user_object_row.html
--rw-r--r--   0        0        0      248 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_zone_object_row.html
--rw-r--r--   0        0        0     1857 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rules_tablerow.html
--rw-r--r--   0        0        0      863 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policyrule_tablehead.html
--rw-r--r--   0        0        0     1652 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policyrule_tablerow.html
--rw-r--r--   0        0        0     1228 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/iprange.html
--rw-r--r--   0        0        0      272 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/natpolicy.html
--rw-r--r--   0        0        0     4384 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/natpolicy_retrieve.html
--rw-r--r--   0        0        0      276 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/natpolicyrule.html
--rw-r--r--   0        0        0     1784 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/natpolicyrule_retrieve.html
--rw-r--r--   0        0        0     4298 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/policy.html
--rw-r--r--   0        0        0     1758 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/policyrule.html
--rw-r--r--   0        0        0      988 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/serviceobject.html
--rw-r--r--   0        0        0     3619 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/serviceobject_edit.html
--rw-r--r--   0        0        0     1156 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/serviceobjectgroup.html
--rw-r--r--   0        0        0      696 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/userobject.html
--rw-r--r--   0        0        0     1148 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/userobjectgroup.html
--rw-r--r--   0        0        0     1555 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/zone.html
--rw-r--r--   0        0        0       33 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templatetags/__init__.py
--rw-r--r--   0        0        0      384 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templatetags/fw_tags.py
--rw-r--r--   0        0        0       54 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tests/__init__.py
--rw-r--r--   0        0        0    14786 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tests/fixtures.py
--rw-r--r--   0        0        0    16576 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tests/test_api.py
--rw-r--r--   0        0        0    25409 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tests/test_capirca.py
--rw-r--r--   0        0        0     1440 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tests/test_filters.py
--rw-r--r--   0        0        0    15544 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tests/test_models.py
--rw-r--r--   0        0        0    21892 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tests/test_ui_views.py
--rw-r--r--   0        0        0    20949 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/urls.py
--rw-r--r--   0        0        0     1029 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/utils/__init__.py
--rw-r--r--   0        0        0    26590 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/utils/capirca.py
--rw-r--r--   0        0        0      563 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/validators.py
--rw-r--r--   0        0        0        0 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/__init__.py
--rw-r--r--   0        0        0     1364 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/address_object.py
--rw-r--r--   0        0        0     1480 2022-12-07 20:34:55.013895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/address_object_group.py
--rw-r--r--   0        0        0     1456 2022-12-07 20:34:55.017895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/application_object.py
--rw-r--r--   0        0        0     1572 2022-12-07 20:34:55.017895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/application_object_group.py
--rw-r--r--   0        0        0     2326 2022-12-07 20:34:55.017895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/capirca_policy.py
--rw-r--r--   0        0        0     1156 2022-12-07 20:34:55.017895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/fqdn.py
--rw-r--r--   0        0        0     1226 2022-12-07 20:34:55.017895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/iprange.py
--rw-r--r--   0        0        0     4238 2022-12-07 20:34:55.017895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/nat_policy.py
--rw-r--r--   0        0        0     1260 2022-12-07 20:34:55.017895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/nat_policy_rule.py
--rw-r--r--   0        0        0     3415 2022-12-07 20:34:55.017895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/policy.py
--rw-r--r--   0        0        0     1302 2022-12-07 20:34:55.017895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/policy_rule.py
--rw-r--r--   0        0        0     1435 2022-12-07 20:34:55.017895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/service_object.py
--rw-r--r--   0        0        0     1480 2022-12-07 20:34:55.017895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/service_object_group.py
--rw-r--r--   0        0        0     1295 2022-12-07 20:34:55.017895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/user_object.py
--rw-r--r--   0        0        0     1411 2022-12-07 20:34:55.017895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/user_object_group.py
--rw-r--r--   0        0        0     1156 2022-12-07 20:34:55.017895 nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/zone.py
--rw-r--r--   0        0        0     3220 2022-12-07 20:35:03.693934 nautobot_firewall_models-1.2.0a2/pyproject.toml
--rw-r--r--   0        0        0     5692 1970-01-01 00:00:00.000000 nautobot_firewall_models-1.2.0a2/setup.py
--rw-r--r--   0        0        0     4715 1970-01-01 00:00:00.000000 nautobot_firewall_models-1.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-05-04 19:33:28.284027 nautobot_firewall_models-1.2.1/LICENSE
+-rw-r--r--   0        0        0     4121 2023-05-04 19:33:28.284027 nautobot_firewall_models-1.2.1/README.md
+-rw-r--r--   0        0        0     1228 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/api/__init__.py
+-rw-r--r--   0        0        0     1564 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/api/nested_serializers.py
+-rw-r--r--   0        0        0    22500 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/api/serializers.py
+-rw-r--r--   0        0        0     1191 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/api/urls.py
+-rw-r--r--   0        0        0     4833 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/api/views.py
+-rw-r--r--   0        0        0      322 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/choices.py
+-rw-r--r--   0        0        0     3487 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/constants.py
+-rw-r--r--   0        0        0     1406 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/fields.py
+-rw-r--r--   0        0        0     7044 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/filters.py
+-rw-r--r--   0        0        0    32931 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/forms.py
+-rw-r--r--   0        0        0     1994 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/homepage.py
+-rw-r--r--   0        0        0     1938 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/jobs.py
+-rw-r--r--   0        0        0        0 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/management/commands/__init__.py
+-rw-r--r--   0        0        0      867 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/management/commands/create_test_firewall_data.py
+-rw-r--r--   0        0        0    43735 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2610 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0002_custom_status.py
+-rw-r--r--   0        0        0     5465 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0003_default_status.py
+-rw-r--r--   0        0        0      551 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0004_add_description.py
+-rw-r--r--   0        0        0     2019 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0005_capircapolicy.py
+-rw-r--r--   0        0        0     5153 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0006_renaming_part1.py
+-rw-r--r--   0        0        0     2548 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0007_renaming_part2.py
+-rw-r--r--   0        0        0      874 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0008_renaming_part3.py
+-rw-r--r--   0        0        0      373 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0009_proper_ordering_on_through.py
+-rw-r--r--   0        0        0    33458 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0010_nat_policy.py
+-rw-r--r--   0        0        0     1950 2023-05-04 19:33:28.300027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0011_custom_status_nat.py
+-rw-r--r--   0        0        0      945 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0012_remove_status_m2m_through_models.py
+-rw-r--r--   0        0        0     9321 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0013_applications.py
+-rw-r--r--   0        0        0     1964 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0014_custom_status_application.py
+-rw-r--r--   0        0        0      709 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0015_alter_capircapolicy_device.py
+-rw-r--r--   0        0        0        0 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/__init__.py
+-rw-r--r--   0        0        0      460 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/services.yml
+-rw-r--r--   0        0        0     2717 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/__init__.py
+-rw-r--r--   0        0        0     9303 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/address.py
+-rw-r--r--   0        0        0     2246 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/capirca_policy.py
+-rw-r--r--   0        0        0    20215 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/nat_policy.py
+-rw-r--r--   0        0        0    14330 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/security_policy.py
+-rw-r--r--   0        0        0     8207 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/service.py
+-rw-r--r--   0        0        0     3288 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/user.py
+-rw-r--r--   0        0        0     2413 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/zone.py
+-rw-r--r--   0        0        0    10324 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/navigation.py
+-rw-r--r--   0        0        0    30920 2023-05-04 19:34:23.812520 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/404.html
+-rw-r--r--   0        0        0    32387 2023-05-04 19:34:23.848520 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/admin/compatibility_matrix.html
+-rw-r--r--   0        0        0    41274 2023-05-04 19:34:23.856521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/admin/install.html
+-rw-r--r--   0        0        0    32052 2023-05-04 19:34:23.868521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/admin/release_notes/index.html
+-rw-r--r--   0        0        0    39770 2023-05-04 19:34:23.876520 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/admin/release_notes/version_0.1.html
+-rw-r--r--   0        0        0    38567 2023-05-04 19:34:23.880521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/admin/release_notes/version_1.0.html
+-rw-r--r--   0        0        0    39977 2023-05-04 19:34:23.884521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/admin/release_notes/version_1.1.html
+-rw-r--r--   0        0        0    42293 2023-05-04 19:34:23.892521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/admin/release_notes/version_1.2.html
+-rw-r--r--   0        0        0    34131 2023-05-04 19:34:23.860520 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/admin/uninstall.html
+-rw-r--r--   0        0        0    33524 2023-05-04 19:34:23.864520 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/admin/upgrade.html
+-rw-r--r--   0        0        0        0 2023-05-04 19:34:23.564518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     4805 2023-05-04 19:34:23.564518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/extra.css
+-rw-r--r--   0        0        0    15086 2023-05-04 19:34:23.564518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     1870 2023-05-04 19:34:23.568518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0   112874 2023-05-04 19:34:23.568518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/bundle.9c69f0bc.min.js
+-rw-r--r--   0        0        0   597452 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/bundle.9c69f0bc.min.js.map
+-rw-r--r--   0        0        0    17058 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0    11232 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0      817 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     3647 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2023-05-04 19:34:23.572518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     1031 2023-05-04 19:34:23.576518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2023-05-04 19:34:23.576518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2023-05-04 19:34:23.576518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2057 2023-05-04 19:34:23.576518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2023-05-04 19:34:23.576518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677455 2023-05-04 19:34:23.576518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    36472 2023-05-04 19:34:23.576518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/workers/search.ecf98df9.min.js
+-rw-r--r--   0        0        0   181894 2023-05-04 19:34:23.576518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/javascripts/workers/search.ecf98df9.min.js.map
+-rw-r--r--   0        0        0     9204 2023-05-04 19:34:23.564518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/nautobot_logo.png
+-rw-r--r--   0        0        0    13318 2023-05-04 19:34:23.564518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/nautobot_logo.svg
+-rw-r--r--   0        0        0     7562 2023-05-04 19:34:23.564518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/networktocode_bw.png
+-rw-r--r--   0        0        0      846 2023-05-04 19:34:23.564518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/overrides/partials/copyright.html
+-rw-r--r--   0        0        0   138680 2023-05-04 19:34:23.576518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/stylesheets/main.69437709.min.css
+-rw-r--r--   0        0        0    47242 2023-05-04 19:34:23.576518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/stylesheets/main.69437709.min.css.map
+-rw-r--r--   0        0        0    12495 2023-05-04 19:34:23.576518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/stylesheets/palette.cbb835fc.min.css
+-rw-r--r--   0        0        0     3519 2023-05-04 19:34:23.576518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/assets/stylesheets/palette.cbb835fc.min.css.map
+-rw-r--r--   0        0        0    33124 2023-05-04 19:34:23.896521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/contributing.html
+-rw-r--r--   0        0        0    87424 2023-05-04 19:34:23.920521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/dev_environment.html
+-rw-r--r--   0        0        0    32241 2023-05-04 19:34:23.924521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/extending.html
+-rw-r--r--   0        0        0    31638 2023-05-04 19:34:23.944521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/addressobject.html
+-rw-r--r--   0        0        0    31247 2023-05-04 19:34:23.948521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/addressobjectgroup.html
+-rw-r--r--   0        0        0    31533 2023-05-04 19:34:23.952521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/applicationobject.html
+-rw-r--r--   0        0        0    31291 2023-05-04 19:34:23.956521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/applicationobjectgroup.html
+-rw-r--r--   0        0        0    31350 2023-05-04 19:34:23.960521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/fqdn.html
+-rw-r--r--   0        0        0    31318 2023-05-04 19:34:23.964521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/iprange.html
+-rw-r--r--   0        0        0    31819 2023-05-04 19:34:23.968521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/natpolicy.html
+-rw-r--r--   0        0        0    31619 2023-05-04 19:34:23.972521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/natpolicydevicem2m.html
+-rw-r--r--   0        0        0    31681 2023-05-04 19:34:23.980522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/natpolicydynamicgroupm2m.html
+-rw-r--r--   0        0        0    33878 2023-05-04 19:34:23.984521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/natpolicyrule.html
+-rw-r--r--   0        0        0    32716 2023-05-04 19:34:23.988521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/policy.html
+-rw-r--r--   0        0        0    31577 2023-05-04 19:34:23.992522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/policydevicem2m.html
+-rw-r--r--   0        0        0    31645 2023-05-04 19:34:23.996522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/policydynamicgroupm2m.html
+-rw-r--r--   0        0        0    32796 2023-05-04 19:34:24.000522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/policyrule.html
+-rw-r--r--   0        0        0    31768 2023-05-04 19:34:24.008522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/serviceobject.html
+-rw-r--r--   0        0        0    31247 2023-05-04 19:34:24.012522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/serviceobjectgroup.html
+-rw-r--r--   0        0        0    31517 2023-05-04 19:34:24.016522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/userobject.html
+-rw-r--r--   0        0        0    31214 2023-05-04 19:34:24.020522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/userobjectgroup.html
+-rw-r--r--   0        0        0    31222 2023-05-04 19:34:24.024522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models/zone.html
+-rw-r--r--   0        0        0    71125 2023-05-04 19:34:23.940521 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/dev/models.html
+-rw-r--r--   0        0        0    97434 2023-05-04 19:34:23.568518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/custom-status.png
+-rw-r--r--   0        0        0   380271 2023-05-04 19:34:23.568518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/datamodel.png
+-rw-r--r--   0        0        0   392814 2023-05-04 19:34:23.568518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/existing-status.png
+-rw-r--r--   0        0        0    24753 2023-05-04 19:34:23.568518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/icon-nautobot-firewall-models.png
+-rw-r--r--   0        0        0   360700 2023-05-04 19:34:23.568518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/navmenu.png
+-rw-r--r--   0        0        0   493383 2023-05-04 19:34:23.568518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/policy.png
+-rw-r--r--   0        0        0    39235 2023-05-04 19:34:23.844520 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/index.html
+-rw-r--r--   0        0        0      155 2023-05-04 19:34:23.564518 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/requirements.txt
+-rw-r--r--   0        0        0   153603 2023-05-04 19:34:24.080522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/search/search_index.json
+-rw-r--r--   0        0        0     8252 2023-05-04 19:34:23.816520 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/sitemap.xml
+-rw-r--r--   0        0        0      522 2023-05-04 19:34:23.816520 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/sitemap.xml.gz
+-rw-r--r--   0        0        0    33730 2023-05-04 19:34:24.028522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/user/app_getting_started.html
+-rw-r--r--   0        0        0    35743 2023-05-04 19:34:24.032522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/user/app_overview.html
+-rw-r--r--   0        0        0    36325 2023-05-04 19:34:24.040522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/user/app_use_cases.html
+-rw-r--r--   0        0        0    42523 2023-05-04 19:34:24.048522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/user/capirca.html
+-rw-r--r--   0        0        0    76387 2023-05-04 19:34:24.072522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/user/external_interactions.html
+-rw-r--r--   0        0        0    32097 2023-05-04 19:34:24.080522 nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/user/faq.html
+-rw-r--r--   0        0        0    10687 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/tables.py
+-rw-r--r--   0        0        0     2541 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/template_content.py
+-rw-r--r--   0        0        0     2216 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/addressobject.html
+-rw-r--r--   0        0        0     1156 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/addressobjectgroup.html
+-rw-r--r--   0        0        0     1330 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/applicationobject.html
+-rw-r--r--   0        0        0      945 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/applicationobjectgroup.html
+-rw-r--r--   0        0        0     1275 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/capircapolicy.html
+-rw-r--r--   0        0        0     1124 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/capircapolicy_details.html
+-rw-r--r--   0        0        0     1134 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/fqdn.html
+-rw-r--r--   0        0        0      499 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/capirca_policy.html
+-rw-r--r--   0        0        0     1382 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/device_policies.html
+-rw-r--r--   0        0        0     1759 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/dynamic_group_device_policies.html
+-rw-r--r--   0        0        0     1556 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/dynamic_group_policies.html
+-rw-r--r--   0        0        0     1670 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_device_weight.html
+-rw-r--r--   0        0        0     1724 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_dynamic_group_weight.html
+-rw-r--r--   0        0        0      662 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_expanded_rules.html
+-rw-r--r--   0        0        0      726 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_rule_address_object_row.html
+-rw-r--r--   0        0        0       85 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_rule_mode_row.html
+-rw-r--r--   0        0        0     1318 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/natpolicyrule_tablehead.html
+-rw-r--r--   0        0        0     2331 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/natpolicyrule_tablerow.html
+-rw-r--r--   0        0        0     1657 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_device_weight.html
+-rw-r--r--   0        0        0     1711 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_dynamic_group_weight.html
+-rw-r--r--   0        0        0      735 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_expanded_rules.html
+-rw-r--r--   0        0        0      306 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_action_row.html
+-rw-r--r--   0        0        0      789 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_address_object_row.html
+-rw-r--r--   0        0        0      690 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_application_object_row.html
+-rw-r--r--   0        0        0      654 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_service_object_row.html
+-rw-r--r--   0        0        0      572 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_user_object_row.html
+-rw-r--r--   0        0        0      248 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_zone_object_row.html
+-rw-r--r--   0        0        0     1857 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rules_tablerow.html
+-rw-r--r--   0        0        0      863 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policyrule_tablehead.html
+-rw-r--r--   0        0        0     1652 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policyrule_tablerow.html
+-rw-r--r--   0        0        0     1228 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/iprange.html
+-rw-r--r--   0        0        0      272 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/natpolicy.html
+-rw-r--r--   0        0        0     4384 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/natpolicy_retrieve.html
+-rw-r--r--   0        0        0      276 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/natpolicyrule.html
+-rw-r--r--   0        0        0     1784 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/natpolicyrule_retrieve.html
+-rw-r--r--   0        0        0     4298 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/policy.html
+-rw-r--r--   0        0        0     1758 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/policyrule.html
+-rw-r--r--   0        0        0      988 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/serviceobject.html
+-rw-r--r--   0        0        0     3619 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/serviceobject_edit.html
+-rw-r--r--   0        0        0     1156 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/serviceobjectgroup.html
+-rw-r--r--   0        0        0      696 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/userobject.html
+-rw-r--r--   0        0        0     1148 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/userobjectgroup.html
+-rw-r--r--   0        0        0     1555 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/zone.html
+-rw-r--r--   0        0        0       33 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templatetags/__init__.py
+-rw-r--r--   0        0        0      384 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/templatetags/fw_tags.py
+-rw-r--r--   0        0        0       54 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/tests/__init__.py
+-rw-r--r--   0        0        0    15163 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/tests/fixtures.py
+-rw-r--r--   0        0        0    16852 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/tests/test_api.py
+-rw-r--r--   0        0        0     1529 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/tests/test_basic.py
+-rw-r--r--   0        0        0    25409 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/tests/test_capirca.py
+-rw-r--r--   0        0        0     1440 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/tests/test_filters.py
+-rw-r--r--   0        0        0    15544 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/tests/test_models.py
+-rw-r--r--   0        0        0    21902 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/tests/test_ui_views.py
+-rw-r--r--   0        0        0    20949 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/urls.py
+-rw-r--r--   0        0        0     1029 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/utils/__init__.py
+-rw-r--r--   0        0        0    26590 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/utils/capirca.py
+-rw-r--r--   0        0        0      563 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/validators.py
+-rw-r--r--   0        0        0        0 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/__init__.py
+-rw-r--r--   0        0        0     1364 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/address_object.py
+-rw-r--r--   0        0        0     1480 2023-05-04 19:33:28.304027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/address_object_group.py
+-rw-r--r--   0        0        0     1456 2023-05-04 19:33:28.308027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/application_object.py
+-rw-r--r--   0        0        0     1572 2023-05-04 19:33:28.308027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/application_object_group.py
+-rw-r--r--   0        0        0     2326 2023-05-04 19:33:28.308027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/capirca_policy.py
+-rw-r--r--   0        0        0     1156 2023-05-04 19:33:28.308027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/fqdn.py
+-rw-r--r--   0        0        0     1226 2023-05-04 19:33:28.308027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/iprange.py
+-rw-r--r--   0        0        0     4238 2023-05-04 19:33:28.308027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/nat_policy.py
+-rw-r--r--   0        0        0     1260 2023-05-04 19:33:28.308027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/nat_policy_rule.py
+-rw-r--r--   0        0        0     3415 2023-05-04 19:33:28.308027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/policy.py
+-rw-r--r--   0        0        0     1302 2023-05-04 19:33:28.308027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/policy_rule.py
+-rw-r--r--   0        0        0     1435 2023-05-04 19:33:28.308027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/service_object.py
+-rw-r--r--   0        0        0     1480 2023-05-04 19:33:28.308027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/service_object_group.py
+-rw-r--r--   0        0        0     1295 2023-05-04 19:33:28.308027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/user_object.py
+-rw-r--r--   0        0        0     1411 2023-05-04 19:33:28.308027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/user_object_group.py
+-rw-r--r--   0        0        0     1156 2023-05-04 19:33:28.308027 nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/zone.py
+-rw-r--r--   0        0        0     3528 2023-05-04 19:33:44.876179 nautobot_firewall_models-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5120 1970-01-01 00:00:00.000000 nautobot_firewall_models-1.2.1/PKG-INFO
```

### Comparing `nautobot_firewall_models-1.2.0a2/LICENSE` & `nautobot_firewall_models-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/__init__.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from nautobot.extras.plugins import PluginConfig
 
 
 class NautobotFirewallModelsConfig(PluginConfig):
     """Plugin configuration for the nautobot_firewall_models plugin."""
 
     name = "nautobot_firewall_models"
-    verbose_name = "Nautobot Plugin Firewall Model"
+    verbose_name = "Firewall & Security Models"
     version = __version__
     author = "Network to Code, LLC"
-    description = "Nautobot plugin to model firewall objects.."
+    description = "Nautobot App to model firewall and security objects. Allows users to model policies in a vendor-neutral manner and use that data to drive network security automation."
     base_url = "firewall"
     required_settings = []
     min_version = "1.4.0"
     max_version = "1.9999"
     default_settings = {"capirca_remark_pass": True, "capirca_os_map": {}, "allowed_status": ["active"]}
     caching_config = {"*": {"timeout": 0}}
     docs_view_name = "plugins:nautobot_firewall_models:docs"
```

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/api/nested_serializers.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/api/nested_serializers.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,7 +37,19 @@
     end_address = CharField()
 
     class Meta:
         """Meta attributes."""
 
         model = models.IPRange
         fields = ["id", "url", "start_address", "end_address"]
+
+
+class NestedZoneSerializer(WritableNestedSerializer):
+    """Nested serializer for Zone."""
+
+    url = HyperlinkedIdentityField(view_name="plugins-api:nautobot_firewall_models-api:zone-detail")
+
+    class Meta:
+        """Meta attributes."""
+
+        model = models.Zone
+        fields = ["id", "url", "name"]
```

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/api/serializers.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/api/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """API serializers for firewall models."""
 
 from rest_framework import serializers
 
 from nautobot.core.api import ValidatedModelSerializer, SerializedPKRelatedField
 from nautobot.dcim.api.nested_serializers import NestedInterfaceSerializer
-from nautobot.dcim.models import Device
+from nautobot.dcim.models import Device, Interface
 from nautobot.extras.api.customfields import CustomFieldModelSerializer
 from nautobot.extras.api.fields import StatusSerializerField
 from nautobot.extras.api.serializers import (
     StatusModelSerializerMixin as _StatusModelSerializerMixin,
     TaggedObjectSerializer,
     NautobotModelSerializer,
 )
@@ -18,14 +18,15 @@
 
 
 from nautobot_firewall_models import models
 from nautobot_firewall_models.api.nested_serializers import (
     NestedFQDNSerializer,
     NestedIPRangeSerializer,
     # NestedApplicationSerializer,
+    NestedZoneSerializer,
 )
 
 
 class StatusModelSerializerMixin(_StatusModelSerializerMixin):  # pylint: disable=abstract-method
     """Overloaded mixing to set status to optional.
 
     Args:
@@ -195,15 +196,17 @@
         fields = "__all__"
 
 
 class ZoneSerializer(TaggedObjectSerializer, StatusModelSerializerMixin, NautobotModelSerializer):
     """Zone Serializer."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_firewall_models-api:zone-detail")
-    interfaces = NestedInterfaceSerializer(required=False, many=True)
+    interfaces = SerializedPKRelatedField(
+        queryset=Interface.objects.all(), serializer=NestedInterfaceSerializer, required=False, many=True
+    )
 
     class Meta:
         """Meta attributes."""
 
         model = models.Zone
         fields = "__all__"
 
@@ -223,25 +226,25 @@
     )
     source_address_groups = SerializedPKRelatedField(
         queryset=models.AddressObjectGroup.objects.all(),
         serializer=AddressObjectGroupSerializer,
         required=False,
         many=True,
     )
-    source_zone = ZoneSerializer(required=False)
+    source_zone = NestedZoneSerializer(required=False)
     destination_addresses = SerializedPKRelatedField(
         queryset=models.AddressObject.objects.all(), serializer=AddressObjectSerializer, required=False, many=True
     )
     destination_address_groups = SerializedPKRelatedField(
         queryset=models.AddressObjectGroup.objects.all(),
         serializer=AddressObjectGroupSerializer,
         required=False,
         many=True,
     )
-    destination_zone = ZoneSerializer(required=False)
+    destination_zone = NestedZoneSerializer(required=False)
     destination_services = SerializedPKRelatedField(
         queryset=models.ServiceObject.objects.all(), serializer=ServiceObjectSerializer, required=False, many=True
     )
     destination_service_groups = SerializedPKRelatedField(
         queryset=models.ServiceObjectGroup.objects.all(),
         serializer=ServiceObjectGroupSerializer,
         required=False,
```

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/api/urls.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/api/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/api/views.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/api/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/constants.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/constants.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/fields.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/fields.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/filters.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     """Filter for ApplicationObject."""
 
     class Meta:
         """Meta attributes for filter."""
 
         model = models.ApplicationObject
 
-        fields = ["id", "name", "description", "category", "subcategory", "risk", "description"]
+        fields = ["id", "name", "description", "category", "subcategory", "risk"]
 
 
 class ApplicationObjectGroupFilterSet(BaseFilterSet, NautobotFilterSet):
     """Filter for ApplicationObjectGroup."""
 
     class Meta:
         """Meta attributes for filter."""
@@ -171,15 +171,15 @@
             Q(name__icontains=value) | Q(description__icontains=value) | Q(request_id__icontains=value)
         )
 
     class Meta:
         """Meta attributes for filter."""
 
         model = models.PolicyRule
-        fields = ["id", "action", "log", "request_id"]
+        fields = ["id", "action", "log", "request_id", "description", "name"]
 
 
 # TODO: Refactor to allow for better filtering, currently very limited.
 class NATPolicyRuleFilterSet(BaseFilterSet, NautobotFilterSet):
     """Filter for NATPolicyRule."""
 
     tag = TagFilter()
@@ -197,15 +197,15 @@
             Q(name__icontains=value) | Q(description__icontains=value) | Q(request_id__icontains=value)
         )
 
     class Meta:
         """Meta attributes for filter."""
 
         model = models.NATPolicyRule
-        fields = ["id", "remark", "log", "request_id"]
+        fields = ["id", "remark", "log", "request_id", "name"]
 
 
 class PolicyFilterSet(BaseFilterSet, NautobotFilterSet):
     """Filter for Policy."""
 
     class Meta:
         """Meta attributes for filter."""
```

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/forms.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
     )
     name = forms.CharField(required=False, label="Name")
 
 
 class AddressObjectGroupForm(LocalContextModelForm, NautobotModelForm):
     """AddressObjectGroup creation/edit form."""
 
-    address_objects = DynamicModelMultipleChoiceField(queryset=models.AddressObject.objects.all())
+    address_objects = DynamicModelMultipleChoiceField(queryset=models.AddressObject.objects.all(), required=False)
 
     class Meta:
         """Meta attributes."""
 
         model = models.AddressObjectGroup
         fields = ["name", "description", "address_objects", "status", "tags"]
```

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/homepage.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/homepage.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/jobs.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/management/commands/create_test_firewall_data.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/management/commands/create_test_firewall_data.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0001_initial.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0002_custom_status.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0002_custom_status.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0003_default_status.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0003_default_status.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0004_add_description.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0004_add_description.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0005_capircapolicy.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0005_capircapolicy.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0006_renaming_part1.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0006_renaming_part1.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0007_renaming_part2.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0007_renaming_part2.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0008_renaming_part3.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0008_renaming_part3.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0010_nat_policy.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0010_nat_policy.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0011_custom_status_nat.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0011_custom_status_nat.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0012_remove_status_m2m_through_models.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0012_remove_status_m2m_through_models.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0013_applications.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0013_applications.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/migrations/0014_custom_status_application.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/migrations/0014_custom_status_application.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/__init__.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/address.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/address.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/capirca_policy.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/capirca_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,17 @@
     "relationships",
     "statuses",
     "webhooks",
 )
 class CapircaPolicy(PrimaryModel):
     """CapircaPolicy model."""
 
-    device = models.OneToOneField(to="dcim.Device", blank=True, null=True, on_delete=models.CASCADE)
+    device = models.OneToOneField(
+        to="dcim.Device", blank=True, null=True, on_delete=models.CASCADE, related_name="capirca_policy"
+    )
     pol = models.TextField(blank=True, null=True)
     net = models.TextField(blank=True, null=True)
     svc = models.TextField(blank=True, null=True)
     cfg = models.TextField(blank=True, null=True)
 
     csv_headers = ["device"]
```

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/nat_policy.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/nat_policy.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/security_policy.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/security_policy.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/service.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/service.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/user.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/user.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/models/zone.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/models/zone.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/navigation.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/navigation.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/custom-status.png` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/custom-status.png`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/datamodel.png` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/datamodel.png`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/existing-status.png` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/existing-status.png`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/navmenu.png` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/navmenu.png`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/policy.png` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/static/nautobot_firewall_models/docs/images/policy.png`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tables.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/tables.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/template_content.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/addressobject.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/addressobject.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/addressobjectgroup.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/addressobjectgroup.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/applicationobject.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/applicationobject.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/applicationobjectgroup.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/applicationobjectgroup.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/capircapolicy.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/capircapolicy.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/capircapolicy_details.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/capircapolicy_details.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/fqdn.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/fqdn.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/device_policies.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/device_policies.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/dynamic_group_device_policies.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/dynamic_group_device_policies.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/dynamic_group_policies.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/dynamic_group_policies.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_device_weight.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_device_weight.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_dynamic_group_weight.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_dynamic_group_weight.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_expanded_rules.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_expanded_rules.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_rule_address_object_row.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/nat_policy_rule_address_object_row.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/natpolicyrule_tablehead.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/natpolicyrule_tablehead.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/natpolicyrule_tablerow.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/natpolicyrule_tablerow.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_device_weight.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_device_weight.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_dynamic_group_weight.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_dynamic_group_weight.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_expanded_rules.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_expanded_rules.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_address_object_row.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_address_object_row.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_application_object_row.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_application_object_row.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_service_object_row.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_service_object_row.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_user_object_row.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rule_user_object_row.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rules_tablerow.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policy_rules_tablerow.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policyrule_tablehead.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policyrule_tablehead.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policyrule_tablerow.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/inc/policyrule_tablerow.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/iprange.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/iprange.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/natpolicy_retrieve.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/natpolicy_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/natpolicyrule_retrieve.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/natpolicyrule_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/policy.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/policy.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/policyrule.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/policyrule.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/serviceobject.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/serviceobject.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/serviceobject_edit.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/serviceobject_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/serviceobjectgroup.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/serviceobjectgroup.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/userobject.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/userobject.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/userobjectgroup.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/userobjectgroup.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/templates/nautobot_firewall_models/zone.html` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/templates/nautobot_firewall_models/zone.html`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tests/fixtures.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/tests/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,42 +79,51 @@
         name="app1",
         category="web",
         subcategory="streaming",
         default_type="443",
         default_ip_protocol="TCP",
         status=status,
         risk=3,
+        description="some description",
     )
     app2 = ApplicationObject.objects.create(
         name="app2",
         category="web",
         subcategory="streaming",
         default_type="443",
         default_ip_protocol="TCP",
         status=status,
         risk=2,
+        description="some description",
     )
     app3 = ApplicationObject.objects.create(
         name="app3",
         category="web",
         subcategory="streaming",
         default_type="443",
         default_ip_protocol="TCP",
         status=status,
         risk=1,
+        description="some description",
     )
-    app_grp1 = ApplicationObjectGroup.objects.create(name="streaming")
+    app_grp1 = ApplicationObjectGroup.objects.create(name="streaming", description="some description")
     app_grp1.application_objects.set([app1])
-    app_grp2 = ApplicationObjectGroup.objects.create(name="gaming")
+    app_grp2 = ApplicationObjectGroup.objects.create(name="gaming", description="some description")
     app_grp2.application_objects.set([app3, app2])
-    app_grp3 = ApplicationObjectGroup.objects.create(name="news")
+    app_grp3 = ApplicationObjectGroup.objects.create(name="news", description="some description")
     app_grp3.application_objects.set([app1, app2, app3])
 
     pol_rule1 = PolicyRule.objects.create(
-        action="deny", log=True, name="Policy Rule 1", status=status, request_id="req1", index=10
+        action="deny",
+        log=True,
+        name="Policy Rule 1",
+        status=status,
+        request_id="req1",
+        index=10,
+        description="some description",
     )
     pol_rule1.source_users.set([usr_obj1])
     pol_rule1.source_user_groups.set([usr_grp1])
     pol_rule1.source_addresses.set([addr_obj1])
     pol_rule1.source_address_groups.set([addr_grp1])
     pol_rule1.source_services.set([src_svc])
     pol_rule1.destination_addresses.set([addr_obj4])
@@ -128,14 +137,15 @@
         destination_zone=zone2,
         action="allow",
         log=True,
         name="Policy Rule 2",
         status=status,
         request_id="req2",
         index=20,
+        description="some description",
     )
     pol_rule2.source_users.set([usr_obj1, usr_obj2])
     pol_rule2.source_user_groups.set([usr_grp1, usr_grp2])
     pol_rule2.source_addresses.set([addr_obj1, addr_obj2])
     pol_rule2.source_address_groups.set([addr_grp1, addr_grp2])
     pol_rule2.destination_addresses.set([addr_obj4])
     pol_rule2.destination_address_groups.set([addr_grp3])
@@ -148,14 +158,15 @@
         destination_zone=zone2,
         action="drop",
         log=True,
         name="Policy Rule 3",
         status=status,
         request_id="req3",
         index=30,
+        description="some description",
     )
     pol_rule3.source_users.set([usr_obj1, usr_obj2, usr_obj3])
     pol_rule3.source_user_groups.set([usr_grp1, usr_grp2, usr_grp3])
     pol_rule3.source_addresses.set([addr_obj1, addr_obj2, addr_obj3])
     pol_rule3.source_address_groups.set([addr_grp1, addr_grp2])
     pol_rule3.destination_addresses.set([addr_obj4])
     pol_rule3.destination_address_groups.set([addr_grp3])
```

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tests/test_api.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/tests/test_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -114,14 +114,18 @@
     def test_bulk_delete_objects(self):
         pass
 
     @skip("on_delete set to PROTECT")
     def test_delete_object_without_permission(self):
         pass
 
+    @skip("Incompatible with nested serializer starting in 1.5.18")
+    def test_update_object(self):
+        pass
+
 
 class AddressObjectAPIViewTest(APIViewTestCases.APIViewTestCase):
     """Test the AddressObject viewsets."""
 
     model = models.AddressObject
     bulk_update_data = {"description": "test update description"}
 
@@ -183,22 +187,22 @@
     def test_bulk_delete_objects(self):
         pass
 
     @skip("on_delete set to PROTECT")
     def test_delete_object_without_permission(self):
         pass
 
+    @skip("Incompatible with nested serializer starting in 1.5.18")
+    def test_update_object(self):
+        pass
+
     def test_create_object(self):
         self.validation_excluded_fields = ["address_objects"]
         return super().test_create_object()
 
-    def test_update_object(self):
-        self.validation_excluded_fields = ["address_objects"]
-        return super().test_update_object()
-
     def test_bulk_create_objects(self):
         self.validation_excluded_fields = ["address_objects"]
         return super().test_bulk_create_objects()
 
 
 class ServiceObjectAPIViewTest(APIViewTestCases.APIViewTestCase):
     """Test the ServiceObject viewsets."""
@@ -263,22 +267,22 @@
     def test_bulk_delete_objects(self):
         pass
 
     @skip("on_delete set to PROTECT")
     def test_delete_object_without_permission(self):
         pass
 
+    @skip("Incompatible with nested serializer starting in 1.5.18")
+    def test_update_object(self):
+        pass
+
     def test_create_object(self):
         self.validation_excluded_fields = ["service_objects"]
         return super().test_create_object()
 
-    def test_update_object(self):
-        self.validation_excluded_fields = ["service_objects"]
-        return super().test_update_object()
-
     def test_bulk_create_objects(self):
         self.validation_excluded_fields = ["service_objects"]
         return super().test_bulk_create_objects()
 
 
 class UserObjectAPIViewTest(APIViewTestCases.APIViewTestCase):
     """Test the User viewsets."""
@@ -342,22 +346,22 @@
     def test_bulk_delete_objects(self):
         pass
 
     @skip("on_delete set to PROTECT")
     def test_delete_object_without_permission(self):
         pass
 
+    @skip("Incompatible with nested serializer starting in 1.5.18")
+    def test_update_object(self):
+        pass
+
     def test_create_object(self):
         self.validation_excluded_fields = ["user_objects"]
         return super().test_create_object()
 
-    def test_update_object(self):
-        self.validation_excluded_fields = ["user_objects"]
-        return super().test_update_object()
-
     def test_bulk_create_objects(self):
         self.validation_excluded_fields = ["user_objects"]
         return super().test_bulk_create_objects()
 
 
 class ZoneAPIViewTest(APIViewTestCases.APIViewTestCase):
     """Test the Zone viewsets."""
@@ -441,14 +445,18 @@
     def test_bulk_delete_objects(self):
         pass
 
     @skip("on_delete set to PROTECT")
     def test_delete_object_without_permission(self):
         pass
 
+    @skip("Incompatible with nested serializer starting in 1.5.18")
+    def test_update_object(self):
+        pass
+
 
 class PolicyAPIViewTest(APIViewTestCases.APIViewTestCase):
     """Test the Policy viewsets."""
 
     model = models.Policy
     bulk_update_data = {"description": "test update description"}
 
@@ -537,14 +545,18 @@
     def test_bulk_delete_objects(self):
         pass
 
     @skip("on_delete set to PROTECT")
     def test_delete_object_without_permission(self):
         pass
 
+    @skip("Incompatible with nested serializer starting in 1.5.18")
+    def test_update_object(self):
+        pass
+
 
 class NATPolicyAPIViewTest(APIViewTestCases.APIViewTestCase):
     """Test the Policy viewsets."""
 
     model = models.NATPolicy
     bulk_update_data = {"description": "test update description"}
```

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tests/test_capirca.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/tests/test_capirca.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tests/test_filters.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tests/test_models.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/tests/test_ui_views.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/tests/test_ui_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         pass
 
 
 class ApplicationObjectUIViewTest(ViewTestCases.PrimaryObjectViewTestCase):
     """Test the ApplicationObject viewsets."""
 
     model = ApplicationObject
-    bulk_edit_data = {"description": "test update description"}
+    bulk_edit_data = {"description": "bulk test update description"}
 
     @classmethod
     def setUpTestData(cls):
         """Create test data for API calls."""
         create_env()
 
         status = Status.objects.get(slug="active").id
@@ -622,15 +622,15 @@
         pass
 
 
 class PolicyRuleUIViewTest(ViewTestCases.PrimaryObjectViewTestCase):
     """Test the PolicyRule viewsets."""
 
     model = PolicyRule
-    bulk_edit_data = {"description": "test update description"}
+    bulk_edit_data = {"description": "bulk test update description"}
 
     @classmethod
     def setUpTestData(cls):
         """Create test data for API calls."""
         create_env()
         src_usr = UserObject.objects.first()
         src_addr = AddressObject.objects.first()
```

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/urls.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/utils/__init__.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/utils/capirca.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/utils/capirca.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/validators.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/validators.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/address_object.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/address_object.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/address_object_group.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/address_object_group.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/application_object.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/application_object.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/application_object_group.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/application_object_group.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/capirca_policy.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/capirca_policy.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/fqdn.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/fqdn.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/iprange.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/iprange.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/nat_policy.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/nat_policy.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/nat_policy_rule.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/nat_policy_rule.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/policy.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/policy.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/policy_rule.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/policy_rule.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/service_object.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/service_object.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/service_object_group.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/service_object_group.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/user_object.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/user_object.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/user_object_group.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/user_object_group.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/nautobot_firewall_models/views/zone.py` & `nautobot_firewall_models-1.2.1/nautobot_firewall_models/views/zone.py`

 * *Files identical despite different names*

### Comparing `nautobot_firewall_models-1.2.0a2/pyproject.toml` & `nautobot_firewall_models-1.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-firewall-models"
-version = "v1.2.0-alpha.2"
+version = "v1.2.1"
 description = "Nautobot plugin to model firewall objects."
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-firewall-models"
 repository = "https://github.com/nautobot/nautobot-plugin-firewall-models"
 keywords = ["nautobot", "nautobot-plugin"]
@@ -26,28 +26,37 @@
 capirca = "^2.0.6"
 
 [tool.poetry.dev-dependencies]
 bandit = "*"
 black = "*"
 coverage = "*"
 django-debug-toolbar = "*"
-# we need to pin flake8 because of package dependencies that cause it to downgrade and 
+# we need to pin flake8 because of package dependencies that cause it to downgrade and
 # therefore cause issues with linting since older versions do not take .flake8 as config
 flake8 = "^3.9.2"
 invoke = "*"
 ipython = "*"
-mkdocs = "*"
-mkdocs-include-markdown-plugin = "*"
 pydocstyle = "*"
 pylint = "*"
 pylint-django = "*"
 pytest = "*"
 yamllint = "*"
 Markdown = "*"
 toml = "*"
+# Rendering docs to HTML
+mkdocs = "1.3.1"
+# Markdown include plugin
+mkdocs-include-markdown-plugin = "3.9.1"
+# Material for MkDocs theme
+mkdocs-material = "8.4.2"
+# Render custom markdown for version added/changed/remove notes
+mkdocs-version-annotations = "1.0.0"
+# Automatic documentation from sources, for MkDocs
+mkdocstrings = "0.19"
+mkdocstrings-python = "0.7.1"
 
 [tool.poetry.extras]
 nautobot = ["nautobot"]
 
 [tool.black]
 line-length = 120
 target-version = ['py37']
```

### Comparing `nautobot_firewall_models-1.2.0a2/PKG-INFO` & `nautobot_firewall_models-1.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,295 +1,320 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e61 7574  : 2.1.Name: naut
 00000020: 6f62 6f74 2d66 6972 6577 616c 6c2d 6d6f  obot-firewall-mo
 00000030: 6465 6c73 0a56 6572 7369 6f6e 3a20 312e  dels.Version: 1.
-00000040: 322e 3061 320a 5375 6d6d 6172 793a 204e  2.0a2.Summary: N
-00000050: 6175 746f 626f 7420 706c 7567 696e 2074  autobot plugin t
-00000060: 6f20 6d6f 6465 6c20 6669 7265 7761 6c6c  o model firewall
-00000070: 206f 626a 6563 7473 2e0a 486f 6d65 2d70   objects..Home-p
-00000080: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
-00000090: 6875 622e 636f 6d2f 6e61 7574 6f62 6f74  hub.com/nautobot
-000000a0: 2f6e 6175 746f 626f 742d 706c 7567 696e  /nautobot-plugin
-000000b0: 2d66 6972 6577 616c 6c2d 6d6f 6465 6c73  -firewall-models
-000000c0: 0a4c 6963 656e 7365 3a20 4170 6163 6865  .License: Apache
-000000d0: 2d32 2e30 0a4b 6579 776f 7264 733a 206e  -2.0.Keywords: n
-000000e0: 6175 746f 626f 742c 6e61 7574 6f62 6f74  autobot,nautobot
-000000f0: 2d70 6c75 6769 6e0a 4175 7468 6f72 3a20  -plugin.Author: 
-00000100: 4e65 7477 6f72 6b20 746f 2043 6f64 652c  Network to Code,
-00000110: 204c 4c43 0a41 7574 686f 722d 656d 6169   LLC.Author-emai
-00000120: 6c3a 2069 6e66 6f40 6e65 7477 6f72 6b74  l: info@networkt
-00000130: 6f63 6f64 652e 636f 6d0a 5265 7175 6972  ocode.com.Requir
-00000140: 6573 2d50 7974 686f 6e3a 203e 3d33 2e37  es-Python: >=3.7
-00000150: 2c3c 342e 300a 436c 6173 7369 6669 6572  ,<4.0.Classifier
-00000160: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
-00000170: 2041 7070 726f 7665 6420 3a3a 2041 7061   Approved :: Apa
-00000180: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
-00000190: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
-000001a0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000001b0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001c0: 3a3a 2033 0a43 6c61 7373 6966 6965 723a  :: 3.Classifier:
-000001d0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000001e0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001f0: 3a3a 2033 2e37 0a43 6c61 7373 6966 6965  :: 3.7.Classifie
-00000200: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000210: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000220: 6e20 3a3a 2033 2e38 0a43 6c61 7373 6966  n :: 3.8.Classif
-00000230: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000240: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000250: 686f 6e20 3a3a 2033 2e39 0a43 6c61 7373  hon :: 3.9.Class
-00000260: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000270: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000280: 7974 686f 6e20 3a3a 2033 2e31 300a 436c  ython :: 3.10.Cl
-00000290: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000002a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002b0: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
-000002c0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-000002d0: 206e 6175 746f 626f 740a 5265 7175 6972   nautobot.Requir
-000002e0: 6573 2d44 6973 743a 2063 6170 6972 6361  es-Dist: capirca
-000002f0: 2028 3e3d 322e 302e 362c 3c33 2e30 2e30   (>=2.0.6,<3.0.0
-00000300: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000310: 206e 6175 746f 626f 7420 283e 3d31 2e34   nautobot (>=1.4
-00000320: 2e30 2c3c 322e 302e 3029 3b20 6578 7472  .0,<2.0.0); extr
-00000330: 6120 3d3d 2022 6e61 7574 6f62 6f74 220a  a == "nautobot".
-00000340: 5265 7175 6972 6573 2d44 6973 743a 206e  Requires-Dist: n
-00000350: 6574 7574 696c 7320 283e 3d31 2e30 2e30  etutils (>=1.0.0
-00000360: 2c3c 322e 302e 3029 0a50 726f 6a65 6374  ,<2.0.0).Project
-00000370: 2d55 524c 3a20 5265 706f 7369 746f 7279  -URL: Repository
-00000380: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-00000390: 2e63 6f6d 2f6e 6175 746f 626f 742f 6e61  .com/nautobot/na
-000003a0: 7574 6f62 6f74 2d70 6c75 6769 6e2d 6669  utobot-plugin-fi
-000003b0: 7265 7761 6c6c 2d6d 6f64 656c 730a 4465  rewall-models.De
-000003c0: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
-000003d0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
-000003e0: 6b64 6f77 6e0a 0a23 204e 6175 746f 626f  kdown..# Nautobo
-000003f0: 7420 4669 7265 7761 6c6c 204d 6f64 656c  t Firewall Model
-00000400: 7320 506c 7567 696e 0a0a 4120 706c 7567  s Plugin..A plug
-00000410: 696e 2066 6f72 205b 4e61 7574 6f62 6f74  in for [Nautobot
-00000420: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000430: 2e63 6f6d 2f6e 6175 746f 626f 742f 6e61  .com/nautobot/na
-00000440: 7574 6f62 6f74 2920 7468 6174 2069 7320  utobot) that is 
-00000450: 6d65 616e 7420 746f 206d 6f64 656c 206c  meant to model l
-00000460: 6179 6572 2034 2066 6972 6577 616c 6c20  ayer 4 firewall 
-00000470: 706f 6c69 6369 6573 2061 6e64 2f6f 7220  policies and/or 
-00000480: 6578 7465 6e64 6564 2061 6363 6573 7320  extended access 
-00000490: 636f 6e74 726f 6c20 6c69 7374 732e 200a  control lists. .
-000004a0: 0a46 7574 7572 6520 6465 7665 6c6f 706d  .Future developm
-000004b0: 656e 7420 7769 6c6c 2069 6e63 6c75 6465  ent will include
-000004c0: 2074 6865 2061 6269 6c69 7479 2074 6f20   the ability to 
-000004d0: 6f6e 626f 6172 6420 616e 2065 7869 7374  onboard an exist
-000004e0: 696e 6720 6163 6365 7373 206c 6973 7420  ing access list 
-000004f0: 6672 6f6d 2061 2064 6576 6963 6520 616e  from a device an
-00000500: 6420 7468 6520 6162 696c 6974 7920 746f  d the ability to
-00000510: 2067 656e 6572 6174 6520 6465 7669 6365   generate device
-00000520: 2063 6f6e 6669 6775 7261 7469 6f6e 2e0a   configuration..
-00000530: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-00000540: 0a0a 5468 6520 706c 7567 696e 2069 7320  ..The plugin is 
-00000550: 6176 6169 6c61 626c 6520 6173 2061 2050  available as a P
-00000560: 7974 686f 6e20 7061 636b 6167 6520 696e  ython package in
-00000570: 2050 7950 4920 616e 6420 6361 6e20 6265   PyPI and can be
-00000580: 2069 6e73 7461 6c6c 6564 2077 6974 6820   installed with 
-00000590: 6070 6970 603a 0a0a 6060 6073 6865 6c6c  `pip`:..```shell
-000005a0: 0a70 6970 2069 6e73 7461 6c6c 206e 6175  .pip install nau
-000005b0: 746f 626f 742d 6669 7265 7761 6c6c 2d6d  tobot-firewall-m
-000005c0: 6f64 656c 730a 6060 600a 0a3e 2054 6865  odels.```..> The
-000005d0: 2070 6c75 6769 6e20 6973 2063 6f6d 7061   plugin is compa
-000005e0: 7469 626c 6520 7769 7468 204e 6175 746f  tible with Nauto
-000005f0: 626f 7420 312e 342e 3020 616e 6420 6869  bot 1.4.0 and hi
-00000600: 6768 6572 0a0a 546f 2065 6e73 7572 6520  gher..To ensure 
-00000610: 4e61 7574 6f62 6f74 2046 6972 6577 616c  Nautobot Firewal
-00000620: 6c20 4d6f 6465 6c73 2050 6c75 6769 6e20  l Models Plugin 
-00000630: 6973 2061 7574 6f6d 6174 6963 616c 6c79  is automatically
-00000640: 2072 652d 696e 7374 616c 6c65 6420 6475   re-installed du
-00000650: 7269 6e67 2066 7574 7572 6520 7570 6772  ring future upgr
-00000660: 6164 6573 2c20 6372 6561 7465 2061 2066  ades, create a f
-00000670: 696c 6520 6e61 6d65 6420 606c 6f63 616c  ile named `local
-00000680: 5f72 6571 7569 7265 6d65 6e74 732e 7478  _requirements.tx
-00000690: 7460 2028 6966 206e 6f74 2061 6c72 6561  t` (if not alrea
-000006a0: 6479 2065 7869 7374 696e 6729 2069 6e20  dy existing) in 
-000006b0: 7468 6520 4e61 7574 6f62 6f74 2072 6f6f  the Nautobot roo
-000006c0: 7420 6469 7265 6374 6f72 7920 2861 6c6f  t directory (alo
-000006d0: 6e67 7369 6465 2060 7265 7175 6972 656d  ngside `requirem
-000006e0: 656e 7473 2e74 7874 6029 2061 6e64 206c  ents.txt`) and l
-000006f0: 6973 7420 7468 6520 606e 6175 746f 626f  ist the `nautobo
-00000700: 742d 6669 7265 7761 6c6c 2d6d 6f64 656c  t-firewall-model
-00000710: 7360 2070 6163 6b61 6765 3a0a 0a60 6060  s` package:..```
-00000720: 6e6f 2d68 6967 686c 6967 6874 0a23 2065  no-highlight.# e
-00000730: 6368 6f20 6e61 7574 6f62 6f74 2d66 6972  cho nautobot-fir
-00000740: 6577 616c 6c2d 6d6f 6465 6c73 203e 3e20  ewall-models >> 
-00000750: 6c6f 6361 6c5f 7265 7175 6972 656d 656e  local_requiremen
-00000760: 7473 2e74 7874 0a60 6060 0a0a 4f6e 6365  ts.txt.```..Once
-00000770: 2069 6e73 7461 6c6c 6564 2c20 7468 6520   installed, the 
-00000780: 706c 7567 696e 206e 6565 6473 2074 6f20  plugin needs to 
-00000790: 6265 2065 6e61 626c 6564 2069 6e20 796f  be enabled in yo
-000007a0: 7572 2060 6e61 7574 6f62 6f74 5f63 6f6e  ur `nautobot_con
-000007b0: 6669 672e 7079 600a 0a60 6060 7079 7468  fig.py`..```pyth
-000007c0: 6f6e 0a23 2049 6e20 796f 7572 206e 6175  on.# In your nau
-000007d0: 746f 626f 745f 636f 6e66 6967 2e70 790a  tobot_config.py.
-000007e0: 504c 5547 494e 5320 3d20 5b22 6e61 7574  PLUGINS = ["naut
-000007f0: 6f62 6f74 5f66 6972 6577 616c 6c5f 6d6f  obot_firewall_mo
-00000800: 6465 6c73 225d 0a60 6060 0a0a 2323 204f  dels"].```..## O
-00000810: 7074 696f 6e61 6c20 5365 7474 696e 6773  ptional Settings
-00000820: 0a0a 4d6f 6465 6c73 2070 726f 7669 6465  ..Models provide
-00000830: 6420 6279 2074 6869 7320 706c 7567 696e  d by this plugin
-00000840: 2068 6176 6520 6120 6073 7461 7475 7360   have a `status`
-00000850: 2061 7474 7269 6275 7465 2061 6e64 2074   attribute and t
-00000860: 6865 2064 6566 6175 6c74 2060 7374 6174  he default `stat
-00000870: 7573 6020 6973 2073 6574 2074 6f20 7573  us` is set to us
-00000880: 6520 6061 6374 6976 6560 2e20 5468 6973  e `active`. This
-00000890: 2063 6f72 7265 7370 6f6e 6473 2074 6f20   corresponds to 
-000008a0: 7468 6520 7072 652d 6275 696c 7420 4e61  the pre-built Na
-000008b0: 7574 6f62 6f74 2060 4163 7469 7665 6020  utobot `Active` 
-000008c0: 5374 6174 7573 206f 626a 6563 742e 0a0a  Status object...
-000008d0: 5573 6520 7468 6520 6064 6566 6175 6c74  Use the `default
-000008e0: 5f73 7461 7475 7360 2070 6c75 6769 6e20  _status` plugin 
-000008f0: 636f 6e66 6967 7572 6174 696f 6e20 7365  configuration se
-00000900: 7474 696e 6720 746f 2063 6861 6e67 6520  tting to change 
-00000910: 7468 6520 6465 6661 756c 7420 7661 6c75  the default valu
-00000920: 6520 666f 7220 7468 6520 6073 7461 7475  e for the `statu
-00000930: 7360 2061 7474 7269 6275 7465 2e0a 0a60  s` attribute...`
-00000940: 6060 7079 7468 6f6e 0a50 4c55 4749 4e53  ``python.PLUGINS
-00000950: 5f43 4f4e 4649 4720 3d20 7b0a 2020 2020  _CONFIG = {.    
-00000960: 226e 6175 746f 626f 745f 6669 7265 7761  "nautobot_firewa
-00000970: 6c6c 5f6d 6f64 656c 7322 3a20 7b0a 2020  ll_models": {.  
-00000980: 2020 2020 2020 2264 6566 6175 6c74 5f73        "default_s
-00000990: 7461 7475 7322 3a20 2261 6374 6976 6522  tatus": "active"
-000009a0: 0a20 2020 2020 2020 2022 616c 6c6f 7765  .        "allowe
-000009b0: 645f 7374 6174 7573 223a 205b 2261 6374  d_status": ["act
-000009c0: 6976 6522 5d2c 2023 2064 6566 6175 6c74  ive"], # default
-000009d0: 2073 686f 776e 2c20 605b 5d60 2061 6c6c   shown, `[]` all
-000009e0: 6f77 7320 616c 6c0a 2020 2020 2020 2020  ows all.        
-000009f0: 2263 6170 6972 6361 5f72 656d 6172 6b5f  "capirca_remark_
-00000a00: 7061 7373 223a 2054 7275 652c 0a20 2020  pass": True,.   
-00000a10: 2020 2020 2022 6361 7069 7263 615f 6f73       "capirca_os
-00000a20: 5f6d 6170 223a 207b 0a20 2020 2020 2020  _map": {.       
-00000a30: 2020 2020 2022 6369 7363 6f5f 696f 7322       "cisco_ios"
-00000a40: 3a20 2263 6973 636f 222c 0a20 2020 2020  : "cisco",.     
-00000a50: 2020 2020 2020 2022 6172 6973 7461 5f65         "arista_e
-00000a60: 6f73 223a 2022 6172 6973 7461 222c 0a20  os": "arista",. 
-00000a70: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00000a80: 2020 2320 2263 7573 746f 6d5f 6361 7069    # "custom_capi
-00000a90: 7263 6122 3a20 226d 792e 6375 7374 6f6d  rca": "my.custom
-00000aa0: 2e66 756e 6322 2c20 2320 7072 6f76 6964  .func", # provid
-00000ab0: 6573 2061 6269 6c69 7479 2074 6f20 6f76  es ability to ov
-00000ac0: 6572 6964 6520 6361 7069 7263 6120 6c6f  eride capirca lo
-00000ad0: 6769 630a 2020 2020 7d0a 7d0a 6060 600a  gic.    }.}.```.
-00000ae0: 0a54 6865 2076 616c 7565 2061 7373 6967  .The value assig
-00000af0: 6e65 6420 746f 2060 6465 6661 756c 745f  ned to `default_
-00000b00: 7374 6174 7573 6020 6d75 7374 206d 6174  status` must mat
-00000b10: 6368 2074 6865 2073 6c75 6720 6f66 2061  ch the slug of a
-00000b20: 6e20 6578 6973 7469 6e67 204e 6175 746f  n existing Nauto
-00000b30: 626f 7420 5374 6174 7573 206f 626a 6563  bot Status objec
-00000b40: 742e 2054 6861 7420 5374 6174 7573 206f  t. That Status o
-00000b50: 626a 6563 7420 6d75 7374 2068 6176 6520  bject must have 
-00000b60: 616c 6c20 6f66 2074 6865 2046 6972 6577  all of the Firew
-00000b70: 616c 6c20 4d6f 6465 6c73 206c 6973 7465  all Models liste
-00000b80: 6420 696e 2074 6865 2043 6f6e 7465 6e74  d in the Content
-00000b90: 2054 7970 6520 6173 736f 6369 6174 696f   Type associatio
-00000ba0: 6e73 2e20 5365 6520 6578 616d 706c 6573  ns. See examples
-00000bb0: 2062 656c 6f77 206f 6e20 7365 6c65 6374   below on select
-00000bc0: 696e 6720 7468 6520 436f 6e74 656e 7420  ing the Content 
-00000bd0: 5479 7065 2873 2920 7768 656e 2063 7265  Type(s) when cre
-00000be0: 6174 696e 672f 6564 6974 696e 6720 6120  ating/editing a 
-00000bf0: 5374 6174 7573 206f 626a 6563 7420 616e  Status object an
-00000c00: 6420 7468 6520 7072 652d 6275 696c 7420  d the pre-built 
-00000c10: 6041 6374 6976 6560 2053 7461 7475 7320  `Active` Status 
-00000c20: 7769 7468 2066 6972 6577 616c 6c20 636f  with firewall co
-00000c30: 6e74 656e 7420 7479 7065 7320 6164 6465  ntent types adde
-00000c40: 642e 0a0a 215b 4375 7374 6f6d 2053 7461  d...![Custom Sta
-00000c50: 7475 735d 2868 7474 7073 3a2f 2f72 6177  tus](https://raw
-00000c60: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000c70: 6e74 2e63 6f6d 2f6e 6175 746f 626f 742f  nt.com/nautobot/
-00000c80: 6e61 7574 6f62 6f74 2d70 6c75 6769 6e2d  nautobot-plugin-
-00000c90: 6669 7265 7761 6c6c 2d6d 6f64 656c 732f  firewall-models/
-00000ca0: 6465 7665 6c6f 702f 646f 6373 2f69 6d61  develop/docs/ima
-00000cb0: 6765 732f 6375 7374 6f6d 2d73 7461 7475  ges/custom-statu
-00000cc0: 732e 706e 6720 2243 7573 746f 6d20 5374  s.png "Custom St
-00000cd0: 6174 7573 2229 0a21 5b45 7869 7374 696e  atus").![Existin
-00000ce0: 6720 5374 6174 7573 5d28 6874 7470 733a  g Status](https:
-00000cf0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00000d00: 636f 6e74 656e 742e 636f 6d2f 6e61 7574  content.com/naut
-00000d10: 6f62 6f74 2f6e 6175 746f 626f 742d 706c  obot/nautobot-pl
-00000d20: 7567 696e 2d66 6972 6577 616c 6c2d 6d6f  ugin-firewall-mo
-00000d30: 6465 6c73 2f64 6576 656c 6f70 2f64 6f63  dels/develop/doc
-00000d40: 732f 696d 6167 6573 2f65 7869 7374 696e  s/images/existin
-00000d50: 672d 7374 6174 7573 2e70 6e67 2022 4578  g-status.png "Ex
-00000d60: 6973 7469 6e67 2053 7461 7475 7322 290a  isting Status").
-00000d70: 0a23 2320 5363 7265 656e 7368 6f74 730a  .## Screenshots.
-00000d80: 0a21 5b4e 6176 6967 6174 696f 6e20 4d65  .![Navigation Me
-00000d90: 6e75 5d28 6874 7470 733a 2f2f 7261 772e  nu](https://raw.
-00000da0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00000db0: 742e 636f 6d2f 6e61 7574 6f62 6f74 2f6e  t.com/nautobot/n
-00000dc0: 6175 746f 626f 742d 706c 7567 696e 2d66  autobot-plugin-f
-00000dd0: 6972 6577 616c 6c2d 6d6f 6465 6c73 2f64  irewall-models/d
-00000de0: 6576 656c 6f70 2f64 6f63 732f 696d 6167  evelop/docs/imag
-00000df0: 6573 2f6e 6176 6d65 6e75 2e70 6e67 2022  es/navmenu.png "
-00000e00: 4e61 7669 6761 7469 6f6e 204d 656e 7522  Navigation Menu"
-00000e10: 290a 215b 506f 6c69 6379 2056 6965 775d  ).![Policy View]
-00000e20: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
-00000e30: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000e40: 6f6d 2f6e 6175 746f 626f 742f 6e61 7574  om/nautobot/naut
-00000e50: 6f62 6f74 2d70 6c75 6769 6e2d 6669 7265  obot-plugin-fire
-00000e60: 7761 6c6c 2d6d 6f64 656c 732f 6465 7665  wall-models/deve
-00000e70: 6c6f 702f 646f 6373 2f69 6d61 6765 732f  lop/docs/images/
-00000e80: 706f 6c69 6379 2e70 6e67 2022 506f 6c69  policy.png "Poli
-00000e90: 6379 2056 6965 7722 290a 0a23 2320 446f  cy View")..## Do
-00000ea0: 6375 6d65 6e74 6174 696f 6e0a 0a44 6f63  cumentation..Doc
-00000eb0: 756d 656e 7461 7469 6f6e 2069 7320 686f  umentation is ho
-00000ec0: 7374 6564 206f 6e20 5265 6164 5468 6544  sted on ReadTheD
-00000ed0: 6f63 7320 6174 205b 4e61 7574 6f62 6f74  ocs at [Nautobot
-00000ee0: 2046 6972 6577 616c 6c20 4d6f 6465 6c73   Firewall Models
-00000ef0: 2050 6c75 6769 6e5d 2868 7474 7073 3a2f   Plugin](https:/
-00000f00: 2f6e 6175 746f 626f 742d 706c 7567 696e  /nautobot-plugin
-00000f10: 2d66 6972 6577 616c 6c2d 6d6f 6465 6c73  -firewall-models
-00000f20: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00000f30: 292e 0a0a 2323 2043 6f6e 7472 6962 7574  )...## Contribut
-00000f40: 696e 670a 0a50 756c 6c20 7265 7175 6573  ing..Pull reques
-00000f50: 7473 2061 7265 2077 656c 636f 6d65 6420  ts are welcomed 
-00000f60: 616e 6420 6175 746f 6d61 7469 6361 6c6c  and automaticall
-00000f70: 7920 6275 696c 7420 616e 6420 7465 7374  y built and test
-00000f80: 6564 2061 6761 696e 7374 206d 756c 7469  ed against multi
-00000f90: 706c 6520 7665 7273 696f 6e20 6f66 2050  ple version of P
-00000fa0: 7974 686f 6e20 616e 6420 6d75 6c74 6970  ython and multip
-00000fb0: 6c65 2076 6572 7369 6f6e 206f 6620 4e61  le version of Na
-00000fc0: 7574 6f62 6f74 2074 6872 6f75 6768 2054  utobot through T
-00000fd0: 7261 7669 7343 492e 0a0a 5468 6520 7072  ravisCI...The pr
-00000fe0: 6f6a 6563 7420 6973 2070 6163 6b61 6765  oject is package
-00000ff0: 6420 7769 7468 2061 206c 6967 6874 2064  d with a light d
-00001000: 6576 656c 6f70 6d65 6e74 2065 6e76 6972  evelopment envir
-00001010: 6f6e 6d65 6e74 2062 6173 6564 206f 6e20  onment based on 
-00001020: 6064 6f63 6b65 722d 636f 6d70 6f73 6560  `docker-compose`
-00001030: 2074 6f20 6865 6c70 2077 6974 6820 7468   to help with th
-00001040: 6520 6c6f 6361 6c20 6465 7665 6c6f 706d  e local developm
-00001050: 656e 7420 6f66 2074 6865 2070 726f 6a65  ent of the proje
-00001060: 6374 2061 6e64 2074 6f20 7275 6e20 7468  ct and to run th
-00001070: 6520 7465 7374 7320 7769 7468 696e 2054  e tests within T
-00001080: 7261 7669 7343 492e 0a0a 5468 6520 7072  ravisCI...The pr
-00001090: 6f6a 6563 7420 6973 2066 6f6c 6c6f 7769  oject is followi
-000010a0: 6e67 204e 6574 776f 726b 2074 6f20 436f  ng Network to Co
-000010b0: 6465 2073 6f66 7477 6172 6520 6465 7665  de software deve
-000010c0: 6c6f 706d 656e 7420 6775 6964 656c 696e  lopment guidelin
-000010d0: 6520 616e 6420 6973 206c 6576 6572 6167  e and is leverag
-000010e0: 696e 673a 0a0a 2d20 426c 6163 6b2c 2050  ing:..- Black, P
-000010f0: 796c 696e 742c 2042 616e 6469 7420 616e  ylint, Bandit an
-00001100: 6420 7079 646f 6373 7479 6c65 2066 6f72  d pydocstyle for
-00001110: 2050 7974 686f 6e20 6c69 6e74 696e 6720   Python linting 
-00001120: 616e 6420 666f 726d 6174 7469 6e67 2e0a  and formatting..
-00001130: 2d20 446a 616e 676f 2075 6e69 7420 7465  - Django unit te
-00001140: 7374 2074 6f20 656e 7375 7265 2074 6865  st to ensure the
-00001150: 2070 6c75 6769 6e20 6973 2077 6f72 6b69   plugin is worki
-00001160: 6e67 2070 726f 7065 726c 792e 0a0a 2323  ng properly...##
-00001170: 2051 7565 7374 696f 6e73 0a0a 466f 7220   Questions..For 
-00001180: 616e 7920 7175 6573 7469 6f6e 7320 6f72  any questions or
-00001190: 2063 6f6d 6d65 6e74 732c 2070 6c65 6173   comments, pleas
-000011a0: 6520 6368 6563 6b20 7468 6520 5b46 4151  e check the [FAQ
-000011b0: 5d28 4641 512e 6d64 2920 6669 7273 7420  ](FAQ.md) first 
-000011c0: 616e 6420 6665 656c 2066 7265 6520 746f  and feel free to
-000011d0: 2073 7769 6e67 2062 7920 7468 6520 5b4e   swing by the [N
-000011e0: 6574 776f 726b 2074 6f20 436f 6465 2073  etwork to Code s
-000011f0: 6c61 636b 2063 6861 6e6e 656c 5d28 6874  lack channel](ht
-00001200: 7470 733a 2f2f 6e65 7477 6f72 6b74 6f63  tps://networktoc
-00001210: 6f64 652e 736c 6163 6b2e 636f 6d2f 2920  ode.slack.com/) 
-00001220: 2863 6861 6e6e 656c 2023 6e65 7477 6f72  (channel #networ
-00001230: 6b74 6f63 6f64 6529 2e0a 5369 676e 2075  ktocode)..Sign u
-00001240: 7020 5b68 6572 655d 2868 7474 703a 2f2f  p [here](http://
-00001250: 736c 6163 6b2e 6e65 7477 6f72 6b74 6f63  slack.networktoc
-00001260: 6f64 652e 636f 6d2f 290a 0a              ode.com/)..
+00000040: 322e 310a 5375 6d6d 6172 793a 204e 6175  2.1.Summary: Nau
+00000050: 746f 626f 7420 706c 7567 696e 2074 6f20  tobot plugin to 
+00000060: 6d6f 6465 6c20 6669 7265 7761 6c6c 206f  model firewall o
+00000070: 626a 6563 7473 2e0a 486f 6d65 2d70 6167  bjects..Home-pag
+00000080: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
+00000090: 622e 636f 6d2f 6e61 7574 6f62 6f74 2f6e  b.com/nautobot/n
+000000a0: 6175 746f 626f 742d 706c 7567 696e 2d66  autobot-plugin-f
+000000b0: 6972 6577 616c 6c2d 6d6f 6465 6c73 0a4c  irewall-models.L
+000000c0: 6963 656e 7365 3a20 4170 6163 6865 2d32  icense: Apache-2
+000000d0: 2e30 0a4b 6579 776f 7264 733a 206e 6175  .0.Keywords: nau
+000000e0: 746f 626f 742c 6e61 7574 6f62 6f74 2d70  tobot,nautobot-p
+000000f0: 6c75 6769 6e0a 4175 7468 6f72 3a20 4e65  lugin.Author: Ne
+00000100: 7477 6f72 6b20 746f 2043 6f64 652c 204c  twork to Code, L
+00000110: 4c43 0a41 7574 686f 722d 656d 6169 6c3a  LC.Author-email:
+00000120: 2069 6e66 6f40 6e65 7477 6f72 6b74 6f63   info@networktoc
+00000130: 6f64 652e 636f 6d0a 5265 7175 6972 6573  ode.com.Requires
+00000140: 2d50 7974 686f 6e3a 203e 3d33 2e37 2c3c  -Python: >=3.7,<
+00000150: 342e 300a 436c 6173 7369 6669 6572 3a20  4.0.Classifier: 
+00000160: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000170: 7070 726f 7665 6420 3a3a 2041 7061 6368  pproved :: Apach
+00000180: 6520 536f 6674 7761 7265 204c 6963 656e  e Software Licen
+00000190: 7365 0a43 6c61 7373 6966 6965 723a 2050  se.Classifier: P
+000001a0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001b0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001c0: 2033 0a43 6c61 7373 6966 6965 723a 2050   3.Classifier: P
+000001d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001f0: 2033 2e37 0a43 6c61 7373 6966 6965 723a   3.7.Classifier:
+00000200: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000210: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000220: 3a3a 2033 2e38 0a43 6c61 7373 6966 6965  :: 3.8.Classifie
+00000230: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000240: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000250: 6e20 3a3a 2033 2e39 0a43 6c61 7373 6966  n :: 3.9.Classif
+00000260: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000270: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000280: 686f 6e20 3a3a 2033 2e31 300a 436c 6173  hon :: 3.10.Clas
+00000290: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000002a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002b0: 5079 7468 6f6e 203a 3a20 332e 3131 0a50  Python :: 3.11.P
+000002c0: 726f 7669 6465 732d 4578 7472 613a 206e  rovides-Extra: n
+000002d0: 6175 746f 626f 740a 5265 7175 6972 6573  autobot.Requires
+000002e0: 2d44 6973 743a 2063 6170 6972 6361 2028  -Dist: capirca (
+000002f0: 3e3d 322e 302e 362c 3c33 2e30 2e30 290a  >=2.0.6,<3.0.0).
+00000300: 5265 7175 6972 6573 2d44 6973 743a 206e  Requires-Dist: n
+00000310: 6175 746f 626f 7420 283e 3d31 2e34 2e30  autobot (>=1.4.0
+00000320: 2c3c 322e 302e 3029 203b 2065 7874 7261  ,<2.0.0) ; extra
+00000330: 203d 3d20 226e 6175 746f 626f 7422 0a52   == "nautobot".R
+00000340: 6571 7569 7265 732d 4469 7374 3a20 6e65  equires-Dist: ne
+00000350: 7475 7469 6c73 2028 3e3d 312e 302e 302c  tutils (>=1.0.0,
+00000360: 3c32 2e30 2e30 290a 5072 6f6a 6563 742d  <2.0.0).Project-
+00000370: 5552 4c3a 2052 6570 6f73 6974 6f72 792c  URL: Repository,
+00000380: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000390: 636f 6d2f 6e61 7574 6f62 6f74 2f6e 6175  com/nautobot/nau
+000003a0: 746f 626f 742d 706c 7567 696e 2d66 6972  tobot-plugin-fir
+000003b0: 6577 616c 6c2d 6d6f 6465 6c73 0a44 6573  ewall-models.Des
+000003c0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+000003d0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+000003e0: 646f 776e 0a0a 2320 4e61 7574 6f62 6f74  down..# Nautobot
+000003f0: 2050 6c75 6769 6e20 4669 7265 7761 6c6c   Plugin Firewall
+00000400: 204d 6f64 656c 730a 0a3c 7020 616c 6967   Models..<p alig
+00000410: 6e3d 2263 656e 7465 7222 3e0a 2020 3c69  n="center">.  <i
+00000420: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000430: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00000440: 6e74 656e 742e 636f 6d2f 6e61 7574 6f62  ntent.com/nautob
+00000450: 6f74 2f6e 6175 746f 626f 742d 706c 7567  ot/nautobot-plug
+00000460: 696e 2d66 6972 6577 616c 6c2d 6d6f 6465  in-firewall-mode
+00000470: 6c73 2f64 6576 656c 6f70 2f64 6f63 732f  ls/develop/docs/
+00000480: 696d 6167 6573 2f69 636f 6e2d 6e61 7574  images/icon-naut
+00000490: 6f62 6f74 2d66 6972 6577 616c 6c2d 6d6f  obot-firewall-mo
+000004a0: 6465 6c73 2e70 6e67 2220 636c 6173 733d  dels.png" class=
+000004b0: 226c 6f67 6f22 2068 6569 6768 743d 2232  "logo" height="2
+000004c0: 3030 7078 223e 0a20 203c 6272 3e0a 2020  00px">.  <br>.  
+000004d0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000004e0: 2f67 6974 6875 622e 636f 6d2f 6e61 7574  /github.com/naut
+000004f0: 6f62 6f74 2f6e 6175 746f 626f 742d 706c  obot/nautobot-pl
+00000500: 7567 696e 2d66 6972 6577 616c 6c2d 6d6f  ugin-firewall-mo
+00000510: 6465 6c73 2f61 6374 696f 6e73 223e 3c69  dels/actions"><i
+00000520: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000530: 6769 7468 7562 2e63 6f6d 2f6e 6175 746f  github.com/nauto
+00000540: 626f 742f 6e61 7574 6f62 6f74 2d70 6c75  bot/nautobot-plu
+00000550: 6769 6e2d 6669 7265 7761 6c6c 2d6d 6f64  gin-firewall-mod
+00000560: 656c 732f 6163 7469 6f6e 732f 776f 726b  els/actions/work
+00000570: 666c 6f77 732f 6369 2e79 6d6c 2f62 6164  flows/ci.yml/bad
+00000580: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
+00000590: 696e 223e 3c2f 613e 0a20 203c 6120 6872  in"></a>.  <a hr
+000005a0: 6566 3d22 6874 7470 733a 2f2f 646f 6373  ef="https://docs
+000005b0: 2e6e 6175 746f 626f 742e 636f 6d2f 7072  .nautobot.com/pr
+000005c0: 6f6a 6563 7473 2f66 6972 6577 616c 6c2d  ojects/firewall-
+000005d0: 6d6f 6465 6c73 2f65 6e2f 6c61 7465 7374  models/en/latest
+000005e0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+000005f0: 733a 2f2f 7265 6164 7468 6564 6f63 732e  s://readthedocs.
+00000600: 6f72 672f 7072 6f6a 6563 7473 2f6e 6175  org/projects/nau
+00000610: 746f 626f 742d 706c 7567 696e 2d66 6972  tobot-plugin-fir
+00000620: 6577 616c 6c2d 6d6f 6465 6c73 2f62 6164  ewall-models/bad
+00000630: 6765 2f22 3e3c 2f61 3e0a 2020 3c61 2068  ge/"></a>.  <a h
+00000640: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+00000650: 692e 6f72 672f 7072 6f6a 6563 742f 6e61  i.org/project/na
+00000660: 7574 6f62 6f74 2d66 6972 6577 616c 6c2d  utobot-firewall-
+00000670: 6d6f 6465 6c73 2f22 3e3c 696d 6720 7372  models/"><img sr
+00000680: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000690: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+000006a0: 2f6e 6175 746f 626f 742d 6669 7265 7761  /nautobot-firewa
+000006b0: 6c6c 2d6d 6f64 656c 7322 3e3c 2f61 3e0a  ll-models"></a>.
+000006c0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000006d0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000006e0: 6563 742f 6e61 7574 6f62 6f74 2d66 6972  ect/nautobot-fir
+000006f0: 6577 616c 6c2d 6d6f 6465 6c73 2f22 3e3c  ewall-models/"><
+00000700: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000710: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000720: 7079 7069 2f64 6d2f 6e61 7574 6f62 6f74  pypi/dm/nautobot
+00000730: 2d66 6972 6577 616c 6c2d 6d6f 6465 6c73  -firewall-models
+00000740: 223e 3c2f 613e 0a20 203c 6272 3e0a 2020  "></a>.  <br>.  
+00000750: 416e 203c 6120 6872 6566 3d22 6874 7470  An <a href="http
+00000760: 733a 2f2f 7777 772e 6e65 7477 6f72 6b74  s://www.networkt
+00000770: 6f63 6f64 652e 636f 6d2f 6e61 7574 6f62  ocode.com/nautob
+00000780: 6f74 2f61 7070 732f 223e 4170 703c 2f61  ot/apps/">App</a
+00000790: 3e20 666f 7220 3c61 2068 7265 663d 2268  > for <a href="h
+000007a0: 7474 7073 3a2f 2f6e 6175 746f 626f 742e  ttps://nautobot.
+000007b0: 636f 6d2f 223e 4e61 7574 6f62 6f74 3c2f  com/">Nautobot</
+000007c0: 613e 2e0a 3c2f 703e 0a0a 2323 204f 7665  a>..</p>..## Ove
+000007d0: 7276 6965 770a 0a41 2070 6c75 6769 6e20  rview..A plugin 
+000007e0: 666f 7220 5b4e 6175 746f 626f 745d 2868  for [Nautobot](h
+000007f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000800: 6d2f 6e61 7574 6f62 6f74 2f6e 6175 746f  m/nautobot/nauto
+00000810: 626f 7429 2074 6861 7420 6973 206d 6561  bot) that is mea
+00000820: 6e74 2074 6f20 6d6f 6465 6c20 6c61 7965  nt to model laye
+00000830: 7220 3420 6669 7265 7761 6c6c 2070 6f6c  r 4 firewall pol
+00000840: 6963 6965 7320 616e 642f 6f72 2065 7874  icies and/or ext
+00000850: 656e 6465 6420 6163 6365 7373 2063 6f6e  ended access con
+00000860: 7472 6f6c 206c 6973 7473 2e0a 0a23 2323  trol lists...###
+00000870: 2053 6372 6565 6e73 686f 7473 0a0a 4d6f   Screenshots..Mo
+00000880: 7265 2073 6372 6565 6e73 686f 7473 2063  re screenshots c
+00000890: 616e 2062 6520 666f 756e 6420 696e 2074  an be found in t
+000008a0: 6865 205b 5573 696e 6720 7468 6520 4170  he [Using the Ap
+000008b0: 705d 2868 7474 7073 3a2f 2f64 6f63 732e  p](https://docs.
+000008c0: 6e61 7574 6f62 6f74 2e63 6f6d 2f70 726f  nautobot.com/pro
+000008d0: 6a65 6374 732f 6669 7265 7761 6c6c 2d6d  jects/firewall-m
+000008e0: 6f64 656c 732f 656e 2f6c 6174 6573 742f  odels/en/latest/
+000008f0: 7573 6572 2f61 7070 5f75 7365 5f63 6173  user/app_use_cas
+00000900: 6573 2f29 2070 6167 6520 696e 2074 6865  es/) page in the
+00000910: 2064 6f63 756d 656e 7461 7469 6f6e 2e20   documentation. 
+00000920: 4865 7265 2773 2061 2071 7569 636b 206f  Here's a quick o
+00000930: 7665 7276 6965 7720 6f66 2073 6f6d 6520  verview of some 
+00000940: 6f66 2074 6865 2070 6c75 6769 6e27 7320  of the plugin's 
+00000950: 6164 6465 6420 6675 6e63 7469 6f6e 616c  added functional
+00000960: 6974 793a 0a0a 215b 4e61 7669 6761 7469  ity:..![Navigati
+00000970: 6f6e 204d 656e 755d 2868 7474 7073 3a2f  on Menu](https:/
+00000980: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00000990: 6f6e 7465 6e74 2e63 6f6d 2f6e 6175 746f  ontent.com/nauto
+000009a0: 626f 742f 6e61 7574 6f62 6f74 2d70 6c75  bot/nautobot-plu
+000009b0: 6769 6e2d 6669 7265 7761 6c6c 2d6d 6f64  gin-firewall-mod
+000009c0: 656c 732f 6465 7665 6c6f 702f 646f 6373  els/develop/docs
+000009d0: 2f69 6d61 6765 732f 6e61 766d 656e 752e  /images/navmenu.
+000009e0: 706e 6720 224e 6176 6967 6174 696f 6e20  png "Navigation 
+000009f0: 4d65 6e75 2229 0a0a 215b 506f 6c69 6379  Menu")..![Policy
+00000a00: 2056 6965 775d 2868 7474 7073 3a2f 2f72   View](https://r
+00000a10: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00000a20: 7465 6e74 2e63 6f6d 2f6e 6175 746f 626f  tent.com/nautobo
+00000a30: 742f 6e61 7574 6f62 6f74 2d70 6c75 6769  t/nautobot-plugi
+00000a40: 6e2d 6669 7265 7761 6c6c 2d6d 6f64 656c  n-firewall-model
+00000a50: 732f 6465 7665 6c6f 702f 646f 6373 2f69  s/develop/docs/i
+00000a60: 6d61 6765 732f 706f 6c69 6379 2e70 6e67  mages/policy.png
+00000a70: 2022 506f 6c69 6379 2056 6965 7722 290a   "Policy View").
+00000a80: 0a0a 2323 2054 7279 2069 7420 6f75 7421  ..## Try it out!
+00000a90: 0a0a 5468 6973 2041 7070 2069 7320 696e  ..This App is in
+00000aa0: 7374 616c 6c65 6420 696e 2074 6865 204e  stalled in the N
+00000ab0: 6175 746f 626f 7420 436f 6d6d 756e 6974  autobot Communit
+00000ac0: 7920 5361 6e64 626f 7820 666f 756e 6420  y Sandbox found 
+00000ad0: 6f76 6572 2061 7420 5b64 656d 6f2e 6e61  over at [demo.na
+00000ae0: 7574 6f62 6f74 2e63 6f6d 5d28 6874 7470  utobot.com](http
+00000af0: 733a 2f2f 6465 6d6f 2e6e 6175 746f 626f  s://demo.nautobo
+00000b00: 742e 636f 6d2f 2921 0a0a 3e20 466f 7220  t.com/)!..> For 
+00000b10: 6120 6675 6c6c 206c 6973 7420 6f66 2061  a full list of a
+00000b20: 6c6c 2074 6865 2061 7661 696c 6162 6c65  ll the available
+00000b30: 2061 6c77 6179 732d 6f6e 2073 616e 6462   always-on sandb
+00000b40: 6f78 2065 6e76 6972 6f6e 6d65 6e74 732c  ox environments,
+00000b50: 2068 6561 6420 6f76 6572 2074 6f20 7468   head over to th
+00000b60: 6520 6d61 696e 2070 6167 6520 6f6e 205b  e main page on [
+00000b70: 6e65 7477 6f72 6b74 6f63 6f64 652e 636f  networktocode.co
+00000b80: 6d5d 2868 7474 7073 3a2f 2f77 7777 2e6e  m](https://www.n
+00000b90: 6574 776f 726b 746f 636f 6465 2e63 6f6d  etworktocode.com
+00000ba0: 2f6e 6175 746f 626f 742f 7361 6e64 626f  /nautobot/sandbo
+00000bb0: 782d 656e 7669 726f 6e6d 656e 7473 2f29  x-environments/)
+00000bc0: 2e0a 0a23 2320 446f 6375 6d65 6e74 6174  ...## Documentat
+00000bd0: 696f 6e0a 0a46 756c 6c20 646f 6375 6d65  ion..Full docume
+00000be0: 6e74 6174 696f 6e20 666f 7220 7468 6973  ntation for this
+00000bf0: 2041 7070 2063 616e 2062 6520 666f 756e   App can be foun
+00000c00: 6420 6f76 6572 206f 6e20 7468 6520 5b4e  d over on the [N
+00000c10: 6175 746f 626f 7420 446f 6373 5d28 6874  autobot Docs](ht
+00000c20: 7470 733a 2f2f 646f 6373 2e6e 6175 746f  tps://docs.nauto
+00000c30: 626f 742e 636f 6d29 2077 6562 7369 7465  bot.com) website
+00000c40: 3a0a 0a2d 205b 5573 6572 2047 7569 6465  :..- [User Guide
+00000c50: 5d28 6874 7470 733a 2f2f 646f 6373 2e6e  ](https://docs.n
+00000c60: 6175 746f 626f 742e 636f 6d2f 7072 6f6a  autobot.com/proj
+00000c70: 6563 7473 2f66 6972 6577 616c 6c2d 6d6f  ects/firewall-mo
+00000c80: 6465 6c73 2f65 6e2f 6c61 7465 7374 2f75  dels/en/latest/u
+00000c90: 7365 722f 6170 705f 6f76 6572 7669 6577  ser/app_overview
+00000ca0: 2f29 202d 204f 7665 7276 6965 772c 2055  /) - Overview, U
+00000cb0: 7369 6e67 2074 6865 2041 7070 2c20 4765  sing the App, Ge
+00000cc0: 7474 696e 6720 5374 6172 7465 642e 0a2d  tting Started..-
+00000cd0: 205b 4164 6d69 6e69 7374 7261 746f 7220   [Administrator 
+00000ce0: 4775 6964 655d 2868 7474 7073 3a2f 2f64  Guide](https://d
+00000cf0: 6f63 732e 6e61 7574 6f62 6f74 2e63 6f6d  ocs.nautobot.com
+00000d00: 2f70 726f 6a65 6374 732f 6669 7265 7761  /projects/firewa
+00000d10: 6c6c 2d6d 6f64 656c 732f 656e 2f6c 6174  ll-models/en/lat
+00000d20: 6573 742f 6164 6d69 6e2f 696e 7374 616c  est/admin/instal
+00000d30: 6c2f 2920 2d20 486f 7720 746f 2049 6e73  l/) - How to Ins
+00000d40: 7461 6c6c 2c20 436f 6e66 6967 7572 652c  tall, Configure,
+00000d50: 2055 7067 7261 6465 2c20 6f72 2055 6e69   Upgrade, or Uni
+00000d60: 6e73 7461 6c6c 2074 6865 2041 7070 2e0a  nstall the App..
+00000d70: 2d20 5b44 6576 656c 6f70 6572 2047 7569  - [Developer Gui
+00000d80: 6465 5d28 6874 7470 733a 2f2f 646f 6373  de](https://docs
+00000d90: 2e6e 6175 746f 626f 742e 636f 6d2f 7072  .nautobot.com/pr
+00000da0: 6f6a 6563 7473 2f66 6972 6577 616c 6c2d  ojects/firewall-
+00000db0: 6d6f 6465 6c73 2f65 6e2f 6c61 7465 7374  models/en/latest
+00000dc0: 2f64 6576 2f63 6f6e 7472 6962 7574 696e  /dev/contributin
+00000dd0: 672f 2920 2d20 4578 7465 6e64 696e 6720  g/) - Extending 
+00000de0: 7468 6520 4170 702c 2043 6f64 6520 5265  the App, Code Re
+00000df0: 6665 7265 6e63 652c 2043 6f6e 7472 6962  ference, Contrib
+00000e00: 7574 696f 6e20 4775 6964 652e 0a2d 205b  ution Guide..- [
+00000e10: 5265 6c65 6173 6520 4e6f 7465 7320 2f20  Release Notes / 
+00000e20: 4368 616e 6765 6c6f 675d 2868 7474 7073  Changelog](https
+00000e30: 3a2f 2f64 6f63 732e 6e61 7574 6f62 6f74  ://docs.nautobot
+00000e40: 2e63 6f6d 2f70 726f 6a65 6374 732f 6669  .com/projects/fi
+00000e50: 7265 7761 6c6c 2d6d 6f64 656c 732f 656e  rewall-models/en
+00000e60: 2f6c 6174 6573 742f 6164 6d69 6e2f 7265  /latest/admin/re
+00000e70: 6c65 6173 655f 6e6f 7465 732f 292e 0a2d  lease_notes/)..-
+00000e80: 205b 4672 6571 7565 6e74 6c79 2041 736b   [Frequently Ask
+00000e90: 6564 2051 7565 7374 696f 6e73 5d28 6874  ed Questions](ht
+00000ea0: 7470 733a 2f2f 646f 6373 2e6e 6175 746f  tps://docs.nauto
+00000eb0: 626f 742e 636f 6d2f 7072 6f6a 6563 7473  bot.com/projects
+00000ec0: 2f66 6972 6577 616c 6c2d 6d6f 6465 6c73  /firewall-models
+00000ed0: 2f65 6e2f 6c61 7465 7374 2f75 7365 722f  /en/latest/user/
+00000ee0: 6661 712f 292e 0a0a 2323 2320 436f 6e74  faq/)...### Cont
+00000ef0: 7269 6275 7469 6e67 2074 6f20 7468 6520  ributing to the 
+00000f00: 446f 6375 6d65 6e74 6174 696f 6e0a 0a59  Documentation..Y
+00000f10: 6f75 2063 616e 2066 696e 6420 616c 6c20  ou can find all 
+00000f20: 7468 6520 4d61 726b 646f 776e 2073 6f75  the Markdown sou
+00000f30: 7263 6520 666f 7220 7468 6520 4170 7020  rce for the App 
+00000f40: 646f 6375 6d65 6e74 6174 696f 6e20 756e  documentation un
+00000f50: 6465 7220 7468 6520 5b60 646f 6373 605d  der the [`docs`]
+00000f60: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000f70: 636f 6d2f 6e61 7574 6f62 6f74 2f6e 6175  com/nautobot/nau
+00000f80: 746f 626f 742d 706c 7567 696e 2d66 6972  tobot-plugin-fir
+00000f90: 6577 616c 6c2d 6d6f 6465 6c73 2f74 7265  ewall-models/tre
+00000fa0: 652f 6465 7665 6c6f 702f 646f 6373 2920  e/develop/docs) 
+00000fb0: 666f 6c64 6572 2069 6e20 7468 6973 2072  folder in this r
+00000fc0: 6570 6f73 6974 6f72 792e 2046 6f72 2073  epository. For s
+00000fd0: 696d 706c 6520 6564 6974 732c 2061 204d  imple edits, a M
+00000fe0: 6172 6b64 6f77 6e20 6361 7061 626c 6520  arkdown capable 
+00000ff0: 6564 6974 6f72 2069 7320 7375 6666 6963  editor is suffic
+00001000: 6965 6e74 3a20 636c 6f6e 6520 7468 6520  ient: clone the 
+00001010: 7265 706f 7369 746f 7279 2061 6e64 2065  repository and e
+00001020: 6469 7420 6177 6179 2e0a 0a49 6620 796f  dit away...If yo
+00001030: 7520 6e65 6564 2074 6f20 7669 6577 2074  u need to view t
+00001040: 6865 2066 756c 6c79 2d67 656e 6572 6174  he fully-generat
+00001050: 6564 2064 6f63 756d 656e 7461 7469 6f6e  ed documentation
+00001060: 2073 6974 652c 2079 6f75 2063 616e 2062   site, you can b
+00001070: 7569 6c64 2069 7420 7769 7468 205b 4d6b  uild it with [Mk
+00001080: 446f 6373 5d28 6874 7470 733a 2f2f 7777  Docs](https://ww
+00001090: 772e 6d6b 646f 6373 2e6f 7267 2f29 2e20  w.mkdocs.org/). 
+000010a0: 4120 636f 6e74 6169 6e65 7220 686f 7374  A container host
+000010b0: 696e 6720 7468 6520 646f 6375 6d65 6e74  ing the document
+000010c0: 6174 696f 6e20 6361 6e20 6265 2073 7461  ation can be sta
+000010d0: 7274 6564 2075 7369 6e67 2074 6865 2060  rted using the `
+000010e0: 696e 766f 6b65 6020 636f 6d6d 616e 6473  invoke` commands
+000010f0: 2028 6465 7461 696c 7320 696e 2074 6865   (details in the
+00001100: 205b 4465 7665 6c6f 706d 656e 7420 456e   [Development En
+00001110: 7669 726f 6e6d 656e 7420 4775 6964 655d  vironment Guide]
+00001120: 2868 7474 7073 3a2f 2f64 6f63 732e 6e61  (https://docs.na
+00001130: 7574 6f62 6f74 2e63 6f6d 2f70 726f 6a65  utobot.com/proje
+00001140: 6374 732f 6669 7265 7761 6c6c 2d6d 6f64  cts/firewall-mod
+00001150: 656c 732f 656e 2f6c 6174 6573 742f 6465  els/en/latest/de
+00001160: 762f 6465 765f 656e 7669 726f 6e6d 656e  v/dev_environmen
+00001170: 742f 2364 6f63 6b65 722d 6465 7665 6c6f  t/#docker-develo
+00001180: 706d 656e 742d 656e 7669 726f 6e6d 656e  pment-environmen
+00001190: 7429 2920 6f6e 205b 6874 7470 3a2f 2f6c  t)) on [http://l
+000011a0: 6f63 616c 686f 7374 3a38 3030 315d 2868  ocalhost:8001](h
+000011b0: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
+000011c0: 3830 3031 292e 2055 7369 6e67 2074 6869  8001). Using thi
+000011d0: 7320 636f 6e74 6169 6e65 722c 2061 7320  s container, as 
+000011e0: 796f 7572 2063 6861 6e67 6573 2074 6f20  your changes to 
+000011f0: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
+00001200: 6e20 6172 6520 7361 7665 642c 2074 6865  n are saved, the
+00001210: 7920 7769 6c6c 2062 6520 6175 746f 6d61  y will be automa
+00001220: 7469 6361 6c6c 7920 7265 6275 696c 7420  tically rebuilt 
+00001230: 616e 6420 616e 7920 7061 6765 7320 6375  and any pages cu
+00001240: 7272 656e 746c 7920 6265 696e 6720 7669  rrently being vi
+00001250: 6577 6564 2077 696c 6c20 6265 2072 656c  ewed will be rel
+00001260: 6f61 6465 6420 696e 2079 6f75 7220 6272  oaded in your br
+00001270: 6f77 7365 722e 0a0a 416e 7920 5052 7320  owser...Any PRs 
+00001280: 7769 7468 2066 6978 6573 206f 7220 696d  with fixes or im
+00001290: 7072 6f76 656d 656e 7473 2061 7265 2076  provements are v
+000012a0: 6572 7920 7765 6c63 6f6d 6521 0a0a 2323  ery welcome!..##
+000012b0: 2051 7565 7374 696f 6e73 0a0a 466f 7220   Questions..For 
+000012c0: 616e 7920 7175 6573 7469 6f6e 7320 6f72  any questions or
+000012d0: 2063 6f6d 6d65 6e74 732c 2070 6c65 6173   comments, pleas
+000012e0: 6520 6368 6563 6b20 7468 6520 5b46 4151  e check the [FAQ
+000012f0: 5d28 6874 7470 733a 2f2f 646f 6373 2e6e  ](https://docs.n
+00001300: 6175 746f 626f 742e 636f 6d2f 7072 6f6a  autobot.com/proj
+00001310: 6563 7473 2f66 6972 6577 616c 6c2d 6d6f  ects/firewall-mo
+00001320: 6465 6c73 2f65 6e2f 6c61 7465 7374 2f75  dels/en/latest/u
+00001330: 7365 722f 6661 712f 2920 6669 7273 742e  ser/faq/) first.
+00001340: 2046 6565 6c20 6672 6565 2074 6f20 616c   Feel free to al
+00001350: 736f 2073 7769 6e67 2062 7920 7468 6520  so swing by the 
+00001360: 5b4e 6574 776f 726b 2074 6f20 436f 6465  [Network to Code
+00001370: 2053 6c61 636b 5d28 6874 7470 733a 2f2f   Slack](https://
+00001380: 6e65 7477 6f72 6b74 6f63 6f64 652e 736c  networktocode.sl
+00001390: 6163 6b2e 636f 6d2f 2920 2863 6861 6e6e  ack.com/) (chann
+000013a0: 656c 2060 236e 6175 746f 626f 7460 292c  el `#nautobot`),
+000013b0: 2073 6967 6e20 7570 205b 6865 7265 5d28   sign up [here](
+000013c0: 6874 7470 3a2f 2f73 6c61 636b 2e6e 6574  http://slack.net
+000013d0: 776f 726b 746f 636f 6465 2e63 6f6d 2f29  worktocode.com/)
+000013e0: 2069 6620 796f 7520 646f 6e27 7420 6861   if you don't ha
+000013f0: 7665 2061 6e20 6163 636f 756e 742e 0a0a  ve an account...
```

