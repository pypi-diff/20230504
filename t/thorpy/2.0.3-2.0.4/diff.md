# Comparing `tmp/thorpy-2.0.3.tar.gz` & `tmp/thorpy-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thorpy-2.0.3.tar", last modified: Mon Apr 24 16:21:54 2023, max compression
+gzip compressed data, was "thorpy-2.0.4.tar", last modified: Thu May  4 15:32:41 2023, max compression
```

## Comparing `thorpy-2.0.3.tar` & `thorpy-2.0.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 16:21:54.900268 thorpy-2.0.3/
--rw-rw-rw-   0        0        0     1093 2023-04-18 20:35:49.000000 thorpy-2.0.3/LICENSE
--rw-rw-rw-   0        0        0      378 2023-04-24 16:21:54.900268 thorpy-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2336 2023-04-24 16:16:09.000000 thorpy-2.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 16:21:54.901269 thorpy-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      596 2023-04-24 16:21:18.000000 thorpy-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:21:54.859259 thorpy-2.0.3/thorpy/
--rw-rw-rw-   0        0        0     3605 2023-04-24 16:20:06.000000 thorpy-2.0.3/thorpy/__init__.py
--rw-rw-rw-   0        0        0    53375 2023-04-24 16:05:08.000000 thorpy-2.0.3/thorpy/canonical.py
--rw-rw-rw-   0        0        0   124135 2023-04-24 16:05:18.000000 thorpy-2.0.3/thorpy/elements.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:21:54.899268 thorpy-2.0.3/thorpy/examples/
--rw-rw-rw-   0        0        0        0 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/__init__.py
--rw-rw-rw-   0        0        0     1132 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_alert.py
--rw-rw-rw-   0        0        0     1243 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_anim_move.py
--rw-rw-rw-   0        0        0     1703 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_animatedgif.py
--rw-rw-rw-   0        0        0      992 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_box.py
--rw-rw-rw-   0        0        0      861 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_button_helloworld.py
--rw-rw-rw-   0        0        0      868 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_color_gradient.py
--rw-rw-rw-   0        0        0     1183 2023-04-24 16:05:29.000000 thorpy-2.0.3/thorpy/examples/_example_colorpicker.py
--rw-rw-rw-   0        0        0     2400 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_colorpicker2.py
--rw-rw-rw-   0        0        0     2402 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_colorpicker_fine_tuning.py
--rw-rw-rw-   0        0        0     3284 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_create_style.py
--rw-rw-rw-   0        0        0     3425 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_create_style2.py
--rw-rw-rw-   0        0        0     2249 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_custom_theme.py
--rw-rw-rw-   0        0        0     2063 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_dropdownlist.py
--rw-rw-rw-   0        0        0     1790 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_events.py
--rw-rw-rw-   0        0        0     1177 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_filebrowser.py
--rw-rw-rw-   0        0        0     2245 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_fx_light_emitting_image.py
--rw-rw-rw-   0        0        0     3235 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_fx_lights.py
--rw-rw-rw-   0        0        0     1984 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_get_value_from_elements.py
--rw-rw-rw-   0        0        0     1376 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_grouping.py
--rw-rw-rw-   0        0        0     1112 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_grouping_without_sorting.py
--rw-rw-rw-   0        0        0     2575 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_groups_of_groups.py
--rw-rw-rw-   0        0        0     3731 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_guess_the_number.py
--rw-rw-rw-   0        0        0     1573 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_helper.py
--rw-rw-rw-   0        0        0      982 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_heterogeneous_texts.py
--rw-rw-rw-   0        0        0      685 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_image_with_text.py
--rw-rw-rw-   0        0        0     1322 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_imagebutton.py
--rw-rw-rw-   0        0        0     1532 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_integration_in_existing_code.py
--rw-rw-rw-   0        0        0     1316 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_labels.py
--rw-rw-rw-   0        0        0     3028 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_launch.py
--rw-rw-rw-   0        0        0     1287 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_lifebar.py
--rw-rw-rw-   0        0        0     1305 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_look_tune.py
--rw-rw-rw-   0        0        0     2297 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_rich_text.py
--rw-rw-rw-   0        0        0     1307 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_set_default_font.py
--rw-rw-rw-   0        0        0     2128 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_shadows.py
--rw-rw-rw-   0        0        0     3051 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_showcase_themes.py
--rw-rw-rw-   0        0        0     3184 2023-04-24 16:00:12.000000 thorpy-2.0.3/thorpy/examples/_example_showcase_themes2.py
--rw-rw-rw-   0        0        0     2119 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_showcase_themes_buttons.py
--rw-rw-rw-   0        0        0     1500 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_showfps.py
--rw-rw-rw-   0        0        0     1660 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_slider.py
--rw-rw-rw-   0        0        0     2460 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_text_input.py
--rw-rw-rw-   0        0        0     2765 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_text_width.py
--rw-rw-rw-   0        0        0     1431 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_togglables_pool.py
--rw-rw-rw-   0        0        0     1105 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_user_choices.py
--rw-rw-rw-   0        0        0     1431 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_user_choices2.py
--rw-rw-rw-   0        0        0     2051 2023-04-24 16:01:46.000000 thorpy-2.0.3/thorpy/examples/_example_user_chooses_font.py
--rw-rw-rw-   0        0        0     2219 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_waiting_bar.py
--rw-rw-rw-   0        0        0     4520 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/gametools.py
--rw-rw-rw-   0        0        0    28781 2023-04-22 19:22:36.000000 thorpy-2.0.3/thorpy/graphics.py
--rw-rw-rw-   0        0        0     6068 2023-04-24 15:17:59.000000 thorpy-2.0.3/thorpy/loops.py
--rw-rw-rw-   0        0        0     2639 2023-04-22 15:23:24.000000 thorpy-2.0.3/thorpy/monitoring.py
--rw-rw-rw-   0        0        0      467 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/parameters.py
--rw-rw-rw-   0        0        0      625 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/setup.py
--rw-rw-rw-   0        0        0     3727 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/shadows.py
--rw-rw-rw-   0        0        0     2540 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/sorting.py
--rw-rw-rw-   0        0        0     2307 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/sound.py
--rw-rw-rw-   0        0        0    35577 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/styles.py
--rw-rw-rw-   0        0        0    32875 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/themes.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:21:54.863260 thorpy-2.0.3/thorpy.egg-info/
--rw-rw-rw-   0        0        0      378 2023-04-24 16:21:54.000000 thorpy-2.0.3/thorpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2349 2023-04-24 16:21:54.000000 thorpy-2.0.3/thorpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 16:21:54.000000 thorpy-2.0.3/thorpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 16:21:54.000000 thorpy-2.0.3/thorpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 15:32:41.676273 thorpy-2.0.4/
+-rw-rw-rw-   0        0        0     1093 2023-04-18 20:35:49.000000 thorpy-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0      378 2023-05-04 15:32:41.675273 thorpy-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2409 2023-05-04 15:31:08.000000 thorpy-2.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 15:32:41.676273 thorpy-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      596 2023-05-04 15:32:24.000000 thorpy-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 15:32:41.623261 thorpy-2.0.4/thorpy/
+-rw-rw-rw-   0        0        0     3603 2023-05-04 15:29:32.000000 thorpy-2.0.4/thorpy/__init__.py
+-rw-rw-rw-   0        0        0    53415 2023-05-04 15:29:59.000000 thorpy-2.0.4/thorpy/canonical.py
+-rw-rw-rw-   0        0        0   124135 2023-04-24 16:05:18.000000 thorpy-2.0.4/thorpy/elements.py
+drwxrwxrwx   0        0        0        0 2023-05-04 15:32:41.674272 thorpy-2.0.4/thorpy/examples/
+-rw-rw-rw-   0        0        0        0 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/__init__.py
+-rw-rw-rw-   0        0        0     1132 2023-04-24 16:24:03.000000 thorpy-2.0.4/thorpy/examples/_example_alert.py
+-rw-rw-rw-   0        0        0     1243 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_anim_move.py
+-rw-rw-rw-   0        0        0     1703 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_animatedgif.py
+-rw-rw-rw-   0        0        0      992 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_box.py
+-rw-rw-rw-   0        0        0      861 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_button_helloworld.py
+-rw-rw-rw-   0        0        0      868 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_color_gradient.py
+-rw-rw-rw-   0        0        0     1183 2023-04-24 16:05:29.000000 thorpy-2.0.4/thorpy/examples/_example_colorpicker.py
+-rw-rw-rw-   0        0        0     2400 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_colorpicker2.py
+-rw-rw-rw-   0        0        0     2402 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_colorpicker_fine_tuning.py
+-rw-rw-rw-   0        0        0     3284 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_create_style.py
+-rw-rw-rw-   0        0        0     3425 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_create_style2.py
+-rw-rw-rw-   0        0        0     2249 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_custom_theme.py
+-rw-rw-rw-   0        0        0     2063 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_dropdownlist.py
+-rw-rw-rw-   0        0        0     1790 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_events.py
+-rw-rw-rw-   0        0        0     1177 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_filebrowser.py
+-rw-rw-rw-   0        0        0     2245 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_fx_light_emitting_image.py
+-rw-rw-rw-   0        0        0     3235 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_fx_lights.py
+-rw-rw-rw-   0        0        0     1984 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_get_value_from_elements.py
+-rw-rw-rw-   0        0        0     1376 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_grouping.py
+-rw-rw-rw-   0        0        0     1112 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_grouping_without_sorting.py
+-rw-rw-rw-   0        0        0     2575 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_groups_of_groups.py
+-rw-rw-rw-   0        0        0     3731 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_guess_the_number.py
+-rw-rw-rw-   0        0        0     1573 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_helper.py
+-rw-rw-rw-   0        0        0      982 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_heterogeneous_texts.py
+-rw-rw-rw-   0        0        0      685 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_image_with_text.py
+-rw-rw-rw-   0        0        0     1322 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_imagebutton.py
+-rw-rw-rw-   0        0        0     1532 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_integration_in_existing_code.py
+-rw-rw-rw-   0        0        0     1316 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_labels.py
+-rw-rw-rw-   0        0        0     3028 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_launch.py
+-rw-rw-rw-   0        0        0     1287 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_lifebar.py
+-rw-rw-rw-   0        0        0     1305 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_look_tune.py
+-rw-rw-rw-   0        0        0     2297 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_rich_text.py
+-rw-rw-rw-   0        0        0     1307 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_set_default_font.py
+-rw-rw-rw-   0        0        0     2128 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_shadows.py
+-rw-rw-rw-   0        0        0     3051 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_showcase_themes.py
+-rw-rw-rw-   0        0        0     3184 2023-04-24 16:00:12.000000 thorpy-2.0.4/thorpy/examples/_example_showcase_themes2.py
+-rw-rw-rw-   0        0        0     2119 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_showcase_themes_buttons.py
+-rw-rw-rw-   0        0        0     1500 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_showfps.py
+-rw-rw-rw-   0        0        0     1660 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_slider.py
+-rw-rw-rw-   0        0        0     2460 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_text_input.py
+-rw-rw-rw-   0        0        0     2765 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_text_width.py
+-rw-rw-rw-   0        0        0     1431 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_togglables_pool.py
+-rw-rw-rw-   0        0        0     1105 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_user_choices.py
+-rw-rw-rw-   0        0        0     1431 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_user_choices2.py
+-rw-rw-rw-   0        0        0     2051 2023-04-24 16:01:46.000000 thorpy-2.0.4/thorpy/examples/_example_user_chooses_font.py
+-rw-rw-rw-   0        0        0     2219 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_waiting_bar.py
+-rw-rw-rw-   0        0        0     4520 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/gametools.py
+-rw-rw-rw-   0        0        0    28781 2023-04-22 19:22:36.000000 thorpy-2.0.4/thorpy/graphics.py
+-rw-rw-rw-   0        0        0     6068 2023-04-24 15:17:59.000000 thorpy-2.0.4/thorpy/loops.py
+-rw-rw-rw-   0        0        0     2639 2023-04-22 15:23:24.000000 thorpy-2.0.4/thorpy/monitoring.py
+-rw-rw-rw-   0        0        0      467 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/parameters.py
+-rw-rw-rw-   0        0        0      625 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/setup.py
+-rw-rw-rw-   0        0        0     3727 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/shadows.py
+-rw-rw-rw-   0        0        0     2540 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/sorting.py
+-rw-rw-rw-   0        0        0     2307 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/sound.py
+-rw-rw-rw-   0        0        0    35577 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/styles.py
+-rw-rw-rw-   0        0        0    32875 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/themes.py
+drwxrwxrwx   0        0        0        0 2023-05-04 15:32:41.635264 thorpy-2.0.4/thorpy.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-05-04 15:32:41.000000 thorpy-2.0.4/thorpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2349 2023-05-04 15:32:41.000000 thorpy-2.0.4/thorpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 15:32:41.000000 thorpy-2.0.4/thorpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 15:32:41.000000 thorpy-2.0.4/thorpy.egg-info/top_level.txt
```

### Comparing `thorpy-2.0.3/LICENSE` & `thorpy-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/README.md` & `thorpy-2.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 * Nothing special to do for the doc description, it is automatic as long as you indicate things in docstrings
 * For the image, put an image with the same name as the class (but lowercase) in the doc folder
 
 Files to upload to server:
 * All things inside to_upload/
 
 Upload on PyPi :
-1. Copy paste the actual thorpy folder to ./thorpy/
-2. Change version number in both setup.py AND thorpy/__init__.py
+1. Copy paste the actual thorpy folder (on my computer its 'Thorpy2') to ./thorpy/
+2. Change version number in both setup.py AND thorpy/__init__.py (and dont forget the actual thorpy git !)
 3. pip install twine setuptools wheel
 4. python setup.py sdist bdist_wheel
 5. twine upload dist/*
 Account : Thorpy
 Pwd : Don't worry
```

### Comparing `thorpy-2.0.3/setup.py` & `thorpy-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 setup(name='thorpy',
-      version='2.0.3',
+      version='2.0.4',
       description='GUI library for pygame',
       long_description='ThorPy is a non-intrusive, straightforward GUI kit for Pygame.',
       author='Yann Thorimbert',
       author_email='yann.thorimbert@gmail.com',
       url='http://www.thorpy.org/',
       keywords=['pygame', 'gui', 'menus', 'buttons', 'widgets', 'user interface', 'toolkit'],
       packages=find_packages(),
```

### Comparing `thorpy-2.0.3/thorpy/__init__.py` & `thorpy-2.0.4/thorpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 #Import styling functions
 from .themes import theme_classic, theme_human, theme_round, theme_simple, theme_text, theme_game2
 from .themes import theme_round_gradient, theme_round2
 from .themes import theme_text_dark, theme_game1, set_style_attr, refresh_all_elements_style, get_theme_bck_color, get_theme_main_bck_color
 from .styles import get_default_font, set_default_font, get_text_size, get_text_height
 
 
-__version__ = "2.0.3"
-
+__version__ = "2.0.4"
 
 def set_screen(screen):
     """Set the default surface display for all elements that will be created after this call."""
     parameters.screen = screen
 
 def get_screen():
     """Get the default surface display for elements that will be created after this call."""
```

### Comparing `thorpy-2.0.3/thorpy/canonical.py` & `thorpy-2.0.4/thorpy/canonical.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,14 +362,16 @@
         <what> : either a pygame Rect, a pygame Surface or a thorpy element.
         It is also possible to specify what = 'screen' as a shortcut for screen's rect.
         """
         if isinstance(what, str):
             rect = p.screen.get_rect()
         elif not isinstance(what, pygame.Rect): #works both for surfaces and elements.
             rect = what.get_rect()
+        else:
+            rect = what
         self.set_center(*rect.center)
 
     def stick_to(self, other, self_side, other_side, delta=(0,0), move_x=True, move_y=True):
         """Sticks the element to another.
         ***Mandatory arguments***
         <other> : another element or pygame surface.
         <self_side> : side of the element beeing sticked. Can be 'left', 'right', 'top' or 'bottom'.
```

### Comparing `thorpy-2.0.3/thorpy/elements.py` & `thorpy-2.0.4/thorpy/elements.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_alert.py` & `thorpy-2.0.4/thorpy/examples/_example_alert.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_anim_move.py` & `thorpy-2.0.4/thorpy/examples/_example_anim_move.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_animatedgif.py` & `thorpy-2.0.4/thorpy/examples/_example_animatedgif.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_box.py` & `thorpy-2.0.4/thorpy/examples/_example_box.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_button_helloworld.py` & `thorpy-2.0.4/thorpy/examples/_example_button_helloworld.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_color_gradient.py` & `thorpy-2.0.4/thorpy/examples/_example_color_gradient.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_colorpicker.py` & `thorpy-2.0.4/thorpy/examples/_example_colorpicker.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_colorpicker2.py` & `thorpy-2.0.4/thorpy/examples/_example_colorpicker2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_colorpicker_fine_tuning.py` & `thorpy-2.0.4/thorpy/examples/_example_colorpicker_fine_tuning.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_create_style.py` & `thorpy-2.0.4/thorpy/examples/_example_create_style.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_create_style2.py` & `thorpy-2.0.4/thorpy/examples/_example_create_style2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_custom_theme.py` & `thorpy-2.0.4/thorpy/examples/_example_custom_theme.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_dropdownlist.py` & `thorpy-2.0.4/thorpy/examples/_example_dropdownlist.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_events.py` & `thorpy-2.0.4/thorpy/examples/_example_events.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_filebrowser.py` & `thorpy-2.0.4/thorpy/examples/_example_filebrowser.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_fx_light_emitting_image.py` & `thorpy-2.0.4/thorpy/examples/_example_fx_light_emitting_image.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_fx_lights.py` & `thorpy-2.0.4/thorpy/examples/_example_fx_lights.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_get_value_from_elements.py` & `thorpy-2.0.4/thorpy/examples/_example_get_value_from_elements.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_grouping.py` & `thorpy-2.0.4/thorpy/examples/_example_grouping.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_grouping_without_sorting.py` & `thorpy-2.0.4/thorpy/examples/_example_grouping_without_sorting.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_groups_of_groups.py` & `thorpy-2.0.4/thorpy/examples/_example_groups_of_groups.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_guess_the_number.py` & `thorpy-2.0.4/thorpy/examples/_example_guess_the_number.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_helper.py` & `thorpy-2.0.4/thorpy/examples/_example_helper.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_heterogeneous_texts.py` & `thorpy-2.0.4/thorpy/examples/_example_heterogeneous_texts.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_image_with_text.py` & `thorpy-2.0.4/thorpy/examples/_example_image_with_text.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_imagebutton.py` & `thorpy-2.0.4/thorpy/examples/_example_imagebutton.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_integration_in_existing_code.py` & `thorpy-2.0.4/thorpy/examples/_example_integration_in_existing_code.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_labels.py` & `thorpy-2.0.4/thorpy/examples/_example_labels.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_launch.py` & `thorpy-2.0.4/thorpy/examples/_example_launch.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_lifebar.py` & `thorpy-2.0.4/thorpy/examples/_example_lifebar.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_look_tune.py` & `thorpy-2.0.4/thorpy/examples/_example_look_tune.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_rich_text.py` & `thorpy-2.0.4/thorpy/examples/_example_rich_text.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_set_default_font.py` & `thorpy-2.0.4/thorpy/examples/_example_set_default_font.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_shadows.py` & `thorpy-2.0.4/thorpy/examples/_example_shadows.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_showcase_themes.py` & `thorpy-2.0.4/thorpy/examples/_example_showcase_themes.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_showcase_themes2.py` & `thorpy-2.0.4/thorpy/examples/_example_showcase_themes2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_showcase_themes_buttons.py` & `thorpy-2.0.4/thorpy/examples/_example_showcase_themes_buttons.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_showfps.py` & `thorpy-2.0.4/thorpy/examples/_example_showfps.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_slider.py` & `thorpy-2.0.4/thorpy/examples/_example_slider.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_text_input.py` & `thorpy-2.0.4/thorpy/examples/_example_text_input.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_text_width.py` & `thorpy-2.0.4/thorpy/examples/_example_text_width.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_togglables_pool.py` & `thorpy-2.0.4/thorpy/examples/_example_togglables_pool.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_user_choices.py` & `thorpy-2.0.4/thorpy/examples/_example_user_choices.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_user_choices2.py` & `thorpy-2.0.4/thorpy/examples/_example_user_choices2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_user_chooses_font.py` & `thorpy-2.0.4/thorpy/examples/_example_user_chooses_font.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/examples/_example_waiting_bar.py` & `thorpy-2.0.4/thorpy/examples/_example_waiting_bar.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/gametools.py` & `thorpy-2.0.4/thorpy/gametools.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/graphics.py` & `thorpy-2.0.4/thorpy/graphics.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/loops.py` & `thorpy-2.0.4/thorpy/loops.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/monitoring.py` & `thorpy-2.0.4/thorpy/monitoring.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/setup.py` & `thorpy-2.0.4/thorpy/setup.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/shadows.py` & `thorpy-2.0.4/thorpy/shadows.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/sorting.py` & `thorpy-2.0.4/thorpy/sorting.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/sound.py` & `thorpy-2.0.4/thorpy/sound.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/styles.py` & `thorpy-2.0.4/thorpy/styles.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy/themes.py` & `thorpy-2.0.4/thorpy/themes.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.3/thorpy.egg-info/SOURCES.txt` & `thorpy-2.0.4/thorpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

