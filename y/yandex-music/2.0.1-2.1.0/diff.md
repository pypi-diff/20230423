# Comparing `tmp/yandex-music-2.0.1.tar.gz` & `tmp/yandex-music-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yandex-music-2.0.1.tar", last modified: Thu Mar  3 20:17:37 2022, max compression
+gzip compressed data, was "dist/yandex-music-2.1.0.tar", last modified: Sun Apr 23 00:46:42 2023, max compression
```

## Comparing `yandex-music-2.0.1.tar` & `yandex-music-2.1.0.tar`

### file list

```diff
@@ -1,284 +1,298 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)    28495 2022-03-03 20:17:30.000000 yandex-music-2.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-03-03 20:17:30.000000 yandex-music-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-03-03 20:17:30.000000 yandex-music-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    23717 2022-03-03 20:17:37.000000 yandex-music-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18423 2022-03-03 20:17:30.000000 yandex-music-2.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-03 20:17:37.000000 yandex-music-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2547 2022-03-03 20:17:30.000000 yandex-music-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32524 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3369 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_account.py
--rw-r--r--   0 runner    (1001) docker     (121)     3154 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_ad_params.py
--rw-r--r--   0 runner    (1001) docker     (121)     9801 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_album.py
--rw-r--r--   0 runner    (1001) docker     (121)     1295 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_album_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     2967 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_alert.py
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_alert_button.py
--rw-r--r--   0 runner    (1001) docker     (121)     6271 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_artist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_artist_albums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_artist_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_artist_tracks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3073 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_auto_renewable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_best.py
--rw-r--r--   0 runner    (1001) docker     (121)     2953 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_block.py
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_block_entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2938 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_brand.py
--rw-r--r--   0 runner    (1001) docker     (121)     6534 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_brief_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     2692 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_case_forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_chart.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_chart_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      930 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_chart_info_menu.py
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_chart_info_menu_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_chart_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     1824 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_contest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_counts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2496 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (121)     1747 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     1878 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_day.py
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_deactivation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_description.py
--rw-r--r--   0 runner    (1001) docker     (121)     1677 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_discrete_scale.py
--rw-r--r--   0 runner    (1001) docker     (121)     3218 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_download_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1268 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     2623 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     3621 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_feed.py
--rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_generated_playlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     4801 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_genre.py
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_icon.py
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_id.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_invocation_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_label.py
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_landing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2960 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_landing_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_licence_text_part.py
--rw-r--r--   0 runner    (1001) docker     (121)     3564 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_like.py
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (121)     4422 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_lyrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_made_for.py
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_major.py
--rw-r--r--   0 runner    (1001) docker     (121)     7601 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     4119 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_mix_link.py
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_non_auto_renewable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1268 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_normalization.py
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_open_graph_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2810 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_pager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_passport_phone.py
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_permission_alerts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_personal_playlists_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_play_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_play_contexts_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_play_counter.py
--rw-r--r--   0 runner    (1001) docker     (121)    12339 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_playlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_playlist_absence.py
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_playlist_id.py
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_playlist_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1268 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_plus.py
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_poetry_lover_match.py
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_price.py
--rw-r--r--   0 runner    (1001) docker     (121)     7687 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_product.py
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_promo_code_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_promotion.py
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_queue_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_ratings.py
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_renewable_remainder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_rotor_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     6795 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_search_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)     2449 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_shot.py
--rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_shot_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_shot_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_shot_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     3615 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_station.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_station_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2592 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_station_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_station_tracks_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     3449 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     2927 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_suggestions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2649 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_supplement.py
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_tag_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_title.py
--rw-r--r--   0 runner    (1001) docker     (121)     8809 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_track.py
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_track_id.py
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_track_position.py
--rw-r--r--   0 runner    (1001) docker     (121)     2392 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_track_short.py
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_track_short_old.py
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_track_with_ads.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_tracks_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_tracks_similar.py
--rw-r--r--   0 runner    (1001) docker     (121)     2057 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     9163 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_user_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_value.py
--rw-r--r--   0 runner    (1001) docker     (121)     2993 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_video.py
--rw-r--r--   0 runner    (1001) docker     (121)     2849 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_video_supplement.py
--rw-r--r--   0 runner    (1001) docker     (121)     2834 2022-03-03 20:17:30.000000 yandex-music-2.0.1/tests/test_vinyl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/
--rw-r--r--   0 runner    (1001) docker     (121)     7081 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/account/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3188 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/account.py
--rw-r--r--   0 runner    (1001) docker     (121)     2334 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/alert.py
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/alert_button.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/auto_renewable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2172 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/deactivation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/non_auto_renewable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1948 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/passport_phone.py
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/plus.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/price.py
--rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/product.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/renewable_remainder.py
--rw-r--r--   0 runner    (1001) docker     (121)     4147 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/subscription.py
--rw-r--r--   0 runner    (1001) docker     (121)     4364 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/account/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/album/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/album/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13539 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/album/album.py
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/album/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2281 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/album/label.py
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/album/track_position.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/artist/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/artist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12435 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/artist/artist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1857 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/artist/artist_albums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/artist/artist_tracks.py
--rw-r--r--   0 runner    (1001) docker     (121)     4617 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/artist/brief_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/artist/counts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/artist/description.py
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/artist/link.py
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/artist/ratings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2919 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/artist/vinyl.py
--rw-r--r--   0 runner    (1001) docker     (121)     5412 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/base.py
--rw-r--r--   0 runner    (1001) docker     (121)   137222 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/client.py
--rw-r--r--   0 runner    (1001) docker     (121)   138503 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/client_async.py
--rw-r--r--   0 runner    (1001) docker     (121)     4714 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/cover.py
--rw-r--r--   0 runner    (1001) docker     (121)     7378 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/download_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1734 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/experiments.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/feed/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/feed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/feed/album_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     2797 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/feed/artist_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/feed/day.py
--rw-r--r--   0 runner    (1001) docker     (121)     4021 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/feed/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/feed/feed.py
--rw-r--r--   0 runner    (1001) docker     (121)     2874 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/feed/generated_playlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/feed/track_with_ads.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/genre/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/genre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3986 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/genre/genre.py
--rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/genre/images.py
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/genre/title.py
--rw-r--r--   0 runner    (1001) docker     (121)     2518 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/icon.py
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/invocation_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/landing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3446 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/block.py
--rw-r--r--   0 runner    (1001) docker     (121)     3280 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/block_entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2623 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/chart.py
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/chart_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/chart_info_menu.py
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/chart_info_menu_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     2237 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/chart_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/landing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/landing_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     6846 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/mix_link.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/personal_playlists_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/play_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/play_contexts_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     4342 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/promotion.py
--rw-r--r--   0 runner    (1001) docker     (121)     3962 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/track_id.py
--rw-r--r--   0 runner    (1001) docker     (121)     2585 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/landing/track_short_old.py
--rw-r--r--   0 runner    (1001) docker     (121)     4180 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/like.py
--rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/pager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/permission_alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/playlist/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/playlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2020 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/playlist/brand.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/playlist/case_forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/playlist/contest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/playlist/made_for.py
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/playlist/open_graph_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/playlist/play_counter.py
--rw-r--r--   0 runner    (1001) docker     (121)    21953 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/playlist/playlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/playlist/playlist_absence.py
--rw-r--r--   0 runner    (1001) docker     (121)     3177 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/playlist/playlist_id.py
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/playlist/playlist_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/playlist/tag.py
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/playlist/tag_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/playlist/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/promo_code_status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/queue/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/queue/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     2409 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     3034 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/queue/queue_item.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/rotor/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/rotor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2473 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/rotor/ad_params.py
--rw-r--r--   0 runner    (1001) docker     (121)     1804 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/rotor/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/rotor/discrete_scale.py
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/rotor/enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/rotor/id.py
--rw-r--r--   0 runner    (1001) docker     (121)     2237 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/rotor/restrictions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/rotor/rotor_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2384 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/rotor/sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)     3554 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/rotor/station.py
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/rotor/station_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3185 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/rotor/station_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/rotor/station_tracks_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/rotor/value.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/search/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/search/best.py
--rw-r--r--   0 runner    (1001) docker     (121)     8171 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/search/search.py
--rw-r--r--   0 runner    (1001) docker     (121)     2478 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/search/search_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/search/suggestions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/shot/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/shot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2556 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/shot/shot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3803 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/shot/shot_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/shot/shot_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/shot/shot_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/supplement/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/supplement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/supplement/lyrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     2064 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/supplement/supplement.py
--rw-r--r--   0 runner    (1001) docker     (121)     2711 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/supplement/video_supplement.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/track/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/track/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2179 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/track/licence_text_part.py
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/track/major.py
--rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/track/meta_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/track/normalization.py
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/track/poetry_lover_match.py
--rw-r--r--   0 runner    (1001) docker     (121)    17387 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/track/track.py
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/track/tracks_similar.py
--rw-r--r--   0 runner    (1001) docker     (121)     4262 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/track_short.py
--rw-r--r--   0 runner    (1001) docker     (121)     3027 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/tracks_list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3462 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/utils/difference.py
--rw-r--r--   0 runner    (1001) docker     (121)    13107 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (121)    13744 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/utils/request_async.py
--rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/utils/response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-03-03 20:17:30.000000 yandex-music-2.0.1/yandex_music/video.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    23717 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7632 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-03-03 20:17:37.000000 yandex-music-2.0.1/yandex_music.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    31383 2023-04-23 00:46:33.000000 yandex-music-2.1.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-23 00:46:33.000000 yandex-music-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-23 00:46:33.000000 yandex-music-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23008 2023-04-23 00:46:42.000000 yandex-music-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-04-23 00:46:33.000000 yandex-music-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:46:42.000000 yandex-music-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-23 00:46:33.000000 yandex-music-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34230 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_ad_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_album.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_album_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_alert_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_artist_albums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_artist_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_artist_tracks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_auto_renewable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_best.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_block_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_brief_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_case_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_chart_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_chart_info_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_chart_info_menu_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_chart_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_contest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_convert_track_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_custom_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_deactivation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_discrete_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_download_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_generated_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_genre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_invocation_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_landing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_landing_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_licence_text_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_lyrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_lyrics_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_lyrics_major.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_made_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_major.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_mix_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_non_auto_renewable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_open_graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_pager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_passport_phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_permission_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_personal_playlists_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_play_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_play_contexts_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_play_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_playlist_absence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_playlist_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_playlist_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_poetry_lover_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_promo_code_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_queue_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_r128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_renewable_remainder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_rotor_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_shot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_shot_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_shot_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_shot_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_sign_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_station.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_station_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_station_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_station_tracks_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_suggestions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_tag_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_track_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_track_lyrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_track_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_track_short.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_track_short_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_track_with_ads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_tracks_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_tracks_similar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_user_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_video_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-23 00:46:33.000000 yandex-music-2.1.0/tests/test_vinyl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/alert_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/auto_renewable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/deactivation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/non_auto_renewable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/passport_phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/renewable_remainder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/account/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/album/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/album/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/album/album.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/album/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/album/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/album/track_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/artist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15692 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/artist_albums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/artist_tracks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/brief_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/artist/vinyl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115301 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116662 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/client_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/download_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/experiments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/feed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/album_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/artist_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/day.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/generated_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/feed/track_with_ads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/genre/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/genre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/genre/genre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/genre/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/genre/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/invocation_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/landing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/block_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/chart_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/chart_info_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/chart_info_menu_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/chart_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/landing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/landing_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/mix_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/personal_playlists_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/play_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/play_contexts_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/track_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/landing/track_short_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/pager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/permission_alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/playlist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/case_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/contest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/custom_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/made_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/open_graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/play_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25913 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/playlist_absence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/playlist_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/playlist_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/tag_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/playlist/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/promo_code_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/queue/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/queue/queue_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/rotor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/ad_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/discrete_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/rotor_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/station.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/station_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/station_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/station_tracks_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/rotor/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/search/best.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/search/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/search/suggestions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/shot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/shot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/shot/shot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/shot/shot_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/shot/shot_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/shot/shot_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/supplement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/supplement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/supplement/lyrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/supplement/supplement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/supplement/video_supplement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/track/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/licence_text_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/lyrics_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/lyrics_major.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/major.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/poetry_lover_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/r128.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26736 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/track_lyrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track/tracks_similar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/track_short.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/tracks_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/utils/convert_track_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/utils/difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/utils/request_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/utils/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/utils/sign_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-23 00:46:33.000000 yandex-music-2.1.0/yandex_music/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23008 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-23 00:46:42.000000 yandex-music-2.1.0/yandex_music.egg-info/top_level.txt
```

### Comparing `yandex-music-2.0.1/CHANGES.rst` & `yandex-music-2.1.0/CHANGES.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,400 +1,390 @@
-================
-Список изменений
-================
+# Список изменений
 
-Версия 2.0.0
-============
+## Версия 2.1.0
+
+**23.04.2023**
+
+**Переломные изменения**
+
+При работе над [#547](https://github.com/MarshalX/yandex-music-api/issues/547) и
+[#550](https://github.com/MarshalX/yandex-music-api/issues/550) 
+были удалены `*args` параметры, у методов класса `Client`, которые не имели никакого эффекта. 
+Передать через позиционные аргументы что-то в конечный запрос не было возможно. 
+Удаление данной конструкции **могло** затронуть код в котором ошибочно передавались лишние аргументы.
+При корректном использовании библиотеки новая версия полностью совместима со старым кодом.
+
+**Крупные изменения**
+
+- Добавлена поддержка Python 3.11.
+- В модели добавлены методы `download_bytes` и `download_bytes_async`, для получения файлов в виде байтов ([#539](https://github.com/MarshalX/yandex-music-api/issues/539)).
+- Добавлен новый метод получения текста и синхронного текста треков ([#568](https://github.com/MarshalX/yandex-music-api/pull/568)).
+- Добавлена возможность задать `timeout` по умолчанию для `Client` ([#362](https://github.com/MarshalX/yandex-music-api/issues/362)).
+- Использование настройки языка клиента во всех методах ([#554](https://github.com/MarshalX/yandex-music-api/issues/554)).
+- Добавлено поле `preview_description` классу `GeneratedPlaylist`.
+- Добавлены поля `pretrial_active` и `userhash` классу `Status`.
+- Добавлено поле `had_any_subscription` классу `Subscription`.
+- Добавлено поле `child` классу `Account`.
+- Добавлены новые поля `up_title`, `rup_description`, `custom_name` классу `StationResult`.
+- Добавлены новые модели: `CustomWave`, `R128`, `LyricsInfo`.
+- Классу `Track` добавлены новые поля: `track_source`, `available_for_options`, `r128`, `lyrics_info`, `track_sharing_flag`.
+- Классу `TrackShort` добавлены новые поля: `original_index`.
+- Классу `Playlist` добавлены новые поля: `custom_wave`, `pager`.
+- Классу `Album` добавлены новые поля: `available_for_options`.
+- Поле `cover_white` класса `MixLink` теперь опциональное.
+
+**Незначительные изменения и/или исправления**
+
+- Добавлен генератор Camel Case псевдонимов для методов ([#542](https://github.com/MarshalX/yandex-music-api/issues/542)).
+- Добавлен Makefile с сокращениями удобными при разработке библиотеки.
+- Добавлено отображение модуля при нахождении неизвестного поля.
+- Добавлена поддержка MD файлов для документации.
+- Добавлена страница в документацию по получению токена.
+- Добавлены примеры в документацию.
+- Переделана структура и обновлена документации.
+- Исправлен запуск генератора async клиента на Windows.
+- Исправлен метод `fetch_tracks_async` у класса `Playlist`.
+- Исправлены type hints у декоратора `log`.
+- Исправлены type hints для `SearchResult` в классе `Search`.
+- Исправлено отображение название класса в `report_unknown_fields_callback`.
+- Исправлены методы-сокращения `like` и `dislike` класса `Playlist` ([#516](https://github.com/MarshalX/yandex-music-api/pull/516)).
+
+## Версия 2.0.0
 
 **23.02.2022**
 
 **Поддержка asyncio и модели на dataclasses**
 
 **Переломные изменения**
 
-- Убрана поддержка ``Python 3.6``.
-- Удалено получение авторизационного токена по логину и паролю (метод ``from_credentials`` класса ``Client``).
-- Удалена возможность задать свой обработчик на полученные неизвестные поля от API (аргумент ``report_new_fields_callback`` конструктора класса ``Client``.
-- Удалён аргумент ``fetch_account_status`` из конструктора класса ``Client``. Теперь необходимо вызывать метод ``init`` для получения ID аккаунта который будет использоваться в последующих запросах. В противном случае, передача ``user_id`` при вызове многих методов класса ``Client`` становится обязательной.
-- Исключение ``BadRequest`` переименовано в ``BadRequestError``.
-- Исключение ``Unauthorized`` переименовано в ``UnauthorizedError``.
-- Исключение ``InvalidBitrate`` переименовано в ``InvalidBitrateError``.
-- Исключение ``TimedOut`` переименовано в ``TimedOutError``.
-- Свойство ``result`` класса ``Response`` удалено. Вместо него добавлен метод ``get_result``.
-- Свойство ``error`` класса ``Response`` удалено. Вместо него добавлен метод ``get_error``.
-- В JSON представлении моделей к полям, чьё имя совпадает с именем стандартных функций, больше не добавляется нижнее подчеркивание в конец (пример: ``id``, а не ``id_``; ``max``, а не ``max_``). Теперь нижнее подчеркивание добавляется только к зарезервированным словам (пример: ``from`` будет ``from_``).
+- Убрана поддержка `Python 3.6`.
+- Удалено получение авторизационного токена по логину и паролю (метод `from_credentials` класса `Client`).
+- Удалена возможность задать свой обработчик на полученные неизвестные поля от API (аргумент `report_new_fields_callback` конструктора класса `Client`.
+- Удалён аргумент `fetch_account_status` из конструктора класса `Client`. Теперь необходимо вызывать метод `init` для получения ID аккаунта который будет использоваться в последующих запросах. В противном случае передача `user_id` при вызове многих методов класса `Client` становится обязательной.
+- Исключение `BadRequest` переименовано в `BadRequestError`.
+- Исключение `Unauthorized` переименовано в `UnauthorizedError`.
+- Исключение `InvalidBitrate` переименовано в `InvalidBitrateError`.
+- Исключение `TimedOut` переименовано в `TimedOutError`.
+- Свойство `result` класса `Response` удалено. Вместо него добавлен метод `get_result`.
+- Свойство `error` класса `Response` удалено. Вместо него добавлен метоl `get_error`.
+- В JSON представлении моделей к полям, чьё имя совпадает с именем стандартных функций, больше не добавляется нижнее подчеркивание в конец (пример: `id`, а не `id_`; `max`, а не `max_`). Теперь нижнее подчеркивание добавляется только к зарезервированным словам (пример: `from` будет `from_`).
 
 **Крупные изменения**
 
-- Добавлена асинхронная версия клиента и всех методов-сокращений (класс ``ClientAsync``).
-- Добавлено новое исключение ``NotFoundError`` (наследник ``NetworkError``). Будет сгенерировано при получении статус кода 404.
-- Проект больше не использует ``pipenv``.
+- Добавлена асинхронная версия клиента и всех методов-сокращений (класс `ClientAsync`).
+- Добавлено новое исключение `NotFoundError` (наследник `NetworkError`). Будет сгенерировано при получении статус кода 404.
+- Проект больше не использует `pipenv`.
 - Зависимости проекта больше не требуют конкретных версий.
-- Для генерации исходных файлов ``Sphinx`` теперь используется ``sphinx-apidoc``.
+- Для генерации исходных файлов `Sphinx` теперь используется `sphinx-apidoc`.
 
 **Незначительные изменения и/или исправления**
 
 - Исправлена обработка серверных ошибок которые вернулись в отличном от JSON формате.
-- Исправлена обработка серверных ошибок метода ``search`` класса ``Client``.
+- Исправлена обработка серверных ошибок метода `search` класса `Client`.
 - Предупреждения о пришедших неизвестных полях от API отключены по умолчанию.
-- Используется английская локализация ``Sphinx``.
+- Используется английская локализация `Sphinx`.
 - Изменена тема документации.
 
-Версия 1.0.0
-============
+## Версия 1.0.0
 
 **06.02.2021**
 
 **Стабильная версия библиотеки**
 
 **Переломные изменения**
 
-- Поле ``error`` класса ``Artist`` теперь называется ``reason``.
-- Метод ``users_playlists`` класса ``Client`` теперь возвращает один объект плейлиста, когда был передан один ``kind``. При передаче списка в ``kind`` вернётся список плейлистов (`#318`_).
-- Поле ``labels`` класса ``Album`` теперь может содержать список из строк, а не только список объектов класса ``Label``.
+- Поле `error` класса `Artist` теперь называется `reason`.
+- Метод `users_playlists` класса `Client` теперь возвращает один объект плейлиста, когда был передан один `kind`. При передаче списка в `kind` вернётся список плейлистов ([#318](https://github.com/MarshalX/yandex-music-api/issues/318)).
+- Поле `labels` класса `Album` теперь может содержать список из строк, а не только список объектов класса `Label`.
 
 **Крупные изменения**
 
-- Добавлены примеры в папку ``examples``.
-- Добавлена поддержка рекомендаций для плейлистов (`#324`_):
-    - Добавлен класс ``PlaylistRecommendations``.
-    - Добавлен метод клиента для получения рекомендаций (``users_playlists_recommendations``).
-    - Добавлен метод ``get_recommendations`` классу ``Playlist`` для получения рекомендаций.
-- Добавлено получение чартов (`#294`_):
-    - Добавлены новые классы: ``ChartInfo``, ``ChartInfoMenu``, ``ChartInfoMenuItem``.
-    - Добавлен метод клиента для получения чарта (``chart``).
-- Добавлена поддержка тегов/подборок (`#192`_):
-    - Добавлены новые классы: ``TagResult``, ``Tag``.
-    - Добавлен новый метод клиента для получения тегов (``tags``).
-- Добавлено присоединение к коллективному плейлисту (`#317`_):
-    - Добавлен новый метод клиента для присоединения (``playlists_collective_join``).
-- Добавлена поддержка очередей прослушивания (`#246`_):
-    - Добавлены новые классы: ``Context``, ``Queue``, ``QueueItem``.
-    - Добавлены новые методы в ``Client``: ``queues_list``, ``queue``, ``queue_update_position``, ``queue_create``.
-    - Добавлены поля ``track_id`` и ``from_`` в класс ``TrackId``.
-    - Добавлена возможность смены языка у клиента для ответов от API.
-    - Добавлена десериализация любого объекта в ``JSON`` пригодного для отправки в запросе на Яндекс API.
-- Добавлены следующие методы для ``Client``:
-    - ``new_releases`` – получение полного списка всех новых релизов.
-    - ``new_playlists`` – получение полного списка всех новый плейлистов.
-    - ``podcasts`` – получение подкаста с лендинга.
-- Добавлены новые сокращения в модели:
-    - ``download_cover_white``, ``download_cover_uri`` в ``MixLink``.
-    - ``download_image`` в ``Promotion``.
-    - ``artists_name`` в ``Album`` и ``Track``.
-    - ``fetch_track``, ``track_full_id`` в ``TrackId``.
-    - ``fetch_tracks`` в ``TracksList``.
-    - ``insert_track``, ``delete_tracks``, ``delete`` в ``Playlist``.
-    - ``playlist_id``, ``fetch_playlist`` в ``PlaylistId``.
-    - ``get_current_track`` в ``Queue``.
-    - ``fetch_queue`` в ``QueueItem``.
-    - ``next_page``, ``get_page``, ``prev_page`` в ``Search``.
-    - и другие...
+- Добавлены примеры в папку `examples`.
+- **Добавлена поддержка рекомендаций для плейлистов ([#324](https://github.com/MarshalX/yandex-music-api/issues/324))**:
+  - Добавлен класс `PlaylistRecommendations`.
+  - Добавлен метод клиента для получения рекомендаций(`users_playlists_recommendations`).
+  - Добавлен метод `get_recommendations` классу `Playlist` для
+- **Добавлено получение чартов ([#294](https://github.com/MarshalX/yandex-music-api/issues/294))**:
+  - Добавлены новые классы: `ChartInfo`, `ChartInfoMenu`,`ChartInfoMenuItem`.
+  - Добавлен метод клиента для получения чарта (`chart`).
+- **Добавлена поддержка тегов/подборок ([#192](https://github.com/MarshalX/yandex-music-api/issues/192))**:
+  - Добавлены новые классы: `TagResult`, `Tag`.
+  - Добавлен новый метод клиента для получения тегов (`tags`).
+- **Добавлено присоединение к коллективному плейлисту ([#317](https://github.com/MarshalX/yandex-music-api/issues/317))**:
+  - Добавлен новый метод клиента для присоединения(`playlists_collective_join`).
+- **Добавлена поддержка очередей прослушивания ([#246](https://github.com/MarshalX/yandex-music-api/issues/246))**:
+  - Добавлены новые классы: `Context`, `Queue`, `QueueItem`.
+  - Добавлены новые методы в `Client`: `queues_list`, `queue`,`queue_update_position`, `queue_create`.
+  - Добавлены поля `track_id` и `from_` в класс `TrackId`.
+  - Добавлена возможность смены языка у клиента для ответов от API.
+  - Добавлена десериализация любого объекта в `JSON` пригодного для отправки в запросе на Яндекс API.
+- **Добавлены следующие методы для `Client`**:
+  - `new_releases` – получение полного списка всех новых релизов.
+  - `new_playlists` – получение полного списка всех новый плейлистов.
+  - `podcasts` – получение подкаста с лендинга.
+- **Добавлены новые сокращения в модели**:
+  - `download_cover_white`, `download_cover_uri` в `MixLink`.
+  - `download_image` в `Promotion`.
+  - `artists_name` в `Album` и `Track`.
+  - `fetch_track`, `track_full_id` в `TrackId`.
+  - `fetch_tracks` в `TracksList`.
+  - `insert_track`, `delete_tracks`, `delete` в `Playlist`.
+  - `playlist_id`, `fetch_playlist` в `PlaylistId`.
+  - `get_current_track` в `Queue`.
+  - `fetch_queue` в `QueueItem`.
+  - `next_page`, `get_page`, `prev_page` в `Search`.
+  - и другие...
 - Добавлена поддержка новых типов поиска: подкасты, выпуски, пользователи.
-- Добавлен коллбек для обработки новых полей.
+- Добавлен callback для обработки новых полей.
 - Добавлена информацию по поводу запуска потока по треку, плейлисту и др.
-- Добавлена десериализация ``decomposed`` у ``Artist`` (`#10`_).
-- Добавлен ``__len__`` для ``TracksList`` (`#380`_).
-- Добавлены ``__iter__``, ``__len__`` и ``__getitem__`` для классов представляющих список каких-либо объектов.
-- Добавлено сокращение ``fetch_tracks`` классу ``Playlist`` для получения треков плейлиста.
-- Добавлен метод ``get_url`` классу ``Icon`` для получения прямой ссылки на изображение.
-- Класс ``User`` расширен для поддержки поля ``user_info`` из ``Track`` (поля ``full_name``, ``display_name``).
-- Добавлены новые классы по отчётам с Telegram бота (`#306`_, `#398`_):
-    - ``LandingList``.
-    - ``RenewableRemainder``.
-    - ``Alert``.
-    - ``AlertButton``.
-    - ``StationData``.
-    - ``Brand``.
-    - ``Contest``.
-    - ``OpenGraphData``.
-    - ``NonAutoRenewable``.
-    - ``Operator``.
-    - ``Deactivation``.
-    - ``PoetryLoverMatch``.
-    - ``Deprecation``.
-- Добавлены новые поля классам по отчётам с Telegram бота (`#306`_, `#398`_):
-    - ``plus`` в ``Product``.
-    - ``non_auto_renewable_remainder`` в ``Subscription``.
-    - ``og_image`` в ``Artist``.
-    - ``meta_type`` в ``Album``.
-    - ``advertisement`` в ``Status``.
-    - ``best`` в ``Track``.
-    - ``offer_id`` и ``artist_ids`` в ``Vinyl``.
-    - ``playlists`` в ``BriefInfo``.
-    - ``is_custom`` в ``Cover``.
-    - ``play_count``, ``recent``, ``chart``, ``track`` в ``TrackShort``.
-    - ``url_part``, ``og_title``, ``image``, ``cover_without_text``, ``background_color``, ``text_color``, ``id_for_from``, ``similar_playlists``, ``last_owner_playlists`` в ``Playlist``.
-    - ``bg_color`` в ``Chart``.
-    - ``error`` в ``Artist``.
-    - ``substituted``, ``matched_track``, ``can_publish``, ``state``, ``desired_visibility``, ``filename``, ``user_info``, ``meta_data`` в ``Track``.
-    - ``copyright_name``, ``copyright_cline`` в ``Cover``.
-    - ``direct`` в ``DownloadInfo``.
-    - ``cheapest``, ``title``, ``family_sub``, ``fb_image``, ``fb_name``, ``family``, ``intro_period_duration``, ``intro_price``, ``start_period_duration``, ``start_price``, ``licence_text_parts`` в ``Product``.
-    - ``storage_dir``, ``duplicates`` в ``Album``.
-    - ``subscribed`` в ``ArtistEvent``.
-    - ``description`` в ``GeneratedPlaylist``.
-    - ``genre`` в ``Event``.
-    - ``show_in_regions`` в ``Genre``.
-    - ``cover_uri`` в ``MixLink``.
-    - ``og_description``, ``top_artist`` в ``Playlist``.
-    - ``full_image_url``, ``mts_full_image_url`` в ``Station``.
-    - ``coauthors`` и ``recent_tracks`` в ``Playlist``.
-    - ``regions`` в ``User``.
-    - ``users``, ``podcasts``, ``podcast_episodes``, ``type_``, ``page``, ``per_page`` в ``Search``.
-    - ``short_description``, ``description``, ``is_premiere``, ``is_banner`` в ``Like``.
-    - ``master_info`` в ``AutoRenewable``.
-    - ``station_data`` и ``bar_below`` в ``Status``.
-    - ``family_auto_renewable`` в ``Subscription``.
-    - ``misspell_result`` и ``misspell_original`` в ``Search``.
-    - ``experiment`` в класс ``Status``.
-    - ``operator`` и ``non_auto_renewable`` в ``Subscription``.
-    - ``text_color``, ``short_description``, ``description``, ``is_premiere`` и ``is_banner`` в ``Album``.
-    - ``hand_made_description`` в ``Artist``.
-    - ``metrika_id`` в ``Playlist``.
-    - ``og_image`` в ``Tag``.
-    - ``url`` в ``Lyrics``.
-    - ``number``, ``genre`` в ``MetaData``.
-    - ``poetry_lover_matches`` в ``Track``.
-    - ``contest``, ``dummy_description``, ``dummy_page_description``, ``dummy_cover``, ``dummy_rollover_cover``, ``og_data``, ``branding`` в ``Playlist``.
-    - ``available_as_rbt``, ``lyrics_available``, ``remember_position``, ``albums``, ``duration_ms``, ``explicit``, ``start_date``, ``likes_count``, ``deprecation`` в ``Album``.
-    - ``lyricist``, ``version``, ``composer`` в ``MetaData``.
-    - ``last_releases`` в ``BriefInfo``.
-    - ``ya_money_id`` в ``Artist`` (`#351`_, `#370`_).
-    - ``playlist_uuid`` в ``Playlist``.
-    - ``sync_queue_enabled`` в ``UserSettings``.
-    - ``background_video_uri``, ``short_description``, ``is_suitable_for_children`` в ``Track`` (`#376`_).
-    - ``meta_type``, ``likes_count`` в ``Album`` (`#386`_).
-    - ``deprecation`` в ``Album``.
-    - ``available_regions`` в ``Album``.
-    - ``type``, ``ready`` в ``Playlist``.
-    - ``description`` в ``Supplement``.
+- Добавлена десериализация `decomposed` у `Artist` ([#10](https://github.com/MarshalX/yandex-music-api/issues/10)).
+- Добавлен `__len__` для `TracksList` ([#380](https://github.com/MarshalX/yandex-music-api/issues/380)).
+- Добавлены `__iter__`, `__len__` и `__getitem__` для классов представляющих список каких-либо объектов.
+- Добавлено сокращение `fetch_tracks` классу `Playlist` для получения треков плейлиста.
+- Добавлен метод `get_url` классу `Icon` для получения прямой ссылки на изображение.
+- Класс `User` расширен для поддержки поля `user_info` из `Track`(поля `full_name`, `display_name`).
+- **Добавлены новые классы по отчётам с Telegram бота ([#306](https://github.com/MarshalX/yandex-music-api/issues/306), [#398](https://github.com/MarshalX/yandex-music-api/issues/398))**:
+  - `LandingList`.
+  - `RenewableRemainder`.
+  - `Alert`.
+  - `AlertButton`.
+  - `StationData`.
+  - `Brand`.
+  - `Contest`.
+  - `OpenGraphData`.
+  - `NonAutoRenewable`.
+  - `Operator`.
+  - `Deactivation`.
+  - `PoetryLoverMatch`.
+  - `Deprecation`.
+- **Добавлены новые поля классам по отчётам с Telegram бота ([#306](https://github.com/MarshalX/yandex-music-api/issues/306), [#398](https://github.com/MarshalX/yandex-music-api/issues/398))**:
+  - `plus` в `Product`.
+  - `non_auto_renewable_remainder` в `Subscription`.
+  - `og_image` в `Artist`.
+  - `meta_type` в `Album`.
+  - `advertisement` в `Status`.
+  - `best` в `Track`.
+  - `offer_id` и `artist_ids` в `Vinyl`.
+  - `playlists` в `BriefInfo`.
+  - `is_custom` в `Cover`.
+  - `play_count`, `recent`, `chart`, `track` в `TrackShort`.
+  - `url_part`, `og_title`, `image`, `cover_without_text`, `background_color`, `text_color`, `id_for_from`,`similar_playlists`, `last_owner_playlists` в `Playlist`.
+  - `bg_color` в `Chart`.
+  - `error` в `Artist`.
+  - `substituted`, `matched_track`, `can_publish`, `state`, `desired_visibility`, `filename`, `user_info`, `meta_data` в`Track`.
+  - `copyright_name`, `copyright_cline` в `Cover`.
+  - `direct` в `DownloadInfo`.
+  - `cheapest`, `title`, `family_sub`, `fb_image`, `fb_name`,`family`, `intro_period_duration`, `intro_price`, `start_period_duration`, `start_price`, `licence_text_parts` в `Product`.
+  - `storage_dir`, `duplicates` в `Album`.
+  - `subscribed` в `ArtistEvent`.
+  - `description` в `GeneratedPlaylist`.
+  - `genre` в `Event`.
+  - `show_in_regions` в `Genre`.
+  - `cover_uri` в `MixLink`.
+  - `og_description`, `top_artist` в `Playlist`.
+  - `full_image_url`, `mts_full_image_url` в `Station`.
+  - `coauthors` и `recent_tracks` в `Playlist`.
+  - `regions` в `User`.
+  - `users`, `podcasts`, `podcast_episodes`, `type_`, `page`, `per_page` в `Search`.
+  - `short_description`, `description`, `is_premiere`, `is_banner` в `Like`.
+  - `master_info` в `AutoRenewable`.
+  - `station_data` и `bar_below` в `Status`.
+  - `family_auto_renewable` в `Subscription`.
+  - `misspell_result` и `misspell_original` в `Search`.
+  - `experiment` в класс `Status`.
+  - `operator` и `non_auto_renewable` в `Subscription`.
+  - `text_color`, `short_description`, `description`, `is_premiere` и `is_banner` в `Album`.
+  - `hand_made_description` в `Artist`.
+  - `metrika_id` в `Playlist`.
+  - `og_image` в `Tag`.
+  - `url` в `Lyrics`.
+  - `number`, `genre` в `MetaData`.
+  - `poetry_lover_matches` в `Track`.
+  - `contest`, `dummy_description`, `dummy_page_description`, `dummy_cover`, `dummy_rollover_cover`, `og_data`, `branding` в `Playlist`.
+  - `available_as_rbt`, `lyrics_available`, `remember_position`, `albums`, `duration_ms`, `explicit`, `start_date`, `likes_count`, `deprecation` в `Album`.
+  - `lyricist`, `version`, `composer` в `MetaData`.
+  - `last_releases` в `BriefInfo`.
+  - `ya_money_id` в `Artist` ([#351](https://github.com/MarshalX/yandex-music-api/issues/351), [#370](https://github.com/MarshalX/yandex-music-api/issues/370)).
+  - `playlist_uuid` в `Playlist`.
+  - `sync_queue_enabled` в `UserSettings`.
+  - `background_video_uri`, `short_description`, `is_suitable_for_children` в `Track` ([#376](https://github.com/MarshalX/yandex-music-api/issues/376)).
+  - `meta_type`, `likes_count` в `Album` ([#386](https://github.com/MarshalX/yandex-music-api/issues/386)).
+  - `deprecation` в `Album`.
+  - `available_regions` в `Album`.
+  - `type`, `ready` в `Playlist`.
+  - `description` в `Supplement`.
 
 **Незначительные изменения и/или исправления**
 
-- Добавлена опциональность следующим полям:
-    - все поля в ``MetaData``.
-    - ``advertisement`` в ``Status``.
-    - ``text_language`` в ``Lyrics``.
-    - ``provider_video_id`` в ``VideoSupplement``.
-    - ``title`` в ``VideoSupplement`` (`#403`_).
-    - ``instructions`` в ``Deactivation`` (`#402`_).
-    - ``id`` в ``Album`` (`#401`_).
+- **Добавлена опциональность следующим полям**:
+  - все поля в `MetaData`.
+  - `advertisement` в `Status`.
+  - `text_language` в `Lyrics`.
+  - `provider_video_id` в `VideoSupplement`.
+  - `title` в `VideoSupplement` ([#403](https://github.com/MarshalX/yandex-music-api/issues/403)).
+  - `instructions` в `Deactivation` ([#402](https://github.com/MarshalX/yandex-music-api/issues/402)).
+  - `id` в `Album` ([#401](https://github.com/MarshalX/yandex-music-api/issues/401)).
+
 - Исправлена десериализация подкастов, эпизодов подкастов и пользователей в лучшем результате поиска.
 - Исправлена десериализация альбомов. В зависимости от запроса содержимое лейблов может быть списком объектом или списком строк (в поиске).
 - Исправлен выбор настроек радио.
 - Исправлены ошибки в документации.
 - Протестирована работа на Python 3.9.
 
-.. _`#318`: https://github.com/MarshalX/yandex-music-api/issues/318
-.. _`#306`: https://github.com/MarshalX/yandex-music-api/issues/306
-.. _`#324`: https://github.com/MarshalX/yandex-music-api/issues/324
-.. _`#294`: https://github.com/MarshalX/yandex-music-api/issues/294
-.. _`#192`: https://github.com/MarshalX/yandex-music-api/issues/192
-.. _`#317`: https://github.com/MarshalX/yandex-music-api/issues/317
-.. _`#10`: https://github.com/MarshalX/yandex-music-api/issues/10
-.. _`#386`: https://github.com/MarshalX/yandex-music-api/issues/386
-.. _`#246`: https://github.com/MarshalX/yandex-music-api/issues/246
-.. _`#376`: https://github.com/MarshalX/yandex-music-api/issues/376
-.. _`#351`: https://github.com/MarshalX/yandex-music-api/issues/351
-.. _`#370`: https://github.com/MarshalX/yandex-music-api/issues/370
-.. _`#380`: https://github.com/MarshalX/yandex-music-api/issues/380
-.. _`#398`: https://github.com/MarshalX/yandex-music-api/issues/398
-.. _`#401`: https://github.com/MarshalX/yandex-music-api/issues/401
-.. _`#402`: https://github.com/MarshalX/yandex-music-api/issues/402
-.. _`#403`: https://github.com/MarshalX/yandex-music-api/issues/403
-
-Версия 0.1.1
-============
+## Версия 0.1.1
 
 **25.03.2020**
 
 **Закончено документирование всех классов и основных методов!**
 
 **Переломные изменения**
 
-- Классы отметок "мне нравится" для альбомов, плейлистов и исполнителей обобщены. Теперь представлены одним классом.
-    - Удаленные классы:
-        - ``ArtistsLikes``.
-        - ``AlbumsLikes``.
-        - ``PlaylistsLikes``.
-    - Новый класс: ``Like`` (поле ``type`` для определения содержимого).
-- Изменено название пакета с ``status`` на ``account`` (`#195`_).
-- Исправлено выбрасываемое исключение при таймауте:
-    - Прошлое исключение: ``TimeoutError`` (built-in).
-    - Новое исключение: ``TimedOut`` (``yandex_music.exceptions``).
-- Удалены следующие файлы: ``requirements.txt``, ``requirements-dev.txt``, ``requirements-docs.txt``.
+- **Классы отметок "мне нравится" для альбомов, плейлистов и исполнителей обобщены. Теперь представлены одним классом**.
+  - **Удаленные классы**:
+    - `ArtistsLikes`.
+    - `AlbumsLikes`.
+    - `PlaylistsLikes`.
+  - Новый класс: `Like` (поле `type` для определения содержимого).
+- Изменено название пакета с `status` на `account` ([#195](https://github.com/MarshalX/yandex-music-api/issues/195)).
+- **Исправлено выбрасываемое исключение при таймауте**:
+  - Прошлое исключение: `TimeoutError` (built-in).
+  - Новое исключение: `TimedOut` (`yandex_music.exceptions`).
+- Удалены следующие файлы: `requirements.txt`, `requirements-dev.txt`,
+  `requirements-docs.txt`.
 
 **Крупные изменения**
 
-- Добавлено обнаружение новых полей с просьбой сообщить о них (`#216`_).
-    - Добавлена проверка на неизвестные поля.
-    - Добавлен вывод отладочной информации в виде warning'a.
-    - Добавлен шаблон issue для отправки логов.
-- Добавлено поле ``type`` для класса ``SearchResult`` для определения типа результата поиска по объекту.
-- Добавлены настройки пользователя (`#195`_):
-    - Добавлен класс ``UserSettings``.
-    - Добавлен метод для получения своих настроек (``account_settings``).
-    - Добавлен метод для получения настроек другого пользователя (``users_settings``).
-    - Добавлен метод для изменения настроек (``account_settings_set``).
-- Добавлен возможность получить похожие треки (`#197`_):
-    - Добавлен класс ``TracksSimilar`` с полями трека и списка похожих треков.
-    - Добавлен метод для получения похожих треков (``tracks_similar``).
-- Добавлены шоты от Алисы (`#185`_):
-    - Добавлен метод ``after_track`` в класс ``Client`` для получения контента для воспроизведения после трека (реклама, шот).
-    - Добавлены методы для загрузки обложки и аудиоверсии шота.
-    - Добавлены новые классы:
-        - ``Shot``
-        - ``ShotData``
-        - ``ShotEvent``
-        - ``ShotType``
-- Добавлен метод для изменения видимости плейлиста (`#179`_).
-- Добавлена поддержка Яндекс.Радио (`#20`_):
-    - Исправлена отправка фидбека.
-    - Написана инструкция по использованию (в доке к методу).
-    - Добавлен аргумент для перехода по цепочке треков.
-    - Добавлен метод для изменения настроек станции.
+- **Добавлено обнаружение новых полей с просьбой сообщить о них ([#216](https://github.com/MarshalX/yandex-music-api/issues/216))**.
+  - Добавлена проверка на неизвестные поля.
+  - Добавлен вывод отладочной информации в виде warning'a.
+  - Добавлен шаблон issue для отправки логов.
+- Добавлено поле `type` для класса `SearchResult` для определения типа результата поиска по объекту.
+- **Добавлены настройки пользователя ([#195](https://github.com/MarshalX/yandex-music-api/issues/195))**:
+  - Добавлен класс `UserSettings`.
+  - Добавлен метод для получения своих настроек (`account_settings`).
+  - Добавлен метод для получения настроек другого пользователя (`users_settings`).
+  - Добавлен метод для изменения настроек (`account_settings_set`).
+- **Добавлен возможность получить похожие треки ([#197](https://github.com/MarshalX/yandex-music-api/issues/197))**:
+  - Добавлен класс `TracksSimilar` с полями трека и списка похожих треков.
+  - Добавлен метод для получения похожих треков (`tracks_similar`).
+- **Добавлены шоты от Алисы ([#185](https://github.com/MarshalX/yandex-music-api/issues/185))**:
+  - Добавлен метод `after_track` в класс `Client` для получения контента для воспроизведения после трека (реклама, шот).
+  - Добавлены методы для загрузки обложки и аудиоверсии шота.
+  - **Добавлены новые классы**:
+    - `Shot`
+    - `ShotData`
+    - `ShotEvent`
+    - `ShotType`
+- Добавлен метод для изменения видимости плейлиста ([#179](https://github.com/MarshalX/yandex-music-api/issues/179)).
+- **Добавлена поддержка Яндекс.Радио ([#20](https://github.com/MarshalX/yandex-music-api/issues/20))**:
+  - Исправлена отправка фидбека.
+  - Написана инструкция по использованию (в доке к методу).
+  - Добавлен аргумент для перехода по цепочке треков.
+  - Добавлен метод для изменения настроек станции.
 
 **Незначительные изменения и/или исправления**
 
-- Убрано дублирование информации в документации (`#247`_).
-- Добавлены новые поля в класс ``Track``: ``version``, ``remember_position`` (`#238`_).
-- Добавлено исключение ``InvalidBitrate`` при попытке загрузить недопустимый трек по критериям (кодек, битрейт).
-- Исправлено получение прямой ссылки на файл с кодеком AAC (`#237`_, `#25`_).
-- Исправлено получение плейлиста с Алисой в лендинге (`#185`_).
-- Исправлено название поля с ссылкой на источник в классе ``Description`` (с ``url`` на ``uri``).
+- Убрано дублирование информации в документации ([#247](https://github.com/MarshalX/yandex-music-api/issues/247)).
+- Добавлены новые поля в класс `Track`: `version`, `remember_position` ([#238](https://github.com/MarshalX/yandex-music-api/issues/238)).
+- Добавлено исключение `InvalidBitrate` при попытке загрузить недопустимый трек по критериям (кодек, битрейт).
+- Исправлено получение прямой ссылки на файл с кодеком AAC ([#237](https://github.com/MarshalX/yandex-music-api/issues/237), [#25](https://github.com/MarshalX/yandex-music-api/issues/25)).
+- Исправлено получение плейлиста с Алисой в лендинге ([#185](https://github.com/MarshalX/yandex-music-api/issues/185)).
+- Исправлено название поля с ссылкой на источник в классе `Description` (с `url` на `uri`).
 - Исправлена десериализация несуществующего исполнителя.
-- Добавлено поле ``version`` в класс ``Album`` (`#178`_).
-- Поле ``picture`` класса ``Vinyl`` теперь опциональное.
-- Поле ``week`` класса ``Ratings`` теперь опциональное.
-- Поле ``product_id`` класса ``AutoRenewable`` теперь опциональное (`#182`_).
+- Добавлено поле `version` в класс `Album` ([#178](https://github.com/MarshalX/yandex-music-api/issues/178)).
+- Поле `picture` класса `Vinyl` теперь опциональное.
+- Поле `week` класса `Ratings` теперь опциональное.
+- Поле `product_id` класса `AutoRenewable` теперь опциональное ([#182](https://github.com/MarshalX/yandex-music-api/issues/182)).
 - Правки замечаний по codacy.
 
-.. _`#216`: https://github.com/MarshalX/yandex-music-api/issues/216
-.. _`#247`: https://github.com/MarshalX/yandex-music-api/issues/247
-.. _`#237`: https://github.com/MarshalX/yandex-music-api/issues/237
-.. _`#25`: https://github.com/MarshalX/yandex-music-api/issues/25
-.. _`#238`: https://github.com/MarshalX/yandex-music-api/issues/238
-.. _`#182`: https://github.com/MarshalX/yandex-music-api/issues/182
-.. _`#195`: https://github.com/MarshalX/yandex-music-api/issues/195
-.. _`#197`: https://github.com/MarshalX/yandex-music-api/issues/197
-.. _`#20`: https://github.com/MarshalX/yandex-music-api/issues/20
-.. _`#185`: https://github.com/MarshalX/yandex-music-api/issues/185
-.. _`#179`: https://github.com/MarshalX/yandex-music-api/issues/179
-.. _`#178`: https://github.com/MarshalX/yandex-music-api/issues/178
-
-Версия 0.0.16
-=============
+## Версия 0.0.16
 
 **29.12.2019**
 
 **Переломные изменения**
 
-- Поле ``account`` переименовано в ``me`` и теперь содержит объект ``Status``, вместо ``Account`` (`#162`_).
-- Убрано использование зарезервированных имён в аргументах конструкторов (теперь они с ``_`` на конце). Имена с нижними подчёркиваниями есть как при сериализации так и при десериализации (`#168`_).
+- Поле `account` переименовано в `me` и теперь содержит объект `Status`, вместо `Account` ([#162](https://github.com/MarshalX/yandex-music-api/issues/162)).
+- Убрано использование зарезервированных имён в аргументах конструкторов (теперь они с `_` на конце). Имена с нижними подчёркиваниями есть как при сериализации так и при десериализации ([#168](https://github.com/MarshalX/yandex-music-api/issues/168)).
 
 **Крупные изменения**
 
 - **Добавлены аннотации типов во всей библиотеке!**
 
 **Незначительные изменения и/или исправления**
 
-- Добавлен аргумент ``fetch_account_status`` для опциональности получения информации об аккаунте при инициализации клиента (`#162`_).
-- Добавлены тесты c передачей пустого словаря в ``de_json`` и ``de_list`` (`#174`_).
-- Использование ``ujson`` при наличии, обновлены зависимости (`#161`_).
-- Добавлен в зависимости для разработки ``importlib_metadata`` для поддержки старых версий (в новой версии ``pytest`` его больше не используют, в угоду ``importlib.metadata`` `#pytest-5537`_)) (`#161`_).
-- Добавлен в зависимости для разработки ``atomicwrites``, который используется ``pytest`` теперь только на ``Windows`` - `#pytest-6148`_ (`#161`_).
-- Исправлен баг с передачей ``timeout`` аргумента в аргумент ``params`` в следующих методах: ``artists``, ``albums``, ``playlists_list`` (`#120`_).
-- Исправлена инициализация клиента при помощи логина и пароля с использованием прокси (`#159`_).
+- Добавлен аргумент `fetch_account_status` для опциональности получения информации об аккаунте при инициализации клиента ([#162](https://github.com/MarshalX/yandex-music-api/issues/162)).
+- Добавлены тесты c передачей пустого словаря в `de_json` и `de_list` ([#174](https://github.com/MarshalX/yandex-music-api/issues/174)).
+- Использование `ujson` при наличии, обновлены зависимости ([#161](https://github.com/MarshalX/yandex-music-api/issues/161)).
+- Добавлен в зависимости для разработки `importlib_metadata` для  поддержки старых версий (в новой версии `pytest` его больше не используют, в угоду `importlib.metadata` [#pytest-5537](https://github.com/pytest-dev/pytest/issues/5537))) ([#161](https://github.com/MarshalX/yandex-music-api/issues/161)).
+- Добавлен в зависимости для разработки `atomicwrites`, который используется `pytest` теперь только на `Windows` - [#pytest-6148](https://github.com/pytest-dev/pytest/pull/6148) ([#161](https://github.com/MarshalX/yandex-music-api/issues/161)).
+- Исправлен баг с передачей `timeout` аргумента в аргумент `params` в следующих методах: `artists`, `albums`, `playlists_list` ([#120](https://github.com/MarshalX/yandex-music-api/issues/120)).
+- Исправлена инициализация клиента при помощи логина и пароля с использованием прокси ([#159](https://github.com/MarshalX/yandex-music-api/issues/159)).
 - Исправлен баг в загрузке обложки альбома.
 
-.. _`#162`: https://github.com/MarshalX/yandex-music-api/issues/162
-.. _`#161`: https://github.com/MarshalX/yandex-music-api/issues/161
-.. _`#159`: https://github.com/MarshalX/yandex-music-api/issues/159
-.. _`#168`: https://github.com/MarshalX/yandex-music-api/issues/168
-.. _`#120`: https://github.com/MarshalX/yandex-music-api/issues/120
-.. _`#174`: https://github.com/MarshalX/yandex-music-api/issues/174
-.. _`#pytest-5537`: https://github.com/pytest-dev/pytest/issues/5537
-.. _`#pytest-6148`: https://github.com/pytest-dev/pytest/pull/6148
-
-Версия 0.0.15
-=============
+## Версия 0.0.15
 
 **01.12.2019**
 
 **Переломные изменения**
 
-- У классов ``Artist``, ``Track`` и ``Playlist`` изменился перечень полей для генерации хеша.
+- У классов `Artist`, `Track` и `Playlist` изменился перечень полей для генерации хеша.
 
 **Крупные изменения**
 
-- Добавлена возможность выполнять запросы через прокси-сервер для использовании библиотеки на зарубежных серверах (`#139`_).
-    - Добавлен пример использования в ``README``.
-- Добавлена обработка капчи при авторизации с возможностью использования callback-функции для её обработки (`#140`_):
-    - Новые исключения:
-        - Captcha:
-            - CaptchaRequired.
-            - CaptchaWrong.
-    - Новые классы:
-        - CaptchaResponse.
-    - Новые примеры в ``README``:
-        - Пример обработки с использованием callback-функции.
-        - Пример полностью своей обработки капчи.
-- Добавлена документация для класса ``Search`` (`#83`_).
-- Добавлена возможность получения всех альбомов исполнителя (`#141`_):
-    - Новые классы:
-        - ArtistAlbums.
-    - Новые методы:
-        - ``artists_direct_albums`` у ``Client``.
-        - ``get_albums`` у ``Artist``.
-- Добавлена обработка несуществующего плейлиста (`#147`_):
-    - Новые классы:
-        - ``PlaylistAbsence``.
+- **Добавлена возможность выполнять запросы через прокси-сервер для использовании библиотеки на зарубежных серверах ([#139](https://github.com/MarshalX/yandex-music-api/issues/139))**.
+  - Добавлен пример использования в `README`.
+- **Добавлена обработка капчи при авторизации с возможностью использования callback-функции для её обработки ([#140](https://github.com/MarshalX/yandex-music-api/issues/140))**:
+  - **Новые исключения**:
+    - **Captcha**:
+      - CaptchaRequired.
+      - CaptchaWrong.
+  - **Новые классы**:
+    - CaptchaResponse.
+  - **Новые примеры в `README`**:
+    - Пример обработки с использованием callback-функции.
+    - Пример полностью своей обработки капчи.
+- Добавлена документация для класса `Search` ([#83](https://github.com/MarshalX/yandex-music-api/issues/83)).
+- **Добавлена возможность получения всех альбомов исполнителя ([#141](https://github.com/MarshalX/yandex-music-api/issues/141))**:
+  - **Новые классы**:
+    - ArtistAlbums.
+  - **Новые методы**:
+    - `artists_direct_albums` у `Client`.
+    - `get_albums` у `Artist`.
+- **Добавлена обработка несуществующего плейлиста ([#147](https://github.com/MarshalX/yandex-music-api/issues/147))**:
+  - **Новые классы**:
+    - `PlaylistAbsence`.
 
 **Незначительные изменения и/или исправления**
 
-- Исправлен баг с загрузкой файлов (`#149`_).
-- Исправлен баг некорректной десериализации плейлиста при отсутствии прав на него (`#147`_).
-- Исправлен баг неправильной десериализации треков и артистов у собственных загруженных файлов (`#154`_).
-
-.. _`#139`: https://github.com/MarshalX/yandex-music-api/issues/139
-.. _`#140`: https://github.com/MarshalX/yandex-music-api/issues/140
-.. _`#83`: https://github.com/MarshalX/yandex-music-api/issues/83
-.. _`#141`: https://github.com/MarshalX/yandex-music-api/issues/141
-.. _`#149`: https://github.com/MarshalX/yandex-music-api/issues/149
-.. _`#147`: https://github.com/MarshalX/yandex-music-api/issues/147
-.. _`#154`: https://github.com/MarshalX/yandex-music-api/issues/154
+- Исправлен баг с загрузкой файлов ([#149](https://github.com/MarshalX/yandex-music-api/issues/149)).
+- Исправлен баг некорректной десериализации плейлиста при отсутствии прав на него ([#147](https://github.com/MarshalX/yandex-music-api/issues/147)).
+- Исправлен баг неправильной десериализации треков и артистов у собственных загруженных файлов ([#154](https://github.com/MarshalX/yandex-music-api/issues/154)).
 
-Версия 0.0.14
-=============
+## Версия 0.0.14
 
 **10.11.2019**
 
 **Переломные изменения**
 
 - Практически у всех классов был обновлён список полей участвующих при сравнении объектов.
 - Если в атрибутах для сравнения объектов присутствуют списки, то они будут преобразованы к frozenset.
 - Убрано конвертирование даты из строки в объект. Теперь все даты представлены строками в ISO формате.
-- Классы ``AlbumSearchResult``, ``ArtistSearchResult``, ``PlaylistSearchResult``, ``TrackSearchResult``, ``VideoSearchResult`` были объединены в один - ``SearchResult``.
+- Классы `AlbumSearchResult`, `ArtistSearchResult`, `PlaylistSearchResult`, `TrackSearchResult`, `VideoSearchResult` были объединены в один – `SearchResult`.
 
 **Крупные изменения**
 
-- Добавлен метод получения треков исполнителя (`#123`_).
-- Добавлены классы-обёртки над пагинацией (``Pager``) и списка треков артиста (``ArtistsTracks``).
+- Добавлен метод получения треков исполнителя ([#123](https://github.com/MarshalX/yandex-music-api/pull/123)).
+- Добавлены классы-обёртки над пагинацией (`Pager`) и списка треков артиста (`ArtistsTracks`).
 - Добавлено **554** unit-теста для всех классов-обёрток над объектами API.
 - Добавлен codecov и workflows для GitHub Actions.
 
-.. _`#123`: https://github.com/MarshalX/yandex-music-api/pull/123
-
 **Незначительные изменения и/или исправления**
 
-- Поле ``cover_uri`` класса ``Album`` теперь опциональное.
-- Поле ``region`` у класса ``Account`` теперь не обязательное.
-- Исправлен баг в ``.to_dict()`` методе, связанный с десериализцией объектов списков и словарей.
-- Исправлен баг в ``.to_dict()`` методе, связанный с не рекурсивной десериализацией.
-- Исправлена десериализация ``similar_artists`` в ``BriefInfo``.
-- Исправлен баг с десериализацией ``artist`` в классе ``ArtistEvent``.
-- Исправлен баг десериализации списка альбомов и артистов у класса ``Track`` (`#122`_).
+- Поле `cover_uri` класса `Album` теперь опциональное.
+- Поле `region` у класса `Account` теперь не обязательное.
+- Исправлен баг в `.to_dict()` методе, связанный с десериализацией объектов списков и словарей.
+- Исправлен баг в `.to_dict()` методе, связанный с не рекурсивной десериализацией.
+- Исправлена десериализация `similar_artists` в `BriefInfo`.
+- Исправлен баг с десериализацией `artist` в классе `ArtistEvent`.
+- Исправлен баг десериализации списка альбомов и артистов у класса `Track` ([#122](https://github.com/MarshalX/yandex-music-api/pull/122)).
 - Исправлена загрузка обложки у трека.
 - Исправлены сравнения объектов.
-
-.. _`#122`: https://github.com/MarshalX/yandex-music-api/pull/122
```

### Comparing `yandex-music-2.0.1/LICENSE` & `yandex-music-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/PKG-INFO` & `yandex-music-2.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,449 +1,320 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: yandex-music
-Version: 2.0.1
+Version: 2.1.0
 Summary: Неофициальная Python библиотека для работы с API сервиса Яндекс.Музыка.
 Home-page: https://github.com/MarshalX/yandex-music-api/
-Author: Il`ya Semyonov
+Author: Ilya (Marshal)
 Author-email: ilya@marshal.dev
 License: LGPLv3
-Project-URL: Code, https://github.com/MarshalX/yandex-music-api
-Project-URL: Documentation, https://yandex-music.readthedocs.io
-Project-URL: Chat, https://t.me/yandex_music_api
+Project-URL: Documentation, https://yandex-music.rtfd.io
+Project-URL: Telegram chat, https://t.me/yandex_music_api
 Project-URL: Codecov, https://codecov.io/gh/MarshalX/yandex-music-api
-Project-URL: Codacy, https://www.codacy.com/manual/MarshalX/yandex-music-api
-Description: ================
-        Yandex Music API
-        ================
+Project-URL: Codacy, https://app.codacy.com/gh/MarshalX/yandex-music-api
+Description: ## Yandex Music API
         
-            Делаю то, что по определённым причинам не сделала компания Yandex.
+        > Делаю то, что по определённым причинам не сделала компания Yandex.
         
         ⚠️ Это неофициальная библиотека.
         
-        Сообщество разработчиков общаются и помогают друг другу
-        в `Telegram чате <https://t.me/yandex_music_api>`_, присоединяйтесь!
+        Сообщество разработчиков общаются и помогают друг другу в [Telegram чате](https://t.me/yandex_music_api), присоединяйтесь!
         
-        .. image:: https://img.shields.io/badge/python-3.7+-blue.svg
-           :target: https://pypi.org/project/yandex-music/
-           :alt: Поддерживаемые Python версии
+        [![Поддерживаемые Python версии](https://img.shields.io/badge/python-3.7+-blue.svg)](https://pypi.org/project/yandex-music/)
+        [![Покрытие кода тестами](https://codecov.io/gh/MarshalX/yandex-music-api/branch/main/graph/badge.svg)](https://codecov.io/gh/MarshalX/yandex-music-api)
+        [![Качество кода](https://api.codacy.com/project/badge/Grade/27011a5a8d9f4b278d1bfe2fe8725fed)](https://app.codacy.com/gh/MarshalX/yandex-music-api)
+        [![Статус тестов](https://github.com/MarshalX/yandex-music-api/actions/workflows/pytest_full.yml/badge.svg)](https://github.com/MarshalX/yandex-music-api/actions/workflows/pytest_full.yml)
+        [![Статус документации](https://readthedocs.org/projects/yandex-music/badge/?version=latest)](https://yandex-music.readthedocs.io/en/latest/?badge=latest)
+        [![Лицензия LGPLv3](https://img.shields.io/badge/license-LGPLv3-lightgrey.svg)](https://www.gnu.org/licenses/lgpl-3.0.html)
+        
+        ### Содержание
+          - [Введение](#введение)
+            1.  [Доступ к вашим данным Яндекс.Музыка](#доступ-к-вашим-данным-яндексмузыка)
+          - [Установка](#установка)
+          - [Начало работы](#начало-работы)
+            1.  [Изучение по примерам](#изучение-по-примерам)
+            2.  [Особенности использования асинхронного клиента](#особенности-использования-асинхронного-клиента)
+            3.  [Логирование](#логирование)
+            4.  [Документация](#документация)
+          - [Получение помощи](#получение-помощи)
+          - [Список изменений](#список-изменений)
+          - [Реализации на других языках](#реализации-на-других-языках)
+            1.  [C#](#c)
+            2.  [PHP](#php)
+            3.  [JavaScript](#javascript)
+          - [Разработанные проекты](#разработанные-проекты)
+            1.  [Плагин для Kodi](#плагин-для-kodi)
+            2.  [Telegram бот-клиент](#telegram-бот-клиент)
+          - [Благодарность](#благодарность)
+          - [Внесение своего вклада в проект](#внесение-своего-вклада-в-проект)
+          - [Спонсоры](#спонсоры)
+          - [Лицензия](#лицензия)
+        
+        ### Введение
+        
+        Эта библиотека предоставляется Python интерфейс для никем незадокументированного и сделанного только для себя API Яндекс Музыки.
+        
+        Она совместима с версиями Python 3.7+ и поддерживает работу как с синхронном, так и асинхронным (asyncio) кодом.
         
-        .. image:: https://codecov.io/gh/MarshalX/yandex-music-api/branch/main/graph/badge.svg
-           :target: https://codecov.io/gh/MarshalX/yandex-music-api
-           :alt: Покрытие кода тестами
+        В дополнение к реализации чистого API данная библиотека имеет ряд классов-обёрток объектов высокого уровня дабы сделать разработку клиентов и скриптов простой и понятной. Вся документация была написана с нуля исходя из логического анализа в ходе обратной разработки(reverse engineering) API.
         
-        .. image:: https://api.codacy.com/project/badge/Grade/27011a5a8d9f4b278d1bfe2fe8725fed
-           :target: https://www.codacy.com/manual/MarshalX/yandex-music-api
-           :alt: Качество кода
+        #### Доступ к вашим данным Яндекс.Музыка
         
-        .. image:: https://github.com/MarshalX/yandex-music-api/actions/workflows/pytest_full.yml/badge.svg
-           :target: https://github.com/MarshalX/yandex-music-api/actions/workflows/pytest_full.yml
-           :alt: Статус тестов
+        Начиная с версии [2.0.0](https://github.com/MarshalX/yandex-music-api/blob/a30082f4929e56381c870cb03103777ae29bcc6b/CHANGES.rst#%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D1%8F-200) библиотека больше не предоставляет интерфейсы для работы с OAuth Яндекс и Яндекс.Паспорт. Задача по получению токена для доступа к данным на плечах разработчиков использующих данную библиотеку. О том как получить токен читайте в документации.
         
-        .. image:: https://readthedocs.org/projects/yandex-music/badge/?version=latest
-           :target: https://yandex-music.readthedocs.io/en/latest/?badge=latest
-           :alt: Статус документации
-        
-        .. image:: https://img.shields.io/badge/license-LGPLv3-lightgrey.svg
-           :target: https://www.gnu.org/licenses/lgpl-3.0.html
-           :alt: Лицензия LGPLv3
-        
-        
-        ==========
-        Содержание
-        ==========
-        
-        - `Введение`_
-        
-          #. `Доступ к вашим данным Яндекс.Музыка`_
-        
-        - `Установка`_
-        
-        - `Начало работы`_
-        
-          #. `Изучение по примерам`_
-        
-          #. `Особенности использования асинхронного клиента`_
-        
-          #. `Логирование`_
-        
-          #. `Документация`_
-        
-        - `Получение помощи`_
-        
-        - `Список изменений`_
-        
-        - `Реализации на других языках`_
-        
-          #. `C#`_
-        
-          #. `PHP`_
-        
-          #. `JavaScript`_
-        
-        - `Разработанные проекты`_
-        
-          #. `Плагин для Kodi`_
-        
-          #. `Telegram бот-клиент`_
-        
-        - `Благодарность`_
-        
-        - `Внесение своего вклада в проект`_
-        
-        - `Лицензия`_
-        
-        ========
-        Введение
-        ========
-        
-        Эта библиотека предоставляется Python интерфейс для никем
-        незадокументированного и сделанного только для себя API Яндекс Музыки.
-        
-        Она совместима с версиями Python 3.7+ и поддерживает работу как с синхронном,
-        так и асинхронным (asyncio) кодом.
-        
-        В дополнение к реализации чистого API данная библиотека имеет ряд
-        классов-обёрток объектов высокого уровня дабы сделать разработку клиентов
-        и скриптов простой и понятной. Вся документация была написана с нуля исходя
-        из логического анализа в ходе обратной разработки (reverse engineering) API.
-        
-        -----------------------------------
-        Доступ к вашим данным Яндекс.Музыка
-        -----------------------------------
-        
-        Начиная с версии `2.0.0 <https://github.com/MarshalX/yandex-music-api/blob/main/CHANGES.rst#%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D1%8F-200>`_ библиотека больше не предоставляет интерфейсы для работы
-        с OAuth Яндекс и Яндекс.Паспорт. Задача по получению токена для доступа к данным
-        на плечах разработчиков использующих данную библиотеку.
-        
-        =========
-        Установка
-        =========
+        ### Установка
         
         Вы можете установить или обновить Yandex Music API при помощи:
         
-        .. code:: shell
-        
-            pip install yandex-music --upgrade
+        ``` shell
+        pip install -U yandex-music
+        ```
         
         Или Вы можете установить из исходного кода с помощью:
         
-        .. code:: shell
+        ``` shell
+        git clone https://github.com/MarshalX/yandex-music-api
+        cd yandex-music-api
+        python setup.py install
+        ```
         
-            git clone https://github.com/MarshalX/yandex-music-api
-            cd yandex-music-api
-            python setup.py install
-        
-        =============
-        Начало работы
-        =============
+        ### Начало работы
         
         Приступив к работе первым делом необходимо создать экземпляр клиента.
         
         Инициализация синхронного клиента:
         
-        .. code:: python
-        
-            from yandex_music import Client
+        ``` python
+        from yandex_music import Client
         
-            client = Client()
-            client.init()
+        client = Client()
+        client.init()
         
-            # или
+        # или
         
-            client = Client().init()
+        client = Client().init()
+        ```
         
         Инициализация асинхронного клиента:
         
-        .. code:: python
-        
-            from yandex_music import ClientAsync
+        ``` python
+        from yandex_music import ClientAsync
         
-            client = ClientAsync()
-            await client.init()
+        client = ClientAsync()
+        await client.init()
         
-            # или
+        # или
         
-            client = await Client().init()
+        client = await Client().init()
+        ```
         
-        Вызов ``init()`` необходим для получение информации для упрощения будущих запросов.
+        Вызов `init()` необходим для получение информации для упрощения будущих запросов.
         
-        Работа без авторизации ограничена. Так, например, для загрузки будут доступны
-        только первые 30 секунд аудиофайла. Для понимания всех ограничений зайдите на
-        сайт Яндекс.Музыка под инкогнито и воспользуйтесь сервисом.
+        Работа без авторизации ограничена. Так, например, для загрузки будут доступны только первые 30 секунд аудиофайла. Для понимания всех ограничений зайдите на сайт Яндекс.Музыка под инкогнито и воспользуйтесь сервисом.
         
-        Для доступа к своим личным данным следует авторизоваться.
-        Это осуществляется через токен аккаунта Яндекс.Музыка.
+        Для доступа к своим личным данным следует авторизоваться. Это осуществляется через токен аккаунта Яндекс.Музыка.
         
         Авторизация:
         
-        .. code:: python
+        ``` python
+        from yandex_music import Client
         
-            from yandex_music import Client
+        client = Client('token').init()
+        ```
         
-            client = Client('token').init()
-        
-        После успешного создания клиента Вы вольны в выборе необходимого метода
-        из API. Все они доступны у объекта класса ``Client``. Подробнее в методах клиента
-        в `документации <https://yandex-music.readthedocs.io/en/latest/yandex_music.client.html>`_.
+        После успешного создания клиента Вы вольны в выборе необходимого метода из API. Все они доступны у объекта класса `Client`. Подробнее в методах клиента в [документации](https://yandex-music.readthedocs.io/en/latest/yandex_music.client.html).
         
         Пример получения первого трека из плейлиста "Мне нравится" и его загрузка:
         
-        .. code:: python
-        
-            from yandex_music import Client
+        ``` python
+        from yandex_music import Client
         
-            client = Client('token').init()
-            client.users_likes_tracks()[0].fetch_track().download('example.mp3')
+        client = Client('token').init()
+        client.users_likes_tracks()[0].fetch_track().download('example.mp3')
+        ```
         
-        В примере выше клиент получает список треков которые были отмечены как
-        понравившиеся. API возвращает объект
-        `TracksList <https://yandex-music.readthedocs.io/en/latest/yandex_music.tracks_list.html>`_
-        в котором содержится список с треками класса
-        `TrackShort <https://yandex-music.readthedocs.io/en/latest/yandex_music.track_short.html>`_.
-        Данный класс содержит наиважнейшую информацию о треке и никаких подробностей,
-        поэтому для получения полной версии трека со всей информацией необходимо
-        обратиться к методу ``fetch_track()``. Затем можно скачать трек методом ``download()``.
+        В примере выше клиент получает список треков которые были отмечены как понравившиеся. API возвращает объект [TracksList](https://yandex-music.readthedocs.io/en/latest/yandex_music.tracks_list.html) в котором содержится список с треками класса [TrackShort](https://yandex-music.readthedocs.io/en/latest/yandex_music.track_short.html). Данный класс содержит наиважнейшую информацию о треке и никаких подробностей, поэтому для получения полной версии трека со всей информацией необходимо обратиться к методу `fetch_track()`. Затем можно скачать трек методом `download()`.
         
         Пример получения треков по ID:
         
-        .. code:: python
-        
-            from yandex_music import Client
+        ``` python
+        from yandex_music import Client
         
-            client = Client().init()
-            client.tracks(['10994777:1193829', '40133452:5206873', '48966383:6693286', '51385674:7163467'])
+        client = Client().init()
+        client.tracks(['10994777:1193829', '40133452:5206873', '48966383:6693286', '51385674:7163467'])
+        ```
         
-        В качестве ID трека выступает его уникальный номер и номер альбома.
-        Первым треком из примера является следующий трек:
-        music.yandex.ru/album/**1193829**/track/**10994777**
+        В качестве ID трека выступает его уникальный номер и номер альбома. Первым треком из примера является следующий трек:music.yandex.ru/album/**1193829**/track/**10994777**
         
         Выполнение запросов с использование прокси в синхронной версии:
         
-        .. code:: python
-        
-            from yandex_music.utils.request import Request
-            from yandex_music import Client
-        
-            request = Request(proxy_url='socks5://user:password@host:port')
-            client = Client(request=request).init()
+        ``` python
+        from yandex_music.utils.request import Request
+        from yandex_music import Client
+        
+        request = Request(proxy_url='socks5://user:password@host:port')
+        client = Client(request=request).init()
+        ```
         
         Примеры proxy url:
+          - socks5://user:<password@host>:port
+          - <http://host:port>
+          - <https://host:port>
+          - <http://user:password@host>
         
-        - socks5://user:password@host:port
-        - http://host:port
-        - https://host:port
-        - http://user:password@host
-        
-        Больше примеров тут: `proxies - advanced usage - requests <https://2.python-requests.org/en/master/user/advanced/#proxies>`_
+        Больше примеров тут: [proxies - advanced usage - requests](https://2.python-requests.org/en/master/user/advanced/#proxies)
         
         Выполнение запросов с использование прокси в асинхронной версии:
         
-        .. code:: python
-        
-            from yandex_music.utils.request_async import Request
-            from yandex_music import ClientAsync
-        
-            request = Request(proxy_url='http://user:pass@some.proxy.com')
-            client = await ClientAsync(request=request).init()
+        ``` python
+        from yandex_music.utils.request_async import Request
+        from yandex_music import ClientAsync
+        
+        request = Request(proxy_url='http://user:pass@some.proxy.com')
+        client = await ClientAsync(request=request).init()
+        ```
         
         Socks прокси не поддерживаются в асинхронной версии.
         
-        Про поддерживаемые прокси тут: `proxy support - advanced usage - aiohttp <https://docs.aiohttp.org/en/stable/client_advanced.html#proxy-support>`_
+        Про поддерживаемые прокси тут: [proxy support - advanced usage - aiohttp](https://docs.aiohttp.org/en/stable/client_advanced.html#proxy-support)
         
-        --------------------
-        Изучение по примерам
-        --------------------
+        #### Изучение по примерам
         
-        Вот несколько примеров для обзора. Даже если это не Ваш подход к
-        обучению, пожалуйста, возьмите и бегло просмотрите их.
+        Вот несколько примеров для обзора. Даже если это не Ваш подход к обучению, пожалуйста, возьмите и бегло просмотрите их.
         
-        Код примеров опубликован в открытом доступе, поэтому
-        Вы можете взять его и начать писать вокруг своё.
+        Код примеров опубликован в открытом доступе, поэтому Вы можете взять его и начать писать вокруг своё.
         
-        Посетите `эту страницу <https://github.com/MarshalX/yandex-music-api/blob/main/examples/>`_
-        чтобы изучить официальные примеры.
+        Посетите [эту страницу](https://github.com/MarshalX/yandex-music-api/blob/main/examples/), чтобы изучить официальные примеры.
         
-        ----------------------------------------------
-        Особенности использования асинхронного клиента
-        ----------------------------------------------
+        #### Особенности использования асинхронного клиента
         
         При работе с асинхронной версией библиотеке стоит всегда помнить
         следующие особенности:
-        
-        - Клиент следует импортировать с названием ``ClientAsync``, а не просто ``Client``.
-        - При использовании методов-сокращений нужно выбирать метод с суффиксом ``_async``.
+          - Клиент следует импортировать с названием `ClientAsync`, а не просто `Client`.
+          - При использовании методов-сокращений нужно выбирать метод с суффиксом `_async`.
         
         Пояснение ко второму пункту:
         
-        .. code:: python
-        
-            from yandex_music import ClientAsync
-        
-            client = await ClientAsync('token').init()
-            liked_short_track = (await client.users_likes_tracks())[0]
-        
-            # правильно
-            full_track = await liked_short_track.fetch_track_async()
-            await full_track.download_async()
+        ``` python
+        from yandex_music import ClientAsync
         
-            # НЕПРАВИЛЬНО
-            full_track = await liked_short_track.fetch_track()
-            await full_track.download()
+        client = await ClientAsync('token').init()
+        liked_short_track = (await client.users_likes_tracks())[0]
         
-        -----------
-        Логирование
-        -----------
-        
-        Данная библиотека использует ``logging`` модуль. Чтобы настроить логирование на
-        стандартный вывод, поместите
-        
-        .. code:: python
-        
-            import logging
-            logging.basicConfig(level=logging.DEBUG,
-                                format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+        # правильно
+        full_track = await liked_short_track.fetch_track_async()
+        await full_track.download_async()
+        
+        # НЕПРАВИЛЬНО
+        full_track = await liked_short_track.fetch_track()
+        await full_track.download()
+        ```
+        
+        #### Логирование
+        
+        Данная библиотека использует `logging` модуль. Чтобы настроить логирование на стандартный вывод, поместите
+        
+        ``` python
+        import logging
+        logging.basicConfig(
+            level=logging.DEBUG,
+            format='%(asctime)s - %(name)s - %(levelname)s - %(message)s'
+        )
+        ```
         
         в начало вашего скрипта.
         
-        Вы также можете использовать логирование в вашем приложении, вызвав
-        ``logging.getLogger()`` и установить уровень какой Вы хотите:
+        Вы также можете использовать логирование в вашем приложении, вызвав `logging.getLogger()` и установить уровень какой Вы хотите:
         
-        .. code:: python
+        ``` python
+        logger = logging.getLogger()
+        logger.setLevel(logging.INFO)
+        ```
         
-            logger = logging.getLogger()
-            logger.setLevel(logging.INFO)
+        Если Вы хотите `DEBUG` логирование:
         
-        Если Вы хотите ``DEBUG`` логирование:
+        ``` python
+        logger.setLevel(logging.DEBUG)
+        ```
         
-        .. code:: python
+        ### Документация
         
-            logger.setLevel(logging.DEBUG)
+        Документация `yandex-music-api` расположена на [readthedocs.io](https://yandex-music.readthedocs.io/). Вашей отправной точкой должен быть класс `Client`, а точнее его методы. Именно они выполняют все запросы на API и возвращают Вам готовые объекты. [Класс Client на readthedocs.io](https://yandex-music.readthedocs.io/en/latest/yandex_music.client.html).
         
-        ============
-        Документация
-        ============
+        ### Получение помощи
         
-        Документация ``yandex-music-api`` расположена на
-        `readthedocs.io <https://yandex-music.readthedocs.io/>`_.
-        Вашей отправной точкой должен быть класс ``Client``, а точнее его методы.
-        Именно они выполняют все
-        запросы на API и возвращают Вам готовые объекты.
-        `Класс Client на readthedocs.io <https://yandex-music.readthedocs.io/en/latest/yandex_music.client.html>`_.
+        Получить помощь можно несколькими путями:
+          - Задать вопрос в [Telegram чате](https://t.me/yandex_music_api), где мы помогаем друг другу, присоединяйтесь\!
+          - Сообщить о баге можно [создав Bug Report](https://github.com/MarshalX/yandex-music-api/issues/new?assignees=MarshalX&labels=bug&template=bug-report.md&title=).
+          - Предложить новую фичу или задать вопрос можно [создав discussion](https://github.com/MarshalX/yandex-music-api/discussions/new).
+          - Найти ответ на вопрос в [документации библиотеки](https://yandex-music.readthedocs.io/en/latest/).
         
-        ================
-        Получение помощи
-        ================
+        ### Список изменений
         
-        Получить помощь можно несколькими путями:
+        Весь список изменений ведётся в файле [CHANGES.md](https://github.com/MarshalX/yandex-music-api/blob/main/CHANGES.md).
+        
+        ### Реализации на других языках
         
-        - Задать вопрос в `Telegram чате <https://t.me/yandex_music_api>`_, где мы помогаем друг другу, присоединяйтесь!
-        - Сообщить о баге можно `создав Bug Report <https://github.com/MarshalX/yandex-music-api/issues/new?assignees=MarshalX&labels=bug&template=bug-report.md&title=>`_.
-        - Предложить новую фичу или задать вопрос можно `создав discussion <https://github.com/MarshalX/yandex-music-api/discussions/new>`_.
-        - Найти ответ на вопрос в `документации библиотеки <https://yandex-music.readthedocs.io/en/latest/>`_.
+        #### C#
         
-        ================
-        Список изменений
-        ================
+        Реализация с совершенно другим подходом, так как используется API для frontend'a, а не мобильных и десктопных приложений: [Winster332/Yandex.Music.Api](https://github.com/Winster332/Yandex.Music.Api).
         
-        Весь список изменений ведётся в файле `CHANGES.rst <https://github.com/MarshalX/yandex-music-api/blob/main/CHANGES.rst>`_.
+        [@Winster332](https://github.com/Winster332) не сильно проявляет активность, но существует форк, который продолжил начатое. Эндпоинты изменены с фронтовых на мобильные: [K1llMan/Yandex.Music.Api](https://github.com/K1llMan/Yandex.Music.Api).
         
+        #### PHP
         
-        ===========================
-        Реализации на других языках
-        ===========================
+        Частично переписанная текущая библиотека на PHP: [LuckyWins/yandex-music-api](https://github.com/LuckyWins/yandex-music-api).
         
-        --
-        C#
-        --
+        #### JavaScript
         
-        Реализация с совершенно другим подходом, так как используется API для frontend'a,
-        а не мобильных и десктопных приложений:
-        `Winster332/Yandex.Music.Api <https://github.com/Winster332/Yandex.Music.Api>`_.
+        API wrapper на Node.JS. Не обновлялся больше двух лет: [itsmepetrov/yandex-music-api](https://github.com/itsmepetrov/yandex-music-api). Продолжение разработки заброшенной библиотеки: [kontsevoye/ym-api](https://github.com/kontsevoye/ym-api).
         
-        `@Winster332 <https://github.com/Winster332>`_ не сильно проявляет активность,
-        но существует форк, который продолжил начатое. Эндпоинты изменены с фронтовых на
-        мобильные: `K1llMan/Yandex.Music.Api <https://github.com/K1llMan/Yandex.Music.Api>`_.
+        ### Разработанные проекты
         
-        ---
-        PHP
-        ---
+        #### Плагин для Kodi
         
-        Частично переписанная текущая библиотека на PHP:
-        `LuckyWins/yandex-music-api <https://github.com/LuckyWins/yandex-music-api>`_.
+        Плагин может проигрывать пользовательские плейлисты и плейлисты Яндекса, поиск по Яндекс Музыке, радио.
         
-        ----------
-        JavaScript
-        ----------
+        Сайт проекта: [ymkodi.ru](https://ymkodi.ru/). Исходный код: [kodi.plugin.yandex-music](https://github.com/Angel777d/kodi.plugin.yandex-music).
+        Автор: [@Angel777d](https://github.com/Angel777d).
         
-        API wrapper на Node.JS. Не обновлялся больше двух лет:
-        `itsmepetrov/yandex-music-api <https://github.com/itsmepetrov/yandex-music-api>`_.
-        Продолжение разработки заброшенной библиотеки: `kontsevoye/ym-api <https://github.com/kontsevoye/ym-api>`_.
+        [![Плагин для Kodi](https://raw.githubusercontent.com/Angel777d/kodi.plugin.yandex-music/master/assets/img/kody_yandex_music_plugin.png)](https://ymkodi.ru/)
         
-        =====================
-        Разработанные проекты
-        =====================
+        #### Telegram бот-клиент
         
-        ---------------
-        Плагин для Kodi
-        ---------------
+        Неофициальный бот. Умные и ваши плейлисты, понравившиеся треки. Лайки, дизлайки, текста песен, поиск, распознавание песен, похожие треки! Полноценный клиент на базе мессенджера.
         
-        Плагин может проигрывать пользовательские плейлисты и плейлисты Яндекса, поиск
-        по Яндекс Музыке, радио.
+        Сайт проекта: [music-yandex-bot.ru](https://music-yandex-bot.ru/). Бот в Telegram: [@music\_yandex\_bot](https://t.me/music_yandex_bot). Автор: [@MarshalX](https://github.com/MarshalX).
         
-        Сайт проекта: `ymkodi.ru <https://ymkodi.ru/>`_.
-        Исходный код: `kodi.plugin.yandex-music  <https://github.com/Angel777d/kodi.plugin.yandex-music>`_.
-        Автор: `@Angel777d <https://github.com/Angel777d>`_.
+        Статья на habr.com с описанием реализации: [Под капотом бота-клиента Яндекс.Музыки](https://habr.com/ru/post/487428/).
         
-        .. image:: https://raw.githubusercontent.com/Angel777d/kodi.plugin.yandex-music/master/assets/img/kody_yandex_music_plugin.png
-           :target: https://ymkodi.ru/
-           :alt: Плагин для Kodi
+        [![Telegram бот-клиент](https://hsto.org/webt/uv/4s/a3/uv4sa3pslohuzlmuzrjzteju2dk.png)](https://music-yandex-bot.ru/)
         
-        -------------------
-        Telegram бот-клиент
-        -------------------
+        ### Благодарность
         
-        Неофициальный бот. Умные и ваши плейлисты, понравившиеся треки. Лайки, дизлайки, текста песен,
-        поиск, распознавание песен, похожие треки! Полноценный клиент на базе мессенджера.
+        Спасибо разработчикам `python-telegram-bot`. Выбрал Вас в качестве примера.
         
-        Сайт проекта: `music-yandex-bot.ru <https://music-yandex-bot.ru/>`_.
-        Бот в Telegram: `@music_yandex_bot <https://t.me/music_yandex_bot>`_.
-        Автор: `@MarshalX <https://github.com/MarshalX>`_.
+        ### Внесение своего вклада в проект
         
-        Статья на habr.com с описанием реализации: `Под капотом бота-клиента Яндекс.Музыки <https://habr.com/ru/post/487428/>`_.
+        Внесение своего вклада максимально приветствуется! Есть перечень пунктов, который стоит соблюдать. Каждый пункт перечня расписан в [CONTRIBUTING.md](https://github.com/MarshalX/yandex-music-api/blob/main/CONTRIBUTING.md).
         
-        .. image:: https://hsto.org/webt/uv/4s/a3/uv4sa3pslohuzlmuzrjzteju2dk.png
-           :target: https://music-yandex-bot.ru/
-           :alt: Telegram бот-клиент
+        Вы можете помочь и сообщив о [баге](https://github.com/MarshalX/yandex-music-api/issues/new?assignees=MarshalX&labels=bug&template=bug-report.md&title=) или о [новом поле пришедшем от API](https://github.com/MarshalX/yandex-music-api/issues/new?assignees=&labels=feature&template=found-unknown-fields.md&title=%D0%9D%D0%BE%D0%B2%D0%BE%D0%B5+%D0%BD%D0%B5%D0%B8%D0%B7%D0%B2%D0%B5%D1%81%D1%82%D0%BD%D0%BE%D0%B5+%D0%BF%D0%BE%D0%BB%D0%B5+%D0%BE%D1%82+API).
         
-        =============
-        Благодарность
-        =============
+        ### Спонсоры
         
-        Спасибо разработчикам ``python-telegram-bot``. Выбрал Вас в качестве примера.
+        #### JetBrains
         
-        ===============================
-        Внесение своего вклада в проект
-        ===============================
+        <img height="150" width="150" src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.png" alt="JetBrains Logo (Main) logo.">
         
-        Внесение своего вклада максимально приветствуется! Есть перечень пунктов,
-        который стоит соблюдать. Каждый пункт перечня расписан в `CONTRIBUTING.md <https://github.com/MarshalX/yandex-music-api/blob/main/CONTRIBUTING.md>`_.
+        > JetBrains предоставляет бесплатный набор инструментов для разработки активным контрибьюторам некоммерческих проектов с открытым исходным кодом.
         
-        Вы можете помочь и сообщив о `баге <https://github.com/MarshalX/yandex-music-api/issues/new?assignees=MarshalX&labels=bug&template=bug-report.md&title=>`_
-        или о `новом поле пришедшем от API <https://github.com/MarshalX/yandex-music-api/issues/new?assignees=&labels=feature&template=found-unknown-fields.md&title=%D0%9D%D0%BE%D0%B2%D0%BE%D0%B5+%D0%BD%D0%B5%D0%B8%D0%B7%D0%B2%D0%B5%D1%81%D1%82%D0%BD%D0%BE%D0%B5+%D0%BF%D0%BE%D0%BB%D0%B5+%D0%BE%D1%82+API>`_.
+        [Лицензии для проектов с открытым исходным кодом — Программы поддержки](https://jb.gg/OpenSourceSupport)
         
-        ========
-        Лицензия
-        ========
+        ### Лицензия
         
-        Вы можете копировать, распространять и модифицировать программное обеспечение
-        при условии, что модификации описаны и лицензированы бесплатно в соответствии
-        с  `LGPL-3 <https://www.gnu.org/licenses/lgpl-3.0.html>`_. Произведения
-        производных (включая модификации или что-либо статически связанное с библиотекой)
-        могут распространяться только в соответствии с  LGPL-3, но приложения, которые
-        используют библиотеку, необязательно.
+        Вы можете копировать, распространять и модифицировать программное обеспечение при условии, что модификации описаны и лицензированы бесплатно в соответствии с [LGPL-3](https://www.gnu.org/licenses/lgpl-3.0.html). Произведения производных (включая модификации или что-либо статически связанное с библиотекой) могут распространяться только в соответствии с LGPL-3, но приложения, которые используют библиотеку, необязательно.
         
 Keywords: python yandex music api wrapper library client питон пайтон яндекс музыка апи обёртка библиотека клиент
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: Russian
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -454,11 +325,13 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
```

### Comparing `yandex-music-2.0.1/README.rst` & `yandex-music-2.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,429 +1,301 @@
-================
-Yandex Music API
-================
+## Yandex Music API
 
-    Делаю то, что по определённым причинам не сделала компания Yandex.
+> Делаю то, что по определённым причинам не сделала компания Yandex.
 
 ⚠️ Это неофициальная библиотека.
 
-Сообщество разработчиков общаются и помогают друг другу
-в `Telegram чате <https://t.me/yandex_music_api>`_, присоединяйтесь!
+Сообщество разработчиков общаются и помогают друг другу в [Telegram чате](https://t.me/yandex_music_api), присоединяйтесь!
 
-.. image:: https://img.shields.io/badge/python-3.7+-blue.svg
-   :target: https://pypi.org/project/yandex-music/
-   :alt: Поддерживаемые Python версии
+[![Поддерживаемые Python версии](https://img.shields.io/badge/python-3.7+-blue.svg)](https://pypi.org/project/yandex-music/)
+[![Покрытие кода тестами](https://codecov.io/gh/MarshalX/yandex-music-api/branch/main/graph/badge.svg)](https://codecov.io/gh/MarshalX/yandex-music-api)
+[![Качество кода](https://api.codacy.com/project/badge/Grade/27011a5a8d9f4b278d1bfe2fe8725fed)](https://app.codacy.com/gh/MarshalX/yandex-music-api)
+[![Статус тестов](https://github.com/MarshalX/yandex-music-api/actions/workflows/pytest_full.yml/badge.svg)](https://github.com/MarshalX/yandex-music-api/actions/workflows/pytest_full.yml)
+[![Статус документации](https://readthedocs.org/projects/yandex-music/badge/?version=latest)](https://yandex-music.readthedocs.io/en/latest/?badge=latest)
+[![Лицензия LGPLv3](https://img.shields.io/badge/license-LGPLv3-lightgrey.svg)](https://www.gnu.org/licenses/lgpl-3.0.html)
+
+### Содержание
+  - [Введение](#введение)
+    1.  [Доступ к вашим данным Яндекс.Музыка](#доступ-к-вашим-данным-яндексмузыка)
+  - [Установка](#установка)
+  - [Начало работы](#начало-работы)
+    1.  [Изучение по примерам](#изучение-по-примерам)
+    2.  [Особенности использования асинхронного клиента](#особенности-использования-асинхронного-клиента)
+    3.  [Логирование](#логирование)
+    4.  [Документация](#документация)
+  - [Получение помощи](#получение-помощи)
+  - [Список изменений](#список-изменений)
+  - [Реализации на других языках](#реализации-на-других-языках)
+    1.  [C#](#c)
+    2.  [PHP](#php)
+    3.  [JavaScript](#javascript)
+  - [Разработанные проекты](#разработанные-проекты)
+    1.  [Плагин для Kodi](#плагин-для-kodi)
+    2.  [Telegram бот-клиент](#telegram-бот-клиент)
+  - [Благодарность](#благодарность)
+  - [Внесение своего вклада в проект](#внесение-своего-вклада-в-проект)
+  - [Спонсоры](#спонсоры)
+  - [Лицензия](#лицензия)
+
+### Введение
+
+Эта библиотека предоставляется Python интерфейс для никем незадокументированного и сделанного только для себя API Яндекс Музыки.
+
+Она совместима с версиями Python 3.7+ и поддерживает работу как с синхронном, так и асинхронным (asyncio) кодом.
 
-.. image:: https://codecov.io/gh/MarshalX/yandex-music-api/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/MarshalX/yandex-music-api
-   :alt: Покрытие кода тестами
+В дополнение к реализации чистого API данная библиотека имеет ряд классов-обёрток объектов высокого уровня дабы сделать разработку клиентов и скриптов простой и понятной. Вся документация была написана с нуля исходя из логического анализа в ходе обратной разработки(reverse engineering) API.
 
-.. image:: https://api.codacy.com/project/badge/Grade/27011a5a8d9f4b278d1bfe2fe8725fed
-   :target: https://www.codacy.com/manual/MarshalX/yandex-music-api
-   :alt: Качество кода
+#### Доступ к вашим данным Яндекс.Музыка
 
-.. image:: https://github.com/MarshalX/yandex-music-api/actions/workflows/pytest_full.yml/badge.svg
-   :target: https://github.com/MarshalX/yandex-music-api/actions/workflows/pytest_full.yml
-   :alt: Статус тестов
+Начиная с версии [2.0.0](https://github.com/MarshalX/yandex-music-api/blob/a30082f4929e56381c870cb03103777ae29bcc6b/CHANGES.rst#%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D1%8F-200) библиотека больше не предоставляет интерфейсы для работы с OAuth Яндекс и Яндекс.Паспорт. Задача по получению токена для доступа к данным на плечах разработчиков использующих данную библиотеку. О том как получить токен читайте в документации.
 
-.. image:: https://readthedocs.org/projects/yandex-music/badge/?version=latest
-   :target: https://yandex-music.readthedocs.io/en/latest/?badge=latest
-   :alt: Статус документации
-
-.. image:: https://img.shields.io/badge/license-LGPLv3-lightgrey.svg
-   :target: https://www.gnu.org/licenses/lgpl-3.0.html
-   :alt: Лицензия LGPLv3
-
-
-==========
-Содержание
-==========
-
-- `Введение`_
-
-  #. `Доступ к вашим данным Яндекс.Музыка`_
-
-- `Установка`_
-
-- `Начало работы`_
-
-  #. `Изучение по примерам`_
-
-  #. `Особенности использования асинхронного клиента`_
-
-  #. `Логирование`_
-
-  #. `Документация`_
-
-- `Получение помощи`_
-
-- `Список изменений`_
-
-- `Реализации на других языках`_
-
-  #. `C#`_
-
-  #. `PHP`_
-
-  #. `JavaScript`_
-
-- `Разработанные проекты`_
-
-  #. `Плагин для Kodi`_
-
-  #. `Telegram бот-клиент`_
-
-- `Благодарность`_
-
-- `Внесение своего вклада в проект`_
-
-- `Лицензия`_
-
-========
-Введение
-========
-
-Эта библиотека предоставляется Python интерфейс для никем
-незадокументированного и сделанного только для себя API Яндекс Музыки.
-
-Она совместима с версиями Python 3.7+ и поддерживает работу как с синхронном,
-так и асинхронным (asyncio) кодом.
-
-В дополнение к реализации чистого API данная библиотека имеет ряд
-классов-обёрток объектов высокого уровня дабы сделать разработку клиентов
-и скриптов простой и понятной. Вся документация была написана с нуля исходя
-из логического анализа в ходе обратной разработки (reverse engineering) API.
-
------------------------------------
-Доступ к вашим данным Яндекс.Музыка
------------------------------------
-
-Начиная с версии `2.0.0 <https://github.com/MarshalX/yandex-music-api/blob/main/CHANGES.rst#%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D1%8F-200>`_ библиотека больше не предоставляет интерфейсы для работы
-с OAuth Яндекс и Яндекс.Паспорт. Задача по получению токена для доступа к данным
-на плечах разработчиков использующих данную библиотеку.
-
-=========
-Установка
-=========
+### Установка
 
 Вы можете установить или обновить Yandex Music API при помощи:
 
-.. code:: shell
-
-    pip install yandex-music --upgrade
+``` shell
+pip install -U yandex-music
+```
 
 Или Вы можете установить из исходного кода с помощью:
 
-.. code:: shell
+``` shell
+git clone https://github.com/MarshalX/yandex-music-api
+cd yandex-music-api
+python setup.py install
+```
 
-    git clone https://github.com/MarshalX/yandex-music-api
-    cd yandex-music-api
-    python setup.py install
-
-=============
-Начало работы
-=============
+### Начало работы
 
 Приступив к работе первым делом необходимо создать экземпляр клиента.
 
 Инициализация синхронного клиента:
 
-.. code:: python
-
-    from yandex_music import Client
+``` python
+from yandex_music import Client
 
-    client = Client()
-    client.init()
+client = Client()
+client.init()
 
-    # или
+# или
 
-    client = Client().init()
+client = Client().init()
+```
 
 Инициализация асинхронного клиента:
 
-.. code:: python
-
-    from yandex_music import ClientAsync
+``` python
+from yandex_music import ClientAsync
 
-    client = ClientAsync()
-    await client.init()
+client = ClientAsync()
+await client.init()
 
-    # или
+# или
 
-    client = await Client().init()
+client = await Client().init()
+```
 
-Вызов ``init()`` необходим для получение информации для упрощения будущих запросов.
+Вызов `init()` необходим для получение информации для упрощения будущих запросов.
 
-Работа без авторизации ограничена. Так, например, для загрузки будут доступны
-только первые 30 секунд аудиофайла. Для понимания всех ограничений зайдите на
-сайт Яндекс.Музыка под инкогнито и воспользуйтесь сервисом.
+Работа без авторизации ограничена. Так, например, для загрузки будут доступны только первые 30 секунд аудиофайла. Для понимания всех ограничений зайдите на сайт Яндекс.Музыка под инкогнито и воспользуйтесь сервисом.
 
-Для доступа к своим личным данным следует авторизоваться.
-Это осуществляется через токен аккаунта Яндекс.Музыка.
+Для доступа к своим личным данным следует авторизоваться. Это осуществляется через токен аккаунта Яндекс.Музыка.
 
 Авторизация:
 
-.. code:: python
+``` python
+from yandex_music import Client
 
-    from yandex_music import Client
+client = Client('token').init()
+```
 
-    client = Client('token').init()
-
-После успешного создания клиента Вы вольны в выборе необходимого метода
-из API. Все они доступны у объекта класса ``Client``. Подробнее в методах клиента
-в `документации <https://yandex-music.readthedocs.io/en/latest/yandex_music.client.html>`_.
+После успешного создания клиента Вы вольны в выборе необходимого метода из API. Все они доступны у объекта класса `Client`. Подробнее в методах клиента в [документации](https://yandex-music.readthedocs.io/en/latest/yandex_music.client.html).
 
 Пример получения первого трека из плейлиста "Мне нравится" и его загрузка:
 
-.. code:: python
-
-    from yandex_music import Client
+``` python
+from yandex_music import Client
 
-    client = Client('token').init()
-    client.users_likes_tracks()[0].fetch_track().download('example.mp3')
+client = Client('token').init()
+client.users_likes_tracks()[0].fetch_track().download('example.mp3')
+```
 
-В примере выше клиент получает список треков которые были отмечены как
-понравившиеся. API возвращает объект
-`TracksList <https://yandex-music.readthedocs.io/en/latest/yandex_music.tracks_list.html>`_
-в котором содержится список с треками класса
-`TrackShort <https://yandex-music.readthedocs.io/en/latest/yandex_music.track_short.html>`_.
-Данный класс содержит наиважнейшую информацию о треке и никаких подробностей,
-поэтому для получения полной версии трека со всей информацией необходимо
-обратиться к методу ``fetch_track()``. Затем можно скачать трек методом ``download()``.
+В примере выше клиент получает список треков которые были отмечены как понравившиеся. API возвращает объект [TracksList](https://yandex-music.readthedocs.io/en/latest/yandex_music.tracks_list.html) в котором содержится список с треками класса [TrackShort](https://yandex-music.readthedocs.io/en/latest/yandex_music.track_short.html). Данный класс содержит наиважнейшую информацию о треке и никаких подробностей, поэтому для получения полной версии трека со всей информацией необходимо обратиться к методу `fetch_track()`. Затем можно скачать трек методом `download()`.
 
 Пример получения треков по ID:
 
-.. code:: python
-
-    from yandex_music import Client
+``` python
+from yandex_music import Client
 
-    client = Client().init()
-    client.tracks(['10994777:1193829', '40133452:5206873', '48966383:6693286', '51385674:7163467'])
+client = Client().init()
+client.tracks(['10994777:1193829', '40133452:5206873', '48966383:6693286', '51385674:7163467'])
+```
 
-В качестве ID трека выступает его уникальный номер и номер альбома.
-Первым треком из примера является следующий трек:
-music.yandex.ru/album/**1193829**/track/**10994777**
+В качестве ID трека выступает его уникальный номер и номер альбома. Первым треком из примера является следующий трек:music.yandex.ru/album/**1193829**/track/**10994777**
 
 Выполнение запросов с использование прокси в синхронной версии:
 
-.. code:: python
-
-    from yandex_music.utils.request import Request
-    from yandex_music import Client
-
-    request = Request(proxy_url='socks5://user:password@host:port')
-    client = Client(request=request).init()
+``` python
+from yandex_music.utils.request import Request
+from yandex_music import Client
+
+request = Request(proxy_url='socks5://user:password@host:port')
+client = Client(request=request).init()
+```
 
 Примеры proxy url:
+  - socks5://user:<password@host>:port
+  - <http://host:port>
+  - <https://host:port>
+  - <http://user:password@host>
 
-- socks5://user:password@host:port
-- http://host:port
-- https://host:port
-- http://user:password@host
-
-Больше примеров тут: `proxies - advanced usage - requests <https://2.python-requests.org/en/master/user/advanced/#proxies>`_
+Больше примеров тут: [proxies - advanced usage - requests](https://2.python-requests.org/en/master/user/advanced/#proxies)
 
 Выполнение запросов с использование прокси в асинхронной версии:
 
-.. code:: python
-
-    from yandex_music.utils.request_async import Request
-    from yandex_music import ClientAsync
-
-    request = Request(proxy_url='http://user:pass@some.proxy.com')
-    client = await ClientAsync(request=request).init()
+``` python
+from yandex_music.utils.request_async import Request
+from yandex_music import ClientAsync
+
+request = Request(proxy_url='http://user:pass@some.proxy.com')
+client = await ClientAsync(request=request).init()
+```
 
 Socks прокси не поддерживаются в асинхронной версии.
 
-Про поддерживаемые прокси тут: `proxy support - advanced usage - aiohttp <https://docs.aiohttp.org/en/stable/client_advanced.html#proxy-support>`_
+Про поддерживаемые прокси тут: [proxy support - advanced usage - aiohttp](https://docs.aiohttp.org/en/stable/client_advanced.html#proxy-support)
 
---------------------
-Изучение по примерам
---------------------
+#### Изучение по примерам
 
-Вот несколько примеров для обзора. Даже если это не Ваш подход к
-обучению, пожалуйста, возьмите и бегло просмотрите их.
+Вот несколько примеров для обзора. Даже если это не Ваш подход к обучению, пожалуйста, возьмите и бегло просмотрите их.
 
-Код примеров опубликован в открытом доступе, поэтому
-Вы можете взять его и начать писать вокруг своё.
+Код примеров опубликован в открытом доступе, поэтому Вы можете взять его и начать писать вокруг своё.
 
-Посетите `эту страницу <https://github.com/MarshalX/yandex-music-api/blob/main/examples/>`_
-чтобы изучить официальные примеры.
+Посетите [эту страницу](https://github.com/MarshalX/yandex-music-api/blob/main/examples/), чтобы изучить официальные примеры.
 
-----------------------------------------------
-Особенности использования асинхронного клиента
-----------------------------------------------
+#### Особенности использования асинхронного клиента
 
 При работе с асинхронной версией библиотеке стоит всегда помнить
 следующие особенности:
-
-- Клиент следует импортировать с названием ``ClientAsync``, а не просто ``Client``.
-- При использовании методов-сокращений нужно выбирать метод с суффиксом ``_async``.
+  - Клиент следует импортировать с названием `ClientAsync`, а не просто `Client`.
+  - При использовании методов-сокращений нужно выбирать метод с суффиксом `_async`.
 
 Пояснение ко второму пункту:
 
-.. code:: python
-
-    from yandex_music import ClientAsync
-
-    client = await ClientAsync('token').init()
-    liked_short_track = (await client.users_likes_tracks())[0]
-
-    # правильно
-    full_track = await liked_short_track.fetch_track_async()
-    await full_track.download_async()
+``` python
+from yandex_music import ClientAsync
 
-    # НЕПРАВИЛЬНО
-    full_track = await liked_short_track.fetch_track()
-    await full_track.download()
+client = await ClientAsync('token').init()
+liked_short_track = (await client.users_likes_tracks())[0]
 
------------
-Логирование
------------
-
-Данная библиотека использует ``logging`` модуль. Чтобы настроить логирование на
-стандартный вывод, поместите
-
-.. code:: python
-
-    import logging
-    logging.basicConfig(level=logging.DEBUG,
-                        format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+# правильно
+full_track = await liked_short_track.fetch_track_async()
+await full_track.download_async()
+
+# НЕПРАВИЛЬНО
+full_track = await liked_short_track.fetch_track()
+await full_track.download()
+```
+
+#### Логирование
+
+Данная библиотека использует `logging` модуль. Чтобы настроить логирование на стандартный вывод, поместите
+
+``` python
+import logging
+logging.basicConfig(
+    level=logging.DEBUG,
+    format='%(asctime)s - %(name)s - %(levelname)s - %(message)s'
+)
+```
 
 в начало вашего скрипта.
 
-Вы также можете использовать логирование в вашем приложении, вызвав
-``logging.getLogger()`` и установить уровень какой Вы хотите:
+Вы также можете использовать логирование в вашем приложении, вызвав `logging.getLogger()` и установить уровень какой Вы хотите:
 
-.. code:: python
+``` python
+logger = logging.getLogger()
+logger.setLevel(logging.INFO)
+```
 
-    logger = logging.getLogger()
-    logger.setLevel(logging.INFO)
+Если Вы хотите `DEBUG` логирование:
 
-Если Вы хотите ``DEBUG`` логирование:
+``` python
+logger.setLevel(logging.DEBUG)
+```
 
-.. code:: python
+### Документация
 
-    logger.setLevel(logging.DEBUG)
+Документация `yandex-music-api` расположена на [readthedocs.io](https://yandex-music.readthedocs.io/). Вашей отправной точкой должен быть класс `Client`, а точнее его методы. Именно они выполняют все запросы на API и возвращают Вам готовые объекты. [Класс Client на readthedocs.io](https://yandex-music.readthedocs.io/en/latest/yandex_music.client.html).
 
-============
-Документация
-============
+### Получение помощи
 
-Документация ``yandex-music-api`` расположена на
-`readthedocs.io <https://yandex-music.readthedocs.io/>`_.
-Вашей отправной точкой должен быть класс ``Client``, а точнее его методы.
-Именно они выполняют все
-запросы на API и возвращают Вам готовые объекты.
-`Класс Client на readthedocs.io <https://yandex-music.readthedocs.io/en/latest/yandex_music.client.html>`_.
+Получить помощь можно несколькими путями:
+  - Задать вопрос в [Telegram чате](https://t.me/yandex_music_api), где мы помогаем друг другу, присоединяйтесь\!
+  - Сообщить о баге можно [создав Bug Report](https://github.com/MarshalX/yandex-music-api/issues/new?assignees=MarshalX&labels=bug&template=bug-report.md&title=).
+  - Предложить новую фичу или задать вопрос можно [создав discussion](https://github.com/MarshalX/yandex-music-api/discussions/new).
+  - Найти ответ на вопрос в [документации библиотеки](https://yandex-music.readthedocs.io/en/latest/).
 
-================
-Получение помощи
-================
+### Список изменений
 
-Получить помощь можно несколькими путями:
+Весь список изменений ведётся в файле [CHANGES.md](https://github.com/MarshalX/yandex-music-api/blob/main/CHANGES.md).
+
+### Реализации на других языках
 
-- Задать вопрос в `Telegram чате <https://t.me/yandex_music_api>`_, где мы помогаем друг другу, присоединяйтесь!
-- Сообщить о баге можно `создав Bug Report <https://github.com/MarshalX/yandex-music-api/issues/new?assignees=MarshalX&labels=bug&template=bug-report.md&title=>`_.
-- Предложить новую фичу или задать вопрос можно `создав discussion <https://github.com/MarshalX/yandex-music-api/discussions/new>`_.
-- Найти ответ на вопрос в `документации библиотеки <https://yandex-music.readthedocs.io/en/latest/>`_.
+#### C#
 
-================
-Список изменений
-================
+Реализация с совершенно другим подходом, так как используется API для frontend'a, а не мобильных и десктопных приложений: [Winster332/Yandex.Music.Api](https://github.com/Winster332/Yandex.Music.Api).
 
-Весь список изменений ведётся в файле `CHANGES.rst <https://github.com/MarshalX/yandex-music-api/blob/main/CHANGES.rst>`_.
+[@Winster332](https://github.com/Winster332) не сильно проявляет активность, но существует форк, который продолжил начатое. Эндпоинты изменены с фронтовых на мобильные: [K1llMan/Yandex.Music.Api](https://github.com/K1llMan/Yandex.Music.Api).
 
+#### PHP
 
-===========================
-Реализации на других языках
-===========================
+Частично переписанная текущая библиотека на PHP: [LuckyWins/yandex-music-api](https://github.com/LuckyWins/yandex-music-api).
 
---
-C#
---
+#### JavaScript
 
-Реализация с совершенно другим подходом, так как используется API для frontend'a,
-а не мобильных и десктопных приложений:
-`Winster332/Yandex.Music.Api <https://github.com/Winster332/Yandex.Music.Api>`_.
+API wrapper на Node.JS. Не обновлялся больше двух лет: [itsmepetrov/yandex-music-api](https://github.com/itsmepetrov/yandex-music-api). Продолжение разработки заброшенной библиотеки: [kontsevoye/ym-api](https://github.com/kontsevoye/ym-api).
 
-`@Winster332 <https://github.com/Winster332>`_ не сильно проявляет активность,
-но существует форк, который продолжил начатое. Эндпоинты изменены с фронтовых на
-мобильные: `K1llMan/Yandex.Music.Api <https://github.com/K1llMan/Yandex.Music.Api>`_.
+### Разработанные проекты
 
----
-PHP
----
+#### Плагин для Kodi
 
-Частично переписанная текущая библиотека на PHP:
-`LuckyWins/yandex-music-api <https://github.com/LuckyWins/yandex-music-api>`_.
+Плагин может проигрывать пользовательские плейлисты и плейлисты Яндекса, поиск по Яндекс Музыке, радио.
 
-----------
-JavaScript
-----------
+Сайт проекта: [ymkodi.ru](https://ymkodi.ru/). Исходный код: [kodi.plugin.yandex-music](https://github.com/Angel777d/kodi.plugin.yandex-music).
+Автор: [@Angel777d](https://github.com/Angel777d).
 
-API wrapper на Node.JS. Не обновлялся больше двух лет:
-`itsmepetrov/yandex-music-api <https://github.com/itsmepetrov/yandex-music-api>`_.
-Продолжение разработки заброшенной библиотеки: `kontsevoye/ym-api <https://github.com/kontsevoye/ym-api>`_.
+[![Плагин для Kodi](https://raw.githubusercontent.com/Angel777d/kodi.plugin.yandex-music/master/assets/img/kody_yandex_music_plugin.png)](https://ymkodi.ru/)
 
-=====================
-Разработанные проекты
-=====================
+#### Telegram бот-клиент
 
----------------
-Плагин для Kodi
----------------
+Неофициальный бот. Умные и ваши плейлисты, понравившиеся треки. Лайки, дизлайки, текста песен, поиск, распознавание песен, похожие треки! Полноценный клиент на базе мессенджера.
 
-Плагин может проигрывать пользовательские плейлисты и плейлисты Яндекса, поиск
-по Яндекс Музыке, радио.
+Сайт проекта: [music-yandex-bot.ru](https://music-yandex-bot.ru/). Бот в Telegram: [@music\_yandex\_bot](https://t.me/music_yandex_bot). Автор: [@MarshalX](https://github.com/MarshalX).
 
-Сайт проекта: `ymkodi.ru <https://ymkodi.ru/>`_.
-Исходный код: `kodi.plugin.yandex-music  <https://github.com/Angel777d/kodi.plugin.yandex-music>`_.
-Автор: `@Angel777d <https://github.com/Angel777d>`_.
+Статья на habr.com с описанием реализации: [Под капотом бота-клиента Яндекс.Музыки](https://habr.com/ru/post/487428/).
 
-.. image:: https://raw.githubusercontent.com/Angel777d/kodi.plugin.yandex-music/master/assets/img/kody_yandex_music_plugin.png
-   :target: https://ymkodi.ru/
-   :alt: Плагин для Kodi
+[![Telegram бот-клиент](https://hsto.org/webt/uv/4s/a3/uv4sa3pslohuzlmuzrjzteju2dk.png)](https://music-yandex-bot.ru/)
 
--------------------
-Telegram бот-клиент
--------------------
+### Благодарность
 
-Неофициальный бот. Умные и ваши плейлисты, понравившиеся треки. Лайки, дизлайки, текста песен,
-поиск, распознавание песен, похожие треки! Полноценный клиент на базе мессенджера.
+Спасибо разработчикам `python-telegram-bot`. Выбрал Вас в качестве примера.
 
-Сайт проекта: `music-yandex-bot.ru <https://music-yandex-bot.ru/>`_.
-Бот в Telegram: `@music_yandex_bot <https://t.me/music_yandex_bot>`_.
-Автор: `@MarshalX <https://github.com/MarshalX>`_.
+### Внесение своего вклада в проект
 
-Статья на habr.com с описанием реализации: `Под капотом бота-клиента Яндекс.Музыки <https://habr.com/ru/post/487428/>`_.
+Внесение своего вклада максимально приветствуется! Есть перечень пунктов, который стоит соблюдать. Каждый пункт перечня расписан в [CONTRIBUTING.md](https://github.com/MarshalX/yandex-music-api/blob/main/CONTRIBUTING.md).
 
-.. image:: https://hsto.org/webt/uv/4s/a3/uv4sa3pslohuzlmuzrjzteju2dk.png
-   :target: https://music-yandex-bot.ru/
-   :alt: Telegram бот-клиент
+Вы можете помочь и сообщив о [баге](https://github.com/MarshalX/yandex-music-api/issues/new?assignees=MarshalX&labels=bug&template=bug-report.md&title=) или о [новом поле пришедшем от API](https://github.com/MarshalX/yandex-music-api/issues/new?assignees=&labels=feature&template=found-unknown-fields.md&title=%D0%9D%D0%BE%D0%B2%D0%BE%D0%B5+%D0%BD%D0%B5%D0%B8%D0%B7%D0%B2%D0%B5%D1%81%D1%82%D0%BD%D0%BE%D0%B5+%D0%BF%D0%BE%D0%BB%D0%B5+%D0%BE%D1%82+API).
 
-=============
-Благодарность
-=============
+### Спонсоры
 
-Спасибо разработчикам ``python-telegram-bot``. Выбрал Вас в качестве примера.
+#### JetBrains
 
-===============================
-Внесение своего вклада в проект
-===============================
+<img height="150" width="150" src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.png" alt="JetBrains Logo (Main) logo.">
 
-Внесение своего вклада максимально приветствуется! Есть перечень пунктов,
-который стоит соблюдать. Каждый пункт перечня расписан в `CONTRIBUTING.md <https://github.com/MarshalX/yandex-music-api/blob/main/CONTRIBUTING.md>`_.
+> JetBrains предоставляет бесплатный набор инструментов для разработки активным контрибьюторам некоммерческих проектов с открытым исходным кодом.
 
-Вы можете помочь и сообщив о `баге <https://github.com/MarshalX/yandex-music-api/issues/new?assignees=MarshalX&labels=bug&template=bug-report.md&title=>`_
-или о `новом поле пришедшем от API <https://github.com/MarshalX/yandex-music-api/issues/new?assignees=&labels=feature&template=found-unknown-fields.md&title=%D0%9D%D0%BE%D0%B2%D0%BE%D0%B5+%D0%BD%D0%B5%D0%B8%D0%B7%D0%B2%D0%B5%D1%81%D1%82%D0%BD%D0%BE%D0%B5+%D0%BF%D0%BE%D0%BB%D0%B5+%D0%BE%D1%82+API>`_.
+[Лицензии для проектов с открытым исходным кодом — Программы поддержки](https://jb.gg/OpenSourceSupport)
 
-========
-Лицензия
-========
+### Лицензия
 
-Вы можете копировать, распространять и модифицировать программное обеспечение
-при условии, что модификации описаны и лицензированы бесплатно в соответствии
-с  `LGPL-3 <https://www.gnu.org/licenses/lgpl-3.0.html>`_. Произведения
-производных (включая модификации или что-либо статически связанное с библиотекой)
-могут распространяться только в соответствии с  LGPL-3, но приложения, которые
-используют библиотеку, необязательно.
+Вы можете копировать, распространять и модифицировать программное обеспечение при условии, что модификации описаны и лицензированы бесплатно в соответствии с [LGPL-3](https://www.gnu.org/licenses/lgpl-3.0.html). Произведения производных (включая модификации или что-либо статически связанное с библиотекой) могут распространяться только в соответствии с LGPL-3, но приложения, которые используют библиотеку, необязательно.
```

### Comparing `yandex-music-2.0.1/setup.py` & `yandex-music-2.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,29 @@
 
         sys.exit(pytest.main(['tests']))
 
 
 with open('yandex_music/__init__.py', encoding='utf-8') as f:
     version = re.findall(r"__version__ = '(.+)'", f.read())[0]
 
-with open('README.rst', 'r', encoding='utf-8') as f:
+with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='yandex-music',
     version=version,
-    author='Il`ya Semyonov',
+    author='Ilya (Marshal)',
     author_email='ilya@marshal.dev',
     license='LGPLv3',
     url='https://github.com/MarshalX/yandex-music-api/',
     keywords='python yandex music api wrapper library client питон пайтон '
     'яндекс музыка апи обёртка библиотека клиент',
     description='Неофициальная Python библиотека для работы с API сервиса Яндекс.Музыка.',
     long_description=readme,
+    long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=['requests[socks]', 'aiohttp', 'aiofiles'],
     include_package_data=True,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Natural Language :: Russian',
         'Intended Audience :: Developers',
@@ -44,22 +45,22 @@
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         "Programming Language :: Python :: Implementation",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     python_requires="~=3.7",
     cmdclass={'test': PyTest},
     tests_require=['pytest'],
     project_urls={
-        'Code': 'https://github.com/MarshalX/yandex-music-api',
-        'Documentation': 'https://yandex-music.readthedocs.io',
-        'Chat': 'https://t.me/yandex_music_api',
+        'Documentation': 'https://yandex-music.rtfd.io',
+        'Telegram chat': 'https://t.me/yandex_music_api',
         'Codecov': 'https://codecov.io/gh/MarshalX/yandex-music-api',
-        'Codacy': 'https://www.codacy.com/manual/MarshalX/yandex-music-api',
+        'Codacy': 'https://app.codacy.com/gh/MarshalX/yandex-music-api',
     },
 )
```

### Comparing `yandex-music-2.0.1/tests/__init__.py` & `yandex-music-2.1.0/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,7 +89,12 @@
 from .test_operator import TestOperator
 from .test_contest import TestContest
 from .test_open_graph_data import TestOpenGraphData
 from .test_brand import TestBrand
 from .test_context import TestContext
 from .test_queue_item import TestQueueItem
 from .test_deprecation import TestDeprecation
+from .test_lyrics_major import TestLyricsMajor
+from .test_track_lyrics import TestTrackLyrics
+from .test_custom_wave import TestCustomWave
+from .test_r128 import TestR128
+from .test_lyrics_info import TestLyricsInfo
```

### Comparing `yandex-music-2.0.1/tests/conftest.py` & `yandex-music-2.1.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     ChartInfo,
     ChartInfoMenu,
     ChartInfoMenuItem,
     ChartItem,
     Client,
     Counts,
     Cover,
+    CustomWave,
     Day,
     Description,
     DiscreteScale,
     Enum,
     Event,
     GeneratedPlaylist,
     Icon,
@@ -88,14 +89,18 @@
     Deactivation,
     Operator,
     Contest,
     OpenGraphData,
     Brand,
     Context,
     Deprecation,
+    TrackLyrics,
+    LyricsMajor,
+    R128,
+    LyricsInfo,
 )
 from . import (
     TestAccount,
     TestAdParams,
     TestAlbum,
     TestArtist,
     TestAutoRenewable,
@@ -104,14 +109,15 @@
     TestBlockEntity,
     TestCaseForms,
     TestChart,
     TestChartInfo,
     TestChartInfoMenuItem,
     TestCounts,
     TestCover,
+    TestCustomWave,
     TestDay,
     TestDescription,
     TestDiscreteScale,
     TestEnum,
     TestEvent,
     TestGeneratedPlaylist,
     TestIcon,
@@ -174,14 +180,18 @@
     TestDeactivation,
     TestOperator,
     TestContest,
     TestOpenGraphData,
     TestBrand,
     TestContext,
     TestDeprecation,
+    TestLyricsMajor,
+    TestTrackLyrics,
+    TestR128,
+    TestLyricsInfo,
 )
 
 
 @pytest.fixture(scope='session')
 def artist_factory(cover, counts, ratings, link, description):
     class ArtistFactory:
         def get(self, popular_tracks, decomposed=None):
@@ -238,15 +248,15 @@
 
 @pytest.fixture(scope='session')
 def artist_decomposed(artist_without_nested_artist):
     return [' & ', artist_without_nested_artist]
 
 
 @pytest.fixture(scope='session')
-def track_factory(major, normalization, user, meta_data, poetry_lover_match):
+def track_factory(major, normalization, user, meta_data, poetry_lover_match, r_128, lyrics_info):
     class TrackFactory:
         def get(self, artists, albums, track_without_nested_tracks=None):
             return Track(
                 TestTrack.id,
                 TestTrack.title,
                 TestTrack.available,
                 artists,
@@ -280,14 +290,19 @@
                 TestTrack.preview_duration_ms,
                 TestTrack.available_full_without_permission,
                 TestTrack.version,
                 TestTrack.remember_position,
                 TestTrack.background_video_uri,
                 TestTrack.short_description,
                 TestTrack.is_suitable_for_children,
+                TestTrack.track_source,
+                TestTrack.available_for_options,
+                r_128,
+                lyrics_info,
+                TestTrack.track_sharing_flag,
             )
 
     return TrackFactory()
 
 
 @pytest.fixture(scope='session')
 def track(track_factory, artist, album, track_without_nested_tracks):
@@ -311,14 +326,34 @@
 
 @pytest.fixture(scope='session')
 def track_without_nested_tracks(artist, album, track_factory):
     return track_factory.get([artist], [album])
 
 
 @pytest.fixture(scope='session')
+def lyrics_major():
+    return LyricsMajor(
+        TestLyricsMajor.id,
+        TestLyricsMajor.name,
+        TestLyricsMajor.pretty_name,
+    )
+
+
+@pytest.fixture(scope='session')
+def track_lyrics(lyrics_major):
+    return TrackLyrics(
+        TestTrackLyrics.download_url,
+        TestTrackLyrics.lyric_id,
+        TestTrackLyrics.external_lyric_id,
+        TestTrackLyrics.writer,
+        lyrics_major,
+    )
+
+
+@pytest.fixture(scope='session')
 def album_factory(label, track_position):
     class AlbumFactory:
         def get(self, artists, volumes, albums=None, deprecation=None):
             return Album(
                 TestAlbum.id,
                 TestAlbum.error,
                 TestAlbum.title,
@@ -360,14 +395,15 @@
                 albums,
                 TestAlbum.duration_ms,
                 TestAlbum.explicit,
                 TestAlbum.start_date,
                 TestAlbum.likes_count,
                 deprecation,
                 TestAlbum.available_regions,
+                TestAlbum.available_for_options,
             )
 
     return AlbumFactory()
 
 
 @pytest.fixture(scope='session')
 def album(album_factory, artist_without_tracks, track_without_albums, album_without_nested_albums, deprecation):
@@ -395,14 +431,16 @@
     play_counter,
     playlist_absence,
     artist,
     track_id,
     contest,
     open_graph_data,
     brand,
+    custom_wave,
+    pager,
 ):
     class PlaylistFactory:
         def get(self, similar_playlists, last_owner_playlists):
             return Playlist(
                 user,
                 cover,
                 made_for,
@@ -454,14 +492,16 @@
                 TestPlaylist.description,
                 TestPlaylist.description_formatted,
                 TestPlaylist.playlist_uuid,
                 TestPlaylist.type,
                 TestPlaylist.ready,
                 TestPlaylist.is_for_from,
                 TestPlaylist.regions,
+                custom_wave,
+                pager,
             )
 
     return PlaylistFactory()
 
 
 @pytest.fixture(scope='session')
 def playlist(playlist_factory, playlist_without_nested_playlists):
@@ -477,14 +517,15 @@
 def generated_playlist(playlist):
     return GeneratedPlaylist(
         TestGeneratedPlaylist.type,
         TestGeneratedPlaylist.ready,
         TestGeneratedPlaylist.notify,
         playlist,
         TestGeneratedPlaylist.description,
+        TestGeneratedPlaylist.preview_description,
     )
 
 
 @pytest.fixture(scope='session')
 def client():
     return Client()
 
@@ -856,14 +897,15 @@
         TestAccount.first_name,
         TestAccount.display_name,
         TestAccount.hosted_user,
         TestAccount.birthday,
         [passport_phone],
         TestAccount.registered_at,
         TestAccount.has_info_for_app_metrica,
+        TestAccount.child,
     )
 
 
 @pytest.fixture(scope='session')
 def plus():
     return Plus(TestPlus.has_plus, TestPlus.is_tutorial_completed)
 
@@ -875,14 +917,15 @@
 
 @pytest.fixture(scope='session')
 def subscription(renewable_remainder, auto_renewable, operator, non_auto_renewable):
     return Subscription(
         renewable_remainder,
         [auto_renewable],
         [auto_renewable],
+        TestSubscription.had_any_subscription,
         [operator],
         non_auto_renewable,
         TestSubscription.can_start_trial,
         TestSubscription.mcdonalds,
         TestSubscription.end,
     )
 
@@ -994,14 +1037,16 @@
         TestStatus.default_email,
         TestStatus.skips_per_hour,
         TestStatus.station_exists,
         station_data,
         alert,
         TestStatus.premium_region,
         TestStatus.experiment,
+        TestStatus.pretrial_active,
+        TestStatus.userhash,
     )
 
 
 @pytest.fixture(scope='session')
 def station_data():
     return StationData(TestStationData.name)
 
@@ -1127,15 +1172,23 @@
 def chart_item(track, chart):
     return ChartItem(track, chart)
 
 
 @pytest.fixture(scope='session')
 def station_result(station, rotor_settings, ad_params):
     return StationResult(
-        station, rotor_settings, rotor_settings, ad_params, TestStationResult.explanation, TestStationResult.prerolls
+        station,
+        rotor_settings,
+        rotor_settings,
+        ad_params,
+        TestStationResult.explanation,
+        TestStationResult.prerolls,
+        TestStationResult.rup_title,
+        TestStationResult.rup_description,
+        TestStationResult.custom_name,
     )
 
 
 @pytest.fixture(scope='session')
 def ad_params():
     return AdParams(
         TestAdParams.partner_id,
@@ -1258,7 +1311,22 @@
             TestSearchResult.per_page,
             TestSearchResult.order,
             [results[request.param]],
         ),
         [results[request.param]],
         types[request.param],
     )
+
+
+@pytest.fixture(scope='session')
+def custom_wave():
+    return CustomWave(TestCustomWave.title, TestCustomWave.animation_url, TestCustomWave.position)
+
+
+@pytest.fixture(scope='session')
+def r_128():
+    return R128(TestR128.i, TestR128.tp)
+
+
+@pytest.fixture(scope='session')
+def lyrics_info():
+    return LyricsInfo(TestLyricsInfo.has_available_sync_lyrics, TestLyricsInfo.has_available_text_lyrics)
```

### Comparing `yandex-music-2.0.1/tests/test_account.py` & `yandex-music-2.1.0/tests/test_account.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     second_name = 'Семёнов'
     first_name = 'Илья'
     display_name = 'Il`ya (Marshal)'
     hosted_user = False
     birthday = '1999-08-10'
     registered_at = '2018-06-10T09:34:22+00:00'
     has_info_for_app_metrica = False
+    child = False
 
     def test_expected_values(self, account, passport_phone):
         assert account.now == self.now
         assert account.region == self.region
         assert account.service_available == self.service_available
         assert account.uid == self.uid
         assert account.login == self.login
@@ -27,24 +28,26 @@
         assert account.first_name == self.first_name
         assert account.display_name == self.display_name
         assert account.hosted_user == self.hosted_user
         assert account.birthday == self.birthday
         assert account.passport_phones == [passport_phone]
         assert account.registered_at == self.registered_at
         assert account.has_info_for_app_metrica == self.has_info_for_app_metrica
+        assert account.child == self.child
 
     def test_de_json_none(self, client):
         assert Account.de_json({}, client) is None
 
     def test_de_json_required(self, client):
-        json_dict = {'now': self.now, 'service_available': self.service_available}
+        json_dict = {'now': self.now, 'service_available': self.service_available, 'child': self.child}
         account = Account.de_json(json_dict, client)
 
         assert account.now == self.now
         assert account.service_available == self.service_available
+        assert account.child == self.child
 
     def test_de_json_all(self, client, passport_phone):
         json_dict = {
             'now': self.now,
             'region': self.region,
             'service_available': self.service_available,
             'uid': self.uid,
@@ -54,14 +57,15 @@
             'first_name': self.first_name,
             'display_name': self.display_name,
             'hosted_user': self.hosted_user,
             'birthday': self.birthday,
             'passport_phones': [passport_phone.to_dict()],
             'registered_at': self.registered_at,
             'has_info_for_app_metrica': self.has_info_for_app_metrica,
+            'child': self.child,
         }
         account = Account.de_json(json_dict, client)
 
         assert account.now == self.now
         assert account.region == self.region
         assert account.service_available == self.service_available
         assert account.uid == self.uid
@@ -71,14 +75,15 @@
         assert account.first_name == self.first_name
         assert account.display_name == self.display_name
         assert account.hosted_user == self.hosted_user
         assert account.birthday == self.birthday
         assert account.passport_phones == [passport_phone]
         assert account.registered_at == self.registered_at
         assert account.has_info_for_app_metrica == self.has_info_for_app_metrica
+        assert account.child == self.child
 
     def test_equality(self, user):
-        a = Account(self.now, self.service_available)
+        a = Account(self.now, self.service_available, self.child)
 
         assert a != user
         assert hash(a) != hash(user)
         assert a is not user
```

### Comparing `yandex-music-2.0.1/tests/test_ad_params.py` & `yandex-music-2.1.0/tests/test_ad_params.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_album.py` & `yandex-music-2.1.0/tests/test_album.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     lyrics_available = True
     remember_position = False
     duration_ms = 200440
     explicit = False
     start_date = '2020-06-30'
     likes_count = 2
     available_regions = ['kg', 'tm', 'by', 'kz', 'md', 'ru', 'am', 'ge', 'uz', 'tj', 'il', 'az', 'ua']
+    available_for_options = ['bookmate']
 
     def test_expected_values(
         self,
         album,
         artist_without_tracks,
         label,
         track_position,
@@ -97,14 +98,15 @@
         assert album.remember_position == self.remember_position
         assert album.duration_ms == self.duration_ms
         assert album.explicit == self.explicit
         assert album.start_date == self.start_date
         assert album.likes_count == self.likes_count
         assert album.deprecation == deprecation
         assert album.available_regions == self.available_regions
+        assert album.available_for_options == self.available_for_options
 
     def test_de_json_none(self, client):
         assert Album.de_json({}, client) is None
 
     def test_de_list_none(self, client):
         assert Album.de_list({}, client) == []
 
@@ -156,14 +158,15 @@
             'albums': [album_without_nested_albums.to_dict()],
             'duration_ms': self.duration_ms,
             'explicit': self.explicit,
             'start_date': self.start_date,
             'likes_count': self.likes_count,
             'deprecation': deprecation.to_dict(),
             'available_regions': self.available_regions,
+            'available_for_options': self.available_for_options,
         }
         album = Album.de_json(json_dict, client)
 
         assert album.id == self.id
         assert album.error == self.error
         assert album.title == self.title
         assert album.version == self.version
@@ -203,14 +206,15 @@
         assert album.remember_position == self.remember_position
         assert album.duration_ms == self.duration_ms
         assert album.explicit == self.explicit
         assert album.start_date == self.start_date
         assert album.likes_count == self.likes_count
         assert album.deprecation == deprecation
         assert album.available_regions == self.available_regions
+        assert album.available_for_options == self.available_for_options
 
     def test_equality(self, artist, label):
         a = Album(self.id)
         b = Album(10)
         c = Album(self.id)
 
         assert a != b
```

### Comparing `yandex-music-2.0.1/tests/test_album_event.py` & `yandex-music-2.1.0/tests/test_album_event.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_alert.py` & `yandex-music-2.1.0/tests/test_alert.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_alert_button.py` & `yandex-music-2.1.0/tests/test_alert_button.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_artist.py` & `yandex-music-2.1.0/tests/test_artist.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_artist_albums.py` & `yandex-music-2.1.0/tests/test_artist_albums.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_artist_event.py` & `yandex-music-2.1.0/tests/test_artist_event.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_artist_tracks.py` & `yandex-music-2.1.0/tests/test_artist_tracks.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_auto_renewable.py` & `yandex-music-2.1.0/tests/test_auto_renewable.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_best.py` & `yandex-music-2.1.0/tests/test_best.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_block.py` & `yandex-music-2.1.0/tests/test_block.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_block_entity.py` & `yandex-music-2.1.0/tests/test_block_entity.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_brand.py` & `yandex-music-2.1.0/tests/test_brand.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_brief_info.py` & `yandex-music-2.1.0/tests/test_brief_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_case_forms.py` & `yandex-music-2.1.0/tests/test_case_forms.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_chart.py` & `yandex-music-2.1.0/tests/test_chart.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_chart_info.py` & `yandex-music-2.1.0/tests/test_chart_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_chart_info_menu.py` & `yandex-music-2.1.0/tests/test_chart_info_menu.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_chart_info_menu_item.py` & `yandex-music-2.1.0/tests/test_chart_info_menu_item.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_chart_item.py` & `yandex-music-2.1.0/tests/test_chart_item.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_contest.py` & `yandex-music-2.1.0/tests/test_contest.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_context.py` & `yandex-music-2.1.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_counts.py` & `yandex-music-2.1.0/tests/test_counts.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_cover.py` & `yandex-music-2.1.0/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_dashboard.py` & `yandex-music-2.1.0/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_day.py` & `yandex-music-2.1.0/tests/test_day.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_deactivation.py` & `yandex-music-2.1.0/tests/test_deactivation.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_deprecation.py` & `yandex-music-2.1.0/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_description.py` & `yandex-music-2.1.0/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_discrete_scale.py` & `yandex-music-2.1.0/tests/test_discrete_scale.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_download_info.py` & `yandex-music-2.1.0/tests/test_download_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_enum.py` & `yandex-music-2.1.0/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_event.py` & `yandex-music-2.1.0/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_feed.py` & `yandex-music-2.1.0/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_generated_playlist.py` & `yandex-music-2.1.0/tests/test_generated_playlist.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 
 
 class TestGeneratedPlaylist:
     type = 'playlistOfTheDay'
     ready = True
     notify = False
     description = []
+    preview_description = 'Звучит по-вашему каждый день'
 
     def test_expected_values(self, generated_playlist, playlist):
         assert generated_playlist.type == self.type
         assert generated_playlist.ready == self.ready
         assert generated_playlist.notify == self.notify
         assert generated_playlist.data == playlist
         assert generated_playlist.description == self.description
+        assert generated_playlist.preview_description == self.preview_description
 
     def test_de_json_none(self, client):
         assert GeneratedPlaylist.de_json({}, client) is None
 
     def test_de_list_none(self, client):
         assert GeneratedPlaylist.de_list({}, client) == []
 
@@ -32,22 +34,24 @@
     def test_de_json_all(self, client, playlist):
         json_dict = {
             'type': self.type,
             'ready': self.ready,
             'notify': self.notify,
             'data': playlist.to_dict(),
             'description': self.description,
+            'preview_description': self.preview_description,
         }
         generated_playlist = GeneratedPlaylist.de_json(json_dict, client)
 
         assert generated_playlist.type == self.type
         assert generated_playlist.ready == self.ready
         assert generated_playlist.notify == self.notify
         assert generated_playlist.data == playlist
         assert generated_playlist.description == self.description
+        assert generated_playlist.preview_description == self.preview_description
 
     def test_equality(self, playlist):
         a = GeneratedPlaylist(self.type, self.ready, self.notify, playlist)
         b = GeneratedPlaylist(self.type, False, self.notify, None)
         c = GeneratedPlaylist(self.type, self.ready, self.notify, playlist)
 
         assert a != b
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yandex-music-2.0.1/tests/test_genre.py` & `yandex-music-2.1.0/tests/test_genre.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_icon.py` & `yandex-music-2.1.0/tests/test_icon.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_id.py` & `yandex-music-2.1.0/tests/test_id.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_images.py` & `yandex-music-2.1.0/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_invocation_info.py` & `yandex-music-2.1.0/tests/test_invocation_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_label.py` & `yandex-music-2.1.0/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_landing.py` & `yandex-music-2.1.0/tests/test_landing.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_landing_list.py` & `yandex-music-2.1.0/tests/test_landing_list.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_licence_text_part.py` & `yandex-music-2.1.0/tests/test_licence_text_part.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_like.py` & `yandex-music-2.1.0/tests/test_like.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_link.py` & `yandex-music-2.1.0/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_lyrics.py` & `yandex-music-2.1.0/tests/test_lyrics.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_made_for.py` & `yandex-music-2.1.0/tests/test_made_for.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_major.py` & `yandex-music-2.1.0/tests/test_major.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_meta_data.py` & `yandex-music-2.1.0/tests/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_mix_link.py` & `yandex-music-2.1.0/tests/test_mix_link.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,25 +33,23 @@
         json_dict = {
             'title': self.title,
             'url': self.url,
             'url_scheme': self.url_scheme,
             'text_color': self.text_color,
             'background_color': self.background_color,
             'background_image_uri': self.background_image_uri,
-            'cover_white': self.cover_white,
         }
         mix_link = MixLink.de_json(json_dict, client)
 
         assert mix_link.title == self.title
         assert mix_link.url == self.url
         assert mix_link.url_scheme == self.url_scheme
         assert mix_link.text_color == self.text_color
         assert mix_link.background_color == self.background_color
         assert mix_link.background_image_uri == self.background_image_uri
-        assert mix_link.cover_white == self.cover_white
 
     def test_de_json_all(self, client):
         json_dict = {
             'title': self.title,
             'url': self.url,
             'url_scheme': self.url_scheme,
             'text_color': self.text_color,
@@ -75,42 +73,38 @@
         a = MixLink(
             self.title,
             self.url,
             self.url_scheme,
             self.text_color,
             self.background_color,
             self.background_image_uri,
-            self.cover_white,
         )
         b = MixLink(
             self.title,
             self.url,
             '',
             self.text_color,
             self.background_color,
             self.background_image_uri,
-            self.cover_white,
         )
         c = MixLink(
             self.title,
             self.url,
             self.url_scheme,
             '#000000',
             self.background_color,
             self.background_image_uri,
-            self.cover_white,
         )
         d = MixLink(
             self.title,
             self.url,
             self.url_scheme,
             self.text_color,
             self.background_color,
             self.background_image_uri,
-            self.cover_white,
         )
 
         assert a != b != c
         assert hash(a) != hash(b) != hash(c)
         assert a is not b is not c
 
         assert a == d
```

### Comparing `yandex-music-2.0.1/tests/test_non_auto_renewable.py` & `yandex-music-2.1.0/tests/test_non_auto_renewable.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_normalization.py` & `yandex-music-2.1.0/tests/test_normalization.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_open_graph_data.py` & `yandex-music-2.1.0/tests/test_open_graph_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_operator.py` & `yandex-music-2.1.0/tests/test_operator.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_pager.py` & `yandex-music-2.1.0/tests/test_pager.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_passport_phone.py` & `yandex-music-2.1.0/tests/test_passport_phone.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_permission_alerts.py` & `yandex-music-2.1.0/tests/test_permission_alerts.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_permissions.py` & `yandex-music-2.1.0/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_personal_playlists_data.py` & `yandex-music-2.1.0/tests/test_personal_playlists_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_play_context.py` & `yandex-music-2.1.0/tests/test_play_context.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_play_contexts_data.py` & `yandex-music-2.1.0/tests/test_play_contexts_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_play_counter.py` & `yandex-music-2.1.0/tests/test_play_counter.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_playlist.py` & `yandex-music-2.1.0/tests/test_playlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
         playlist_absence,
         playlist_without_nested_playlists,
         artist,
         track_id,
         contest,
         open_graph_data,
         brand,
+        custom_wave,
+        pager,
     ):
         assert playlist.owner == user
         assert playlist.uid == self.uid
         assert playlist.kind == self.kind
         assert playlist.title == self.title
         assert playlist.track_count == self.track_count
         assert playlist.cover == cover
@@ -111,14 +113,16 @@
         assert playlist.description == self.description
         assert playlist.description_formatted == self.description_formatted
         assert playlist.playlist_uuid == self.playlist_uuid
         assert playlist.type == self.type
         assert playlist.ready == self.ready
         assert playlist.is_for_from == self.is_for_from
         assert playlist.regions == self.regions
+        assert playlist.custom_wave == custom_wave
+        assert playlist.pager == pager
 
     def test_de_json_none(self, client):
         assert Playlist.de_json({}, client) is None
 
     def test_de_list_none(self, client):
         assert Playlist.de_list({}, client) == []
 
@@ -149,14 +153,16 @@
         playlist_absence,
         playlist_without_nested_playlists,
         artist,
         track_id,
         contest,
         open_graph_data,
         brand,
+        custom_wave,
+        pager,
     ):
         json_dict = {
             'owner': user.to_dict(),
             'uid': self.uid,
             'kind': self.kind,
             'title': self.title,
             'track_count': self.track_count,
@@ -206,14 +212,16 @@
             'dummy_cover': cover.to_dict(),
             'dummy_rollover_cover': cover.to_dict(),
             'og_data': open_graph_data.to_dict(),
             'branding': brand.to_dict(),
             'playlist_uuid': self.playlist_uuid,
             'type': self.type,
             'ready': self.ready,
+            'custom_wave': custom_wave.to_dict(),
+            'pager': pager.to_dict(),
         }
         playlist = Playlist.de_json(json_dict, client)
 
         assert playlist.owner == user
         assert playlist.uid == self.uid
         assert playlist.kind == self.kind
         assert playlist.title == self.title
@@ -264,14 +272,16 @@
         assert playlist.description == self.description
         assert playlist.description_formatted == self.description_formatted
         assert playlist.playlist_uuid == self.playlist_uuid
         assert playlist.type == self.type
         assert playlist.ready == self.ready
         assert playlist.is_for_from == self.is_for_from
         assert playlist.regions == self.regions
+        assert playlist.custom_wave == custom_wave
+        assert playlist.pager == pager
 
     def test_equality(self, user, cover, made_for, play_counter, playlist_absence):
         a = Playlist(user, cover, made_for, play_counter, playlist_absence)
         b = Playlist(user, cover, made_for, play_counter, None)
         c = Playlist(user, None, made_for, play_counter, playlist_absence)
         d = Playlist(user, cover, made_for, play_counter, playlist_absence)
```

### Comparing `yandex-music-2.0.1/tests/test_playlist_absence.py` & `yandex-music-2.1.0/tests/test_playlist_absence.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_playlist_id.py` & `yandex-music-2.1.0/tests/test_playlist_id.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_playlist_recommendations.py` & `yandex-music-2.1.0/tests/test_playlist_recommendations.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_plus.py` & `yandex-music-2.1.0/tests/test_plus.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_poetry_lover_match.py` & `yandex-music-2.1.0/tests/test_poetry_lover_match.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_price.py` & `yandex-music-2.1.0/tests/test_price.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_product.py` & `yandex-music-2.1.0/tests/test_product.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_promo_code_status.py` & `yandex-music-2.1.0/tests/test_promo_code_status.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_promotion.py` & `yandex-music-2.1.0/tests/test_promotion.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_queue.py` & `yandex-music-2.1.0/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_queue_item.py` & `yandex-music-2.1.0/tests/test_queue_item.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_ratings.py` & `yandex-music-2.1.0/tests/test_ratings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_renewable_remainder.py` & `yandex-music-2.1.0/tests/test_renewable_remainder.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_restrictions.py` & `yandex-music-2.1.0/tests/test_restrictions.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_rotor_settings.py` & `yandex-music-2.1.0/tests/test_rotor_settings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_search.py` & `yandex-music-2.1.0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_search_result.py` & `yandex-music-2.1.0/tests/test_search_result.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_sequence.py` & `yandex-music-2.1.0/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_settings.py` & `yandex-music-2.1.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_shot.py` & `yandex-music-2.1.0/tests/test_shot.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_shot_data.py` & `yandex-music-2.1.0/tests/test_shot_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_shot_event.py` & `yandex-music-2.1.0/tests/test_shot_event.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_shot_type.py` & `yandex-music-2.1.0/tests/test_shot_type.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_station.py` & `yandex-music-2.1.0/tests/test_station.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_station_data.py` & `yandex-music-2.1.0/tests/test_station_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_station_result.py` & `yandex-music-2.1.0/tests/test_station_tracks_result.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,61 @@
-from yandex_music import StationResult
+import pytest
 
+from yandex_music import StationTracksResult
 
-class TestStationResult:
-    explanation = ''
-    prerolls = []
-
-    def test_expected_values(self, station_result, station, rotor_settings, ad_params):
-        assert station_result.station == station
-        assert station_result.settings == rotor_settings
-        assert station_result.settings2 == rotor_settings
-        assert station_result.ad_params == ad_params
-        assert station_result.explanation == self.explanation
-        assert station_result.prerolls == self.prerolls
 
-    def test_de_json_none(self, client):
-        assert StationResult.de_json({}, client) is None
+@pytest.fixture(scope='class')
+def station_tracks_result(id_, sequence):
+    return StationTracksResult(id_, [sequence], TestStationTracksResult.batch_id, TestStationTracksResult.pumpkin)
+
+
+class TestStationTracksResult:
+    batch_id = '1573227402825981-2727432063278102211'
+    pumpkin = False
 
-    def test_de_list_none(self, client):
-        assert StationResult.de_list({}, client) == []
+    def test_expected_values(self, station_tracks_result, id_, sequence):
+        assert station_tracks_result.id == id_
+        assert station_tracks_result.sequence == [sequence]
+        assert station_tracks_result.batch_id == self.batch_id
+        assert station_tracks_result.pumpkin == self.pumpkin
+
+    def test_de_json_none(self, client):
+        assert StationTracksResult.de_json({}, client) is None
 
-    def test_de_json_required(self, client, station, rotor_settings, ad_params):
+    def test_de_json_required(self, client, id_, sequence):
         json_dict = {
-            'station': station.to_dict(),
-            'settings': rotor_settings.to_dict(),
-            'settings2': rotor_settings.to_dict(),
-            'ad_params': ad_params.to_dict(),
+            'id': id_.to_dict(),
+            'sequence': [sequence.to_dict()],
+            'batch_id': self.batch_id,
+            'pumpkin': self.pumpkin,
         }
-        station_result = StationResult.de_json(json_dict, client)
+        station_tracks_result = StationTracksResult.de_json(json_dict, client)
 
-        assert station_result.station == station
-        assert station_result.settings == rotor_settings
-        assert station_result.settings2 == rotor_settings
-        assert station_result.ad_params == ad_params
+        assert station_tracks_result.id == id_
+        assert station_tracks_result.sequence == [sequence]
+        assert station_tracks_result.batch_id == self.batch_id
+        assert station_tracks_result.pumpkin == self.pumpkin
 
-    def test_de_json_all(self, client, station, rotor_settings, ad_params):
+    def test_de_json_all(self, client, id_, sequence):
         json_dict = {
-            'station': station.to_dict(),
-            'settings': rotor_settings.to_dict(),
-            'settings2': rotor_settings.to_dict(),
-            'ad_params': ad_params.to_dict(),
-            'explanation': self.explanation,
-            'prerolls': self.prerolls,
+            'id': id_.to_dict(),
+            'sequence': [sequence.to_dict()],
+            'batch_id': self.batch_id,
+            'pumpkin': self.pumpkin,
         }
-        station_result = StationResult.de_json(json_dict, client)
+        station_tracks_result = StationTracksResult.de_json(json_dict, client)
 
-        assert station_result.station == station
-        assert station_result.settings == rotor_settings
-        assert station_result.settings2 == rotor_settings
-        assert station_result.ad_params == ad_params
-        assert station_result.explanation == self.explanation
-        assert station_result.prerolls == self.prerolls
-
-    def test_equality(self, station, rotor_settings, ad_params):
-        a = StationResult(station, rotor_settings, rotor_settings, ad_params)
-        b = StationResult(None, rotor_settings, rotor_settings, ad_params)
-        c = StationResult(station, None, rotor_settings, ad_params)
-        d = StationResult(station, rotor_settings, rotor_settings, ad_params)
-
-        assert a != b != c
-        assert hash(a) != hash(b) != hash(c)
-        assert a is not b is not c
+        assert station_tracks_result.id == id_
+        assert station_tracks_result.sequence == [sequence]
+        assert station_tracks_result.batch_id == self.batch_id
+        assert station_tracks_result.pumpkin == self.pumpkin
+
+    def test_equality(self, id_, sequence):
+        a = StationTracksResult(id_, sequence, self.batch_id, self.pumpkin)
+        b = StationTracksResult(id_, sequence, "", False)
+        c = StationTracksResult(id_, sequence, self.batch_id, self.pumpkin)
+
+        assert a != b
+        assert hash(a) != hash(b)
+        assert a is not b
 
-        assert a == d
+        assert a == c
```

### Comparing `yandex-music-2.0.1/tests/test_status.py` & `yandex-music-2.1.0/tests/test_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 
 class TestStatus:
     advertisement = 'Оформите постоянную подписку – первый месяц бесплатно!'
     cache_limit = 99
     subeditor = False
     subeditor_level = 0
-    default_email = 'Ilya@marshal.by'
+    default_email = 'yandex_music@yandex.com'
     skips_per_hour = None
     station_exists = None
     premium_region = None
     experiment = 109
+    pretrial_active = False
+    userhash = '2a1d970ce4dadc3333280aa8727d1c41a380a7622521ecef67928cd4213adb8f'
 
     def test_expected_values(self, status, account, permissions, subscription, plus, alert):
         assert status.account == account
         assert status.permissions == permissions
         assert status.subscription == subscription
         assert status.advertisement == self.advertisement
         assert status.cache_limit == self.cache_limit
@@ -23,14 +25,16 @@
         assert status.plus == plus
         assert status.default_email == self.default_email
         assert status.skips_per_hour == self.skips_per_hour
         assert status.station_exists == self.station_exists
         assert status.bar_below == alert
         assert status.premium_region == self.premium_region
         assert status.experiment == self.experiment
+        assert status.pretrial_active == self.pretrial_active
+        assert status.userhash == self.userhash
 
     def test_de_json_none(self, client):
         assert Status.de_json({}, client) is None
 
     def test_de_json_required(self, client, account, permissions):
         json_dict = {'account': account.to_dict(), 'permissions': permissions.to_dict()}
         status = Status.de_json(json_dict, client)
@@ -50,14 +54,16 @@
             'default_email': self.default_email,
             'skips_per_hour': self.skips_per_hour,
             'station_exists': self.station_exists,
             'premium_region': self.premium_region,
             'advertisement': self.advertisement,
             'bar_below': alert.to_dict(),
             'experiment': self.experiment,
+            'pretrial_active': self.pretrial_active,
+            'userhash': self.userhash,
         }
         status = Status.de_json(json_dict, client)
 
         assert status.account == account
         assert status.permissions == permissions
         assert status.subscription == subscription
         assert status.advertisement == self.advertisement
@@ -67,14 +73,16 @@
         assert status.plus == plus
         assert status.default_email == self.default_email
         assert status.skips_per_hour == self.skips_per_hour
         assert status.station_exists == self.station_exists
         assert status.bar_below == alert
         assert status.premium_region == self.premium_region
         assert status.experiment == self.experiment
+        assert status.pretrial_active == self.pretrial_active
+        assert status.userhash == self.userhash
 
     def test_equality(self, account, permissions, subscription):
         a = Status(account, permissions)
         b = Status(None, permissions)
         c = Status(account, permissions)
 
         assert a != b
```

### Comparing `yandex-music-2.0.1/tests/test_subscription.py` & `yandex-music-2.1.0/tests/test_subscription.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,68 @@
 from yandex_music import Subscription
 
 
 class TestSubscription:
     can_start_trial = False
     mcdonalds = False
     end = None
+    had_any_subscription = False
 
     def test_expected_values(self, subscription, renewable_remainder, auto_renewable, non_auto_renewable, operator):
         assert subscription.non_auto_renewable_remainder == renewable_remainder
         assert subscription.auto_renewable == [auto_renewable]
         assert subscription.family_auto_renewable == [auto_renewable]
         assert subscription.operator == [operator]
         assert subscription.non_auto_renewable == non_auto_renewable
         assert subscription.can_start_trial == self.can_start_trial
         assert subscription.mcdonalds == self.mcdonalds
         assert subscription.end == self.end
+        assert subscription.had_any_subscription == self.had_any_subscription
 
     def test_de_json_none(self, client):
         assert Subscription.de_json({}, client) is None
 
     def test_de_json_required(self, client, renewable_remainder, auto_renewable):
         json_dict = {
             'non_auto_renewable_remainder': renewable_remainder.to_dict(),
             'auto_renewable': [auto_renewable.to_dict()],
             'family_auto_renewable': [auto_renewable.to_dict()],
+            'had_any_subscription': self.had_any_subscription,
         }
         subscription = Subscription.de_json(json_dict, client)
 
         assert subscription.non_auto_renewable_remainder == renewable_remainder
         assert subscription.auto_renewable == [auto_renewable]
         assert subscription.family_auto_renewable == [auto_renewable]
+        assert subscription.had_any_subscription == self.had_any_subscription
 
     def test_de_json_all(self, client, renewable_remainder, auto_renewable, non_auto_renewable, operator):
         json_dict = {
             'auto_renewable': [auto_renewable.to_dict()],
             'can_start_trial': self.can_start_trial,
             'mcdonalds': self.mcdonalds,
             'end': self.end,
             'non_auto_renewable_remainder': renewable_remainder.to_dict(),
             'family_auto_renewable': [auto_renewable.to_dict()],
             'non_auto_renewable': non_auto_renewable.to_dict(),
             'operator': [operator.to_dict()],
+            'had_any_subscription': self.had_any_subscription,
         }
         subscription = Subscription.de_json(json_dict, client)
 
         assert subscription.non_auto_renewable_remainder == renewable_remainder
         assert subscription.auto_renewable == [auto_renewable]
         assert subscription.family_auto_renewable == [auto_renewable]
         assert subscription.operator == [operator]
         assert subscription.non_auto_renewable == non_auto_renewable
         assert subscription.can_start_trial == self.can_start_trial
         assert subscription.mcdonalds == self.mcdonalds
         assert subscription.end == self.end
+        assert subscription.had_any_subscription == self.had_any_subscription
 
     def test_equality(self, renewable_remainder, auto_renewable):
-        a = Subscription(renewable_remainder, [auto_renewable], [auto_renewable])
-        b = Subscription(renewable_remainder, [], [auto_renewable])
+        a = Subscription(renewable_remainder, [auto_renewable], [auto_renewable], self.had_any_subscription)
+        b = Subscription(renewable_remainder, [], [auto_renewable], self.had_any_subscription)
 
         assert a != b != auto_renewable
         assert hash(a) != hash(b) != hash(auto_renewable)
         assert a is not auto_renewable
```

### Comparing `yandex-music-2.0.1/tests/test_suggestions.py` & `yandex-music-2.1.0/tests/test_suggestions.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_supplement.py` & `yandex-music-2.1.0/tests/test_supplement.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_tag.py` & `yandex-music-2.1.0/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_tag_result.py` & `yandex-music-2.1.0/tests/test_tag_result.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_title.py` & `yandex-music-2.1.0/tests/test_title.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_track.py` & `yandex-music-2.1.0/tests/test_track.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,26 +32,31 @@
     short_description = (
         'По каким признакам во внешности, в поведении, в одежде можно понять, что девушка несвободна?'
         ' Чтобы не ошибиться со своими чувствами и устремлениями…» — такой замечательный вопрос'
         ' пришел мне от подписчика. Причин, которые могут остановить мужчин в момент появления'
         ' желания познакомиться с девушкой, достаточно много. Обычно они сводятся к опасениям,'
     )
     is_suitable_for_children = True
+    track_source = 'OWN'
+    available_for_options = ['bookmate']
+    track_sharing_flag = 'VIDEO_ALLOWED'
 
     def test_expected_values(
         self,
         track,
         artist,
         album,
         major,
         normalization,
         track_without_nested_tracks,
         user,
         meta_data,
         poetry_lover_match,
+        r_128,
+        lyrics_info,
     ):
         assert track.id == self.id
         assert track.title == self.title
         assert track.available == self.available
         assert track.available_for_premium_users == self.available_for_premium_users
         assert track.artists == [artist]
         assert track.albums == [album]
@@ -83,14 +88,19 @@
         assert track.state == self.state
         assert track.desired_visibility == self.desired_visibility
         assert track.filename == self.filename
         assert track.user_info == user
         assert track.background_video_uri == self.background_video_uri
         assert track.short_description == self.short_description
         assert track.is_suitable_for_children == self.is_suitable_for_children
+        assert track.track_source == self.track_source
+        assert track.available_for_options == self.available_for_options
+        assert track.r128 == r_128
+        assert track.lyrics_info == lyrics_info
+        assert track.track_sharing_flag == self.track_sharing_flag
 
     def test_de_json_none(self, client):
         assert Track.de_json({}, client) is None
 
     def test_de_list_none(self, client):
         assert Track.de_list({}, client) == []
 
@@ -107,14 +117,16 @@
         album,
         major,
         normalization,
         track_without_nested_tracks,
         user,
         meta_data,
         poetry_lover_match,
+        r_128,
+        lyrics_info,
     ):
         json_dict = {
             'id': self.id,
             'title': self.title,
             'available': self.available,
             'available_for_premium_users': self.available_for_premium_users,
             'artists': [artist.to_dict()],
@@ -147,14 +159,19 @@
             'filename': self.filename,
             'user_info': user.to_dict(),
             'meta_data': meta_data.to_dict(),
             'poetry_lover_matches': [poetry_lover_match.to_dict()],
             'background_video_uri': self.background_video_uri,
             'short_description': self.short_description,
             'is_suitable_for_children': self.is_suitable_for_children,
+            'track_source': self.track_source,
+            'available_for_options': self.available_for_options,
+            'r128': r_128.to_dict(),
+            'lyrics_info': lyrics_info.to_dict(),
+            'track_sharing_flag': self.track_sharing_flag,
         }
         track = Track.de_json(json_dict, client)
 
         assert track.id == self.id
         assert track.title == self.title
         assert track.available == self.available
         assert track.available_for_premium_users == self.available_for_premium_users
@@ -188,14 +205,19 @@
         assert track.state == self.state
         assert track.desired_visibility == self.desired_visibility
         assert track.filename == self.filename
         assert track.user_info == user
         assert track.background_video_uri == self.background_video_uri
         assert track.short_description == self.short_description
         assert track.is_suitable_for_children == self.is_suitable_for_children
+        assert track.track_source == self.track_source
+        assert track.available_for_options == self.available_for_options
+        assert track.r128 == r_128
+        assert track.lyrics_info == lyrics_info
+        assert track.track_sharing_flag == self.track_sharing_flag
 
     def test_equality(self):
         a = Track(self.id)
         b = Track(10)
         c = Track(self.id)
 
         assert a != b
```

### Comparing `yandex-music-2.0.1/tests/test_track_id.py` & `yandex-music-2.1.0/tests/test_track_id.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_track_position.py` & `yandex-music-2.1.0/tests/test_track_position.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_track_short.py` & `yandex-music-2.1.0/tests/test_track_short.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,32 +9,35 @@
         TestTrackShort.id,
         TestTrackShort.timestamp,
         TestTrackShort.album_id,
         TestTrackShort.play_count,
         TestTrackShort.recent,
         chart,
         track,
+        TestTrackShort.original_index,
     )
 
 
 class TestTrackShort:
     id = 21997388
     timestamp = '2019-11-07T03:00:00+00:00'
     album_id = None
     play_count = 0
     recent = False
+    original_index = 23
 
     def test_expected_values(self, track_short, track, chart):
         assert track_short.id == self.id
         assert track_short.timestamp == self.timestamp
         assert track_short.album_id == self.album_id
         assert track_short.play_count == self.play_count
         assert track_short.recent == self.recent
         assert track_short.track == track
         assert track_short.chart == chart
+        assert track_short.original_index == self.original_index
 
     def test_de_json_none(self, client):
         assert TrackShort.de_json({}, client) is None
 
     def test_de_list_none(self, client):
         assert TrackShort.de_list({}, client) == []
 
@@ -50,24 +53,26 @@
             'id': self.id,
             'timestamp': self.timestamp,
             'album_id': self.album_id,
             'play_count': self.play_count,
             'recent': self.recent,
             'track': track.to_dict(),
             'chart': chart.to_dict(),
+            'original_index': self.original_index,
         }
         track_short = TrackShort.de_json(json_dict, client)
 
         assert track_short.id == self.id
         assert track_short.timestamp == self.timestamp
         assert track_short.album_id == self.album_id
         assert track_short.play_count == self.play_count
         assert track_short.recent == self.recent
         assert track_short.track == track
         assert track_short.chart == chart
+        assert track_short.original_index == self.original_index
 
     def test_equality(self):
         a = TrackShort(self.id, self.timestamp, self.album_id)
         b = TrackShort(23, self.timestamp, self.album_id)
         c = TrackShort(self.id, self.timestamp)
 
         assert a != b
```

### Comparing `yandex-music-2.0.1/tests/test_track_short_old.py` & `yandex-music-2.1.0/tests/test_track_short_old.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_track_with_ads.py` & `yandex-music-2.1.0/tests/test_track_with_ads.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_tracks_list.py` & `yandex-music-2.1.0/tests/test_tracks_list.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_tracks_similar.py` & `yandex-music-2.1.0/tests/test_tracks_similar.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_user.py` & `yandex-music-2.1.0/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_user_settings.py` & `yandex-music-2.1.0/tests/test_user_settings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_value.py` & `yandex-music-2.1.0/tests/test_value.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_video.py` & `yandex-music-2.1.0/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_video_supplement.py` & `yandex-music-2.1.0/tests/test_video_supplement.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/tests/test_vinyl.py` & `yandex-music-2.1.0/tests/test_vinyl.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/__init__.py` & `yandex-music-2.1.0/yandex_music/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-__version__ = '2.0.1'
+__version__ = '2.1.0'
 __license__ = 'GNU Lesser General Public License v3 (LGPLv3)'
-__copyright__ = 'Copyright (C) 2019-2022 Il`ya (Marshal) <https://github.com/MarshalX>'
+__copyright__ = 'Copyright (C) 2019-2023 Ilya (Marshal) <https://github.com/MarshalX>'
 
 from .base import YandexMusicObject
 
 from .settings import Settings
 from .permission_alerts import PermissionAlerts
 from .experiments import Experiments
 
@@ -40,14 +40,15 @@
 from .artist.ratings import Ratings
 from .artist.vinyl import Vinyl
 
 from .playlist.case_forms import CaseForms
 from .playlist.made_for import MadeFor
 from .playlist.user import User
 from .playlist.contest import Contest
+from .playlist.custom_wave import CustomWave
 from .playlist.open_graph_data import OpenGraphData
 from .playlist.brand import Brand
 from .playlist.play_counter import PlayCounter
 from .playlist.playlist_id import PlaylistId
 from .playlist.tag import Tag
 from .playlist.tag_result import TagResult
 from .playlist.playlist_absence import PlaylistAbsence
@@ -58,19 +59,23 @@
 from .shot.shot_data import ShotData
 from .shot.shot import Shot
 from .shot.shot_event import ShotEvent
 
 from .tracks_list import TracksList
 from .track.major import Major
 from .track.licence_text_part import LicenceTextPart
+from .track.track_lyrics import TrackLyrics
+from .track.lyrics_major import LyricsMajor
 from .track.poetry_lover_match import PoetryLoverMatch
 from .track.meta_data import MetaData
 from .track.normalization import Normalization
 from .track.track import Track
 from .track.tracks_similar import SimilarTracks
+from .track.r128 import R128
+from .track.lyrics_info import LyricsInfo
 
 from .feed.generated_playlist import GeneratedPlaylist
 from .feed.album_event import AlbumEvent
 from .feed.artist_event import ArtistEvent
 from .feed.track_with_ads import TrackWithAds
 from .feed.day import Day
 from .feed.event import Event
@@ -256,8 +261,12 @@
     'Contest',
     'OpenGraphData',
     'Brand',
     'Context',
     'Queue',
     'QueueItem',
     'Deprecation',
+    'TrackLyrics',
+    'CustomWave',
+    'R128',
+    'LyricsInfo',
 ]
```

### Comparing `yandex-music-2.0.1/yandex_music/account/account.py` & `yandex-music-2.1.0/yandex_music/account/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         service_available (:obj:`bool`): Доступен ли сервис.
         hosted_user (:obj:`bool`, optional): Является ли пользователем чьим-то другим.
         birthday (:obj:`str`, optional): Дата рождения.
         region (:obj:`int`, optional): Регион.
         passport_phones (:obj:`list` из :obj:`yandex_music.PassportPhone`): Мобильные номера.
         registered_at (:obj:`str`, optional): Дата создания учётной записи.
         has_info_for_app_metrica (:obj:`bool`, optional): Наличие информации для App Metrica.
+        child (:obj:`bool`): Дочерний / детский аккаунт (скорее детский, позволяет ограничить доступный контент ребенку на Кинопоиске).
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
         **kwargs: Произвольные ключевые аргументы полученные от API.
     """
 
     now: str
     service_available: bool
     region: Optional[int] = None
@@ -39,15 +40,16 @@
     second_name: Optional[str] = None
     first_name: Optional[str] = None
     display_name: Optional[str] = None
     hosted_user: Optional[bool] = None
     birthday: Optional[str] = None
     passport_phones: List['PassportPhone'] = None
     registered_at: Optional[str] = None
-    has_info_for_app_metrica: bool = False
+    has_info_for_app_metrica: bool = None
+    child: bool = None
     client: Optional['Client'] = None
 
     def __post_init__(self):
         if self.uid:
             self._id_attrs = (self.uid,)
 
     @classmethod
```

### Comparing `yandex-music-2.0.1/yandex_music/account/alert.py` & `yandex-music-2.1.0/yandex_music/account/alert.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/account/alert_button.py` & `yandex-music-2.1.0/yandex_music/account/alert_button.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/account/auto_renewable.py` & `yandex-music-2.1.0/yandex_music/account/auto_renewable.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/account/deactivation.py` & `yandex-music-2.1.0/yandex_music/account/deactivation.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/account/non_auto_renewable.py` & `yandex-music-2.1.0/yandex_music/account/non_auto_renewable.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/account/operator.py` & `yandex-music-2.1.0/yandex_music/account/operator.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/account/passport_phone.py` & `yandex-music-2.1.0/yandex_music/account/passport_phone.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/account/permissions.py` & `yandex-music-2.1.0/yandex_music/account/permissions.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/account/plus.py` & `yandex-music-2.1.0/yandex_music/account/plus.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/account/price.py` & `yandex-music-2.1.0/yandex_music/account/price.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/account/product.py` & `yandex-music-2.1.0/yandex_music/account/product.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/account/renewable_remainder.py` & `yandex-music-2.1.0/yandex_music/account/renewable_remainder.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/account/status.py` & `yandex-music-2.1.0/yandex_music/account/status.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         default_email (:obj:`str`, optional): Основной e-mail адрес аккаунта.
         skips_per_hour (:obj:`int`, optional): Количество переключение треков на радио в час.
         station_exists (:obj:`bool`, optional): Наличие личной станции.
         station_data (:obj:`yandex_music.StationData`, optional): Информация о личной станции.
         bar_below (:obj:`yandex_music.Alert`, optional): Блок с предупреждениями о конце подписке и подарках.
         premium_region (:obj:`int`, optional): Регион TODO.
         experiment (:obj:`int`, optional): Включенная новая фича на аккаунте (её ID) TODO.
+        pretrial_active (:obj:`bool`, optional): TODO.
+        userhash (:obj:`str`, optional): Хэш-код идентификатора пользователя.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
     account: Optional['Account']
     permissions: Optional['Permissions']
     advertisement: Optional[str] = None
     subscription: Optional['Subscription'] = None
@@ -41,14 +43,16 @@
     default_email: Optional[str] = None
     skips_per_hour: Optional[int] = None
     station_exists: Optional[bool] = None
     station_data: Optional['StationData'] = None
     bar_below: Optional['Alert'] = None
     premium_region: Optional[int] = None
     experiment: Optional[int] = None
+    pretrial_active: Optional[bool] = None
+    userhash: Optional[str] = None
     client: Optional['Client'] = None
 
     def __post_init__(self):
         self._id_attrs = (self.account, self.permissions)
 
     @classmethod
     def de_json(cls, data: dict, client: 'Client') -> Optional['Status']:
```

### Comparing `yandex-music-2.0.1/yandex_music/account/subscription.py` & `yandex-music-2.1.0/yandex_music/account/subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,20 +16,22 @@
         auto_renewable (:obj:`list` из :obj:`yandex_music.AutoRenewable`, optional): Автопродление.
         family_auto_renewable (:obj:`list` из :obj:`yandex_music.AutoRenewable`): Автопродление семейной подписки.
         operator (:obj:`list` из :obj:`yandex_music.Operator`, optional): Услуги сотового оператора.
         non_auto_renewable (:obj:`yandex_music.NonAutoRenewable`, optional): Отключённое автопродление.
         can_start_trial (:obj:`bool`, optional): Есть ли возможность начать пробный период.
         mcdonalds (:obj:`bool`, optional): mcdonalds TODO.
         end (:obj:`str`, optional): Дата окончания.
+        had_any_subscription (:obj:'bool'): Наличие какой-либо подписки в прошлом.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
     non_auto_renewable_remainder: 'RenewableRemainder'
     auto_renewable: List['AutoRenewable']
     family_auto_renewable: List['AutoRenewable']
+    had_any_subscription: bool
     operator: List['Operator'] = None
     non_auto_renewable: Optional['NonAutoRenewable'] = None
     can_start_trial: Optional[bool] = None
     mcdonalds: Optional[bool] = None
     end: Optional[str] = None
     client: Optional['Client'] = None
```

### Comparing `yandex-music-2.0.1/yandex_music/account/user_settings.py` & `yandex-music-2.1.0/yandex_music/account/user_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """Класс, представляющий настройки пользователя.
 
     Note:
         Доступные значения для поля `theme`: `white`, `black`.
 
         Доступные значения для полей `user_music_visibility` и `user_social_visibility`: `private`, `public`.
 
-    Notes:
+    Note:
         `promos_disabled`, `ads_disabled`, `rbt_disabled` устарели и не работают.
 
         `last_fm_scrobbling_enabled`, `facebook_scrobbling_enabled` выглядят устаревшими.
 
     Attributes:
         uid (:obj:`int`): Уникальный идентификатор пользователя.
         last_fm_scrobbling_enabled (:obj:`bool`): Скробблинг lastfm.
```

### Comparing `yandex-music-2.0.1/yandex_music/album/album.py` & `yandex-music-2.1.0/yandex_music/artist/artist.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,272 +1,339 @@
 from typing import Any, TYPE_CHECKING, Optional, List, Union
 
 from yandex_music import YandexMusicObject
 from yandex_music.utils import model
 
 if TYPE_CHECKING:
-    from yandex_music import Client, Artist, Label, TrackPosition, Track, Deprecation
+    from yandex_music import Client, Cover, Ratings, Counts, Link, Track, Description, ArtistTracks, ArtistAlbums
 
 
 @model
-class Album(YandexMusicObject):
-    """Класс, представляющий альбом.
-
-    Note:
-        Известные типы альбома: `single` - сингл, `compilation` - сборник.
-
-        Известные предупреждения о содержимом: `explicit` - ненормативная лексика.
-
-        Известные ошибки: `not-found` - альбом с таким ID не существует.
-
-        Известные значения поля `meta_type`: `music`.
+class Artist(YandexMusicObject):
+    """Класс, представляющий исполнителя.
 
     Attributes:
-        id_(:obj:`int`, optional): Идентификатор альбома.
-        error (:obj:`str`, optional): Ошибка получения альбома.
-        title (:obj:`str`, optional): Название альбома.
-        track_count (:obj:`int`, optional): Количество треков.
-        artists (:obj:`list` из :obj:`yandex_music.Artist`, optional): Артисты.
-        labels (:obj:`list` из :obj:`yandex_music.Label` или :obj:`str`, optional): Лейблы.
-        available (:obj:`bool`, optional): Доступен ли альбом.
-        available_for_premium_users (:obj:`bool`, optional): Доступен ли альбом для пользователей с подпиской.
-        version (:obj:`str`, optional): Дополнительная информация об альбоме.
-        cover_uri (:obj:`str`, optional): Ссылка на обложку.
-        content_warning (:obj:`str`, optional): Предупреждение о содержимом альбома.
-        original_release_year: TODO.
-        genre (:obj:`str`, optional): Жанр музыки.
-        text_color (:obj:`str`, optional): Цвет текста описания.
-        short_description (:obj:`str`, optional): Короткое описание.
-        description (:obj:`str`, optional): Описание.
-        is_premiere (:obj:`bool`, optional): Премьера ли.
-        is_banner (:obj:`bool`, optional): Является ли баннером.
-        meta_type (:obj:`str`, optional): Мета тип TODO.
-        storage_dir (:obj:`str`, optional): В какой папке на сервере хранится файл TODO.
-        og_image (:obj:`str`, optional): Ссылка на превью Open Graph.
-        recent (:obj:`bool`, optional): Является ли альбом новым.
-        very_important (:obj:`bool`, optional): Популярен ли альбом у слушателей.
-        available_for_mobile (:obj:`bool`, optional): Доступен ли альбом из приложения для телефона.
-        available_partially (:obj:`bool`, optional): Доступен ли альбом частично для пользователей без подписки.
-        bests (:obj:`list` из :obj:`int`, optional): ID лучших треков альбома.
-        duplicates (:obj:`list` из :obj:`yandex_music.Album`, optional): Альбомы-дубликаты.
-        prerolls (:obj:`list`, optional): Прероллы TODO.
-        volumes (:obj:`list` из :obj:`list` из :obj:`Track`, optional): Треки альбома, разделённые по дискам.
-        year (:obj:`int`, optional): Год релиза.
-        release_date (:obj:`str`, optional): Дата релиза в формате ISO 8601.
-        type (:obj:`str`, optional): Тип альбома.
-        track_position (:obj:`yandex_music.TrackPosition`, optional): Позиция трека в альбоме. Возвращается при
-            получении альбома в составе трека.
-        regions (:obj:`list` из :obj:`str`, optional): Список регионов в которых доступен альбом.
-        available_as_rbt (:obj:`bool`, optional): TODO.
-        lyrics_available (:obj:`bool`, optional): Доступны ли слова TODO.
-        remember_position (:obj:`bool`, optional): Запоминание позиции TODO.
-        albums (:obj:`list` из :obj:`yandex_music.Album`, optional): Альбомы TODO.
-        duration_ms (:obj:`int`, optional): Длительность в миллисекундах.
-        explicit (:obj:`bool`, optional): Есть ли в треке ненормативная лексика.
-        start_date (:obj:`str`, optional): Дата начала в формате ISO 8601 TODO.
-        likes_count (:obj:`int`, optional): Количество лайков TODO.
-        deprecation (:obj:`yandex_music.Deprecation`, optional): TODO.
-        available_regions (:obj:`list` из :obj:`str`, optional): Регионы, где доступн альбом.
-        client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
+        id (:obj:`int`): Уникальный идентификатор.
+        error (:obj:`str`, optional): Сообщение об ошибке с объяснением почему не вернуло исполнителя.
+        reason (:obj:`str`, optional): Причина отсутствия исполнителя (сообщение об ошибке).
+        name (:obj:`str`, optional): Название.
+        cover (:obj:`yandex_music.Cover`, optional): Обложка.
+        various (:obj:`bool`, optional): TODO.
+        composer (:obj:`bool`, optional): TODO.
+        genres (:obj:`list` из :obj:`str`, optional): Жанры.
+        og_image (:obj:`str`, optional): Ссылка на изображение для Open Graph.
+        op_image (:obj:`str`, optional): Ссылка на изображение обложки. Используется когда не указано поле cover.
+        no_pictures_from_search: TODO.
+        counts (:obj:`yandex_music.Counts`, optional): Счётчики.
+        available (:obj:`bool`, optional): Доступен ли для прослушивания.
+        ratings (:obj:`yandex_music.Ratings`, optional): Рейтинги.
+        links (:obj:`list` из :obj:`yandex_music.Link`, optional): Ссылки на ресурсы исполнителя.
+        tickets_available (:obj:`bool`, optional): Имеются ли в продаже билеты на концерт.
+        likes_count (:obj:`int`, optional): Количество лайков.
+        popular_tracks (:obj:`list` из :obj:`yandex_music.Track`, optional): Популярные треки.
+        regions (:obj:`list` из :obj:`str`, optional): Регион TODO.
+        decomposed (:obj:`list` из :obj:`str` и :obj:`yandex_music.Artist`, optional): Декомпозиция всех исполнителей.
+            Лист, где чередуется разделитель и артист. Фиты и прочее.
+        full_names: TODO.
+        hand_made_description (:obj:`str`, optional): Описание от Яндекс TODO.
+        description (:obj:`yandex_music.Description`, optional): Описание.
+        countries (:obj:`list` из :obj:`str`, optional): Страны.
+        en_wikipedia_link (:obj:`str`, optional): Адрес страницы на wikipedia.org.
+        db_aliases (:obj:`list` из :obj:`str`, optional): Другие названия. Как правило названия на разных языках.
+        aliases: TODO.
+        init_date (:obj:`str`, optional): Дата начала в формате YYYY-MM-DD или YYYY.
+        end_date (:obj:`str`, optional): Дата окончания в формате YYYY-MM-DD или YYYY.
+        ya_money_id (:obj:`str`): Номер кошеляка Яндекс.Деньги TODO.
+        client (:obj:`yandex_music.Client`): Клиент Yandex Music.
     """
 
-    id: Optional[int] = None
+    id: int
     error: Optional[str] = None
-    title: Optional[str] = None
-    track_count: Optional[int] = None
-    artists: List['Artist'] = None
-    labels: List[Union['Label', str]] = None
-    available: Optional[bool] = None
-    available_for_premium_users: Optional[bool] = None
-    version: Optional[str] = None
-    cover_uri: Optional[str] = None
-    content_warning: Optional[str] = None
-    original_release_year: Any = None
-    genre: Optional[str] = None
-    text_color: Optional[str] = None
-    short_description: Optional[str] = None
-    description: Optional[str] = None
-    is_premiere: Optional[bool] = None
-    is_banner: Optional[bool] = None
-    meta_type: Optional[str] = None
-    storage_dir: Optional[str] = None
+    reason: Optional[str] = None
+    name: Optional[str] = None
+    cover: Optional['Cover'] = None
+    various: Optional[bool] = None
+    composer: Optional[bool] = None
+    genres: Optional[List[str]] = None
     og_image: Optional[str] = None
-    buy: Optional[list] = None
-    recent: Optional[bool] = None
-    very_important: Optional[bool] = None
-    available_for_mobile: Optional[bool] = None
-    available_partially: Optional[bool] = None
-    bests: Optional[List[int]] = None
-    duplicates: List['Album'] = None
-    prerolls: Optional[list] = None
-    volumes: Optional[List[List['Track']]] = None
-    year: Optional[int] = None
-    release_date: Optional[str] = None
-    type: Optional[str] = None
-    track_position: Optional['TrackPosition'] = None
-    regions: Optional[List[str]] = None
-    available_as_rbt: Optional[bool] = None
-    lyrics_available: Optional[bool] = None
-    remember_position: Optional[bool] = None
-    albums: Optional[List['Album']] = None
-    duration_ms: Optional[int] = None
-    explicit: Optional[bool] = None
-    start_date: Optional[str] = None
+    op_image: Optional[str] = None
+    no_pictures_from_search: Any = None
+    counts: Optional['Counts'] = None
+    available: Optional[bool] = None
+    ratings: Optional['Ratings'] = None
+    links: Optional[List['Link']] = None
+    tickets_available: Optional[bool] = None
     likes_count: Optional[int] = None
-    deprecation: Optional['Deprecation'] = None
-    available_regions: Optional[List[str]] = None
-    client: Optional['Client'] = None
+    popular_tracks: Optional[List['Track']] = None
+    regions: Optional[List[str]] = None
+    decomposed: Optional[List[Union[str, 'Artist']]] = None
+    full_names: Any = None
+    hand_made_description: Optional[str] = None
+    description: Optional['Description'] = None
+    countries: Optional[List[str]] = None
+    en_wikipedia_link: Optional[str] = None
+    db_aliases: Optional[List[str]] = None
+    aliases: Any = None
+    init_date: Optional[str] = None
+    end_date: Optional[str] = None
+    ya_money_id: Optional[str] = None
+    client: 'Client' = None
 
     def __post_init__(self):
-        self._id_attrs = (self.id,)
+        self._id_attrs = (self.id, self.name, self.cover)
 
-    def with_tracks(self, *args, **kwargs) -> Optional['Album']:
-        """Сокращение для::
+    def get_op_image_url(self, size: str = '200x200') -> str:
+        """Возвращает URL OP обложки.
 
-        client.albums_with_tracks(album.id, *args, **kwargs)
+        Args:
+            size (:obj:`str`, optional): Размер обложки.
+
+        Returns:
+            :obj:`str`: URL обложки.
         """
-        return self.client.albums_with_tracks(self.id, *args, **kwargs)
+        return f'https://{self.op_image.replace("%%", size)}'
 
-    async def with_tracks_async(self, *args, **kwargs) -> Optional['Album']:
-        """Сокращение для::
+    def get_og_image_url(self, size: str = '200x200') -> str:
+        """Возвращает URL OG обложки.
+
+        Args:
+            size (:obj:`str`, optional): Размер обложки.
 
-        await client.albums_with_tracks(album.id, *args, **kwargs)
+        Returns:
+            :obj:`str`: URL обложки.
         """
-        return await self.client.albums_with_tracks(self.id, *args, **kwargs)
+        return f'https://{self.og_image.replace("%%", size)}'
 
-    def download_cover(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка обложки.
+    def download_og_image(self, filename: str, size: str = '200x200') -> None:
+        """Загрузка изображения для Open Graph.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             size (:obj:`str`, optional): Размер обложки.
         """
-        self.client.request.download(f'https://{self.cover_uri.replace("%%", size)}', filename)
+        self.client.request.download(self.get_og_image_url(size), filename)
 
-    async def download_cover_async(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка обложки.
+    async def download_og_image_async(self, filename: str, size: str = '200x200') -> None:
+        """Загрузка изображения для Open Graph.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             size (:obj:`str`, optional): Размер обложки.
         """
-        await self.client.request.download(f'https://{self.cover_uri.replace("%%", size)}', filename)
+        await self.client.request.download(self.get_og_image_url(size), filename)
 
-    def download_og_image(self, filename: str, size: str = '200x200') -> None:
+    def download_op_image(self, filename: str, size: str = '200x200') -> None:
         """Загрузка обложки.
 
-        Предпочтительнее использовать `self.download_cover()`.
+        Notes:
+            Используйте это только когда нет self.cover!
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             size (:obj:`str`, optional): Размер обложки.
         """
-        self.client.request.download(f'https://{self.og_image.replace("%%", size)}', filename)
+        self.client.request.download(self.get_op_image_url(size), filename)
 
-    async def download_og_image_async(self, filename: str, size: str = '200x200') -> None:
+    async def download_op_image_async(self, filename: str, size: str = '200x200') -> None:
         """Загрузка обложки.
 
-        Предпочтительнее использовать `self.download_cover_async()`.
+        Notes:
+            Используйте это только когда нет self.cover!
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             size (:obj:`str`, optional): Размер обложки.
         """
-        await self.client.request.download(f'https://{self.og_image.replace("%%", size)}', filename)
+        await self.client.request.download(self.get_op_image_url(size), filename)
+
+    def download_og_image_bytes(self, size: str = '200x200') -> bytes:
+        """Загрузка изображения для Open Graph и возврат в виде байтов.
+
+        Args:
+            size (:obj:`str`, optional): Размер обложки.
+
+        Returns:
+            :obj:`bytes`: Изображение в виде байтов.
+        """
+        return self.client.request.retrieve(self.get_og_image_url(size))
+
+    async def download_og_image_bytes_async(self, size: str = '200x200') -> bytes:
+        """Загрузка изображения для Open Graph и возврат в виде байтов.
+
+        Args:
+            size (:obj:`str`, optional): Размер обложки.
+
+        Returns:
+            :obj:`bytes`: Изображение в виде байтов.
+        """
+        return await self.client.request.retrieve(self.get_og_image_url(size))
+
+    def download_op_image_bytes(self, size: str = '200x200') -> bytes:
+        """Загрузка обложки и возврат в виде байтов.
+
+        Notes:
+            Используйте это только когда нет self.cover!
+
+        Args:
+            size (:obj:`str`, optional): Размер обложки.
+
+        Returns:
+            :obj:`bytes`: Обложка в виде байтов.
+        """
+        return self.client.request.retrieve(self.get_op_image_url(size))
+
+    async def download_op_image_bytes_async(self, size: str = '200x200') -> bytes:
+        """Загрузка обложки и возврат в виде байтов.
+
+        Notes:
+            Используйте это только когда нет self.cover!
+
+        Args:
+            size (:obj:`str`, optional): Размер обложки.
+
+        Returns:
+            :obj:`bytes`: Обложка в виде байтов.
+        """
+        return await self.client.request.retrieve(self.get_op_image_url(size))
 
     def like(self, *args, **kwargs) -> bool:
         """Сокращение для::
 
-        client.users_likes_albums_add(album.id, user.id *args, **kwargs)
+        client.users_likes_artists_add(artist.id, user.id *args, **kwargs)
         """
-        return self.client.users_likes_albums_add(self.id, self.client.me.account.uid, *args, **kwargs)
+        return self.client.users_likes_artists_add(self.id, self.client.me.account.uid, *args, **kwargs)
 
     async def like_async(self, *args, **kwargs) -> bool:
         """Сокращение для::
 
-        await client.users_likes_albums_add(album.id, user.id *args, **kwargs)
+        await client.users_likes_artists_add(artist.id, user.id *args, **kwargs)
         """
-        return await self.client.users_likes_albums_add(self.id, self.client.me.account.uid, *args, **kwargs)
+        return await self.client.users_likes_artists_add(self.id, self.client.me.account.uid, *args, **kwargs)
 
     def dislike(self, *args, **kwargs) -> bool:
         """Сокращение для::
 
-        client.users_likes_albums_remove(album.id, user.id *args, **kwargs)
+        client.users_likes_artists_remove(artist.id, user.id *args, **kwargs)
         """
-        return self.client.users_likes_albums_remove(self.id, self.client.me.account.uid, *args, **kwargs)
+        return self.client.users_likes_artists_remove(self.id, self.client.me.account.uid, *args, **kwargs)
 
     async def dislike_async(self, *args, **kwargs) -> bool:
         """Сокращение для::
 
-        await client.users_likes_albums_remove(album.id, user.id *args, **kwargs)
+        await client.users_likes_artists_remove(artist.id, user.id *args, **kwargs)
         """
-        return await self.client.users_likes_albums_remove(self.id, self.client.me.account.uid, *args, **kwargs)
+        return await self.client.users_likes_artists_remove(self.id, self.client.me.account.uid, *args, **kwargs)
 
-    def artists_name(self) -> List[str]:
-        """Получает имена всех исполнителей.
+    def get_tracks(self, page=0, page_size=20, *args, **kwargs) -> Optional['ArtistTracks']:
+        """Сокращение для::
 
-        Returns:
-              :obj:`list` из :obj:`str`: Имена исполнителей.
+        client.artists_tracks(artist.id, page, page_size, *args, **kwargs)
         """
+        return self.client.artists_tracks(self.id, page, page_size, *args, **kwargs)
 
-        return [i.name for i in self.artists]
+    async def get_tracks_async(self, page=0, page_size=20, *args, **kwargs) -> Optional['ArtistTracks']:
+        """Сокращение для::
+
+        await client.artists_tracks(artist.id, page, page_size, *args, **kwargs)
+        """
+        return await self.client.artists_tracks(self.id, page, page_size, *args, **kwargs)
+
+    def get_albums(self, page=0, page_size=20, sort_by='year', *args, **kwargs) -> Optional['ArtistAlbums']:
+        """Сокращение для::
+
+        client.artists_direct_albums(artist.id, page, page_size, sort_by, *args, **kwargs)
+        """
+        return self.client.artists_direct_albums(self.id, page, page_size, sort_by, *args, **kwargs)
+
+    async def get_albums_async(self, page=0, page_size=20, sort_by='year', *args, **kwargs) -> Optional['ArtistAlbums']:
+        """Сокращение для::
+
+        await client.artists_direct_albums(artist.id, page, page_size, sort_by, *args, **kwargs)
+        """
+        return await self.client.artists_direct_albums(self.id, page, page_size, sort_by, *args, **kwargs)
 
     @classmethod
-    def de_json(cls, data: dict, client: 'Client') -> Optional['Album']:
+    def de_json(cls, data: dict, client: 'Client') -> Optional['Artist']:
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
-            client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
+            client (:obj:`yandex_music.Client`): Клиент Yandex Music.
 
         Returns:
-            :obj:`yandex_music.Album`: Альбом.
+            :obj:`yandex_music.Artist`: Исполнитель.
         """
         if not data:
             return None
 
-        data = super(Album, cls).de_json(data, client)
-        from yandex_music import Artist, Label, TrackPosition, Track, Deprecation
+        data = super(Artist, cls).de_json(data, client)
+        from yandex_music import Cover, Ratings, Counts, Link, Track, Description
 
-        data['artists'] = Artist.de_list(data.get('artists'), client)
-        data['labels'] = Label.de_list(data.get('labels'), client)
-        data['track_position'] = TrackPosition.de_json(data.get('track_position'), client)
-        data['duplicates'] = Album.de_list(data.get('duplicates'), client)
-        data['albums'] = Album.de_list(data.get('albums'), client)
-        data['deprecation'] = Deprecation.de_json(data.get('deprecation'), client)
-        if data.get('volumes'):
-            data['volumes'] = [Track.de_list(i, client) for i in data['volumes']]
+        data['cover'] = Cover.de_json(data.get('cover'), client)
+        data['ratings'] = Ratings.de_json(data.get('ratings'), client)
+        data['counts'] = Counts.de_json(data.get('counts'), client)
+        data['links'] = Link.de_list(data.get('links'), client)
+        data['popular_tracks'] = Track.de_list(data.get('popular_tracks'), client)
+        data['description'] = Description.de_json(data.get('description'), client)
+
+        # Мне очень интересно увидеть как в яндухе на клиентах солвят свой бэковский костыль, пригласите на экскурсию
+        if data.get('decomposed'):
+            data['decomposed'] = [
+                Artist.de_json(part, client) if isinstance(part, dict) else part for part in data['decomposed']
+            ]
 
         return cls(client=client, **data)
 
     @classmethod
-    def de_list(cls, data: dict, client: 'Client') -> List['Album']:
+    def de_list(cls, data: dict, client: 'Client') -> List['Artist']:
         """Десериализация списка объектов.
 
         Args:
             data (:obj:`list`): Список словарей с полями и значениями десериализуемого объекта.
-            client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
+            client (:obj:`yandex_music.Client`): Клиент Yandex Music.
 
         Returns:
-            :obj:`list` из :obj:`yandex_music.Album`: Альбомы.
+            :obj:`list` из :obj:`yandex_music.Artist`: Исполнители.
         """
         if not data:
             return []
 
-        return [cls.de_json(album, client) for album in data]
+        artists = list()
+        for artist in data:
+            artists.append(cls.de_json(artist, client))
+
+        return artists
 
     # camelCase псевдонимы
 
-    #: Псевдоним для :attr:`with_tracks`
-    withTracks = with_tracks
-    #: Псевдоним для :attr:`with_tracks_async`
-    withTracksAsync = with_tracks_async
-    #: Псевдоним для :attr:`download_cover`
-    downloadCover = download_cover
-    #: Псевдоним для :attr:`download_cover_async`
-    downloadCoverAsync = download_cover_async
+    #: Псевдоним для :attr:`get_op_image_url`
+    getOpImageUrl = get_op_image_url
+    #: Псевдоним для :attr:`get_og_image_url`
+    getOgImageUrl = get_og_image_url
     #: Псевдоним для :attr:`download_og_image`
     downloadOgImage = download_og_image
     #: Псевдоним для :attr:`download_og_image_async`
     downloadOgImageAsync = download_og_image_async
-    #: Псевдоним для :attr:`artists_name`
-    artistsName = artists_name
+    #: Псевдоним для :attr:`download_op_image`
+    downloadOpImage = download_op_image
+    #: Псевдоним для :attr:`download_op_image_async`
+    downloadOpImageAsync = download_op_image_async
+    #: Псевдоним для :attr:`download_og_image_bytes`
+    downloadOgImageBytes = download_og_image_bytes
+    #: Псевдоним для :attr:`download_og_image_bytes_async`
+    downloadOgImageBytesAsync = download_og_image_bytes_async
+    #: Псевдоним для :attr:`download_op_image_bytes`
+    downloadOpImageBytes = download_op_image_bytes
+    #: Псевдоним для :attr:`download_op_image_bytes_async`
+    downloadOpImageBytesAsync = download_op_image_bytes_async
+    #: Псевдоним для :attr:`like_async`
+    likeAsync = like_async
+    #: Псевдоним для :attr:`dislike_async`
+    dislikeAsync = dislike_async
+    #: Псевдоним для :attr:`get_tracks`
+    getTracks = get_tracks
+    #: Псевдоним для :attr:`get_tracks_async`
+    getTracksAsync = get_tracks_async
+    #: Псевдоним для :attr:`get_albums`
+    getAlbums = get_albums
+    #: Псевдоним для :attr:`get_albums_async`
+    getAlbumsAsync = get_albums_async
```

### Comparing `yandex-music-2.0.1/yandex_music/album/deprecation.py` & `yandex-music-2.1.0/yandex_music/album/deprecation.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/album/label.py` & `yandex-music-2.1.0/yandex_music/album/label.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/album/track_position.py` & `yandex-music-2.1.0/yandex_music/album/track_position.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from yandex_music import Client
 
 
 @model
 class TrackPosition(YandexMusicObject):
     """Класс, представляющий позицию трека.
 
-    None:
+    Note:
         Позиция трека в альбоме, который возвращается при получении самого трека.
 
         Volume на фронте именуется как "Диск".
 
     Attributes:
         volume (:obj:`int`): Номер альбома.
         index (:obj:`int`): Порядковый номер трека.
```

### Comparing `yandex-music-2.0.1/yandex_music/artist/artist.py` & `yandex-music-2.1.0/yandex_music/utils/request_async.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,255 +1,336 @@
-from typing import Any, TYPE_CHECKING, Optional, List, Union
-
-from yandex_music import YandexMusicObject
-from yandex_music.utils import model
+####################################################################
+# THIS IS AUTO GENERATED COPY OF client.py. DON'T EDIT IN BY HANDS #
+####################################################################
+
+import re
+import logging
+import keyword
+
+from typing import TYPE_CHECKING, Optional, Union
+
+# Не используется ujson из-за отсутствия в нём object_hook'a
+# Отправка вообще application/x-www-form-urlencoded, а не JSON'a
+# https://github.com/psf/requests/blob/master/requests/models.py#L508
+import json
+
+import asyncio
+import aiohttp
+import aiofiles
+
+from yandex_music.utils.response import Response
+from yandex_music.exceptions import (
+    UnauthorizedError,
+    BadRequestError,
+    NetworkError,
+    YandexMusicError,
+    TimedOutError,
+    NotFoundError,
+)
 
 if TYPE_CHECKING:
-    from yandex_music import Client, Cover, Ratings, Counts, Link, Track, Description, ArtistTracks, ArtistAlbums
+    from yandex_music import Client
+
+
+USER_AGENT = 'Yandex-Music-API'
+HEADERS = {
+    'X-Yandex-Music-Client': 'YandexMusicAndroid/23020251',
+}
+DEFAULT_TIMEOUT = 5
+
+reserved_names = keyword.kwlist + ['client']
+
+logging.getLogger('urllib3').setLevel(logging.WARNING)
+
+default_timeout = object()
 
 
-@model
-class Artist(YandexMusicObject):
-    """Класс, представляющий исполнителя.
-
-    Attributes:
-        id (:obj:`int`): Уникальный идентификатор.
-        error (:obj:`str`, optional): Сообщение об ошибке с объяснением почему не вернуло исполнителя.
-        reason (:obj:`str`, optional): Причина отсутствия исполнителя (сообщение об ошибке).
-        name (:obj:`str`, optional): Название.
-        cover (:obj:`yandex_music.Cover`, optional): Обложка.
-        various (:obj:`bool`, optional): TODO.
-        composer (:obj:`bool`, optional): TODO.
-        genres (:obj:`list` из :obj:`str`, optional): Жанры.
-        og_image (:obj:`str`, optional): Ссылка на изображение для Open Graph.
-        op_image (:obj:`str`, optional): Ссылка на изображение обложки. Используется когда не указано поле cover.
-        no_pictures_from_search: TODO.
-        counts (:obj:`yandex_music.Counts`, optional): Счётчики.
-        available (:obj:`bool`, optional): Доступен ли для прослушивания.
-        ratings (:obj:`yandex_music.Ratings`, optional): Рейтинги.
-        links (:obj:`list` из :obj:`yandex_music.Link`, optional): Ссылки на ресурсы исполнителя.
-        tickets_available (:obj:`bool`, optional): Имеются ли в продаже билеты на концерт.
-        likes_count (:obj:`int`, optional): Количество лайков.
-        popular_tracks (:obj:`list` :obj:`yandex_music.Track`, optional): Популярные треки.
-        regions (:obj:`list` из :obj:`str`, optional): Регион TODO.
-        decomposed (:obj:`list` из :obj:`str` и :obj:`yandex_music.Artist`, optional): Декомпозиция всех исполнителей.
-            Лист, где чередуется разделитель и артист. Фиты и прочее.
-        full_names: TODO.
-        hand_made_description (:obj:`str`, optional): Описание от Яндекс TODO.
-        description (:obj:`yandex_music.Description`, optional): Описание.
-        countries (:obj:`list` из :obj:`str`, optional): Страны.
-        en_wikipedia_link (:obj:`str`, optional): Адрес страницы на wikipedia.org.
-        db_aliases (:obj:`list` из :obj:`str`, optional): Другие названия. Как правило названия на разных языках.
-        aliases: TODO.
-        init_date (:obj:`str`, optional): Дата начала в формате YYYY-MM-DD или YYYY.
-        end_date (:obj:`str`, optional): Дата окончания в формате YYYY-MM-DD или YYYY.
-        ya_money_id (:obj:`str`): Номер кошеляка Яндекс.Деньги TODO.
-        client (:obj:`yandex_music.Client`): Клиент Yandex Music.
+class Request:
+    """Вспомогательный класс для yandex_music, представляющий методы для выполнения POST и GET запросов, скачивания
+    файлов.
+
+    Args:
+        client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
+        headers (:obj:`dict`, optional): Заголовки передаваемые с каждым запросом.
+        proxy_url (:obj:`str`, optional): Прокси.
     """
 
-    id: int
-    error: Optional[str] = None
-    reason: Optional[str] = None
-    name: Optional[str] = None
-    cover: Optional['Cover'] = None
-    various: Optional[bool] = None
-    composer: Optional[bool] = None
-    genres: Optional[List[str]] = None
-    og_image: Optional[str] = None
-    op_image: Optional[str] = None
-    no_pictures_from_search: Any = None
-    counts: Optional['Counts'] = None
-    available: Optional[bool] = None
-    ratings: Optional['Ratings'] = None
-    links: Optional[List['Link']] = None
-    tickets_available: Optional[bool] = None
-    likes_count: Optional[int] = None
-    popular_tracks: Optional[List['Track']] = None
-    regions: Optional[List[str]] = None
-    decomposed: Optional[List[Union[str, 'Artist']]] = None
-    full_names: Any = None
-    hand_made_description: Optional[str] = None
-    description: Optional['Description'] = None
-    countries: Optional[List[str]] = None
-    en_wikipedia_link: Optional[str] = None
-    db_aliases: Optional[List[str]] = None
-    aliases: Any = None
-    init_date: Optional[str] = None
-    end_date: Optional[str] = None
-    ya_money_id: Optional[str] = None
-    client: 'Client' = None
+    def __init__(self, client=None, headers=None, proxy_url=None, timeout=default_timeout):
+        self.headers = headers or HEADERS.copy()
+
+        self._timeout = DEFAULT_TIMEOUT
+        self.set_timeout(timeout)
+
+        self.client = self.set_and_return_client(client)
 
-    def __post_init__(self):
-        self._id_attrs = (self.id, self.name, self.cover)
+        # aiohttp
+        self.proxy_url = proxy_url
 
-    def download_og_image(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка изображения для Open Graph.
+        # requests
+        self.proxies = {'http': proxy_url, 'https': proxy_url} if proxy_url else None
+
+    def set_language(self, lang: str) -> None:
+        """Добавляет заголовок языка для каждого запроса.
+
+        Note:
+            Возможные значения `lang`: en/uz/uk/us/ru/kk/hy.
 
         Args:
-            filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-            size (:obj:`str`, optional): Размер обложки.
+            lang (:obj:`str`): Язык.
         """
-        self.client.request.download(f'https://{self.og_image.replace("%%", size)}', filename)
+        self.headers.update({'Accept-Language': lang})
 
-    async def download_og_image_async(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка изображения для Open Graph.
+    def set_timeout(self, timeout: Union[int, float, object] = default_timeout):
+        """Устанавливает время ожидания для всех запросов.
 
         Args:
-            filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-            size (:obj:`str`, optional): Размер обложки.
+            timeout (:obj:`int` | :obj:`float`): Время ожидания от сервера.
         """
-        await self.client.request.download(f'https://{self.og_image.replace("%%", size)}', filename)
+        self._timeout = timeout
+        if timeout is default_timeout:
+            self._timeout = DEFAULT_TIMEOUT
 
-    def download_op_image(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка обложки.
+    def set_authorization(self, token: str) -> None:
+        """Добавляет заголовок авторизации для каждого запроса.
 
-        Notes:
-            Используйте это только когда нет self.cover!
+        Note:
+            Используется при передаче своего экземпляра Request'a клиенту.
 
         Args:
-            filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-            size (:obj:`str`, optional): Размер обложки.
+            token (:obj:`str`): OAuth токен.
         """
-        self.client.request.download(f'https://{self.op_image.replace("%%", size)}', filename)
-
-    async def download_op_image_async(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка обложки.
+        self.headers.update({'Authorization': f'OAuth {token}'})
 
-        Notes:
-            Используйте это только когда нет self.cover!
+    def set_and_return_client(self, client) -> 'Client':
+        """Принимает клиент и присваивает его текущему объекту. При наличии авторизации добавляет заголовок.
 
         Args:
-            filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-            size (:obj:`str`, optional): Размер обложки.
+            client (:obj:`yandex_music.Client`): Клиент Yandex Music.
+
+        Returns:
+            :obj:`yandex_music.Client`: Клиент Yandex Music.
         """
-        await self.client.request.download(f'https://{self.op_image.replace("%%", size)}', filename)
+        self.client = client
 
-    def like(self, *args, **kwargs) -> bool:
-        """Сокращение для::
+        if self.client and self.client.token:
+            self.set_authorization(self.client.token)
 
-        client.users_likes_artists_add(artist.id, user.id *args, **kwargs)
-        """
-        return self.client.users_likes_artists_add(self.id, self.client.me.account.uid, *args, **kwargs)
+        return self.client
+
+    @staticmethod
+    def _convert_camel_to_snake(text: str) -> str:
+        """Конвертация CamelCase в SnakeCase.
 
-    async def like_async(self, *args, **kwargs) -> bool:
-        """Сокращение для::
+        Args:
+            text (:obj:`str`): Название переменной в CamelCase.
 
-        await client.users_likes_artists_add(artist.id, user.id *args, **kwargs)
+        Returns:
+            :obj:`str`: Название переменной в SnakeCase.
         """
-        return await self.client.users_likes_artists_add(self.id, self.client.me.account.uid, *args, **kwargs)
+        s = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', text)
+        return re.sub('([a-z0-9])([A-Z])', r'\1_\2', s).lower()
+
+    @staticmethod
+    def _object_hook(obj: dict) -> dict:
+        """Нормализация имён переменных пришедших с API.
+
+        Note:
+            В названии переменной заменяет "-" на "_", конвертирует в SnakeCase, если название является
+            зарезервированным словом или "client" - добавляет "_" в конец. Если название переменной начинается с цифры -
+            добавляет в начало "_".
 
-    def dislike(self, *args, **kwargs) -> bool:
-        """Сокращение для::
+        Args:
+            obj (:obj:`dict`): Словарь, где ключ название переменной, а значение - содержимое.
 
-        client.users_likes_artists_remove(artist.id, user.id *args, **kwargs)
+        Returns:
+            :obj:`dict`: Тот же словарь, что и на входе, но с нормализованными ключами.
         """
-        return self.client.users_likes_artists_remove(self.id, self.client.me.account.uid, *args, **kwargs)
+        cleaned_object = {}
+        for key, value in obj.items():
+            key = Request._convert_camel_to_snake(key.replace('-', '_'))
+            key = key.lower()
 
-    async def dislike_async(self, *args, **kwargs) -> bool:
-        """Сокращение для::
+            if key in reserved_names:
+                key += '_'
 
-        await client.users_likes_artists_remove(artist.id, user.id *args, **kwargs)
-        """
-        return await self.client.users_likes_artists_remove(self.id, self.client.me.account.uid, *args, **kwargs)
+            if len(key) and key[0].isdigit():
+                key = '_' + key
 
-    def get_tracks(self, page=0, page_size=20, *args, **kwargs) -> Optional['ArtistTracks']:
-        """Сокращение для::
+            cleaned_object.update({key: value})
 
-        client.artists_tracks(artist.id, page, page_size, *args, **kwargs)
-        """
-        return self.client.artists_tracks(self.id, page, page_size, *args, **kwargs)
+        return cleaned_object
 
-    async def get_tracks_async(self, page=0, page_size=20, *args, **kwargs) -> Optional['ArtistTracks']:
-        """Сокращение для::
+    def _parse(self, json_data: bytes) -> Optional[Response]:
+        """Разбор ответа от API.
 
-        await client.artists_tracks(artist.id, page, page_size, *args, **kwargs)
-        """
-        return await self.client.artists_tracks(self.id, page, page_size, *args, **kwargs)
+        Note:
+            Если данные отсутствуют в `result`, то переформировывает ответ используя данные из корня.
+
+        Args:
+            json_data (:obj:`bytes`): Ответ от API.
 
-    def get_albums(self, page=0, page_size=20, sort_by='year', *args, **kwargs) -> Optional['ArtistAlbums']:
-        """Сокращение для::
+        Returns:
+            :obj:`yandex_music.utils.response.Response`: Ответ API.
 
-        client.artists_direct_albums(artist.id, page, page_size, sort_by, *args, **kwargs)
+        Raises:
+            :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self.client.artists_direct_albums(self.id, page, page_size, sort_by, *args, **kwargs)
+        try:
+            decoded_s = json_data.decode('utf-8')
+            data = json.loads(decoded_s, object_hook=Request._object_hook)
 
-    async def get_albums_async(self, page=0, page_size=20, sort_by='year', *args, **kwargs) -> Optional['ArtistAlbums']:
-        """Сокращение для::
+        except UnicodeDecodeError:
+            logging.getLogger(__name__).debug('Logging raw invalid UTF-8 response:\n%r', json_data)
+            raise YandexMusicError('Server response could not be decoded using UTF-8')
+        except (AttributeError, ValueError):
+            raise YandexMusicError('Invalid server response')
 
-        await client.artists_direct_albums(artist.id, page, page_size, sort_by, *args, **kwargs)
-        """
-        return await self.client.artists_direct_albums(self.id, page, page_size, sort_by, *args, **kwargs)
+        if data.get('result') is None:
+            data = {'result': data, 'error': data.get('error'), 'error_description': data.get('error_description')}
+
+        return Response.de_json(data, self.client)
 
-    @classmethod
-    def de_json(cls, data: dict, client: 'Client') -> Optional['Artist']:
-        """Десериализация объекта.
+    async def _request_wrapper(self, *args, **kwargs):
+        """Обёртка над запросом библиотеки `aiohttp`.
+
+        Note:
+            Добавляет необходимые заголовки для запроса, обрабатывает статус коды, следит за таймаутом, кидает
+            необходимые исключения, возвращает ответ. Передаёт пользовательские аргументы в запрос.
 
         Args:
-            data (:obj:`dict`): Поля и значения десериализуемого объекта.
-            client (:obj:`yandex_music.Client`): Клиент Yandex Music.
+            *args: Произвольные аргументы для `aiohttp.request`.
+            **kwargs: Произвольные ключевые аргументы для `aiohttp.request`.
 
         Returns:
-            :obj:`yandex_music.Artist`: Исполнитель.
+            :obj:`bytes`: Тело ответа.
+
+        Raises:
+            :class:`yandex_music.exceptions.TimedOutError`: При превышении времени ожидания.
+            :class:`yandex_music.exceptions.UnauthorizedError`: При невалидном токене, долгом ожидании прямой ссылки на файл.
+            :class:`yandex_music.exceptions.BadRequestError`: При неправильном запросе.
+            :class:`yandex_music.exceptions.NetworkError`: При проблемах с сетью.
+        """
+        if 'headers' not in kwargs:
+            kwargs['headers'] = {}
+
+        kwargs['headers']['User-Agent'] = USER_AGENT
+
+        if kwargs['timeout'] is default_timeout:
+            kwargs['timeout'] = aiohttp.ClientTimeout(total=self._timeout)
+        else:
+            kwargs['timeout'] = aiohttp.ClientTimeout(total=kwargs['timeout'])
+
+        try:
+            async with aiohttp.request(*args, **kwargs) as _resp:
+                resp = _resp
+                content = await resp.content.read()
+        except asyncio.TimeoutError:
+            raise TimedOutError()
+        except aiohttp.ClientError as e:
+            raise NetworkError(e)
+
+        if 200 <= resp.status <= 299:
+            return content
+
+        try:
+            parse = self._parse(content)
+            message = parse.get_error()
+        except YandexMusicError:
+            message = 'Unknown HTTPError'
+
+        if resp.status in (401, 403):
+            raise UnauthorizedError(message)
+        elif resp.status == 400:
+            raise BadRequestError(message)
+        elif resp.status == 404:
+            raise NotFoundError(message)
+        elif resp.status in (409, 413):
+            raise NetworkError(message)
+
+        elif resp.status == 502:
+            raise NetworkError('Bad Gateway')
+        else:
+            raise NetworkError(f'{message} ({resp.status}): {content}')
+
+    async def get(
+        self, url: str, params: dict = None, timeout: Union[int, float] = default_timeout, *args, **kwargs
+    ) -> Union[dict, str]:
+        """Отправка GET запроса.
+
+        Args:
+            url (:obj:`str`): Адрес для запроса.
+            params (:obj:`str`): GET параметры для запроса.
+            timeout (:obj:`int` | :obj:`float`): Используется как время ожидания ответа от сервера вместо указанного
+                при создании пула.
+            *args: Произвольные аргументы для `aiohttp.request`.
+            **kwargs: Произвольные ключевые аргументы для `aiohttp.request`.
+
+        Returns:
+            :obj:`dict` | :obj:`str`: Обработанное тело ответа.
+
+        Raises:
+            :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        if not data:
-            return None
+        result = await self._request_wrapper(
+            'GET', url, params=params, headers=self.headers, proxy=self.proxy_url, timeout=timeout, *args, **kwargs
+        )
+
+        return self._parse(result).get_result()
 
-        data = super(Artist, cls).de_json(data, client)
-        from yandex_music import Cover, Ratings, Counts, Link, Track, Description
+    async def post(self, url, data=None, timeout=default_timeout, *args, **kwargs) -> Union[dict, str]:
+        """Отправка POST запроса.
 
-        data['cover'] = Cover.de_json(data.get('cover'), client)
-        data['ratings'] = Ratings.de_json(data.get('ratings'), client)
-        data['counts'] = Counts.de_json(data.get('counts'), client)
-        data['links'] = Link.de_list(data.get('links'), client)
-        data['popular_tracks'] = Track.de_list(data.get('popular_tracks'), client)
-        data['description'] = Description.de_json(data.get('description'), client)
+        Args:
+            url (:obj:`str`): Адрес для запроса.
+            data (:obj:`str`): POST тело запроса.
+            timeout (:obj:`int` | :obj:`float`): Используется как время ожидания ответа от сервера вместо указанного
+                при создании пула.
+            *args: Произвольные аргументы для `aiohttp.request`.
+            **kwargs: Произвольные ключевые аргументы для `aiohttp.request`.
 
-        # Мне очень интересно увидеть как в яндухе на клиентах солвят свой бэковский костыль, пригласите на экскурсию
-        if data.get('decomposed'):
-            data['decomposed'] = [
-                Artist.de_json(part, client) if isinstance(part, dict) else part for part in data['decomposed']
-            ]
+        Returns:
+            :obj:`dict` | :obj:`str`: Обработанное тело ответа.
 
-        return cls(client=client, **data)
+        Raises:
+            :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
+        """
+        result = await self._request_wrapper(
+            'POST', url, headers=self.headers, proxy=self.proxy_url, data=data, timeout=timeout, *args, **kwargs
+        )
 
-    @classmethod
-    def de_list(cls, data: dict, client: 'Client') -> List['Artist']:
-        """Десериализация списка объектов.
+        return self._parse(result).get_result()
+
+    async def retrieve(self, url, timeout=default_timeout, *args, **kwargs) -> bytes:
+        """Отправка GET запроса и получение содержимого без обработки (парсинга).
 
         Args:
-            data (:obj:`list`): Список словарей с полями и значениями десериализуемого объекта.
-            client (:obj:`yandex_music.Client`): Клиент Yandex Music.
+            url (:obj:`str`): Адрес для запроса.
+            timeout (:obj:`int` | :obj:`float`): Используется как время ожидания ответа от сервера вместо указанного
+                при создании пула.
+            *args: Произвольные аргументы для `aiohttp.request`.
+            **kwargs: Произвольные ключевые аргументы для `aiohttp.request`.
 
         Returns:
-            :obj:`list` из :obj:`yandex_music.Artist`: Исполнители.
+            :obj:`bytes`: Тело ответа.
+
+        Raises:
+            :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        if not data:
-            return []
+        return await self._request_wrapper('GET', url, proxy=self.proxy_url, timeout=timeout, *args, **kwargs)
 
-        artists = list()
-        for artist in data:
-            artists.append(cls.de_json(artist, client))
-
-        return artists
-
-    # camelCase псевдонимы
-
-    #: Псевдоним для :attr:`download_og_image`
-    downloadOgImage = download_og_image
-    #: Псевдоним для :attr:`download_og_image_async`
-    downloadOgImageAsync = download_og_image_async
-    #: Псевдоним для :attr:`download_op_image`
-    downloadOpImage = download_op_image
-    #: Псевдоним для :attr:`download_op_image_async`
-    downloadOpImageAsync = download_op_image_async
-    #: Псевдоним для :attr:`get_tracks`
-    getTracks = get_tracks
-    #: Псевдоним для :attr:`get_tracks_async`
-    getTracksAsync = get_tracks_async
-    #: Псевдоним для :attr:`get_albums`
-    getAlbums = get_albums
-    #: Псевдоним для :attr:`get_albums_async`
-    getAlbumsAsync = get_albums_async
-    #: Псевдоним для :attr:`like_async`
-    likeAsync = like_async
-    #: Псевдоним для :attr:`dislike_async`
-    dislikeAsync = dislike_async
+    async def download(self, url, filename, timeout=default_timeout, *args, **kwargs) -> None:
+        """Отправка запроса на получение содержимого и его запись в файл.
+
+        Args:
+            url (:obj:`str`): Адрес для запроса.
+            filename (:obj:`str`): Путь и(или) название файла вместе с расширением.
+            timeout (:obj:`int` | :obj:`float`): Используется как время ожидания ответа от сервера вместо указанного
+                при создании пула.
+            *args: Произвольные аргументы для `aiohttp.request`.
+            **kwargs: Произвольные ключевые аргументы для `aiohttp.request`.
+
+        Raises:
+            :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
+        """
+        result = await self.retrieve(url, timeout=timeout, *args, *kwargs)
+        async with aiofiles.open(filename, 'wb') as f:
+            await f.write(result)
```

### Comparing `yandex-music-2.0.1/yandex_music/artist/artist_albums.py` & `yandex-music-2.1.0/yandex_music/artist/artist_albums.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/artist/artist_tracks.py` & `yandex-music-2.1.0/yandex_music/artist/artist_tracks.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/artist/brief_info.py` & `yandex-music-2.1.0/yandex_music/artist/brief_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/artist/counts.py` & `yandex-music-2.1.0/yandex_music/artist/counts.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/artist/description.py` & `yandex-music-2.1.0/yandex_music/artist/description.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/artist/link.py` & `yandex-music-2.1.0/yandex_music/artist/link.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/artist/ratings.py` & `yandex-music-2.1.0/yandex_music/artist/ratings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/artist/vinyl.py` & `yandex-music-2.1.0/yandex_music/artist/vinyl.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/base.py` & `yandex-music-2.1.0/yandex_music/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,20 @@
     def __repr__(self) -> str:
         return str(self)
 
     def __getitem__(self, item):
         return self.__dict__[item]
 
     @staticmethod
-    def report_unknown_fields_callback(obj, unknown_fields):
+    def report_unknown_fields_callback(cls, unknown_fields):
         logger.warning(
             f'Found unknown fields received from API! Please copy warn message '
             f'and send to {new_issue_by_template_url} (github issue), thank you!'
         )
-        logger.warning(f'Type: {type(obj)}; fields: {unknown_fields}')
+        logger.warning(f'Type: {cls.__module__}.{cls.__name__}; fields: {unknown_fields}')
 
     @classmethod
     def de_json(cls, data: dict, client: Optional['Client']) -> Optional[dict]:
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
@@ -66,15 +66,15 @@
         for k, v in data.items():
             if k in fields:
                 cleaned_data[k] = v
             else:
                 unknown_data[k] = v
 
         if client.report_unknown_fields and unknown_data:
-            YandexMusicObject.report_unknown_fields_callback(cls, unknown_data)
+            cls.report_unknown_fields_callback(cls, unknown_data)
 
         return cleaned_data
 
     def to_json(self, for_request=False) -> str:
         """Сериализация объекта.
 
         Args:
```

### Comparing `yandex-music-2.0.1/yandex_music/client.py` & `yandex-music-2.1.0/yandex_music/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import functools
 import logging
 from datetime import datetime
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union, TypeVar, Callable, Any
 
 from yandex_music import (
     Album,
     Artist,
     ArtistAlbums,
     ArtistTracks,
     BriefInfo,
@@ -24,14 +24,15 @@
     ShotEvent,
     Supplement,
     StationResult,
     StationTracksResult,
     Status,
     Suggestions,
     SimilarTracks,
+    TrackLyrics,
     Track,
     TracksList,
     UserSettings,
     YandexMusicObject,
     ChartInfo,
     TagResult,
     PlaylistRecommendations,
@@ -41,30 +42,33 @@
     __copyright__,
     __license__,
     __version__,
 )
 from yandex_music.exceptions import BadRequestError
 from yandex_music.utils.difference import Difference
 from yandex_music.utils.request import Request
+from yandex_music.utils.sign_request import get_sign_request
 
 de_list = {
     'artist': Artist.de_list,
     'album': Album.de_list,
     'track': Track.de_list,
     'playlist': Playlist.de_list,
 }
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
+F = TypeVar('F', bound=Callable[..., Any])
 
-def log(method):
+
+def log(method: F) -> F:
     logger = logging.getLogger(method.__module__)
 
     @functools.wraps(method)
-    def wrapper(*args, **kwargs):
+    def wrapper(*args, **kwargs) -> Any:
         logger.debug(f'Entering: {method.__name__}')
 
         result = method(*args, **kwargs)
         logger.debug(result)
 
         logger.debug(f'Exiting: {method.__name__}')
 
@@ -91,33 +95,33 @@
             которых нет в библиотеке.
 
     Args:
         token (:obj:`str`, optional): Уникальный ключ для аутентификации.
         base_url (:obj:`str`, optional): Ссылка на API Yandex Music.
         request (:obj:`yandex_music.utils.request.Request`, optional): Пре-инициализация
             :class:`yandex_music.utils.request.Request`.
-        language (:obj:`str`, optional): Язык, на котором будут приходить ответы от API.
+        language (:obj:`str`, optional): Язык, на котором будут приходить ответы от API. По умолчанию русский.
         report_unknown_fields (:obj:`bool`, optional): Включить предупреждения о неизвестных полях от API,
             которых нет в библиотеке.
     """
 
-    notice_displayed = False
+    __notice_displayed = False
 
     def __init__(
         self,
         token: str = None,
         base_url: str = None,
         request: Request = None,
         language: str = 'ru',
         report_unknown_fields=False,
     ) -> None:
-        if not Client.notice_displayed:
+        if not Client.__notice_displayed:
             print(f'Yandex Music API v{__version__}, {__copyright__}')
             print(f'Licensed under the terms of the {__license__}', end='\n\n')
-            Client.notice_displayed = True
+            Client.__notice_displayed = True
 
         self.logger = logging.getLogger(__name__)
         self.token = token
 
         if base_url is None:
             base_url = 'https://api.music.yandex.net'
 
@@ -149,478 +153,485 @@
     @log
     def init(self):
         """Получение информацию об аккаунте использующихся в других запросах."""
         self.me = self.account_status()
         return self
 
     @log
-    def account_status(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Status]:
+    def account_status(self, *args, **kwargs) -> Optional[Status]:
         """Получение статуса аккаунта. Нет обязательных параметров.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Status` | :obj:`None`: Информация об аккаунте если он валиден, иначе :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/account/status'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return Status.de_json(result, self)
 
     @log
-    def account_settings(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[UserSettings]:
+    def account_settings(self, *args, **kwargs) -> Optional[UserSettings]:
         """Получение настроек текущего пользователя.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.UserSettings` | :obj:`None`: Настройки пользователя если аккаунт валиден,
                 иначе :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/account/settings'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return UserSettings.de_json(result, self)
 
     @log
     def account_settings_set(
         self,
         param: str = None,
         value: Union[str, int, bool] = None,
         data: Dict[str, Union[str, int, bool]] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[UserSettings]:
         """Изменение настроек текущего пользователя.
 
         Note:
             Доступные названия параметров есть поля в классе :class:`yandex_music.UserSettings`, только в CamelCase.
 
         Args:
             param (:obj:`str`): Название параметра для изменения.
             value (:obj:`str` | :obj:`int` | :obj:`bool`): Значение параметра.
             data (:obj:`dict`): Словарь параметров и значений для множественного изменения.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.UserSettings` | :obj:`None`: Настройки пользователя или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/account/settings'
 
         if not data:
             data = {param: str(value)}
 
-        # TODO (MarshalX) значения в data типа bool должны быть приведены к str при работе с async клиентом.
-
-        result = self._request.post(url, data=data, timeout=timeout, *args, **kwargs)
+        result = self._request.post(url, data, *args, **kwargs)
 
         return UserSettings.de_json(result, self)
 
     @log
-    def settings(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Settings]:
+    def settings(self, *args, **kwargs) -> Optional[Settings]:
         """Получение предложений по покупке. Нет обязательных параметров.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Settings` | :obj:`None`: Информацию о предлагаемых продуктах если аккаунт валиден
                 или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/settings'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return Settings.de_json(result, self)
 
     @log
-    def permission_alerts(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[PermissionAlerts]:
+    def permission_alerts(self, *args, **kwargs) -> Optional[PermissionAlerts]:
         """Получение оповещений. Нет обязательных параметров.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.PermissionAlerts` | :obj:`None`: Оповещения если аккаунт валиден или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/permission-alerts'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return PermissionAlerts.de_json(result, self)
 
     @log
-    def account_experiments(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Experiments]:
+    def account_experiments(self, *args, **kwargs) -> Optional[Experiments]:
         """Получение значений экспериментальных функций аккаунта.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Experiments` | :obj:`None`: Состояние экспериментальных функций или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/account/experiments'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return Experiments.de_json(result, self)
 
     @log
     def consume_promo_code(
-        self, code: str, language: str = 'en', timeout: Union[int, float] = None, *args, **kwargs
+        self, code: str, language: Optional[str] = None, *args, **kwargs
     ) -> Optional[PromoCodeStatus]:
         """Активация промо-кода.
 
+        Note:
+            Доступные языки: en, uz, uk, us, ru, kk, hy.
+
         Args:
             code (:obj:`str`): Промо-код.
-            language (:obj:`str`, optional): Язык ответа API в ISO 639-1.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
+            language (:obj:`str`, optional): Язык ответа API в ISO 639-1. По умолчанию язык клиента.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.PromoCodeStatus` | :obj:`None`: Информация об активации промо-кода или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/account/consume-promo-code'
 
-        result = self._request.post(url, {'code': code, 'language': language}, timeout=timeout, *args, **kwargs)
+        if not language:
+            language = self.language
+
+        result = self._request.post(url, {'code': code, 'language': language}, *args, **kwargs)
 
         return PromoCodeStatus.de_json(result, self)
 
     @log
-    def feed(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Feed]:
+    def feed(self, *args, **kwargs) -> Optional[Feed]:
         """Получение потока информации (фида) подобранного под пользователя. Содержит умные плейлисты.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Feed` | :obj:`None`: Умные плейлисты пользователя или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/feed'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return Feed.de_json(result, self)
 
     @log
-    def feed_wizard_is_passed(self, timeout: Union[int, float] = None, *args, **kwargs) -> bool:
+    def feed_wizard_is_passed(self, *args, **kwargs) -> bool:
         url = f'{self.base_url}/feed/wizard/is-passed'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return result.get('is_wizard_passed') or False
 
     @log
-    def landing(
-        self, blocks: Union[str, List[str]], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[Landing]:
+    def landing(self, blocks: Union[str, List[str]], *args, **kwargs) -> Optional[Landing]:
         """Получение лендинг-страницы содержащий блоки с новыми релизами, чартами, плейлистами с новинками и т.д.
 
         Note:
             Поддерживаемые типы блоков: `personalplaylists`, `promotions`, `new-releases`, `new-playlists`, `mixes`,
             `chart`, `artists`, `albums`, `playlists`, `play_contexts`.
 
         Args:
             blocks (:obj:`str` | :obj:`list` из :obj:`str`): Блок или список блоков необходимых для выдачи.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Landing` | :obj:`None`: Лендинг-страница или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/landing3'
 
-        result = self._request.get(
-            url, {'blocks': blocks, 'eitherUserId': '10254713668400548221'}, timeout=timeout, *args, **kwargs
-        )
+        result = self._request.get(url, {'blocks': blocks, 'eitherUserId': '10254713668400548221'}, *args, **kwargs)
+        # TODO (MarshalX) что тут делает константа с чьим-то User ID
+        #  https://github.com/MarshalX/yandex-music-api/issues/553
 
         return Landing.de_json(result, self)
 
     @log
-    def chart(self, chart_option: str = '', timeout: Union[int, float] = None, *args, **kwargs) -> Optional[ChartInfo]:
+    def chart(self, chart_option: str = '', *args, **kwargs) -> Optional[ChartInfo]:
         """Получение чарта.
 
         Note:
             `chart_option` - это постфикс к запросу из поля `menu` чарта.
             Например, на сайте можно выбрать глобальный (world) чарт или российский (russia).
 
         Args:
             chart_option (:obj:`str` optional): Параметры чарта.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.ChartInfo`: Чарт.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/landing3/chart'
 
         if chart_option:
             url = f'{url}/{chart_option}'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return ChartInfo.de_json(result, self)
 
     @log
-    def new_releases(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[LandingList]:
+    def new_releases(self, *args, **kwargs) -> Optional[LandingList]:
         """Получение полного списка всех новых релизов (альбомов).
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.LandingList`: Список новых альбомов.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/landing3/new-releases'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return LandingList.de_json(result, self)
 
     @log
-    def new_playlists(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[LandingList]:
+    def new_playlists(self, *args, **kwargs) -> Optional[LandingList]:
         """Получение полного списка всех новых плейлистов.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.LandingList`: Список новых плейлистов.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/landing3/new-playlists'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return LandingList.de_json(result, self)
 
     @log
-    def podcasts(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[LandingList]:
+    def podcasts(self, *args, **kwargs) -> Optional[LandingList]:
         """Получение подкастов с лендинга.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
-            :obj:`yandex_music.LandingList`: Список подскастов.
+            :obj:`yandex_music.LandingList`: Список подкастов.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/landing3/podcasts'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return LandingList.de_json(result, self)
 
     @log
-    def genres(self, timeout: Union[int, float] = None, *args, **kwargs) -> List[Genre]:
+    def genres(self, *args, **kwargs) -> List[Genre]:
         """Получение жанров музыки.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Genre` | :obj:`None`: Жанры музыки или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/genres'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return Genre.de_list(result, self)
 
     @log
-    def tags(self, tag_id: str, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[TagResult]:
+    def tags(self, tag_id: str, *args, **kwargs) -> Optional[TagResult]:
         """Получение тега (подборки).
 
         Note:
             Теги есть в `MixLink` у `Landing`, а также плейлистов в `.tags`.
 
             У `MixLink` есть `URL`, но `tag_id` только его последняя часть.
             Например, `/tag/belarus/`. `Tag` - `belarus`.
 
         Args:
             tag_id (:obj:`str`): Уникальный идентификатор тега.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
            :obj:`yandex_music.TagResult`: Тег с плейлистами.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/tags/{tag_id}/playlist-ids'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return TagResult.de_json(result, self)
 
     @log
     def tracks_download_info(
         self,
         track_id: Union[str, int],
         get_direct_links: bool = False,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> List[DownloadInfo]:
         """Получение информации о доступных вариантах загрузки трека.
 
         Args:
             track_id (:obj:`str` | :obj:`list` из :obj:`str`): Уникальный идентификатор трека или треков.
             get_direct_links (:obj:`bool`, optional): Получить ли при вызове метода прямую ссылку на загрузку.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.DownloadInfo` | :obj:`None`: Варианты загрузки трека или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/tracks/{track_id}/download-info'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return DownloadInfo.de_list(result, self, get_direct_links)
 
     @log
-    def track_supplement(
-        self, track_id: Union[str, int], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[Supplement]:
+    def track_supplement(self, track_id: Union[str, int], *args, **kwargs) -> Optional[Supplement]:
         """Получение дополнительной информации о треке.
 
+        Warning:
+            Получение текста из дополнительной информации устарело. Используйте
+            :func:`yandex_music.Client.tracks_lyrics`.
+
         Args:
-            track_id (:obj:`str`): Уникальный идентификатор трека.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
+            track_id (:obj:`str` | :obj:`int`): Уникальный идентификатор трека.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Supplement`: Дополнительная информация о треке.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/tracks/{track_id}/supplement'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return Supplement.de_json(result, self)
 
     @log
-    def tracks_similar(
-        self, track_id: Union[str, int], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[SimilarTracks]:
+    def tracks_lyrics(
+        self,
+        track_id: Union[str, int],
+        format: str = 'TEXT',
+        **kwargs,
+    ) -> Optional[TrackLyrics]:
+        """Получение текста трека.
+
+        Note:
+            Для работы с методом необходима авторизация.
+
+            Известные значения для аргумента format:
+                - `LRC` - формат с временными метками.
+                - `TEXT` - простой текст.
+
+        Args:
+            track_id (:obj:`str` | :obj:`int`): Уникальный идентификатор трека.
+            format (:obj:`str`): Формат текста.
+            **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
+
+        Returns:
+            :obj:`yandex_music.TrackLyrics` | :obj:`None`: Информация о тексте трека.
+
+        Raises:
+            :class:`yandex_music.exceptions.UnauthorizedError`: Метод вызван без авторизации.
+            :class:`yandex_music.exceptions.NotFoundError`: Текст у трека отсутствует.
+            :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
+        """
+
+        url = f'{self.base_url}/tracks/{track_id}/lyrics'
+
+        sign = get_sign_request(track_id)
+        params = {
+            'format': format,
+            'timeStamp': sign.timestamp,
+            'sign': sign.value,
+        }
+
+        result = self._request.get(url, params=params, **kwargs)
+
+        return TrackLyrics.de_json(result, self)
+
+    @log
+    def tracks_similar(self, track_id: Union[str, int], *args, **kwargs) -> Optional[SimilarTracks]:
         """Получение похожих треков.
 
         Args:
-            track_id (:obj:`str`): Уникальный идентификатор трека.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
+            track_id (:obj:`str` | :obj:`int`): Уникальный идентификатор трека.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.SimilarTracks`: Похожие треки на другой трек.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/tracks/{track_id}/similar'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return SimilarTracks.de_json(result, self)
 
     @log
     def play_audio(
         self,
         track_id: Union[str, int],
@@ -631,15 +642,14 @@
         play_id: str = None,
         uid: int = None,
         timestamp: str = None,
         track_length_seconds: int = 0,
         total_played_seconds: int = 0,
         end_position_seconds: int = 0,
         client_now: str = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> bool:
         """Метод для отправки текущего состояния прослушиваемого трека.
 
         Args:
             track_id (:obj:`str` | :obj:`int`): Уникальный идентификатор трека.
@@ -650,16 +660,14 @@
             play_id (:obj:`str`, optional): Уникальный идентификатор проигрывания.
             uid (:obj:`int`, optional): Уникальный идентификатор пользователя.
             timestamp (:obj:`str`, optional): Текущая дата и время в ISO.
             track_length_seconds (:obj:`int`, optional): Продолжительность трека в секундах.
             total_played_seconds (:obj:`int`, optional): Сколько было всего воспроизведено трека в секундах.
             end_position_seconds (:obj:`int`, optional): Окончательное значение воспроизведенных секунд.
             client_now (:obj:`str`, optional): Текущая дата и время клиента в ISO.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -681,52 +689,47 @@
             'total-played-seconds': total_played_seconds,
             'end-position-seconds': end_position_seconds,
             'album-id': album_id,
             'playlist-id': playlist_id,
             'client-now': client_now or f'{datetime.now().isoformat()}Z',
         }
 
-        result = self._request.post(url, data, timeout=timeout, *args, **kwargs)
+        result = self._request.post(url, data, *args, **kwargs)
 
         return result == 'ok'
 
     @log
-    def albums_with_tracks(
-        self, album_id: Union[str, int], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[Album]:
+    def albums_with_tracks(self, album_id: Union[str, int], *args, **kwargs) -> Optional[Album]:
         """Получение альбома по его уникальному идентификатору вместе с треками.
 
         Args:
             album_id (:obj:`str` | :obj:`int`): Уникальный идентификатор альбома.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Album` | :obj:`None`: Альбом или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/albums/{album_id}/with-tracks'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return Album.de_json(result, self)
 
     @log
     def search(
         self,
         text: str,
         nocorrect: bool = False,
         type_: str = 'all',
         page: int = 0,
         playlist_in_best: bool = True,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[Search]:
         """Осуществление поиска по запросу и типу, получение результатов.
 
         Note:
             Известные значения для поля `type_`: `all`, `artist`, `user`, `album`, `playlist`, `track`, `podcast`,
@@ -737,16 +740,14 @@
         Args:
             text (:obj:`str`): Текст запроса.
             nocorrect (:obj:`bool`): Если :obj:`False`, то ошибочный запрос будет исправлен. Например, запрос
                 "Гражданская абарона" будет исправлен на "Гражданская оборона".
             type_ (:obj:`str`): Среди какого типа искать (трек, плейлист, альбом, исполнитель, пользователь, подкаст).
             page (:obj:`int`): Номер страницы.
             playlist_in_best (:obj:`bool`): Выдавать ли плейлисты лучшим вариантом поиска.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Search` | :obj:`None`: Результаты поиска или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -758,96 +759,87 @@
             'text': text,
             'nocorrect': str(nocorrect),
             'type': type_,
             'page': page,
             'playlist-in-best': str(playlist_in_best),
         }
 
-        result = self._request.get(url, params, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, params, *args, **kwargs)
 
         if isinstance(result, str):
             raise BadRequestError(result)
 
         return Search.de_json(result, self)
 
     @log
-    def search_suggest(self, part: str, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Suggestions]:
+    def search_suggest(self, part: str, *args, **kwargs) -> Optional[Suggestions]:
         """Получение подсказок по введенной части поискового запроса.
 
         Args:
             part (:obj:`str`): Часть поискового запроса.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Suggestions` | :obj:`None`: Подсказки для запроса или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/search/suggest'
 
-        result = self._request.get(url, {'part': part}, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, {'part': part}, *args, **kwargs)
 
         return Suggestions.de_json(result, self)
 
     @log
-    def users_settings(
-        self, user_id: Union[str, int] = None, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[UserSettings]:
+    def users_settings(self, user_id: Union[str, int] = None, *args, **kwargs) -> Optional[UserSettings]:
         """Получение настроек пользователя.
 
         Note:
             Для получения настроек пользователя нужно быть авторизованным или владеть `user_id`.
 
         Args:
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя чьи настройки хотим
                 получить.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.UserSettings` | :obj:`None`: Настройки пользователя или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/settings'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return UserSettings.de_json(result.get('user_settings'), self)
 
     @log
     def users_playlists(
         self,
         kind: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Union[Playlist, List[Playlist]]:
         """Получение плейлиста или списка плейлистов по уникальным идентификаторам.
 
         Note:
             Если передан один `kind`, то вернётся не список плейлистов, а один плейлист.
 
         Args:
             kind (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста
                 или их список.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Playlist` | :obj:`yandex_music.Playlist` | :obj:`None`:
             Список плейлистов или плейлист, иначе :obj:`None`.
 
         Raises:
@@ -858,69 +850,62 @@
             user_id = self.me.account.uid
 
         if isinstance(kind, list):
             url = f'{self.base_url}/users/{user_id}/playlists'
 
             data = {'kinds': kind}
 
-            result = self._request.post(url, data, timeout=timeout, *args, **kwargs)
+            result = self._request.post(url, data, *args, **kwargs)
 
             return Playlist.de_list(result, self)
         else:
             url = f'{self.base_url}/users/{user_id}/playlists/{kind}'
-            result = self._request.get(url, timeout=timeout, *args, **kwargs)
+            result = self._request.get(url, *args, **kwargs)
 
             return Playlist.de_json(result, self)
 
     @log
-    def users_playlists_recommendations(
-        self, kind: Union[str, int], user_id: Union[str, int] = None, timeout: Union[int, float] = None, *args, **kwargs
-    ):
+    def users_playlists_recommendations(self, kind: Union[str, int], user_id: Union[str, int] = None, *args, **kwargs):
         """Получение рекомендаций для плейлиста.
 
         Args:
             kind (:obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста.
             user_id (:obj:`str` | :obj:`int`): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.PlaylistRecommendations` | :obj:`None`: Рекомендации для плейлиста или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/playlists/{kind}/recommendations'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return PlaylistRecommendations.de_json(result, self)
 
     @log
     def users_playlists_create(
         self,
         title: str,
         visibility: str = 'public',
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[Playlist]:
         """Создание плейлиста.
 
         Args:
             title (:obj:`str`): Название.
             visibility (:obj:`str`, optional): Модификатор доступа.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Playlist` | :obj:`None`: Созданный плейлист или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -929,130 +914,119 @@
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/playlists/create'
 
         data = {'title': title, 'visibility': visibility}
 
-        result = self._request.post(url, data, timeout=timeout, *args, **kwargs)
+        result = self._request.post(url, data, *args, **kwargs)
 
         return Playlist.de_json(result, self)
 
     @log
-    def users_playlists_delete(
-        self, kind: Union[str, int], user_id: Union[str, int] = None, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> bool:
+    def users_playlists_delete(self, kind: Union[str, int], user_id: Union[str, int] = None, *args, **kwargs) -> bool:
         """Удаление плейлиста.
 
         Args:
             kind (:obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/playlists/{kind}/delete'
 
-        result = self._request.post(url, timeout=timeout, *args, **kwargs)
+        result = self._request.post(url, *args, **kwargs)
 
         return result == 'ok'
 
     @log
     def users_playlists_name(
         self,
         kind: Union[str, int],
         name: str,
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[Playlist]:
         """Изменение названия плейлиста.
 
         Args:
             kind (:obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста.
             name (:obj:`str`): Новое название.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Playlist` | :obj:`None`: Изменённый плейлист или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/playlists/{kind}/name'
 
-        result = self._request.post(url, {'value': name}, timeout=timeout, *args, **kwargs)
+        result = self._request.post(url, {'value': name}, *args, **kwargs)
 
         return Playlist.de_json(result, self)
 
     @log
     def users_playlists_visibility(
         self,
         kind: Union[str, int],
         visibility: str,
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[Playlist]:
         """Изменение видимости плейлиста.
 
         Note:
             Видимость (`visibility`) может быть задана только одним из двух значений: `private`, `public`.
 
         Args:
             kind (:obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста.
             visibility (:obj:`str`): Новое название.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Playlist` | :obj:`None`: Изменённый плейлист или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/playlists/{kind}/visibility'
 
-        result = self._request.post(url, {'value': visibility}, timeout=timeout, *args, **kwargs)
+        result = self._request.post(url, {'value': visibility}, *args, **kwargs)
 
         return Playlist.de_json(result, self)
 
     @log
     def users_playlists_change(
         self,
         kind: Union[str, int],
         diff: str,
         revision: int = 1,
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[Playlist]:
         """Изменение плейлиста.
 
         Note:
             Для получения отличий есть вспомогательный класс :class:`yandex_music.utils.difference.Difference`.
@@ -1060,16 +1034,14 @@
             Так же существуют уже готовые методы-обёртки над операциями.
 
         Args:
             kind (:obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста.
             revision (:obj:`int`): TODO.
             diff (:obj:`str`): JSON представления отличий старого и нового плейлиста.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Playlist`: Изменённый плейлист или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -1078,28 +1050,27 @@
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/playlists/{kind}/change'
 
         data = {'kind': kind, 'revision': revision, 'diff': diff}
 
-        result = self._request.post(url, data, timeout=timeout, *args, **kwargs)
+        result = self._request.post(url, data, *args, **kwargs)
 
         return Playlist.de_json(result, self)
 
     @log
     def users_playlists_insert_track(
         self,
         kind: Union[str, int],
         track_id: Union[str, int],
         album_id: Union[str, int],
         at: int = 0,
         revision: int = 1,
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[Playlist]:
         """Добавление трека в плейлист.
 
         Note:
             Трек можно вставить с любое место плейлиста задав индекс вставки (аргумент `at`).
@@ -1107,186 +1078,174 @@
         Args:
             kind (:obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста.
             track_id (:obj:`str` | :obj:`int`): Уникальный идентификатор трека.
             album_id (:obj:`str` | :obj:`int`): Уникальный идентификатор альбома.
             at (:obj:`int`): Индекс для вставки.
             revision (:obj:`int`): TODO.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Playlist`: Изменённый плейлист или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         diff = Difference().add_insert(at, {'id': track_id, 'album_id': album_id})
 
-        return self.users_playlists_change(kind, diff.to_json(), revision, user_id, timeout, *args, **kwargs)
+        return self.users_playlists_change(kind, diff.to_json(), revision, user_id, *args, **kwargs)
 
     @log
     def users_playlists_delete_track(
         self,
         kind: Union[str, int],
         from_: int,
         to: int,
         revision: int = 1,
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[Playlist]:
         """Удаление треков из плейлиста.
 
         Note:
             Для удаление необходимо указать границы с какого по какой элемент (трек) удалить.
 
         Args:
             kind (:obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста.
             from_ (:obj:`int`): С какого индекса.
             to (:obj:`int`): По какой индекс.
             revision (:obj:`int`): TODO.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Playlist` | :obj:`None`: Изменённый плейлист или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         diff = Difference().add_delete(from_, to)
 
-        return self.users_playlists_change(kind, diff.to_json(), revision, user_id, timeout, *args, **kwargs)
+        return self.users_playlists_change(kind, diff.to_json(), revision, user_id, *args, **kwargs)
 
     @log
-    def rotor_account_status(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Status]:
-        """Получение статуса пользователя с дополнителньыми полями.
+    def rotor_account_status(self, *args, **kwargs) -> Optional[Status]:
+        """Получение статуса пользователя с дополнительными полями.
 
         Note:
             Данный статус отличается от обычного наличием дополнительных полей, например, `skips_per_hour`.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Status` | :obj:`None`: Статус пользователя с дополнительными полями от радио или
                 :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/rotor/account/status'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return Status.de_json(result, self)
 
     @log
-    def rotor_stations_dashboard(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Dashboard]:
+    def rotor_stations_dashboard(self, *args, **kwargs) -> Optional[Dashboard]:
         """Получение рекомендованных станций текущего пользователя.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Dashboard` | :obj:`None`: Рекомендованные станции или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/rotor/stations/dashboard'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return Dashboard.de_json(result, self)
 
     @log
-    def rotor_stations_list(
-        self, language: str = 'ru', timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[StationResult]:
+    def rotor_stations_list(self, language: Optional[str] = None, *args, **kwargs) -> List[StationResult]:
         """Получение всех радиостанций с настройками пользователя.
 
         Note:
+            Доступные языки: en, uz, uk, us, ru, kk, hy.
+
             Чтобы определить что за тип станции (жанры, настроения, занятие и т.д.) необходимо смотреть в поле
             `id_for_from`.
 
         Args:
-            language (:obj:`str`): Язык, на котором будет информация о станциях.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
+            language (:obj:`str`, optional): Язык, на котором будет информация о станциях. По умолчанию язык клиента.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
-            :obj:`list` из :obj:`yandex_music.StationResult` | :obj:`None`: Станции или :obj:`None`.
+            :obj:`list` из :obj:`yandex_music.StationResult`: Список станций.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/rotor/stations/list'
 
-        result = self._request.get(url, {'language': language}, timeout=timeout, *args, **kwargs)
+        if not language:
+            language = self.language
+
+        result = self._request.get(url, {'language': language}, *args, **kwargs)
 
         return StationResult.de_list(result, self)
 
     @log
     def rotor_station_feedback(
         self,
         station: str,
         type_: str,
         timestamp: Union[str, float, int] = None,
         from_: str = None,
         batch_id: str = None,
         total_played_seconds: Union[int, float] = None,
         track_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
-        """Отправка ответной реакции на происходящее при прослушивании радио.
+        """Отправка обратной связи на действия при прослушивании радио.
 
         Note:
             Сообщения о начале прослушивания радио, начале и конце трека, его пропуска.
 
-            Известные типы фидбека: `radioStarted`, `trackStarted`, `trackFinished`, `skip`.
+            Известные типы обратной связи: `radioStarted`, `trackStarted`, `trackFinished`, `skip`.
 
             Пример `station`: `user:onyourwave`, `genre:allrock`.
 
             Пример `from_`: `mobile-radio-user-123456789`.
 
         Args:
             station (:obj:`str`): Станция.
-            type_ (:obj:`str`): Тип отправляемого фидбека.
+            type_ (:obj:`str`): Тип отправляемого отзыва.
             timestamp (:obj:`str` | :obj:`float` | :obj:`int`, optional): Текущее время и дата.
             from_ (:obj:`str`, optional): Откуда начато воспроизведение радио.
             batch_id (:obj:`str`, optional): Уникальный идентификатор партии треков. Возвращается при получении треков.
             total_played_seconds (:obj:`int` |:obj:`float`, optional): Сколько было проиграно секунд трека
                 перед действием.
             track_id (:obj:`int` | :obj:`str`, optional): Уникальной идентификатор трека.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -1308,173 +1267,154 @@
 
         if from_:
             data.update({'from': from_})
 
         if total_played_seconds:
             data.update({'totalPlayedSeconds': total_played_seconds})
 
-        result = self._request.post(url, params=params, json=data, timeout=timeout, *args, **kwargs)
+        result = self._request.post(url, params=params, json=data, **kwargs)
 
         return result == 'ok'
 
     @log
     def rotor_station_feedback_radio_started(
         self,
         station: str,
         from_: str,
         batch_id: str = None,
         timestamp: Union[str, float, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Сокращение для::
 
-            client.rotor_station_feedback(station, 'radioStarted', timestamp, from, *args, **kwargs)
+            client.rotor_station_feedback(station, 'radioStarted', timestamp, from, batch_id, **kwargs)
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self.rotor_station_feedback(
-            station, 'radioStarted', timestamp, from_=from_, batch_id=batch_id, timeout=timeout, *args, **kwargs
-        )
+        return self.rotor_station_feedback(station, 'radioStarted', timestamp, from_=from_, batch_id=batch_id, **kwargs)
 
     @log
     def rotor_station_feedback_track_started(
         self,
         station: str,
         track_id: Union[str, int],
         batch_id: str = None,
         timestamp: Union[str, float, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Сокращение для::
 
-            client.rotor_station_feedback(station, 'trackStarted', timestamp, track_id, *args, **kwargs)
+            client.rotor_station_feedback(station, 'trackStarted', timestamp, track_id=track_id,
+            batch_id=batch_id, **kwargs)
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         return self.rotor_station_feedback(
-            station, 'trackStarted', timestamp, track_id=track_id, batch_id=batch_id, timeout=timeout, *args, **kwargs
+            station, 'trackStarted', timestamp, track_id=track_id, batch_id=batch_id, **kwargs
         )
 
     @log
     def rotor_station_feedback_track_finished(
         self,
         station: str,
         track_id: Union[str, int],
         total_played_seconds: float,
         batch_id: str = None,
         timestamp: Union[str, float, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Сокращение для::
 
-            client.rotor_station_feedback(station, 'trackFinished', timestamp, track_id, total_played_seconds,
-            *args, **kwargs)
+            client.rotor_station_feedback(station, 'trackFinished', timestamp,
+            track_id=track_id, total_played_seconds=total_played_seconds, batch_id=batch_id, **kwargs)
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         return self.rotor_station_feedback(
             station,
             'trackFinished',
             timestamp,
             track_id=track_id,
             total_played_seconds=total_played_seconds,
             batch_id=batch_id,
-            timeout=timeout,
-            *args,
             **kwargs,
         )
 
     @log
     def rotor_station_feedback_skip(
         self,
         station: str,
         track_id: Union[str, int],
         total_played_seconds: float,
         batch_id: str = None,
         timestamp: Union[str, float, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Сокращение для::
 
-            client.rotor_station_feedback(station, 'skip', timestamp, track_id, total_played_seconds,
-            *args, **kwargs)
+            client.rotor_station_feedback(station, 'skip', timestamp, track_id=track_id,
+            total_played_seconds=total_played_seconds, batch_id=batch_id, **kwargs)
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         return self.rotor_station_feedback(
             station,
             'skip',
             timestamp,
             track_id=track_id,
             total_played_seconds=total_played_seconds,
             batch_id=batch_id,
-            timeout=timeout,
-            *args,
             **kwargs,
         )
 
     @log
-    def rotor_station_info(
-        self, station: str, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[StationResult]:
+    def rotor_station_info(self, station: str, *args, **kwargs) -> List[StationResult]:
         """Получение информации о станции и пользовательских настроек на неё.
 
         Args:
             station (:obj:`str`): Станция.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.StationResult` | :obj:`None`: Информация о станции или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/rotor/station/{station}/info'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return StationResult.de_list(result, self)
 
     @log
     def rotor_station_settings2(
         self,
         station: str,
         mood_energy: str,
         diversity: str,
-        language: str = 'not-russian',
+        language: str = 'not-russian',  # TODO(#555): заменить на any
         type_: str = 'rotor',
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Изменение настроек определённой станции.
 
         Note:
             Доступные значения для `mood_energy`: `fun`, `active`, `calm`, `sad`, `all`.
 
@@ -1488,16 +1428,14 @@
 
         Args:
             station (:obj:`str`): Станция.
             mood_energy (:obj:`str`): Настроение.
             diversity (:obj:`str`): Треки.
             language (:obj:`str`): Язык.
             type_ (:obj:`str`): Тип.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -1506,51 +1444,48 @@
         url = f'{self.base_url}/rotor/station/{station}/settings3'
 
         data = {'moodEnergy': mood_energy, 'diversity': diversity, 'type': type_}
 
         if language:
             data.update({'language': language})
 
-        result = self._request.post(url, json=data, timeout=timeout, *args, **kwargs)
+        result = self._request.post(url, json=data, **kwargs)
 
         return result == 'ok'
 
     @log
     def rotor_station_tracks(
         self,
         station: str,
         settings2: bool = True,
         queue: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[StationTracksResult]:
         """Получение цепочки треков определённой станции.
 
         Note:
             Запуск потока по сущности сервиса осуществляется через станцию `<type>:<id>`.
             Например, станцией для запуска потока по треку будет `track:1234`.
 
             Для продолжения цепочки треков необходимо:
 
             1. Передавать `ID` трека, что был до этого (первый в цепочки).
-            2. Отправить фидбек о конче или скипе трека, что был передан в `queue`.
+            2. Отправить фидбек о конце или скипе трека, что был передан в `queue`.
             3. Отправить фидбек о начале следующего трека (второй в цепочки).
             4. Выполнить запрос получения треков. В ответе придёт новые треки или произойдёт сдвиг цепочки на 1 элемент.
 
-            Проход по цепочке до коцна не изучен. Часто встречаются дубликаты.
+            Проход по цепочке до конца не изучен. Часто встречаются дубликаты.
 
             Все официальные клиенты выполняют запросы с `settings2 = True`.
 
         Args:
             station (:obj:`str`): Станция.
             settings2 (:obj:`bool`, optional): Использовать ли второй набор настроек.
             queue (:obj:`str` | :obj:`int` , optional): Уникальной идентификатор трека, который только что был.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.StationTracksResult` | :obj:`None`: Последовательность треков станции или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -1561,124 +1496,113 @@
         params = {}
         if settings2:
             params = {'settings2': str(True)}
 
         if queue:
             params = {'queue': queue}
 
-        result = self._request.get(url, params=params, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, params, *args, **kwargs)
 
         return StationTracksResult.de_json(result, self)
 
     @log
-    def artists_brief_info(
-        self, artist_id: Union[str, int], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[BriefInfo]:
+    def artists_brief_info(self, artist_id: Union[str, int], *args, **kwargs) -> Optional[BriefInfo]:
         """Получение информации об артисте.
 
         Args:
             artist_id (:obj:`str` | :obj:`int`): Уникальный идентификатор исполнителя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.BriefInfo` | :obj:`None`: Информация об артисте или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         url = f'{self.base_url}/artists/{artist_id}/brief-info'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return BriefInfo.de_json(result, self)
 
     @log
     def artists_tracks(
         self,
         artist_id: Union[str, int],
         page: int = 0,
         page_size: int = 20,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[ArtistTracks]:
         """Получение треков артиста.
 
         Args:
             artist_id (:obj:`str` | :obj:`int`): Уникальный идентификатор артиста.
             page (:obj:`int`, optional): Номер страницы.
             page_size (:obj:`int`, optional): Количество треков на странице.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.ArtistsTracks` | :obj:`None`: Страница списка треков артиста или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/artists/{artist_id}/tracks'
 
         params = {'page': page, 'page-size': page_size}
 
-        result = self._request.get(url, params, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, params, *args, **kwargs)
 
         return ArtistTracks.de_json(result, self)
 
     @log
     def artists_direct_albums(
         self,
         artist_id: Union[str, int],
         page: int = 0,
         page_size: int = 20,
         sort_by: str = 'year',
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[ArtistAlbums]:
         """Получение альбомов артиста.
 
         Note:
             Известные значения для `sort_by`: `year`, `rating`.
 
         Args:
             artist_id (:obj:`str` | :obj:`int`): Уникальный идентификатор артиста.
             page (:obj:`int`, optional): Номер страницы.
             page_size (:obj:`int`, optional): Количество альбомов на странице.
             sort_by (:obj:`str`, optional): Параметр для сортировки.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.ArtistAlbums` | :obj:`None`: Страница списка альбомов артиста или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/artists/{artist_id}/direct-albums'
 
         params = {'sort-by': sort_by, 'page': page, 'page-size': page_size}
 
-        result = self._request.get(url, params, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, params, *args, **kwargs)
 
         return ArtistAlbums.de_json(result, self)
 
     def _like_action(
         self,
         object_type: str,
         ids: Union[List[Union[str, int]], str, int],
         remove: bool = False,
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> bool:
         """Действия с отметкой "Мне нравится".
 
         Note:
             Типы объектов: `track` - трек, `artist` - исполнитель, `playlist` - плейлист, `album` - альбом.
@@ -1689,290 +1613,253 @@
         Args:
             object_type (:obj:`str`): Тип объекта.
             ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор объекта или объектов.
             remove (:obj:`bool`, optional): Если :obj:`True` то снимает отметку, иначе ставит.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         action = 'remove' if remove else 'add-multiple'
         url = f'{self.base_url}/users/{user_id}/likes/{object_type}s/{action}'
 
-        result = self._request.post(url, {f'{object_type}-ids': ids}, timeout=timeout, *args, **kwargs)
+        result = self._request.post(url, {f'{object_type}-ids': ids}, *args, **kwargs)
 
         if object_type == 'track':
             return 'revision' in result
 
         return result == 'ok'
 
     @log
     def users_likes_tracks_add(
         self,
         track_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Поставить отметку "Мне нравится" треку/трекам.
 
         Note:
             Так же снимает отметку "Не рекомендовать" если она есть.
 
         Args:
             track_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор трека или треков.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._like_action('track', track_ids, False, user_id, timeout, *args, **kwargs)
+        return self._like_action('track', track_ids, remove=False, user_id=user_id, **kwargs)
 
     @log
     def users_likes_tracks_remove(
         self,
         track_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Снять отметку "Мне нравится" у трека/треков.
 
         Args:
             track_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор трека или треков.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._like_action('track', track_ids, True, user_id, timeout, *args, **kwargs)
+        return self._like_action('track', track_ids, remove=True, user_id=user_id, **kwargs)
 
     @log
     def users_likes_artists_add(
         self,
         artist_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Поставить отметку "Мне нравится" исполнителю/исполнителям.
 
         Args:
             artist_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор артиста или артистов.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._like_action('artist', artist_ids, False, user_id, timeout, *args, **kwargs)
+        return self._like_action('artist', artist_ids, remove=False, user_id=user_id, **kwargs)
 
     @log
     def users_likes_artists_remove(
         self,
         artist_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Снять отметку "Мне нравится" у исполнителя/исполнителей.
 
         Args:
             artist_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор артиста или артистов.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._like_action('artist', artist_ids, True, user_id, timeout, *args, **kwargs)
+        return self._like_action('artist', artist_ids, remove=True, user_id=user_id, **kwargs)
 
     @log
     def users_likes_playlists_add(
         self,
         playlist_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Поставить отметку "Мне нравится" плейлисту/плейлистам.
 
         Note:
             Идентификатор плейлиста указывается в формате `owner_id:playlist_id`. Где `playlist_id` - идентификатор
             плейлиста, `owner_id` - уникальный идентификатор владельца плейлиста.
 
         Args:
             playlist_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор плейлиста или плейлистов.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._like_action('playlist', playlist_ids, False, user_id, timeout, *args, **kwargs)
+        return self._like_action('playlist', playlist_ids, remove=False, user_id=user_id, **kwargs)
 
     @log
     def users_likes_playlists_remove(
         self,
         playlist_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Снять отметку "Мне нравится" у плейлиста/плейлистов.
 
         Note:
             Идентификатор плейлиста указывается в формате `owner_id:playlist_id`. Где `playlist_id` - идентификатор
             плейлиста, `owner_id` - уникальный идентификатор владельца плейлиста.
 
         Args:
             playlist_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор плейлиста или плейлистов.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._like_action('playlist', playlist_ids, True, user_id, timeout, *args, **kwargs)
+        return self._like_action('playlist', playlist_ids, remove=True, user_id=user_id, **kwargs)
 
     @log
     def users_likes_albums_add(
         self,
         album_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Поставить отметку "Мне нравится" альбому/альбомам.
 
         Args:
             album_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор артиста или артистов.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._like_action('album', album_ids, False, user_id, timeout, *args, **kwargs)
+        return self._like_action('album', album_ids, remove=False, user_id=user_id, **kwargs)
 
     @log
     def users_likes_albums_remove(
         self,
         album_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Снять отметку "Мне нравится" у альбома/альбомов.
 
         Args:
             album_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор артиста или артистов.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._like_action('album', album_ids, True, user_id, timeout, *args, **kwargs)
+        return self._like_action('album', album_ids, remove=True, user_id=user_id, **kwargs)
 
     def _get_list(
         self,
         object_type: str,
         ids: Union[List[Union[str, int]], int, str],
         params: dict = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> List[Union[Artist, Album, Track, Playlist]]:
         """Получение объекта/объектов.
 
         Args:
             object_type (:obj:`str`): Тип объекта.
             ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор объекта или объектов.
             params (:obj:`dict`, optional): Параметры, которые будут переданы в запрос.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Artist` | :obj:`list` из :obj:`yandex_music.Album` |
                 :obj:`list` из :obj:`yandex_music.Track` | :obj:`list` из :obj:`yandex_music.Playlist`: Запрошенный
                 объект.
 
@@ -1981,452 +1868,402 @@
         """
         if params is None:
             params = {}
         params.update({f'{object_type}-ids': ids})
 
         url = f'{self.base_url}/{object_type}s' + ('/list' if object_type == 'playlist' else '')
 
-        result = self._request.post(url, params, timeout=timeout, *args, **kwargs)
+        result = self._request.post(url, params, *args, **kwargs)
 
         return de_list[object_type](result, self)
 
     @log
-    def artists(
-        self, artist_ids: Union[List[Union[str, int]], int, str], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[Artist]:
+    def artists(self, artist_ids: Union[List[Union[str, int]], int, str], *args, **kwargs) -> List[Artist]:
         """Получение исполнителя/исполнителей.
 
         Args:
             artist_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор исполнителя или исполнителей.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Artist`: Исполнитель или исполнители.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._get_list('artist', artist_ids, timeout=timeout, *args, **kwargs)
+        return self._get_list('artist', artist_ids, *args, **kwargs)
 
     @log
-    def albums(
-        self, album_ids: Union[List[Union[str, int]], int, str], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[Album]:
+    def albums(self, album_ids: Union[List[Union[str, int]], int, str], *args, **kwargs) -> List[Album]:
         """Получение альбома/альбомов.
 
         Args:
             album_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор альбома или альбомов.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Album`: Альбом или альбомы.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._get_list('album', album_ids, timeout=timeout, *args, **kwargs)
+        return self._get_list('album', album_ids, *args, **kwargs)
 
     @log
     def tracks(
         self,
         track_ids: Union[List[Union[str, int]], int, str],
         with_positions: bool = True,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> List[Track]:
         """Получение трека/треков.
 
         Args:
             track_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор трека или треков.
             with_positions (:obj:`bool`, optional): С позициями TODO.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Track`: Трек или Треки.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._get_list('track', track_ids, {'with-positions': str(with_positions)}, timeout, *args, **kwargs)
+        return self._get_list('track', track_ids, {'with-positions': str(with_positions)}, *args, **kwargs)
 
     @log
-    def playlists_list(
-        self, playlist_ids: Union[List[Union[str, int]], int, str], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[Playlist]:
+    def playlists_list(self, playlist_ids: Union[List[Union[str, int]], int, str], *args, **kwargs) -> List[Playlist]:
         """Получение плейлиста/плейлистов.
 
         Note:
             Идентификатор плейлиста указывается в формате `owner_id:playlist_id`. Где `playlist_id` - идентификатор
             плейлиста, `owner_id` - уникальный идентификатор владельца плейлиста.
 
+            Данный метод возвращает сокращенную модель плейлиста для отображения больших список.
+
+        Warning:
+            Данный метод не возвращает список треков у плейлиста! Для получения объекта :obj:`yandex_music.Playlist` c
+            заполненным полем `tracks` используйте метод :func:`yandex_music.Client.users_playlists` или
+            метод :func:`yandex_music.Playlist.fetch_tracks`.
+
         Args:
             playlist_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор плейлиста или плейлистов.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Playlist`: Плейлист или плейлисты.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._get_list('playlist', playlist_ids, timeout=timeout, *args, **kwargs)
+        return self._get_list('playlist', playlist_ids, *args, **kwargs)
 
     @log
-    def playlists_collective_join(
-        self, user_id: int, token: str, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> bool:
+    def playlists_collective_join(self, user_id: int, token: str, **kwargs) -> bool:
         """Присоединение к плейлисту как соавтор.
 
         Note:
             В качестве `user_id` принимается исключительно числовой уникальный идентификатор пользователя, не username.
 
             Токен можно получить в Web-версии. Для этого, на странице плейлиста нужно нажать на
             "Добавить соавтора". В полученной ссылке GET параметр `token` и будет токеном для присоединения.
 
         Args:
             user_id (:obj:`int`): Владелец плейлиста.
             token (:obj:`str`): Токен для присоединения.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs: Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         url = f'{self.base_url}/playlists/collective/join'
 
         params = {'uid': user_id, 'token': token}
 
-        result = self._request.post(url, params=params, timeout=timeout, *args, **kwargs)
+        result = self._request.post(url, params=params, **kwargs)
 
         return result == 'ok'
 
     @log
-    def users_playlists_list(
-        self, user_id: Union[str, int] = None, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[Playlist]:
+    def users_playlists_list(self, user_id: Union[str, int] = None, *args, **kwargs) -> List[Playlist]:
         """Получение списка плейлистов пользователя.
 
         Args:
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Playlist`: Плейлисты пользователя.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/playlists/list'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return Playlist.de_list(result, self)
 
     def _get_likes(
         self,
         object_type: str,
         user_id: Union[str, int] = None,
         params: dict = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Union[List[Like], Optional[TracksList]]:
         """Получение объектов с отметкой "Мне нравится".
 
         Args:
             object_type (:obj:`str`): Тип объекта.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
             params (:obj:`dict`, optional): Параметры, которые будут переданы в запрос.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Like` | :obj:`yandex_music.TracksList`: Объекты с отметкой "Мне нравится".
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/likes/{object_type}s'
 
-        result = self._request.get(url, params, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, params, *args, **kwargs)
 
         if object_type == 'track':
             return TracksList.de_json(result.get('library'), self)
 
         return Like.de_list(result, self, object_type)
 
     @log
     def users_likes_tracks(
         self,
         user_id: Union[str, int] = None,
         if_modified_since_revision: int = 0,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[TracksList]:
         """Получение треков с отметкой "Мне нравится".
 
         Args:
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
             if_modified_since_revision (:obj:`int`, optional): TODO.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.TracksList`: Треки с отметкой "Мне нравится".
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         return self._get_likes(
-            'track', user_id, {'if-modified-since-revision': if_modified_since_revision}, timeout, *args, **kwargs
+            'track', user_id, {'if-modified-since-revision': if_modified_since_revision}, *args, **kwargs
         )
 
     @log
-    def users_likes_albums(
-        self, user_id: Union[str, int] = None, rich: bool = True, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[Like]:
+    def users_likes_albums(self, user_id: Union[str, int] = None, rich: bool = True, *args, **kwargs) -> List[Like]:
         """Получение альбомов с отметкой "Мне нравится".
 
         Args:
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
             rich (:obj:`bool`, optional): Если False, то приходит укороченная версия.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Like`: Альбомы с отметкой "Мне нравится".
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._get_likes('album', user_id, {'rich': str(rich)}, timeout, *args, **kwargs)
+        return self._get_likes('album', user_id, {'rich': str(rich)}, *args, **kwargs)
 
     @log
     def users_likes_artists(
         self,
         user_id: Union[str, int] = None,
         with_timestamps: bool = True,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> List[Like]:
         """Получение артистов с отметкой "Мне нравится".
 
         Args:
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
             with_timestamps (:obj:`bool`, optional):  С временными метками TODO.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Like`: Артисты с отметкой "Мне нравится".
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._get_likes('artist', user_id, {'with-timestamps': str(with_timestamps)}, timeout, *args, **kwargs)
+        return self._get_likes('artist', user_id, {'with-timestamps': str(with_timestamps)}, *args, **kwargs)
 
     @log
-    def users_likes_playlists(
-        self, user_id: Union[str, int] = None, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[Like]:
+    def users_likes_playlists(self, user_id: Union[str, int] = None, *args, **kwargs) -> List[Like]:
         """Получение плейлистов с отметкой "Мне нравится".
 
         Args:
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Like`: Плейлисты с отметкой "Мне нравится".
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._get_likes('playlist', user_id, timeout=timeout, *args, **kwargs)
+        return self._get_likes('playlist', user_id, *args, **kwargs)
 
     @log
     def users_dislikes_tracks(
         self,
         user_id: Union[str, int] = None,
         if_modified_since_revision: int = 0,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[TracksList]:
         """Получение треков с отметкой "Не рекомендовать".
 
         Args:
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
             if_modified_since_revision (:obj:`bool`, optional): TODO.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.TracksList`: Треки с отметкой "Не рекомендовать".
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/dislikes/tracks'
 
-        result = self._request.get(
-            url, {'if_modified_since_revision': if_modified_since_revision}, timeout=timeout, *args, **kwargs
-        )
+        result = self._request.get(url, {'if_modified_since_revision': if_modified_since_revision}, *args, **kwargs)
 
         return TracksList.de_json(result.get('library'), self)
 
     def _dislike_action(
         self,
         ids: Union[List[Union[str, int]], str, int],
         remove: bool = False,
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> bool:
         """Действия с отметкой "Не рекомендовать".
 
         Args:
             ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор объекта или объектов.
             remove (:obj:`bool`, optional): Если :obj:`True`, то снимает отметку, иначе ставит.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         action = 'remove' if remove else 'add-multiple'
         url = f'{self.base_url}/users/{user_id}/dislikes/tracks/{action}'
 
-        result = self._request.post(url, {f'track-ids': ids}, timeout=timeout, *args, **kwargs)
+        result = self._request.post(url, {f'track-ids': ids}, *args, **kwargs)
 
         return 'revision' in result
 
     @log
     def users_dislikes_tracks_add(
         self,
         track_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Поставить отметку "Не рекомендовать" треку/трекам.
 
         Note:
             Так же снимает отметку "Мне нравится" если она есть.
 
         Args:
             track_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор трека или треков.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._dislike_action(track_ids, False, user_id, timeout, *args, **kwargs)
+        return self._dislike_action(track_ids, remove=False, user_id=user_id, **kwargs)
 
     @log
     def users_dislikes_tracks_remove(
         self,
         track_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Снять отметку "Не рекомендовать" у трека/треков.
 
         Args:
             track_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор трека или треков.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return self._dislike_action(track_ids, True, user_id, timeout, *args, **kwargs)
+        return self._dislike_action(track_ids, remove=True, user_id=user_id, **kwargs)
 
     @log
     def after_track(
         self,
         next_track_id: Union[str, int],
         context_item: str,
         prev_track_id: Union[str, int] = None,
         context: str = 'playlist',
         types: str = 'shot',
         from_: str = 'mobile-landing-origin-default',
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[ShotEvent]:
         """Получение рекламы или шота от Алисы после трека.
 
         Note:
             При получения шота от Алисы `prev_track_id` можно не указывать.
@@ -2443,16 +2280,14 @@
         Args:
             prev_track_id (:obj:`str` | :obj:`int`): Уникальный идентификатор предыдущего трека.
             next_track_id (:obj:`str` | :obj:`int`): Уникальный идентификатор следующего трека.
             context_item (:obj:`str`): Уникальный идентификатор контекста.
             context (:obj:`str`, optional): Место, откуда было вызвано получение.
             types (:obj:`str`, optional): Тип того, что вернуть после трека.
             from_ (:obj:`str`, optional): Место, с которого попали в контекст.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.ShotEvent`: Шот от Алисы или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -2465,119 +2300,106 @@
             'prevTrackId': prev_track_id,
             'nextTrackId': next_track_id,
             'context': context,
             'contextItem': context_item,
             'types': types,
         }
 
-        result = self._request.get(url, params=params, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, params, *args, **kwargs)
 
-        # TODO судя по всему эндпоинт ещё возвращает рекламу после треков для пользователей без подписки.
+        # TODO (MarshalX) судя по всему ручка ещё возвращает рекламу после треков для пользователей без подписки.
+        #  https://github.com/MarshalX/yandex-music-api/issues/557
         return ShotEvent.de_json(result.get('shot_event'), self)
 
     @log
-    def queues_list(self, device: str = None, timeout: Union[int, float] = None, *args, **kwargs) -> List[QueueItem]:
+    def queues_list(self, device: str = None, *args, **kwargs) -> List[QueueItem]:
         """Получение всех очередей треков с разных устройств для синхронизации между ними.
 
         Note:
             Именно к `device` привязывается очередь. На одном устройстве может быть создана одна очередь.
 
             Аргумент `device` имеет следующий формат: `ключ=значение; ключ2=значение2`. Обязательные паля указы в
             значении по умолчанию.
 
         Args:
             device (:obj:`str`, optional): Содержит информацию об устройстве с которого выполняется запрос.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.QueueItem`: Элементы очереди всех устройств.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if not device:
             device = self.device
 
         url = f'{self.base_url}/queues'
 
         self._request.headers['X-Yandex-Music-Device'] = device
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return QueueItem.de_list(result.get('queues'), self)
 
     @log
-    def queue(self, queue_id: str, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Queue]:
+    def queue(self, queue_id: str, *args, **kwargs) -> Optional[Queue]:
         """Получение информации об очереди треков и самих треков в ней.
 
         Args:
             queue_id (:obj:`str`): Уникальный идентификатор очереди.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Queue`: Очередь или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         url = f'{self.base_url}/queues/{queue_id}'
 
-        result = self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = self._request.get(url, *args, **kwargs)
 
         return Queue.de_json(result, self)
 
     @log
-    def queue_update_position(
-        self, queue_id: str, current_index: int, device: str = None, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> bool:
+    def queue_update_position(self, queue_id: str, current_index: int, device: str = None, **kwargs) -> bool:
         """Установка текущего индекса проигрываемого трека в очереди треков.
 
         Note:
             Изменить можно только у той очереди, которая была создана с переданного `device`!
 
         Args:
             queue_id (:obj:`str`): Уникальный идентификатор очереди.
             current_index (:obj:`int`): Текущий индекс.
             device (:obj:`str`, optional): Содержит информацию об устройстве с которого выполняется запрос.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if not device:
             device = self.device
 
         url = f'{self.base_url}/queues/{queue_id}/update-position'
 
         self._request.headers['X-Yandex-Music-Device'] = device
-        result = self._request.post(
-            url, {'isInteractive': False}, params={'currentIndex': current_index}, timeout=timeout, *args, **kwargs
-        )
+        result = self._request.post(url, {'isInteractive': False}, params={'currentIndex': current_index}, **kwargs)
 
         return result.get('status') == 'ok'
 
     @log
-    def queue_create(
-        self, queue: Union[Queue, str], device: str = None, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[str]:
+    def queue_create(self, queue: Union[Queue, str], device: str = None, *args, **kwargs) -> Optional[str]:
         """Создание новой очереди треков.
 
         Args:
             queue (:obj:`yandex_music.Queue` | :obj:`str`): Объект очереди или JSON строка с этим объектом.
             device (:obj:`str`, optional): Содержит информацию об устройстве с которого выполняется запрос.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`str`: Вернёт уникальный идентификатор созданной очереди, иначе :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -2587,17 +2409,17 @@
 
         if isinstance(queue, Queue):
             queue = queue.to_json(True)
 
         url = f'{self.base_url}/queues'
 
         self._request.headers['X-Yandex-Music-Device'] = device
-        result = self._request.post(url, queue, timeout=timeout, *args, **kwargs)
+        result = self._request.post(url, queue, *args, **kwargs)
 
-        return result.get('id_')
+        return result.get('id')
 
     # camelCase псевдонимы
 
     #: Псевдоним для :attr:`account_status`
     accountStatus = account_status
     #: Псевдоним для :attr:`account_settings`
     accountSettings = account_settings
@@ -2615,14 +2437,16 @@
     newReleases = new_releases
     #: Псевдоним для :attr:`new_playlists`
     newPlaylists = new_playlists
     #: Псевдоним для :attr:`tracks_download_info`
     tracksDownloadInfo = tracks_download_info
     #: Псевдоним для :attr:`track_supplement`
     trackSupplement = track_supplement
+    #: Псевдоним для :attr:`tracks_lyrics`
+    tracksLyrics = tracks_lyrics
     #: Псевдоним для :attr:`tracks_similar`
     tracksSimilar = tracks_similar
     #: Псевдоним для :attr:`play_audio`
     playAudio = play_audio
     #: Псевдоним для :attr:`albums_with_tracks`
     albumsWithTracks = albums_with_tracks
     #: Псевдоним для :attr:`search_suggest`
```

### Comparing `yandex-music-2.0.1/yandex_music/client_async.py` & `yandex-music-2.1.0/yandex_music/client_async.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ####################################################################
 # THIS IS AUTO GENERATED COPY OF client.py. DON'T EDIT IN BY HANDS #
 ####################################################################
 
 import functools
 import logging
 from datetime import datetime
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union, TypeVar, Callable, Any
 
 from yandex_music import (
     Album,
     Artist,
     ArtistAlbums,
     ArtistTracks,
     BriefInfo,
@@ -28,14 +28,15 @@
     ShotEvent,
     Supplement,
     StationResult,
     StationTracksResult,
     Status,
     Suggestions,
     SimilarTracks,
+    TrackLyrics,
     Track,
     TracksList,
     UserSettings,
     YandexMusicObject,
     ChartInfo,
     TagResult,
     PlaylistRecommendations,
@@ -45,30 +46,33 @@
     __copyright__,
     __license__,
     __version__,
 )
 from yandex_music.exceptions import BadRequestError
 from yandex_music.utils.difference import Difference
 from yandex_music.utils.request_async import Request
+from yandex_music.utils.sign_request import get_sign_request
 
 de_list = {
     'artist': Artist.de_list,
     'album': Album.de_list,
     'track': Track.de_list,
     'playlist': Playlist.de_list,
 }
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
+F = TypeVar('F', bound=Callable[..., Any])
 
-def log(method):
+
+def log(method: F) -> F:
     logger = logging.getLogger(method.__module__)
 
     @functools.wraps(method)
-    async def wrapper(*args, **kwargs):
+    async def wrapper(*args, **kwargs) -> Any:
         logger.debug(f'Entering: {method.__name__}')
 
         result = await method(*args, **kwargs)
         logger.debug(result)
 
         logger.debug(f'Exiting: {method.__name__}')
 
@@ -95,33 +99,33 @@
             которых нет в библиотеке.
 
     Args:
         token (:obj:`str`, optional): Уникальный ключ для аутентификации.
         base_url (:obj:`str`, optional): Ссылка на API Yandex Music.
         request (:obj:`yandex_music.utils.request.Request`, optional): Пре-инициализация
             :class:`yandex_music.utils.request.Request`.
-        language (:obj:`str`, optional): Язык, на котором будут приходить ответы от API.
+        language (:obj:`str`, optional): Язык, на котором будут приходить ответы от API. По умолчанию русский.
         report_unknown_fields (:obj:`bool`, optional): Включить предупреждения о неизвестных полях от API,
             которых нет в библиотеке.
     """
 
-    notice_displayed = False
+    __notice_displayed = False
 
     def __init__(
         self,
         token: str = None,
         base_url: str = None,
         request: Request = None,
         language: str = 'ru',
         report_unknown_fields=False,
     ) -> None:
-        if not ClientAsync.notice_displayed:
+        if not ClientAsync.__notice_displayed:
             print(f'Yandex Music API v{__version__}, {__copyright__}')
             print(f'Licensed under the terms of the {__license__}', end='\n\n')
-            ClientAsync.notice_displayed = True
+            ClientAsync.__notice_displayed = True
 
         self.logger = logging.getLogger(__name__)
         self.token = token
 
         if base_url is None:
             base_url = 'https://api.music.yandex.net'
 
@@ -153,480 +157,487 @@
     @log
     async def init(self):
         """Получение информацию об аккаунте использующихся в других запросах."""
         self.me = await self.account_status()
         return self
 
     @log
-    async def account_status(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Status]:
+    async def account_status(self, *args, **kwargs) -> Optional[Status]:
         """Получение статуса аккаунта. Нет обязательных параметров.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Status` | :obj:`None`: Информация об аккаунте если он валиден, иначе :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/account/status'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return Status.de_json(result, self)
 
     @log
-    async def account_settings(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[UserSettings]:
+    async def account_settings(self, *args, **kwargs) -> Optional[UserSettings]:
         """Получение настроек текущего пользователя.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.UserSettings` | :obj:`None`: Настройки пользователя если аккаунт валиден,
                 иначе :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/account/settings'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return UserSettings.de_json(result, self)
 
     @log
     async def account_settings_set(
         self,
         param: str = None,
         value: Union[str, int, bool] = None,
         data: Dict[str, Union[str, int, bool]] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[UserSettings]:
         """Изменение настроек текущего пользователя.
 
         Note:
             Доступные названия параметров есть поля в классе :class:`yandex_music.UserSettings`, только в CamelCase.
 
         Args:
             param (:obj:`str`): Название параметра для изменения.
             value (:obj:`str` | :obj:`int` | :obj:`bool`): Значение параметра.
             data (:obj:`dict`): Словарь параметров и значений для множественного изменения.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.UserSettings` | :obj:`None`: Настройки пользователя или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/account/settings'
 
         if not data:
             data = {param: str(value)}
 
-        # TODO (MarshalX) значения в data типа bool должны быть приведены к str при работе с async клиентом.
-
-        result = await self._request.post(url, data=data, timeout=timeout, *args, **kwargs)
+        result = await self._request.post(url, data, *args, **kwargs)
 
         return UserSettings.de_json(result, self)
 
     @log
-    async def settings(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Settings]:
+    async def settings(self, *args, **kwargs) -> Optional[Settings]:
         """Получение предложений по покупке. Нет обязательных параметров.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Settings` | :obj:`None`: Информацию о предлагаемых продуктах если аккаунт валиден
                 или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/settings'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return Settings.de_json(result, self)
 
     @log
-    async def permission_alerts(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[PermissionAlerts]:
+    async def permission_alerts(self, *args, **kwargs) -> Optional[PermissionAlerts]:
         """Получение оповещений. Нет обязательных параметров.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.PermissionAlerts` | :obj:`None`: Оповещения если аккаунт валиден или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/permission-alerts'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return PermissionAlerts.de_json(result, self)
 
     @log
-    async def account_experiments(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Experiments]:
+    async def account_experiments(self, *args, **kwargs) -> Optional[Experiments]:
         """Получение значений экспериментальных функций аккаунта.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Experiments` | :obj:`None`: Состояние экспериментальных функций или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/account/experiments'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return Experiments.de_json(result, self)
 
     @log
     async def consume_promo_code(
-        self, code: str, language: str = 'en', timeout: Union[int, float] = None, *args, **kwargs
+        self, code: str, language: Optional[str] = None, *args, **kwargs
     ) -> Optional[PromoCodeStatus]:
         """Активация промо-кода.
 
+        Note:
+            Доступные языки: en, uz, uk, us, ru, kk, hy.
+
         Args:
             code (:obj:`str`): Промо-код.
-            language (:obj:`str`, optional): Язык ответа API в ISO 639-1.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
+            language (:obj:`str`, optional): Язык ответа API в ISO 639-1. По умолчанию язык клиента.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.PromoCodeStatus` | :obj:`None`: Информация об активации промо-кода или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/account/consume-promo-code'
 
-        result = await self._request.post(url, {'code': code, 'language': language}, timeout=timeout, *args, **kwargs)
+        if not language:
+            language = self.language
+
+        result = await self._request.post(url, {'code': code, 'language': language}, *args, **kwargs)
 
         return PromoCodeStatus.de_json(result, self)
 
     @log
-    async def feed(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Feed]:
+    async def feed(self, *args, **kwargs) -> Optional[Feed]:
         """Получение потока информации (фида) подобранного под пользователя. Содержит умные плейлисты.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Feed` | :obj:`None`: Умные плейлисты пользователя или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/feed'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return Feed.de_json(result, self)
 
     @log
-    async def feed_wizard_is_passed(self, timeout: Union[int, float] = None, *args, **kwargs) -> bool:
+    async def feed_wizard_is_passed(self, *args, **kwargs) -> bool:
         url = f'{self.base_url}/feed/wizard/is-passed'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return result.get('is_wizard_passed') or False
 
     @log
-    async def landing(
-        self, blocks: Union[str, List[str]], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[Landing]:
+    async def landing(self, blocks: Union[str, List[str]], *args, **kwargs) -> Optional[Landing]:
         """Получение лендинг-страницы содержащий блоки с новыми релизами, чартами, плейлистами с новинками и т.д.
 
         Note:
             Поддерживаемые типы блоков: `personalplaylists`, `promotions`, `new-releases`, `new-playlists`, `mixes`,
             `chart`, `artists`, `albums`, `playlists`, `play_contexts`.
 
         Args:
             blocks (:obj:`str` | :obj:`list` из :obj:`str`): Блок или список блоков необходимых для выдачи.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Landing` | :obj:`None`: Лендинг-страница или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/landing3'
 
         result = await self._request.get(
-            url, {'blocks': blocks, 'eitherUserId': '10254713668400548221'}, timeout=timeout, *args, **kwargs
+            url, {'blocks': blocks, 'eitherUserId': '10254713668400548221'}, *args, **kwargs
         )
+        # TODO (MarshalX) что тут делает константа с чьим-то User ID
+        #  https://github.com/MarshalX/yandex-music-api/issues/553
 
         return Landing.de_json(result, self)
 
     @log
-    async def chart(
-        self, chart_option: str = '', timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[ChartInfo]:
+    async def chart(self, chart_option: str = '', *args, **kwargs) -> Optional[ChartInfo]:
         """Получение чарта.
 
         Note:
             `chart_option` - это постфикс к запросу из поля `menu` чарта.
             Например, на сайте можно выбрать глобальный (world) чарт или российский (russia).
 
         Args:
             chart_option (:obj:`str` optional): Параметры чарта.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.ChartInfo`: Чарт.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/landing3/chart'
 
         if chart_option:
             url = f'{url}/{chart_option}'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return ChartInfo.de_json(result, self)
 
     @log
-    async def new_releases(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[LandingList]:
+    async def new_releases(self, *args, **kwargs) -> Optional[LandingList]:
         """Получение полного списка всех новых релизов (альбомов).
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.LandingList`: Список новых альбомов.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/landing3/new-releases'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return LandingList.de_json(result, self)
 
     @log
-    async def new_playlists(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[LandingList]:
+    async def new_playlists(self, *args, **kwargs) -> Optional[LandingList]:
         """Получение полного списка всех новых плейлистов.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.LandingList`: Список новых плейлистов.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/landing3/new-playlists'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return LandingList.de_json(result, self)
 
     @log
-    async def podcasts(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[LandingList]:
+    async def podcasts(self, *args, **kwargs) -> Optional[LandingList]:
         """Получение подкастов с лендинга.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
-            :obj:`yandex_music.LandingList`: Список подскастов.
+            :obj:`yandex_music.LandingList`: Список подкастов.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/landing3/podcasts'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return LandingList.de_json(result, self)
 
     @log
-    async def genres(self, timeout: Union[int, float] = None, *args, **kwargs) -> List[Genre]:
+    async def genres(self, *args, **kwargs) -> List[Genre]:
         """Получение жанров музыки.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Genre` | :obj:`None`: Жанры музыки или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/genres'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return Genre.de_list(result, self)
 
     @log
-    async def tags(self, tag_id: str, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[TagResult]:
+    async def tags(self, tag_id: str, *args, **kwargs) -> Optional[TagResult]:
         """Получение тега (подборки).
 
         Note:
             Теги есть в `MixLink` у `Landing`, а также плейлистов в `.tags`.
 
             У `MixLink` есть `URL`, но `tag_id` только его последняя часть.
             Например, `/tag/belarus/`. `Tag` - `belarus`.
 
         Args:
             tag_id (:obj:`str`): Уникальный идентификатор тега.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
            :obj:`yandex_music.TagResult`: Тег с плейлистами.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/tags/{tag_id}/playlist-ids'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return TagResult.de_json(result, self)
 
     @log
     async def tracks_download_info(
         self,
         track_id: Union[str, int],
         get_direct_links: bool = False,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> List[DownloadInfo]:
         """Получение информации о доступных вариантах загрузки трека.
 
         Args:
             track_id (:obj:`str` | :obj:`list` из :obj:`str`): Уникальный идентификатор трека или треков.
             get_direct_links (:obj:`bool`, optional): Получить ли при вызове метода прямую ссылку на загрузку.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.DownloadInfo` | :obj:`None`: Варианты загрузки трека или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/tracks/{track_id}/download-info'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return await DownloadInfo.de_list_async(result, self, get_direct_links)
 
     @log
-    async def track_supplement(
-        self, track_id: Union[str, int], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[Supplement]:
+    async def track_supplement(self, track_id: Union[str, int], *args, **kwargs) -> Optional[Supplement]:
         """Получение дополнительной информации о треке.
 
+        Warning:
+            Получение текста из дополнительной информации устарело. Используйте
+            :func:`yandex_music.ClientAsync.tracks_lyrics`.
+
         Args:
-            track_id (:obj:`str`): Уникальный идентификатор трека.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
+            track_id (:obj:`str` | :obj:`int`): Уникальный идентификатор трека.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Supplement`: Дополнительная информация о треке.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/tracks/{track_id}/supplement'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return Supplement.de_json(result, self)
 
     @log
-    async def tracks_similar(
-        self, track_id: Union[str, int], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[SimilarTracks]:
+    async def tracks_lyrics(
+        self,
+        track_id: Union[str, int],
+        format: str = 'TEXT',
+        **kwargs,
+    ) -> Optional[TrackLyrics]:
+        """Получение текста трека.
+
+        Note:
+            Для работы с методом необходима авторизация.
+
+            Известные значения для аргумента format:
+                - `LRC` - формат с временными метками.
+                - `TEXT` - простой текст.
+
+        Args:
+            track_id (:obj:`str` | :obj:`int`): Уникальный идентификатор трека.
+            format (:obj:`str`): Формат текста.
+            **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
+
+        Returns:
+            :obj:`yandex_music.TrackLyrics` | :obj:`None`: Информация о тексте трека.
+
+        Raises:
+            :class:`yandex_music.exceptions.UnauthorizedError`: Метод вызван без авторизации.
+            :class:`yandex_music.exceptions.NotFoundError`: Текст у трека отсутствует.
+            :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
+        """
+
+        url = f'{self.base_url}/tracks/{track_id}/lyrics'
+
+        sign = get_sign_request(track_id)
+        params = {
+            'format': format,
+            'timeStamp': sign.timestamp,
+            'sign': sign.value,
+        }
+
+        result = await self._request.get(url, params=params, **kwargs)
+
+        return TrackLyrics.de_json(result, self)
+
+    @log
+    async def tracks_similar(self, track_id: Union[str, int], *args, **kwargs) -> Optional[SimilarTracks]:
         """Получение похожих треков.
 
         Args:
-            track_id (:obj:`str`): Уникальный идентификатор трека.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
+            track_id (:obj:`str` | :obj:`int`): Уникальный идентификатор трека.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.SimilarTracks`: Похожие треки на другой трек.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/tracks/{track_id}/similar'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return SimilarTracks.de_json(result, self)
 
     @log
     async def play_audio(
         self,
         track_id: Union[str, int],
@@ -637,15 +648,14 @@
         play_id: str = None,
         uid: int = None,
         timestamp: str = None,
         track_length_seconds: int = 0,
         total_played_seconds: int = 0,
         end_position_seconds: int = 0,
         client_now: str = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> bool:
         """Метод для отправки текущего состояния прослушиваемого трека.
 
         Args:
             track_id (:obj:`str` | :obj:`int`): Уникальный идентификатор трека.
@@ -656,16 +666,14 @@
             play_id (:obj:`str`, optional): Уникальный идентификатор проигрывания.
             uid (:obj:`int`, optional): Уникальный идентификатор пользователя.
             timestamp (:obj:`str`, optional): Текущая дата и время в ISO.
             track_length_seconds (:obj:`int`, optional): Продолжительность трека в секундах.
             total_played_seconds (:obj:`int`, optional): Сколько было всего воспроизведено трека в секундах.
             end_position_seconds (:obj:`int`, optional): Окончательное значение воспроизведенных секунд.
             client_now (:obj:`str`, optional): Текущая дата и время клиента в ISO.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -687,52 +695,47 @@
             'total-played-seconds': total_played_seconds,
             'end-position-seconds': end_position_seconds,
             'album-id': album_id,
             'playlist-id': playlist_id,
             'client-now': client_now or f'{datetime.now().isoformat()}Z',
         }
 
-        result = await self._request.post(url, data, timeout=timeout, *args, **kwargs)
+        result = await self._request.post(url, data, *args, **kwargs)
 
         return result == 'ok'
 
     @log
-    async def albums_with_tracks(
-        self, album_id: Union[str, int], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[Album]:
+    async def albums_with_tracks(self, album_id: Union[str, int], *args, **kwargs) -> Optional[Album]:
         """Получение альбома по его уникальному идентификатору вместе с треками.
 
         Args:
             album_id (:obj:`str` | :obj:`int`): Уникальный идентификатор альбома.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Album` | :obj:`None`: Альбом или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/albums/{album_id}/with-tracks'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return Album.de_json(result, self)
 
     @log
     async def search(
         self,
         text: str,
         nocorrect: bool = False,
         type_: str = 'all',
         page: int = 0,
         playlist_in_best: bool = True,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[Search]:
         """Осуществление поиска по запросу и типу, получение результатов.
 
         Note:
             Известные значения для поля `type_`: `all`, `artist`, `user`, `album`, `playlist`, `track`, `podcast`,
@@ -743,16 +746,14 @@
         Args:
             text (:obj:`str`): Текст запроса.
             nocorrect (:obj:`bool`): Если :obj:`False`, то ошибочный запрос будет исправлен. Например, запрос
                 "Гражданская абарона" будет исправлен на "Гражданская оборона".
             type_ (:obj:`str`): Среди какого типа искать (трек, плейлист, альбом, исполнитель, пользователь, подкаст).
             page (:obj:`int`): Номер страницы.
             playlist_in_best (:obj:`bool`): Выдавать ли плейлисты лучшим вариантом поиска.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Search` | :obj:`None`: Результаты поиска или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -764,98 +765,87 @@
             'text': text,
             'nocorrect': str(nocorrect),
             'type': type_,
             'page': page,
             'playlist-in-best': str(playlist_in_best),
         }
 
-        result = await self._request.get(url, params, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, params, *args, **kwargs)
 
         if isinstance(result, str):
             raise BadRequestError(result)
 
         return Search.de_json(result, self)
 
     @log
-    async def search_suggest(
-        self, part: str, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[Suggestions]:
+    async def search_suggest(self, part: str, *args, **kwargs) -> Optional[Suggestions]:
         """Получение подсказок по введенной части поискового запроса.
 
         Args:
             part (:obj:`str`): Часть поискового запроса.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Suggestions` | :obj:`None`: Подсказки для запроса или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/search/suggest'
 
-        result = await self._request.get(url, {'part': part}, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, {'part': part}, *args, **kwargs)
 
         return Suggestions.de_json(result, self)
 
     @log
-    async def users_settings(
-        self, user_id: Union[str, int] = None, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[UserSettings]:
+    async def users_settings(self, user_id: Union[str, int] = None, *args, **kwargs) -> Optional[UserSettings]:
         """Получение настроек пользователя.
 
         Note:
             Для получения настроек пользователя нужно быть авторизованным или владеть `user_id`.
 
         Args:
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя чьи настройки хотим
                 получить.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.UserSettings` | :obj:`None`: Настройки пользователя или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/settings'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return UserSettings.de_json(result.get('user_settings'), self)
 
     @log
     async def users_playlists(
         self,
         kind: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Union[Playlist, List[Playlist]]:
         """Получение плейлиста или списка плейлистов по уникальным идентификаторам.
 
         Note:
             Если передан один `kind`, то вернётся не список плейлистов, а один плейлист.
 
         Args:
             kind (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста
                 или их список.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Playlist` | :obj:`yandex_music.Playlist` | :obj:`None`:
             Список плейлистов или плейлист, иначе :obj:`None`.
 
         Raises:
@@ -866,69 +856,64 @@
             user_id = self.me.account.uid
 
         if isinstance(kind, list):
             url = f'{self.base_url}/users/{user_id}/playlists'
 
             data = {'kinds': kind}
 
-            result = await self._request.post(url, data, timeout=timeout, *args, **kwargs)
+            result = await self._request.post(url, data, *args, **kwargs)
 
             return Playlist.de_list(result, self)
         else:
             url = f'{self.base_url}/users/{user_id}/playlists/{kind}'
-            result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+            result = await self._request.get(url, *args, **kwargs)
 
             return Playlist.de_json(result, self)
 
     @log
     async def users_playlists_recommendations(
-        self, kind: Union[str, int], user_id: Union[str, int] = None, timeout: Union[int, float] = None, *args, **kwargs
+        self, kind: Union[str, int], user_id: Union[str, int] = None, *args, **kwargs
     ):
         """Получение рекомендаций для плейлиста.
 
         Args:
             kind (:obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста.
             user_id (:obj:`str` | :obj:`int`): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.PlaylistRecommendations` | :obj:`None`: Рекомендации для плейлиста или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/playlists/{kind}/recommendations'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return PlaylistRecommendations.de_json(result, self)
 
     @log
     async def users_playlists_create(
         self,
         title: str,
         visibility: str = 'public',
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[Playlist]:
         """Создание плейлиста.
 
         Args:
             title (:obj:`str`): Название.
             visibility (:obj:`str`, optional): Модификатор доступа.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Playlist` | :obj:`None`: Созданный плейлист или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -937,130 +922,121 @@
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/playlists/create'
 
         data = {'title': title, 'visibility': visibility}
 
-        result = await self._request.post(url, data, timeout=timeout, *args, **kwargs)
+        result = await self._request.post(url, data, *args, **kwargs)
 
         return Playlist.de_json(result, self)
 
     @log
     async def users_playlists_delete(
-        self, kind: Union[str, int], user_id: Union[str, int] = None, timeout: Union[int, float] = None, *args, **kwargs
+        self, kind: Union[str, int], user_id: Union[str, int] = None, *args, **kwargs
     ) -> bool:
         """Удаление плейлиста.
 
         Args:
             kind (:obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/playlists/{kind}/delete'
 
-        result = await self._request.post(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.post(url, *args, **kwargs)
 
         return result == 'ok'
 
     @log
     async def users_playlists_name(
         self,
         kind: Union[str, int],
         name: str,
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[Playlist]:
         """Изменение названия плейлиста.
 
         Args:
             kind (:obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста.
             name (:obj:`str`): Новое название.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Playlist` | :obj:`None`: Изменённый плейлист или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/playlists/{kind}/name'
 
-        result = await self._request.post(url, {'value': name}, timeout=timeout, *args, **kwargs)
+        result = await self._request.post(url, {'value': name}, *args, **kwargs)
 
         return Playlist.de_json(result, self)
 
     @log
     async def users_playlists_visibility(
         self,
         kind: Union[str, int],
         visibility: str,
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[Playlist]:
         """Изменение видимости плейлиста.
 
         Note:
             Видимость (`visibility`) может быть задана только одним из двух значений: `private`, `public`.
 
         Args:
             kind (:obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста.
             visibility (:obj:`str`): Новое название.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Playlist` | :obj:`None`: Изменённый плейлист или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/playlists/{kind}/visibility'
 
-        result = await self._request.post(url, {'value': visibility}, timeout=timeout, *args, **kwargs)
+        result = await self._request.post(url, {'value': visibility}, *args, **kwargs)
 
         return Playlist.de_json(result, self)
 
     @log
     async def users_playlists_change(
         self,
         kind: Union[str, int],
         diff: str,
         revision: int = 1,
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[Playlist]:
         """Изменение плейлиста.
 
         Note:
             Для получения отличий есть вспомогательный класс :class:`yandex_music.utils.difference.Difference`.
@@ -1068,16 +1044,14 @@
             Так же существуют уже готовые методы-обёртки над операциями.
 
         Args:
             kind (:obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста.
             revision (:obj:`int`): TODO.
             diff (:obj:`str`): JSON представления отличий старого и нового плейлиста.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Playlist`: Изменённый плейлист или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -1086,28 +1060,27 @@
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/playlists/{kind}/change'
 
         data = {'kind': kind, 'revision': revision, 'diff': diff}
 
-        result = await self._request.post(url, data, timeout=timeout, *args, **kwargs)
+        result = await self._request.post(url, data, *args, **kwargs)
 
         return Playlist.de_json(result, self)
 
     @log
     async def users_playlists_insert_track(
         self,
         kind: Union[str, int],
         track_id: Union[str, int],
         album_id: Union[str, int],
         at: int = 0,
         revision: int = 1,
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[Playlist]:
         """Добавление трека в плейлист.
 
         Note:
             Трек можно вставить с любое место плейлиста задав индекс вставки (аргумент `at`).
@@ -1115,186 +1088,174 @@
         Args:
             kind (:obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста.
             track_id (:obj:`str` | :obj:`int`): Уникальный идентификатор трека.
             album_id (:obj:`str` | :obj:`int`): Уникальный идентификатор альбома.
             at (:obj:`int`): Индекс для вставки.
             revision (:obj:`int`): TODO.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Playlist`: Изменённый плейлист или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         diff = Difference().add_insert(at, {'id': track_id, 'album_id': album_id})
 
-        return await self.users_playlists_change(kind, diff.to_json(), revision, user_id, timeout, *args, **kwargs)
+        return await self.users_playlists_change(kind, diff.to_json(), revision, user_id, *args, **kwargs)
 
     @log
     async def users_playlists_delete_track(
         self,
         kind: Union[str, int],
         from_: int,
         to: int,
         revision: int = 1,
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[Playlist]:
         """Удаление треков из плейлиста.
 
         Note:
             Для удаление необходимо указать границы с какого по какой элемент (трек) удалить.
 
         Args:
             kind (:obj:`str` | :obj:`int`): Уникальный идентификатор плейлиста.
             from_ (:obj:`int`): С какого индекса.
             to (:obj:`int`): По какой индекс.
             revision (:obj:`int`): TODO.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя владеющим плейлистом.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Playlist` | :obj:`None`: Изменённый плейлист или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         diff = Difference().add_delete(from_, to)
 
-        return await self.users_playlists_change(kind, diff.to_json(), revision, user_id, timeout, *args, **kwargs)
+        return await self.users_playlists_change(kind, diff.to_json(), revision, user_id, *args, **kwargs)
 
     @log
-    async def rotor_account_status(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Status]:
-        """Получение статуса пользователя с дополнителньыми полями.
+    async def rotor_account_status(self, *args, **kwargs) -> Optional[Status]:
+        """Получение статуса пользователя с дополнительными полями.
 
         Note:
             Данный статус отличается от обычного наличием дополнительных полей, например, `skips_per_hour`.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Status` | :obj:`None`: Статус пользователя с дополнительными полями от радио или
                 :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/rotor/account/status'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return Status.de_json(result, self)
 
     @log
-    async def rotor_stations_dashboard(self, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Dashboard]:
+    async def rotor_stations_dashboard(self, *args, **kwargs) -> Optional[Dashboard]:
         """Получение рекомендованных станций текущего пользователя.
 
         Args:
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Dashboard` | :obj:`None`: Рекомендованные станции или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/rotor/stations/dashboard'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return Dashboard.de_json(result, self)
 
     @log
-    async def rotor_stations_list(
-        self, language: str = 'ru', timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[StationResult]:
+    async def rotor_stations_list(self, language: Optional[str] = None, *args, **kwargs) -> List[StationResult]:
         """Получение всех радиостанций с настройками пользователя.
 
         Note:
+            Доступные языки: en, uz, uk, us, ru, kk, hy.
+
             Чтобы определить что за тип станции (жанры, настроения, занятие и т.д.) необходимо смотреть в поле
             `id_for_from`.
 
         Args:
-            language (:obj:`str`): Язык, на котором будет информация о станциях.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
+            language (:obj:`str`, optional): Язык, на котором будет информация о станциях. По умолчанию язык клиента.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
-            :obj:`list` из :obj:`yandex_music.StationResult` | :obj:`None`: Станции или :obj:`None`.
+            :obj:`list` из :obj:`yandex_music.StationResult`: Список станций.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/rotor/stations/list'
 
-        result = await self._request.get(url, {'language': language}, timeout=timeout, *args, **kwargs)
+        if not language:
+            language = self.language
+
+        result = await self._request.get(url, {'language': language}, *args, **kwargs)
 
         return StationResult.de_list(result, self)
 
     @log
     async def rotor_station_feedback(
         self,
         station: str,
         type_: str,
         timestamp: Union[str, float, int] = None,
         from_: str = None,
         batch_id: str = None,
         total_played_seconds: Union[int, float] = None,
         track_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
-        """Отправка ответной реакции на происходящее при прослушивании радио.
+        """Отправка обратной связи на действия при прослушивании радио.
 
         Note:
             Сообщения о начале прослушивания радио, начале и конце трека, его пропуска.
 
-            Известные типы фидбека: `radioStarted`, `trackStarted`, `trackFinished`, `skip`.
+            Известные типы обратной связи: `radioStarted`, `trackStarted`, `trackFinished`, `skip`.
 
             Пример `station`: `user:onyourwave`, `genre:allrock`.
 
             Пример `from_`: `mobile-radio-user-123456789`.
 
         Args:
             station (:obj:`str`): Станция.
-            type_ (:obj:`str`): Тип отправляемого фидбека.
+            type_ (:obj:`str`): Тип отправляемого отзыва.
             timestamp (:obj:`str` | :obj:`float` | :obj:`int`, optional): Текущее время и дата.
             from_ (:obj:`str`, optional): Откуда начато воспроизведение радио.
             batch_id (:obj:`str`, optional): Уникальный идентификатор партии треков. Возвращается при получении треков.
             total_played_seconds (:obj:`int` |:obj:`float`, optional): Сколько было проиграно секунд трека
                 перед действием.
             track_id (:obj:`int` | :obj:`str`, optional): Уникальной идентификатор трека.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -1316,173 +1277,156 @@
 
         if from_:
             data.update({'from': from_})
 
         if total_played_seconds:
             data.update({'totalPlayedSeconds': total_played_seconds})
 
-        result = await self._request.post(url, params=params, json=data, timeout=timeout, *args, **kwargs)
+        result = await self._request.post(url, params=params, json=data, **kwargs)
 
         return result == 'ok'
 
     @log
     async def rotor_station_feedback_radio_started(
         self,
         station: str,
         from_: str,
         batch_id: str = None,
         timestamp: Union[str, float, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Сокращение для::
 
-            client.rotor_station_feedback(station, 'radioStarted', timestamp, from, *args, **kwargs)
+            client.rotor_station_feedback(station, 'radioStarted', timestamp, from, batch_id, **kwargs)
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         return await self.rotor_station_feedback(
-            station, 'radioStarted', timestamp, from_=from_, batch_id=batch_id, timeout=timeout, *args, **kwargs
+            station, 'radioStarted', timestamp, from_=from_, batch_id=batch_id, **kwargs
         )
 
     @log
     async def rotor_station_feedback_track_started(
         self,
         station: str,
         track_id: Union[str, int],
         batch_id: str = None,
         timestamp: Union[str, float, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Сокращение для::
 
-            client.rotor_station_feedback(station, 'trackStarted', timestamp, track_id, *args, **kwargs)
+            client.rotor_station_feedback(station, 'trackStarted', timestamp, track_id=track_id,
+            batch_id=batch_id, **kwargs)
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         return await self.rotor_station_feedback(
-            station, 'trackStarted', timestamp, track_id=track_id, batch_id=batch_id, timeout=timeout, *args, **kwargs
+            station, 'trackStarted', timestamp, track_id=track_id, batch_id=batch_id, **kwargs
         )
 
     @log
     async def rotor_station_feedback_track_finished(
         self,
         station: str,
         track_id: Union[str, int],
         total_played_seconds: float,
         batch_id: str = None,
         timestamp: Union[str, float, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Сокращение для::
 
-            client.rotor_station_feedback(station, 'trackFinished', timestamp, track_id, total_played_seconds,
-            *args, **kwargs)
+            client.rotor_station_feedback(station, 'trackFinished', timestamp,
+            track_id=track_id, total_played_seconds=total_played_seconds, batch_id=batch_id, **kwargs)
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         return await self.rotor_station_feedback(
             station,
             'trackFinished',
             timestamp,
             track_id=track_id,
             total_played_seconds=total_played_seconds,
             batch_id=batch_id,
-            timeout=timeout,
-            *args,
             **kwargs,
         )
 
     @log
     async def rotor_station_feedback_skip(
         self,
         station: str,
         track_id: Union[str, int],
         total_played_seconds: float,
         batch_id: str = None,
         timestamp: Union[str, float, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Сокращение для::
 
-            client.rotor_station_feedback(station, 'skip', timestamp, track_id, total_played_seconds,
-            *args, **kwargs)
+            client.rotor_station_feedback(station, 'skip', timestamp, track_id=track_id,
+            total_played_seconds=total_played_seconds, batch_id=batch_id, **kwargs)
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         return await self.rotor_station_feedback(
             station,
             'skip',
             timestamp,
             track_id=track_id,
             total_played_seconds=total_played_seconds,
             batch_id=batch_id,
-            timeout=timeout,
-            *args,
             **kwargs,
         )
 
     @log
-    async def rotor_station_info(
-        self, station: str, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[StationResult]:
+    async def rotor_station_info(self, station: str, *args, **kwargs) -> List[StationResult]:
         """Получение информации о станции и пользовательских настроек на неё.
 
         Args:
             station (:obj:`str`): Станция.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.StationResult` | :obj:`None`: Информация о станции или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/rotor/station/{station}/info'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return StationResult.de_list(result, self)
 
     @log
     async def rotor_station_settings2(
         self,
         station: str,
         mood_energy: str,
         diversity: str,
-        language: str = 'not-russian',
+        language: str = 'not-russian',  # TODO(#555): заменить на any
         type_: str = 'rotor',
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Изменение настроек определённой станции.
 
         Note:
             Доступные значения для `mood_energy`: `fun`, `active`, `calm`, `sad`, `all`.
 
@@ -1496,16 +1440,14 @@
 
         Args:
             station (:obj:`str`): Станция.
             mood_energy (:obj:`str`): Настроение.
             diversity (:obj:`str`): Треки.
             language (:obj:`str`): Язык.
             type_ (:obj:`str`): Тип.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -1514,51 +1456,48 @@
         url = f'{self.base_url}/rotor/station/{station}/settings3'
 
         data = {'moodEnergy': mood_energy, 'diversity': diversity, 'type': type_}
 
         if language:
             data.update({'language': language})
 
-        result = await self._request.post(url, json=data, timeout=timeout, *args, **kwargs)
+        result = await self._request.post(url, json=data, **kwargs)
 
         return result == 'ok'
 
     @log
     async def rotor_station_tracks(
         self,
         station: str,
         settings2: bool = True,
         queue: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[StationTracksResult]:
         """Получение цепочки треков определённой станции.
 
         Note:
             Запуск потока по сущности сервиса осуществляется через станцию `<type>:<id>`.
             Например, станцией для запуска потока по треку будет `track:1234`.
 
             Для продолжения цепочки треков необходимо:
 
             1. Передавать `ID` трека, что был до этого (первый в цепочки).
-            2. Отправить фидбек о конче или скипе трека, что был передан в `queue`.
+            2. Отправить фидбек о конце или скипе трека, что был передан в `queue`.
             3. Отправить фидбек о начале следующего трека (второй в цепочки).
             4. Выполнить запрос получения треков. В ответе придёт новые треки или произойдёт сдвиг цепочки на 1 элемент.
 
-            Проход по цепочке до коцна не изучен. Часто встречаются дубликаты.
+            Проход по цепочке до конца не изучен. Часто встречаются дубликаты.
 
             Все официальные клиенты выполняют запросы с `settings2 = True`.
 
         Args:
             station (:obj:`str`): Станция.
             settings2 (:obj:`bool`, optional): Использовать ли второй набор настроек.
             queue (:obj:`str` | :obj:`int` , optional): Уникальной идентификатор трека, который только что был.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.StationTracksResult` | :obj:`None`: Последовательность треков станции или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -1569,124 +1508,113 @@
         params = {}
         if settings2:
             params = {'settings2': str(True)}
 
         if queue:
             params = {'queue': queue}
 
-        result = await self._request.get(url, params=params, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, params, *args, **kwargs)
 
         return StationTracksResult.de_json(result, self)
 
     @log
-    async def artists_brief_info(
-        self, artist_id: Union[str, int], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[BriefInfo]:
+    async def artists_brief_info(self, artist_id: Union[str, int], *args, **kwargs) -> Optional[BriefInfo]:
         """Получение информации об артисте.
 
         Args:
             artist_id (:obj:`str` | :obj:`int`): Уникальный идентификатор исполнителя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.BriefInfo` | :obj:`None`: Информация об артисте или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         url = f'{self.base_url}/artists/{artist_id}/brief-info'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return BriefInfo.de_json(result, self)
 
     @log
     async def artists_tracks(
         self,
         artist_id: Union[str, int],
         page: int = 0,
         page_size: int = 20,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[ArtistTracks]:
         """Получение треков артиста.
 
         Args:
             artist_id (:obj:`str` | :obj:`int`): Уникальный идентификатор артиста.
             page (:obj:`int`, optional): Номер страницы.
             page_size (:obj:`int`, optional): Количество треков на странице.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.ArtistsTracks` | :obj:`None`: Страница списка треков артиста или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/artists/{artist_id}/tracks'
 
         params = {'page': page, 'page-size': page_size}
 
-        result = await self._request.get(url, params, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, params, *args, **kwargs)
 
         return ArtistTracks.de_json(result, self)
 
     @log
     async def artists_direct_albums(
         self,
         artist_id: Union[str, int],
         page: int = 0,
         page_size: int = 20,
         sort_by: str = 'year',
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[ArtistAlbums]:
         """Получение альбомов артиста.
 
         Note:
             Известные значения для `sort_by`: `year`, `rating`.
 
         Args:
             artist_id (:obj:`str` | :obj:`int`): Уникальный идентификатор артиста.
             page (:obj:`int`, optional): Номер страницы.
             page_size (:obj:`int`, optional): Количество альбомов на странице.
             sort_by (:obj:`str`, optional): Параметр для сортировки.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.ArtistAlbums` | :obj:`None`: Страница списка альбомов артиста или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
 
         url = f'{self.base_url}/artists/{artist_id}/direct-albums'
 
         params = {'sort-by': sort_by, 'page': page, 'page-size': page_size}
 
-        result = await self._request.get(url, params, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, params, *args, **kwargs)
 
         return ArtistAlbums.de_json(result, self)
 
     async def _like_action(
         self,
         object_type: str,
         ids: Union[List[Union[str, int]], str, int],
         remove: bool = False,
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> bool:
         """Действия с отметкой "Мне нравится".
 
         Note:
             Типы объектов: `track` - трек, `artist` - исполнитель, `playlist` - плейлист, `album` - альбом.
@@ -1697,290 +1625,253 @@
         Args:
             object_type (:obj:`str`): Тип объекта.
             ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор объекта или объектов.
             remove (:obj:`bool`, optional): Если :obj:`True` то снимает отметку, иначе ставит.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         action = 'remove' if remove else 'add-multiple'
         url = f'{self.base_url}/users/{user_id}/likes/{object_type}s/{action}'
 
-        result = await self._request.post(url, {f'{object_type}-ids': ids}, timeout=timeout, *args, **kwargs)
+        result = await self._request.post(url, {f'{object_type}-ids': ids}, *args, **kwargs)
 
         if object_type == 'track':
             return 'revision' in result
 
         return result == 'ok'
 
     @log
     async def users_likes_tracks_add(
         self,
         track_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Поставить отметку "Мне нравится" треку/трекам.
 
         Note:
             Так же снимает отметку "Не рекомендовать" если она есть.
 
         Args:
             track_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор трека или треков.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._like_action('track', track_ids, False, user_id, timeout, *args, **kwargs)
+        return await self._like_action('track', track_ids, remove=False, user_id=user_id, **kwargs)
 
     @log
     async def users_likes_tracks_remove(
         self,
         track_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Снять отметку "Мне нравится" у трека/треков.
 
         Args:
             track_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор трека или треков.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._like_action('track', track_ids, True, user_id, timeout, *args, **kwargs)
+        return await self._like_action('track', track_ids, remove=True, user_id=user_id, **kwargs)
 
     @log
     async def users_likes_artists_add(
         self,
         artist_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Поставить отметку "Мне нравится" исполнителю/исполнителям.
 
         Args:
             artist_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор артиста или артистов.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._like_action('artist', artist_ids, False, user_id, timeout, *args, **kwargs)
+        return await self._like_action('artist', artist_ids, remove=False, user_id=user_id, **kwargs)
 
     @log
     async def users_likes_artists_remove(
         self,
         artist_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Снять отметку "Мне нравится" у исполнителя/исполнителей.
 
         Args:
             artist_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор артиста или артистов.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._like_action('artist', artist_ids, True, user_id, timeout, *args, **kwargs)
+        return await self._like_action('artist', artist_ids, remove=True, user_id=user_id, **kwargs)
 
     @log
     async def users_likes_playlists_add(
         self,
         playlist_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Поставить отметку "Мне нравится" плейлисту/плейлистам.
 
         Note:
             Идентификатор плейлиста указывается в формате `owner_id:playlist_id`. Где `playlist_id` - идентификатор
             плейлиста, `owner_id` - уникальный идентификатор владельца плейлиста.
 
         Args:
             playlist_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор плейлиста или плейлистов.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._like_action('playlist', playlist_ids, False, user_id, timeout, *args, **kwargs)
+        return await self._like_action('playlist', playlist_ids, remove=False, user_id=user_id, **kwargs)
 
     @log
     async def users_likes_playlists_remove(
         self,
         playlist_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Снять отметку "Мне нравится" у плейлиста/плейлистов.
 
         Note:
             Идентификатор плейлиста указывается в формате `owner_id:playlist_id`. Где `playlist_id` - идентификатор
             плейлиста, `owner_id` - уникальный идентификатор владельца плейлиста.
 
         Args:
             playlist_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор плейлиста или плейлистов.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._like_action('playlist', playlist_ids, True, user_id, timeout, *args, **kwargs)
+        return await self._like_action('playlist', playlist_ids, remove=True, user_id=user_id, **kwargs)
 
     @log
     async def users_likes_albums_add(
         self,
         album_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Поставить отметку "Мне нравится" альбому/альбомам.
 
         Args:
             album_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор артиста или артистов.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._like_action('album', album_ids, False, user_id, timeout, *args, **kwargs)
+        return await self._like_action('album', album_ids, remove=False, user_id=user_id, **kwargs)
 
     @log
     async def users_likes_albums_remove(
         self,
         album_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Снять отметку "Мне нравится" у альбома/альбомов.
 
         Args:
             album_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор артиста или артистов.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._like_action('album', album_ids, True, user_id, timeout, *args, **kwargs)
+        return await self._like_action('album', album_ids, remove=True, user_id=user_id, **kwargs)
 
     async def _get_list(
         self,
         object_type: str,
         ids: Union[List[Union[str, int]], int, str],
         params: dict = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> List[Union[Artist, Album, Track, Playlist]]:
         """Получение объекта/объектов.
 
         Args:
             object_type (:obj:`str`): Тип объекта.
             ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор объекта или объектов.
             params (:obj:`dict`, optional): Параметры, которые будут переданы в запрос.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Artist` | :obj:`list` из :obj:`yandex_music.Album` |
                 :obj:`list` из :obj:`yandex_music.Track` | :obj:`list` из :obj:`yandex_music.Playlist`: Запрошенный
                 объект.
 
@@ -1989,456 +1880,408 @@
         """
         if params is None:
             params = {}
         params.update({f'{object_type}-ids': ids})
 
         url = f'{self.base_url}/{object_type}s' + ('/list' if object_type == 'playlist' else '')
 
-        result = await self._request.post(url, params, timeout=timeout, *args, **kwargs)
+        result = await self._request.post(url, params, *args, **kwargs)
 
         return de_list[object_type](result, self)
 
     @log
-    async def artists(
-        self, artist_ids: Union[List[Union[str, int]], int, str], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[Artist]:
+    async def artists(self, artist_ids: Union[List[Union[str, int]], int, str], *args, **kwargs) -> List[Artist]:
         """Получение исполнителя/исполнителей.
 
         Args:
             artist_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор исполнителя или исполнителей.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Artist`: Исполнитель или исполнители.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._get_list('artist', artist_ids, timeout=timeout, *args, **kwargs)
+        return await self._get_list('artist', artist_ids, *args, **kwargs)
 
     @log
-    async def albums(
-        self, album_ids: Union[List[Union[str, int]], int, str], timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[Album]:
+    async def albums(self, album_ids: Union[List[Union[str, int]], int, str], *args, **kwargs) -> List[Album]:
         """Получение альбома/альбомов.
 
         Args:
             album_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор альбома или альбомов.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Album`: Альбом или альбомы.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._get_list('album', album_ids, timeout=timeout, *args, **kwargs)
+        return await self._get_list('album', album_ids, *args, **kwargs)
 
     @log
     async def tracks(
         self,
         track_ids: Union[List[Union[str, int]], int, str],
         with_positions: bool = True,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> List[Track]:
         """Получение трека/треков.
 
         Args:
             track_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор трека или треков.
             with_positions (:obj:`bool`, optional): С позициями TODO.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Track`: Трек или Треки.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._get_list(
-            'track', track_ids, {'with-positions': str(with_positions)}, timeout, *args, **kwargs
-        )
+        return await self._get_list('track', track_ids, {'with-positions': str(with_positions)}, *args, **kwargs)
 
     @log
     async def playlists_list(
-        self, playlist_ids: Union[List[Union[str, int]], int, str], timeout: Union[int, float] = None, *args, **kwargs
+        self, playlist_ids: Union[List[Union[str, int]], int, str], *args, **kwargs
     ) -> List[Playlist]:
         """Получение плейлиста/плейлистов.
 
         Note:
             Идентификатор плейлиста указывается в формате `owner_id:playlist_id`. Где `playlist_id` - идентификатор
             плейлиста, `owner_id` - уникальный идентификатор владельца плейлиста.
 
+            Данный метод возвращает сокращенную модель плейлиста для отображения больших список.
+
+        Warning:
+            Данный метод не возвращает список треков у плейлиста! Для получения объекта :obj:`yandex_music.Playlist` c
+            заполненным полем `tracks` используйте метод :func:`yandex_music.ClientAsync.users_playlists` или
+            метод :func:`yandex_music.Playlist.fetch_tracks`.
+
         Args:
             playlist_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор плейлиста или плейлистов.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Playlist`: Плейлист или плейлисты.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._get_list('playlist', playlist_ids, timeout=timeout, *args, **kwargs)
+        return await self._get_list('playlist', playlist_ids, *args, **kwargs)
 
     @log
-    async def playlists_collective_join(
-        self, user_id: int, token: str, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> bool:
+    async def playlists_collective_join(self, user_id: int, token: str, **kwargs) -> bool:
         """Присоединение к плейлисту как соавтор.
 
         Note:
             В качестве `user_id` принимается исключительно числовой уникальный идентификатор пользователя, не username.
 
             Токен можно получить в Web-версии. Для этого, на странице плейлиста нужно нажать на
             "Добавить соавтора". В полученной ссылке GET параметр `token` и будет токеном для присоединения.
 
         Args:
             user_id (:obj:`int`): Владелец плейлиста.
             token (:obj:`str`): Токен для присоединения.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs: Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         url = f'{self.base_url}/playlists/collective/join'
 
         params = {'uid': user_id, 'token': token}
 
-        result = await self._request.post(url, params=params, timeout=timeout, *args, **kwargs)
+        result = await self._request.post(url, params=params, **kwargs)
 
         return result == 'ok'
 
     @log
-    async def users_playlists_list(
-        self, user_id: Union[str, int] = None, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[Playlist]:
+    async def users_playlists_list(self, user_id: Union[str, int] = None, *args, **kwargs) -> List[Playlist]:
         """Получение списка плейлистов пользователя.
 
         Args:
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Playlist`: Плейлисты пользователя.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/playlists/list'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return Playlist.de_list(result, self)
 
     async def _get_likes(
         self,
         object_type: str,
         user_id: Union[str, int] = None,
         params: dict = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Union[List[Like], Optional[TracksList]]:
         """Получение объектов с отметкой "Мне нравится".
 
         Args:
             object_type (:obj:`str`): Тип объекта.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
             params (:obj:`dict`, optional): Параметры, которые будут переданы в запрос.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Like` | :obj:`yandex_music.TracksList`: Объекты с отметкой "Мне нравится".
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/likes/{object_type}s'
 
-        result = await self._request.get(url, params, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, params, *args, **kwargs)
 
         if object_type == 'track':
             return TracksList.de_json(result.get('library'), self)
 
         return Like.de_list(result, self, object_type)
 
     @log
     async def users_likes_tracks(
         self,
         user_id: Union[str, int] = None,
         if_modified_since_revision: int = 0,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[TracksList]:
         """Получение треков с отметкой "Мне нравится".
 
         Args:
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
             if_modified_since_revision (:obj:`int`, optional): TODO.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.TracksList`: Треки с отметкой "Мне нравится".
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         return await self._get_likes(
-            'track', user_id, {'if-modified-since-revision': if_modified_since_revision}, timeout, *args, **kwargs
+            'track', user_id, {'if-modified-since-revision': if_modified_since_revision}, *args, **kwargs
         )
 
     @log
     async def users_likes_albums(
-        self, user_id: Union[str, int] = None, rich: bool = True, timeout: Union[int, float] = None, *args, **kwargs
+        self, user_id: Union[str, int] = None, rich: bool = True, *args, **kwargs
     ) -> List[Like]:
         """Получение альбомов с отметкой "Мне нравится".
 
         Args:
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
             rich (:obj:`bool`, optional): Если False, то приходит укороченная версия.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Like`: Альбомы с отметкой "Мне нравится".
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._get_likes('album', user_id, {'rich': str(rich)}, timeout, *args, **kwargs)
+        return await self._get_likes('album', user_id, {'rich': str(rich)}, *args, **kwargs)
 
     @log
     async def users_likes_artists(
         self,
         user_id: Union[str, int] = None,
         with_timestamps: bool = True,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> List[Like]:
         """Получение артистов с отметкой "Мне нравится".
 
         Args:
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
             with_timestamps (:obj:`bool`, optional):  С временными метками TODO.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Like`: Артисты с отметкой "Мне нравится".
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._get_likes(
-            'artist', user_id, {'with-timestamps': str(with_timestamps)}, timeout, *args, **kwargs
-        )
+        return await self._get_likes('artist', user_id, {'with-timestamps': str(with_timestamps)}, *args, **kwargs)
 
     @log
-    async def users_likes_playlists(
-        self, user_id: Union[str, int] = None, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[Like]:
+    async def users_likes_playlists(self, user_id: Union[str, int] = None, *args, **kwargs) -> List[Like]:
         """Получение плейлистов с отметкой "Мне нравится".
 
         Args:
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.Like`: Плейлисты с отметкой "Мне нравится".
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._get_likes('playlist', user_id, timeout=timeout, *args, **kwargs)
+        return await self._get_likes('playlist', user_id, *args, **kwargs)
 
     @log
     async def users_dislikes_tracks(
         self,
         user_id: Union[str, int] = None,
         if_modified_since_revision: int = 0,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[TracksList]:
         """Получение треков с отметкой "Не рекомендовать".
 
         Args:
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
             if_modified_since_revision (:obj:`bool`, optional): TODO.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.TracksList`: Треки с отметкой "Не рекомендовать".
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         url = f'{self.base_url}/users/{user_id}/dislikes/tracks'
 
         result = await self._request.get(
-            url, {'if_modified_since_revision': if_modified_since_revision}, timeout=timeout, *args, **kwargs
+            url, {'if_modified_since_revision': if_modified_since_revision}, *args, **kwargs
         )
 
         return TracksList.de_json(result.get('library'), self)
 
     async def _dislike_action(
         self,
         ids: Union[List[Union[str, int]], str, int],
         remove: bool = False,
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> bool:
         """Действия с отметкой "Не рекомендовать".
 
         Args:
             ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор объекта или объектов.
             remove (:obj:`bool`, optional): Если :obj:`True`, то снимает отметку, иначе ставит.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if user_id is None and self.me is not None:
             user_id = self.me.account.uid
 
         action = 'remove' if remove else 'add-multiple'
         url = f'{self.base_url}/users/{user_id}/dislikes/tracks/{action}'
 
-        result = await self._request.post(url, {f'track-ids': ids}, timeout=timeout, *args, **kwargs)
+        result = await self._request.post(url, {f'track-ids': ids}, *args, **kwargs)
 
         return 'revision' in result
 
     @log
     async def users_dislikes_tracks_add(
         self,
         track_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Поставить отметку "Не рекомендовать" треку/трекам.
 
         Note:
             Так же снимает отметку "Мне нравится" если она есть.
 
         Args:
             track_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор трека или треков.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._dislike_action(track_ids, False, user_id, timeout, *args, **kwargs)
+        return await self._dislike_action(track_ids, remove=False, user_id=user_id, **kwargs)
 
     @log
     async def users_dislikes_tracks_remove(
         self,
         track_ids: Union[List[Union[str, int]], str, int],
         user_id: Union[str, int] = None,
-        timeout: Union[int, float] = None,
-        *args,
         **kwargs,
     ) -> bool:
         """Снять отметку "Не рекомендовать" у трека/треков.
 
         Args:
             track_ids (:obj:`str` | :obj:`int` | :obj:`list` из :obj:`str` | :obj:`list` из :obj:`int`): Уникальный
                 идентификатор трека или треков.
             user_id (:obj:`str` | :obj:`int`, optional): Уникальный идентификатор пользователя. Если не указан
                 используется ID текущего пользователя.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
-        return await self._dislike_action(track_ids, True, user_id, timeout, *args, **kwargs)
+        return await self._dislike_action(track_ids, remove=True, user_id=user_id, **kwargs)
 
     @log
     async def after_track(
         self,
         next_track_id: Union[str, int],
         context_item: str,
         prev_track_id: Union[str, int] = None,
         context: str = 'playlist',
         types: str = 'shot',
         from_: str = 'mobile-landing-origin-default',
-        timeout: Union[int, float] = None,
         *args,
         **kwargs,
     ) -> Optional[ShotEvent]:
         """Получение рекламы или шота от Алисы после трека.
 
         Note:
             При получения шота от Алисы `prev_track_id` можно не указывать.
@@ -2455,16 +2298,14 @@
         Args:
             prev_track_id (:obj:`str` | :obj:`int`): Уникальный идентификатор предыдущего трека.
             next_track_id (:obj:`str` | :obj:`int`): Уникальный идентификатор следующего трека.
             context_item (:obj:`str`): Уникальный идентификатор контекста.
             context (:obj:`str`, optional): Место, откуда было вызвано получение.
             types (:obj:`str`, optional): Тип того, что вернуть после трека.
             from_ (:obj:`str`, optional): Место, с которого попали в контекст.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.ShotEvent`: Шот от Алисы или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -2477,90 +2318,81 @@
             'prevTrackId': prev_track_id,
             'nextTrackId': next_track_id,
             'context': context,
             'contextItem': context_item,
             'types': types,
         }
 
-        result = await self._request.get(url, params=params, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, params, *args, **kwargs)
 
-        # TODO судя по всему эндпоинт ещё возвращает рекламу после треков для пользователей без подписки.
+        # TODO (MarshalX) судя по всему ручка ещё возвращает рекламу после треков для пользователей без подписки.
+        #  https://github.com/MarshalX/yandex-music-api/issues/557
         return ShotEvent.de_json(result.get('shot_event'), self)
 
     @log
-    async def queues_list(
-        self, device: str = None, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> List[QueueItem]:
+    async def queues_list(self, device: str = None, *args, **kwargs) -> List[QueueItem]:
         """Получение всех очередей треков с разных устройств для синхронизации между ними.
 
         Note:
             Именно к `device` привязывается очередь. На одном устройстве может быть создана одна очередь.
 
             Аргумент `device` имеет следующий формат: `ключ=значение; ключ2=значение2`. Обязательные паля указы в
             значении по умолчанию.
 
         Args:
             device (:obj:`str`, optional): Содержит информацию об устройстве с которого выполняется запрос.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`list` из :obj:`yandex_music.QueueItem`: Элементы очереди всех устройств.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         if not device:
             device = self.device
 
         url = f'{self.base_url}/queues'
 
         self._request.headers['X-Yandex-Music-Device'] = device
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return QueueItem.de_list(result.get('queues'), self)
 
     @log
-    async def queue(self, queue_id: str, timeout: Union[int, float] = None, *args, **kwargs) -> Optional[Queue]:
+    async def queue(self, queue_id: str, *args, **kwargs) -> Optional[Queue]:
         """Получение информации об очереди треков и самих треков в ней.
 
         Args:
             queue_id (:obj:`str`): Уникальный идентификатор очереди.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`yandex_music.Queue`: Очередь или :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         url = f'{self.base_url}/queues/{queue_id}'
 
-        result = await self._request.get(url, timeout=timeout, *args, **kwargs)
+        result = await self._request.get(url, *args, **kwargs)
 
         return Queue.de_json(result, self)
 
     @log
-    async def queue_update_position(
-        self, queue_id: str, current_index: int, device: str = None, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> bool:
+    async def queue_update_position(self, queue_id: str, current_index: int, device: str = None, **kwargs) -> bool:
         """Установка текущего индекса проигрываемого трека в очереди треков.
 
         Note:
             Изменить можно только у той очереди, которая была создана с переданного `device`!
 
         Args:
             queue_id (:obj:`str`): Уникальный идентификатор очереди.
             current_index (:obj:`int`): Текущий индекс.
             device (:obj:`str`, optional): Содержит информацию об устройстве с которого выполняется запрос.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`bool`: :obj:`True` при успешном выполнении запроса, иначе :obj:`False`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -2568,30 +2400,26 @@
         if not device:
             device = self.device
 
         url = f'{self.base_url}/queues/{queue_id}/update-position'
 
         self._request.headers['X-Yandex-Music-Device'] = device
         result = await self._request.post(
-            url, {'isInteractive': False}, params={'currentIndex': current_index}, timeout=timeout, *args, **kwargs
+            url, {'isInteractive': False}, params={'currentIndex': current_index}, **kwargs
         )
 
         return result.get('status') == 'ok'
 
     @log
-    async def queue_create(
-        self, queue: Union[Queue, str], device: str = None, timeout: Union[int, float] = None, *args, **kwargs
-    ) -> Optional[str]:
+    async def queue_create(self, queue: Union[Queue, str], device: str = None, *args, **kwargs) -> Optional[str]:
         """Создание новой очереди треков.
 
         Args:
             queue (:obj:`yandex_music.Queue` | :obj:`str`): Объект очереди или JSON строка с этим объектом.
             device (:obj:`str`, optional): Содержит информацию об устройстве с которого выполняется запрос.
-            timeout (:obj:`int` | :obj:`float`, optional): Если это значение указано, используется как время ожидания
-                ответа от сервера вместо указанного при создании пула.
             **kwargs (:obj:`dict`, optional): Произвольные аргументы (будут переданы в запрос).
 
         Returns:
             :obj:`str`: Вернёт уникальный идентификатор созданной очереди, иначе :obj:`None`.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
@@ -2601,17 +2429,17 @@
 
         if isinstance(queue, Queue):
             queue = queue.to_json(True)
 
         url = f'{self.base_url}/queues'
 
         self._request.headers['X-Yandex-Music-Device'] = device
-        result = await self._request.post(url, queue, timeout=timeout, *args, **kwargs)
+        result = await self._request.post(url, queue, *args, **kwargs)
 
-        return result.get('id_')
+        return result.get('id')
 
     # camelCase псевдонимы
 
     #: Псевдоним для :attr:`account_status`
     accountStatus = account_status
     #: Псевдоним для :attr:`account_settings`
     accountSettings = account_settings
@@ -2629,14 +2457,16 @@
     newReleases = new_releases
     #: Псевдоним для :attr:`new_playlists`
     newPlaylists = new_playlists
     #: Псевдоним для :attr:`tracks_download_info`
     tracksDownloadInfo = tracks_download_info
     #: Псевдоним для :attr:`track_supplement`
     trackSupplement = track_supplement
+    #: Псевдоним для :attr:`tracks_lyrics`
+    tracksLyrics = tracks_lyrics
     #: Псевдоним для :attr:`tracks_similar`
     tracksSimilar = tracks_similar
     #: Псевдоним для :attr:`play_audio`
     playAudio = play_audio
     #: Псевдоним для :attr:`albums_with_tracks`
     albumsWithTracks = albums_with_tracks
     #: Псевдоним для :attr:`search_suggest`
```

### Comparing `yandex-music-2.0.1/yandex_music/cover.py` & `yandex-music-2.1.0/yandex_music/cover.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,37 +38,71 @@
     prefix: Optional[str] = None
     error: Optional[str] = None
     client: Optional['Client'] = None
 
     def __post_init__(self):
         self._id_attrs = (self.prefix, self.version, self.uri, self.items_uri)
 
+    def get_url(self, index: int = 0, size: str = '200x200') -> str:
+        """Возвращает URL обложки.
+
+        Args:
+            index (:obj:`int`, optional): Индекс элемента в списке ссылок на обложки если нет `self.uri`.
+            size (:obj:`str`, optional): Размер изображения.
+
+        Returns:
+            :obj:`str`: URL адрес.
+        """
+        uri = self.uri or self.items_uri[index]
+
+        return f'https://{uri.replace("%%", size)}'
+
     def download(self, filename: str, index: int = 0, size: str = '200x200') -> None:
         """Загрузка обложки.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             index (:obj:`int`, optional): Индекс элемента в списке ссылок на обложки если нет `self.uri`.
             size (:obj:`str`, optional): Размер изображения.
         """
-        uri = self.uri or self.items_uri[index]
-
-        self.client.request.download(f'https://{uri.replace("%%", size)}', filename)
+        self.client.request.download(self.get_url(index, size), filename)
 
     async def download_async(self, filename: str, index: int = 0, size: str = '200x200') -> None:
         """Загрузка обложки.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             index (:obj:`int`, optional): Индекс элемента в списке ссылок на обложки если нет `self.uri`.
             size (:obj:`str`, optional): Размер изображения.
         """
-        uri = self.uri or self.items_uri[index]
+        await self.client.request.download(self.get_url(index, size), filename)
+
+    def download_bytes(self, index: int = 0, size: str = '200x200') -> bytes:
+        """Загрузка обложки и возврат в виде байтов.
 
-        await self.client.request.download(f'https://{uri.replace("%%", size)}', filename)
+        Args:
+            index (:obj:`int`, optional): Индекс элемента в списке ссылок на обложки если нет `self.uri`.
+            size (:obj:`str`, optional): Размер изображения.
+
+        Returns:
+            :obj:`bytes`: Обложка в виде байтов.
+        """
+        return self.client.request.retrieve(self.get_url(index, size))
+
+    async def download_bytes_async(self, index: int = 0, size: str = '200x200') -> bytes:
+        """Загрузка обложки и возврат в виде байтов.
+
+        Args:
+            index (:obj:`int`, optional): Индекс элемента в списке ссылок на обложки если нет `self.uri`.
+            size (:obj:`str`, optional): Размер изображения.
+
+        Returns:
+            :obj:`bytes`: Обложка в виде байтов.
+        """
+        return await self.client.request.retrieve(self.get_url(index, size))
 
     @classmethod
     def de_json(cls, data: dict, client: 'Client') -> Optional['Cover']:
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
@@ -102,9 +136,15 @@
         for cover in data:
             covers.append(cls.de_json(cover, client))
 
         return covers
 
     # camelCase псевдонимы
 
+    #: Псевдоним для :attr:`get_url`
+    getUrl = get_url
     #: Псевдоним для :attr:`download_async`
     downloadAsync = download_async
+    #: Псевдоним для :attr:`download_bytes`
+    downloadBytes = download_bytes
+    #: Псевдоним для :attr:`download_bytes_async`
+    downloadBytesAsync = download_bytes_async
```

### Comparing `yandex-music-2.0.1/yandex_music/download_info.py` & `yandex-music-2.1.0/yandex_music/download_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from yandex_music import YandexMusicObject
 from yandex_music.utils import model
 
 if TYPE_CHECKING:
     from yandex_music import Client
     from xml.dom.minicompat import NodeList
 
+SIGN_SALT = 'XGRlBW9FXlekgbPrRHuSiA'
+
 
 @model
 class DownloadInfo(YandexMusicObject):
     """Класс, представляющий информацию о вариантах загрузки трека.
 
     Attributes:
         codec (:obj:`str`): Кодек аудиофайла.
@@ -48,15 +50,15 @@
 
     def __build_direct_link(self, xml: str) -> str:
         doc = minidom.parseString(xml)
         host = self._get_text_node_data(doc.getElementsByTagName('host'))
         path = self._get_text_node_data(doc.getElementsByTagName('path'))
         ts = self._get_text_node_data(doc.getElementsByTagName('ts'))
         s = self._get_text_node_data(doc.getElementsByTagName('s'))
-        sign = md5(('XGRlBW9FXlekgbPrRHuSiA' + path[1::] + s).encode('utf-8')).hexdigest()
+        sign = md5((SIGN_SALT + path[1::] + s).encode('utf-8')).hexdigest()
 
         return f'https://{host}/get-mp3/{sign}/{ts}{path}'
 
     def get_direct_link(self) -> str:
         """Получение прямой ссылки на загрузку из XML ответа.
 
         Метод доступен только одну минуту с момента получения информации о загрузке, иначе 410 ошибка!
@@ -104,14 +106,36 @@
             filename (:obj:`str`): Путь и(или) название файла вместе с расширением.
         """
         if self.direct_link is None:
             await self.get_direct_link_async()
 
         await self.client.request.download(self.direct_link, filename)
 
+    def download_bytes(self) -> bytes:
+        """Загрузка трека и возврат в виде байтов.
+
+        Returns:
+            :obj:`bytes`: Трек в виде байтов.
+        """
+        if self.direct_link is None:
+            self.get_direct_link()
+
+        return self.client.request.retrieve(self.direct_link)
+
+    async def download_bytes_async(self) -> bytes:
+        """Загрузка трека и возврат в виде байтов.
+
+        Returns:
+            :obj:`bytes`: Трек в виде байтов.
+        """
+        if self.direct_link is None:
+            await self.get_direct_link_async()
+
+        return await self.client.request.retrieve(self.direct_link)
+
     @classmethod
     def de_json(cls, data: dict, client: 'Client') -> Optional['DownloadInfo']:
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
@@ -180,7 +204,11 @@
 
     #: Псевдоним для :attr:`get_direct_link`
     getDirectLink = get_direct_link
     #: Псевдоним для :attr:`get_direct_link_async`
     getDirectLinkAsync = get_direct_link_async
     #: Псевдоним для :attr:`download_async`
     downloadAsync = download_async
+    #: Псевдоним для :attr:`download_bytes`
+    downloadBytes = download_bytes
+    #: Псевдоним для :attr:`download_bytes_async`
+    downloadBytesAsync = download_bytes_async
```

### Comparing `yandex-music-2.0.1/yandex_music/exceptions.py` & `yandex-music-2.1.0/yandex_music/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 class UnauthorizedError(YandexMusicError):
     """Класс исключения, вызываемого для случаев ошибок
     аутентификации и авторизации.
     """
 
 
+# TODO (MarshalX) На самом деле поиск еще происходит по кодеку
+#  https://github.com/MarshalX/yandex-music-api/issues/552
 class InvalidBitrateError(YandexMusicError):
     """Класс исключения, вызываемого при попытке загрузки трека
     с недоступным битрейтом.
     """
 
 
 class NetworkError(YandexMusicError):
@@ -24,13 +26,13 @@
     """Класс исключения, вызываемый в случае отправки неправильного запроса."""
 
 
 class NotFoundError(NetworkError):
     """Класс исключения, вызываемый в случае ответа от сервера со статус кодом 404."""
 
 
-# TimeoutError builtin. И не знаю хотим ли использовать его для синк и asyncio.TimeoutError для асинк
+# TimeoutError builtin. Пока не знаю хотим ли использовать его для синхронной и asyncio.TimeoutError для асинхронной
 class TimedOutError(NetworkError):
     """Класс исключения, вызываемого для случаев истечения времени ожидания."""
 
     def __init__(self):
         super().__init__('Timed out')
```

### Comparing `yandex-music-2.0.1/yandex_music/experiments.py` & `yandex-music-2.1.0/yandex_music/experiments.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 if TYPE_CHECKING:
     from yandex_music import Client
 
 
 @model
 class Experiments(YandexMusicObject):
-    """Класс, представляющий какие-то свистелки-перделки, флажки, режимы экспериментальных функций.
+    """Класс, представляющий какие-то свистелки и перделки, флажки, режимы экспериментальных функций.
 
     Attributes:
         client (:obj:`yandex_music.Client`): Клиент Yandex Music.
         название_эксперимента (:obj:`str`): Содержит режим или состояние, или функцию, или ещё что угодно.
 
     Args:
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
@@ -31,15 +31,15 @@
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`yandex_music.Experiments`: Какие-то свистелки-перделки, флажки, режимы экспериментальных функций.
+            :obj:`yandex_music.Experiments`: Какие-то свистелки и перделки, флажки, режимы экспериментальных функций.
         """
         if not data:
             return None
 
         data = super(Experiments, cls).de_json(data, client)
 
         return cls(client=client, **data)
```

### Comparing `yandex-music-2.0.1/yandex_music/feed/album_event.py` & `yandex-music-2.1.0/yandex_music/feed/album_event.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 @model
 class AlbumEvent(YandexMusicObject):
     """Класс, представляющий альбом в событии фида.
 
     Attributes:
-        album (:obj:`yandex_music.Album` | :obj:`None`): Альбом.
+        album (:obj:`yandex_music.Album`, optional): Альбом.
         tracks (:obj:`list` из :obj:`yandex_music.Track`): Треки.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
     album: Optional['Album']
     tracks: List['Track']
     client: Optional['Client'] = None
```

### Comparing `yandex-music-2.0.1/yandex_music/feed/artist_event.py` & `yandex-music-2.1.0/yandex_music/feed/artist_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 
 @model
 class ArtistEvent(YandexMusicObject):
     """Класс, представляющий артиста в событии фида.
 
     Attributes:
-        artist (:obj:`yandex_music.Artist` | :obj:`None`): Артист.
-        tracks (:obj:`list` :obj:`yandex_music.Track`): Треки.
-        similar_to_artists_from_history (:obj:`list` :obj:`yandex_music.Artist`): Похожие артисты из истории.
+        artist (:obj:`yandex_music.Artist`, optional): Артист.
+        tracks (:obj:`list` из :obj:`yandex_music.Track`): Треки.
+        similar_to_artists_from_history (:obj:`list` из :obj:`yandex_music.Artist`): Похожие артисты из истории.
         subscribed (:obj:`bool`): Подписан ли на событие.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
     artist: Optional['Artist']
     tracks: List['Track']
     similar_to_artists_from_history: List['Artist']
```

### Comparing `yandex-music-2.0.1/yandex_music/feed/day.py` & `yandex-music-2.1.0/yandex_music/feed/day.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/feed/event.py` & `yandex-music-2.1.0/yandex_music/feed/event.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/feed/feed.py` & `yandex-music-2.1.0/yandex_music/feed/feed.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/feed/generated_playlist.py` & `yandex-music-2.1.0/yandex_music/feed/generated_playlist.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,22 +17,24 @@
 
     Attributes:
         type (:obj:`str`): Тип сгенерированного плейлиста.
         ready (:obj:`bool`): Готовность плейлиста.
         notify (:obj:`bool`): Уведомлён ли пользователь об обновлении содержания.
         data (:obj:`yandex_music.Playlist`, optional): Сгенерированный плейлист.
         description (:obj:`list`, optional): Описание TODO.
+        preview_description (:obj:`str`, optional): Короткое описание под блоком лендинга.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
     type: str
     ready: bool
     notify: bool
     data: Optional['Playlist']
     description: Optional[list] = None
+    preview_description: Optional[str] = None
     client: Optional['Client'] = None
 
     def __post_init__(self):
         self._id_attrs = (self.type, self.ready, self.notify, self.data)
 
     @classmethod
     def de_json(cls, data: dict, client: 'Client') -> Optional['GeneratedPlaylist']:
```

### Comparing `yandex-music-2.0.1/yandex_music/feed/track_with_ads.py` & `yandex-music-2.1.0/yandex_music/feed/track_with_ads.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/genre/genre.py` & `yandex-music-2.1.0/yandex_music/genre/genre.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/genre/images.py` & `yandex-music-2.1.0/yandex_music/playlist/open_graph_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,48 @@
 from typing import TYPE_CHECKING, Optional
 
 from yandex_music import YandexMusicObject
 from yandex_music.utils import model
 
 if TYPE_CHECKING:
-    from yandex_music import Client
+    from yandex_music import Client, Cover
 
 
 @model
-class Images(YandexMusicObject):
-    """Класс, представляющий изображение жанра.
+class OpenGraphData(YandexMusicObject):
+    """Класс, представляющий данные для Open Graph.
 
     Attributes:
-        _208x208 (:obj:`str`, optional): Ссылка на изображение размером 208 на 208.
-        _300x300 (:obj:`str`, optional): Ссылка на изображение размером 300 на 300.
+        title (:obj:`str`): Заголовок.
+        description (:obj:`str`): Описание.
+        image (:obj:`yandex_music.Cover`): Изображение.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
-    _208x208: Optional[str] = None
-    _300x300: Optional[str] = None
+    title: str
+    description: str
+    image: 'Cover'
     client: Optional['Client'] = None
 
     def __post_init__(self):
-        self._id_attrs = (self._208x208, self._300x300)
-
-    def download_208x208(self, filename: str) -> None:
-        """Загрузка изображения 208x208.
-
-        Args:
-            filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-        """
-        self.client.request.download(self._208x208, filename)
-
-    def download_300x300(self, filename: str) -> None:
-        """Загрузка изображения 300x300.
-
-        Args:
-            filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-        """
-        self.client.request.download(self._300x300, filename)
+        self._id_attrs = (self.title, self.description, self.image)
 
     @classmethod
-    def de_json(cls, data: dict, client: 'Client') -> Optional['Images']:
+    def de_json(cls, data: dict, client: 'Client') -> Optional['OpenGraphData']:
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`yandex_music.Images`: Изображение жанра.
+            :obj:`yandex_music.OpenGraphData`: Данные для Open Graph.
         """
         if not data:
             return None
 
-        data = super(Images, cls).de_json(data, client)
+        data = super(OpenGraphData, cls).de_json(data, client)
+        from yandex_music import Cover
+
+        data['image'] = Cover.de_json(data.get('image'), client)
 
         return cls(client=client, **data)
```

### Comparing `yandex-music-2.0.1/yandex_music/genre/title.py` & `yandex-music-2.1.0/yandex_music/genre/title.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/icon.py` & `yandex-music-2.1.0/yandex_music/rotor/sequence.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,71 @@
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Optional, List
 
 from yandex_music import YandexMusicObject
 from yandex_music.utils import model
 
 if TYPE_CHECKING:
-    from yandex_music import Client
+    from yandex_music import Client, Track
 
 
 @model
-class Icon(YandexMusicObject):
-    """Класс, представляющий иконку.
+class Sequence(YandexMusicObject):
+    """Класс, представляющий звено последовательности.
+
+    Note:
+        Известные значения поля `type_`: `track`. Возможно есть `ad`.
 
     Attributes:
-        background_color (:obj:`str`): Цвет заднего фона в HEX.
-        image_url (:obj:`str`): Ссылка на изображение.
+        type (:obj:`str`): Тип звена.
+        track (:obj:`yandex_music.Track` | :obj:`None`): Трек.
+        liked (:obj:`bool`): Связанное ли.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
-    background_color: str
-    image_url: str
+    type: str
+    track: Optional['Track']
+    liked: bool
     client: Optional['Client'] = None
 
     def __post_init__(self):
-        self._id_attrs = (self.background_color, self.image_url)
+        self._id_attrs = (self.type, self.track, self.liked)
 
-    def download(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка иконки.
+    @classmethod
+    def de_json(cls, data: dict, client: 'Client') -> Optional['Sequence']:
+        """Десериализация объекта.
 
         Args:
-            filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-            size (:obj:`str`, optional): Размер иконки.
-        """
-        self.client.request.download(self.get_url(size), filename)
-
-    async def download_async(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка иконки.
+            data (:obj:`dict`): Поля и значения десериализуемого объекта.
+            client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
-        Args:
-            filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-            size (:obj:`str`, optional): Размер иконки.
+        Returns:
+            :obj:`yandex_music.Sequence`: Звено последовательности.
         """
-        await self.client.request.download(self.get_url(size), filename)
+        if not data:
+            return None
 
-    def get_url(self, size: str = '200x200'):
-        """Получение URL иконки.
+        data = super(Sequence, cls).de_json(data, client)
+        from yandex_music import Track
 
-        Args:
-            size (:obj:`str`, optional): Размер иконки.
-        """
-        return f'https://{self.image_url.replace("%%", size)}'
+        data['track'] = Track.de_json(data.get('track'), client)
+
+        return cls(client=client, **data)
 
     @classmethod
-    def de_json(cls, data: dict, client: 'Client') -> Optional['Icon']:
-        """Десериализация объекта.
+    def de_list(cls, data: dict, client: 'Client') -> List['Sequence']:
+        """Десериализация списка объектов.
 
         Args:
-            data (:obj:`dict`): Поля и значения десериализуемого объекта.
+            data (:obj:`list`): Список словарей с полями и значениями десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`yandex_music.Icon`: Иконка.
+            :obj:`list` из :obj:`yandex_music.Sequence`: Последовательность треков.
         """
         if not data:
-            return None
-
-        data = super(Icon, cls).de_json(data, client)
-
-        return cls(client=client, **data)
+            return []
 
-    # camelCase псевдонимы
+        sequences = list()
+        for sequence in data:
+            sequences.append(cls.de_json(sequence, client))
 
-    #: Псевдоним для :attr:`download_async`
-    downloadAsync = download_async
+        return sequences
```

### Comparing `yandex-music-2.0.1/yandex_music/invocation_info.py` & `yandex-music-2.1.0/yandex_music/invocation_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/landing/block.py` & `yandex-music-2.1.0/yandex_music/landing/block.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/landing/block_entity.py` & `yandex-music-2.1.0/yandex_music/landing/block_entity.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/landing/chart.py` & `yandex-music-2.1.0/yandex_music/landing/chart.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/landing/chart_info.py` & `yandex-music-2.1.0/yandex_music/landing/chart_info.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/landing/chart_info_menu.py` & `yandex-music-2.1.0/yandex_music/landing/chart_info_menu.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/landing/chart_info_menu_item.py` & `yandex-music-2.1.0/yandex_music/landing/chart_info_menu_item.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/landing/chart_item.py` & `yandex-music-2.1.0/yandex_music/landing/chart_item.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/landing/landing.py` & `yandex-music-2.1.0/yandex_music/landing/landing.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/landing/landing_list.py` & `yandex-music-2.1.0/yandex_music/landing/landing_list.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/landing/mix_link.py` & `yandex-music-2.1.0/yandex_music/shot/shot_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,157 +1,154 @@
-from typing import TYPE_CHECKING, Optional, List
+from typing import TYPE_CHECKING, Optional
 
 from yandex_music import YandexMusicObject
 from yandex_music.utils import model
 
 if TYPE_CHECKING:
-    from yandex_music import Client
+    from yandex_music import Client, ShotType
 
 
 @model
-class MixLink(YandexMusicObject):
-    """Класс, представляющий ссылку (кликабельный блок) на подборку.
-
-    Note:
-        В цветах может как оказаться HEX (`#6c65a9`), так и какой-нибудь `transparent`.
-
-        Ссылка со схемой отличается от просто ссылки наличием `yandexmusic://` в начале.
+class ShotData(YandexMusicObject):
+    """Класс, представляющий основную информацию о шоте.
 
     Attributes:
-        title (:obj:`str`): Заголовок ссылки.
-        url (:obj:`str`): Ссылка на подборку.
-        url_scheme (:obj:`str`): Ссылка со схемой на подборку.
-        text_color (:obj:`str`): Цвет текста (HEX).
-        background_color (:obj:`str`): Цвет заднего фона.
-        background_image_uri (:obj:`str`): Ссылка на изображение заднего фона.
-        cover_white (:obj:`str`): Ссылка на изображение с обложкой TODO.
-        cover_uri (:obj:`str`, optional): Ссылка на изображение с обложкой.
+        cover_uri (:obj:`str`): Ссылка на обложку шота (иконка Алисы).
+        mds_url (:obj:`str`): Ссылка на аудиоверсию шота в озвучке от Алисы.
+        shot_text (:obj:`str`): Текстовая версия шота.
+        shot_type (:obj:`yandex_music.ShotType`): Тип шота.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
-    title: str
-    url: str
-    url_scheme: str
-    text_color: str
-    background_color: str
-    background_image_uri: str
-    cover_white: str
-    cover_uri: Optional[str] = None
+    cover_uri: str
+    mds_url: str
+    shot_text: str
+    shot_type: 'ShotType'
     client: Optional['Client'] = None
 
     def __post_init__(self):
-        self._id_attrs = (
-            self.url,
-            self.title,
-            self.url_scheme,
-            self.text_color,
-            self.background_color,
-            self.background_image_uri,
-            self.cover_white,
-        )
+        self._id_attrs = (self.cover_uri, self.mds_url, self.shot_text, self.shot_type)
 
-    def download_background_image(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка заднего фона.
+    def get_cover_url(self, size: str = '200x200') -> str:
+        """Возвращает URL обложки.
 
         Args:
-            filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-            size (:obj:`str`, optional): Размер заднего фона.
+            size (:obj:`str`, optional): Размер обложки.
+
+        Returns:
+            :obj:`str`: URL обложки.
         """
-        self.client.request.download(f'https://{self.background_image_uri.replace("%%", size)}', filename)
+        return f'https://{self.cover_uri.replace("%%", size)}'
 
-    async def download_background_image_async(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка заднего фона.
+    def download_cover(self, filename: str, size: str = '200x200') -> None:
+        """Загрузка обложки.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-            size (:obj:`str`, optional): Размер заднего фона.
+            size (:obj:`str`, optional): Размер обложки.
         """
-        await self.client.request.download(f'https://{self.background_image_uri.replace("%%", size)}', filename)
+        self.client.request.download(self.get_cover_url(size), filename)
 
-    def download_cover_white(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка обложки TODO.
+    async def download_cover_async(self, filename: str, size: str = '200x200') -> None:
+        """Загрузка обложки.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             size (:obj:`str`, optional): Размер обложки.
         """
-        self.client.request.download(f'https://{self.cover_white.replace("%%", size)}', filename)
+        await self.client.request.download(self.get_cover_url(size), filename)
 
-    async def download_cover_white_async(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка обложки TODO.
+    def download_mds(self, filename: str) -> None:
+        """Загрузка аудиоверсии шота.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-            size (:obj:`str`, optional): Размер обложки.
         """
-        await self.client.request.download(f'https://{self.cover_white.replace("%%", size)}', filename)
+        self.client.request.download(self.mds_url, filename)
 
-    def download_cover_uri(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка обложки.
+    async def download_mds_async(self, filename: str) -> None:
+        """Загрузка аудиоверсии шота.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-            size (:obj:`str`, optional): Размер обложки.
         """
-        self.client.request.download(f'https://{self.cover_uri.replace("%%", size)}', filename)
+        await self.client.request.download(self.mds_url, filename)
 
-    async def download_cover_uri_async(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка обложки.
+    def download_cover_bytes(self, size: str = '200x200') -> bytes:
+        """Загрузка обложки и возврат в виде байтов.
 
         Args:
-            filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             size (:obj:`str`, optional): Размер обложки.
+
+        Returns:
+            :obj:`bytes`: Обложка в виде байтов
         """
-        await self.client.request.download(f'https://{self.cover_uri.replace("%%", size)}', filename)
+        return self.client.request.retrieve(self.get_cover_url(size))
 
-    @classmethod
-    def de_json(cls, data: dict, client: 'Client') -> Optional['MixLink']:
-        """Десериализация объекта.
+    async def download_cover_bytes_async(self, size: str = '200x200') -> bytes:
+        """Загрузка обложки и возврат в виде байтов.
 
         Args:
-            data (:obj:`dict`): Поля и значения десериализуемого объекта.
-            client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
+            size (:obj:`str`, optional): Размер обложки.
 
         Returns:
-            :obj:`yandex_music.MixLink`: Блок-ссылка на подборку.
+            :obj:`bytes`: Обложка в виде байтов
         """
-        if not data:
-            return None
+        return await self.client.request.retrieve(self.get_cover_url(size))
 
-        data = super(MixLink, cls).de_json(data, client)
+    def download_mds_bytes(self) -> bytes:
+        """Загрузка аудиоверсии шота и возврат в виде байтов.
 
-        return cls(client=client, **data)
+        Returns:
+            :obj:`bytes`: Аудиоверсия шота в виде байтов
+        """
+        return self.client.request.retrieve(self.mds_url)
+
+    async def download_mds_bytes_async(self) -> bytes:
+        """Загрузка аудиоверсии шота и возврат в виде байтов.
+
+        Returns:
+            :obj:`bytes`: Аудиоверсия шота в виде байтов
+        """
+        return await self.client.request.retrieve(self.mds_url)
 
     @classmethod
-    def de_list(cls, data: dict, client: 'Client') -> List['MixLink']:
-        """Десериализация списка объектов.
+    def de_json(cls, data: dict, client: 'Client') -> Optional['ShotData']:
+        """Десериализация объекта.
 
         Args:
-            data (:obj:`list`): Список словарей с полями и значениями десериализуемого объекта.
+            data (:obj:`dict`): Поля и значения десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`list` из :obj:`yandex_music.MixLink`: Блоки-ссылки на подборки.
+            :obj:`yandex_music.ShotData`: Основная информация о шоте.
         """
         if not data:
-            return []
+            return None
 
-        mix_links = list()
-        for mix_link in data:
-            mix_links.append(cls.de_json(mix_link, client))
+        data = super(ShotData, cls).de_json(data, client)
+        from yandex_music import ShotType
 
-        return mix_links
+        data['shot_type'] = ShotType.de_json(data.get('shot_type'), client)
+
+        return cls(client=client, **data)
 
     # camelCase псевдонимы
 
-    #: Псевдоним для :attr:`download_background_image`
-    downloadBackgroundImage = download_background_image
-    #: Псевдоним для :attr:`download_background_image_async`
-    downloadBackgroundImageAsync = download_background_image_async
-    #: Псевдоним для :attr:`download_cover_white`
-    downloadCoverWhite = download_cover_white
-    #: Псевдоним для :attr:`download_cover_white_async`
-    downloadCoverWhiteAsync = download_cover_white_async
-    #: Псевдоним для :attr:`download_cover_uri`
-    downloadCoverUri = download_cover_uri
-    #: Псевдоним для :attr:`download_cover_uri_async`
-    downloadCoverUriAsync = download_cover_uri_async
+    #: Псевдоним для :attr:`get_cover_url`
+    getCoverUrl = get_cover_url
+    #: Псевдоним для :attr:`download_cover`
+    downloadCover = download_cover
+    #: Псевдоним для :attr:`download_cover_async`
+    downloadCoverAsync = download_cover_async
+    #: Псевдоним для :attr:`download_mds`
+    downloadMds = download_mds
+    #: Псевдоним для :attr:`download_mds_async`
+    downloadMdsAsync = download_mds_async
+    #: Псевдоним для :attr:`download_cover_bytes`
+    downloadCoverBytes = download_cover_bytes
+    #: Псевдоним для :attr:`download_cover_bytes_async`
+    downloadCoverBytesAsync = download_cover_bytes_async
+    #: Псевдоним для :attr:`download_mds_bytes`
+    downloadMdsBytes = download_mds_bytes
+    #: Псевдоним для :attr:`download_mds_bytes_async`
+    downloadMdsBytesAsync = download_mds_bytes_async
```

### Comparing `yandex-music-2.0.1/yandex_music/landing/personal_playlists_data.py` & `yandex-music-2.1.0/yandex_music/landing/personal_playlists_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/landing/play_context.py` & `yandex-music-2.1.0/yandex_music/landing/play_context.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/landing/play_contexts_data.py` & `yandex-music-2.1.0/yandex_music/landing/play_contexts_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/landing/promotion.py` & `yandex-music-2.1.0/yandex_music/landing/promotion.py`

 * *Files 17% similar despite different names*

```diff
@@ -49,31 +49,64 @@
             self.url,
             self.url_scheme,
             self.text_color,
             self.gradient,
             self.image,
         )
 
+    def get_image_url(self, size: str = '300x300') -> str:
+        """Возвращает URL изображения.
+
+        Args:
+            size (:obj:`str`, optional): Размер изображения.
+
+        Returns:
+            :obj:`str`: URL изображения.
+        """
+        return f'https://{self.image.replace("%%", size)}'
+
     def download_image(self, filename: str, size: str = '300x300') -> None:
         """Загрузка рекламного изображения.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             size (:obj:`str`, optional): Размер изображения.
         """
-        self.client.request.download(f'https://{self.image.replace("%%", size)}', filename)
+        self.client.request.download(self.get_image_url(size), filename)
 
     async def download_image_async(self, filename: str, size: str = '300x300') -> None:
         """Загрузка рекламного изображения.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             size (:obj:`str`, optional): Размер изображения.
         """
-        await self.client.request.download(f'https://{self.image.replace("%%", size)}', filename)
+        await self.client.request.download(self.get_image_url(size), filename)
+
+    def download_image_bytes(self, size: str = '300x300') -> bytes:
+        """Загрузка рекламного изображения и возврат в виде байтов.
+
+        Args:
+            size (:obj:`str`, optional): Размер изображения.
+
+        Returns:
+            :obj:`bytes`: Рекламное изображение в виде байтов.
+        """
+        return self.client.request.retrieve(self.get_image_url(size))
+
+    async def download_image_bytes_async(self, size: str = '300x300') -> bytes:
+        """Загрузка рекламного изображения и возврат в виде байтов.
+
+        Args:
+            size (:obj:`str`, optional): Размер изображения.
+
+        Returns:
+            :obj:`bytes`: Рекламное изображение в виде байтов.
+        """
+        return await self.client.request.retrieve(self.get_image_url(size))
 
     @classmethod
     def de_json(cls, data: dict, client: 'Client') -> Optional['Promotion']:
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
@@ -107,11 +140,17 @@
         for promotion in data:
             promotions.append(cls.de_json(promotion, client))
 
         return promotions
 
     # camelCase псевдонимы
 
+    #: Псевдоним для :attr:`get_image_url`
+    getImageUrl = get_image_url
     #: Псевдоним для :attr:`download_image`
     downloadImage = download_image
     #: Псевдоним для :attr:`download_image_async`
     downloadImageAsync = download_image_async
+    #: Псевдоним для :attr:`download_image_bytes`
+    downloadImageBytes = download_image_bytes
+    #: Псевдоним для :attr:`download_image_bytes_async`
+    downloadImageBytesAsync = download_image_bytes_async
```

### Comparing `yandex-music-2.0.1/yandex_music/landing/track_id.py` & `yandex-music-2.1.0/yandex_music/landing/track_id.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -91,13 +91,13 @@
         if not data:
             return []
 
         return [cls.de_json(track_id, client) for track_id in data]
 
     # camelCase псевдонимы
 
+    #: Псевдоним для :attr:`track_full_id`
+    trackFullId = track_full_id
     #: Псевдоним для :attr:`fetch_track`
     fetchTrack = fetch_track
     #: Псевдоним для :attr:`fetch_track_async`
     fetchTrackAsync = fetch_track_async
-    #: Псевдоним для :attr:`track_full_id`
-    trackFullId = track_full_id
```

### Comparing `yandex-music-2.0.1/yandex_music/landing/track_short_old.py` & `yandex-music-2.1.0/yandex_music/landing/track_short_old.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/like.py` & `yandex-music-2.1.0/yandex_music/like.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/pager.py` & `yandex-music-2.1.0/yandex_music/pager.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if TYPE_CHECKING:
     from yandex_music import Client
 
 
 @model
 class Pager(YandexMusicObject):
-    """Класс, представляющий пагинатор.
+    """Класс, представляющий пагинацию.
 
     Attributes:
         total (:obj:`int`): Всего треков.
         page (:obj:`int`): Номер страницы.
         per_page (:obj:`int`): Количество треков на странице.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
@@ -31,15 +31,15 @@
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`yandex_music.Pager`: Пагинатор.
+            :obj:`yandex_music.Pager`: Пагинация.
         """
         if not data:
             return None
 
         data = super(Pager, cls).de_json(data, client)
 
         return cls(client=client, **data)
```

### Comparing `yandex-music-2.0.1/yandex_music/permission_alerts.py` & `yandex-music-2.1.0/yandex_music/permission_alerts.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/playlist/brand.py` & `yandex-music-2.1.0/yandex_music/playlist/brand.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/playlist/case_forms.py` & `yandex-music-2.1.0/yandex_music/playlist/case_forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`yandex_music.CaseForms`: TODO.
+            :obj:`yandex_music.CaseForms`: Склонение имени.
         """
         if not data:
             return None
 
         data = super(CaseForms, cls).de_json(data, client)
 
         return cls(client=client, **data)
```

### Comparing `yandex-music-2.0.1/yandex_music/playlist/contest.py` & `yandex-music-2.1.0/yandex_music/playlist/contest.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/playlist/made_for.py` & `yandex-music-2.1.0/yandex_music/playlist/made_for.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/playlist/open_graph_data.py` & `yandex-music-2.1.0/yandex_music/rotor/id.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 from typing import TYPE_CHECKING, Optional
 
 from yandex_music import YandexMusicObject
 from yandex_music.utils import model
 
 if TYPE_CHECKING:
-    from yandex_music import Client, Cover
+    from yandex_music import Client
 
 
 @model
-class OpenGraphData(YandexMusicObject):
-    """Класс, представляющий данные для Open Graph.
+class Id(YandexMusicObject):
+    """Класс, представляющий уникальный идентификатор станции.
+
+    Note:
+        Известные типы станций: `user`, `genre`.
 
     Attributes:
-        title (:obj:`str`): Заголовок.
-        description (:obj:`str`): Описание.
-        image (:obj:`yandex_music.Cover`): Изображение.
+        type (:obj:`str`): Тип станции.
+        tag (:obj:`str`): Тег станции.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
+        **kwargs: Произвольные ключевые аргументы полученные от API.
     """
 
-    title: str
-    description: str
-    image: 'Cover'
+    type: str
+    tag: str
     client: Optional['Client'] = None
 
     def __post_init__(self):
-        self._id_attrs = (self.title, self.description, self.image)
+        self._id_attrs = (self.type, self.tag)
 
     @classmethod
-    def de_json(cls, data: dict, client: 'Client') -> Optional['OpenGraphData']:
+    def de_json(cls, data: dict, client: 'Client') -> Optional['Id']:
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`yandex_music.OpenGraphData`: Данные для Open Graph.
+            :obj:`yandex_music.Id`: Уникальный идентификатор станции.
         """
         if not data:
             return None
 
-        data = super(OpenGraphData, cls).de_json(data, client)
-        from yandex_music import Cover
-
-        data['image'] = Cover.de_json(data.get('image'), client)
+        data = super(Id, cls).de_json(data, client)
 
         return cls(client=client, **data)
```

### Comparing `yandex-music-2.0.1/yandex_music/playlist/play_counter.py` & `yandex-music-2.1.0/yandex_music/playlist/play_counter.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/playlist/playlist.py` & `yandex-music-2.1.0/yandex_music/playlist/playlist.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,14 +14,16 @@
         PlayCounter,
         PlaylistRecommendations,
         Artist,
         TrackId,
         Contest,
         OpenGraphData,
         Brand,
+        Pager,
+        CustomWave,
     )
 
 
 @model
 class Playlist(YandexMusicObject):
     """Класс, представляющий плейлист.
 
@@ -90,14 +92,16 @@
         description (:obj:`str`, optional): Описание плейлиста с разметкой Markdown.
         description_formatted (:obj:`str`, optional): Описание плейлиста. Только текст, без разметки.
         playlist_uuid (:obj:`str`, optional): TODO.
         type (:obj:`str`, optional): TODO.
         ready (:obj:`bool`, optional): Готовность TODO.
         is_for_from: TODO.
         regions: Регион TODO.
+        custom_wave (:obj:'yandex_music.CustomWave`, optional): Описание плейлиста. TODO.
+        pager (:obj:`yandex_music.Pager`, optional): Пагинатор.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
     owner: Optional['User']
     cover: Optional['Cover']
     made_for: Optional['MadeFor']
     play_counter: Optional['PlayCounter']
@@ -148,14 +152,16 @@
     description: Optional[str] = None
     description_formatted: Optional[str] = None
     playlist_uuid: Optional[str] = None
     type: Optional[str] = None
     ready: Optional[bool] = None
     is_for_from: Any = None
     regions: Any = None
+    custom_wave: Optional['CustomWave'] = None
+    pager: Optional['Pager'] = None
     client: Optional['Client'] = None
 
     def __post_init__(self):
         self._id_attrs = (self.uid, self.kind, self.title, self.playlist_absence)
 
     @property
     def is_mine(self) -> bool:
@@ -175,53 +181,123 @@
     async def get_recommendations_async(self, *args, **kwargs) -> Optional['PlaylistRecommendations']:
         """Сокращение для::
 
         await client.users_playlists_recommendations(playlist.kind, playlist.owner.uid, *args, **kwargs)
         """
         return await self.client.users_playlists_recommendations(self.kind, self.owner.uid, *args, **kwargs)
 
+    def get_animated_cover_url(self, size: str = '300x300') -> str:
+        """Возвращает URL анимированной обложки.
+
+        Args:
+            size (:obj:`str`, optional): Размер анимированной обложки.
+
+        Returns:
+            :obj:`str`: URL анимированной обложки.
+        """
+        return f'https://{self.animated_cover_uri.replace("%%", size)}'
+
+    def get_og_image_url(self, size: str = '300x300') -> str:
+        """Возвращает URL обложки.
+
+        Args:
+            size (:obj:`str`, optional): Размер обложки.
+
+        Returns:
+            :obj:`str`: URL обложки.
+        """
+        return f'https://{self.og_image.replace("%%", size)}'
+
     def download_animated_cover(self, filename: str, size: str = '200x200') -> None:
         """Загрузка анимированной обложки.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением (GIF).
             size (:obj:`str`, optional): Размер анимированной обложки.
         """
-        self.client.request.download(f'https://{self.animated_cover_uri.replace("%%", size)}', filename)
+        self.client.request.download(self.get_animated_cover_url(size), filename)
 
     async def download_animated_cover_async(self, filename: str, size: str = '200x200') -> None:
         """Загрузка анимированной обложки.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением (GIF).
             size (:obj:`str`, optional): Размер анимированной обложки.
         """
-        await self.client.request.download(f'https://{self.animated_cover_uri.replace("%%", size)}', filename)
+        await self.client.request.download(self.get_animated_cover_url(size), filename)
 
     def download_og_image(self, filename: str, size: str = '200x200') -> None:
         """Загрузка обложки.
 
         Используйте это только когда нет self.cover!
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             size (:obj:`str`, optional): Размер обложки.
         """
-        self.client.request.download(f'https://{self.og_image.replace("%%", size)}', filename)
+        self.client.request.download(self.get_og_image_url(size), filename)
 
     async def download_og_image_async(self, filename: str, size: str = '200x200') -> None:
         """Загрузка обложки.
 
         Используйте это только когда нет self.cover!
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             size (:obj:`str`, optional): Размер обложки.
         """
-        await self.client.request.download(f'https://{self.og_image.replace("%%", size)}', filename)
+        await self.client.request.download(self.get_og_image_url(size), filename)
+
+    def download_animated_cover_bytes(self, size: str = '200x200') -> bytes:
+        """Загрузка анимированной обложки и возврат в виде байтов.
+
+        Args:
+            size (:obj:`str`, optional): Размер анимированной обложки.
+
+        Returns:
+            :obj:`bytes`: Анимированная обложка в виде байтов.
+        """
+        return self.client.request.retrieve(self.get_animated_cover_url(size))
+
+    async def download_animated_cover_bytes_async(self, size: str = '200x200') -> bytes:
+        """Загрузка анимированной обложки и возврат в виде байтов.
+
+        Args:
+            size (:obj:`str`, optional): Размер анимированной обложки.
+
+        Returns:
+            :obj:`bytes`: Анимированная обложка в виде байтов.
+        """
+        return await self.client.request.retrieve(self.get_animated_cover_url(size))
+
+    def download_og_image_bytes(self, size: str = '200x200') -> bytes:
+        """Загрузка обложки и возврат в виде байтов.
+
+        Используйте это только когда нет self.cover!
+
+        Args:
+            size (:obj:`str`, optional): Размер обложки.
+
+        Returns:
+            :obj:`bytes`: Обложка в виде байтов.
+        """
+        return self.client.request.retrieve(self.get_og_image_url(size))
+
+    async def download_og_image_bytes_async(self, size: str = '200x200') -> bytes:
+        """Загрузка обложки и возврат в виде байтов.
+
+        Используйте это только когда нет self.cover!
+
+        Args:
+            size (:obj:`str`, optional): Размер обложки.
+
+        Returns:
+            :obj:`bytes`: Обложка в виде байтов.
+        """
+        return await self.client.request.retrieve(self.get_og_image_url(size))
 
     def rename(self, name: str) -> None:
         client, kind = self.client, self.kind
 
         self.__dict__.clear()
         self.__dict__.update(client.users_playlists_name(kind, name).__dict__)
 
@@ -271,15 +347,15 @@
         return self.client.users_playlists(self.kind, self.owner.uid, *args, **kwargs).tracks
 
     async def fetch_tracks_async(self, *args, **kwargs) -> List['TrackShort']:
         """Сокращение для::
 
         await client.users_playlists(playlist.kind, playlist.owner.id, *args, **kwargs).tracks
         """
-        return await self.client.users_playlists(self.kind, self.owner.uid, *args, **kwargs).tracks
+        return (await self.client.users_playlists(self.kind, self.owner.uid, *args, **kwargs)).tracks
 
     def insert_track(self, track_id: int, album_id: int, *args, **kwargs) -> Optional['Playlist']:
         """Сокращение для::
 
         client.users_playlists_insert_track(self.kind, track_id, album_id, user_id=self.owner.uid,
         revision=self.revision, *args, **kwargs)
         """
@@ -352,14 +428,16 @@
             TrackShort,
             PlaylistAbsence,
             Artist,
             TrackId,
             Contest,
             OpenGraphData,
             Brand,
+            CustomWave,
+            Pager,
         )
 
         data['owner'] = User.de_json(data.get('owner'), client)
         data['cover'] = Cover.de_json(data.get('cover'), client)
         data['cover_without_text'] = Cover.de_json(data.get('cover_without_text'), client)
         data['made_for'] = MadeFor.de_json(data.get('made_for'), client)
         data['tracks'] = TrackShort.de_list(data.get('tracks'), client)
@@ -376,14 +454,17 @@
         data['last_owner_playlists'] = Playlist.de_list(data.get('last_owner_playlists'), client)
 
         data['playlist_absence'] = PlaylistAbsence.de_json(data.get('playlist_absence'), client)  # на случай фикса
         if data.get('playlist_absense'):  # очепятка яндуха
             data['playlist_absence'] = PlaylistAbsence.de_json(data.get('playlist_absense'), client)
             data.pop('playlist_absense')
 
+        data['custom_wave'] = CustomWave.de_json(data.get('custom_wave'), client)
+        data['pager'] = Pager.de_json(data.get('pager'), client)
+
         return cls(client=client, **data)
 
     @classmethod
     def de_list(cls, data: dict, client: 'Client') -> List['Playlist']:
         """Десериализация списка объектов.
 
         Args:
@@ -404,35 +485,47 @@
     isMine = is_mine
     #: Псевдоним для :attr:`playlist_id`
     playlistId = playlist_id
     #: Псевдоним для :attr:`get_recommendations`
     getRecommendations = get_recommendations
     #: Псевдоним для :attr:`get_recommendations_async`
     getRecommendationsAsync = get_recommendations_async
+    #: Псевдоним для :attr:`get_animated_cover_url`
+    getAnimatedCoverUrl = get_animated_cover_url
+    #: Псевдоним для :attr:`get_og_image_url`
+    getOgImageUrl = get_og_image_url
     #: Псевдоним для :attr:`download_animated_cover`
     downloadAnimatedCover = download_animated_cover
     #: Псевдоним для :attr:`download_animated_cover_async`
     downloadAnimatedCoverAsync = download_animated_cover_async
     #: Псевдоним для :attr:`download_og_image`
     downloadOgImage = download_og_image
     #: Псевдоним для :attr:`download_og_image_async`
     downloadOgImageAsync = download_og_image_async
+    #: Псевдоним для :attr:`download_animated_cover_bytes`
+    downloadAnimatedCoverBytes = download_animated_cover_bytes
+    #: Псевдоним для :attr:`download_animated_cover_bytes_async`
+    downloadAnimatedCoverBytesAsync = download_animated_cover_bytes_async
+    #: Псевдоним для :attr:`download_og_image_bytes`
+    downloadOgImageBytes = download_og_image_bytes
+    #: Псевдоним для :attr:`download_og_image_bytes_async`
+    downloadOgImageBytesAsync = download_og_image_bytes_async
+    #: Псевдоним для :attr:`rename_async`
+    renameAsync = rename_async
+    #: Псевдоним для :attr:`like_async`
+    likeAsync = like_async
+    #: Псевдоним для :attr:`dislike_async`
+    dislikeAsync = dislike_async
     #: Псевдоним для :attr:`fetch_tracks`
     fetchTracks = fetch_tracks
     #: Псевдоним для :attr:`fetch_tracks_async`
     fetchTracksAsync = fetch_tracks_async
     #: Псевдоним для :attr:`insert_track`
     insertTrack = insert_track
     #: Псевдоним для :attr:`insert_track_async`
     insertTrackAsync = insert_track_async
     #: Псевдоним для :attr:`delete_tracks`
     deleteTracks = delete_tracks
     #: Псевдоним для :attr:`delete_tracks_async`
     deleteTracksAsync = delete_tracks_async
-    #: Псевдоним для :attr:`rename_async`
-    renameAsync = rename_async
-    #: Псевдоним для :attr:`like_async`
-    likeAsync = like_async
-    #: Псевдоним для :attr:`dislike_async`
-    dislikeAsync = dislike_async
     #: Псевдоним для :attr:`delete_async`
     deleteAsync = delete_async
```

### Comparing `yandex-music-2.0.1/yandex_music/playlist/playlist_absence.py` & `yandex-music-2.1.0/yandex_music/playlist/playlist_absence.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/playlist/playlist_id.py` & `yandex-music-2.1.0/yandex_music/playlist/playlist_id.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/playlist/playlist_recommendation.py` & `yandex-music-2.1.0/yandex_music/playlist/playlist_recommendation.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/playlist/tag.py` & `yandex-music-2.1.0/yandex_music/playlist/tag.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,7 +45,8 @@
             return None
 
         data = super(Tag, cls).de_json(data, client)
 
         return cls(client=client, **data)
 
     # TODO (MarshalX) add download_og_image shortcut?
+    #  https://github.com/MarshalX/yandex-music-api/issues/556
```

### Comparing `yandex-music-2.0.1/yandex_music/playlist/tag_result.py` & `yandex-music-2.1.0/yandex_music/playlist/tag_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,7 +43,8 @@
 
         data['tag'] = Tag.de_json(data.get('tag'), client)
         data['ids'] = PlaylistId.de_list(data.get('ids'), client)
 
         return cls(client=client, **data)
 
     # TODO (MarshalX) add fetch_playlists shortcut?
+    #  https://github.com/MarshalX/yandex-music-api/issues/551
```

### Comparing `yandex-music-2.0.1/yandex_music/playlist/user.py` & `yandex-music-2.1.0/yandex_music/playlist/user.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/promo_code_status.py` & `yandex-music-2.1.0/yandex_music/promo_code_status.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/queue/context.py` & `yandex-music-2.1.0/yandex_music/queue/context.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/queue/queue.py` & `yandex-music-2.1.0/yandex_music/queue/queue.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/queue/queue_item.py` & `yandex-music-2.1.0/yandex_music/queue/queue_item.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/rotor/ad_params.py` & `yandex-music-2.1.0/yandex_music/rotor/ad_params.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/rotor/dashboard.py` & `yandex-music-2.1.0/yandex_music/rotor/dashboard.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/rotor/discrete_scale.py` & `yandex-music-2.1.0/yandex_music/rotor/discrete_scale.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         Известные значения поля `type`: `discrete-scale`.
 
     Attributes:
         type (:obj:`str`): Тип.
         name (:obj:`str`): Название.
         min (:obj:`yandex_music.Value`): Минимальное значение.
         max (:obj:`yandex_music.Value`): Максимальное значение.
-        client (:obj:`yandex_music.Client` optional): Клиент Yandex Music.
+        client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
     type: str
     name: str
     min: Optional['Value']
     max: Optional['Value']
     client: Optional['Client'] = None
```

### Comparing `yandex-music-2.0.1/yandex_music/rotor/enum.py` & `yandex-music-2.1.0/yandex_music/rotor/enum.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 @model
 class Enum(YandexMusicObject):
     """Класс, представляющий перечисления.
 
     Attributes:
         type (:obj:`str`): Тип перечисления.
         name (:obj:`str`): Название перечисления.
-        possible_values (:obj:`list` из :obj:`yandex_Music.Value`): Доступные значения.
+        possible_values (:obj:`list` из :obj:`yandex_music.Value`): Доступные значения.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
         **kwargs: Произвольные ключевые аргументы полученные от API.
     """
 
     type: str
     name: str
     possible_values: List['Value']
```

### Comparing `yandex-music-2.0.1/yandex_music/rotor/id.py` & `yandex-music-2.1.0/yandex_music/rotor/station_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,44 +4,38 @@
 from yandex_music.utils import model
 
 if TYPE_CHECKING:
     from yandex_music import Client
 
 
 @model
-class Id(YandexMusicObject):
-    """Класс, представляющий уникальный идентификатор станции.
-
-    Note:
-        Известные типы станций: `user`, `genre`.
+class StationData(YandexMusicObject):
+    """Класс, представляющий информацию о личной станции.
 
     Attributes:
-        type (:obj:`str`): Тип станции.
-        tag (:obj:`str`): Тег станции.
+        name (:obj:`str`): Название станции.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
-        **kwargs: Произвольные ключевые аргументы полученные от API.
     """
 
-    type: str
-    tag: str
+    name: str
     client: Optional['Client'] = None
 
     def __post_init__(self):
-        self._id_attrs = (self.type, self.tag)
+        self._id_attrs = (self.name,)
 
     @classmethod
-    def de_json(cls, data: dict, client: 'Client') -> Optional['Id']:
+    def de_json(cls, data: dict, client: 'Client') -> Optional['StationData']:
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`yandex_music.Id`: Уникальный идентификатор станции.
+            :obj:`yandex_music.StationData`: Информация о личной станции.
         """
         if not data:
             return None
 
-        data = super(Id, cls).de_json(data, client)
+        data = super(StationData, cls).de_json(data, client)
 
         return cls(client=client, **data)
```

### Comparing `yandex-music-2.0.1/yandex_music/rotor/restrictions.py` & `yandex-music-2.1.0/yandex_music/rotor/restrictions.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/rotor/rotor_settings.py` & `yandex-music-2.1.0/yandex_music/rotor/rotor_settings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/rotor/sequence.py` & `yandex-music-2.1.0/yandex_music/shot/shot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,75 @@
 from typing import TYPE_CHECKING, Optional, List
 
 from yandex_music import YandexMusicObject
 from yandex_music.utils import model
 
 if TYPE_CHECKING:
-    from yandex_music import Client, Track
+    from yandex_music import Client, ShotData
 
 
 @model
-class Sequence(YandexMusicObject):
-    """Класс, представляющий звено последовательности.
+class Shot(YandexMusicObject):
+    """Класс, представляющий шот от Алисы.
 
     Note:
-        Известные значения поля `type_`: `track`. Возможно есть `ad`.
+        Известные значения поля `status`: `ready`.
 
     Attributes:
-        type (:obj:`str`): Тип звена.
-        track (:obj:`yandex_music.Track` | :obj:`None`): Трек.
-        liked (:obj:`bool`): Связанное ли.
+        order (:obj:`int`): Порядковый номер при воспроизведении.
+        played (:obj:`bool`): Был ли проигран шот.
+        shot_data (:obj:`yandex_music.ShotData`): Основная информация о шоте.
+        shot_id (:obj:`str`): Уникальный идентификатор шота.
+        status (:obj:`str`): Статус шота.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
-    type: str
-    track: Optional['Track']
-    liked: bool
+    order: int
+    played: bool
+    shot_data: 'ShotData'
+    shot_id: str
+    status: str
     client: Optional['Client'] = None
 
     def __post_init__(self):
-        self._id_attrs = (self.type, self.track, self.liked)
+        self._id_attrs = (self.order, self.played, self.shot_data, self.shot_id, self.status)
 
     @classmethod
-    def de_json(cls, data: dict, client: 'Client') -> Optional['Sequence']:
+    def de_json(cls, data: dict, client: 'Client') -> Optional['Shot']:
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`yandex_music.Sequence`: Звено последовательности.
+            :obj:`yandex_music.Shot`: Шот от Алисы.
         """
         if not data:
             return None
 
-        data = super(Sequence, cls).de_json(data, client)
-        from yandex_music import Track
+        data = super(Shot, cls).de_json(data, client)
+        from yandex_music import ShotData
 
-        data['track'] = Track.de_json(data.get('track'), client)
+        data['shot_data'] = ShotData.de_json(data.get('shot_data'), client)
 
         return cls(client=client, **data)
 
     @classmethod
-    def de_list(cls, data: dict, client: 'Client') -> List['Sequence']:
+    def de_list(cls, data: dict, client: 'Client') -> List['Shot']:
         """Десериализация списка объектов.
 
         Args:
             data (:obj:`list`): Список словарей с полями и значениями десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`list` из :obj:`yandex_music.Sequence`: Последовательность треков.
+            :obj:`list` из :obj:`yandex_music.Shot`: Шоты от Алисы.
         """
         if not data:
             return []
 
-        sequences = list()
-        for sequence in data:
-            sequences.append(cls.de_json(sequence, client))
+        shots = list()
+        for shot in data:
+            shots.append(cls.de_json(shot, client))
 
-        return sequences
+        return shots
```

### Comparing `yandex-music-2.0.1/yandex_music/rotor/station.py` & `yandex-music-2.1.0/yandex_music/rotor/station.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/rotor/station_data.py` & `yandex-music-2.1.0/yandex_music/track/lyrics_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,38 +4,40 @@
 from yandex_music.utils import model
 
 if TYPE_CHECKING:
     from yandex_music import Client
 
 
 @model
-class StationData(YandexMusicObject):
-    """Класс, представляющий информацию о личной станции.
+class LyricsInfo(YandexMusicObject):
+    """Класс, описывающий доступные тексты трека.
 
     Attributes:
-        name (:obj:`str`): Название станции.
+        has_available_sync_lyrics (:obj:`bool`): Наличие синхронизированного текста.
+        has_available_text_lyrics (:obj:`bool`): Наличие текста трека.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
-    name: str
+    has_available_sync_lyrics: bool
+    has_available_text_lyrics: bool
     client: Optional['Client'] = None
 
     def __post_init__(self):
-        self._id_attrs = (self.name,)
+        self._id_attrs = (self.has_available_sync_lyrics, self.has_available_text_lyrics)
 
     @classmethod
-    def de_json(cls, data: dict, client: 'Client') -> Optional['StationData']:
+    def de_json(cls, data: dict, client: 'Client') -> Optional['LyricsInfo']:
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`yandex_music.StationData`: Информация о личной станции.
+            :obj:`yandex_music.LyricsInfo`: Типы доступных текстов трека.
         """
         if not data:
             return None
 
-        data = super(StationData, cls).de_json(data, client)
+        data = super(LyricsInfo, cls).de_json(data, client)
 
         return cls(client=client, **data)
```

### Comparing `yandex-music-2.0.1/yandex_music/rotor/station_result.py` & `yandex-music-2.1.0/yandex_music/rotor/station_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,30 +7,39 @@
     from yandex_music import Client, Station, RotorSettings, AdParams
 
 
 @model
 class StationResult(YandexMusicObject):
     """Класс, представляющий радиостанцию с настройками.
 
+    Note:
+        Известные значения `custom_name`: `Танцую`, `R'n'B`, `Отдыхаю`, `Просыпаюсь`, `Тренируюсь`, `В дороге`, `Работаю`, `Засыпаю`.
+
     Attributes:
         station (:obj:`yandex_music.Station` | :obj:`None`): Станция.
         settings (:obj:`yandex_music.RotorSettings` | :obj:`None`): Первый набор настроек.
         settings2 (:obj:`yandex_music.RotorSettings` | :obj:`None`): Второй набор настроек.
         ad_params (:obj:`yandex_music.AdParams` | :obj:`None`): Настройки рекламы.
         explanation (:obj:`str`, optional): TODO.
         prerolls (:obj:`list` из :obj:`str`, optional): Прероллы TODO.
+        rup_title (:obj:`str`): Название станции / Моя волна TODO.
+        rup_description (:obj:`str`): Описание станции.
+        custom_name (:obj:`str`, optional): Название станции TODO.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
     station: Optional['Station']
     settings: Optional['RotorSettings']
     settings2: Optional['RotorSettings']
     ad_params: Optional['AdParams']
     explanation: Optional[str] = None
     prerolls: Optional[list] = None
+    rup_title: str = None
+    rup_description: str = None
+    custom_name: Optional[str] = None
     client: Optional['Client'] = None
 
     def __post_init__(self):
         self._id_attrs = (self.station, self.settings, self.settings2, self.ad_params)
 
     @classmethod
     def de_json(cls, data: dict, client: 'Client') -> Optional['StationResult']:
```

### Comparing `yandex-music-2.0.1/yandex_music/rotor/station_tracks_result.py` & `yandex-music-2.1.0/yandex_music/rotor/station_tracks_result.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/rotor/value.py` & `yandex-music-2.1.0/yandex_music/rotor/value.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/search/best.py` & `yandex-music-2.1.0/yandex_music/search/best.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/search/search.py` & `yandex-music-2.1.0/yandex_music/search/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import TYPE_CHECKING, Optional
 
-from yandex_music import YandexMusicObject
+from yandex_music import YandexMusicObject, Album, Artist, Playlist, Track, Video, User
 from yandex_music.utils import model
 
 if TYPE_CHECKING:
     from yandex_music import Client, Best, SearchResult
 
 
 @model
@@ -32,22 +32,22 @@
         nocorrect (:obj:`bool`, optional): Было ли отключено исправление результата.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
     search_request_id: str
     text: str
     best: Optional['Best']
-    albums: Optional['SearchResult']
-    artists: Optional['SearchResult']
-    playlists: Optional['SearchResult']
-    tracks: Optional['SearchResult']
-    videos: Optional['SearchResult']
-    users: Optional['SearchResult']
-    podcasts: Optional['SearchResult']
-    podcast_episodes: Optional['SearchResult']
+    albums: Optional['SearchResult[Album]']
+    artists: Optional['SearchResult[Artist]']
+    playlists: Optional['SearchResult[Playlist]']
+    tracks: Optional['SearchResult[Track]']
+    videos: Optional['SearchResult[Video]']
+    users: Optional['SearchResult[User]']
+    podcasts: Optional['SearchResult[Album]']
+    podcast_episodes: Optional['SearchResult[Track]']
     type: Optional[str] = None
     page: Optional[int] = None
     per_page: Optional[int] = None
     misspell_result: Optional[str] = None
     misspell_original: Optional[str] = None
     misspell_corrected: Optional[bool] = None
     nocorrect: Optional[bool] = None
@@ -161,12 +161,12 @@
     #: Псевдоним для :attr:`get_page`
     getPage = get_page
     #: Псевдоним для :attr:`get_page_async`
     getPageAsync = get_page_async
     #: Псевдоним для :attr:`next_page`
     nextPage = next_page
     #: Псевдоним для :attr:`next_page_async`
-    nextPageASync = next_page_async
+    nextPageAsync = next_page_async
     #: Псевдоним для :attr:`prev_page`
     prevPage = prev_page
     #: Псевдоним для :attr:`prev_page_async`
     prevPageAsync = prev_page_async
```

### Comparing `yandex-music-2.0.1/yandex_music/search/search_result.py` & `yandex-music-2.1.0/yandex_music/search/search_result.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from typing import TYPE_CHECKING, Optional, List, Union
+from typing import TYPE_CHECKING, Optional, List, Union, TypeVar, Generic, Type, Dict
 
 from yandex_music import YandexMusicObject, Artist, Album, Track, Playlist, Video, User
 from yandex_music.utils import model
 
 if TYPE_CHECKING:
     from yandex_music import Client
 
+T = TypeVar('T', bound=Union[Track, Artist, Album, Playlist, Video])
 
-de_json_result = {
-    'track': Track.de_list,
-    'artist': Artist.de_list,
-    'album': Album.de_list,
-    'playlist': Playlist.de_list,
-    'video': Video.de_list,
-    'user': User.de_list,
-    'podcast': Album.de_list,
-    'podcast_episode': Track.de_list,
+
+type_class_by_str: Dict[str, Type[T]] = {
+    'track': Track,
+    'artist': Artist,
+    'album': Album,
+    'playlist': Playlist,
+    'video': Video,
+    'user': User,
+    'podcast': Album,
+    'podcast_episode': Track,
 }
 
 
 @model
-class SearchResult(YandexMusicObject):
+class SearchResult(YandexMusicObject, Generic[T]):
     """Класс, представляющий результаты поиска.
 
     Note:
         Значения поля `type`: `track`, `artist`, `playlist`, `album`, `video`.
 
     Attributes:
         type (:obj:`str`):  Тип результата.
@@ -36,22 +38,22 @@
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
     type: str
     total: int
     per_page: int
     order: int
-    results: List[Union[Track, Artist, Album, Playlist, Video]]
+    results: List[T]
     client: Optional['Client'] = None
 
     def __post_init__(self):
         self._id_attrs = (self.total, self.per_page, self.order, self.results)
 
     @classmethod
-    def de_json(cls, data: dict, client: 'Client', type_: str = None) -> Optional['SearchResult']:
+    def de_json(cls, data: Dict[str, Dict], client: 'Client', type_: str = None) -> Optional['SearchResult']:
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
             type_ (:obj:`str`, optional): Тип результата.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
@@ -59,10 +61,11 @@
             :obj:`yandex_music.SearchResult`: Результаты поиска.
         """
         if not data:
             return None
 
         data = super(SearchResult, cls).de_json(data, client)
         data['type'] = type_
-        data['results'] = de_json_result.get(type_)(data.get('results'), client)
+        type_class = type_class_by_str.get(type_)
+        data['results'] = type_class.de_list(data.get('results'), client)
 
         return cls(client=client, **data)
```

### Comparing `yandex-music-2.0.1/yandex_music/search/suggestions.py` & `yandex-music-2.1.0/yandex_music/search/suggestions.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/settings.py` & `yandex-music-2.1.0/yandex_music/settings.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/shot/shot.py` & `yandex-music-2.1.0/yandex_music/track/track_lyrics.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,79 @@
-from typing import TYPE_CHECKING, Optional, List
+from typing import TYPE_CHECKING, List, Optional
 
 from yandex_music import YandexMusicObject
 from yandex_music.utils import model
 
+
 if TYPE_CHECKING:
-    from yandex_music import Client, ShotData
+    from yandex_music import Client, LyricsMajor
 
 
 @model
-class Shot(YandexMusicObject):
-    """Класс, представляющий шот от Алисы.
-
-    Note:
-        Известные значения поля `status`: `ready`.
+class TrackLyrics(YandexMusicObject):
+    """Класс, представляющий текст трека.
 
     Attributes:
-        order (:obj:`int`): Порядковый номер при воспроизведении.
-        played (:obj:`bool`): Был ли проигран шот.
-        shot_data (:obj:`yandex_music.ShotData`): Основная информация о шоте.
-        shot_id (:obj:`str`): Уникальный идентификатор шота.
-        status (:obj:`str`): Статус шота.
+        download_url (:obj:`str`): Ссылка на скачивание текста.
+        lyric_id (:obj:`int`): Уникальный идентификатор текста.
+        external_lyric_id (:obj:`str`): Уникальный идентификатор текста на сервисе предоставляющий текст.
+        writers (:obj:`list` из :obj:`str`): Авторы текста.
+        major (:obj:`yandex_music.LyricsMajor`): Сервис, откуда был получен текст.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
-    order: int
-    played: bool
-    shot_data: 'ShotData'
-    shot_id: str
-    status: str
+    download_url: str
+    lyric_id: int
+    external_lyric_id: str
+    writers: List[str]
+    major: 'LyricsMajor'
     client: Optional['Client'] = None
 
     def __post_init__(self):
-        self._id_attrs = (self.order, self.played, self.shot_data, self.shot_id, self.status)
+        self._id_attrs = (
+            self.lyric_id,
+            self.external_lyric_id,
+        )
+
+    def fetch_lyrics(self) -> str:
+        """Получает текст песни по ссылке :attr:`yandex_music.TrackLyrics.download_url`.
+
+        Returns:
+            :obj:`str`: Текст песни.
+        """
+        return self.client.request.retrieve(self.download_url).decode('UTF-8')
+
+    async def fetch_lyrics_async(self) -> str:
+        """Получает текст песни по ссылке :attr:`yandex_music.TrackLyrics.download_url`.
+
+        Returns:
+            :obj:`str`: Текст песни.
+        """
+        return await self.client.request.retrieve(self.download_url).decode('UTF-8')
 
     @classmethod
-    def de_json(cls, data: dict, client: 'Client') -> Optional['Shot']:
+    def de_json(cls, data: dict, client: 'Client') -> Optional['TrackLyrics']:
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`yandex_music.Shot`: Шот от Алисы.
+            :obj:`yandex_music.TrackLyrics`: Текст трека.
         """
         if not data:
             return None
 
-        data = super(Shot, cls).de_json(data, client)
-        from yandex_music import ShotData
+        data = super(TrackLyrics, cls).de_json(data, client)
+        from yandex_music import LyricsMajor
 
-        data['shot_data'] = ShotData.de_json(data.get('shot_data'), client)
+        data['major'] = LyricsMajor.de_json(data.get('major'), client)
 
         return cls(client=client, **data)
 
-    @classmethod
-    def de_list(cls, data: dict, client: 'Client') -> List['Shot']:
-        """Десериализация списка объектов.
-
-        Args:
-            data (:obj:`list`): Список словарей с полями и значениями десериализуемого объекта.
-            client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
-
-        Returns:
-            :obj:`list` из :obj:`yandex_music.Shot`: Шоты от Алисы.
-        """
-        if not data:
-            return []
-
-        shots = list()
-        for shot in data:
-            shots.append(cls.de_json(shot, client))
+    # camelCase псевдонимы
 
-        return shots
+    #: Псевдоним для :attr:`fetch_lyrics`
+    fetchLyrics = fetch_lyrics
+    #: Псевдоним для :attr:`fetch_lyrics_async`
+    fetchLyricsAsync = fetch_lyrics_async
```

### Comparing `yandex-music-2.0.1/yandex_music/shot/shot_data.py` & `yandex-music-2.1.0/yandex_music/icon.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,102 @@
 from typing import TYPE_CHECKING, Optional
 
 from yandex_music import YandexMusicObject
 from yandex_music.utils import model
 
 if TYPE_CHECKING:
-    from yandex_music import Client, ShotType
+    from yandex_music import Client
 
 
 @model
-class ShotData(YandexMusicObject):
-    """Класс, представляющий основную информацию о шоте.
+class Icon(YandexMusicObject):
+    """Класс, представляющий иконку.
 
     Attributes:
-        cover_uri (:obj:`str`): Ссылка на обложку шота (иконка Алисы).
-        mds_url (:obj:`str`): Ссылка на аудиоверсию шота в озвучке от Алисы.
-        shot_text (:obj:`str`): Текстовая версия шота.
-        shot_type (:obj:`yandex_music.ShotType`): Тип шота.
+        background_color (:obj:`str`): Цвет заднего фона в HEX.
+        image_url (:obj:`str`): Ссылка на изображение.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
-    cover_uri: str
-    mds_url: str
-    shot_text: str
-    shot_type: 'ShotType'
+    background_color: str
+    image_url: str
     client: Optional['Client'] = None
 
     def __post_init__(self):
-        self._id_attrs = (self.cover_uri, self.mds_url, self.shot_text, self.shot_type)
+        self._id_attrs = (self.background_color, self.image_url)
 
-    def download_cover(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка обложки.
+    def download(self, filename: str, size: str = '200x200') -> None:
+        """Загрузка иконки.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-            size (:obj:`str`, optional): Размер обложки.
+            size (:obj:`str`, optional): Размер иконки.
         """
-        self.client.request.download(f'https://{self.cover_uri.replace("%%", size)}', filename)
+        self.client.request.download(self.get_url(size), filename)
 
-    async def download_cover_async(self, filename: str, size: str = '200x200') -> None:
-        """Загрузка обложки.
+    async def download_async(self, filename: str, size: str = '200x200') -> None:
+        """Загрузка иконки.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-            size (:obj:`str`, optional): Размер обложки.
+            size (:obj:`str`, optional): Размер иконки.
         """
-        await self.client.request.download(f'https://{self.cover_uri.replace("%%", size)}', filename)
+        await self.client.request.download(self.get_url(size), filename)
 
-    def download_mds(self, filename: str) -> None:
-        """Загрузка аудиоверсии шота.
+    def download_bytes(self, size: str = '200x200') -> bytes:
+        """Загрузка иконки и возврат в виде байтов.
 
         Args:
-            filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
+            size (:obj:`str`, optional): Размер иконки.
+
+        Returns:
+            :obj:`bytes`: Иконка в виде байтов.
         """
-        self.client.request.download(self.mds_url, filename)
+        return self.client.request.retrieve(self.get_url(size))
 
-    async def download_mds_async(self, filename: str) -> None:
-        """Загрузка аудиоверсии шота.
+    async def download_bytes_async(self, size: str = '200x200') -> bytes:
+        """Загрузка иконки и возврат в виде байтов.
 
         Args:
-            filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
+            size (:obj:`str`, optional): Размер иконки.
+
+        Returns:
+            :obj:`bytes`: Иконка в виде байтов.
         """
-        await self.client.request.download(self.mds_url, filename)
+        return await self.client.request.retrieve(self.get_url(size))
+
+    def get_url(self, size: str = '200x200'):
+        """Получение URL иконки.
+
+        Args:
+            size (:obj:`str`, optional): Размер иконки.
+        """
+        return f'https://{self.image_url.replace("%%", size)}'
 
     @classmethod
-    def de_json(cls, data: dict, client: 'Client') -> Optional['ShotData']:
+    def de_json(cls, data: dict, client: 'Client') -> Optional['Icon']:
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`yandex_music.ShotData`: Основная информация о шоте.
+            :obj:`yandex_music.Icon`: Иконка.
         """
         if not data:
             return None
 
-        data = super(ShotData, cls).de_json(data, client)
-        from yandex_music import ShotType
-
-        data['shot_type'] = ShotType.de_json(data.get('shot_type'), client)
+        data = super(Icon, cls).de_json(data, client)
 
         return cls(client=client, **data)
 
     # camelCase псевдонимы
 
-    #: Псевдоним для :attr:`download_cover`
-    downloadCover = download_cover
-    #: Псевдоним для :attr:`download_cover_async`
-    downloadCoverAsync = download_cover_async
-    #: Псевдоним для :attr:`download_mds`
-    downloadMds = download_mds
-    #: Псевдоним для :attr:`download_mds_async`
-    downloadMdsAsync = download_mds_async
+    #: Псевдоним для :attr:`download_async`
+    downloadAsync = download_async
+    #: Псевдоним для :attr:`download_bytes`
+    downloadBytes = download_bytes
+    #: Псевдоним для :attr:`download_bytes_async`
+    downloadBytesAsync = download_bytes_async
+    #: Псевдоним для :attr:`get_url`
+    getUrl = get_url
```

### Comparing `yandex-music-2.0.1/yandex_music/shot/shot_event.py` & `yandex-music-2.1.0/yandex_music/shot/shot_event.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/shot/shot_type.py` & `yandex-music-2.1.0/yandex_music/shot/shot_type.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/supplement/lyrics.py` & `yandex-music-2.1.0/yandex_music/supplement/lyrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,18 @@
     from yandex_music import Client
 
 
 @model
 class Lyrics(YandexMusicObject):
     """Класс, представляющий текст трека.
 
+    Warning:
+        Получение текста из дополнительной информации устарело. Используйте
+        :func:`yandex_music.Client.tracks_lyrics`.
+
     Attributes:
         id (:obj:`int`): Уникальный идентификатор текста трека.
         lyrics (:obj:`str`): Первые строки текст песни.
         has_rights (:obj:`bool`): Есть ли права.
         full_lyrics (:obj:`str`): Текст песни.
         show_translation (:obj:`bool`): Доступен ли перевод.
         text_language (:obj:`str`, optional): Язык песни.
```

### Comparing `yandex-music-2.0.1/yandex_music/supplement/supplement.py` & `yandex-music-2.1.0/yandex_music/supplement/supplement.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,18 @@
     from yandex_music import Client, Lyrics, VideoSupplement
 
 
 @model
 class Supplement(YandexMusicObject):
     """Класс, представляющий дополнительную информацию о треке.
 
+    Warning:
+        Получение текста из дополнительной информации устарело. Используйте
+        :func:`yandex_music.Client.tracks_lyrics`.
+
     Attributes:
         id (:obj:`int`): Уникальный идентификатор дополнительной информации.
         lyrics (:obj:`yandex_music.Lyrics`): Текст песни.
         videos (:obj:`yandex_music.VideoSupplement`): Видео.
         radio_is_available (:obj:`bool`, optional): Доступно ли радио.
         description (:obj:`str`, optional): Полное описание эпизода подкаста.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
```

### Comparing `yandex-music-2.0.1/yandex_music/supplement/video_supplement.py` & `yandex-music-2.1.0/yandex_music/supplement/video_supplement.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/track/licence_text_part.py` & `yandex-music-2.1.0/yandex_music/track/licence_text_part.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/track/major.py` & `yandex-music-2.1.0/yandex_music/track/major.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/track/meta_data.py` & `yandex-music-2.1.0/yandex_music/track/meta_data.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/track/normalization.py` & `yandex-music-2.1.0/yandex_music/track/normalization.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/track/poetry_lover_match.py` & `yandex-music-2.1.0/yandex_music/track/poetry_lover_match.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/track/track.py` & `yandex-music-2.1.0/yandex_music/album/album.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,363 +1,362 @@
-from typing import TYPE_CHECKING, Optional, List, Union
+from typing import Any, TYPE_CHECKING, Optional, List, Union
 
 from yandex_music import YandexMusicObject
 from yandex_music.utils import model
-from yandex_music.exceptions import InvalidBitrateError
 
 if TYPE_CHECKING:
-    from yandex_music import (
-        Client,
-        Normalization,
-        Major,
-        Album,
-        Artist,
-        Supplement,
-        DownloadInfo,
-        User,
-        MetaData,
-        PoetryLoverMatch,
-    )
+    from yandex_music import Client, Artist, Label, TrackPosition, Track, Deprecation
 
 
 @model
-class Track(YandexMusicObject):
-    """Класс, представляющий трек.
+class Album(YandexMusicObject):
+    """Класс, представляющий альбом.
 
     Note:
-        Известные значения поля `content_warning`: `explicit`.
+        Известные типы альбома: `single` - сингл, `compilation` - сборник.
 
-        Известные значения поля `type`: `music`.
+        Известные предупреждения о содержимом: `explicit` - ненормативная лексика.
 
-        Поля `can_publish`, `state`, `desired_visibility`, `filename`, `user_info` доступны только у треков что были
-        загружены пользователем.
+        Известные ошибки: `not-found` - альбом с таким ID не существует.
 
-        Обычно у подкастов поле `remember_position == True`, а у треков `remember_position == False`.
+        Известные значения поля `meta_type`: `music`.
 
-        Полное описание можно получить используя :func:`Track.get_supplement`.
+        Известные значения поля `available_for_options`: `bookmate`.
 
     Attributes:
-        id (:obj:`int` | :obj:`str`): Уникальный идентификатор.
-        title (:obj:`str`, optional): Название.
-        available (:obj:`bool`, optional): Доступен ли для прослушивания.
-        artists (:obj:`list` из :obj:`yandex_music.Artist`, optional): Исполнители.
-        albums (:obj:`list` из :obj:`yandex_music.Album`, optional): Альбомы.
-        available_for_premium_users (:obj:`bool`, optional): Доступен ли для пользователей с подпиской.
-        lyrics_available (:obj:`bool`, optional): Доступен ли текст песни.
-        poetry_lover_matches (:obj:`list` из :obj:`yandex_music.PoetryLoverMatch`, optional): Список слов TODO.
-        best (:obj:`bool`, optional): Лучшей ли трек TODO.
-        real_id (:obj:`int` | :obj:`str`, optional): TODO.
-        og_image (:obj:`str`, optional): Ссылка на превью Open Graph.
-        type (:obj:`str`, optional): Тип.
-        cover_uri (:obj:`str`, optional): Ссылка на изображение с обложкой.
-        major (:obj:`yandex_music.Major`, optional): Мейджор-лейбл.
-        duration_ms (:obj:`int`, optional): Длительность трека в миллисекундах.
+        id (:obj:`int`, optional): Идентификатор альбома.
+        error (:obj:`str`, optional): Ошибка получения альбома.
+        title (:obj:`str`, optional): Название альбома.
+        track_count (:obj:`int`, optional): Количество треков.
+        artists (:obj:`list` из :obj:`yandex_music.Artist`, optional): Артисты.
+        labels (:obj:`list` из :obj:`yandex_music.Label` или :obj:`str`, optional): Лейблы.
+        available (:obj:`bool`, optional): Доступен ли альбом.
+        available_for_premium_users (:obj:`bool`, optional): Доступен ли альбом для пользователей с подпиской.
+        version (:obj:`str`, optional): Дополнительная информация об альбоме.
+        cover_uri (:obj:`str`, optional): Ссылка на обложку.
+        content_warning (:obj:`str`, optional): Предупреждение о содержимом альбома.
+        original_release_year: TODO.
+        genre (:obj:`str`, optional): Жанр музыки.
+        text_color (:obj:`str`, optional): Цвет текста описания.
+        short_description (:obj:`str`, optional): Короткое описание.
+        description (:obj:`str`, optional): Описание.
+        is_premiere (:obj:`bool`, optional): Премьера ли.
+        is_banner (:obj:`bool`, optional): Является ли баннером.
+        meta_type (:obj:`str`, optional): Мета тип TODO.
         storage_dir (:obj:`str`, optional): В какой папке на сервере хранится файл TODO.
-        file_size (:obj:`int`, optional): Размер файла. TODO добавить единицу измерения.
-        substituted (:obj:`yandex_music.Track`, optional): Замещённый трек.
-        matched_track (:obj:`yandex_music.Track`, optional): Соответствующий трек TODO.
-        normalization (:obj:`list` из :obj:`yandex_music.Normalization`, optional): Значения для нормализации трека.
-        error (:obj:`str`, optional): Сообщение об ошибке.
-        can_publish (:obj:`bool`, optional): Может ли быть опубликован.
-        state (:obj:`str`, optional): Состояние, например, playable.
-        desired_visibility (:obj:`str`, optional): Видимость трека.
-        filename (:obj:`str`, optional): Название файла.
-        user_info (:obj:`yandex_music.User`, optional): Информация о пользователе, который загрузил трек.
-        meta_data (:obj:`yandex_music.MetaData`, optional): Информация о метаданных трека.
-        regions (:obj:`list` из :obj:`str`, optional): Регион TODO.
+        og_image (:obj:`str`, optional): Ссылка на превью Open Graph.
+        recent (:obj:`bool`, optional): Является ли альбом новым.
+        very_important (:obj:`bool`, optional): Популярен ли альбом у слушателей.
+        available_for_mobile (:obj:`bool`, optional): Доступен ли альбом из приложения для телефона.
+        available_partially (:obj:`bool`, optional): Доступен ли альбом частично для пользователей без подписки.
+        bests (:obj:`list` из :obj:`int`, optional): ID лучших треков альбома.
+        duplicates (:obj:`list` из :obj:`yandex_music.Album`, optional): Альбомы-дубликаты.
+        prerolls (:obj:`list`, optional): Прероллы TODO.
+        volumes (:obj:`list` из :obj:`list` из :obj:`Track`, optional): Треки альбома, разделённые по дискам.
+        year (:obj:`int`, optional): Год релиза.
+        release_date (:obj:`str`, optional): Дата релиза в формате ISO 8601.
+        type (:obj:`str`, optional): Тип альбома.
+        track_position (:obj:`yandex_music.TrackPosition`, optional): Позиция трека в альбоме. Возвращается при
+            получении альбома в составе трека.
+        regions (:obj:`list` из :obj:`str`, optional): Список регионов в которых доступен альбом.
         available_as_rbt (:obj:`bool`, optional): TODO.
-        content_warning (:obj:`str`, optional): Тип откровенного контента.
-        explicit (:obj:`bool`, optional): Содержит ли откровенный контент.
-        preview_duration_ms (:obj:`int`, optional): TODO.
-        available_full_without_permission (:obj:`bool`, optional): Доступен ли без подписки.
-        version (:obj:`str`, optional): Версия.
-        remember_position (:obj:`bool`, optional): Если :obj:`True`, то запоминатся последняя позиция прослушивания,
-            иначе позиция не запоминается.
-        background_video_uri (:obj:`str`, optional): Ссылка на видеошот.
-        short_description (:obj:`str`, optional): Краткое опсание эпизода подкаста.
-        is_suitable_for_children (:obj:`bool`, optional): Подходит ли для детей TODO.
-        client (:obj:`yandex_music.Client`): Клиент Yandex Music.
+        lyrics_available (:obj:`bool`, optional): Доступны ли слова TODO.
+        remember_position (:obj:`bool`, optional): Запоминание позиции TODO.
+        albums (:obj:`list` из :obj:`yandex_music.Album`, optional): Альбомы TODO.
+        duration_ms (:obj:`int`, optional): Длительность в миллисекундах.
+        explicit (:obj:`bool`, optional): Есть ли в треке ненормативная лексика.
+        start_date (:obj:`str`, optional): Дата начала в формате ISO 8601 TODO.
+        likes_count (:obj:`int`, optional): Количество лайков TODO.
+        deprecation (:obj:`yandex_music.Deprecation`, optional): TODO.
+        available_regions (:obj:`list` из :obj:`str`, optional): Регионы, где доступен альбом.
+        available_for_options (:obj:`list` из :obj:`str`, optional): Возможные опции для альбома.
+        client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
-    id: Union[str, int]
+    id: Optional[int] = None
+    error: Optional[str] = None
     title: Optional[str] = None
-    available: Optional[bool] = None
+    track_count: Optional[int] = None
     artists: List['Artist'] = None
-    albums: List['Album'] = None
+    labels: List[Union['Label', str]] = None
+    available: Optional[bool] = None
     available_for_premium_users: Optional[bool] = None
-    lyrics_available: Optional[bool] = None
-    poetry_lover_matches: List['PoetryLoverMatch'] = None
-    best: Optional[bool] = None
-    real_id: Optional[Union[str, int]] = None
-    og_image: Optional[str] = None
-    type: Optional[str] = None
+    version: Optional[str] = None
     cover_uri: Optional[str] = None
-    major: Optional['Major'] = None
-    duration_ms: Optional[int] = None
+    content_warning: Optional[str] = None
+    original_release_year: Any = None
+    genre: Optional[str] = None
+    text_color: Optional[str] = None
+    short_description: Optional[str] = None
+    description: Optional[str] = None
+    is_premiere: Optional[bool] = None
+    is_banner: Optional[bool] = None
+    meta_type: Optional[str] = None
     storage_dir: Optional[str] = None
-    file_size: Optional[int] = None
-    substituted: Optional['Track'] = None
-    matched_track: Optional['Track'] = None
-    normalization: Optional['Normalization'] = None
-    error: Optional[str] = None
-    can_publish: Optional[bool] = None
-    state: Optional[str] = None
-    desired_visibility: Optional[str] = None
-    filename: Optional[str] = None
-    user_info: Optional['User'] = None
-    meta_data: Optional['MetaData'] = None
+    og_image: Optional[str] = None
+    buy: Optional[list] = None
+    recent: Optional[bool] = None
+    very_important: Optional[bool] = None
+    available_for_mobile: Optional[bool] = None
+    available_partially: Optional[bool] = None
+    bests: Optional[List[int]] = None
+    duplicates: List['Album'] = None
+    prerolls: Optional[list] = None
+    volumes: Optional[List[List['Track']]] = None
+    year: Optional[int] = None
+    release_date: Optional[str] = None
+    type: Optional[str] = None
+    track_position: Optional['TrackPosition'] = None
     regions: Optional[List[str]] = None
     available_as_rbt: Optional[bool] = None
-    content_warning: Optional[str] = None
-    explicit: Optional[bool] = None
-    preview_duration_ms: Optional[int] = None
-    available_full_without_permission: Optional[bool] = None
-    version: Optional[str] = None
+    lyrics_available: Optional[bool] = None
     remember_position: Optional[bool] = None
-    background_video_uri: Optional[str] = None
-    short_description: Optional[str] = None
-    is_suitable_for_children: Optional[bool] = None
+    albums: Optional[List['Album']] = None
+    duration_ms: Optional[int] = None
+    explicit: Optional[bool] = None
+    start_date: Optional[str] = None
+    likes_count: Optional[int] = None
+    deprecation: Optional['Deprecation'] = None
+    available_regions: Optional[List[str]] = None
+    available_for_options: Optional[List[str]] = None
     client: Optional['Client'] = None
 
     def __post_init__(self):
-        self.download_info = None
         self._id_attrs = (self.id,)
 
-    def get_download_info(self, get_direct_links=False) -> List['DownloadInfo']:
+    def with_tracks(self, *args, **kwargs) -> Optional['Album']:
         """Сокращение для::
 
-        client.tracks_download_info(self.track_id, get_direct_links)
+        client.albums_with_tracks(album.id, *args, **kwargs)
         """
-        self.download_info = self.client.tracks_download_info(self.track_id, get_direct_links)
-
-        return self.download_info
+        return self.client.albums_with_tracks(self.id, *args, **kwargs)
 
-    async def get_download_info_async(self, get_direct_links=False) -> List['DownloadInfo']:
+    async def with_tracks_async(self, *args, **kwargs) -> Optional['Album']:
         """Сокращение для::
 
-        await client.tracks_download_info(self.track_id, get_direct_links)
+        await client.albums_with_tracks(album.id, *args, **kwargs)
         """
-        self.download_info = await self.client.tracks_download_info(self.track_id, get_direct_links)
+        return await self.client.albums_with_tracks(self.id, *args, **kwargs)
 
-        return self.download_info
+    def get_cover_url(self, size: str = '200x200') -> str:
+        """Возвращает URL обложки.
 
-    def get_supplement(self, *args, **kwargs) -> Optional['Supplement']:
-        """Сокращение для::
+        Args:
+            size (:obj:`str`, optional): Размер обложки.
 
-        client.track_supplement(track.id, *args, **kwargs)
+        Returns:
+            :obj:`str`: URL обложки.
         """
-        return self.client.track_supplement(self.id, *args, **kwargs)
+        return f'https://{self.cover_uri.replace("%%", size)}'
 
-    async def get_supplement_async(self, *args, **kwargs) -> Optional['Supplement']:
-        """Сокращение для::
+    def get_og_image_url(self, size: str = '200x200') -> str:
+        """Возвращает URL OG обложки.
 
-        await client.track_supplement(track.id, *args, **kwargs)
+        Args:
+            size (:obj:`str`, optional): Размер обложки.
+
+        Returns:
+            :obj:`str`: URL обложки.
         """
-        return await self.client.track_supplement(self.id, *args, **kwargs)
+        return f'https://{self.og_image.replace("%%", size)}'
 
     def download_cover(self, filename: str, size: str = '200x200') -> None:
         """Загрузка обложки.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             size (:obj:`str`, optional): Размер обложки.
         """
-        self.client.request.download(f'https://{self.cover_uri.replace("%%", size)}', filename)
+        self.client.request.download(self.get_cover_url(size), filename)
 
     async def download_cover_async(self, filename: str, size: str = '200x200') -> None:
         """Загрузка обложки.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             size (:obj:`str`, optional): Размер обложки.
         """
-        await self.client.request.download(f'https://{self.cover_uri.replace("%%", size)}', filename)
+        await self.client.request.download(self.get_cover_url(size), filename)
 
     def download_og_image(self, filename: str, size: str = '200x200') -> None:
         """Загрузка обложки.
 
         Предпочтительнее использовать `self.download_cover()`.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             size (:obj:`str`, optional): Размер обложки.
         """
-        self.client.request.download(f'https://{self.og_image.replace("%%", size)}', filename)
+        self.client.request.download(self.get_og_image_url(size), filename)
 
     async def download_og_image_async(self, filename: str, size: str = '200x200') -> None:
         """Загрузка обложки.
 
         Предпочтительнее использовать `self.download_cover_async()`.
 
         Args:
             filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
             size (:obj:`str`, optional): Размер обложки.
         """
-        await self.client.request.download(f'https://{self.og_image.replace("%%", size)}', filename)
+        await self.client.request.download(self.get_og_image_url(size), filename)
 
-    def download(self, filename: str, codec: str = 'mp3', bitrate_in_kbps: int = 192) -> None:
-        """Загрузка трека.
+    def download_cover_bytes(self, size: str = '200x200') -> bytes:
+        """Загрузка обложки и возврат в виде байтов.
+
+        Args:
+            size (:obj:`str`, optional): Размер обложки.
 
-        Note:
-            Известные значения `codec`: `mp3`, `aac`.
+        Returns:
+            :obj:`bytes`: Обложка в виде байтов.
+        """
+        return self.client.request.retrieve(self.get_cover_url(size))
 
-            Известные значения `bitrate_in_kbps`: `64`, `128`, `192`, `320`.
+    async def download_cover_bytes_async(self, size: str = '200x200') -> bytes:
+        """Загрузка обложки и возврат в виде байтов.
 
         Args:
-            filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-            codec (:obj:`str`, optional): Кодек из доступных в `self.download_info`.
-            bitrate_in_kbps (:obj:`int`, optional): Битрейт из доступных в `self.download_info` для данного кодека.
+            size (:obj:`str`, optional): Размер обложки.
 
-        Raises:
-            :class:`yandex_music.exceptions.InvalidBitrateError`: Если в `self.download_info` не найден подходящий трек.
+        Returns:
+            :obj:`bytes`: Обложка в виде байтов.
         """
-        if self.download_info is None:
-            self.get_download_info()
+        return await self.client.request.retrieve(self.get_cover_url(size))
 
-        for info in self.download_info:
-            if info.codec == codec and info.bitrate_in_kbps == bitrate_in_kbps:
-                info.download(filename)
-                break
-        else:
-            raise InvalidBitrateError('Unavailable bitrate')
+    def download_og_image_bytes(self, size: str = '200x200') -> bytes:
+        """Загрузка обложки и возврат в виде байтов.
 
-    async def download_async(self, filename: str, codec: str = 'mp3', bitrate_in_kbps: int = 192) -> None:
-        """Загрузка трека.
+        Предпочтительнее использовать `self.download_cover()`.
 
-        Note:
-            Известные значения `codec`: `mp3`, `aac`.
+        Args:
+            size (:obj:`str`, optional): Размер обложки.
+
+        Returns:
+            :obj:`bytes`: Обложка в виде байтов.
+        """
+        return self.client.request.retrieve(self.get_og_image_url(size))
 
-            Известные значения `bitrate_in_kbps`: `64`, `128`, `192`, `320`.
+    async def download_og_image_bytes_async(self, size: str = '200x200') -> bytes:
+        """Загрузка обложки и возврат в виде байтов.
+
+        Предпочтительнее использовать `self.download_cover_async()`.
 
         Args:
-            filename (:obj:`str`): Путь для сохранения файла с названием и расширением.
-            codec (:obj:`str`, optional): Кодек из доступных в `self.download_info`.
-            bitrate_in_kbps (:obj:`int`, optional): Битрейт из доступных в `self.download_info` для данного кодека.
+            size (:obj:`str`, optional): Размер обложки.
 
-        Raises:
-            :class:`yandex_music.exceptions.InvalidBitrateError`: Если в `self.download_info` не найден подходящий трек.
+        Returns:
+            :obj:`bytes`: Обложка в виде байтов.
         """
-        if self.download_info is None:
-            await self.get_download_info_async()
-
-        for info in self.download_info:
-            if info.codec == codec and info.bitrate_in_kbps == bitrate_in_kbps:
-                await info.download_async(filename)
-                break
-        else:
-            raise InvalidBitrateError('Unavailable bitrate')
+        return await self.client.request.retrieve(self.get_og_image_url(size))
 
     def like(self, *args, **kwargs) -> bool:
         """Сокращение для::
 
-        client.users_likes_tracks_add(track.id, user.id, *args, **kwargs)
+        client.users_likes_albums_add(album.id, user.id *args, **kwargs)
         """
-        return self.client.users_likes_tracks_add(self.track_id, self.client.me.account.uid, *args, **kwargs)
+        return self.client.users_likes_albums_add(self.id, self.client.me.account.uid, *args, **kwargs)
 
     async def like_async(self, *args, **kwargs) -> bool:
         """Сокращение для::
 
-        await client.users_likes_tracks_add(track.id, user.id, *args, **kwargs)
+        await client.users_likes_albums_add(album.id, user.id *args, **kwargs)
         """
-        return await self.client.users_likes_tracks_add(self.track_id, self.client.me.account.uid, *args, **kwargs)
+        return await self.client.users_likes_albums_add(self.id, self.client.me.account.uid, *args, **kwargs)
 
     def dislike(self, *args, **kwargs) -> bool:
         """Сокращение для::
 
-        client.users_likes_tracks_remove(track.id, user.id *args, **kwargs)
+        client.users_likes_albums_remove(album.id, user.id *args, **kwargs)
         """
-        return self.client.users_likes_tracks_remove(self.track_id, self.client.me.account.uid, *args, **kwargs)
+        return self.client.users_likes_albums_remove(self.id, self.client.me.account.uid, *args, **kwargs)
 
     async def dislike_async(self, *args, **kwargs) -> bool:
         """Сокращение для::
 
-        await client.users_likes_tracks_remove(track.id, user.id *args, **kwargs)
+        await client.users_likes_albums_remove(album.id, user.id *args, **kwargs)
         """
-        return await self.client.users_likes_tracks_remove(self.track_id, self.client.me.account.uid, *args, **kwargs)
+        return await self.client.users_likes_albums_remove(self.id, self.client.me.account.uid, *args, **kwargs)
 
     def artists_name(self) -> List[str]:
         """Получает имена всех исполнителей.
 
         Returns:
               :obj:`list` из :obj:`str`: Имена исполнителей.
         """
 
         return [i.name for i in self.artists]
 
-    @property
-    def track_id(self) -> str:
-        """:obj:`str`: Уникальный идентификатор трека состоящий из его номера и номера альбома или просто из номера."""
-        if self.albums:
-            return f'{self.id}:{self.albums[0].id}'
-        return f'{self.id}'
-
     @classmethod
-    def de_json(cls, data: dict, client: 'Client') -> Optional['Track']:
+    def de_json(cls, data: dict, client: 'Client') -> Optional['Album']:
         """Десериализация объекта.
 
         Args:
             data (:obj:`dict`): Поля и значения десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`yandex_music.Track`: Трек.
+            :obj:`yandex_music.Album`: Альбом.
         """
         if not data:
             return None
 
-        data = super(Track, cls).de_json(data, client)
-        from yandex_music import Normalization, Major, Album, Artist, User, MetaData, PoetryLoverMatch
+        data = super(Album, cls).de_json(data, client)
+        from yandex_music import Artist, Label, TrackPosition, Track, Deprecation
 
-        data['albums'] = Album.de_list(data.get('albums'), client)
         data['artists'] = Artist.de_list(data.get('artists'), client)
-        data['normalization'] = Normalization.de_json(data.get('normalization'), client)
-        data['major'] = Major.de_json(data.get('major'), client)
-        data['substituted'] = Track.de_json(data.get('substituted'), client)
-        data['matched_track'] = Track.de_json(data.get('matched_track'), client)
-        data['user_info'] = User.de_json(data.get('user_info'), client)
-        data['meta_data'] = MetaData.de_json(data.get('meta_data'), client)
-        data['poetry_lover_matches'] = PoetryLoverMatch.de_list(data.get('poetry_lover_matches'), client)
+        data['labels'] = Label.de_list(data.get('labels'), client)
+        data['track_position'] = TrackPosition.de_json(data.get('track_position'), client)
+        data['duplicates'] = Album.de_list(data.get('duplicates'), client)
+        data['albums'] = Album.de_list(data.get('albums'), client)
+        data['deprecation'] = Deprecation.de_json(data.get('deprecation'), client)
+        if data.get('volumes'):
+            data['volumes'] = [Track.de_list(i, client) for i in data['volumes']]
 
         return cls(client=client, **data)
 
     @classmethod
-    def de_list(cls, data: dict, client: 'Client') -> List['Track']:
+    def de_list(cls, data: dict, client: 'Client') -> List['Album']:
         """Десериализация списка объектов.
 
         Args:
             data (:obj:`list`): Список словарей с полями и значениями десериализуемого объекта.
             client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
 
         Returns:
-            :obj:`list` из :obj:`yandex_music.Track`: Треки.
+            :obj:`list` из :obj:`yandex_music.Album`: Альбомы.
         """
         if not data:
             return []
 
-        return [cls.de_json(track, client) for track in data]
+        return [cls.de_json(album, client) for album in data]
 
     # camelCase псевдонимы
 
-    #: Псевдоним для :attr:`get_download_info`
-    getDownloadInfo = get_download_info
-    #: Псевдоним для :attr:`get_download_info_async`
-    getDownloadInfoAsync = get_download_info_async
-    #: Псевдоним для :attr:`get_supplement`
-    getSupplement = get_supplement
-    #: Псевдоним для :attr:`get_supplement_async`
-    getSupplementAsync = get_supplement_async
+    #: Псевдоним для :attr:`with_tracks`
+    withTracks = with_tracks
+    #: Псевдоним для :attr:`with_tracks_async`
+    withTracksAsync = with_tracks_async
+    #: Псевдоним для :attr:`get_cover_url`
+    getCoverUrl = get_cover_url
+    #: Псевдоним для :attr:`get_og_image_url`
+    getOgImageUrl = get_og_image_url
     #: Псевдоним для :attr:`download_cover`
     downloadCover = download_cover
     #: Псевдоним для :attr:`download_cover_async`
     downloadCoverAsync = download_cover_async
     #: Псевдоним для :attr:`download_og_image`
     downloadOgImage = download_og_image
     #: Псевдоним для :attr:`download_og_image_async`
     downloadOgImageAsync = download_og_image_async
-    #: Псевдоним для :attr:`track_id`
-    trackId = track_id
+    #: Псевдоним для :attr:`download_cover_bytes`
+    downloadCoverBytes = download_cover_bytes
+    #: Псевдоним для :attr:`download_cover_bytes_async`
+    downloadCoverBytesAsync = download_cover_bytes_async
+    #: Псевдоним для :attr:`download_og_image_bytes`
+    downloadOgImageBytes = download_og_image_bytes
+    #: Псевдоним для :attr:`download_og_image_bytes_async`
+    downloadOgImageBytesAsync = download_og_image_bytes_async
     #: Псевдоним для :attr:`like_async`
     likeAsync = like_async
     #: Псевдоним для :attr:`dislike_async`
-    dislike_async = dislike_async
-    #: Псевдоним для :attr:`download_async`
-    downloadAsync = download_async
+    dislikeAsync = dislike_async
+    #: Псевдоним для :attr:`artists_name`
+    artistsName = artists_name
```

### Comparing `yandex-music-2.0.1/yandex_music/track/tracks_similar.py` & `yandex-music-2.1.0/yandex_music/track/tracks_similar.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/track_short.py` & `yandex-music-2.1.0/yandex_music/track_short.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,24 +18,26 @@
         id (:obj:`str`): Уникальный идентификатор трека.
         timestamp (:obj:`str`): Дата TODO.
         album_id (:obj:`str`, optional): Уникальный идентификатор альбома.
         play_count (:obj:`int`, optional): Количество проигрываний.
         recent (:obj:`bool`, optional): Недавний.
         chart (:obj:`yandex_music.Chart`, optional): Позиция в чарте.
         track (:obj:`yandex_music.Track`, optional): Полная версия трека.
+        original_index (:obj:`int`, optional): Индекс в плейлисте или альбоме. TODO уточнить про альбом.
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
     """
 
     id: Union[str, int]
     timestamp: str
     album_id: Optional[str] = None
     play_count: Optional[int] = None
     recent: Optional[bool] = None
     chart: Optional['Chart'] = None
     track: Optional['Track'] = None
+    original_index: Optional[int] = None
     client: Optional['Client'] = None
 
     def __post_init__(self):
         self._id_attrs = (self.id, self.album_id)
 
     def fetch_track(self) -> 'Track':
         """Получение полной версии трека.
```

### Comparing `yandex-music-2.0.1/yandex_music/tracks_list.py` & `yandex-music-2.1.0/yandex_music/tracks_list.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/utils/difference.py` & `yandex-music-2.1.0/yandex_music/utils/difference.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,20 +71,24 @@
         Args:
             at (:obj:`int`): Индекс для вставки.
             tracks (:obj:`dict` | :obj:`list: из :obj:`dict`): Словарь уникальными идентификаторами треков.
 
         Returns:
             :obj:`yandex_music.utils.difference.Difference`: Набор операций над плейлистом.
         """
-        # TODO принимать TrackId, а так же строку и сплитить её по ":". При отсутствии album_id кидать исключение.
+        # TODO (MarshalX) принимать TrackId, а так же строку и сплитить её по ":".
+        #  При отсутствии album_id кидать исключение.
+        #  https://github.com/MarshalX/yandex-music-api/issues/558
         if not isinstance(tracks, list):
             tracks = [tracks]
 
         operation = {'op': Operation.INSERT.value, 'at': at, 'tracks': []}
 
         for track in tracks:
-            track = type('TrackId', (), track)  # TODO replace to normal TrackId object
+            # TODO (MarshalX) replace to normal TrackId object
+            #  https://github.com/MarshalX/yandex-music-api/issues/558
+            track = type('TrackId', (), track)
 
             operation['tracks'].append({'id': track.id, 'albumId': track.album_id})
 
         self.operations.append(operation)
         return self
```

### Comparing `yandex-music-2.0.1/yandex_music/utils/request.py` & `yandex-music-2.1.0/yandex_music/utils/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,33 +25,39 @@
     from yandex_music import Client
 
 
 USER_AGENT = 'Yandex-Music-API'
 HEADERS = {
     'X-Yandex-Music-Client': 'YandexMusicAndroid/23020251',
 }
+DEFAULT_TIMEOUT = 5
 
 reserved_names = keyword.kwlist + ['client']
 
 logging.getLogger('urllib3').setLevel(logging.WARNING)
 
+default_timeout = object()
+
 
 class Request:
     """Вспомогательный класс для yandex_music, представляющий методы для выполнения POST и GET запросов, скачивания
     файлов.
 
     Args:
         client (:obj:`yandex_music.Client`, optional): Клиент Yandex Music.
         headers (:obj:`dict`, optional): Заголовки передаваемые с каждым запросом.
         proxy_url (:obj:`str`, optional): Прокси.
     """
 
-    def __init__(self, client=None, headers=None, proxy_url=None):
+    def __init__(self, client=None, headers=None, proxy_url=None, timeout=default_timeout):
         self.headers = headers or HEADERS.copy()
 
+        self._timeout = DEFAULT_TIMEOUT
+        self.set_timeout(timeout)
+
         self.client = self.set_and_return_client(client)
 
         # aiohttp
         self.proxy_url = proxy_url
 
         # requests
         self.proxies = {'http': proxy_url, 'https': proxy_url} if proxy_url else None
@@ -63,14 +69,24 @@
             Возможные значения `lang`: en/uz/uk/us/ru/kk/hy.
 
         Args:
             lang (:obj:`str`): Язык.
         """
         self.headers.update({'Accept-Language': lang})
 
+    def set_timeout(self, timeout: Union[int, float, object] = default_timeout):
+        """Устанавливает время ожидания для всех запросов.
+
+        Args:
+            timeout (:obj:`int` | :obj:`float`): Время ожидания от сервера.
+        """
+        self._timeout = timeout
+        if timeout is default_timeout:
+            self._timeout = DEFAULT_TIMEOUT
+
     def set_authorization(self, token: str) -> None:
         """Добавляет заголовок авторизации для каждого запроса.
 
         Note:
             Используется при передаче своего экземпляра Request'a клиенту.
 
         Args:
@@ -188,14 +204,17 @@
             :class:`yandex_music.exceptions.NetworkError`: При проблемах с сетью.
         """
         if 'headers' not in kwargs:
             kwargs['headers'] = {}
 
         kwargs['headers']['User-Agent'] = USER_AGENT
 
+        if kwargs['timeout'] is default_timeout:
+            kwargs['timeout'] = self._timeout
+
         try:
             resp = requests.request(*args, **kwargs)
         except requests.Timeout:
             raise TimedOutError()
         except requests.RequestException as e:
             raise NetworkError(e)
 
@@ -218,15 +237,17 @@
             raise NetworkError(message)
 
         elif resp.status_code == 502:
             raise NetworkError('Bad Gateway')
         else:
             raise NetworkError(f'{message} ({resp.status_code}): {resp.content}')
 
-    def get(self, url: str, params: dict = None, timeout: Union[int, float] = 5, *args, **kwargs) -> Union[dict, str]:
+    def get(
+        self, url: str, params: dict = None, timeout: Union[int, float] = default_timeout, *args, **kwargs
+    ) -> Union[dict, str]:
         """Отправка GET запроса.
 
         Args:
             url (:obj:`str`): Адрес для запроса.
             params (:obj:`str`): GET параметры для запроса.
             timeout (:obj:`int` | :obj:`float`): Используется как время ожидания ответа от сервера вместо указанного
                 при создании пула.
@@ -241,15 +262,15 @@
         """
         result = self._request_wrapper(
             'GET', url, params=params, headers=self.headers, proxies=self.proxies, timeout=timeout, *args, **kwargs
         )
 
         return self._parse(result).get_result()
 
-    def post(self, url, data=None, timeout=5, *args, **kwargs) -> Union[dict, str]:
+    def post(self, url, data=None, timeout=default_timeout, *args, **kwargs) -> Union[dict, str]:
         """Отправка POST запроса.
 
         Args:
             url (:obj:`str`): Адрес для запроса.
             data (:obj:`str`): POST тело запроса.
             timeout (:obj:`int` | :obj:`float`): Используется как время ожидания ответа от сервера вместо указанного
                 при создании пула.
@@ -264,15 +285,15 @@
         """
         result = self._request_wrapper(
             'POST', url, headers=self.headers, proxies=self.proxies, data=data, timeout=timeout, *args, **kwargs
         )
 
         return self._parse(result).get_result()
 
-    def retrieve(self, url, timeout=5, *args, **kwargs) -> bytes:
+    def retrieve(self, url, timeout=default_timeout, *args, **kwargs) -> bytes:
         """Отправка GET запроса и получение содержимого без обработки (парсинга).
 
         Args:
             url (:obj:`str`): Адрес для запроса.
             timeout (:obj:`int` | :obj:`float`): Используется как время ожидания ответа от сервера вместо указанного
                 при создании пула.
             *args: Произвольные аргументы для `requests.request`.
@@ -282,15 +303,15 @@
             :obj:`bytes`: Тело ответа.
 
         Raises:
             :class:`yandex_music.exceptions.YandexMusicError`: Базовое исключение библиотеки.
         """
         return self._request_wrapper('GET', url, proxies=self.proxies, timeout=timeout, *args, **kwargs)
 
-    def download(self, url, filename, timeout=5, *args, **kwargs) -> None:
+    def download(self, url, filename, timeout=default_timeout, *args, **kwargs) -> None:
         """Отправка запроса на получение содержимого и его запись в файл.
 
         Args:
             url (:obj:`str`): Адрес для запроса.
             filename (:obj:`str`): Путь и(или) название файла вместе с расширением.
             timeout (:obj:`int` | :obj:`float`): Используется как время ожидания ответа от сервера вместо указанного
                 при создании пула.
```

### Comparing `yandex-music-2.0.1/yandex_music/utils/response.py` & `yandex-music-2.1.0/yandex_music/utils/response.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music/video.py` & `yandex-music-2.1.0/yandex_music/video.py`

 * *Files identical despite different names*

### Comparing `yandex-music-2.0.1/yandex_music.egg-info/PKG-INFO` & `yandex-music-2.1.0/yandex_music.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,449 +1,320 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: yandex-music
-Version: 2.0.1
+Version: 2.1.0
 Summary: Неофициальная Python библиотека для работы с API сервиса Яндекс.Музыка.
 Home-page: https://github.com/MarshalX/yandex-music-api/
-Author: Il`ya Semyonov
+Author: Ilya (Marshal)
 Author-email: ilya@marshal.dev
 License: LGPLv3
-Project-URL: Code, https://github.com/MarshalX/yandex-music-api
-Project-URL: Documentation, https://yandex-music.readthedocs.io
-Project-URL: Chat, https://t.me/yandex_music_api
+Project-URL: Documentation, https://yandex-music.rtfd.io
+Project-URL: Telegram chat, https://t.me/yandex_music_api
 Project-URL: Codecov, https://codecov.io/gh/MarshalX/yandex-music-api
-Project-URL: Codacy, https://www.codacy.com/manual/MarshalX/yandex-music-api
-Description: ================
-        Yandex Music API
-        ================
+Project-URL: Codacy, https://app.codacy.com/gh/MarshalX/yandex-music-api
+Description: ## Yandex Music API
         
-            Делаю то, что по определённым причинам не сделала компания Yandex.
+        > Делаю то, что по определённым причинам не сделала компания Yandex.
         
         ⚠️ Это неофициальная библиотека.
         
-        Сообщество разработчиков общаются и помогают друг другу
-        в `Telegram чате <https://t.me/yandex_music_api>`_, присоединяйтесь!
+        Сообщество разработчиков общаются и помогают друг другу в [Telegram чате](https://t.me/yandex_music_api), присоединяйтесь!
         
-        .. image:: https://img.shields.io/badge/python-3.7+-blue.svg
-           :target: https://pypi.org/project/yandex-music/
-           :alt: Поддерживаемые Python версии
+        [![Поддерживаемые Python версии](https://img.shields.io/badge/python-3.7+-blue.svg)](https://pypi.org/project/yandex-music/)
+        [![Покрытие кода тестами](https://codecov.io/gh/MarshalX/yandex-music-api/branch/main/graph/badge.svg)](https://codecov.io/gh/MarshalX/yandex-music-api)
+        [![Качество кода](https://api.codacy.com/project/badge/Grade/27011a5a8d9f4b278d1bfe2fe8725fed)](https://app.codacy.com/gh/MarshalX/yandex-music-api)
+        [![Статус тестов](https://github.com/MarshalX/yandex-music-api/actions/workflows/pytest_full.yml/badge.svg)](https://github.com/MarshalX/yandex-music-api/actions/workflows/pytest_full.yml)
+        [![Статус документации](https://readthedocs.org/projects/yandex-music/badge/?version=latest)](https://yandex-music.readthedocs.io/en/latest/?badge=latest)
+        [![Лицензия LGPLv3](https://img.shields.io/badge/license-LGPLv3-lightgrey.svg)](https://www.gnu.org/licenses/lgpl-3.0.html)
+        
+        ### Содержание
+          - [Введение](#введение)
+            1.  [Доступ к вашим данным Яндекс.Музыка](#доступ-к-вашим-данным-яндексмузыка)
+          - [Установка](#установка)
+          - [Начало работы](#начало-работы)
+            1.  [Изучение по примерам](#изучение-по-примерам)
+            2.  [Особенности использования асинхронного клиента](#особенности-использования-асинхронного-клиента)
+            3.  [Логирование](#логирование)
+            4.  [Документация](#документация)
+          - [Получение помощи](#получение-помощи)
+          - [Список изменений](#список-изменений)
+          - [Реализации на других языках](#реализации-на-других-языках)
+            1.  [C#](#c)
+            2.  [PHP](#php)
+            3.  [JavaScript](#javascript)
+          - [Разработанные проекты](#разработанные-проекты)
+            1.  [Плагин для Kodi](#плагин-для-kodi)
+            2.  [Telegram бот-клиент](#telegram-бот-клиент)
+          - [Благодарность](#благодарность)
+          - [Внесение своего вклада в проект](#внесение-своего-вклада-в-проект)
+          - [Спонсоры](#спонсоры)
+          - [Лицензия](#лицензия)
+        
+        ### Введение
+        
+        Эта библиотека предоставляется Python интерфейс для никем незадокументированного и сделанного только для себя API Яндекс Музыки.
+        
+        Она совместима с версиями Python 3.7+ и поддерживает работу как с синхронном, так и асинхронным (asyncio) кодом.
         
-        .. image:: https://codecov.io/gh/MarshalX/yandex-music-api/branch/main/graph/badge.svg
-           :target: https://codecov.io/gh/MarshalX/yandex-music-api
-           :alt: Покрытие кода тестами
+        В дополнение к реализации чистого API данная библиотека имеет ряд классов-обёрток объектов высокого уровня дабы сделать разработку клиентов и скриптов простой и понятной. Вся документация была написана с нуля исходя из логического анализа в ходе обратной разработки(reverse engineering) API.
         
-        .. image:: https://api.codacy.com/project/badge/Grade/27011a5a8d9f4b278d1bfe2fe8725fed
-           :target: https://www.codacy.com/manual/MarshalX/yandex-music-api
-           :alt: Качество кода
+        #### Доступ к вашим данным Яндекс.Музыка
         
-        .. image:: https://github.com/MarshalX/yandex-music-api/actions/workflows/pytest_full.yml/badge.svg
-           :target: https://github.com/MarshalX/yandex-music-api/actions/workflows/pytest_full.yml
-           :alt: Статус тестов
+        Начиная с версии [2.0.0](https://github.com/MarshalX/yandex-music-api/blob/a30082f4929e56381c870cb03103777ae29bcc6b/CHANGES.rst#%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D1%8F-200) библиотека больше не предоставляет интерфейсы для работы с OAuth Яндекс и Яндекс.Паспорт. Задача по получению токена для доступа к данным на плечах разработчиков использующих данную библиотеку. О том как получить токен читайте в документации.
         
-        .. image:: https://readthedocs.org/projects/yandex-music/badge/?version=latest
-           :target: https://yandex-music.readthedocs.io/en/latest/?badge=latest
-           :alt: Статус документации
-        
-        .. image:: https://img.shields.io/badge/license-LGPLv3-lightgrey.svg
-           :target: https://www.gnu.org/licenses/lgpl-3.0.html
-           :alt: Лицензия LGPLv3
-        
-        
-        ==========
-        Содержание
-        ==========
-        
-        - `Введение`_
-        
-          #. `Доступ к вашим данным Яндекс.Музыка`_
-        
-        - `Установка`_
-        
-        - `Начало работы`_
-        
-          #. `Изучение по примерам`_
-        
-          #. `Особенности использования асинхронного клиента`_
-        
-          #. `Логирование`_
-        
-          #. `Документация`_
-        
-        - `Получение помощи`_
-        
-        - `Список изменений`_
-        
-        - `Реализации на других языках`_
-        
-          #. `C#`_
-        
-          #. `PHP`_
-        
-          #. `JavaScript`_
-        
-        - `Разработанные проекты`_
-        
-          #. `Плагин для Kodi`_
-        
-          #. `Telegram бот-клиент`_
-        
-        - `Благодарность`_
-        
-        - `Внесение своего вклада в проект`_
-        
-        - `Лицензия`_
-        
-        ========
-        Введение
-        ========
-        
-        Эта библиотека предоставляется Python интерфейс для никем
-        незадокументированного и сделанного только для себя API Яндекс Музыки.
-        
-        Она совместима с версиями Python 3.7+ и поддерживает работу как с синхронном,
-        так и асинхронным (asyncio) кодом.
-        
-        В дополнение к реализации чистого API данная библиотека имеет ряд
-        классов-обёрток объектов высокого уровня дабы сделать разработку клиентов
-        и скриптов простой и понятной. Вся документация была написана с нуля исходя
-        из логического анализа в ходе обратной разработки (reverse engineering) API.
-        
-        -----------------------------------
-        Доступ к вашим данным Яндекс.Музыка
-        -----------------------------------
-        
-        Начиная с версии `2.0.0 <https://github.com/MarshalX/yandex-music-api/blob/main/CHANGES.rst#%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D1%8F-200>`_ библиотека больше не предоставляет интерфейсы для работы
-        с OAuth Яндекс и Яндекс.Паспорт. Задача по получению токена для доступа к данным
-        на плечах разработчиков использующих данную библиотеку.
-        
-        =========
-        Установка
-        =========
+        ### Установка
         
         Вы можете установить или обновить Yandex Music API при помощи:
         
-        .. code:: shell
-        
-            pip install yandex-music --upgrade
+        ``` shell
+        pip install -U yandex-music
+        ```
         
         Или Вы можете установить из исходного кода с помощью:
         
-        .. code:: shell
+        ``` shell
+        git clone https://github.com/MarshalX/yandex-music-api
+        cd yandex-music-api
+        python setup.py install
+        ```
         
-            git clone https://github.com/MarshalX/yandex-music-api
-            cd yandex-music-api
-            python setup.py install
-        
-        =============
-        Начало работы
-        =============
+        ### Начало работы
         
         Приступив к работе первым делом необходимо создать экземпляр клиента.
         
         Инициализация синхронного клиента:
         
-        .. code:: python
-        
-            from yandex_music import Client
+        ``` python
+        from yandex_music import Client
         
-            client = Client()
-            client.init()
+        client = Client()
+        client.init()
         
-            # или
+        # или
         
-            client = Client().init()
+        client = Client().init()
+        ```
         
         Инициализация асинхронного клиента:
         
-        .. code:: python
-        
-            from yandex_music import ClientAsync
+        ``` python
+        from yandex_music import ClientAsync
         
-            client = ClientAsync()
-            await client.init()
+        client = ClientAsync()
+        await client.init()
         
-            # или
+        # или
         
-            client = await Client().init()
+        client = await Client().init()
+        ```
         
-        Вызов ``init()`` необходим для получение информации для упрощения будущих запросов.
+        Вызов `init()` необходим для получение информации для упрощения будущих запросов.
         
-        Работа без авторизации ограничена. Так, например, для загрузки будут доступны
-        только первые 30 секунд аудиофайла. Для понимания всех ограничений зайдите на
-        сайт Яндекс.Музыка под инкогнито и воспользуйтесь сервисом.
+        Работа без авторизации ограничена. Так, например, для загрузки будут доступны только первые 30 секунд аудиофайла. Для понимания всех ограничений зайдите на сайт Яндекс.Музыка под инкогнито и воспользуйтесь сервисом.
         
-        Для доступа к своим личным данным следует авторизоваться.
-        Это осуществляется через токен аккаунта Яндекс.Музыка.
+        Для доступа к своим личным данным следует авторизоваться. Это осуществляется через токен аккаунта Яндекс.Музыка.
         
         Авторизация:
         
-        .. code:: python
+        ``` python
+        from yandex_music import Client
         
-            from yandex_music import Client
+        client = Client('token').init()
+        ```
         
-            client = Client('token').init()
-        
-        После успешного создания клиента Вы вольны в выборе необходимого метода
-        из API. Все они доступны у объекта класса ``Client``. Подробнее в методах клиента
-        в `документации <https://yandex-music.readthedocs.io/en/latest/yandex_music.client.html>`_.
+        После успешного создания клиента Вы вольны в выборе необходимого метода из API. Все они доступны у объекта класса `Client`. Подробнее в методах клиента в [документации](https://yandex-music.readthedocs.io/en/latest/yandex_music.client.html).
         
         Пример получения первого трека из плейлиста "Мне нравится" и его загрузка:
         
-        .. code:: python
-        
-            from yandex_music import Client
+        ``` python
+        from yandex_music import Client
         
-            client = Client('token').init()
-            client.users_likes_tracks()[0].fetch_track().download('example.mp3')
+        client = Client('token').init()
+        client.users_likes_tracks()[0].fetch_track().download('example.mp3')
+        ```
         
-        В примере выше клиент получает список треков которые были отмечены как
-        понравившиеся. API возвращает объект
-        `TracksList <https://yandex-music.readthedocs.io/en/latest/yandex_music.tracks_list.html>`_
-        в котором содержится список с треками класса
-        `TrackShort <https://yandex-music.readthedocs.io/en/latest/yandex_music.track_short.html>`_.
-        Данный класс содержит наиважнейшую информацию о треке и никаких подробностей,
-        поэтому для получения полной версии трека со всей информацией необходимо
-        обратиться к методу ``fetch_track()``. Затем можно скачать трек методом ``download()``.
+        В примере выше клиент получает список треков которые были отмечены как понравившиеся. API возвращает объект [TracksList](https://yandex-music.readthedocs.io/en/latest/yandex_music.tracks_list.html) в котором содержится список с треками класса [TrackShort](https://yandex-music.readthedocs.io/en/latest/yandex_music.track_short.html). Данный класс содержит наиважнейшую информацию о треке и никаких подробностей, поэтому для получения полной версии трека со всей информацией необходимо обратиться к методу `fetch_track()`. Затем можно скачать трек методом `download()`.
         
         Пример получения треков по ID:
         
-        .. code:: python
-        
-            from yandex_music import Client
+        ``` python
+        from yandex_music import Client
         
-            client = Client().init()
-            client.tracks(['10994777:1193829', '40133452:5206873', '48966383:6693286', '51385674:7163467'])
+        client = Client().init()
+        client.tracks(['10994777:1193829', '40133452:5206873', '48966383:6693286', '51385674:7163467'])
+        ```
         
-        В качестве ID трека выступает его уникальный номер и номер альбома.
-        Первым треком из примера является следующий трек:
-        music.yandex.ru/album/**1193829**/track/**10994777**
+        В качестве ID трека выступает его уникальный номер и номер альбома. Первым треком из примера является следующий трек:music.yandex.ru/album/**1193829**/track/**10994777**
         
         Выполнение запросов с использование прокси в синхронной версии:
         
-        .. code:: python
-        
-            from yandex_music.utils.request import Request
-            from yandex_music import Client
-        
-            request = Request(proxy_url='socks5://user:password@host:port')
-            client = Client(request=request).init()
+        ``` python
+        from yandex_music.utils.request import Request
+        from yandex_music import Client
+        
+        request = Request(proxy_url='socks5://user:password@host:port')
+        client = Client(request=request).init()
+        ```
         
         Примеры proxy url:
+          - socks5://user:<password@host>:port
+          - <http://host:port>
+          - <https://host:port>
+          - <http://user:password@host>
         
-        - socks5://user:password@host:port
-        - http://host:port
-        - https://host:port
-        - http://user:password@host
-        
-        Больше примеров тут: `proxies - advanced usage - requests <https://2.python-requests.org/en/master/user/advanced/#proxies>`_
+        Больше примеров тут: [proxies - advanced usage - requests](https://2.python-requests.org/en/master/user/advanced/#proxies)
         
         Выполнение запросов с использование прокси в асинхронной версии:
         
-        .. code:: python
-        
-            from yandex_music.utils.request_async import Request
-            from yandex_music import ClientAsync
-        
-            request = Request(proxy_url='http://user:pass@some.proxy.com')
-            client = await ClientAsync(request=request).init()
+        ``` python
+        from yandex_music.utils.request_async import Request
+        from yandex_music import ClientAsync
+        
+        request = Request(proxy_url='http://user:pass@some.proxy.com')
+        client = await ClientAsync(request=request).init()
+        ```
         
         Socks прокси не поддерживаются в асинхронной версии.
         
-        Про поддерживаемые прокси тут: `proxy support - advanced usage - aiohttp <https://docs.aiohttp.org/en/stable/client_advanced.html#proxy-support>`_
+        Про поддерживаемые прокси тут: [proxy support - advanced usage - aiohttp](https://docs.aiohttp.org/en/stable/client_advanced.html#proxy-support)
         
-        --------------------
-        Изучение по примерам
-        --------------------
+        #### Изучение по примерам
         
-        Вот несколько примеров для обзора. Даже если это не Ваш подход к
-        обучению, пожалуйста, возьмите и бегло просмотрите их.
+        Вот несколько примеров для обзора. Даже если это не Ваш подход к обучению, пожалуйста, возьмите и бегло просмотрите их.
         
-        Код примеров опубликован в открытом доступе, поэтому
-        Вы можете взять его и начать писать вокруг своё.
+        Код примеров опубликован в открытом доступе, поэтому Вы можете взять его и начать писать вокруг своё.
         
-        Посетите `эту страницу <https://github.com/MarshalX/yandex-music-api/blob/main/examples/>`_
-        чтобы изучить официальные примеры.
+        Посетите [эту страницу](https://github.com/MarshalX/yandex-music-api/blob/main/examples/), чтобы изучить официальные примеры.
         
-        ----------------------------------------------
-        Особенности использования асинхронного клиента
-        ----------------------------------------------
+        #### Особенности использования асинхронного клиента
         
         При работе с асинхронной версией библиотеке стоит всегда помнить
         следующие особенности:
-        
-        - Клиент следует импортировать с названием ``ClientAsync``, а не просто ``Client``.
-        - При использовании методов-сокращений нужно выбирать метод с суффиксом ``_async``.
+          - Клиент следует импортировать с названием `ClientAsync`, а не просто `Client`.
+          - При использовании методов-сокращений нужно выбирать метод с суффиксом `_async`.
         
         Пояснение ко второму пункту:
         
-        .. code:: python
-        
-            from yandex_music import ClientAsync
-        
-            client = await ClientAsync('token').init()
-            liked_short_track = (await client.users_likes_tracks())[0]
-        
-            # правильно
-            full_track = await liked_short_track.fetch_track_async()
-            await full_track.download_async()
+        ``` python
+        from yandex_music import ClientAsync
         
-            # НЕПРАВИЛЬНО
-            full_track = await liked_short_track.fetch_track()
-            await full_track.download()
+        client = await ClientAsync('token').init()
+        liked_short_track = (await client.users_likes_tracks())[0]
         
-        -----------
-        Логирование
-        -----------
-        
-        Данная библиотека использует ``logging`` модуль. Чтобы настроить логирование на
-        стандартный вывод, поместите
-        
-        .. code:: python
-        
-            import logging
-            logging.basicConfig(level=logging.DEBUG,
-                                format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+        # правильно
+        full_track = await liked_short_track.fetch_track_async()
+        await full_track.download_async()
+        
+        # НЕПРАВИЛЬНО
+        full_track = await liked_short_track.fetch_track()
+        await full_track.download()
+        ```
+        
+        #### Логирование
+        
+        Данная библиотека использует `logging` модуль. Чтобы настроить логирование на стандартный вывод, поместите
+        
+        ``` python
+        import logging
+        logging.basicConfig(
+            level=logging.DEBUG,
+            format='%(asctime)s - %(name)s - %(levelname)s - %(message)s'
+        )
+        ```
         
         в начало вашего скрипта.
         
-        Вы также можете использовать логирование в вашем приложении, вызвав
-        ``logging.getLogger()`` и установить уровень какой Вы хотите:
+        Вы также можете использовать логирование в вашем приложении, вызвав `logging.getLogger()` и установить уровень какой Вы хотите:
         
-        .. code:: python
+        ``` python
+        logger = logging.getLogger()
+        logger.setLevel(logging.INFO)
+        ```
         
-            logger = logging.getLogger()
-            logger.setLevel(logging.INFO)
+        Если Вы хотите `DEBUG` логирование:
         
-        Если Вы хотите ``DEBUG`` логирование:
+        ``` python
+        logger.setLevel(logging.DEBUG)
+        ```
         
-        .. code:: python
+        ### Документация
         
-            logger.setLevel(logging.DEBUG)
+        Документация `yandex-music-api` расположена на [readthedocs.io](https://yandex-music.readthedocs.io/). Вашей отправной точкой должен быть класс `Client`, а точнее его методы. Именно они выполняют все запросы на API и возвращают Вам готовые объекты. [Класс Client на readthedocs.io](https://yandex-music.readthedocs.io/en/latest/yandex_music.client.html).
         
-        ============
-        Документация
-        ============
+        ### Получение помощи
         
-        Документация ``yandex-music-api`` расположена на
-        `readthedocs.io <https://yandex-music.readthedocs.io/>`_.
-        Вашей отправной точкой должен быть класс ``Client``, а точнее его методы.
-        Именно они выполняют все
-        запросы на API и возвращают Вам готовые объекты.
-        `Класс Client на readthedocs.io <https://yandex-music.readthedocs.io/en/latest/yandex_music.client.html>`_.
+        Получить помощь можно несколькими путями:
+          - Задать вопрос в [Telegram чате](https://t.me/yandex_music_api), где мы помогаем друг другу, присоединяйтесь\!
+          - Сообщить о баге можно [создав Bug Report](https://github.com/MarshalX/yandex-music-api/issues/new?assignees=MarshalX&labels=bug&template=bug-report.md&title=).
+          - Предложить новую фичу или задать вопрос можно [создав discussion](https://github.com/MarshalX/yandex-music-api/discussions/new).
+          - Найти ответ на вопрос в [документации библиотеки](https://yandex-music.readthedocs.io/en/latest/).
         
-        ================
-        Получение помощи
-        ================
+        ### Список изменений
         
-        Получить помощь можно несколькими путями:
+        Весь список изменений ведётся в файле [CHANGES.md](https://github.com/MarshalX/yandex-music-api/blob/main/CHANGES.md).
+        
+        ### Реализации на других языках
         
-        - Задать вопрос в `Telegram чате <https://t.me/yandex_music_api>`_, где мы помогаем друг другу, присоединяйтесь!
-        - Сообщить о баге можно `создав Bug Report <https://github.com/MarshalX/yandex-music-api/issues/new?assignees=MarshalX&labels=bug&template=bug-report.md&title=>`_.
-        - Предложить новую фичу или задать вопрос можно `создав discussion <https://github.com/MarshalX/yandex-music-api/discussions/new>`_.
-        - Найти ответ на вопрос в `документации библиотеки <https://yandex-music.readthedocs.io/en/latest/>`_.
+        #### C#
         
-        ================
-        Список изменений
-        ================
+        Реализация с совершенно другим подходом, так как используется API для frontend'a, а не мобильных и десктопных приложений: [Winster332/Yandex.Music.Api](https://github.com/Winster332/Yandex.Music.Api).
         
-        Весь список изменений ведётся в файле `CHANGES.rst <https://github.com/MarshalX/yandex-music-api/blob/main/CHANGES.rst>`_.
+        [@Winster332](https://github.com/Winster332) не сильно проявляет активность, но существует форк, который продолжил начатое. Эндпоинты изменены с фронтовых на мобильные: [K1llMan/Yandex.Music.Api](https://github.com/K1llMan/Yandex.Music.Api).
         
+        #### PHP
         
-        ===========================
-        Реализации на других языках
-        ===========================
+        Частично переписанная текущая библиотека на PHP: [LuckyWins/yandex-music-api](https://github.com/LuckyWins/yandex-music-api).
         
-        --
-        C#
-        --
+        #### JavaScript
         
-        Реализация с совершенно другим подходом, так как используется API для frontend'a,
-        а не мобильных и десктопных приложений:
-        `Winster332/Yandex.Music.Api <https://github.com/Winster332/Yandex.Music.Api>`_.
+        API wrapper на Node.JS. Не обновлялся больше двух лет: [itsmepetrov/yandex-music-api](https://github.com/itsmepetrov/yandex-music-api). Продолжение разработки заброшенной библиотеки: [kontsevoye/ym-api](https://github.com/kontsevoye/ym-api).
         
-        `@Winster332 <https://github.com/Winster332>`_ не сильно проявляет активность,
-        но существует форк, который продолжил начатое. Эндпоинты изменены с фронтовых на
-        мобильные: `K1llMan/Yandex.Music.Api <https://github.com/K1llMan/Yandex.Music.Api>`_.
+        ### Разработанные проекты
         
-        ---
-        PHP
-        ---
+        #### Плагин для Kodi
         
-        Частично переписанная текущая библиотека на PHP:
-        `LuckyWins/yandex-music-api <https://github.com/LuckyWins/yandex-music-api>`_.
+        Плагин может проигрывать пользовательские плейлисты и плейлисты Яндекса, поиск по Яндекс Музыке, радио.
         
-        ----------
-        JavaScript
-        ----------
+        Сайт проекта: [ymkodi.ru](https://ymkodi.ru/). Исходный код: [kodi.plugin.yandex-music](https://github.com/Angel777d/kodi.plugin.yandex-music).
+        Автор: [@Angel777d](https://github.com/Angel777d).
         
-        API wrapper на Node.JS. Не обновлялся больше двух лет:
-        `itsmepetrov/yandex-music-api <https://github.com/itsmepetrov/yandex-music-api>`_.
-        Продолжение разработки заброшенной библиотеки: `kontsevoye/ym-api <https://github.com/kontsevoye/ym-api>`_.
+        [![Плагин для Kodi](https://raw.githubusercontent.com/Angel777d/kodi.plugin.yandex-music/master/assets/img/kody_yandex_music_plugin.png)](https://ymkodi.ru/)
         
-        =====================
-        Разработанные проекты
-        =====================
+        #### Telegram бот-клиент
         
-        ---------------
-        Плагин для Kodi
-        ---------------
+        Неофициальный бот. Умные и ваши плейлисты, понравившиеся треки. Лайки, дизлайки, текста песен, поиск, распознавание песен, похожие треки! Полноценный клиент на базе мессенджера.
         
-        Плагин может проигрывать пользовательские плейлисты и плейлисты Яндекса, поиск
-        по Яндекс Музыке, радио.
+        Сайт проекта: [music-yandex-bot.ru](https://music-yandex-bot.ru/). Бот в Telegram: [@music\_yandex\_bot](https://t.me/music_yandex_bot). Автор: [@MarshalX](https://github.com/MarshalX).
         
-        Сайт проекта: `ymkodi.ru <https://ymkodi.ru/>`_.
-        Исходный код: `kodi.plugin.yandex-music  <https://github.com/Angel777d/kodi.plugin.yandex-music>`_.
-        Автор: `@Angel777d <https://github.com/Angel777d>`_.
+        Статья на habr.com с описанием реализации: [Под капотом бота-клиента Яндекс.Музыки](https://habr.com/ru/post/487428/).
         
-        .. image:: https://raw.githubusercontent.com/Angel777d/kodi.plugin.yandex-music/master/assets/img/kody_yandex_music_plugin.png
-           :target: https://ymkodi.ru/
-           :alt: Плагин для Kodi
+        [![Telegram бот-клиент](https://hsto.org/webt/uv/4s/a3/uv4sa3pslohuzlmuzrjzteju2dk.png)](https://music-yandex-bot.ru/)
         
-        -------------------
-        Telegram бот-клиент
-        -------------------
+        ### Благодарность
         
-        Неофициальный бот. Умные и ваши плейлисты, понравившиеся треки. Лайки, дизлайки, текста песен,
-        поиск, распознавание песен, похожие треки! Полноценный клиент на базе мессенджера.
+        Спасибо разработчикам `python-telegram-bot`. Выбрал Вас в качестве примера.
         
-        Сайт проекта: `music-yandex-bot.ru <https://music-yandex-bot.ru/>`_.
-        Бот в Telegram: `@music_yandex_bot <https://t.me/music_yandex_bot>`_.
-        Автор: `@MarshalX <https://github.com/MarshalX>`_.
+        ### Внесение своего вклада в проект
         
-        Статья на habr.com с описанием реализации: `Под капотом бота-клиента Яндекс.Музыки <https://habr.com/ru/post/487428/>`_.
+        Внесение своего вклада максимально приветствуется! Есть перечень пунктов, который стоит соблюдать. Каждый пункт перечня расписан в [CONTRIBUTING.md](https://github.com/MarshalX/yandex-music-api/blob/main/CONTRIBUTING.md).
         
-        .. image:: https://hsto.org/webt/uv/4s/a3/uv4sa3pslohuzlmuzrjzteju2dk.png
-           :target: https://music-yandex-bot.ru/
-           :alt: Telegram бот-клиент
+        Вы можете помочь и сообщив о [баге](https://github.com/MarshalX/yandex-music-api/issues/new?assignees=MarshalX&labels=bug&template=bug-report.md&title=) или о [новом поле пришедшем от API](https://github.com/MarshalX/yandex-music-api/issues/new?assignees=&labels=feature&template=found-unknown-fields.md&title=%D0%9D%D0%BE%D0%B2%D0%BE%D0%B5+%D0%BD%D0%B5%D0%B8%D0%B7%D0%B2%D0%B5%D1%81%D1%82%D0%BD%D0%BE%D0%B5+%D0%BF%D0%BE%D0%BB%D0%B5+%D0%BE%D1%82+API).
         
-        =============
-        Благодарность
-        =============
+        ### Спонсоры
         
-        Спасибо разработчикам ``python-telegram-bot``. Выбрал Вас в качестве примера.
+        #### JetBrains
         
-        ===============================
-        Внесение своего вклада в проект
-        ===============================
+        <img height="150" width="150" src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.png" alt="JetBrains Logo (Main) logo.">
         
-        Внесение своего вклада максимально приветствуется! Есть перечень пунктов,
-        который стоит соблюдать. Каждый пункт перечня расписан в `CONTRIBUTING.md <https://github.com/MarshalX/yandex-music-api/blob/main/CONTRIBUTING.md>`_.
+        > JetBrains предоставляет бесплатный набор инструментов для разработки активным контрибьюторам некоммерческих проектов с открытым исходным кодом.
         
-        Вы можете помочь и сообщив о `баге <https://github.com/MarshalX/yandex-music-api/issues/new?assignees=MarshalX&labels=bug&template=bug-report.md&title=>`_
-        или о `новом поле пришедшем от API <https://github.com/MarshalX/yandex-music-api/issues/new?assignees=&labels=feature&template=found-unknown-fields.md&title=%D0%9D%D0%BE%D0%B2%D0%BE%D0%B5+%D0%BD%D0%B5%D0%B8%D0%B7%D0%B2%D0%B5%D1%81%D1%82%D0%BD%D0%BE%D0%B5+%D0%BF%D0%BE%D0%BB%D0%B5+%D0%BE%D1%82+API>`_.
+        [Лицензии для проектов с открытым исходным кодом — Программы поддержки](https://jb.gg/OpenSourceSupport)
         
-        ========
-        Лицензия
-        ========
+        ### Лицензия
         
-        Вы можете копировать, распространять и модифицировать программное обеспечение
-        при условии, что модификации описаны и лицензированы бесплатно в соответствии
-        с  `LGPL-3 <https://www.gnu.org/licenses/lgpl-3.0.html>`_. Произведения
-        производных (включая модификации или что-либо статически связанное с библиотекой)
-        могут распространяться только в соответствии с  LGPL-3, но приложения, которые
-        используют библиотеку, необязательно.
+        Вы можете копировать, распространять и модифицировать программное обеспечение при условии, что модификации описаны и лицензированы бесплатно в соответствии с [LGPL-3](https://www.gnu.org/licenses/lgpl-3.0.html). Произведения производных (включая модификации или что-либо статически связанное с библиотекой) могут распространяться только в соответствии с LGPL-3, но приложения, которые используют библиотеку, необязательно.
         
 Keywords: python yandex music api wrapper library client питон пайтон яндекс музыка апи обёртка библиотека клиент
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: Russian
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -454,11 +325,13 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
```

### Comparing `yandex-music-2.0.1/yandex_music.egg-info/SOURCES.txt` & `yandex-music-2.1.0/yandex_music.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-CHANGES.rst
+CHANGES.md
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 setup.py
 tests/__init__.py
 tests/conftest.py
 tests/test_account.py
 tests/test_ad_params.py
 tests/test_album.py
 tests/test_album_event.py
@@ -25,16 +25,18 @@
 tests/test_chart.py
 tests/test_chart_info.py
 tests/test_chart_info_menu.py
 tests/test_chart_info_menu_item.py
 tests/test_chart_item.py
 tests/test_contest.py
 tests/test_context.py
+tests/test_convert_track_id.py
 tests/test_counts.py
 tests/test_cover.py
+tests/test_custom_wave.py
 tests/test_dashboard.py
 tests/test_day.py
 tests/test_deactivation.py
 tests/test_deprecation.py
 tests/test_description.py
 tests/test_discrete_scale.py
 tests/test_download_info.py
@@ -50,14 +52,16 @@
 tests/test_label.py
 tests/test_landing.py
 tests/test_landing_list.py
 tests/test_licence_text_part.py
 tests/test_like.py
 tests/test_link.py
 tests/test_lyrics.py
+tests/test_lyrics_info.py
+tests/test_lyrics_major.py
 tests/test_made_for.py
 tests/test_major.py
 tests/test_meta_data.py
 tests/test_mix_link.py
 tests/test_non_auto_renewable.py
 tests/test_normalization.py
 tests/test_open_graph_data.py
@@ -78,39 +82,42 @@
 tests/test_poetry_lover_match.py
 tests/test_price.py
 tests/test_product.py
 tests/test_promo_code_status.py
 tests/test_promotion.py
 tests/test_queue.py
 tests/test_queue_item.py
+tests/test_r128.py
 tests/test_ratings.py
 tests/test_renewable_remainder.py
 tests/test_restrictions.py
 tests/test_rotor_settings.py
 tests/test_search.py
 tests/test_search_result.py
 tests/test_sequence.py
 tests/test_settings.py
 tests/test_shot.py
 tests/test_shot_data.py
 tests/test_shot_event.py
 tests/test_shot_type.py
+tests/test_sign_request.py
 tests/test_station.py
 tests/test_station_data.py
 tests/test_station_result.py
 tests/test_station_tracks_result.py
 tests/test_status.py
 tests/test_subscription.py
 tests/test_suggestions.py
 tests/test_supplement.py
 tests/test_tag.py
 tests/test_tag_result.py
 tests/test_title.py
 tests/test_track.py
 tests/test_track_id.py
+tests/test_track_lyrics.py
 tests/test_track_position.py
 tests/test_track_short.py
 tests/test_track_short_old.py
 tests/test_track_with_ads.py
 tests/test_tracks_list.py
 tests/test_tracks_similar.py
 tests/test_user.py
@@ -203,14 +210,15 @@
 yandex_music/landing/promotion.py
 yandex_music/landing/track_id.py
 yandex_music/landing/track_short_old.py
 yandex_music/playlist/__init__.py
 yandex_music/playlist/brand.py
 yandex_music/playlist/case_forms.py
 yandex_music/playlist/contest.py
+yandex_music/playlist/custom_wave.py
 yandex_music/playlist/made_for.py
 yandex_music/playlist/open_graph_data.py
 yandex_music/playlist/play_counter.py
 yandex_music/playlist/playlist.py
 yandex_music/playlist/playlist_absence.py
 yandex_music/playlist/playlist_id.py
 yandex_music/playlist/playlist_recommendation.py
@@ -247,18 +255,24 @@
 yandex_music/shot/shot_type.py
 yandex_music/supplement/__init__.py
 yandex_music/supplement/lyrics.py
 yandex_music/supplement/supplement.py
 yandex_music/supplement/video_supplement.py
 yandex_music/track/__init__.py
 yandex_music/track/licence_text_part.py
+yandex_music/track/lyrics_info.py
+yandex_music/track/lyrics_major.py
 yandex_music/track/major.py
 yandex_music/track/meta_data.py
 yandex_music/track/normalization.py
 yandex_music/track/poetry_lover_match.py
+yandex_music/track/r128.py
 yandex_music/track/track.py
+yandex_music/track/track_lyrics.py
 yandex_music/track/tracks_similar.py
 yandex_music/utils/__init__.py
+yandex_music/utils/convert_track_id.py
 yandex_music/utils/difference.py
 yandex_music/utils/request.py
 yandex_music/utils/request_async.py
-yandex_music/utils/response.py
+yandex_music/utils/response.py
+yandex_music/utils/sign_request.py
```

