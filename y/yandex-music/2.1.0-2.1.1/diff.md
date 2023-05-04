# Comparing `tmp/yandex-music-2.1.0.tar.gz` & `tmp/yandex-music-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yandex-music-2.1.0.tar", last modified: Sun Apr 23 00:46:42 2023, max compression
+gzip compressed data, was "dist/yandex-music-2.1.1.tar", last modified: Thu May  4 19:14:42 2023, max compression
```

## Comparing `yandex-music-2.1.0.tar` & `yandex-music-2.1.1.tar`

### file list

```diff
@@ -1,298 +1,298 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    31383 2023-04-23 00:46:33.000000 yandex-music-2.1.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-23 00:46:33.000000 yandex-music-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-23 00:46:33.000000 yandex-music-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23008 2023-04-23 00:46:42.000000 yandex-music-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-04-23 00:46:33.000000 yandex-music-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:46:42.000000 yandex-music-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-23 00:46:33.000000 yandex-music-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34230 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_ad_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_album.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_album_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_alert_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_artist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_artist_albums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_artist_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_artist_tracks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_auto_renewable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_best.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_block_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_brief_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_case_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_chart_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_chart_info_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_chart_info_menu_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_chart_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_contest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_convert_track_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_custom_wave.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_day.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_deactivation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_discrete_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_download_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_generated_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_genre.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_icon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_invocation_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_landing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_landing_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_licence_text_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_like.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_lyrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_lyrics_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_lyrics_major.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_made_for.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_major.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_mix_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_non_auto_renewable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_open_graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_pager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_passport_phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_permission_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_personal_playlists_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_play_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_play_contexts_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_play_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_playlist_absence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_playlist_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_playlist_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_plus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_poetry_lover_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_promo_code_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_promotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_queue_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_r128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_ratings.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_renewable_remainder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_rotor_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_shot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_shot_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_shot_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_shot_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_sign_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_station.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_station_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_station_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_station_tracks_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_suggestions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_supplement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_tag_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_track_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_track_lyrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_track_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_track_short.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_track_short_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_track_with_ads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_tracks_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_tracks_similar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_user_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_video_supplement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_vinyl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/account/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/alert_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/auto_renewable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/deactivation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/non_auto_renewable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/passport_phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/plus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/product.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/renewable_remainder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/album/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/album/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/album/album.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/album/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/album/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/album/track_position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/artist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15692 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/artist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/artist_albums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/artist_tracks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/brief_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/ratings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/vinyl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   115301 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   116662 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/client_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/download_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/experiments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/feed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/album_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/artist_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/day.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/feed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/generated_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/track_with_ads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/genre/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/genre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/genre/genre.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/genre/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/genre/title.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/icon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/invocation_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/landing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/block_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/chart_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/chart_info_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/chart_info_menu_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/chart_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/landing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/landing_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/mix_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/personal_playlists_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/play_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/play_contexts_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/promotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/track_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/track_short_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/like.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/pager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/permission_alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/playlist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/brand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/case_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/contest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/custom_wave.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/made_for.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/open_graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/play_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    25913 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/playlist_absence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/playlist_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/playlist_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/tag_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/promo_code_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/queue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/queue/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/queue/queue_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/rotor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/ad_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/discrete_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/restrictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/rotor_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/station.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/station_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/station_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/station_tracks_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/search/best.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/search/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/search/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/search/suggestions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/shot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/shot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/shot/shot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/shot/shot_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/shot/shot_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/shot/shot_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/supplement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/supplement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/supplement/lyrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/supplement/supplement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/supplement/video_supplement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/track/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/licence_text_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/lyrics_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/lyrics_major.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/major.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/poetry_lover_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/r128.py
--rw-r--r--   0 runner    (1001) docker     (123)    26736 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/track_lyrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/tracks_similar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track_short.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/tracks_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/utils/convert_track_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/utils/difference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/utils/request_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/utils/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/utils/sign_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23008 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    31383 2023-05-04 19:14:29.000000 yandex-music-2.1.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-04 19:14:29.000000 yandex-music-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 19:14:29.000000 yandex-music-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23008 2023-05-04 19:14:42.000000 yandex-music-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-05-04 19:14:29.000000 yandex-music-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 19:14:42.000000 yandex-music-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-04 19:14:29.000000 yandex-music-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34230 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_ad_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_album.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_album_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_alert_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_artist_albums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_artist_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_artist_tracks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_auto_renewable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_best.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_block_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_brief_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_case_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_chart_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_chart_info_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_chart_info_menu_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_chart_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_contest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_convert_track_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_custom_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_deactivation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_discrete_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_download_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_generated_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_genre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_invocation_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_landing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_landing_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_licence_text_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_lyrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_lyrics_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_lyrics_major.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_made_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_major.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_mix_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_non_auto_renewable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_open_graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_pager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_passport_phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_permission_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_personal_playlists_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_play_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_play_contexts_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_play_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_playlist_absence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_playlist_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_playlist_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_poetry_lover_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_promo_code_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_queue_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_r128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_renewable_remainder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_rotor_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_shot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_shot_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_shot_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_shot_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_sign_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_station.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_station_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_station_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_station_tracks_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_suggestions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_tag_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_track_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_track_lyrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_track_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_track_short.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_track_short_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_track_with_ads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_tracks_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_tracks_similar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_user_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_video_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-04 19:14:29.000000 yandex-music-2.1.1/tests/test_vinyl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/alert_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/auto_renewable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/deactivation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/non_auto_renewable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/passport_phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/renewable_remainder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/account/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/album/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/album/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/album/album.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/album/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/album/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/album/track_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/artist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/artist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15692 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/artist/artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/artist/artist_albums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/artist/artist_tracks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/artist/brief_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/artist/counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/artist/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/artist/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/artist/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/artist/vinyl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115301 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116662 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/client_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/download_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/experiments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/feed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/feed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/feed/album_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/feed/artist_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/feed/day.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/feed/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/feed/feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/feed/generated_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/feed/track_with_ads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/genre/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/genre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/genre/genre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/genre/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/genre/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/invocation_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/landing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/block_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/chart_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/chart_info_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/chart_info_menu_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/chart_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/landing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/landing_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/mix_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/personal_playlists_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/play_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/play_contexts_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/track_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/landing/track_short_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/pager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/permission_alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/playlist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/case_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/contest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/custom_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/made_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/open_graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/play_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25913 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/playlist_absence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/playlist_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/playlist_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/tag_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/playlist/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/promo_code_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/queue/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/queue/queue_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/rotor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/rotor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/rotor/ad_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/rotor/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/rotor/discrete_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/rotor/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/rotor/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/rotor/restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/rotor/rotor_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/rotor/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/rotor/station.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/rotor/station_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/rotor/station_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/rotor/station_tracks_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/rotor/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/search/best.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/search/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/search/suggestions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/shot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/shot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/shot/shot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/shot/shot_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/shot/shot_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/shot/shot_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/supplement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/supplement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/supplement/lyrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/supplement/supplement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/supplement/video_supplement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/track/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/track/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/track/licence_text_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/track/lyrics_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/track/lyrics_major.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/track/major.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/track/meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/track/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/track/poetry_lover_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/track/r128.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26736 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/track/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/track/track_lyrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/track/tracks_similar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/track_short.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/tracks_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/utils/convert_track_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/utils/difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/utils/request_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/utils/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/utils/sign_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-04 19:14:29.000000 yandex-music-2.1.1/yandex_music/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23008 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 19:14:42.000000 yandex-music-2.1.1/yandex_music.egg-info/top_level.txt
```

### Comparing `yandex-music-2.1.0/CHANGES.md` & `yandex-music-2.1.1/CHANGES.md`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/LICENSE` & `yandex-music-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/PKG-INFO` & `yandex-music-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandex-music
-Version: 2.1.0
+Version: 2.1.1
 Summary: Неофициальная Python библиотека для работы с API сервиса Яндекс.Музыка.
 Home-page: https://github.com/MarshalX/yandex-music-api/
 Author: Ilya (Marshal)
 Author-email: ilya@marshal.dev
 License: LGPLv3
 Project-URL: Documentation, https://yandex-music.rtfd.io
 Project-URL: Telegram chat, https://t.me/yandex_music_api
```

### Comparing `yandex-music-2.1.0/README.md` & `yandex-music-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/setup.py` & `yandex-music-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/__init__.py` & `yandex-music-2.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/conftest.py` & `yandex-music-2.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_account.py` & `yandex-music-2.1.1/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_ad_params.py` & `yandex-music-2.1.1/tests/test_ad_params.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_album.py` & `yandex-music-2.1.1/tests/test_album.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_album_event.py` & `yandex-music-2.1.1/tests/test_album_event.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_alert.py` & `yandex-music-2.1.1/tests/test_alert.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_alert_button.py` & `yandex-music-2.1.1/tests/test_alert_button.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_artist.py` & `yandex-music-2.1.1/tests/test_artist.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_artist_albums.py` & `yandex-music-2.1.1/tests/test_artist_albums.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_artist_event.py` & `yandex-music-2.1.1/tests/test_artist_event.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_artist_tracks.py` & `yandex-music-2.1.1/tests/test_artist_tracks.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_auto_renewable.py` & `yandex-music-2.1.1/tests/test_auto_renewable.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_best.py` & `yandex-music-2.1.1/tests/test_best.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_block.py` & `yandex-music-2.1.1/tests/test_block.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_block_entity.py` & `yandex-music-2.1.1/tests/test_block_entity.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_brand.py` & `yandex-music-2.1.1/tests/test_brand.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_brief_info.py` & `yandex-music-2.1.1/tests/test_brief_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_case_forms.py` & `yandex-music-2.1.1/tests/test_case_forms.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_chart.py` & `yandex-music-2.1.1/tests/test_chart.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_chart_info.py` & `yandex-music-2.1.1/tests/test_chart_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_chart_info_menu.py` & `yandex-music-2.1.1/tests/test_chart_info_menu.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_chart_info_menu_item.py` & `yandex-music-2.1.1/tests/test_chart_info_menu_item.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_chart_item.py` & `yandex-music-2.1.1/tests/test_chart_item.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_contest.py` & `yandex-music-2.1.1/tests/test_contest.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_context.py` & `yandex-music-2.1.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_convert_track_id.py` & `yandex-music-2.1.1/tests/test_convert_track_id.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_counts.py` & `yandex-music-2.1.1/tests/test_counts.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_cover.py` & `yandex-music-2.1.1/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_custom_wave.py` & `yandex-music-2.1.1/tests/test_custom_wave.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_dashboard.py` & `yandex-music-2.1.1/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_day.py` & `yandex-music-2.1.1/tests/test_day.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_deactivation.py` & `yandex-music-2.1.1/tests/test_deactivation.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_deprecation.py` & `yandex-music-2.1.1/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_description.py` & `yandex-music-2.1.1/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_discrete_scale.py` & `yandex-music-2.1.1/tests/test_discrete_scale.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_download_info.py` & `yandex-music-2.1.1/tests/test_download_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_enum.py` & `yandex-music-2.1.1/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_event.py` & `yandex-music-2.1.1/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_feed.py` & `yandex-music-2.1.1/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_generated_playlist.py` & `yandex-music-2.1.1/tests/test_generated_playlist.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_genre.py` & `yandex-music-2.1.1/tests/test_genre.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_icon.py` & `yandex-music-2.1.1/tests/test_icon.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_id.py` & `yandex-music-2.1.1/tests/test_id.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_images.py` & `yandex-music-2.1.1/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_invocation_info.py` & `yandex-music-2.1.1/tests/test_invocation_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_label.py` & `yandex-music-2.1.1/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_landing.py` & `yandex-music-2.1.1/tests/test_landing.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_landing_list.py` & `yandex-music-2.1.1/tests/test_landing_list.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_licence_text_part.py` & `yandex-music-2.1.1/tests/test_licence_text_part.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_like.py` & `yandex-music-2.1.1/tests/test_like.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_link.py` & `yandex-music-2.1.1/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_lyrics.py` & `yandex-music-2.1.1/tests/test_lyrics.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_lyrics_info.py` & `yandex-music-2.1.1/tests/test_lyrics_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_lyrics_major.py` & `yandex-music-2.1.1/tests/test_lyrics_major.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_made_for.py` & `yandex-music-2.1.1/tests/test_made_for.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_major.py` & `yandex-music-2.1.1/tests/test_major.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_meta_data.py` & `yandex-music-2.1.1/tests/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_mix_link.py` & `yandex-music-2.1.1/tests/test_mix_link.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_non_auto_renewable.py` & `yandex-music-2.1.1/tests/test_non_auto_renewable.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_normalization.py` & `yandex-music-2.1.1/tests/test_normalization.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_open_graph_data.py` & `yandex-music-2.1.1/tests/test_open_graph_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_operator.py` & `yandex-music-2.1.1/tests/test_operator.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_pager.py` & `yandex-music-2.1.1/tests/test_pager.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_passport_phone.py` & `yandex-music-2.1.1/tests/test_passport_phone.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_permission_alerts.py` & `yandex-music-2.1.1/tests/test_permission_alerts.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_permissions.py` & `yandex-music-2.1.1/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_personal_playlists_data.py` & `yandex-music-2.1.1/tests/test_personal_playlists_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_play_context.py` & `yandex-music-2.1.1/tests/test_play_context.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_play_contexts_data.py` & `yandex-music-2.1.1/tests/test_play_contexts_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_play_counter.py` & `yandex-music-2.1.1/tests/test_play_counter.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_playlist.py` & `yandex-music-2.1.1/tests/test_playlist.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_playlist_absence.py` & `yandex-music-2.1.1/tests/test_playlist_absence.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_playlist_id.py` & `yandex-music-2.1.1/tests/test_playlist_id.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_playlist_recommendations.py` & `yandex-music-2.1.1/tests/test_playlist_recommendations.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_plus.py` & `yandex-music-2.1.1/tests/test_plus.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_poetry_lover_match.py` & `yandex-music-2.1.1/tests/test_poetry_lover_match.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_price.py` & `yandex-music-2.1.1/tests/test_price.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_product.py` & `yandex-music-2.1.1/tests/test_product.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_promo_code_status.py` & `yandex-music-2.1.1/tests/test_promo_code_status.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_promotion.py` & `yandex-music-2.1.1/tests/test_promotion.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_queue.py` & `yandex-music-2.1.1/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_queue_item.py` & `yandex-music-2.1.1/tests/test_queue_item.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_r128.py` & `yandex-music-2.1.1/tests/test_r128.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_ratings.py` & `yandex-music-2.1.1/tests/test_ratings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_renewable_remainder.py` & `yandex-music-2.1.1/tests/test_renewable_remainder.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_restrictions.py` & `yandex-music-2.1.1/tests/test_restrictions.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_rotor_settings.py` & `yandex-music-2.1.1/tests/test_rotor_settings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_search.py` & `yandex-music-2.1.1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_search_result.py` & `yandex-music-2.1.1/tests/test_search_result.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_sequence.py` & `yandex-music-2.1.1/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_settings.py` & `yandex-music-2.1.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_shot.py` & `yandex-music-2.1.1/tests/test_shot.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_shot_data.py` & `yandex-music-2.1.1/tests/test_shot_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_shot_event.py` & `yandex-music-2.1.1/tests/test_shot_event.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_shot_type.py` & `yandex-music-2.1.1/tests/test_shot_type.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_sign_request.py` & `yandex-music-2.1.1/tests/test_sign_request.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_station.py` & `yandex-music-2.1.1/tests/test_station.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_station_data.py` & `yandex-music-2.1.1/tests/test_station_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_station_result.py` & `yandex-music-2.1.1/tests/test_station_result.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_station_tracks_result.py` & `yandex-music-2.1.1/tests/test_station_tracks_result.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_status.py` & `yandex-music-2.1.1/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_subscription.py` & `yandex-music-2.1.1/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_suggestions.py` & `yandex-music-2.1.1/tests/test_suggestions.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_supplement.py` & `yandex-music-2.1.1/tests/test_supplement.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_tag.py` & `yandex-music-2.1.1/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_tag_result.py` & `yandex-music-2.1.1/tests/test_tag_result.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_title.py` & `yandex-music-2.1.1/tests/test_title.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_track.py` & `yandex-music-2.1.1/tests/test_track.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_track_id.py` & `yandex-music-2.1.1/tests/test_track_id.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_track_lyrics.py` & `yandex-music-2.1.1/tests/test_track_lyrics.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_track_position.py` & `yandex-music-2.1.1/tests/test_track_position.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_track_short.py` & `yandex-music-2.1.1/tests/test_track_short.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_track_short_old.py` & `yandex-music-2.1.1/tests/test_track_short_old.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_track_with_ads.py` & `yandex-music-2.1.1/tests/test_track_with_ads.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_tracks_list.py` & `yandex-music-2.1.1/tests/test_tracks_list.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_tracks_similar.py` & `yandex-music-2.1.1/tests/test_tracks_similar.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_user.py` & `yandex-music-2.1.1/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_user_settings.py` & `yandex-music-2.1.1/tests/test_user_settings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_value.py` & `yandex-music-2.1.1/tests/test_value.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_video.py` & `yandex-music-2.1.1/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_video_supplement.py` & `yandex-music-2.1.1/tests/test_video_supplement.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/tests/test_vinyl.py` & `yandex-music-2.1.1/tests/test_vinyl.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/__init__.py` & `yandex-music-2.1.1/yandex_music/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 __license__ = 'GNU Lesser General Public License v3 (LGPLv3)'
 __copyright__ = 'Copyright (C) 2019-2023 Ilya (Marshal) <https://github.com/MarshalX>'
 
 from .base import YandexMusicObject
 
 from .settings import Settings
 from .permission_alerts import PermissionAlerts
```

### Comparing `yandex-music-2.1.0/yandex_music/account/account.py` & `yandex-music-2.1.1/yandex_music/account/account.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/alert.py` & `yandex-music-2.1.1/yandex_music/account/alert.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/alert_button.py` & `yandex-music-2.1.1/yandex_music/account/alert_button.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/auto_renewable.py` & `yandex-music-2.1.1/yandex_music/account/auto_renewable.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/deactivation.py` & `yandex-music-2.1.1/yandex_music/account/deactivation.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/non_auto_renewable.py` & `yandex-music-2.1.1/yandex_music/account/non_auto_renewable.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/operator.py` & `yandex-music-2.1.1/yandex_music/account/operator.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/passport_phone.py` & `yandex-music-2.1.1/yandex_music/account/passport_phone.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/permissions.py` & `yandex-music-2.1.1/yandex_music/account/permissions.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/plus.py` & `yandex-music-2.1.1/yandex_music/account/plus.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/price.py` & `yandex-music-2.1.1/yandex_music/account/price.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/product.py` & `yandex-music-2.1.1/yandex_music/account/product.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/renewable_remainder.py` & `yandex-music-2.1.1/yandex_music/account/renewable_remainder.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/status.py` & `yandex-music-2.1.1/yandex_music/account/status.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/subscription.py` & `yandex-music-2.1.1/yandex_music/account/subscription.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/account/user_settings.py` & `yandex-music-2.1.1/yandex_music/account/user_settings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/album/album.py` & `yandex-music-2.1.1/yandex_music/album/album.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/album/deprecation.py` & `yandex-music-2.1.1/yandex_music/album/deprecation.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/album/label.py` & `yandex-music-2.1.1/yandex_music/album/label.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/album/track_position.py` & `yandex-music-2.1.1/yandex_music/album/track_position.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/artist/artist.py` & `yandex-music-2.1.1/yandex_music/artist/artist.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/artist/artist_albums.py` & `yandex-music-2.1.1/yandex_music/artist/artist_albums.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/artist/artist_tracks.py` & `yandex-music-2.1.1/yandex_music/artist/artist_tracks.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/artist/brief_info.py` & `yandex-music-2.1.1/yandex_music/artist/brief_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/artist/counts.py` & `yandex-music-2.1.1/yandex_music/artist/counts.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/artist/description.py` & `yandex-music-2.1.1/yandex_music/artist/description.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/artist/link.py` & `yandex-music-2.1.1/yandex_music/artist/link.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/artist/ratings.py` & `yandex-music-2.1.1/yandex_music/artist/ratings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/artist/vinyl.py` & `yandex-music-2.1.1/yandex_music/artist/vinyl.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/base.py` & `yandex-music-2.1.1/yandex_music/base.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/client.py` & `yandex-music-2.1.1/yandex_music/client.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/client_async.py` & `yandex-music-2.1.1/yandex_music/client_async.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/cover.py` & `yandex-music-2.1.1/yandex_music/cover.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/download_info.py` & `yandex-music-2.1.1/yandex_music/download_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/exceptions.py` & `yandex-music-2.1.1/yandex_music/exceptions.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/experiments.py` & `yandex-music-2.1.1/yandex_music/experiments.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/feed/album_event.py` & `yandex-music-2.1.1/yandex_music/feed/album_event.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/feed/artist_event.py` & `yandex-music-2.1.1/yandex_music/feed/artist_event.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/feed/day.py` & `yandex-music-2.1.1/yandex_music/feed/day.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/feed/event.py` & `yandex-music-2.1.1/yandex_music/feed/event.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/feed/feed.py` & `yandex-music-2.1.1/yandex_music/feed/feed.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/feed/generated_playlist.py` & `yandex-music-2.1.1/yandex_music/feed/generated_playlist.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/feed/track_with_ads.py` & `yandex-music-2.1.1/yandex_music/feed/track_with_ads.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/genre/genre.py` & `yandex-music-2.1.1/yandex_music/genre/genre.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/genre/images.py` & `yandex-music-2.1.1/yandex_music/genre/images.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/genre/title.py` & `yandex-music-2.1.1/yandex_music/genre/title.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/icon.py` & `yandex-music-2.1.1/yandex_music/icon.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/invocation_info.py` & `yandex-music-2.1.1/yandex_music/invocation_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/block.py` & `yandex-music-2.1.1/yandex_music/landing/block.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/block_entity.py` & `yandex-music-2.1.1/yandex_music/landing/block_entity.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/chart.py` & `yandex-music-2.1.1/yandex_music/landing/chart.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/chart_info.py` & `yandex-music-2.1.1/yandex_music/landing/chart_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/chart_info_menu.py` & `yandex-music-2.1.1/yandex_music/landing/chart_info_menu.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/chart_info_menu_item.py` & `yandex-music-2.1.1/yandex_music/landing/chart_info_menu_item.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/chart_item.py` & `yandex-music-2.1.1/yandex_music/landing/chart_item.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/landing.py` & `yandex-music-2.1.1/yandex_music/landing/landing.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/landing_list.py` & `yandex-music-2.1.1/yandex_music/landing/landing_list.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/mix_link.py` & `yandex-music-2.1.1/yandex_music/landing/mix_link.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/personal_playlists_data.py` & `yandex-music-2.1.1/yandex_music/landing/personal_playlists_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/play_context.py` & `yandex-music-2.1.1/yandex_music/landing/play_context.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/play_contexts_data.py` & `yandex-music-2.1.1/yandex_music/landing/play_contexts_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/promotion.py` & `yandex-music-2.1.1/yandex_music/landing/promotion.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/track_id.py` & `yandex-music-2.1.1/yandex_music/landing/track_id.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/landing/track_short_old.py` & `yandex-music-2.1.1/yandex_music/landing/track_short_old.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/like.py` & `yandex-music-2.1.1/yandex_music/like.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/pager.py` & `yandex-music-2.1.1/yandex_music/pager.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/permission_alerts.py` & `yandex-music-2.1.1/yandex_music/permission_alerts.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/playlist/brand.py` & `yandex-music-2.1.1/yandex_music/playlist/brand.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/playlist/case_forms.py` & `yandex-music-2.1.1/yandex_music/playlist/case_forms.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/playlist/contest.py` & `yandex-music-2.1.1/yandex_music/playlist/contest.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/playlist/custom_wave.py` & `yandex-music-2.1.1/yandex_music/playlist/custom_wave.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/playlist/made_for.py` & `yandex-music-2.1.1/yandex_music/playlist/made_for.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/playlist/open_graph_data.py` & `yandex-music-2.1.1/yandex_music/playlist/open_graph_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/playlist/play_counter.py` & `yandex-music-2.1.1/yandex_music/playlist/play_counter.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/playlist/playlist.py` & `yandex-music-2.1.1/yandex_music/playlist/playlist.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/playlist/playlist_absence.py` & `yandex-music-2.1.1/yandex_music/playlist/playlist_absence.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/playlist/playlist_id.py` & `yandex-music-2.1.1/yandex_music/playlist/playlist_id.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/playlist/playlist_recommendation.py` & `yandex-music-2.1.1/yandex_music/playlist/playlist_recommendation.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/playlist/tag.py` & `yandex-music-2.1.1/yandex_music/playlist/tag.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/playlist/tag_result.py` & `yandex-music-2.1.1/yandex_music/playlist/tag_result.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/playlist/user.py` & `yandex-music-2.1.1/yandex_music/playlist/user.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/promo_code_status.py` & `yandex-music-2.1.1/yandex_music/promo_code_status.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/queue/context.py` & `yandex-music-2.1.1/yandex_music/queue/context.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/queue/queue.py` & `yandex-music-2.1.1/yandex_music/queue/queue.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/queue/queue_item.py` & `yandex-music-2.1.1/yandex_music/queue/queue_item.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/rotor/ad_params.py` & `yandex-music-2.1.1/yandex_music/rotor/ad_params.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/rotor/dashboard.py` & `yandex-music-2.1.1/yandex_music/rotor/dashboard.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/rotor/discrete_scale.py` & `yandex-music-2.1.1/yandex_music/rotor/discrete_scale.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/rotor/enum.py` & `yandex-music-2.1.1/yandex_music/rotor/enum.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/rotor/id.py` & `yandex-music-2.1.1/yandex_music/rotor/id.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/rotor/restrictions.py` & `yandex-music-2.1.1/yandex_music/rotor/restrictions.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/rotor/rotor_settings.py` & `yandex-music-2.1.1/yandex_music/rotor/rotor_settings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/rotor/sequence.py` & `yandex-music-2.1.1/yandex_music/rotor/sequence.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/rotor/station.py` & `yandex-music-2.1.1/yandex_music/rotor/station.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/rotor/station_data.py` & `yandex-music-2.1.1/yandex_music/rotor/station_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/rotor/station_result.py` & `yandex-music-2.1.1/yandex_music/rotor/station_result.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/rotor/station_tracks_result.py` & `yandex-music-2.1.1/yandex_music/rotor/station_tracks_result.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/rotor/value.py` & `yandex-music-2.1.1/yandex_music/rotor/value.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/search/best.py` & `yandex-music-2.1.1/yandex_music/search/best.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/search/search.py` & `yandex-music-2.1.1/yandex_music/search/search.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/search/search_result.py` & `yandex-music-2.1.1/yandex_music/search/search_result.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/search/suggestions.py` & `yandex-music-2.1.1/yandex_music/search/suggestions.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/settings.py` & `yandex-music-2.1.1/yandex_music/settings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/shot/shot.py` & `yandex-music-2.1.1/yandex_music/shot/shot.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/shot/shot_data.py` & `yandex-music-2.1.1/yandex_music/shot/shot_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/shot/shot_event.py` & `yandex-music-2.1.1/yandex_music/shot/shot_event.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/shot/shot_type.py` & `yandex-music-2.1.1/yandex_music/shot/shot_type.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/supplement/lyrics.py` & `yandex-music-2.1.1/yandex_music/supplement/lyrics.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/supplement/supplement.py` & `yandex-music-2.1.1/yandex_music/supplement/supplement.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/supplement/video_supplement.py` & `yandex-music-2.1.1/yandex_music/supplement/video_supplement.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/track/licence_text_part.py` & `yandex-music-2.1.1/yandex_music/track/licence_text_part.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/track/lyrics_info.py` & `yandex-music-2.1.1/yandex_music/track/lyrics_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/track/lyrics_major.py` & `yandex-music-2.1.1/yandex_music/track/lyrics_major.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/track/major.py` & `yandex-music-2.1.1/yandex_music/track/major.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/track/meta_data.py` & `yandex-music-2.1.1/yandex_music/track/meta_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/track/normalization.py` & `yandex-music-2.1.1/yandex_music/track/normalization.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/track/poetry_lover_match.py` & `yandex-music-2.1.1/yandex_music/track/poetry_lover_match.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/track/r128.py` & `yandex-music-2.1.1/yandex_music/track/r128.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/track/track.py` & `yandex-music-2.1.1/yandex_music/track/track.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/track/track_lyrics.py` & `yandex-music-2.1.1/yandex_music/track/track_lyrics.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/track/tracks_similar.py` & `yandex-music-2.1.1/yandex_music/track/tracks_similar.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/track_short.py` & `yandex-music-2.1.1/yandex_music/track_short.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/tracks_list.py` & `yandex-music-2.1.1/yandex_music/tracks_list.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/utils/convert_track_id.py` & `yandex-music-2.1.1/yandex_music/utils/convert_track_id.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/utils/difference.py` & `yandex-music-2.1.1/yandex_music/utils/difference.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/utils/request.py` & `yandex-music-2.1.1/yandex_music/utils/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 if TYPE_CHECKING:
     from yandex_music import Client
 
 
 USER_AGENT = 'Yandex-Music-API'
 HEADERS = {
-    'X-Yandex-Music-Client': 'YandexMusicAndroid/23020251',
+    'X-Yandex-Music-Client': 'YandexMusicAndroid/24023231',
 }
 DEFAULT_TIMEOUT = 5
 
 reserved_names = keyword.kwlist + ['client']
 
 logging.getLogger('urllib3').setLevel(logging.WARNING)
```

### Comparing `yandex-music-2.1.0/yandex_music/utils/request_async.py` & `yandex-music-2.1.1/yandex_music/utils/request_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 if TYPE_CHECKING:
     from yandex_music import Client
 
 
 USER_AGENT = 'Yandex-Music-API'
 HEADERS = {
-    'X-Yandex-Music-Client': 'YandexMusicAndroid/23020251',
+    'X-Yandex-Music-Client': 'YandexMusicAndroid/24023231',
 }
 DEFAULT_TIMEOUT = 5
 
 reserved_names = keyword.kwlist + ['client']
 
 logging.getLogger('urllib3').setLevel(logging.WARNING)
```

### Comparing `yandex-music-2.1.0/yandex_music/utils/response.py` & `yandex-music-2.1.1/yandex_music/utils/response.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/utils/sign_request.py` & `yandex-music-2.1.1/yandex_music/utils/sign_request.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music/video.py` & `yandex-music-2.1.1/yandex_music/video.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.1.0/yandex_music.egg-info/PKG-INFO` & `yandex-music-2.1.1/yandex_music.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandex-music
-Version: 2.1.0
+Version: 2.1.1
 Summary: Неофициальная Python библиотека для работы с API сервиса Яндекс.Музыка.
 Home-page: https://github.com/MarshalX/yandex-music-api/
 Author: Ilya (Marshal)
 Author-email: ilya@marshal.dev
 License: LGPLv3
 Project-URL: Documentation, https://yandex-music.rtfd.io
 Project-URL: Telegram chat, https://t.me/yandex_music_api
```

### Comparing `yandex-music-2.1.0/yandex_music.egg-info/SOURCES.txt` & `yandex-music-2.1.1/yandex_music.egg-info/SOURCES.txt`

 * *Files identical despite different names*

