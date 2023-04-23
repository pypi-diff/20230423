# Comparing `tmp/ooresults-0.2.2.tar.gz` & `tmp/ooresults-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooresults-0.2.2.tar", last modified: Fri Apr  7 09:55:30 2023, max compression
+gzip compressed data, was "ooresults-0.2.3.tar", last modified: Sun Apr 23 16:35:30 2023, max compression
```

## Comparing `ooresults-0.2.2.tar` & `ooresults-0.2.3.tar`

### file list

```diff
@@ -1,159 +1,162 @@
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.567350 ooresults-0.2.2/
--rw-r--r--   0 rainer    (1000) users      (100)    34523 2023-03-01 18:09:04.000000 ooresults-0.2.2/LICENSE
--rw-r--r--   0 rainer    (1000) users      (100)      260 2023-03-01 18:09:04.000000 ooresults-0.2.2/MANIFEST.in
--rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-04-07 09:55:30.567350 ooresults-0.2.2/PKG-INFO
--rw-r--r--   0 rainer    (1000) users      (100)     2278 2023-03-01 18:09:04.000000 ooresults-0.2.2/README.rst
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.535350 ooresults-0.2.2/ooresults/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)    15992 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/_reader.py
--rw-r--r--   0 rainer    (1000) users      (100)    11645 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/_server.py
--rw-r--r--   0 rainer    (1000) users      (100)     4363 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/configuration.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.539350 ooresults-0.2.2/ooresults/handler/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/handler/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     7873 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/handler/classes.py
--rw-r--r--   0 rainer    (1000) users      (100)     2597 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/handler/clubs.py
--rw-r--r--   0 rainer    (1000) users      (100)     4559 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/handler/competitors.py
--rw-r--r--   0 rainer    (1000) users      (100)     5824 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/handler/courses.py
--rw-r--r--   0 rainer    (1000) users      (100)     1110 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/handler/demo_reader.py
--rw-r--r--   0 rainer    (1000) users      (100)    12420 2023-03-31 20:12:46.000000 ooresults-0.2.2/ooresults/handler/entries.py
--rw-r--r--   0 rainer    (1000) users      (100)     3351 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/handler/events.py
--rw-r--r--   0 rainer    (1000) users      (100)     4504 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/handler/handicap.py
--rw-r--r--   0 rainer    (1000) users      (100)    30157 2023-03-26 08:00:56.000000 ooresults-0.2.2/ooresults/handler/model.py
--rw-r--r--   0 rainer    (1000) users      (100)     8221 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/handler/results.py
--rw-r--r--   0 rainer    (1000) users      (100)     9873 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/handler/series.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.539350 ooresults-0.2.2/ooresults/pdf/
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.543350 ooresults-0.2.2/ooresults/pdf/fonts/
--rw-r--r--   0 rainer    (1000) users      (100)   690516 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/pdf/fonts/Carlito-Bold.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   816716 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/pdf/fonts/Carlito-BoldItalic.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   623416 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/pdf/fonts/Carlito-Italic.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   635996 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/pdf/fonts/Carlito-Regular.ttf
--rw-r--r--   0 rainer    (1000) users      (100)     2806 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/pdf/pdf.py
--rw-r--r--   0 rainer    (1000) users      (100)    11206 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/pdf/result.py
--rw-r--r--   0 rainer    (1000) users      (100)     5283 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/pdf/series.py
--rw-r--r--   0 rainer    (1000) users      (100)    10007 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/pdf/splittimes.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.547350 ooresults-0.2.2/ooresults/plugins/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/plugins/__init__.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.531350 ooresults-0.2.2/ooresults/plugins/imports/
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.547350 ooresults-0.2.2/ooresults/plugins/imports/entries/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/plugins/imports/entries/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     2948 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/plugins/imports/entries/text.py
--rw-r--r--   0 rainer    (1000) users      (100)     2813 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/plugins/iof_class_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     4068 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/plugins/iof_competitor_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     5935 2023-04-07 09:54:41.000000 ooresults-0.2.2/ooresults/plugins/iof_course_data.py
--rw-r--r--   0 rainer    (1000) users      (100)     5184 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/plugins/iof_entry_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    10074 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/plugins/iof_result_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     7446 2023-03-31 20:12:46.000000 ooresults-0.2.2/ooresults/plugins/oe12.py
--rw-r--r--   0 rainer    (1000) users      (100)    14580 2023-03-31 20:12:46.000000 ooresults-0.2.2/ooresults/plugins/oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/reader.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.547350 ooresults-0.2.2/ooresults/repo/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/repo/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     2237 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/repo/class_params.py
--rw-r--r--   0 rainer    (1000) users      (100)     7358 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/repo/repo.py
--rw-r--r--   0 rainer    (1000) users      (100)    16171 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/repo/result_type.py
--rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/repo/series_type.py
--rw-r--r--   0 rainer    (1000) users      (100)    36349 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/repo/sqlite_repo.py
--rw-r--r--   0 rainer    (1000) users      (100)     1265 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/repo/start_type.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.547350 ooresults-0.2.2/ooresults/repo/update/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/repo/update/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     4728 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/repo/update/update_008.py
--rw-r--r--   0 rainer    (1000) users      (100)     1890 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/repo/update/update_tables.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.547350 ooresults-0.2.2/ooresults/schema/
--rw-r--r--   0 rainer    (1000) users      (100)   177863 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/schema/IOF.xsd
--rwxr-xr-x   0 rainer    (1000) users      (100)     2117 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/schema/cardreader_log.json
--rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/server.py
--rw-r--r--   0 rainer    (1000) users      (100)     2257 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/set_legacy_mode.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.551350 ooresults-0.2.2/ooresults/static/
--rw-r--r--   0 rainer    (1000) users      (100)      643 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/static/style-tab.css
--rw-r--r--   0 rainer    (1000) users      (100)     1267 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/static/style.css
--rw-r--r--   0 rainer    (1000) users      (100)    12106 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/static/w3.js
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.555350 ooresults-0.2.2/ooresults/templates/
--rw-r--r--   0 rainer    (1000) users      (100)     5964 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/templates/add_class.html
--rw-r--r--   0 rainer    (1000) users      (100)      883 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/add_club.html
--rw-r--r--   0 rainer    (1000) users      (100)     3093 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/add_competitor.html
--rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/add_course.html
--rw-r--r--   0 rainer    (1000) users      (100)     6139 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/add_entry.html
--rw-r--r--   0 rainer    (1000) users      (100)     1811 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/add_entry_competitors.html
--rw-r--r--   0 rainer    (1000) users      (100)     7204 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/templates/add_entry_result.html
--rw-r--r--   0 rainer    (1000) users      (100)     2511 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/add_event.html
--rw-r--r--   0 rainer    (1000) users      (100)      466 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/base.html
--rw-r--r--   0 rainer    (1000) users      (100)    11941 2023-04-07 09:54:41.000000 ooresults-0.2.2/ooresults/templates/classes_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     2957 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/templates/classes_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     6858 2023-04-07 09:54:41.000000 ooresults-0.2.2/ooresults/templates/clubs_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)      453 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/clubs_table.html
--rwxr-xr-x   0 rainer    (1000) users      (100)    11673 2023-04-07 09:54:41.000000 ooresults-0.2.2/ooresults/templates/competitors_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1030 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/competitors_table.html
--rw-r--r--   0 rainer    (1000) users      (100)    11955 2023-04-07 09:54:41.000000 ooresults-0.2.2/ooresults/templates/courses_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1386 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/courses_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     6529 2023-03-26 08:00:56.000000 ooresults-0.2.2/ooresults/templates/demo_reader.html
--rwxr-xr-x   0 rainer    (1000) users      (100)    19221 2023-04-07 09:54:41.000000 ooresults-0.2.2/ooresults/templates/entries_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     3006 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/templates/entries_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     9445 2023-04-07 09:54:41.000000 ooresults-0.2.2/ooresults/templates/events_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/events_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     5937 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/main.html
--rw-r--r--   0 rainer    (1000) users      (100)     5924 2023-04-07 09:54:41.000000 ooresults-0.2.2/ooresults/templates/results_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     5390 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/templates/results_table.html
--rw-r--r--   0 rainer    (1000) users      (100)      528 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/root.html
--rw-r--r--   0 rainer    (1000) users      (100)     1084 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/select_event.html
--rw-r--r--   0 rainer    (1000) users      (100)     2500 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/series_settings.html
--rw-r--r--   0 rainer    (1000) users      (100)     8367 2023-04-07 09:54:41.000000 ooresults-0.2.2/ooresults/templates/series_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1541 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/series_table.html
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.555350 ooresults-0.2.2/ooresults/templates/si/
--rw-r--r--   0 rainer    (1000) users      (100)      902 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/templates/si/si1_data.html
--rw-r--r--   0 rainer    (1000) users      (100)      396 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/si/si1_error.html
--rw-r--r--   0 rainer    (1000) users      (100)     6992 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/si/si1_page.html
--rw-r--r--   0 rainer    (1000) users      (100)     4161 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/templates/si/si2_data.html
--rw-r--r--   0 rainer    (1000) users      (100)     3589 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/si/si2_page.html
--rw-r--r--   0 rainer    (1000) users      (100)      383 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/templates/unauthorized.html
--rw-r--r--   0 rainer    (1000) users      (100)     2407 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/user.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.555350 ooresults-0.2.2/ooresults/utils/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/utils/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     1666 2023-04-03 19:51:02.000000 ooresults-0.2.2/ooresults/utils/globals.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.559350 ooresults-0.2.2/ooresults/websocket_server/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/websocket_server/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     1749 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/websocket_server/si.py
--rw-r--r--   0 rainer    (1000) users      (100)    14523 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/websocket_server/websocket_handler.py
--rw-r--r--   0 rainer    (1000) users      (100)     2143 2023-03-01 18:09:04.000000 ooresults-0.2.2/ooresults/websocket_server/websocket_server.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.535350 ooresults-0.2.2/ooresults.egg-info/
--rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-04-07 09:55:30.000000 ooresults-0.2.2/ooresults.egg-info/PKG-INFO
--rw-r--r--   0 rainer    (1000) users      (100)     4448 2023-04-07 09:55:30.000000 ooresults-0.2.2/ooresults.egg-info/SOURCES.txt
--rw-r--r--   0 rainer    (1000) users      (100)        1 2023-04-07 09:55:30.000000 ooresults-0.2.2/ooresults.egg-info/dependency_links.txt
--rw-r--r--   0 rainer    (1000) users      (100)      102 2023-04-07 09:55:30.000000 ooresults-0.2.2/ooresults.egg-info/entry_points.txt
--rw-r--r--   0 rainer    (1000) users      (100)      152 2023-04-07 09:55:30.000000 ooresults-0.2.2/ooresults.egg-info/requires.txt
--rw-r--r--   0 rainer    (1000) users      (100)       10 2023-04-07 09:55:30.000000 ooresults-0.2.2/ooresults.egg-info/top_level.txt
--rwxr-xr-x   0 rainer    (1000) users      (100)      977 2023-04-07 09:54:41.000000 ooresults-0.2.2/pyproject.toml
--rwxr-xr-x   0 rainer    (1000) users      (100)      616 2023-04-07 09:55:30.567350 ooresults-0.2.2/setup.cfg
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.559350 ooresults-0.2.2/tests/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     1414 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/competitor.py
--rw-r--r--   0 rainer    (1000) users      (100)     2061 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/entry.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.559350 ooresults-0.2.2/tests/model/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/model/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)    10750 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/model/test_courses.py
--rw-r--r--   0 rainer    (1000) users      (100)    16528 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/model/test_parse_cardreader_log.py
--rw-r--r--   0 rainer    (1000) users      (100)    27576 2023-03-26 08:00:56.000000 ooresults-0.2.2/tests/model/test_store_cardreader_result.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.563350 ooresults-0.2.2/tests/plugins/
--rw-r--r--   0 rainer    (1000) users      (100)    13070 2023-03-31 20:12:46.000000 ooresults-0.2.2/tests/plugins/test_export_competitors_oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)    29297 2023-03-31 20:12:46.000000 ooresults-0.2.2/tests/plugins/test_import_competitors_oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)     2766 2023-04-03 19:51:02.000000 ooresults-0.2.2/tests/plugins/test_plugin_iof_class_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     4000 2023-04-03 19:51:02.000000 ooresults-0.2.2/tests/plugins/test_plugin_iof_competitor_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    10229 2023-04-03 19:51:02.000000 ooresults-0.2.2/tests/plugins/test_plugin_iof_course_data.py
--rw-r--r--   0 rainer    (1000) users      (100)     8789 2023-04-03 19:51:02.000000 ooresults-0.2.2/tests/plugins/test_plugin_iof_entry_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    28112 2023-04-03 19:51:02.000000 ooresults-0.2.2/tests/plugins/test_plugin_iof_result_list.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-07 09:55:30.567350 ooresults-0.2.2/tests/repo/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/repo/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     9402 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/repo/test_classes.py
--rw-r--r--   0 rainer    (1000) users      (100)     5314 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/repo/test_clubs.py
--rw-r--r--   0 rainer    (1000) users      (100)    10687 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/repo/test_competitors.py
--rw-r--r--   0 rainer    (1000) users      (100)     7336 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/repo/test_courses.py
--rw-r--r--   0 rainer    (1000) users      (100)    39414 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/repo/test_entries.py
--rw-r--r--   0 rainer    (1000) users      (100)     7540 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/repo/test_events.py
--rw-r--r--   0 rainer    (1000) users      (100)     2353 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/repo/test_settings.py
--rw-r--r--   0 rainer    (1000) users      (100)     9467 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/test_compute_result_net.py
--rw-r--r--   0 rainer    (1000) users      (100)    15440 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/test_compute_result_score.py
--rw-r--r--   0 rainer    (1000) users      (100)    38250 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/test_compute_result_standard.py
--rw-r--r--   0 rainer    (1000) users      (100)     7257 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/test_configuration.py
--rw-r--r--   0 rainer    (1000) users      (100)     1973 2023-04-03 19:51:02.000000 ooresults-0.2.2/tests/test_globals.py
--rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/test_handicap.py
--rw-r--r--   0 rainer    (1000) users      (100)    19384 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/test_ranking.py
--rw-r--r--   0 rainer    (1000) users      (100)    26017 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/test_series.py
--rw-r--r--   0 rainer    (1000) users      (100)     2326 2023-03-01 18:09:04.000000 ooresults-0.2.2/tests/test_user.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.453791 ooresults-0.2.3/
+-rw-r--r--   0 rainer    (1000) users      (100)    34523 2023-03-01 18:09:04.000000 ooresults-0.2.3/LICENSE
+-rw-r--r--   0 rainer    (1000) users      (100)      260 2023-03-01 18:09:04.000000 ooresults-0.2.3/MANIFEST.in
+-rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-04-23 16:35:30.453791 ooresults-0.2.3/PKG-INFO
+-rw-r--r--   0 rainer    (1000) users      (100)     2278 2023-03-01 18:09:04.000000 ooresults-0.2.3/README.rst
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.429791 ooresults-0.2.3/ooresults/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)    15992 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/_reader.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11381 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/_server.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4363 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/configuration.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.433791 ooresults-0.2.3/ooresults/handler/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/handler/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     9134 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/build_results.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7873 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/classes.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2597 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/clubs.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4559 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/handler/competitors.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5824 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1110 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/demo_reader.py
+-rw-r--r--   0 rainer    (1000) users      (100)    12416 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/entries.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3351 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/events.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4504 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/handler/handicap.py
+-rw-r--r--   0 rainer    (1000) users      (100)    31886 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/model.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3536 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/results.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4892 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/series.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.433791 ooresults-0.2.3/ooresults/pdf/
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.437791 ooresults-0.2.3/ooresults/pdf/fonts/
+-rw-r--r--   0 rainer    (1000) users      (100)   690516 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/pdf/fonts/Carlito-Bold.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   816716 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/pdf/fonts/Carlito-BoldItalic.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   623416 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/pdf/fonts/Carlito-Italic.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   635996 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/pdf/fonts/Carlito-Regular.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)     2806 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/pdf/pdf.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11206 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/pdf/result.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5283 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/pdf/series.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10007 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/pdf/splittimes.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.437791 ooresults-0.2.3/ooresults/plugins/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/plugins/__init__.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.429791 ooresults-0.2.3/ooresults/plugins/imports/
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.441791 ooresults-0.2.3/ooresults/plugins/imports/entries/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/plugins/imports/entries/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2948 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/plugins/imports/entries/text.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2813 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/plugins/iof_class_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4068 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/plugins/iof_competitor_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5935 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/plugins/iof_course_data.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5184 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/plugins/iof_entry_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10702 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/plugins/iof_result_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7446 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/plugins/oe12.py
+-rw-r--r--   0 rainer    (1000) users      (100)    14580 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/plugins/oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/reader.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.441791 ooresults-0.2.3/ooresults/repo/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2237 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/class_params.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7358 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/repo.py
+-rw-r--r--   0 rainer    (1000) users      (100)    16171 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/result_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/series_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)    36849 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/repo/sqlite_repo.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1265 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/start_type.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.441791 ooresults-0.2.3/ooresults/repo/update/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/update/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4728 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/update/update_008.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1890 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/update/update_tables.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.441791 ooresults-0.2.3/ooresults/schema/
+-rw-r--r--   0 rainer    (1000) users      (100)   177863 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/schema/IOF.xsd
+-rwxr-xr-x   0 rainer    (1000) users      (100)     2117 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/schema/cardreader_log.json
+-rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/server.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2257 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/set_legacy_mode.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.441791 ooresults-0.2.3/ooresults/static/
+-rw-r--r--   0 rainer    (1000) users      (100)      643 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/static/style-tab.css
+-rw-r--r--   0 rainer    (1000) users      (100)     1267 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/static/style.css
+-rw-r--r--   0 rainer    (1000) users      (100)    12106 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/static/w3.js
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.445791 ooresults-0.2.3/ooresults/templates/
+-rw-r--r--   0 rainer    (1000) users      (100)     5964 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/add_class.html
+-rw-r--r--   0 rainer    (1000) users      (100)      883 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/add_club.html
+-rw-r--r--   0 rainer    (1000) users      (100)     3093 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/add_competitor.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/add_course.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6139 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/add_entry.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1811 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/add_entry_competitors.html
+-rw-r--r--   0 rainer    (1000) users      (100)     7204 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/add_entry_result.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2511 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/add_event.html
+-rw-r--r--   0 rainer    (1000) users      (100)      466 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/base.html
+-rw-r--r--   0 rainer    (1000) users      (100)    11941 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/classes_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2957 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/classes_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6858 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/clubs_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)      453 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/clubs_table.html
+-rwxr-xr-x   0 rainer    (1000) users      (100)    11673 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/competitors_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1030 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/competitors_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)    11955 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/courses_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1386 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/courses_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6529 2023-04-23 07:11:17.000000 ooresults-0.2.3/ooresults/templates/demo_reader.html
+-rwxr-xr-x   0 rainer    (1000) users      (100)    19221 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/entries_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     3006 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/entries_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     9445 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/events_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/events_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5937 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/main.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5924 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/results_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5390 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/results_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)      528 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/root.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1084 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/select_event.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2500 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/series_settings.html
+-rw-r--r--   0 rainer    (1000) users      (100)     8367 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/series_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1541 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/series_table.html
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.445791 ooresults-0.2.3/ooresults/templates/si/
+-rw-r--r--   0 rainer    (1000) users      (100)      902 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/si/si1_data.html
+-rw-r--r--   0 rainer    (1000) users      (100)      396 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/si/si1_error.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6992 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/si/si1_page.html
+-rw-r--r--   0 rainer    (1000) users      (100)     4161 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/si/si2_data.html
+-rw-r--r--   0 rainer    (1000) users      (100)     3589 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/si/si2_page.html
+-rw-r--r--   0 rainer    (1000) users      (100)      383 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/unauthorized.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2407 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/user.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.445791 ooresults-0.2.3/ooresults/utils/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/utils/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1666 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/utils/globals.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.449791 ooresults-0.2.3/ooresults/websocket_server/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/websocket_server/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1749 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/websocket_server/si.py
+-rw-r--r--   0 rainer    (1000) users      (100)    14523 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/websocket_server/websocket_handler.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2143 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/websocket_server/websocket_server.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.433791 ooresults-0.2.3/ooresults.egg-info/
+-rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-04-23 16:35:30.000000 ooresults-0.2.3/ooresults.egg-info/PKG-INFO
+-rw-r--r--   0 rainer    (1000) users      (100)     4563 2023-04-23 16:35:30.000000 ooresults-0.2.3/ooresults.egg-info/SOURCES.txt
+-rw-r--r--   0 rainer    (1000) users      (100)        1 2023-04-23 16:35:30.000000 ooresults-0.2.3/ooresults.egg-info/dependency_links.txt
+-rw-r--r--   0 rainer    (1000) users      (100)      102 2023-04-23 16:35:30.000000 ooresults-0.2.3/ooresults.egg-info/entry_points.txt
+-rw-r--r--   0 rainer    (1000) users      (100)      152 2023-04-23 16:35:30.000000 ooresults-0.2.3/ooresults.egg-info/requires.txt
+-rw-r--r--   0 rainer    (1000) users      (100)       10 2023-04-23 16:35:30.000000 ooresults-0.2.3/ooresults.egg-info/top_level.txt
+-rwxr-xr-x   0 rainer    (1000) users      (100)      977 2023-04-23 16:33:35.000000 ooresults-0.2.3/pyproject.toml
+-rwxr-xr-x   0 rainer    (1000) users      (100)      616 2023-04-23 16:35:30.453791 ooresults-0.2.3/setup.cfg
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.449791 ooresults-0.2.3/tests/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1414 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/competitor.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2061 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/entry.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.449791 ooresults-0.2.3/tests/model/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/model/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     8015 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/model/test_build_series_result.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11820 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/model/test_courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)     6578 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/model/test_event_class_results.py
+-rw-r--r--   0 rainer    (1000) users      (100)    16528 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/model/test_parse_cardreader_log.py
+-rw-r--r--   0 rainer    (1000) users      (100)    27576 2023-04-23 07:11:17.000000 ooresults-0.2.3/tests/model/test_store_cardreader_result.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.449791 ooresults-0.2.3/tests/plugins/
+-rw-r--r--   0 rainer    (1000) users      (100)    13070 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/plugins/test_export_competitors_oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)    29297 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/plugins/test_import_competitors_oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2766 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/plugins/test_plugin_iof_class_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4000 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/plugins/test_plugin_iof_competitor_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10229 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/plugins/test_plugin_iof_course_data.py
+-rw-r--r--   0 rainer    (1000) users      (100)     8789 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/plugins/test_plugin_iof_entry_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    30446 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/plugins/test_plugin_iof_result_list.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.453791 ooresults-0.2.3/tests/repo/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/repo/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11959 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/repo/test_classes.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5314 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/repo/test_clubs.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10687 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/repo/test_competitors.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7336 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/repo/test_courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)    39686 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/repo/test_entries.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7540 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/repo/test_events.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2353 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/repo/test_settings.py
+-rw-r--r--   0 rainer    (1000) users      (100)     9467 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/test_compute_result_net.py
+-rw-r--r--   0 rainer    (1000) users      (100)    15440 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/test_compute_result_score.py
+-rw-r--r--   0 rainer    (1000) users      (100)    38250 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/test_compute_result_standard.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7257 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/test_configuration.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1973 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/test_globals.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/test_handicap.py
+-rw-r--r--   0 rainer    (1000) users      (100)    23885 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/test_ranking.py
+-rw-r--r--   0 rainer    (1000) users      (100)    26132 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/test_series.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2326 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/test_user.py
```

### Comparing `ooresults-0.2.2/LICENSE` & `ooresults-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/PKG-INFO` & `ooresults-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooresults
-Version: 0.2.2
+Version: 0.2.3
 Summary: A software for the evaluation of the results of orienteering events
 Author: Rainer Garus
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ooresults-0.2.2/README.rst` & `ooresults-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/__init__.py` & `ooresults-0.2.3/ooresults/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/_reader.py` & `ooresults-0.2.3/ooresults/_reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/_server.py` & `ooresults-0.2.3/ooresults/_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 import logging
 import argparse
-import copy
 import re
 import base64
 import pathlib
 import sys
 import sqlite3
 from typing import Optional
 
@@ -60,19 +59,15 @@
 
 
 class Root:
     def GET(self):
         events = list(model.get_events())
         for event in events:
             if event.publish:
-                classes = list(model.get_classes(event_id=event.id))
-                entry_list = list(model.get_entries(event_id=event.id))
-                class_results = results.build_results(
-                    classes, copy.deepcopy(entry_list)
-                )
+                event, class_results = model.event_class_results(event_id=event.id)
                 columns = results.build_columns(class_results)
                 results_table = render.results_table(event, class_results, columns)
                 return render.root(results_table)
         else:
             return render.root(None)
 
 
@@ -93,17 +88,15 @@
         events_tab_content = render.events_tab_content(events_table)
         entries_table = render.entries_table(event, [])
         entries_tab_content = render.entries_tab_content(entries_table)
         classes_table = render.classes_table(event, [])
         classes_tab_content = render.classes_tab_content(classes_table)
         courses_table = render.courses_table(event, [])
         courses_tab_content = render.courses_tab_content(courses_table)
-        results_table = render.results_table(
-            event, ooresults.handler.results.build_results([], []), set()
-        )
+        results_table = render.results_table(event, [], set())
         results_tab_content = render.results_tab_content(results_table)
         series_table = render.series_table(0, [])
         series_tab_content = render.series_tab_content(series_table)
         competitors_table = render.competitors_table([])
         competitors_tab_content = render.competitors_tab_content(competitors_table)
         clubs_table = render.clubs_table([])
         clubs_tab_content = render.clubs_tab_content(clubs_table)
```

### Comparing `ooresults-0.2.2/ooresults/configuration.py` & `ooresults-0.2.3/ooresults/configuration.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/handler/__init__.py` & `ooresults-0.2.3/ooresults/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/handler/classes.py` & `ooresults-0.2.3/ooresults/handler/classes.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/handler/clubs.py` & `ooresults-0.2.3/ooresults/handler/clubs.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/handler/competitors.py` & `ooresults-0.2.3/ooresults/handler/competitors.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/handler/courses.py` & `ooresults-0.2.3/ooresults/handler/courses.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/handler/demo_reader.py` & `ooresults-0.2.3/ooresults/handler/demo_reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/handler/entries.py` & `ooresults-0.2.3/ooresults/handler/entries.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                 entries = text.parse(content=data.browse4)
                 model.import_entries(event_id=event_id, entries=entries)
 
         except EventNotFoundError:
             raise web.conflict("No event selected or event deleted")
 
         except Exception as e:
-            raise web.Conflict(str(e))
+            raise web.conflict(str(e))
 
         return update(event_id)
 
 
 class Export:
     def POST(self):
         """Export entries"""
@@ -129,31 +129,30 @@
         event_id = int(data.event_id) if data.event_id != "" else -1
         try:
             if data.entr_export == "entr.export.1":
                 event = model.get_event(id=event_id)
                 entry_list = model.get_entries(event_id=event_id)
                 content = iof_entry_list.create_entry_list(event[0], entry_list)
             elif data.entr_export == "entr.export.2":
-                event = model.get_event(id=event_id)
-                entry_list = model.get_entries(event_id=event_id)
-                content = iof_result_list.create_result_list(event[0], entry_list)
+                event, class_results = model.event_class_results(event_id=event_id)
+                content = iof_result_list.create_result_list(event, class_results)
             elif data.entr_export == "entr.export.3":
                 class_list = model.get_classes(event_id=event_id)
                 entry_list = model.get_entries(event_id=event_id)
                 content = oe2003.create(entry_list, list(class_list))
             elif data.entr_export == "entr.export.4":
                 class_list = model.get_classes(event_id=event_id)
                 entry_list = model.get_entries(event_id=event_id)
                 content = oe12.create(entry_list, list(class_list))
 
         except KeyError:
             raise web.conflict("Entry deleted")
-        except:
-            logging.exception("Internal server error")
-            raise
+        except Exception as e:
+            logging.exception(e)
+            raise web.conflict("Internal server error")
 
         return content
 
 
 class Add:
     def parse_start_time(
         self, item: str, event_date: datetime.date
```

### Comparing `ooresults-0.2.2/ooresults/handler/events.py` & `ooresults-0.2.3/ooresults/handler/events.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/handler/handicap.py` & `ooresults-0.2.3/ooresults/handler/handicap.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/handler/model.py` & `ooresults-0.2.3/ooresults/handler/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,25 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 import asyncio
 import datetime
 import pathlib
+import copy
 import json
 from typing import Optional
 from typing import List
 from typing import Dict
 from typing import Tuple
 
 import iso8601
 import jsonschema
 
+from ooresults.handler import build_results
 from ooresults.repo.sqlite_repo import SqliteRepo
 from ooresults.repo.repo import EventNotFoundError
 from ooresults.repo.repo import TransactionMode
 from ooresults.repo.class_params import ClassParams
 from ooresults.repo import result_type
 from ooresults.repo import start_type
 from ooresults.repo.result_type import ResultStatus
@@ -906,7 +908,62 @@
     with db.transaction():
         return db.get_series_settings()
 
 
 def update_series_settings(settings: Settings) -> None:
     with db.transaction(mode=TransactionMode.IMMEDIATE):
         db.update_series_settings(settings=settings)
+
+
+def event_class_results(event_id: int) -> Tuple[Dict, List[Tuple[Dict, List[Dict]]]]:
+    with db.transaction():
+        event = list(db.get_event(id=event_id))
+        event = event[0] if event != [] else {}
+
+        classes = list(db.get_classes(event_id=event_id))
+        entry_list = list(db.get_entries(event_id=event_id))
+
+    class_results = build_results.build_results(
+        classes=classes,
+        results=copy.deepcopy(entry_list),
+    )
+    return event, class_results
+
+
+def create_event_list(events):
+    # filter list
+    e_list = [e for e in events if e.series is not None]
+    # sort list
+    e_list.sort(key=lambda e: e.series)
+    e_list.sort(key=lambda e: e.date)
+    return e_list
+
+
+def build_series_result():
+    with db.transaction():
+        settings = db.get_series_settings()
+        # build event list
+        events = list(db.get_events())
+        events = create_event_list(events=events)
+
+        list_of_results = []
+        organizers = []
+        for i, event in enumerate(events):
+            classes = list(db.get_classes(event_id=event.id))
+            entry_list = list(db.get_entries(event_id=event.id))
+            class_results = build_results.build_results(
+                classes=classes,
+                results=copy.deepcopy(entry_list),
+            )
+            list_of_results.append(class_results)
+            organizers.append([e for e in entry_list if e.class_ == "Organizer"])
+
+    ranked_classes = build_results.build_total_results(
+        settings=settings,
+        list_of_results=list_of_results,
+        organizers=organizers,
+    )
+    return (
+        settings,
+        events,
+        ranked_classes,
+    )
```

### Comparing `ooresults-0.2.2/ooresults/handler/results.py` & `ooresults-0.2.3/ooresults/handler/build_results.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,35 +13,26 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-import logging
-import copy
-import pathlib
+from decimal import Decimal
 from typing import List
 from typing import Dict
 from typing import Tuple
 
-import web
-
-from ooresults.handler import model
+from ooresults.repo import series_type
 from ooresults.repo.result_type import ResultStatus
-import ooresults.pdf.result
-import ooresults.pdf.splittimes
-from ooresults.utils.globals import t_globals
-
 
-templates = pathlib.Path(__file__).resolve().parent.parent / "templates"
-render = web.template.render(templates, globals=t_globals)
 
-
-def build_results(classes: List[Dict], results: List[Dict]):
+def build_results(
+    classes: List[Dict], results: List[Dict]
+) -> List[Tuple[Dict, List[Dict]]]:
     all_results = []
     for class_ in classes:
         if class_.name == "Organizer":
             continue
         # filter results belonging to this class
         class_results = []
         for r in results:
@@ -105,14 +96,18 @@
                 if r["result"].status == ResultStatus.OK and not r["not_competing"]:
                     if i > 0 and result_equal(
                         class_results[i]["result"], class_results[i - 1]["result"]
                     ):
                         r["rank"] = class_results[i - 1]["rank"]
                     else:
                         r["rank"] = i + 1
+
+                    if class_.params.otype != "score":
+                        winner_time = class_results[0]["result"].time
+                        r["time_behind"] = r["result"].time - winner_time
                 else:
                     r["rank"] = None
 
             # add points
             if class_.params.otype != "score":
                 ref_time = class_results[0]["result"].time
                 for r in class_results:
@@ -128,96 +123,97 @@
                     ):
                         r["points"] = 0
 
             all_results.append((class_, class_results))
     return all_results
 
 
-def build_columns(class_results: List[Tuple[Dict, Dict]]) -> set:
-    columns = set()
-    for class_, _ in class_results:
-        if class_.params.apply_handicap_rule:
-            columns.add("factor")
-        if class_.params.penalty_controls is not None:
-            columns.add("penalties_controls")
-        if class_.params.penalty_overtime is not None:
-            columns.add("penalties_overtime")
-        if class_.params.otype == "score":
-            columns.add("score")
-    return columns
-
-
-class Update:
-    def POST(self):
-        """Update data"""
-        data = web.input()
-        event_id = int(data.event_id) if data.event_id != "" else -1
-        event = list(model.get_event(id=event_id))
-        event = event[0] if event != [] else {}
-
-        classes = list(model.get_classes(event_id=event_id))
-        entry_list = list(model.get_entries(event_id=event_id))
-        class_results = build_results(
-            classes=classes, results=copy.deepcopy(entry_list)
-        )
-        columns = build_columns(class_results)
-        return render.results_table(event, class_results, columns)
-
-
-class PdfResult:
-    def POST(self):
-        """Print results"""
-        data = web.input()
-        event_id = int(data.event_id) if data.event_id != "" else -1
-        include_dns = "res_include_dns" in data
-
-        try:
-            event = list(model.get_event(id=event_id))
-            event = event[0] if event != [] else {}
-            classes = list(model.get_classes(event_id=event_id))
-
-            entry_list = list(model.get_entries(event_id=event_id))
-            class_results = build_results(classes, copy.deepcopy(entry_list))
-            columns = build_columns(class_results)
-            content = ooresults.pdf.result.create_pdf(
-                event=event,
-                results=class_results,
-                include_dns=include_dns,
-                landscape=len(columns) > 0,
-            )
-            return content
-
-        except KeyError:
-            raise web.conflict("Entry deleted")
-        except:
-            logging.exception("Internal server error")
-            raise
-
-        return content
-
-
-class PdfSplittimes:
-    def POST(self):
-        """Print results"""
-        data = web.input()
-        event_id = int(data.event_id) if data.event_id != "" else -1
-        landscape = "res_landscape" in data
-
-        try:
-            event = list(model.get_event(id=event_id))
-            event = event[0] if event != [] else {}
-            classes = list(model.get_classes(event_id=event_id))
-
-            entry_list = list(model.get_entries(event_id=event_id))
-            class_results = build_results(classes, copy.deepcopy(entry_list))
-            content = ooresults.pdf.splittimes.create_pdf(
-                event=event, results=class_results, landscape=landscape
+def build_total_results(
+    settings: series_type.Settings, list_of_results: List, organizers: List = []
+) -> List[Tuple[str, List[Dict]]]:
+    q = Decimal(10) ** -settings.decimal_places
+
+    r = {}
+    for i, class_results in enumerate(list_of_results):
+        for class_, results in class_results:
+            if class_.name == "Organizer":
+                continue
+            if class_.name not in r:
+                r[class_.name] = {}
+            for entry in results:
+                # check if competitor has points
+                if entry.get("points", None) is not None:
+                    if (entry["last_name"], entry["first_name"]) not in r[class_.name]:
+                        r[class_.name][(entry["last_name"], entry["first_name"])] = {
+                            "last_name": entry["last_name"],
+                            "first_name": entry["first_name"],
+                            "year": entry.get("year", None),
+                            "club": entry.get("club", None),
+                            "sum": 0,
+                            "races": {},
+                            "organizer": {},
+                        }
+
+                    p = Decimal(settings.maximum_points * entry["points"]).quantize(q)
+                    r[class_.name][(entry["last_name"], entry["first_name"])]["races"][
+                        i
+                    ] = p
+            # add organizers
+            if len(organizers) > i:
+                for entry in organizers[i]:
+                    if (entry["last_name"], entry["first_name"]) not in r[class_.name]:
+                        r[class_.name][(entry["last_name"], entry["first_name"])] = {
+                            "last_name": entry["last_name"],
+                            "first_name": entry["first_name"],
+                            "year": entry.get("year", None),
+                            "club": entry.get("club", None),
+                            "sum": 0,
+                            "races": {},
+                            "organizer": {},
+                        }
+                    r[class_.name][(entry["last_name"], entry["first_name"])][
+                        "organizer"
+                    ][i] = 0
+
+    # build sum of points
+    ranked_classes = []
+    for class_name, entries in r.items():
+        for entry in entries.values():
+            points_of_series = sorted(entry["races"].values(), reverse=True)
+            # add organizer bonus
+            if entry["organizer"] != {}:
+                if len(points_of_series) == 0:
+                    points = Decimal(0)
+                elif len(points_of_series) == 1:
+                    points = points_of_series[0] / 2
+                else:
+                    points = (points_of_series[0] + points_of_series[1]) / 2
+                for i in entry["organizer"].keys():
+                    entry["organizer"][i] = points.quantize(q)
+
+            # compute sum
+            points_of_series = sorted(
+                list(entry["races"].values()) + list(entry["organizer"].values()),
+                reverse=True,
             )
-            return content
+            if settings.nr_of_best_results is not None:
+                points_of_series = points_of_series[0 : settings.nr_of_best_results]
+            for points in points_of_series:
+                entry["sum"] += points
+
+        # build a list and rank the list
+        ranked_entries = list(entries.values())
+        ranked_entries.sort(key=lambda e: e["last_name"] + "," + e["first_name"])
+        ranked_entries.sort(key=lambda e: e["sum"], reverse=True)
+
+        for j, e in enumerate(ranked_entries):
+            if j > 0 and ranked_entries[j]["sum"] == ranked_entries[j - 1]["sum"]:
+                e["rank"] = ranked_entries[j - 1]["rank"]
+            else:
+                e["rank"] = j + 1
+            # rank is None if sum is 0
+            if e["sum"] == 0:
+                e["rank"] = None
 
-        except KeyError:
-            raise web.conflict("Entry deleted")
-        except:
-            logging.exception("Internal server error")
-            raise
+        ranked_classes.append((class_name, ranked_entries))
 
-        return content
+    return ranked_classes
```

### Comparing `ooresults-0.2.2/ooresults/pdf/fonts/Carlito-Bold.ttf` & `ooresults-0.2.3/ooresults/pdf/fonts/Carlito-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/pdf/fonts/Carlito-BoldItalic.ttf` & `ooresults-0.2.3/ooresults/pdf/fonts/Carlito-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/pdf/fonts/Carlito-Italic.ttf` & `ooresults-0.2.3/ooresults/pdf/fonts/Carlito-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/pdf/fonts/Carlito-Regular.ttf` & `ooresults-0.2.3/ooresults/pdf/fonts/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/pdf/pdf.py` & `ooresults-0.2.3/ooresults/pdf/pdf.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/pdf/result.py` & `ooresults-0.2.3/ooresults/pdf/result.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/pdf/series.py` & `ooresults-0.2.3/ooresults/pdf/series.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/pdf/splittimes.py` & `ooresults-0.2.3/ooresults/pdf/splittimes.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/plugins/__init__.py` & `ooresults-0.2.3/ooresults/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/plugins/imports/entries/__init__.py` & `ooresults-0.2.3/ooresults/plugins/imports/entries/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/plugins/imports/entries/text.py` & `ooresults-0.2.3/ooresults/plugins/imports/entries/text.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/plugins/iof_class_list.py` & `ooresults-0.2.3/ooresults/plugins/iof_class_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/plugins/iof_competitor_list.py` & `ooresults-0.2.3/ooresults/plugins/iof_competitor_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/plugins/iof_course_data.py` & `ooresults-0.2.3/ooresults/plugins/iof_course_data.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/plugins/iof_entry_list.py` & `ooresults-0.2.3/ooresults/plugins/iof_entry_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/plugins/iof_result_list.py` & `ooresults-0.2.3/ooresults/plugins/iof_result_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,62 +34,76 @@
 xml_schema = etree.XMLSchema(etree.parse(str(schema_file)))
 
 
 iof_namespace = "http://www.orienteering.org/datastandard/3.0"
 namespaces = {None: iof_namespace}
 
 
-def create_result_list(event: Dict, results: List[Dict]) -> bytes:
+def create_result_list(
+    event: Dict, class_results: List[Tuple[Dict, List[Dict]]]
+) -> bytes:
     E = ElementMaker(namespace=iof_namespace, nsmap=namespaces)
 
     RESULTLIST = E.ResultList
     EVENT = E.Event
     NAME = E.Name
     STARTTIME = E.StartTime
     DATE = E.Date
     CLASSRESULT = E.ClassResult
     CLASS = E.Class
+    COURSE = E.Course
+    LENGTH = E.Length
+    CLIMB = E.Climb
+    NUMBEROFCONTROLS = E.NumberOfControls
     PERSONRESULT = E.PersonResult
     PERSON = E.Person
     FAMILY = E.Family
     GIVEN = E.Given
     BIRTHDATE = E.BirthDate
     ORGANISATION = E.Organisation
     RESULT = E.Result
     CONTROLCARD = E.ControlCard
     POSITION = E.Position
     STATUS = E.Status
     STARTTIME = E.StartTime
     FINISHTIME = E.FinishTime
     TIME = E.Time
+    TIMEBEHIND = E.TimeBehind
     SPLITTIME = E.SplitTime
     CONTROLCODE = E.ControlCode
 
     root = RESULTLIST(
         iofVersion="3.0",
         creator="ooresults (https://pypi.org/project/ooresults)",
     )
 
     e_event = EVENT()
     e_event.append(NAME(event.get("name", "")))
     if event.get("date", None) is not None:
         e_event.append(STARTTIME(DATE(event["date"].isoformat())))
     root.append(e_event)
 
-    classes: Dict[str, List[Dict]] = {}
-    for result in results:
-        if result["class_"] is not None:
-            if result["class_"] not in classes:
-                classes[result["class_"]] = []
-            classes[result["class_"]].append(result)
-
-    for c in classes:
+    for class_, ranked_results in class_results:
         cr = CLASSRESULT()
-        cr.append(CLASS(NAME(c)))
-        for r in classes[c]:
+        cr.append(CLASS(NAME(class_["name"])))
+
+        co = COURSE()
+        if class_["course_length"] is not None:
+            co.append(LENGTH(str(round(class_["course_length"]))))
+        if class_["course_climb"] is not None:
+            co.append(CLIMB(str(round(class_["course_climb"]))))
+        if (
+            class_["number_of_controls"] is not None
+            and class_["number_of_controls"] > 0
+        ):
+            co.append(NUMBEROFCONTROLS(str(class_["number_of_controls"])))
+        if len(co):
+            cr.append(co)
+
+        for r in ranked_results:
             pr = PERSONRESULT()
             person = PERSON(
                 NAME(
                     FAMILY(r["last_name"]),
                     GIVEN(r["first_name"]),
                 ),
             )
@@ -118,15 +132,18 @@
             if r["result"].time is not None:
                 result.append(TIME(str(r["result"].time)))
 
             if r["result"].status == ResultStatus.OK:
                 if r["not_competing"]:
                     result.append(STATUS("NotCompeting"))
                 else:
-                    if "rank" in r:
+                    if "time_behind" in r and r["time_behind"] is not None:
+                        result.append(TIMEBEHIND(str(r["time_behind"])))
+
+                    if "rank" in r and r["rank"] is not None:
                         result.append(POSITION(str(r["rank"])))
                     result.append(STATUS("OK"))
             else:
                 result.append(
                     STATUS(
                         {
                             ResultStatus.INACTIVE: "Inactive",
```

### Comparing `ooresults-0.2.2/ooresults/plugins/oe12.py` & `ooresults-0.2.3/ooresults/plugins/oe12.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/plugins/oe2003.py` & `ooresults-0.2.3/ooresults/plugins/oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/reader.py` & `ooresults-0.2.3/ooresults/reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/repo/__init__.py` & `ooresults-0.2.3/ooresults/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/repo/class_params.py` & `ooresults-0.2.3/ooresults/repo/class_params.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/repo/repo.py` & `ooresults-0.2.3/ooresults/repo/repo.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/repo/result_type.py` & `ooresults-0.2.3/ooresults/repo/result_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/repo/series_type.py` & `ooresults-0.2.3/ooresults/repo/series_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/repo/sqlite_repo.py` & `ooresults-0.2.3/ooresults/repo/sqlite_repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,25 +178,34 @@
         values = self.db.query(
             "SELECT "
             "classes.id,"
             "classes.name,"
             "classes.short_name,"
             "courses.id,"
             "courses.name,"
+            "courses.length,"
+            "courses.climb,"
+            "courses.controls,"
             "classes.params "
             "FROM classes "
             "LEFT JOIN courses ON classes.course_id = courses.id "
             "WHERE classes.event_id = " + web.db.sqlquote(event_id) + " "
             "ORDER BY classes.name ASC;"
         )
         values.names[values.names.index("id", 1)] = "course_id"
         values.names[values.names.index("name", 2)] = "course"
+        values.names[values.names.index("length", 1)] = "course_length"
+        values.names[values.names.index("climb", 1)] = "course_climb"
+        values.names[values.names.index("controls", 1)] = "number_of_controls"
         values = list(values)
         for c in values:
             c.params = UnpicklerZoneInfo(io.BytesIO(c.params)).load()
+            if c.number_of_controls is not None:
+                controls = UnpicklerZoneInfo(io.BytesIO(c.number_of_controls)).load()
+                c.number_of_controls = len(controls)
         return values
 
     def get_class(self, id: int):
         values = list(self.db.where("classes", id=id))
         for c in values:
             c.params = UnpicklerZoneInfo(io.BytesIO(c.params)).load()
         return values
```

### Comparing `ooresults-0.2.2/ooresults/repo/start_type.py` & `ooresults-0.2.3/ooresults/repo/start_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/repo/update/__init__.py` & `ooresults-0.2.3/ooresults/repo/update/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/repo/update/update_008.py` & `ooresults-0.2.3/ooresults/repo/update/update_008.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/repo/update/update_tables.py` & `ooresults-0.2.3/ooresults/repo/update/update_tables.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/schema/IOF.xsd` & `ooresults-0.2.3/ooresults/schema/IOF.xsd`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/schema/cardreader_log.json` & `ooresults-0.2.3/ooresults/schema/cardreader_log.json`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/server.py` & `ooresults-0.2.3/ooresults/server.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/set_legacy_mode.py` & `ooresults-0.2.3/ooresults/set_legacy_mode.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/static/style-tab.css` & `ooresults-0.2.3/ooresults/static/style-tab.css`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/static/style.css` & `ooresults-0.2.3/ooresults/static/style.css`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/static/w3.js` & `ooresults-0.2.3/ooresults/static/w3.js`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/add_class.html` & `ooresults-0.2.3/ooresults/templates/add_class.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/add_club.html` & `ooresults-0.2.3/ooresults/templates/add_club.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/add_competitor.html` & `ooresults-0.2.3/ooresults/templates/add_competitor.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/add_course.html` & `ooresults-0.2.3/ooresults/templates/add_course.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/add_entry.html` & `ooresults-0.2.3/ooresults/templates/add_entry.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/add_entry_competitors.html` & `ooresults-0.2.3/ooresults/templates/add_entry_competitors.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/add_entry_result.html` & `ooresults-0.2.3/ooresults/templates/add_entry_result.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/add_event.html` & `ooresults-0.2.3/ooresults/templates/add_event.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/classes_tab_content.html` & `ooresults-0.2.3/ooresults/templates/classes_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/classes_table.html` & `ooresults-0.2.3/ooresults/templates/classes_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/clubs_tab_content.html` & `ooresults-0.2.3/ooresults/templates/clubs_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/competitors_tab_content.html` & `ooresults-0.2.3/ooresults/templates/competitors_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/competitors_table.html` & `ooresults-0.2.3/ooresults/templates/competitors_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/courses_tab_content.html` & `ooresults-0.2.3/ooresults/templates/courses_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/courses_table.html` & `ooresults-0.2.3/ooresults/templates/courses_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/demo_reader.html` & `ooresults-0.2.3/ooresults/templates/demo_reader.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/entries_tab_content.html` & `ooresults-0.2.3/ooresults/templates/entries_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/entries_table.html` & `ooresults-0.2.3/ooresults/templates/entries_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/events_tab_content.html` & `ooresults-0.2.3/ooresults/templates/events_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/events_table.html` & `ooresults-0.2.3/ooresults/templates/events_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/main.html` & `ooresults-0.2.3/ooresults/templates/main.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/results_tab_content.html` & `ooresults-0.2.3/ooresults/templates/results_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/results_table.html` & `ooresults-0.2.3/ooresults/templates/results_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/root.html` & `ooresults-0.2.3/ooresults/templates/root.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/select_event.html` & `ooresults-0.2.3/ooresults/templates/select_event.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/series_settings.html` & `ooresults-0.2.3/ooresults/templates/series_settings.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/series_tab_content.html` & `ooresults-0.2.3/ooresults/templates/series_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/series_table.html` & `ooresults-0.2.3/ooresults/templates/series_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/si/si1_data.html` & `ooresults-0.2.3/ooresults/templates/si/si1_data.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/si/si1_page.html` & `ooresults-0.2.3/ooresults/templates/si/si1_page.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/si/si2_data.html` & `ooresults-0.2.3/ooresults/templates/si/si2_data.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/templates/si/si2_page.html` & `ooresults-0.2.3/ooresults/templates/si/si2_page.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/user.py` & `ooresults-0.2.3/ooresults/user.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/utils/__init__.py` & `ooresults-0.2.3/ooresults/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/utils/globals.py` & `ooresults-0.2.3/ooresults/utils/globals.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/websocket_server/__init__.py` & `ooresults-0.2.3/ooresults/websocket_server/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/websocket_server/si.py` & `ooresults-0.2.3/ooresults/websocket_server/si.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/websocket_server/websocket_handler.py` & `ooresults-0.2.3/ooresults/websocket_server/websocket_handler.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults/websocket_server/websocket_server.py` & `ooresults-0.2.3/ooresults/websocket_server/websocket_server.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/ooresults.egg-info/PKG-INFO` & `ooresults-0.2.3/ooresults.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooresults
-Version: 0.2.2
+Version: 0.2.3
 Summary: A software for the evaluation of the results of orienteering events
 Author: Rainer Garus
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ooresults-0.2.2/ooresults.egg-info/SOURCES.txt` & `ooresults-0.2.3/ooresults.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ooresults.egg-info/PKG-INFO
 ooresults.egg-info/SOURCES.txt
 ooresults.egg-info/dependency_links.txt
 ooresults.egg-info/entry_points.txt
 ooresults.egg-info/requires.txt
 ooresults.egg-info/top_level.txt
 ooresults/handler/__init__.py
+ooresults/handler/build_results.py
 ooresults/handler/classes.py
 ooresults/handler/clubs.py
 ooresults/handler/competitors.py
 ooresults/handler/courses.py
 ooresults/handler/demo_reader.py
 ooresults/handler/entries.py
 ooresults/handler/events.py
@@ -113,15 +114,17 @@
 tests/test_configuration.py
 tests/test_globals.py
 tests/test_handicap.py
 tests/test_ranking.py
 tests/test_series.py
 tests/test_user.py
 tests/model/__init__.py
+tests/model/test_build_series_result.py
 tests/model/test_courses.py
+tests/model/test_event_class_results.py
 tests/model/test_parse_cardreader_log.py
 tests/model/test_store_cardreader_result.py
 tests/plugins/test_export_competitors_oe2003.py
 tests/plugins/test_import_competitors_oe2003.py
 tests/plugins/test_plugin_iof_class_list.py
 tests/plugins/test_plugin_iof_competitor_list.py
 tests/plugins/test_plugin_iof_course_data.py
```

### Comparing `ooresults-0.2.2/pyproject.toml` & `ooresults-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ooresults"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   {name="Rainer Garus"},
 ]
 description = "A software for the evaluation of the results of orienteering events"
 readme = "README.rst"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
```

### Comparing `ooresults-0.2.2/setup.cfg` & `ooresults-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/__init__.py` & `ooresults-0.2.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/competitor.py` & `ooresults-0.2.3/tests/competitor.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/entry.py` & `ooresults-0.2.3/tests/entry.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/model/__init__.py` & `ooresults-0.2.3/tests/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/model/test_courses.py` & `ooresults-0.2.3/tests/model/test_courses.py`

 * *Files 4% similar despite different names*

```diff
@@ -205,23 +205,29 @@
     assert co[0].length == 4500
     assert co[0].climb == 90
     assert co[0].controls == ["101", "102", "103"]
     cl = list(model.get_classes(event_id=event_id))
     assert len(cl) == 2
     assert cl[0].id != cl[1].id
     assert cl[0].name == "Beginners"
-    assert cl[0].short_name == None
-    assert cl[0].course_id == None
-    assert cl[0].course == None
+    assert cl[0].short_name is None
+    assert cl[0].course_id is None
+    assert cl[0].course is None
+    assert cl[0].course_length is None
+    assert cl[0].course_climb is None
+    assert cl[0].number_of_controls is None
     assert cl[0].params == ClassParams()
     assert cl[1].id == class_1_id
     assert cl[1].name == "Elite Men"
     assert cl[1].short_name == "E Men"
     assert cl[1].course_id == course_1_id
     assert cl[1].course == "Bahn A"
+    assert cl[1].course_length == 4500
+    assert cl[1].course_climb == 90
+    assert cl[1].number_of_controls == 3
     assert cl[1].params == ClassParams()
 
 
 def test_import_course_data_update_class_course_assignment(
     db, event_id, class_1_id, class_2_id, course_1_id
 ):
     courses = [
@@ -255,20 +261,26 @@
     cl = list(model.get_classes(event_id=event_id))
     assert len(cl) == 2
     assert cl[0].id == class_1_id
     assert cl[0].name == "Elite Men"
     assert cl[0].short_name == "E Men"
     assert cl[0].course_id == co[1].id
     assert cl[0].course == "Bahn B"
+    assert cl[0].course_length == 3900
+    assert cl[0].course_climb == 120
+    assert cl[0].number_of_controls == 2
     assert cl[0].params == ClassParams()
     assert cl[1].id == class_2_id
     assert cl[1].name == "Elite Women"
     assert cl[1].short_name == "E Women"
     assert cl[1].course_id is None
     assert cl[1].course is None
+    assert cl[1].course_length is None
+    assert cl[1].course_climb is None
+    assert cl[1].number_of_controls is None
     assert cl[1].params == ClassParams()
 
 
 def test_import_course_data_remove_class_course_assigment(
     db, event_id, class_1_id, course_1_id
 ):
     class_course = [
@@ -289,14 +301,17 @@
     cl = list(model.get_classes(event_id=event_id))
     assert len(cl) == 1
     assert cl[0].id == class_1_id
     assert cl[0].name == "Elite Men"
     assert cl[0].short_name == "E Men"
     assert cl[0].course_id is None
     assert cl[0].course is None
+    assert cl[0].course_length is None
+    assert cl[0].course_climb is None
+    assert cl[0].number_of_controls is None
     assert cl[0].params == ClassParams()
 
 
 def test_import_course_data_update_or_add_class_course_assigments(
     db, event_id, course_1_id, class_1_id, class_2_id
 ):
     courses = [
@@ -338,36 +353,48 @@
     assert co[0].id == course_1_id
     assert co[0].name == "Bahn A"
     assert co[0].length == 4800
     assert co[0].climb == 120
     assert co[0].controls == ["101", "102"]
     assert co[1].id != co[0].id
     assert co[1].name == "Bahn B"
-    assert co[1].length == None
-    assert co[1].climb == None
+    assert co[1].length is None
+    assert co[1].climb is None
     assert co[1].controls == ["104"]
 
     cl = list(model.get_classes(event_id=event_id))
     assert len(cl) == 4
     assert cl[0].id not in (cl[2], cl[3])
     assert cl[0].name == "Beginners"
-    assert cl[0].course_id == None
-    assert cl[0].course == None
+    assert cl[0].course_id is None
+    assert cl[0].course is None
+    assert cl[0].course_length is None
+    assert cl[0].course_climb is None
+    assert cl[0].number_of_controls is None
     assert cl[0].params == ClassParams()
     assert cl[1].id not in (cl[2], cl[3])
     assert cl[1].name == "Elite"
-    assert cl[1].short_name == None
+    assert cl[1].short_name is None
     assert cl[1].course_id == co[1].id
     assert cl[1].course == "Bahn B"
+    assert cl[1].course_length is None
+    assert cl[1].course_climb is None
+    assert cl[1].number_of_controls == 1
     assert cl[1].params == ClassParams()
     assert cl[2].id == class_1_id
     assert cl[2].name == "Elite Men"
     assert cl[2].short_name == "E Men"
     assert cl[2].course_id == co[1].id
     assert cl[2].course == "Bahn B"
+    assert cl[2].course_length is None
+    assert cl[2].course_climb is None
+    assert cl[2].number_of_controls == 1
     assert cl[2].params == ClassParams()
     assert cl[3].id == class_2_id
     assert cl[3].name == "Elite Women"
     assert cl[3].short_name == "E Women"
     assert cl[3].course_id == course_1_id
     assert cl[3].course == "Bahn A"
+    assert cl[3].course_length == 4800
+    assert cl[3].course_climb == 120
+    assert cl[3].number_of_controls == 2
     assert cl[3].params == ClassParams()
```

### Comparing `ooresults-0.2.2/tests/model/test_parse_cardreader_log.py` & `ooresults-0.2.3/tests/model/test_parse_cardreader_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,19 +50,19 @@
 
     d = model.parse_cardreader_log(item=item)
     assert d["entryType"] == "cardRead"
     assert d["entryTime"] == e1
     assert d["controlCard"] == "123"
     assert d["result"].start_time == s1
     assert d["result"].finish_time == f1
-    assert d["result"].punched_clear_time == None
-    assert d["result"].punched_check_time == None
+    assert d["result"].punched_clear_time is None
+    assert d["result"].punched_check_time is None
     assert d["result"].punched_start_time == s1
     assert d["result"].punched_finish_time == f1
-    assert d["result"].time == None
+    assert d["result"].time is None
     assert d["result"].status == ResultStatus.FINISHED
     assert len(d["result"].split_times) == 2
     assert d["result"].split_times[0] == SplitTime(
         control_code="101", punch_time=c1, time=None, status="Additional"
     )
     assert d["result"].split_times[1] == SplitTime(
         control_code="103", punch_time=c2, time=None, status="Additional"
@@ -86,21 +86,21 @@
         "finishTime": "2015-01-01T12:39:07Z",
     }
 
     d = model.parse_cardreader_log(item=item)
     assert d["entryType"] == "cardRead"
     assert d["entryTime"] == e1
     assert d["controlCard"] == "123"
-    assert d["result"].start_time == None
+    assert d["result"].start_time is None
     assert d["result"].finish_time == f1
-    assert d["result"].punched_clear_time == None
-    assert d["result"].punched_check_time == None
-    assert d["result"].punched_start_time == None
+    assert d["result"].punched_clear_time is None
+    assert d["result"].punched_check_time is None
+    assert d["result"].punched_start_time is None
     assert d["result"].punched_finish_time == f1
-    assert d["result"].time == None
+    assert d["result"].time is None
     assert d["result"].status == ResultStatus.FINISHED
     assert len(d["result"].split_times) == 2
     assert d["result"].split_times[0] == SplitTime(
         control_code="101", punch_time=c1, time=None, status="Additional"
     )
     assert d["result"].split_times[1] == SplitTime(
         control_code="103", punch_time=c2, time=None, status="Additional"
@@ -125,20 +125,20 @@
     }
 
     d = model.parse_cardreader_log(item=item)
     assert d["entryType"] == "cardRead"
     assert d["entryTime"] == e1
     assert d["controlCard"] == "123"
     assert d["result"].start_time == s1
-    assert d["result"].finish_time == None
-    assert d["result"].punched_clear_time == None
-    assert d["result"].punched_check_time == None
+    assert d["result"].finish_time is None
+    assert d["result"].punched_clear_time is None
+    assert d["result"].punched_check_time is None
     assert d["result"].punched_start_time == s1
-    assert d["result"].punched_finish_time == None
-    assert d["result"].time == None
+    assert d["result"].punched_finish_time is None
+    assert d["result"].time is None
     assert d["result"].status == ResultStatus.FINISHED
     assert len(d["result"].split_times) == 2
     assert d["result"].split_times[0] == SplitTime(
         control_code="101", punch_time=c1, time=None, status="Additional"
     )
     assert d["result"].split_times[1] == SplitTime(
         control_code="103", punch_time=c2, time=None, status="Additional"
@@ -160,21 +160,21 @@
         ],
     }
 
     d = model.parse_cardreader_log(item=item)
     assert d["entryType"] == "cardRead"
     assert d["entryTime"] == e1
     assert d["controlCard"] == "123"
-    assert d["result"].start_time == None
-    assert d["result"].finish_time == None
-    assert d["result"].punched_clear_time == None
-    assert d["result"].punched_check_time == None
-    assert d["result"].punched_start_time == None
-    assert d["result"].punched_finish_time == None
-    assert d["result"].time == None
+    assert d["result"].start_time is None
+    assert d["result"].finish_time is None
+    assert d["result"].punched_clear_time is None
+    assert d["result"].punched_check_time is None
+    assert d["result"].punched_start_time is None
+    assert d["result"].punched_finish_time is None
+    assert d["result"].time is None
     assert d["result"].status == ResultStatus.FINISHED
     assert len(d["result"].split_times) == 2
     assert d["result"].split_times[0] == SplitTime(
         control_code="101", punch_time=c1, time=None, status="Additional"
     )
     assert d["result"].split_times[1] == SplitTime(
         control_code="103", punch_time=c2, time=None, status="Additional"
@@ -198,21 +198,21 @@
         ],
     }
 
     d = model.parse_cardreader_log(item=item)
     assert d["entryType"] == "cardRead"
     assert d["entryTime"] == e1
     assert d["controlCard"] == "123"
-    assert d["result"].start_time == None
-    assert d["result"].finish_time == None
+    assert d["result"].start_time is None
+    assert d["result"].finish_time is None
     assert d["result"].punched_clear_time == cl
-    assert d["result"].punched_check_time == None
-    assert d["result"].punched_start_time == None
-    assert d["result"].punched_finish_time == None
-    assert d["result"].time == None
+    assert d["result"].punched_check_time is None
+    assert d["result"].punched_start_time is None
+    assert d["result"].punched_finish_time is None
+    assert d["result"].time is None
     assert d["result"].status == ResultStatus.FINISHED
     assert len(d["result"].split_times) == 2
     assert d["result"].split_times[0] == SplitTime(
         control_code="101", punch_time=c1, time=None, status="Additional"
     )
     assert d["result"].split_times[1] == SplitTime(
         control_code="103", punch_time=c2, time=None, status="Additional"
@@ -236,21 +236,21 @@
         ],
     }
 
     d = model.parse_cardreader_log(item=item)
     assert d["entryType"] == "cardRead"
     assert d["entryTime"] == e1
     assert d["controlCard"] == "123"
-    assert d["result"].start_time == None
-    assert d["result"].finish_time == None
-    assert d["result"].punched_clear_time == None
+    assert d["result"].start_time is None
+    assert d["result"].finish_time is None
+    assert d["result"].punched_clear_time is None
     assert d["result"].punched_check_time == ch
-    assert d["result"].punched_start_time == None
-    assert d["result"].punched_finish_time == None
-    assert d["result"].time == None
+    assert d["result"].punched_start_time is None
+    assert d["result"].punched_finish_time is None
+    assert d["result"].time is None
     assert d["result"].status == ResultStatus.FINISHED
     assert len(d["result"].split_times) == 2
     assert d["result"].split_times[0] == SplitTime(
         control_code="101", punch_time=c1, time=None, status="Additional"
     )
     assert d["result"].split_times[1] == SplitTime(
         control_code="103", punch_time=c2, time=None, status="Additional"
@@ -273,19 +273,19 @@
 
     d = model.parse_cardreader_log(item=item)
     assert d["entryType"] == "cardRead"
     assert d["entryTime"] == e1
     assert d["controlCard"] == "123"
     assert d["result"].start_time == s1
     assert d["result"].finish_time == f1
-    assert d["result"].punched_clear_time == None
-    assert d["result"].punched_check_time == None
+    assert d["result"].punched_clear_time is None
+    assert d["result"].punched_check_time is None
     assert d["result"].punched_start_time == s1
     assert d["result"].punched_finish_time == f1
-    assert d["result"].time == None
+    assert d["result"].time is None
     assert d["result"].status == ResultStatus.FINISHED
     assert len(d["result"].split_times) == 0
     assert d["result"].split_times == []
 
 
 def test_parse_with_many_controls():
     e1 = datetime(2015, 1, 1, 13, 0, 0, tzinfo=timezone.utc)
@@ -319,19 +319,19 @@
 
     d = model.parse_cardreader_log(item=item)
     assert d["entryType"] == "cardRead"
     assert d["entryTime"] == e1
     assert d["controlCard"] == "123"
     assert d["result"].start_time == s1
     assert d["result"].finish_time == f1
-    assert d["result"].punched_clear_time == None
-    assert d["result"].punched_check_time == None
+    assert d["result"].punched_clear_time is None
+    assert d["result"].punched_check_time is None
     assert d["result"].punched_start_time == s1
     assert d["result"].punched_finish_time == f1
-    assert d["result"].time == None
+    assert d["result"].time is None
     assert d["result"].status == ResultStatus.FINISHED
     assert len(d["result"].split_times) == 7
     assert d["result"].split_times[0] == SplitTime(
         control_code="101", punch_time=c1, time=None, status="Additional"
     )
     assert d["result"].split_times[1] == SplitTime(
         control_code="105", punch_time=c2, time=None, status="Additional"
```

### Comparing `ooresults-0.2.2/tests/model/test_store_cardreader_result.py` & `ooresults-0.2.3/tests/model/test_store_cardreader_result.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/plugins/test_export_competitors_oe2003.py` & `ooresults-0.2.3/tests/plugins/test_export_competitors_oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/plugins/test_import_competitors_oe2003.py` & `ooresults-0.2.3/tests/plugins/test_import_competitors_oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/plugins/test_plugin_iof_class_list.py` & `ooresults-0.2.3/tests/plugins/test_plugin_iof_class_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/plugins/test_plugin_iof_competitor_list.py` & `ooresults-0.2.3/tests/plugins/test_plugin_iof_competitor_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/plugins/test_plugin_iof_course_data.py` & `ooresults-0.2.3/tests/plugins/test_plugin_iof_course_data.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/plugins/test_plugin_iof_entry_list.py` & `ooresults-0.2.3/tests/plugins/test_plugin_iof_entry_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/plugins/test_plugin_iof_result_list.py` & `ooresults-0.2.3/tests/plugins/test_plugin_iof_result_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,14 +51,16 @@
       <Organisation>
         <Name>OC Kanzleramt</Name>
       </Organisation>
       <Result>
         <StartTime>2020-02-09T10:00:00+01:00</StartTime>
         <FinishTime>2020-02-09T10:33:21+01:00</FinishTime>
         <Time>2001</Time>
+        <TimeBehind>0</TimeBehind>
+        <Position>1</Position>
         <Status>OK</Status>
         <SplitTime>
           <ControlCode>31</ControlCode>
           <Time>501</Time>
         </SplitTime>
         <SplitTime>
           <ControlCode>32</ControlCode>
@@ -220,14 +222,16 @@
       <Organisation>
         <Name>OC Kanzleramt</Name>
       </Organisation>
       <Result>
         <StartTime>2020-02-09T10:00:00+01:00</StartTime>
         <FinishTime>2020-02-09T10:33:21+01:00</FinishTime>
         <Time>2001</Time>
+        <TimeBehind>0</TimeBehind>
+        <Position>1</Position>
         <Status>OK</Status>
         <SplitTime>
           <ControlCode>31</ControlCode>
           <Time>501</Time>
         </SplitTime>
         <SplitTime>
           <ControlCode>32</ControlCode>
@@ -253,45 +257,75 @@
 """
     document = iof_result_list.create_result_list(
         {
             "name": "1. O-Cup 2020",
             "date": datetime.date(year=2020, month=2, day=9),
         },
         [
-            {
-                "first_name": "Angela",
-                "last_name": "Merkel",
-                "class_": "Bahn A - Lang",
-                "club": "OC Kanzleramt",
-                "chip": "1234567",
-                "gender": "F",
-                "year": 1972,
-                "not_competing": False,
-                "result": result_type.PersonRaceResult(
-                    start_time=datetime.datetime(
-                        2020, 2, 9, 10, 0, 0, tzinfo=timezone(timedelta(hours=1))
-                    ),
-                    finish_time=datetime.datetime(
-                        2020, 2, 9, 10, 33, 21, tzinfo=timezone(timedelta(hours=1))
-                    ),
-                    status=ResultStatus.OK,
-                    time=2001,
-                    split_times=[
-                        result_type.SplitTime(control_code="31", status="OK", time=501),
-                        result_type.SplitTime(control_code="32", status="OK", time=720),
-                        result_type.SplitTime(control_code="31", status="OK", time=818),
-                        result_type.SplitTime(
-                            control_code="33", status="OK", time=1136
-                        ),
-                        result_type.SplitTime(
-                            control_code="31", status="OK", time=1593
+            (
+                {
+                    "name": "Bahn A - Lang",
+                    "course_length": None,
+                    "course_climb": None,
+                    "number_of_controls": None,
+                },
+                [
+                    {
+                        "first_name": "Angela",
+                        "last_name": "Merkel",
+                        "class_": "Bahn A - Lang",
+                        "club": "OC Kanzleramt",
+                        "chip": "1234567",
+                        "gender": "F",
+                        "year": 1972,
+                        "not_competing": False,
+                        "result": result_type.PersonRaceResult(
+                            start_time=datetime.datetime(
+                                2020,
+                                2,
+                                9,
+                                10,
+                                0,
+                                0,
+                                tzinfo=timezone(timedelta(hours=1)),
+                            ),
+                            finish_time=datetime.datetime(
+                                2020,
+                                2,
+                                9,
+                                10,
+                                33,
+                                21,
+                                tzinfo=timezone(timedelta(hours=1)),
+                            ),
+                            status=ResultStatus.OK,
+                            time=2001,
+                            split_times=[
+                                result_type.SplitTime(
+                                    control_code="31", status="OK", time=501
+                                ),
+                                result_type.SplitTime(
+                                    control_code="32", status="OK", time=720
+                                ),
+                                result_type.SplitTime(
+                                    control_code="31", status="OK", time=818
+                                ),
+                                result_type.SplitTime(
+                                    control_code="33", status="OK", time=1136
+                                ),
+                                result_type.SplitTime(
+                                    control_code="31", status="OK", time=1593
+                                ),
+                            ],
                         ),
-                    ],
-                ),
-            },
+                        "time_behind": 0,
+                        "rank": 1,
+                    },
+                ],
+            ),
         ],
     )
     assert document == bytes(content, encoding="utf-8")
 
 
 def test_export_result_list_not_competing():
     content = """\
@@ -331,103 +365,57 @@
 """
     document = iof_result_list.create_result_list(
         {
             "name": "1. O-Cup 2020",
             "date": datetime.date(year=2020, month=2, day=9),
         },
         [
-            {
-                "first_name": "Angela",
-                "last_name": "Merkel",
-                "class_": "Bahn A - Lang",
-                "club": "OC Kanzleramt",
-                "chip": "1234567",
-                "gender": "F",
-                "year": 1972,
-                "not_competing": True,
-                "result": result_type.PersonRaceResult(
-                    start_time=datetime.datetime(
-                        2020, 2, 9, 10, 0, 0, tzinfo=timezone(timedelta(hours=1))
-                    ),
-                    finish_time=datetime.datetime(
-                        2020, 2, 9, 10, 33, 21, tzinfo=timezone(timedelta(hours=1))
-                    ),
-                    status=ResultStatus.OK,
-                    time=2001,
-                ),
-            },
-        ],
-    )
-    assert document == bytes(content, encoding="utf-8")
-
-
-def test_export_result_list_not_competing():
-    content = """\
-<?xml version='1.0' encoding='UTF-8'?>
-<ResultList xmlns="http://www.orienteering.org/datastandard/3.0" iofVersion="3.0" creator="ooresults (https://pypi.org/project/ooresults)">
-  <Event>
-    <Name>1. O-Cup 2020</Name>
-    <StartTime>
-      <Date>2020-02-09</Date>
-    </StartTime>
-  </Event>
-  <ClassResult>
-    <Class>
-      <Name>Bahn A - Lang</Name>
-    </Class>
-    <PersonResult>
-      <Person sex="F">
-        <Name>
-          <Family>Merkel</Family>
-          <Given>Angela</Given>
-        </Name>
-        <BirthDate>1972-01-01</BirthDate>
-      </Person>
-      <Organisation>
-        <Name>OC Kanzleramt</Name>
-      </Organisation>
-      <Result>
-        <StartTime>2020-02-09T10:00:00+01:00</StartTime>
-        <FinishTime>2020-02-09T10:33:21+01:00</FinishTime>
-        <Time>2001</Time>
-        <Position>1</Position>
-        <Status>OK</Status>
-        <ControlCard punchingSystem="SI">1234567</ControlCard>
-      </Result>
-    </PersonResult>
-  </ClassResult>
-</ResultList>
-"""
-    document = iof_result_list.create_result_list(
-        {
-            "name": "1. O-Cup 2020",
-            "date": datetime.date(year=2020, month=2, day=9),
-        },
-        [
-            {
-                "first_name": "Angela",
-                "last_name": "Merkel",
-                "class_": "Bahn A - Lang",
-                "club": "OC Kanzleramt",
-                "chip": "1234567",
-                "gender": "F",
-                "year": 1972,
-                "not_competing": False,
-                "rank": 1,
-                "result": result_type.PersonRaceResult(
-                    start_time=datetime.datetime(
-                        2020, 2, 9, 10, 0, 0, tzinfo=timezone(timedelta(hours=1))
-                    ),
-                    finish_time=datetime.datetime(
-                        2020, 2, 9, 10, 33, 21, tzinfo=timezone(timedelta(hours=1))
-                    ),
-                    status=ResultStatus.OK,
-                    time=2001,
-                ),
-            },
+            (
+                {
+                    "name": "Bahn A - Lang",
+                    "course_length": None,
+                    "course_climb": None,
+                    "number_of_controls": None,
+                },
+                [
+                    {
+                        "first_name": "Angela",
+                        "last_name": "Merkel",
+                        "class_": "Bahn A - Lang",
+                        "club": "OC Kanzleramt",
+                        "chip": "1234567",
+                        "gender": "F",
+                        "year": 1972,
+                        "not_competing": True,
+                        "result": result_type.PersonRaceResult(
+                            start_time=datetime.datetime(
+                                2020,
+                                2,
+                                9,
+                                10,
+                                0,
+                                0,
+                                tzinfo=timezone(timedelta(hours=1)),
+                            ),
+                            finish_time=datetime.datetime(
+                                2020,
+                                2,
+                                9,
+                                10,
+                                33,
+                                21,
+                                tzinfo=timezone(timedelta(hours=1)),
+                            ),
+                            status=ResultStatus.OK,
+                            time=2001,
+                        ),
+                        "rank": None,
+                    },
+                ],
+            ),
         ],
     )
     assert document == bytes(content, encoding="utf-8")
 
 
 def test_import_result_list_without_class_result():
     content = """\
@@ -492,14 +480,16 @@
           <Given>Angela</Given>
         </Name>
       </Person>
       <Result>
         <StartTime>2020-02-09T10:05:00Z</StartTime>
         <FinishTime>2020-02-09T10:25:21Z</FinishTime>
         <Time>1221</Time>
+        <TimeBehind>0</TimeBehind>
+        <Position>1</Position>
         <Status>OK</Status>
         <SplitTime>
           <ControlCode>41</ControlCode>
           <Time>301</Time>
         </SplitTime>
         <SplitTime>
           <ControlCode>42</ControlCode>
@@ -682,25 +672,32 @@
       <Date>2020-02-09</Date>
     </StartTime>
   </Event>
   <ClassResult>
     <Class>
       <Name>Bahn A - Lang</Name>
     </Class>
+    <Course>
+      <Length>5100</Length>
+      <Climb>110</Climb>
+      <NumberOfControls>10</NumberOfControls>
+    </Course>
     <PersonResult>
       <Person>
         <Name>
           <Family>Merkel</Family>
           <Given>Angela</Given>
         </Name>
       </Person>
       <Result>
         <StartTime>2020-02-09T10:05:00+00:00</StartTime>
         <FinishTime>2020-02-09T10:25:21+00:00</FinishTime>
         <Time>1221</Time>
+        <TimeBehind>0</TimeBehind>
+        <Position>1</Position>
         <Status>OK</Status>
         <SplitTime>
           <ControlCode>41</ControlCode>
           <Time>301</Time>
         </SplitTime>
         <SplitTime>
           <ControlCode>42</ControlCode>
@@ -743,14 +740,17 @@
       </Result>
     </PersonResult>
   </ClassResult>
   <ClassResult>
     <Class>
       <Name>Bahn B - Mittel</Name>
     </Class>
+    <Course>
+      <Length>2800</Length>
+    </Course>
     <PersonResult>
       <Person>
         <Name>
           <Family>Merkel</Family>
           <Given>Claudia</Given>
         </Name>
       </Person>
@@ -781,77 +781,121 @@
 """
     document = iof_result_list.create_result_list(
         {
             "name": "1. O-Cup 2020",
             "date": datetime.date(year=2020, month=2, day=9),
         },
         [
-            {
-                "first_name": "Angela",
-                "last_name": "Merkel",
-                "class_": "Bahn A - Lang",
-                "not_competing": False,
-                "result": result_type.PersonRaceResult(
-                    status=ResultStatus.OK,
-                    start_time=datetime.datetime(
-                        2020, 2, 9, 10, 5, 0, tzinfo=timezone.utc
-                    ),
-                    finish_time=datetime.datetime(
-                        2020, 2, 9, 10, 25, 21, tzinfo=timezone.utc
-                    ),
-                    time=1221,
-                    split_times=[
-                        result_type.SplitTime(control_code="41", status="OK", time=301),
-                        result_type.SplitTime(control_code="42", status="OK", time=526),
-                        result_type.SplitTime(control_code="41", status="OK", time=914),
-                        result_type.SplitTime(
-                            control_code="43", status="OK", time=1100
+            (
+                {
+                    "name": "Bahn A - Lang",
+                    "course_length": 5100.0,
+                    "course_climb": 110.0,
+                    "number_of_controls": 10,
+                },
+                [
+                    {
+                        "first_name": "Angela",
+                        "last_name": "Merkel",
+                        "class_": "Bahn A - Lang",
+                        "not_competing": False,
+                        "result": result_type.PersonRaceResult(
+                            status=ResultStatus.OK,
+                            start_time=datetime.datetime(
+                                2020, 2, 9, 10, 5, 0, tzinfo=timezone.utc
+                            ),
+                            finish_time=datetime.datetime(
+                                2020, 2, 9, 10, 25, 21, tzinfo=timezone.utc
+                            ),
+                            time=1221,
+                            split_times=[
+                                result_type.SplitTime(
+                                    control_code="41", status="OK", time=301
+                                ),
+                                result_type.SplitTime(
+                                    control_code="42", status="OK", time=526
+                                ),
+                                result_type.SplitTime(
+                                    control_code="41", status="OK", time=914
+                                ),
+                                result_type.SplitTime(
+                                    control_code="43", status="OK", time=1100
+                                ),
+                            ],
                         ),
-                    ],
-                ),
-            },
-            {
-                "first_name": "Claudia",
-                "last_name": "Merkel",
-                "class_": "Bahn B - Mittel",
-                "chip": "1234567",
-                "not_competing": False,
-                "result": result_type.PersonRaceResult(
-                    status=ResultStatus.MISSING_PUNCH,
-                    start_time=datetime.datetime(
-                        2020, 2, 9, 10, 0, 0, tzinfo=timezone.utc
-                    ),
-                    finish_time=datetime.datetime(
-                        2020, 2, 9, 10, 33, 21, tzinfo=timezone.utc
-                    ),
-                    time=2001,
-                    split_times=[
-                        result_type.SplitTime(control_code="31", status="OK", time=501),
-                        result_type.SplitTime(control_code="32", status="Missing"),
-                        result_type.SplitTime(control_code="31", status="Missing"),
-                        result_type.SplitTime(
-                            control_code="33", status="Additional", time=1136
+                        "time_behind": 0,
+                        "rank": 1,
+                    },
+                    {
+                        "first_name": "Birgit",
+                        "last_name": "Merkel",
+                        "class_": "Bahn A - Lang",
+                        "not_competing": False,
+                        "result": result_type.PersonRaceResult(
+                            status=ResultStatus.DID_NOT_FINISH,
+                            start_time=datetime.datetime(
+                                2020, 2, 9, 10, 6, 0, tzinfo=timezone.utc
+                            ),
+                            split_times=[
+                                result_type.SplitTime(
+                                    control_code="41", status="OK", time=501
+                                ),
+                                result_type.SplitTime(
+                                    control_code="42", status="OK", time=720
+                                ),
+                                result_type.SplitTime(
+                                    control_code="41", status="Missing"
+                                ),
+                                result_type.SplitTime(
+                                    control_code="43", status="Missing"
+                                ),
+                            ],
                         ),
-                    ],
-                ),
-            },
-            {
-                "first_name": "Birgit",
-                "last_name": "Merkel",
-                "class_": "Bahn A - Lang",
-                "not_competing": False,
-                "result": result_type.PersonRaceResult(
-                    status=ResultStatus.DID_NOT_FINISH,
-                    start_time=datetime.datetime(
-                        2020, 2, 9, 10, 6, 0, tzinfo=timezone.utc
-                    ),
-                    split_times=[
-                        result_type.SplitTime(control_code="41", status="OK", time=501),
-                        result_type.SplitTime(control_code="42", status="OK", time=720),
-                        result_type.SplitTime(control_code="41", status="Missing"),
-                        result_type.SplitTime(control_code="43", status="Missing"),
-                    ],
-                ),
-            },
+                        "rank": None,
+                    },
+                ],
+            ),
+            (
+                {
+                    "name": "Bahn B - Mittel",
+                    "course_length": 2800.0,
+                    "course_climb": None,
+                    "number_of_controls": 0,
+                },
+                [
+                    {
+                        "first_name": "Claudia",
+                        "last_name": "Merkel",
+                        "class_": "Bahn B - Mittel",
+                        "chip": "1234567",
+                        "not_competing": False,
+                        "result": result_type.PersonRaceResult(
+                            status=ResultStatus.MISSING_PUNCH,
+                            start_time=datetime.datetime(
+                                2020, 2, 9, 10, 0, 0, tzinfo=timezone.utc
+                            ),
+                            finish_time=datetime.datetime(
+                                2020, 2, 9, 10, 33, 21, tzinfo=timezone.utc
+                            ),
+                            time=2001,
+                            split_times=[
+                                result_type.SplitTime(
+                                    control_code="31", status="OK", time=501
+                                ),
+                                result_type.SplitTime(
+                                    control_code="32", status="Missing"
+                                ),
+                                result_type.SplitTime(
+                                    control_code="31", status="Missing"
+                                ),
+                                result_type.SplitTime(
+                                    control_code="33", status="Additional", time=1136
+                                ),
+                            ],
+                        ),
+                        "rank": None,
+                    },
+                ],
+            ),
         ],
     )
     assert document == bytes(content, encoding="utf-8")
```

### Comparing `ooresults-0.2.2/tests/repo/__init__.py` & `ooresults-0.2.3/tests/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/repo/test_classes.py` & `ooresults-0.2.3/tests/repo/test_classes.py`

 * *Files 18% similar despite different names*

```diff
@@ -51,21 +51,32 @@
         key=None,
         publish=False,
         series=None,
     )
 
 
 @pytest.fixture
-def course_id(db, event_1_id):
+def course_1_id(db, event_1_id):
     return db.add_course(
         event_id=event_1_id,
         name="Course 1",
         length=None,
         climb=None,
-        controls="",
+        controls=[],
+    )
+
+
+@pytest.fixture
+def course_2_id(db, event_1_id):
+    return db.add_course(
+        event_id=event_1_id,
+        name="Course 2",
+        length=2300,
+        climb=90,
+        controls=["101", "102"],
     )
 
 
 @pytest.fixture
 def class_1_id(db, event_1_id):
     return db.add_class(
         event_id=event_1_id,
@@ -73,20 +84,20 @@
         short_name="C 1",
         course_id=None,
         params=ClassParams(),
     )
 
 
 @pytest.fixture
-def class_2_id(db, event_1_id, course_id):
+def class_2_id(db, event_1_id, course_1_id):
     return db.add_class(
         event_id=event_1_id,
         name="Class 2",
         short_name=None,
-        course_id=course_id,
+        course_id=course_1_id,
         params=ClassParams(),
     )
 
 
 @pytest.fixture
 def class_3_id(db, event_2_id):
     return db.add_class(
@@ -119,97 +130,115 @@
 
 def test_get_classes_after_adding_one_class(db, event_1_id, class_1_id):
     c = list(db.get_classes(event_id=event_1_id))
     assert len(c) == 1
     assert c[0].id == class_1_id
     assert c[0].name == "Class 1"
     assert c[0].short_name == "C 1"
-    assert c[0].course_id == None
-    assert c[0].course == None
+    assert c[0].course_id is None
+    assert c[0].course is None
+    assert c[0].course_length is None
+    assert c[0].course_climb is None
+    assert c[0].number_of_controls is None
     assert c[0].params == ClassParams()
 
 
 def test_get_classes_for_first_event(
-    db, event_1_id, course_id, class_1_id, class_2_id, class_3_id
+    db, event_1_id, course_1_id, class_1_id, class_2_id, class_3_id
 ):
     c = list(db.get_classes(event_id=event_1_id))
     assert len(c) == 2
     assert c[0].id != c[1].id
 
     assert c[0].id == class_1_id
     assert c[0].name == "Class 1"
     assert c[0].short_name == "C 1"
-    assert c[0].course_id == None
-    assert c[0].course == None
+    assert c[0].course_id is None
+    assert c[0].course is None
+    assert c[0].course_length is None
+    assert c[0].course_climb is None
+    assert c[0].number_of_controls is None
     assert c[0].params == ClassParams()
     assert c[1].id == class_2_id
     assert c[1].name == "Class 2"
-    assert c[1].short_name == None
-    assert c[1].course_id == course_id
+    assert c[1].short_name is None
+    assert c[1].course_id == course_1_id
     assert c[1].course == "Course 1"
+    assert c[1].course_length is None
+    assert c[1].course_climb is None
+    assert c[1].number_of_controls == 0
     assert c[1].params == ClassParams()
 
 
 def test_get_classes_for_second_event(
-    db, event_2_id, course_id, class_1_id, class_2_id, class_3_id
+    db, event_2_id, course_1_id, class_1_id, class_2_id, class_3_id
 ):
     c = list(db.get_classes(event_id=event_2_id))
     assert len(c) == 1
 
     assert c[0].id == class_3_id
     assert c[0].name == "Class 3"
     assert c[0].short_name == "C 3"
-    assert c[0].course_id == None
-    assert c[0].course == None
+    assert c[0].course_id is None
+    assert c[0].course is None
+    assert c[0].course_length is None
+    assert c[0].course_climb is None
+    assert c[0].number_of_controls is None
     assert c[0].params == ClassParams()
 
 
 def test_get_first_added_class(db, class_1_id, class_2_id):
     c = list(db.get_class(id=class_1_id))
     assert len(c) == 1
     assert c[0].id == class_1_id
     assert c[0].name == "Class 1"
     assert c[0].short_name == "C 1"
-    assert c[0].course_id == None
+    assert c[0].course_id is None
     assert c[0].params == ClassParams()
 
 
-def test_get_last_added_class(db, course_id, class_1_id, class_2_id):
+def test_get_last_added_class(db, course_1_id, class_1_id, class_2_id):
     c = list(db.get_class(id=class_2_id))
     assert len(c) == 1
     assert c[0].id == class_2_id
     assert c[0].name == "Class 2"
-    assert c[0].short_name == None
-    assert c[0].course_id == course_id
+    assert c[0].short_name is None
+    assert c[0].course_id == course_1_id
     assert c[0].params == ClassParams()
 
 
-def test_update_first_added_class(db, event_1_id, course_id, class_1_id, class_2_id):
+def test_update_first_added_class(db, event_1_id, course_1_id, class_1_id, class_2_id):
     db.update_class(
         id=class_1_id,
         name="Class 3",
         short_name="C 3",
-        course_id=course_id,
+        course_id=course_1_id,
         params=ClassParams(),
     )
     c = list(db.get_classes(event_id=event_1_id))
     assert len(c) == 2
     assert c[0].id != c[1].id
 
     assert c[0].id == class_2_id
     assert c[0].name == "Class 2"
-    assert c[0].short_name == None
-    assert c[0].course_id == course_id
+    assert c[0].short_name is None
+    assert c[0].course_id == course_1_id
     assert c[0].course == "Course 1"
+    assert c[0].course_length is None
+    assert c[0].course_climb is None
+    assert c[0].number_of_controls == 0
     assert c[0].params == ClassParams()
     assert c[1].id == class_1_id
     assert c[1].name == "Class 3"
     assert c[1].short_name == "C 3"
-    assert c[1].course_id == course_id
+    assert c[1].course_id == course_1_id
     assert c[1].course == "Course 1"
+    assert c[1].course_length is None
+    assert c[1].course_climb is None
+    assert c[1].number_of_controls == 0
     assert c[1].params == ClassParams()
 
 
 def test_update_last_added_class(db, event_1_id, class_1_id, class_2_id):
     db.update_class(
         id=class_2_id,
         name="Class 3",
@@ -220,46 +249,58 @@
     c = list(db.get_classes(event_id=event_1_id))
     assert len(c) == 2
     assert c[0].id != c[1].id
 
     assert c[0].id == class_1_id
     assert c[0].name == "Class 1"
     assert c[0].short_name == "C 1"
-    assert c[0].course_id == None
-    assert c[0].course == None
+    assert c[0].course_id is None
+    assert c[0].course is None
+    assert c[0].course_length is None
+    assert c[0].course_climb is None
+    assert c[0].number_of_controls is None
     assert c[0].params == ClassParams()
     assert c[1].id == class_2_id
     assert c[1].name == "Class 3"
     assert c[1].short_name == "C 3"
-    assert c[1].course_id == None
-    assert c[1].course == None
+    assert c[1].course_id is None
+    assert c[1].course is None
+    assert c[1].course_length is None
+    assert c[1].course_climb is None
+    assert c[1].number_of_controls is None
     assert c[1].params == ClassParams()
 
 
-def test_delete_first_added_class(db, event_1_id, course_id, class_1_id, class_2_id):
+def test_delete_first_added_class(db, event_1_id, course_1_id, class_1_id, class_2_id):
     db.delete_class(id=class_1_id)
     c = list(db.get_classes(event_id=event_1_id))
     assert len(c) == 1
     assert c[0].id == class_2_id
     assert c[0].name == "Class 2"
-    assert c[0].short_name == None
-    assert c[0].course_id == course_id
+    assert c[0].short_name is None
+    assert c[0].course_id == course_1_id
     assert c[0].course == "Course 1"
+    assert c[0].course_length is None
+    assert c[0].course_climb is None
+    assert c[0].number_of_controls == 0
     assert c[0].params == ClassParams()
 
 
 def test_delete_last_added_class(db, event_1_id, class_1_id, class_2_id):
     db.delete_class(id=class_2_id)
     c = list(db.get_classes(event_id=event_1_id))
     assert len(c) == 1
     assert c[0].id == class_1_id
     assert c[0].name == "Class 1"
     assert c[0].short_name == "C 1"
-    assert c[0].course_id == None
-    assert c[0].course == None
+    assert c[0].course_id is None
+    assert c[0].course is None
+    assert c[0].course_length is None
+    assert c[0].course_climb is None
+    assert c[0].number_of_controls is None
     assert c[0].params == ClassParams()
 
 
 def test_delete_classes_deletes_all_classes(db, event_1_id, class_1_id, class_2_id):
     db.delete_classes(event_id=event_1_id)
     c = list(db.get_classes(event_id=event_1_id))
     assert len(c) == 0
@@ -314,16 +355,19 @@
 ):
     db.delete_class(id=class_1_id + 1)
     c = list(db.get_classes(event_id=event_1_id))
     assert len(c) == 1
     assert c[0].id == class_1_id
     assert c[0].name == "Class 1"
     assert c[0].short_name == "C 1"
-    assert c[0].course_id == None
-    assert c[0].course == None
+    assert c[0].course_id is None
+    assert c[0].course is None
+    assert c[0].course_length is None
+    assert c[0].course_climb is None
+    assert c[0].number_of_controls is None
     assert c[0].params == ClassParams()
 
 
 def test_delete_class_used_in_entry_raises_exception(
     db, event_1_id, entry_id, class_1_id
 ):
     with pytest.raises(repo.ClassUsedError):
@@ -331,7 +375,41 @@
 
 
 def test_delete_classes_if_entry_exist_raises_exception(
     db, event_1_id, entry_id, class_1_id
 ):
     with pytest.raises(repo.ClassUsedError):
         db.delete_classes(event_id=event_1_id)
+
+
+def test_get_course_data(
+    db, event_1_id, course_1_id, course_2_id, class_1_id, class_2_id
+):
+    db.update_class(
+        id=class_1_id,
+        name="Class 3",
+        short_name="C 3",
+        course_id=course_2_id,
+        params=ClassParams(),
+    )
+    c = list(db.get_classes(event_id=event_1_id))
+    assert len(c) == 2
+    assert c[0].id != c[1].id
+
+    assert c[0].id == class_2_id
+    assert c[0].name == "Class 2"
+    assert c[0].short_name is None
+    assert c[0].course_id == course_1_id
+    assert c[0].course == "Course 1"
+    assert c[0].course_length is None
+    assert c[0].course_climb is None
+    assert c[0].number_of_controls == 0
+    assert c[0].params == ClassParams()
+    assert c[1].id == class_1_id
+    assert c[1].name == "Class 3"
+    assert c[1].short_name == "C 3"
+    assert c[1].course_id == course_2_id
+    assert c[1].course == "Course 2"
+    assert c[1].course_length == 2300
+    assert c[1].course_climb == 90
+    assert c[1].number_of_controls == 2
+    assert c[1].params == ClassParams()
```

### Comparing `ooresults-0.2.2/tests/repo/test_clubs.py` & `ooresults-0.2.3/tests/repo/test_clubs.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/repo/test_competitors.py` & `ooresults-0.2.3/tests/repo/test_competitors.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,16 +106,16 @@
 
 def test_get_competitors_after_adding_one_competitor(db, competitor_1_id, club_id):
     c = list(db.get_competitors())
     assert len(c) == 1
     assert c[0].id == competitor_1_id
     assert c[0].first_name == "Jogi"
     assert c[0].last_name == "Löw"
-    assert c[0].club_id == None
-    assert c[0].club_name == None
+    assert c[0].club_id is None
+    assert c[0].club_name is None
     assert c[0].gender == "M"
     assert c[0].year is None
     assert c[0].chip == ""
 
 
 def test_get_competitors_after_adding_two_competitors(
     db, competitor_1_id, competitor_2_id, club_id
@@ -123,16 +123,16 @@
     c = list(db.get_competitors())
     assert len(c) == 2
     assert c[0].id != c[1].id
 
     assert c[0].id == competitor_1_id
     assert c[0].first_name == "Jogi"
     assert c[0].last_name == "Löw"
-    assert c[0].club_id == None
-    assert c[0].club_name == None
+    assert c[0].club_id is None
+    assert c[0].club_name is None
     assert c[0].gender == "M"
     assert c[0].year is None
     assert c[0].chip == ""
     assert c[1].id == competitor_2_id
     assert c[1].first_name == "Angela"
     assert c[1].last_name == "Merkel"
     assert c[1].club_id == club_id
@@ -144,15 +144,15 @@
 
 def test_get_first_added_competitor(db, competitor_1_id, competitor_2_id, club_id):
     c = list(db.get_competitor(id=competitor_1_id))
     assert len(c) == 1
     assert c[0].id == competitor_1_id
     assert c[0].first_name == "Jogi"
     assert c[0].last_name == "Löw"
-    assert c[0].club_id == None
+    assert c[0].club_id is None
     assert c[0].gender == "M"
     assert c[0].year is None
     assert c[0].chip == ""
 
 
 def test_get_last_added_competitor(db, competitor_1_id, competitor_2_id, club_id):
     c = list(db.get_competitor(id=competitor_2_id))
@@ -211,24 +211,24 @@
     c = list(db.get_competitors())
     assert len(c) == 2
     assert c[0].id != c[1].id
 
     assert c[0].id == competitor_2_id
     assert c[0].first_name == "Anton"
     assert c[0].last_name == "Berkel"
-    assert c[0].club_id == None
-    assert c[0].club_name == None
+    assert c[0].club_id is None
+    assert c[0].club_name is None
     assert c[0].gender == "M"
     assert c[0].year == 1958
     assert c[0].chip == ""
     assert c[1].id == competitor_1_id
     assert c[1].first_name == "Jogi"
     assert c[1].last_name == "Löw"
-    assert c[1].club_id == None
-    assert c[1].club_name == None
+    assert c[1].club_id is None
+    assert c[1].club_name is None
     assert c[1].gender == "M"
     assert c[1].year is None
     assert c[1].chip == ""
 
 
 def test_add_competitor_with_same_first_name(db, competitor_1_id, club_id):
     competitor_2_id = db.add_competitor(
@@ -242,24 +242,24 @@
     c = list(db.get_competitors())
     assert len(c) == 2
     assert c[0].id != c[1].id
 
     assert c[0].id == competitor_2_id
     assert c[0].first_name == "Jogi"
     assert c[0].last_name == "Berkel"
-    assert c[0].club_id == None
-    assert c[0].club_name == None
+    assert c[0].club_id is None
+    assert c[0].club_name is None
     assert c[0].gender == "M"
     assert c[0].year == 1958
     assert c[0].chip == ""
     assert c[1].id == competitor_1_id
     assert c[1].first_name == "Jogi"
     assert c[1].last_name == "Löw"
-    assert c[1].club_id == None
-    assert c[1].club_name == None
+    assert c[1].club_id is None
+    assert c[1].club_name is None
     assert c[1].gender == "M"
     assert c[1].year is None
     assert c[1].chip == ""
 
 
 def test_add_competitor_with_same_last_name(db, competitor_1_id, club_id):
     competitor_2_id = db.add_competitor(
@@ -273,24 +273,24 @@
     c = list(db.get_competitors())
     assert len(c) == 2
     assert c[0].id != c[1].id
 
     assert c[0].id == competitor_1_id
     assert c[0].first_name == "Jogi"
     assert c[0].last_name == "Löw"
-    assert c[0].club_id == None
-    assert c[0].club_name == None
+    assert c[0].club_id is None
+    assert c[0].club_name is None
     assert c[0].gender == "M"
     assert c[0].year is None
     assert c[0].chip == ""
     assert c[1].id == competitor_2_id
     assert c[1].first_name == "Norbert"
     assert c[1].last_name == "Löw"
-    assert c[1].club_id == None
-    assert c[1].club_name == None
+    assert c[1].club_id is None
+    assert c[1].club_name is None
     assert c[1].gender == "M"
     assert c[1].year == 1958
     assert c[1].chip == ""
 
 
 def test_delete_first_added_competitor(db, competitor_1_id, competitor_2_id, club_id):
     db.delete_competitor(id=competitor_1_id)
@@ -309,16 +309,16 @@
 def test_delete_last_added_competitor(db, competitor_1_id, competitor_2_id, club_id):
     db.delete_competitor(id=competitor_2_id)
     c = list(db.get_competitors())
     assert len(c) == 1
     assert c[0].id == competitor_1_id
     assert c[0].first_name == "Jogi"
     assert c[0].last_name == "Löw"
-    assert c[0].club_id == None
-    assert c[0].club_name == None
+    assert c[0].club_id is None
+    assert c[0].club_name is None
     assert c[0].gender == "M"
     assert c[0].year is None
     assert c[0].chip == ""
 
 
 def test_add_existing_name_raises_exception(db, competitor_1_id):
     with pytest.raises(repo.ConstraintError, match="Competitor already exist"):
@@ -361,16 +361,16 @@
 def test_delete_competitor_with_unknown_id_do_not_change_anything(db, competitor_1_id):
     db.delete_competitor(id=competitor_1_id + 1)
     c = list(db.get_competitors())
     assert len(c) == 1
     assert c[0].id == competitor_1_id
     assert c[0].first_name == "Jogi"
     assert c[0].last_name == "Löw"
-    assert c[0].club_id == None
-    assert c[0].club_name == None
+    assert c[0].club_id is None
+    assert c[0].club_name is None
     assert c[0].gender == "M"
     assert c[0].year is None
     assert c[0].chip == ""
 
 
 def test_delete_competitor_used_in_entry_raises_exception(
     db, entry_id, competitor_1_id
```

### Comparing `ooresults-0.2.2/tests/repo/test_courses.py` & `ooresults-0.2.3/tests/repo/test_courses.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,16 +93,16 @@
     assert c[0].id == course_1_id
     assert c[0].name == "Course 1"
     assert c[0].length == 4500
     assert c[0].climb == 90
     assert c[0].controls == ["101", "102", "103"]
     assert c[1].id == course_2_id
     assert c[1].name == "Course 2"
-    assert c[1].length == None
-    assert c[1].climb == None
+    assert c[1].length is None
+    assert c[1].climb is None
     assert c[1].controls == []
 
 
 def test_get_first_added_course(db, course_1_id, course_2_id):
     c = list(db.get_course(id=course_1_id))
     assert len(c) == 1
     assert c[0].id == course_1_id
@@ -113,31 +113,31 @@
 
 
 def test_get_last_added_course(db, course_1_id, course_2_id):
     c = list(db.get_course(id=course_2_id))
     assert len(c) == 1
     assert c[0].id == course_2_id
     assert c[0].name == "Course 2"
-    assert c[0].length == None
-    assert c[0].climb == None
+    assert c[0].length is None
+    assert c[0].climb is None
     assert c[0].controls == []
 
 
 def test_update_first_added_course(db, event_id, course_1_id, course_2_id):
     db.update_course(
         id=course_1_id, name="Course 3", length=3900, climb=150, controls=["101"]
     )
     c = list(db.get_courses(event_id=event_id))
     assert len(c) == 2
     assert c[0].id != c[1].id
 
     assert c[0].id == course_2_id
     assert c[0].name == "Course 2"
-    assert c[0].length == None
-    assert c[0].climb == None
+    assert c[0].length is None
+    assert c[0].climb is None
     assert c[0].controls == []
     assert c[1].id == course_1_id
     assert c[1].name == "Course 3"
     assert c[1].length == 3900
     assert c[1].climb == 150
     assert c[1].controls == ["101"]
 
@@ -158,26 +158,26 @@
     assert c[0].name == "Course 1"
     assert c[0].length == 4500
     assert c[0].climb == 90
     assert c[0].controls == ["101", "102", "103"]
     assert c[1].id == course_2_id
     assert c[1].name == "Course 3"
     assert c[1].length == 5100
-    assert c[1].climb == None
+    assert c[1].climb is None
     assert c[1].controls == ["301", "302", "303"]
 
 
 def test_delete_first_added_course(db, event_id, course_1_id, course_2_id):
     db.delete_course(id=course_1_id)
     c = list(db.get_courses(event_id=event_id))
     assert len(c) == 1
     assert c[0].id == course_2_id
     assert c[0].name == "Course 2"
-    assert c[0].length == None
-    assert c[0].climb == None
+    assert c[0].length is None
+    assert c[0].climb is None
     assert c[0].controls == []
 
 
 def test_delete_last_added_course(db, event_id, course_1_id, course_2_id):
     db.delete_course(id=course_2_id)
     c = list(db.get_courses(event_id=event_id))
     assert len(c) == 1
```

### Comparing `ooresults-0.2.2/tests/repo/test_entries.py` & `ooresults-0.2.3/tests/repo/test_entries.py`

 * *Files 1% similar despite different names*

```diff
@@ -718,20 +718,26 @@
     assert len(classes) == 2
     assert classes[0].id != classes[1].id
 
     assert classes[0].name == "Class 1"
     assert classes[0].short_name is None
     assert classes[0].course_id is None
     assert classes[0].course is None
+    assert classes[0].course_length is None
+    assert classes[0].course_climb is None
+    assert classes[0].number_of_controls is None
     assert classes[0].params == ClassParams()
 
     assert classes[1].name == "Class 2"
     assert classes[1].short_name is None
     assert classes[1].course_id is None
     assert classes[1].course is None
+    assert classes[1].course_length is None
+    assert classes[1].course_climb is None
+    assert classes[1].number_of_controls is None
     assert classes[1].params == ClassParams()
 
     clubs = list(db.get_clubs())
     assert len(clubs) == 1
 
     assert clubs[0].name == "OL Bundestag"
```

### Comparing `ooresults-0.2.2/tests/repo/test_events.py` & `ooresults-0.2.3/tests/repo/test_events.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/repo/test_settings.py` & `ooresults-0.2.3/tests/repo/test_settings.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/test_compute_result_net.py` & `ooresults-0.2.3/tests/test_compute_result_net.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/test_compute_result_score.py` & `ooresults-0.2.3/tests/test_compute_result_score.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/test_compute_result_standard.py` & `ooresults-0.2.3/tests/test_compute_result_standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,35 +428,35 @@
     )
     class_params = ClassParams(
         otype=otype,
         time_limit=time_limit,
     )
 
     result.compute_result(controls=controls, class_params=class_params)
-    assert result.start_time == None
-    assert result.punched_start_time == None
+    assert result.start_time is None
+    assert result.punched_start_time is None
     assert result.finish_time == f1
     assert result.punched_finish_time == f1
-    assert result.time == None
+    assert result.time is None
     assert result.status == ResultStatus.DISQUALIFIED
     assert len(result.split_times) == 3
     assert result.split_times[0] == SplitTime(
         control_code="101", punch_time=c1, time=None, status="OK"
     )
     assert result.split_times[1] == SplitTime(
         control_code="102", punch_time=c2, time=None, status="OK"
     )
     assert result.split_times[2] == SplitTime(
         control_code="103", punch_time=c3, time=None, status="OK"
     )
     if otype == "score":
         assert len(result.extensions) == 3
         assert result.extensions["score_controls"] == 3
-        assert result.extensions["score_overtime"] == None
-        assert result.extensions["score"] == None
+        assert result.extensions["score_overtime"] is None
+        assert result.extensions["score"] is None
 
 
 @pytest.mark.parametrize("otype", ["standard", "net", "score"])
 def test_given_no_controls_and_status_ok_when_compute_result_then_result_is_not_changed(
     otype,
 ):
     time_limit = 60 if otype == "score" else None
@@ -541,35 +541,35 @@
     )
     class_params = ClassParams(
         otype=otype,
         time_limit=time_limit,
     )
 
     result.compute_result(controls=controls, class_params=class_params)
-    assert result.start_time == None
-    assert result.punched_start_time == None
+    assert result.start_time is None
+    assert result.punched_start_time is None
     assert result.finish_time == f1
     assert result.punched_finish_time == f1
-    assert result.time == None
+    assert result.time is None
     assert result.status == ResultStatus.MISSING_PUNCH
     assert len(result.split_times) == 3
     assert result.split_times[0] == SplitTime(
         control_code="101", punch_time=c1, time=None, status="OK"
     )
     assert result.split_times[1] == SplitTime(
         control_code="102", punch_time=c2, time=None, status="OK"
     )
     assert result.split_times[2] == SplitTime(
         control_code="103", punch_time=c3, time=None, status="OK"
     )
     if otype == "score":
         assert len(result.extensions) == 3
         assert result.extensions["score_controls"] == 3
-        assert result.extensions["score_overtime"] == None
-        assert result.extensions["score"] == None
+        assert result.extensions["score_overtime"] is None
+        assert result.extensions["score"] is None
 
 
 @pytest.mark.parametrize("otype", ["standard", "net", "score"])
 def test_compute_result_status_no_finish_time(otype):
     time_limit = 60 if otype == "score" else None
     s1 = datetime(2015, 1, 1, 12, 38, 59, tzinfo=timezone.utc)
     c1 = datetime(2015, 1, 1, 12, 39, 1, tzinfo=timezone.utc)
@@ -592,17 +592,17 @@
         otype=otype,
         time_limit=time_limit,
     )
 
     result.compute_result(controls=controls, class_params=class_params)
     assert result.start_time == s1
     assert result.punched_start_time == s1
-    assert result.finish_time == None
-    assert result.punched_finish_time == None
-    assert result.time == None
+    assert result.finish_time is None
+    assert result.punched_finish_time is None
+    assert result.time is None
     assert result.status == ResultStatus.DID_NOT_FINISH
     assert len(result.split_times) == 3
     assert result.split_times[0] == SplitTime(
         control_code="101", punch_time=c1, time=t(s1, c1), status="OK"
     )
     assert result.split_times[1] == SplitTime(
         control_code="102", punch_time=c2, time=t(s1, c2), status="OK"
@@ -628,19 +628,19 @@
     )
     class_params = ClassParams(
         otype=otype,
         time_limit=time_limit,
     )
 
     result.compute_result(controls=controls, class_params=class_params)
-    assert result.start_time == None
-    assert result.punched_start_time == None
-    assert result.finish_time == None
-    assert result.punched_finish_time == None
-    assert result.time == None
+    assert result.start_time is None
+    assert result.punched_start_time is None
+    assert result.finish_time is None
+    assert result.punched_finish_time is None
+    assert result.time is None
     assert result.status == ResultStatus.DID_NOT_START
     assert len(result.split_times) == 2
     assert result.split_times[0] == SplitTime(
         control_code="101", punch_time=None, time=None, status="Missing"
     )
     assert result.split_times[1] == SplitTime(
         control_code="102", punch_time=None, time=None, status="Missing"
@@ -668,19 +668,19 @@
     )
     class_params = ClassParams(
         otype=otype,
         time_limit=time_limit,
     )
 
     result.compute_result(controls=controls, class_params=class_params)
-    assert result.start_time == None
-    assert result.punched_start_time == None
-    assert result.finish_time == None
-    assert result.punched_finish_time == None
-    assert result.time == None
+    assert result.start_time is None
+    assert result.punched_start_time is None
+    assert result.finish_time is None
+    assert result.punched_finish_time is None
+    assert result.time is None
     assert result.status == ResultStatus.INACTIVE
     assert len(result.split_times) == 0
     if otype == "score":
         assert len(result.extensions) == 3
         assert result.extensions["score_controls"] == 0
         assert result.extensions["score_overtime"] is None
         assert result.extensions["score"] is None
@@ -970,15 +970,15 @@
         using_start_control="if_punched",
         mass_start=p1,
         time_limit=time_limit,
     )
 
     result.compute_result(controls=controls, class_params=class_params, start_time=p1)
     assert result.start_time == p1
-    assert result.punched_start_time == None
+    assert result.punched_start_time is None
     assert result.finish_time == f1
     assert result.punched_finish_time == f1
     assert result.time == int((f1 - p1).total_seconds())
     assert result.status == ResultStatus.OK
     assert len(result.split_times) == 1
     assert result.split_times[0] == SplitTime(
         control_code="101", punch_time=c1, time=t(p1, c1), status="OK"
```

### Comparing `ooresults-0.2.2/tests/test_configuration.py` & `ooresults-0.2.3/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/test_globals.py` & `ooresults-0.2.3/tests/test_globals.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/test_handicap.py` & `ooresults-0.2.3/tests/test_handicap.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.2/tests/test_ranking.py` & `ooresults-0.2.3/tests/test_ranking.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-from ooresults.handler import results
+from ooresults.handler import build_results
 from ooresults.repo import result_type
 from ooresults.repo.result_type import ResultStatus
 from ooresults.repo.class_params import ClassParams
 
 
 class Class_:
     def __init__(self, name: str, params: ClassParams):
         self.name = name
         self.params = params
 
 
 def test_ranking_with_one_class():
     class_a = Class_(name="Bahn A - Lang", params=ClassParams())
-    data = results.build_results(
+    data = build_results.build_results(
         classes=[
             class_a,
         ],
         results=[
             {
                 "first_name": "Angela",
                 "last_name": "Merkel",
@@ -93,27 +93,29 @@
                     "gender": "",
                     "year": "",
                     "not_competing": False,
                     "result": result_type.PersonRaceResult(
                         status=ResultStatus.OK, time=2001
                     ),
                     "rank": 1,
+                    "time_behind": 0,
                     "points": 1.0,
                 },
                 {
                     "first_name": "Angela",
                     "last_name": "Merkel",
                     "class_": "Bahn A - Lang",
                     "gender": "",
                     "year": "",
                     "not_competing": False,
                     "result": result_type.PersonRaceResult(
                         status=ResultStatus.OK, time=9876
                     ),
                     "rank": 2,
+                    "time_behind": 9876 - 2001,
                     "points": 2001 / 9876,
                 },
                 {
                     "first_name": "Birgit",
                     "last_name": "Merkel",
                     "class_": "Bahn A - Lang",
                     "gender": "",
@@ -138,17 +140,142 @@
                     "rank": None,
                 },
             ],
         )
     ]
 
 
+def test_ranking_with_two_classes():
+    class_a = Class_(name="Bahn A - Lang", params=ClassParams())
+    class_b = Class_(name="Bahn B - Mittel", params=ClassParams())
+    data = build_results.build_results(
+        classes=[
+            class_a,
+            class_b,
+        ],
+        results=[
+            {
+                "first_name": "Angela",
+                "last_name": "Merkel",
+                "gender": "",
+                "year": "",
+                "not_competing": False,
+                "class_": "Bahn A - Lang",
+                "result": result_type.PersonRaceResult(
+                    status=ResultStatus.OK, time=9876
+                ),
+            },
+            {
+                "first_name": "Claudia",
+                "last_name": "Merkel",
+                "gender": "",
+                "year": "",
+                "not_competing": False,
+                "class_": "Bahn B - Mittel",
+                "result": result_type.PersonRaceResult(
+                    status=ResultStatus.OK, time=2001
+                ),
+            },
+            {
+                "first_name": "Birgit",
+                "last_name": "Merkel",
+                "gender": "",
+                "year": "",
+                "not_competing": False,
+                "class_": "Bahn B - Mittel",
+                "result": result_type.PersonRaceResult(
+                    status=ResultStatus.OK, time=2113
+                ),
+            },
+            {
+                "first_name": "Birgit",
+                "last_name": "Derkel",
+                "gender": "",
+                "year": "",
+                "not_competing": False,
+                "class_": "Bahn A - Lang",
+                "result": result_type.PersonRaceResult(
+                    status=ResultStatus.OK, time=3333
+                ),
+            },
+        ],
+    )
+    assert data == [
+        (
+            class_a,
+            [
+                {
+                    "first_name": "Birgit",
+                    "last_name": "Derkel",
+                    "class_": "Bahn A - Lang",
+                    "gender": "",
+                    "year": "",
+                    "not_competing": False,
+                    "result": result_type.PersonRaceResult(
+                        status=ResultStatus.OK, time=3333
+                    ),
+                    "rank": 1,
+                    "time_behind": 0,
+                    "points": 1.0,
+                },
+                {
+                    "first_name": "Angela",
+                    "last_name": "Merkel",
+                    "class_": "Bahn A - Lang",
+                    "gender": "",
+                    "year": "",
+                    "not_competing": False,
+                    "result": result_type.PersonRaceResult(
+                        status=ResultStatus.OK, time=9876
+                    ),
+                    "rank": 2,
+                    "time_behind": 9876 - 3333,
+                    "points": 3333 / 9876,
+                },
+            ],
+        ),
+        (
+            class_b,
+            [
+                {
+                    "first_name": "Claudia",
+                    "last_name": "Merkel",
+                    "class_": "Bahn B - Mittel",
+                    "gender": "",
+                    "year": "",
+                    "not_competing": False,
+                    "result": result_type.PersonRaceResult(
+                        status=ResultStatus.OK, time=2001
+                    ),
+                    "rank": 1,
+                    "time_behind": 0,
+                    "points": 1.0,
+                },
+                {
+                    "first_name": "Birgit",
+                    "last_name": "Merkel",
+                    "class_": "Bahn B - Mittel",
+                    "gender": "",
+                    "year": "",
+                    "not_competing": False,
+                    "result": result_type.PersonRaceResult(
+                        status=ResultStatus.OK, time=2113
+                    ),
+                    "rank": 2,
+                    "time_behind": 2113 - 2001,
+                    "points": 2001 / 2113,
+                },
+            ],
+        ),
+    ]
+
+
 def test_ranking_with_two_winners():
     class_a = Class_(name="Bahn A - Lang", params=ClassParams())
-    data = results.build_results(
+    data = build_results.build_results(
         classes=[
             class_a,
         ],
         results=[
             {
                 "first_name": "Angela",
                 "last_name": "Merkel",
@@ -195,27 +322,29 @@
                     "gender": "",
                     "year": "",
                     "not_competing": False,
                     "result": result_type.PersonRaceResult(
                         status=ResultStatus.OK, time=2001
                     ),
                     "rank": 1,
+                    "time_behind": 0,
                     "points": 1.0,
                 },
                 {
                     "first_name": "Claudia",
                     "last_name": "Merkel",
                     "class_": "Bahn A - Lang",
                     "gender": "",
                     "year": "",
                     "not_competing": False,
                     "result": result_type.PersonRaceResult(
                         status=ResultStatus.OK, time=2001
                     ),
                     "rank": 1,
+                    "time_behind": 0,
                     "points": 1.0,
                 },
                 {
                     "first_name": "Angela",
                     "last_name": "Merkel",
                     "class_": "Bahn A - Lang",
                     "gender": "",
@@ -230,15 +359,15 @@
             ],
         )
     ]
 
 
 def test_ranking_entries_with_same_time_are_orderd_by_name():
     class_a = Class_(name="Bahn A - Lang", params=ClassParams())
-    data = results.build_results(
+    data = build_results.build_results(
         classes=[
             class_a,
         ],
         results=[
             {
                 "first_name": "Angela",
                 "last_name": "Merkel",
@@ -281,15 +410,14 @@
                 "class_": "Bahn A - Lang",
                 "result": result_type.PersonRaceResult(
                     status=ResultStatus.OK, time=2001
                 ),
             },
         ],
     )
-    print(data)
     assert data == [
         (
             class_a,
             [
                 {
                     "first_name": "Birgit",
                     "last_name": "Derkel",
@@ -297,63 +425,67 @@
                     "gender": "",
                     "year": "",
                     "not_competing": False,
                     "result": result_type.PersonRaceResult(
                         status=ResultStatus.OK, time=2001
                     ),
                     "rank": 1,
+                    "time_behind": 0,
                     "points": 1.0,
                 },
                 {
                     "first_name": "Angela",
                     "last_name": "Merkel",
                     "class_": "Bahn A - Lang",
                     "gender": "",
                     "year": "",
                     "not_competing": False,
                     "result": result_type.PersonRaceResult(
                         status=ResultStatus.OK, time=2001
                     ),
                     "rank": 1,
+                    "time_behind": 0,
                     "points": 1.0,
                 },
                 {
                     "first_name": "Birgit",
                     "last_name": "Merkel",
                     "class_": "Bahn A - Lang",
                     "gender": "",
                     "year": "",
                     "not_competing": False,
                     "result": result_type.PersonRaceResult(
                         status=ResultStatus.OK, time=2001
                     ),
                     "rank": 1,
+                    "time_behind": 0,
                     "points": 1.0,
                 },
                 {
                     "first_name": "Claudia",
                     "last_name": "Merkel",
                     "class_": "Bahn A - Lang",
                     "gender": "",
                     "year": "",
                     "not_competing": False,
                     "result": result_type.PersonRaceResult(
                         status=ResultStatus.OK, time=2001
                     ),
                     "rank": 1,
+                    "time_behind": 0,
                     "points": 1.0,
                 },
             ],
         )
     ]
 
 
 def test_ranking_entries_with_same_time_are_orderd_by_name_2():
     class_a = Class_(name="Bahn A - Lang", params=ClassParams(otype="score"))
-    data = results.build_results(
+    data = build_results.build_results(
         classes=[
             class_a,
         ],
         results=[
             {
                 "first_name": "Claudia",
                 "last_name": "Merkel",
@@ -455,15 +587,15 @@
             ],
         )
     ]
 
 
 def test_ranking_with_not_competing_runners():
     class_a = Class_(name="Bahn A - Lang", params=ClassParams())
-    data = results.build_results(
+    data = build_results.build_results(
         classes=[
             class_a,
         ],
         results=[
             {
                 "first_name": "Angela",
                 "last_name": "Merkel",
@@ -506,15 +638,14 @@
                 "class_": "Bahn A - Lang",
                 "result": result_type.PersonRaceResult(
                     status=ResultStatus.DID_NOT_START
                 ),
             },
         ],
     )
-    print(data[0])
     assert data == [
         (
             class_a,
             [
                 {
                     "first_name": "Angela",
                     "last_name": "Merkel",
@@ -522,14 +653,15 @@
                     "gender": "",
                     "year": "",
                     "not_competing": False,
                     "result": result_type.PersonRaceResult(
                         status=ResultStatus.OK, time=9876
                     ),
                     "rank": 1,
+                    "time_behind": 0,
                     "points": 2001 / 2001,
                 },
                 {
                     "first_name": "Claudia",
                     "last_name": "Merkel",
                     "class_": "Bahn A - Lang",
                     "gender": "",
```

### Comparing `ooresults-0.2.2/tests/test_series.py` & `ooresults-0.2.3/tests/test_series.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 from decimal import Decimal
 
 import pytest
 
-from ooresults.handler import series
+from ooresults.handler import build_results
+from ooresults.handler import model
 from ooresults.repo import result_type
 from ooresults.repo import series_type
 
 
 class Event:
     def __init__(self, name: str, date: str, series: bool):
         self.name = name
@@ -61,41 +62,41 @@
 @pytest.fixture
 def event_5():
     return Event(name="ev5", date="2021-02-19", series="Run 5")
 
 
 def test_use_only_events_in_series(event_1, event_2, event_3):
     events = [event_1, event_2, event_3]
-    data = series.create_event_list(events=events)
+    data = model.create_event_list(events=events)
     assert data == [event_3, event_1]
 
 
 def test_sort_events_by_date(event_1, event_3, event_5):
     events = [event_1, event_3, event_5]
-    data = series.create_event_list(events=events)
+    data = model.create_event_list(events=events)
     assert data == [event_5, event_3, event_1]
 
     events = [event_1, event_3, event_5]
-    data = series.create_event_list(events=events)
+    data = model.create_event_list(events=events)
     assert data == [event_5, event_3, event_1]
 
 
 def test_sort_events_by_name_if_dates_are_equal(event_3, event_4):
     events = [event_3, event_4]
-    data = series.create_event_list(events=events)
+    data = model.create_event_list(events=events)
     assert data == [event_3, event_4]
 
     events = [event_4, event_3]
-    data = series.create_event_list(events=events)
+    data = model.create_event_list(events=events)
     assert data == [event_3, event_4]
 
 
 def test_no_results():
     class_a = Class_(name="Bahn A - Lang")
-    data = series.build_total_results(
+    data = build_results.build_total_results(
         settings=series_type.Settings(),
         list_of_results=[
             [
                 (
                     class_a,
                     [
                         {
@@ -128,15 +129,15 @@
         ],
     )
     assert data == [(class_a.name, [])]
 
 
 def test_best_3_of_1_race():
     class_a = Class_(name="Bahn A - Lang")
-    data = series.build_total_results(
+    data = build_results.build_total_results(
         settings=series_type.Settings(
             nr_of_best_results=3,
         ),
         list_of_results=[
             [
                 (
                     class_a,
@@ -173,15 +174,15 @@
             ],
         ),
     ]
 
 
 def test_best_3_of_2_races():
     class_a = Class_(name="Bahn A - Lang")
-    data = series.build_total_results(
+    data = build_results.build_total_results(
         settings=series_type.Settings(
             nr_of_best_results=3,
         ),
         list_of_results=[
             [
                 (
                     class_a,
@@ -234,15 +235,15 @@
             ],
         ),
     ]
 
 
 def test_best_3_of_4_races():
     class_a = Class_(name="Bahn A - Lang")
-    data = series.build_total_results(
+    data = build_results.build_total_results(
         settings=series_type.Settings(
             nr_of_best_results=3,
         ),
         list_of_results=[
             [
                 (
                     class_a,
@@ -332,15 +333,15 @@
             ],
         ),
     ]
 
 
 def test_bonus_1_race():
     class_a = Class_(name="Bahn A - Lang")
-    data = series.build_total_results(
+    data = build_results.build_total_results(
         settings=series_type.Settings(),
         list_of_results=[
             [
                 (
                     class_a,
                     [
                         {
@@ -382,15 +383,15 @@
             ],
         ),
     ]
 
 
 def test_bonus_2_races():
     class_a = Class_(name="Bahn A - Lang")
-    data = series.build_total_results(
+    data = build_results.build_total_results(
         settings=series_type.Settings(),
         list_of_results=[
             [
                 (
                     class_a,
                     [
                         {
@@ -449,15 +450,15 @@
             ],
         ),
     ]
 
 
 def test_bonus_4_races():
     class_a = Class_(name="Bahn A - Lang")
-    data = series.build_total_results(
+    data = build_results.build_total_results(
         settings=series_type.Settings(
             nr_of_best_results=3,
         ),
         list_of_results=[
             [
                 (
                     class_a,
@@ -557,15 +558,15 @@
             ],
         ),
     ]
 
 
 def test_ranking_1():
     class_a = Class_(name="Bahn A - Lang")
-    data = series.build_total_results(
+    data = build_results.build_total_results(
         settings=series_type.Settings(),
         list_of_results=[
             [
                 (
                     class_a,
                     [
                         {
@@ -619,15 +620,15 @@
             ],
         ),
     ]
 
 
 def test_ranking_2():
     class_a = Class_(name="Bahn A - Lang")
-    data = series.build_total_results(
+    data = build_results.build_total_results(
         settings=series_type.Settings(),
         list_of_results=[
             [
                 (
                     class_a,
                     [
                         {
@@ -688,15 +689,15 @@
             ],
         ),
     ]
 
 
 def test_ranking_3():
     class_a = Class_(name="Bahn A - Lang")
-    data = series.build_total_results(
+    data = build_results.build_total_results(
         settings=series_type.Settings(),
         list_of_results=[
             [
                 (
                     class_a,
                     [
                         {
@@ -766,15 +767,15 @@
             ],
         ),
     ]
 
 
 def test_if_sum_is_0_then_rank_is_None():
     class_a = Class_(name="Bahn A - Lang")
-    data = series.build_total_results(
+    data = build_results.build_total_results(
         settings=series_type.Settings(),
         list_of_results=[
             [
                 (
                     class_a,
                     [
                         {
```

### Comparing `ooresults-0.2.2/tests/test_user.py` & `ooresults-0.2.3/tests/test_user.py`

 * *Files identical despite different names*

