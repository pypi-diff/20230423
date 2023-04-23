# Comparing `tmp/amulet-map-editor-0.9.5.tar.gz` & `tmp/amulet-map-editor-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\a\Amulet-Map-Editor\Amulet-Map-Editor\dist\tmpbt7txmv6\amulet-map-editor-0.9.5.tar", last modified: Sun Jun 19 18:36:06 2022, max compression
+gzip compressed data, was "D:\a\Amulet-Map-Editor\Amulet-Map-Editor\dist\tmpov35s0e2\amulet-map-editor-0.9.6.tar", last modified: Tue Jun 21 09:03:47 2022, max compression
```

## Comparing `amulet-map-editor-0.9.5.tar` & `amulet-map-editor-0.9.6.tar`

### file list

```diff
@@ -1,655 +1,655 @@
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/
--rw-rw-rw-   0        0        0      227 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/MANIFEST.in
--rw-rw-rw-   0        0        0      429 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/
--rw-rw-rw-   0        0        0      202 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/__init__.py
--rw-rw-rw-   0        0        0     1293 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/__pyinstaller/
--rw-rw-rw-   0        0        0       43 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      277 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/__pyinstaller/hook-amulet_map_editor.py
--rw-rw-rw-   0        0        0      518 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/_version.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/
--rw-rw-rw-   0        0        0       26 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/__init__.py
--rw-rw-rw-   0        0        0     1147 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/config.py
--rw-rw-rw-   0        0        0      345 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/datatypes.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/framework/
--rw-rw-rw-   0        0        0       61 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/framework/__init__.py
--rw-rw-rw-   0        0        0     8340 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/framework/amulet_ui.py
--rw-rw-rw-   0        0        0      660 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/framework/app.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/framework/pages/
--rw-rw-rw-   0        0        0      111 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/framework/pages/__init__.py
--rw-rw-rw-   0        0        0      264 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/framework/pages/base_page.py
--rw-rw-rw-   0        0        0     3004 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/framework/pages/main_menu.py
--rw-rw-rw-   0        0        0     6402 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/framework/pages/world_page.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/framework/programs/
--rw-rw-rw-   0        0        0       80 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/framework/programs/__init__.py
--rw-rw-rw-   0        0        0     1557 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/framework/programs/about_program.py
--rw-rw-rw-   0        0        0      705 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/framework/programs/base_program.py
--rw-rw-rw-   0        0        0     4869 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/framework/update_check.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/
--rw-rw-rw-   0        0        0     2295 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/
--rw-rw-rw-   0        0        0     5695 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/accessible.png
--rw-rw-rw-   0        0        0     3210 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/adjustments.png
--rw-rw-rw-   0        0        0     4924 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/alert_circle.png
--rw-rw-rw-   0        0        0     3398 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/alert_triangle.png
--rw-rw-rw-   0        0        0     1207 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/align_center.png
--rw-rw-rw-   0        0        0     1184 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/align_justified.png
--rw-rw-rw-   0        0        0     1201 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/align_left.png
--rw-rw-rw-   0        0        0     1207 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/align_right.png
--rw-rw-rw-   0        0        0     3781 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/anchor.png
--rw-rw-rw-   0        0        0     6426 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/aperture.png
--rw-rw-rw-   0        0        0     2280 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/apps.png
--rw-rw-rw-   0        0        0     2655 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/archive.png
--rw-rw-rw-   0        0        0     2242 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_back.png
--rw-rw-rw-   0        0        0     2315 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_back_up.png
--rw-rw-rw-   0        0        0     1543 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_bar_down.png
--rw-rw-rw-   0        0        0     1756 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_bar_left.png
--rw-rw-rw-   0        0        0     1652 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_bar_right.png
--rw-rw-rw-   0        0        0     1537 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_bar_up.png
--rw-rw-rw-   0        0        0     1470 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_down.png
--rw-rw-rw-   0        0        0     5351 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_down_circle.png
--rw-rw-rw-   0        0        0     1323 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_down_left.png
--rw-rw-rw-   0        0        0     5196 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_down_left_circle.png
--rw-rw-rw-   0        0        0     1286 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_down_right.png
--rw-rw-rw-   0        0        0     5187 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_down_right_circle.png
--rw-rw-rw-   0        0        0     2127 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_forward.png
--rw-rw-rw-   0        0        0     2192 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_forward_up.png
--rw-rw-rw-   0        0        0     1233 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_left.png
--rw-rw-rw-   0        0        0     5185 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_left_circle.png
--rw-rw-rw-   0        0        0     1317 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_down.png
--rw-rw-rw-   0        0        0     1146 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_left.png
--rw-rw-rw-   0        0        0     1054 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_right.png
--rw-rw-rw-   0        0        0     1300 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_up.png
--rw-rw-rw-   0        0        0     1135 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_right.png
--rw-rw-rw-   0        0        0     5108 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_right_circle.png
--rw-rw-rw-   0        0        0     1398 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_up.png
--rw-rw-rw-   0        0        0     5368 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_up_circle.png
--rw-rw-rw-   0        0        0     1328 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_up_left.png
--rw-rw-rw-   0        0        0     5186 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_up_left_circle.png
--rw-rw-rw-   0        0        0     1329 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_up_right.png
--rw-rw-rw-   0        0        0     5188 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_up_right_circle.png
--rw-rw-rw-   0        0        0     1774 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrows_diagonal.png
--rw-rw-rw-   0        0        0     1751 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrows_diagonal_2.png
--rw-rw-rw-   0        0        0     1461 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrows_horizontal.png
--rw-rw-rw-   0        0        0     2792 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrows_maximize.png
--rw-rw-rw-   0        0        0     2746 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrows_minimize.png
--rw-rw-rw-   0        0        0     2179 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrows_sort.png
--rw-rw-rw-   0        0        0     1793 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrows_vertical.png
--rw-rw-rw-   0        0        0     2160 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/artboard.png
--rw-rw-rw-   0        0        0     5971 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/at.png
--rw-rw-rw-   0        0        0     5172 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/award.png
--rw-rw-rw-   0        0        0     2218 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/backspace.png
--rw-rw-rw-   0        0        0     2707 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/box.png
--rw-rw-rw-   0        0        0     3272 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/braces.png
--rw-rw-rw-   0        0        0     1386 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/brackets.png
--rw-rw-rw-   0        0        0     1020 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/caret_down.png
--rw-rw-rw-   0        0        0     1268 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/caret_left.png
--rw-rw-rw-   0        0        0     1245 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/caret_right.png
--rw-rw-rw-   0        0        0     1037 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/caret_up.png
--rw-rw-rw-   0        0        0     1132 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/check.png
--rw-rw-rw-   0        0        0     2598 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/checkbox.png
--rw-rw-rw-   0        0        0     1543 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/checks.png
--rw-rw-rw-   0        0        0     1062 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevron_down.png
--rw-rw-rw-   0        0        0      995 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevron_left.png
--rw-rw-rw-   0        0        0      952 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevron_right.png
--rw-rw-rw-   0        0        0     1001 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevron_up.png
--rw-rw-rw-   0        0        0     1627 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevrons_down.png
--rw-rw-rw-   0        0        0     1410 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevrons_left.png
--rw-rw-rw-   0        0        0     1302 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevrons_right.png
--rw-rw-rw-   0        0        0     1515 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevrons_up.png
--rw-rw-rw-   0        0        0     4478 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/circle.png
--rw-rw-rw-   0        0        0     5101 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/circle_check.png
--rw-rw-rw-   0        0        0     4738 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/circle_minus.png
--rw-rw-rw-   0        0        0     4975 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/circle_plus.png
--rw-rw-rw-   0        0        0     5221 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/circle_x.png
--rw-rw-rw-   0        0        0     3038 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/click.png
--rw-rw-rw-   0        0        0     2538 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/clipboard.png
--rw-rw-rw-   0        0        0     3280 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/clipboard_check.png
--rw-rw-rw-   0        0        0     3267 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/clipboard_list.png
--rw-rw-rw-   0        0        0     3445 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/clipboard_x.png
--rw-rw-rw-   0        0        0     4938 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/clock.png
--rw-rw-rw-   0        0        0     3766 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/cloud.png
--rw-rw-rw-   0        0        0     4512 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/cloud_download.png
--rw-rw-rw-   0        0        0     4632 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/cloud_upload.png
--rw-rw-rw-   0        0        0     2371 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/code.png
--rw-rw-rw-   0        0        0     2076 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/color_picker.png
--rw-rw-rw-   0        0        0     4107 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/color_swatch.png
--rw-rw-rw-   0        0        0     2358 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/command.png
--rw-rw-rw-   0        0        0     2731 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/copy.png
--rw-rw-rw-   0        0        0     5801 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/copyright.png
--rw-rw-rw-   0        0        0     1733 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_down_left.png
--rw-rw-rw-   0        0        0     1696 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_down_right.png
--rw-rw-rw-   0        0        0     1798 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_left_down.png
--rw-rw-rw-   0        0        0     1783 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_left_up.png
--rw-rw-rw-   0        0        0     1801 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_right_down.png
--rw-rw-rw-   0        0        0     1774 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_right_up.png
--rw-rw-rw-   0        0        0     1774 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_up_left.png
--rw-rw-rw-   0        0        0     1639 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_up_right.png
--rw-rw-rw-   0        0        0     1477 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/crop.png
--rw-rw-rw-   0        0        0     3425 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/cut.png
--rw-rw-rw-   0        0        0     4739 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/dashboard.png
--rw-rw-rw-   0        0        0     4530 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/database.png
--rw-rw-rw-   0        0        0     1646 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_desktop.png
--rw-rw-rw-   0        0        0     3025 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_floppy.png
--rw-rw-rw-   0        0        0     2580 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_gamepad.png
--rw-rw-rw-   0        0        0     1558 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_laptop.png
--rw-rw-rw-   0        0        0     1772 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_mobile.png
--rw-rw-rw-   0        0        0     1979 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_tablet.png
--rw-rw-rw-   0        0        0     2281 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_tv.png
--rw-rw-rw-   0        0        0     2493 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_watch.png
--rw-rw-rw-   0        0        0     1980 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/devices.png
--rw-rw-rw-   0        0        0     1364 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/direction.png
--rw-rw-rw-   0        0        0     1182 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/direction_horizontal.png
--rw-rw-rw-   0        0        0      948 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/dots.png
--rw-rw-rw-   0        0        0     4827 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/dots_circle_horizontal.png
--rw-rw-rw-   0        0        0     1563 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/dots_diagonal.png
--rw-rw-rw-   0        0        0     1563 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/dots_diagonal_2.png
--rw-rw-rw-   0        0        0     1601 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/dots_vertical.png
--rw-rw-rw-   0        0        0     2248 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/download.png
--rw-rw-rw-   0        0        0     3797 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/drag_drop.png
--rw-rw-rw-   0        0        0     2810 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/drag_drop_2.png
--rw-rw-rw-   0        0        0     3169 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/edit.png
--rw-rw-rw-   0        0        0     1975 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/eraser.png
--rw-rw-rw-   0        0        0     4115 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/exchange.png
--rw-rw-rw-   0        0        0     2649 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/external_link.png
--rw-rw-rw-   0        0        0     2136 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file.png
--rw-rw-rw-   0        0        0     2875 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_check.png
--rw-rw-rw-   0        0        0     3175 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_code.png
--rw-rw-rw-   0        0        0     3005 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_download.png
--rw-rw-rw-   0        0        0     2065 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_horizontal.png
--rw-rw-rw-   0        0        0     2878 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_invoice.png
--rw-rw-rw-   0        0        0     2450 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_minus.png
--rw-rw-rw-   0        0        0     3003 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_music.png
--rw-rw-rw-   0        0        0     2676 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_plus.png
--rw-rw-rw-   0        0        0     2335 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_shredder.png
--rw-rw-rw-   0        0        0     2965 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_text.png
--rw-rw-rw-   0        0        0     3042 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_x.png
--rw-rw-rw-   0        0        0     1969 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/filter.png
--rw-rw-rw-   0        0        0     3138 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/flag.png
--rw-rw-rw-   0        0        0     3368 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/flame.png
--rw-rw-rw-   0        0        0     2170 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/flask.png
--rw-rw-rw-   0        0        0     1852 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/flip_horizontal.png
--rw-rw-rw-   0        0        0     2407 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/flip_vertical.png
--rw-rw-rw-   0        0        0     2931 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/floppy_disk.png
--rw-rw-rw-   0        0        0     4886 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/focus.png
--rw-rw-rw-   0        0        0     4412 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/focus_2.png
--rw-rw-rw-   0        0        0     1998 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/folder.png
--rw-rw-rw-   0        0        0     2312 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/folder_minus.png
--rw-rw-rw-   0        0        0     2502 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/folder_plus.png
--rw-rw-rw-   0        0        0     2871 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/folder_x.png
--rw-rw-rw-   0        0        0     2819 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/folders.png
--rw-rw-rw-   0        0        0     4968 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/forbid.png
--rw-rw-rw-   0        0        0     4970 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/forbid_2.png
--rw-rw-rw-   0        0        0     1521 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/frame.png
--rw-rw-rw-   0        0        0     3231 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/friends.png
--rw-rw-rw-   0        0        0     3562 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/gift.png
--rw-rw-rw-   0        0        0     2900 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/git_branch.png
--rw-rw-rw-   0        0        0     1916 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/git_commit.png
--rw-rw-rw-   0        0        0     3512 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/git_compare.png
--rw-rw-rw-   0        0        0     2566 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/git_fork.png
--rw-rw-rw-   0        0        0     2789 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/git_merge.png
--rw-rw-rw-   0        0        0     2908 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/git_pull_request.png
--rw-rw-rw-   0        0        0     1924 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/grid.png
--rw-rw-rw-   0        0        0     2101 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/grid_dots.png
--rw-rw-rw-   0        0        0     1522 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/grip_horizontal.png
--rw-rw-rw-   0        0        0     1924 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/grip_vertical.png
--rw-rw-rw-   0        0        0     3118 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/hand_stop.png
--rw-rw-rw-   0        0        0     2221 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/hash.png
--rw-rw-rw-   0        0        0     5570 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/help.png
--rw-rw-rw-   0        0        0     3495 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/hexagon.png
--rw-rw-rw-   0        0        0     5131 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/history.png
--rw-rw-rw-   0        0        0     2712 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/home.png
--rw-rw-rw-   0        0        0     2363 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/home_2.png
--rw-rw-rw-   0        0        0     1745 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/indent_decrease.png
--rw-rw-rw-   0        0        0     1694 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/indent_increase.png
--rw-rw-rw-   0        0        0     3729 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/infinity.png
--rw-rw-rw-   0        0        0     5031 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/info_circle.png
--rw-rw-rw-   0        0        0     2571 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/info_square.png
--rw-rw-rw-   0        0        0     2794 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/keyboard.png
--rw-rw-rw-   0        0        0     3306 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/language.png
--rw-rw-rw-   0        0        0     3161 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layers_difference.png
--rw-rw-rw-   0        0        0     2959 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layers_intersect.png
--rw-rw-rw-   0        0        0     2716 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layers_subtract.png
--rw-rw-rw-   0        0        0     2572 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layers_union.png
--rw-rw-rw-   0        0        0     3445 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout.png
--rw-rw-rw-   0        0        0     2909 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_2.png
--rw-rw-rw-   0        0        0     1977 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_align_bottom.png
--rw-rw-rw-   0        0        0     2077 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_align_center.png
--rw-rw-rw-   0        0        0     2124 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_align_left.png
--rw-rw-rw-   0        0        0     1979 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_align_middle.png
--rw-rw-rw-   0        0        0     2158 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_align_right.png
--rw-rw-rw-   0        0        0     1962 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_align_top.png
--rw-rw-rw-   0        0        0     1924 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_bottombar.png
--rw-rw-rw-   0        0        0     2462 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_cards.png
--rw-rw-rw-   0        0        0     1958 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_columns.png
--rw-rw-rw-   0        0        0     2207 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_distribute_horizontal.png
--rw-rw-rw-   0        0        0     2287 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_distribute_vertical.png
--rw-rw-rw-   0        0        0     2845 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_list.png
--rw-rw-rw-   0        0        0     1925 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_navbar.png
--rw-rw-rw-   0        0        0     1924 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_rows.png
--rw-rw-rw-   0        0        0     1937 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_sidebar.png
--rw-rw-rw-   0        0        0     1972 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_sidebar_right.png
--rw-rw-rw-   0        0        0     2907 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/license.png
--rw-rw-rw-   0        0        0     2457 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/line_height.png
--rw-rw-rw-   0        0        0     3800 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/link.png
--rw-rw-rw-   0        0        0     1650 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/list.png
--rw-rw-rw-   0        0        0     2543 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/list_check.png
--rw-rw-rw-   0        0        0     3414 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/location.png
--rw-rw-rw-   0        0        0     3313 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/lock.png
--rw-rw-rw-   0        0        0     3463 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/lock_open.png
--rw-rw-rw-   0        0        0     2726 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/login.png
--rw-rw-rw-   0        0        0     2681 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/logout.png
--rw-rw-rw-   0        0        0     2912 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/magnet.png
--rw-rw-rw-   0        0        0     2557 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/mail.png
--rw-rw-rw-   0        0        0     2911 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/mail_opened.png
--rw-rw-rw-   0        0        0     2019 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/man.png
--rw-rw-rw-   0        0        0     1960 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/map.png
--rw-rw-rw-   0        0        0     4351 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/map_2.png
--rw-rw-rw-   0        0        0     4932 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/map_pin.png
--rw-rw-rw-   0        0        0     2493 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/math.png
--rw-rw-rw-   0        0        0     1910 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/maximize.png
--rw-rw-rw-   0        0        0     3895 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/medical_cross.png
--rw-rw-rw-   0        0        0      915 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/menu.png
--rw-rw-rw-   0        0        0     2725 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/message.png
--rw-rw-rw-   0        0        0     3050 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/message_2.png
--rw-rw-rw-   0        0        0     4720 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/message_circle.png
--rw-rw-rw-   0        0        0     2452 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/message_dots.png
--rw-rw-rw-   0        0        0     2335 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/messages.png
--rw-rw-rw-   0        0        0     4047 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/microphone.png
--rw-rw-rw-   0        0        0     1945 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/minimize.png
--rw-rw-rw-   0        0        0      653 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/minus.png
--rw-rw-rw-   0        0        0      616 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/minus_red.png
--rw-rw-rw-   0        0        0     1885 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/mist.png
--rw-rw-rw-   0        0        0     2866 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/mouse.png
--rw-rw-rw-   0        0        0     2049 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/movie.png
--rw-rw-rw-   0        0        0     2559 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/mug.png
--rw-rw-rw-   0        0        0     2201 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/music.png
--rw-rw-rw-   0        0        0     2429 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/new_section.png
--rw-rw-rw-   0        0        0     2932 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/news.png
--rw-rw-rw-   0        0        0     2147 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/note.png
--rw-rw-rw-   0        0        0     2352 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/notebook.png
--rw-rw-rw-   0        0        0     2825 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/notes.png
--rw-rw-rw-   0        0        0     2840 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/notification.png
--rw-rw-rw-   0        0        0     2470 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/outlet.png
--rw-rw-rw-   0        0        0     2914 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/package.png
--rw-rw-rw-   0        0        0     3173 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/paint.png
--rw-rw-rw-   0        0        0     3946 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/palette.png
--rw-rw-rw-   0        0        0     4342 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/paperclip.png
--rw-rw-rw-   0        0        0     3625 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/parentheses.png
--rw-rw-rw-   0        0        0     2107 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/pencil.png
--rw-rw-rw-   0        0        0     3572 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/photo.png
--rw-rw-rw-   0        0        0     2200 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/plug.png
--rw-rw-rw-   0        0        0     1165 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/plus.png
--rw-rw-rw-   0        0        0     1004 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/plus_green.png
--rw-rw-rw-   0        0        0     2402 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/point.png
--rw-rw-rw-   0        0        0     4075 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/power.png
--rw-rw-rw-   0        0        0     2708 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/presentation.png
--rw-rw-rw-   0        0        0     3534 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/printer.png
--rw-rw-rw-   0        0        0     1208 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/prompt.png
--rw-rw-rw-   0        0        0     2848 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/puzzle.png
--rw-rw-rw-   0        0        0     3046 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/qrcode.png
--rw-rw-rw-   0        0        0     1800 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/record_mail.png
--rw-rw-rw-   0        0        0     4501 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/recycle.png
--rw-rw-rw-   0        0        0     4309 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/refresh.png
--rw-rw-rw-   0        0        0     5443 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/registered.png
--rw-rw-rw-   0        0        0     2582 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/repeat.png
--rw-rw-rw-   0        0        0     2934 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/repeat_once.png
--rw-rw-rw-   0        0        0     3597 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/replace.png
--rw-rw-rw-   0        0        0     4342 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/rotate.png
--rw-rw-rw-   0        0        0     3966 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/rotate_2.png
--rw-rw-rw-   0        0        0     4334 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/rotate_clockwise.png
--rw-rw-rw-   0        0        0     4017 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/rotate_clockwise_2.png
--rw-rw-rw-   0        0        0     3008 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/rotate_rectangle.png
--rw-rw-rw-   0        0        0     3880 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/route.png
--rw-rw-rw-   0        0        0     4099 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/router.png
--rw-rw-rw-   0        0        0     4103 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/rss.png
--rw-rw-rw-   0        0        0     2384 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/ruler.png
--rw-rw-rw-   0        0        0     3453 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/scale.png
--rw-rw-rw-   0        0        0     2169 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/scan.png
--rw-rw-rw-   0        0        0     3249 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/scissors.png
--rw-rw-rw-   0        0        0     3948 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/search.png
--rw-rw-rw-   0        0        0     1460 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/selector.png
--rw-rw-rw-   0        0        0     3627 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/send.png
--rw-rw-rw-   0        0        0      853 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/separator.png
--rw-rw-rw-   0        0        0     3689 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/server.png
--rw-rw-rw-   0        0        0     2059 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/servicemark.png
--rw-rw-rw-   0        0        0     4623 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/settings.png
--rw-rw-rw-   0        0        0     2160 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/shape.png
--rw-rw-rw-   0        0        0     4054 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/share.png
--rw-rw-rw-   0        0        0     4377 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/shield.png
--rw-rw-rw-   0        0        0     4912 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/shield_check.png
--rw-rw-rw-   0        0        0     5078 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/shield_x.png
--rw-rw-rw-   0        0        0     2900 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/shopping_cart.png
--rw-rw-rw-   0        0        0     2957 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/sitemap.png
--rw-rw-rw-   0        0        0     3768 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/slideshow.png
--rw-rw-rw-   0        0        0     3111 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/social.png
--rw-rw-rw-   0        0        0     1983 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/sort_ascending.png
--rw-rw-rw-   0        0        0     2027 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/sort_descending.png
--rw-rw-rw-   0        0        0      935 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/space.png
--rw-rw-rw-   0        0        0     1919 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/square.png
--rw-rw-rw-   0        0        0     2664 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/square_check.png
--rw-rw-rw-   0        0        0     2210 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/square_minus.png
--rw-rw-rw-   0        0        0     2413 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/square_plus.png
--rw-rw-rw-   0        0        0     2789 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/square_x.png
--rw-rw-rw-   0        0        0     2173 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/stack.png
--rw-rw-rw-   0        0        0     4785 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/star.png
--rw-rw-rw-   0        0        0     4379 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/sticker.png
--rw-rw-rw-   0        0        0     2789 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/strikethrough.png
--rw-rw-rw-   0        0        0     2617 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/subscript.png
--rw-rw-rw-   0        0        0     2687 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/superscript.png
--rw-rw-rw-   0        0        0     2410 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/switch.png
--rw-rw-rw-   0        0        0     1790 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/switch_horizontal.png
--rw-rw-rw-   0        0        0     2016 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/switch_vertical.png
--rw-rw-rw-   0        0        0     1968 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/table.png
--rw-rw-rw-   0        0        0     2903 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/tag.png
--rw-rw-rw-   0        0        0     6690 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/target.png
--rw-rw-rw-   0        0        0     3594 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/tax.png
--rw-rw-rw-   0        0        0     2588 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/template.png
--rw-rw-rw-   0        0        0     1213 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/terminal.png
--rw-rw-rw-   0        0        0     2898 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/terminal_2.png
--rw-rw-rw-   0        0        0     2381 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/text_wrap.png
--rw-rw-rw-   0        0        0     2707 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/ticket.png
--rw-rw-rw-   0        0        0     4053 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/toggle_left.png
--rw-rw-rw-   0        0        0     4077 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/toggle_right.png
--rw-rw-rw-   0        0        0     3045 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/tool.png
--rw-rw-rw-   0        0        0     3601 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/tools.png
--rw-rw-rw-   0        0        0     2994 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/trash.png
--rw-rw-rw-   0        0        0     4060 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/trees.png
--rw-rw-rw-   0        0        0     1629 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/trending_down.png
--rw-rw-rw-   0        0        0     1658 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/trending_up.png
--rw-rw-rw-   0        0        0     2827 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/triangle.png
--rw-rw-rw-   0        0        0     3275 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/trophy.png
--rw-rw-rw-   0        0        0     2051 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/underline.png
--rw-rw-rw-   0        0        0     4631 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/unlink.png
--rw-rw-rw-   0        0        0     2204 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/upload.png
--rw-rw-rw-   0        0        0     3148 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/urgent.png
--rw-rw-rw-   0        0        0     3568 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/user.png
--rw-rw-rw-   0        0        0     4047 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/user_check.png
--rw-rw-rw-   0        0        0     4029 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/user_exclamation.png
--rw-rw-rw-   0        0        0     3816 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/user_minus.png
--rw-rw-rw-   0        0        0     4132 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/user_plus.png
--rw-rw-rw-   0        0        0     4198 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/user_x.png
--rw-rw-rw-   0        0        0     5017 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/users.png
--rw-rw-rw-   0        0        0     5251 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/viewfinder.png
--rw-rw-rw-   0        0        0     2214 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/viewport_narrow.png
--rw-rw-rw-   0        0        0     2266 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/viewport_wide.png
--rw-rw-rw-   0        0        0     4312 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/virus.png
--rw-rw-rw-   0        0        0     4418 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/volume.png
--rw-rw-rw-   0        0        0     3153 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/volume_2.png
--rw-rw-rw-   0        0        0     2954 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/volume_3.png
--rw-rw-rw-   0        0        0     2539 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/wallet.png
--rw-rw-rw-   0        0        0     2761 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/wand.png
--rw-rw-rw-   0        0        0     3742 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/wifi.png
--rw-rw-rw-   0        0        0      549 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/wifi_0.png
--rw-rw-rw-   0        0        0     1307 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/wifi_1.png
--rw-rw-rw-   0        0        0     2399 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/wifi_2.png
--rw-rw-rw-   0        0        0     3913 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/wind.png
--rw-rw-rw-   0        0        0     2280 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/woman.png
--rw-rw-rw-   0        0        0     5571 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/world.png
--rw-rw-rw-   0        0        0     1505 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/x.png
--rw-rw-rw-   0        0        0     6512 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/yin_yang.png
--rw-rw-rw-   0        0        0     4478 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/zoom_in.png
--rw-rw-rw-   0        0        0     4180 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/zoom_out.png
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/logo/
--rw-rw-rw-   0        0        0   148555 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/logo/amulet_logo.png
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/
--rw-rw-rw-   0        0        0      629 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_array.png
--rw-rw-rw-   0        0        0      609 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_byte.png
--rw-rw-rw-   0        0        0      664 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_compound.png
--rw-rw-rw-   0        0        0      597 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_double.png
--rw-rw-rw-   0        0        0      558 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_float.png
--rw-rw-rw-   0        0        0      574 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_int.png
--rw-rw-rw-   0        0        0      666 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_list.png
--rw-rw-rw-   0        0        0      554 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_long.png
--rw-rw-rw-   0        0        0      601 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_short.png
--rw-rw-rw-   0        0        0      604 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_string.png
--rw-rw-rw-   0        0        0     4503 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/lang.py
--rw-rw-rw-   0        0        0      646 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/logging.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/
--rw-rw-rw-   0        0        0      835 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/camera/
--rw-rw-rw-   0        0        0      213 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/camera/__init__.py
--rw-rw-rw-   0        0        0    12019 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/camera/camera.py
--rw-rw-rw-   0        0        0     1356 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/camera/controllable_camera.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/canvas/
--rw-rw-rw-   0        0        0       71 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/canvas/__init__.py
--rw-rw-rw-   0        0        0     1898 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/canvas/canvas.py
--rw-rw-rw-   0        0        0     2004 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/canvas/event_canvas.py
--rw-rw-rw-   0        0        0      477 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/canvas_container.py
--rw-rw-rw-   0        0        0      293 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/context_manager.py
--rw-rw-rw-   0        0        0      229 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/data_types.py
--rw-rw-rw-   0        0        0      289 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/drawable.py
--rw-rw-rw-   0        0        0      308 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/events.py
--rw-rw-rw-   0        0        0     1661 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/matrix.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/
--rw-rw-rw-   0        0        0       64 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level/
--rw-rw-rw-   0        0        0       32 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level/chunk/
--rw-rw-rw-   0        0        0       32 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level/chunk/__init__.py
--rw-rw-rw-   0        0        0    11030 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level/chunk/chunk.py
--rw-rw-rw-   0        0        0    10527 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level/chunk/chunk_builder.py
--rw-rw-rw-   0        0        0    11879 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level/level.py
--rw-rw-rw-   0        0        0    11257 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level/region.py
--rw-rw-rw-   0        0        0      468 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level/selection.py
--rw-rw-rw-   0        0        0     7037 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level_group.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/
--rw-rw-rw-   0        0        0      165 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/box/
--rw-rw-rw-   0        0        0      185 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/box/__init__.py
--rw-rw-rw-   0        0        0      243 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/box/colours.json
--rw-rw-rw-   0        0        0      506 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/box/colours.py
--rw-rw-rw-   0        0        0     9498 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/box/render_selection.py
--rw-rw-rw-   0        0        0    11559 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/box/render_selection_editable.py
--rw-rw-rw-   0        0        0     1921 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/box/render_selection_highlightable.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/group/
--rw-rw-rw-   0        0        0      143 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/group/__init__.py
--rw-rw-rw-   0        0        0     2243 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/group/render_selection_group.py
--rw-rw-rw-   0        0        0      914 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/group/render_selection_group_highlightable.py
--rw-rw-rw-   0        0        0     2881 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/sky_box.py
--rw-rw-rw-   0        0        0     6237 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/tri_mesh.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/resource_pack/
--rw-rw-rw-   0        0        0      158 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/resource_pack/__init__.py
--rw-rw-rw-   0        0        0     6890 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/resource_pack/resource_pack.py
--rw-rw-rw-   0        0        0     1166 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/resource_pack/resource_pack_manager.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/shaders/
--rw-rw-rw-   0        0        0     2196 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/shaders/__init__.py
--rw-rw-rw-   0        0        0      436 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/shaders/render_chunk_120.frag
--rw-rw-rw-   0        0        0      504 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/shaders/render_chunk_120.vert
--rw-rw-rw-   0        0        0      437 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/shaders/render_chunk_330.frag
--rw-rw-rw-   0        0        0      437 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/shaders/render_chunk_330.vert
--rw-rw-rw-   0        0        0    10315 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/textureatlas.py
--rw-rw-rw-   0        0        0     1930 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/thread_generator.py
--rw-rw-rw-   0        0        0     3099 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/resources.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/
--rw-rw-rw-   0        0        0        0 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/
--rw-rw-rw-   0        0        0        0 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/__init__.py
--rw-rw-rw-   0        0        0     3361 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/base_define.py
--rw-rw-rw-   0        0        0     7850 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/base_select.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/biome_select/
--rw-rw-rw-   0        0        0       39 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/biome_select/__init__.py
--rw-rw-rw-   0        0        0     1967 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/biome_select/biome_define.py
--rw-rw-rw-   0        0        0      920 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/biome_select/biome_select.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/block_select/
--rw-rw-rw-   0        0        0      191 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/block_select/__init__.py
--rw-rw-rw-   0        0        0     5646 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/block_select/block_define.py
--rw-rw-rw-   0        0        0     1804 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/block_select/block_select.py
--rw-rw-rw-   0        0        0     6907 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/block_select/multi_block_define.py
--rw-rw-rw-   0        0        0    13667 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/block_select/properties.py
--rw-rw-rw-   0        0        0    14216 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/nbt_editor.py
--rw-rw-rw-   0        0        0    12102 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/select_world.py
--rw-rw-rw-   0        0        0     5947 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/simple.py
--rw-rw-rw-   0        0        0     2706 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/traceback_dialog.py
--rw-rw-rw-   0        0        0     9009 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/version_select.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/util/
--rw-rw-rw-   0        0        0        0 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/util/__init__.py
--rw-rw-rw-   0        0        0     9141 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/util/button_input.py
--rw-rw-rw-   0        0        0    16783 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/util/key_config.py
--rw-rw-rw-   0        0        0     5204 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/util/mouse_movement.py
--rw-rw-rw-   0        0        0     2350 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/util/ui_preferences.py
--rw-rw-rw-   0        0        0     1062 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/util/validators.py
--rw-rw-rw-   0        0        0      457 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/api/wx/util/window_container.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/lang/
--rw-rw-rw-   0        0        0    16234 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/lang/cs.lang
--rw-rw-rw-   0        0        0    14748 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/lang/de.lang
--rw-rw-rw-   0        0        0    15730 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/lang/en.lang
--rw-rw-rw-   0        0        0    17293 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/lang/fr.lang
--rw-rw-rw-   0        0        0    13212 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/lang/id.lang
--rw-rw-rw-   0        0        0    18609 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/lang/ja.lang
--rw-rw-rw-   0        0        0    14396 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/lang/ko.lang
--rw-rw-rw-   0        0        0    22815 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/lang/ru.lang
--rw-rw-rw-   0        0        0    18106 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/lang/vi.lang
--rw-rw-rw-   0        0        0    13331 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/lang/zh_CN.lang
--rw-rw-rw-   0        0        0    12652 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/lang/zh_TW.lang
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/
--rw-rw-rw-   0        0        0        0 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/convert/
--rw-rw-rw-   0        0        0      158 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/convert/__init__.py
--rw-rw-rw-   0        0        0     6439 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/convert/convert.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/
--rw-rw-rw-   0        0        0      255 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/
--rw-rw-rw-   0        0        0     6950 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/down.png
--rw-rw-rw-   0        0        0    36091 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/east.png
--rw-rw-rw-   0        0        0    29789 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/north.png
--rw-rw-rw-   0        0        0    41677 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/south.png
--rw-rw-rw-   0        0        0    36204 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/up.png
--rw-rw-rw-   0        0        0    36917 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/west.png
--rw-rw-rw-   0        0        0     1292 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/selection.png
--rw-rw-rw-   0        0        0     1383 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/translucent_white.png
--rw-rw-rw-   0        0        0      540 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/manifest.json
--rw-rw-rw-   0        0        0     1337 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/pack_icon.png
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/textures/
--rw-rw-rw-   0        0        0      340 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/textures/terrain_texture.json
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/
--rw-rw-rw-   0        0        0     6950 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/down.png
--rw-rw-rw-   0        0        0    36091 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/east.png
--rw-rw-rw-   0        0        0    29789 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/north.png
--rw-rw-rw-   0        0        0    41677 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/south.png
--rw-rw-rw-   0        0        0    36204 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/up.png
--rw-rw-rw-   0        0        0    36917 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/west.png
--rw-rw-rw-   0        0        0     1292 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/selection.png
--rw-rw-rw-   0        0        0     1383 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/translucent_white.png
--rw-rw-rw-   0        0        0       94 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/pack.mcmeta
--rw-rw-rw-   0        0        0     1337 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/pack.png
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/
--rw-rw-rw-   0        0        0       88 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/
--rw-rw-rw-   0        0        0      536 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/__init__.py
--rw-rw-rw-   0        0        0      611 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/base_behaviour.py
--rw-rw-rw-   0        0        0    22005 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/block_selection_behaviour.py
--rw-rw-rw-   0        0        0     7819 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/camera_behaviour.py
--rw-rw-rw-   0        0        0     6820 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/chunk_selection_behaviour.py
--rw-rw-rw-   0        0        0     4184 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/inspect_block_behaviour.py
--rw-rw-rw-   0        0        0     3377 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/pointer_behaviour.py
--rw-rw-rw-   0        0        0     9545 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/raycast_behaviour.py
--rw-rw-rw-   0        0        0     1415 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/static_selection_behaviour.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/canvas/
--rw-rw-rw-   0        0        0       37 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/canvas/__init__.py
--rw-rw-rw-   0        0        0    11000 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/canvas/base_edit_canvas.py
--rw-rw-rw-   0        0        0    11712 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/canvas/edit_canvas.py
--rw-rw-rw-   0        0        0     1238 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/chunk_generator.py
--rw-rw-rw-   0        0        0      554 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/edit_canvas_container.py
--rw-rw-rw-   0        0        0     1061 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/events.py
--rw-rw-rw-   0        0        0     4661 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/key_config.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/
--rw-rw-rw-   0        0        0      256 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/base/
--rw-rw-rw-   0        0        0      110 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/base/__init__.py
--rw-rw-rw-   0        0        0     2420 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/base/default_operation_ui.py
--rw-rw-rw-   0        0        0     3192 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/base/operation_ui.py
--rw-rw-rw-   0        0        0      956 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/errors.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/manager/
--rw-rw-rw-   0        0        0      189 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/manager/loader/
--rw-rw-rw-   0        0        0      155 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/manager/loader/__init__.py
--rw-rw-rw-   0        0        0     1735 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/manager/loader/base_operation_loader.py
--rw-rw-rw-   0        0        0     1588 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/manager/loader/operation_loader.py
--rw-rw-rw-   0        0        0     3643 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/manager/loader/ui_operation_loader.py
--rw-rw-rw-   0        0        0     5907 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/manager/operation_manager.py
--rw-rw-rw-   0        0        0      356 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/manager/util.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/ui/
--rw-rw-rw-   0        0        0        0 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/ui/__init__.py
--rw-rw-rw-   0        0        0     8343 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/ui/fixed_pipeline.py
--rw-rw-rw-   0        0        0     1495 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/ui/simple_operation_panel.py
--rw-rw-rw-   0        0        0     8718 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/renderer.py
--rw-rw-rw-   0        0        0     5795 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/selection.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/
--rw-rw-rw-   0        0        0        2 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/__init__.py
--rw-rw-rw-   0        0        0      839 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/canvas_toggle_element.py
--rw-rw-rw-   0        0        0     6779 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/file.py
--rw-rw-rw-   0        0        0     4790 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/goto.py
--rw-rw-rw-   0        0        0     3507 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/nudge_button.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/select_location/
--rw-rw-rw-   0        0        0      326 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/select_location/__init__.py
--rw-rw-rw-   0        0        0     3062 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/select_location/events.py
--rw-rw-rw-   0        0        0     4202 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/select_location/select_location.py
--rw-rw-rw-   0        0        0     2995 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/select_location/select_transform.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/tool/
--rw-rw-rw-   0        0        0      153 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/tool/__init__.py
--rw-rw-rw-   0        0        0     6306 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/tool/base_operation_choice.py
--rw-rw-rw-   0        0        0     1162 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/tool/base_tool_ui.py
--rw-rw-rw-   0        0        0     3174 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/tool/default_base_tool_ui.py
--rw-rw-rw-   0        0        0     4614 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/tool_manager.py
--rw-rw-rw-   0        0        0    12624 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/edit.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/
--rw-rw-rw-   0        0        0        0 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/
--rw-rw-rw-   0        0        0        0 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/examples/
--rw-rw-rw-   0        0        0     1251 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/examples/1_fixed_function_pipeline.py
--rw-rw-rw-   0        0        0     1148 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/examples/2_fixed_function_pipeline.py
--rw-rw-rw-   0        0        0     3420 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/examples/3_fixed_function_pipeline.py
--rw-rw-rw-   0        0        0        0 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/
--rw-rw-rw-   0        0        0        0 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/
--rw-rw-rw-   0        0        0        0 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/__init__.py
--rw-rw-rw-   0        0        0     3717 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/construction.py
--rw-rw-rw-   0        0        0     3929 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/mcstructure.py
--rw-rw-rw-   0        0        0     4303 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/schematic.py
--rw-rw-rw-   0        0        0     3926 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/sponge_schematic.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/
--rw-rw-rw-   0        0        0       74 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/__init__.py
--rw-rw-rw-   0        0        0      896 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/copy.py
--rw-rw-rw-   0        0        0      973 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/cut.py
--rw-rw-rw-   0        0        0      801 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/delete.py
--rw-rw-rw-   0        0        0      865 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/prune_chunks.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/
--rw-rw-rw-   0        0        0        0 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/__init__.py
--rw-rw-rw-   0        0        0     1204 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/clone.py
--rw-rw-rw-   0        0        0     3198 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/fill.py
--rw-rw-rw-   0        0        0     7354 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/replace.py
--rw-rw-rw-   0        0        0     6007 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/set_biome.py
--rw-rw-rw-   0        0        0    10932 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/waterlog.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/tools/
--rw-rw-rw-   0        0        0      204 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/tools/__init__.py
--rw-rw-rw-   0        0        0    10143 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/tools/chunk.py
--rw-rw-rw-   0        0        0      249 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/tools/export_tool.py
--rw-rw-rw-   0        0        0     2945 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/tools/import_tool.py
--rw-rw-rw-   0        0        0      248 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/tools/operation.py
--rw-rw-rw-   0        0        0    23618 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/tools/paste.py
--rw-rw-rw-   0        0        0    13768 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/tools/select.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor.egg-info/
--rw-rw-rw-   0        0        0      429 2022-06-19 18:36:05.000000 amulet-map-editor-0.9.5/amulet_map_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    34995 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      190 2022-06-19 18:36:05.000000 amulet-map-editor-0.9.5/amulet_map_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2022-06-19 18:36:05.000000 amulet-map-editor-0.9.5/amulet_map_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/amulet_map_editor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4076 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/icon.ico
--rw-rw-rw-   0        0        0      175 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/pyproject.toml
--rw-rw-rw-   0        0        0      263 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/requirements.txt
--rw-rw-rw-   0        0        0      925 2022-06-19 18:36:06.000000 amulet-map-editor-0.9.5/setup.cfg
--rw-rw-rw-   0        0        0     4441 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/setup.py
--rw-rw-rw-   0        0        0    70636 2022-06-19 18:35:16.000000 amulet-map-editor-0.9.5/versioneer.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/
+-rw-rw-rw-   0        0        0      227 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      429 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/
+-rw-rw-rw-   0        0        0      202 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/__init__.py
+-rw-rw-rw-   0        0        0     1293 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor/__pyinstaller/
+-rw-rw-rw-   0        0        0       43 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      277 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/__pyinstaller/hook-amulet_map_editor.py
+-rw-rw-rw-   0        0        0      518 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/_version.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/
+-rw-rw-rw-   0        0        0       26 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/__init__.py
+-rw-rw-rw-   0        0        0     1147 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/config.py
+-rw-rw-rw-   0        0        0      345 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/datatypes.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/framework/
+-rw-rw-rw-   0        0        0       61 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/framework/__init__.py
+-rw-rw-rw-   0        0        0     8340 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/framework/amulet_ui.py
+-rw-rw-rw-   0        0        0      660 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/framework/app.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/framework/pages/
+-rw-rw-rw-   0        0        0      111 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/framework/pages/__init__.py
+-rw-rw-rw-   0        0        0      264 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/framework/pages/base_page.py
+-rw-rw-rw-   0        0        0     3004 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/framework/pages/main_menu.py
+-rw-rw-rw-   0        0        0     6402 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/framework/pages/world_page.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/framework/programs/
+-rw-rw-rw-   0        0        0       80 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/framework/programs/__init__.py
+-rw-rw-rw-   0        0        0     1557 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/framework/programs/about_program.py
+-rw-rw-rw-   0        0        0      705 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/framework/programs/base_program.py
+-rw-rw-rw-   0        0        0     4869 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/framework/update_check.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/
+-rw-rw-rw-   0        0        0     2295 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/
+-rw-rw-rw-   0        0        0     5695 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/accessible.png
+-rw-rw-rw-   0        0        0     3210 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/adjustments.png
+-rw-rw-rw-   0        0        0     4924 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/alert_circle.png
+-rw-rw-rw-   0        0        0     3398 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/alert_triangle.png
+-rw-rw-rw-   0        0        0     1207 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/align_center.png
+-rw-rw-rw-   0        0        0     1184 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/align_justified.png
+-rw-rw-rw-   0        0        0     1201 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/align_left.png
+-rw-rw-rw-   0        0        0     1207 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/align_right.png
+-rw-rw-rw-   0        0        0     3781 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/anchor.png
+-rw-rw-rw-   0        0        0     6426 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/aperture.png
+-rw-rw-rw-   0        0        0     2280 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/apps.png
+-rw-rw-rw-   0        0        0     2655 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/archive.png
+-rw-rw-rw-   0        0        0     2242 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_back.png
+-rw-rw-rw-   0        0        0     2315 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_back_up.png
+-rw-rw-rw-   0        0        0     1543 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_bar_down.png
+-rw-rw-rw-   0        0        0     1756 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_bar_left.png
+-rw-rw-rw-   0        0        0     1652 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_bar_right.png
+-rw-rw-rw-   0        0        0     1537 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_bar_up.png
+-rw-rw-rw-   0        0        0     1470 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_down.png
+-rw-rw-rw-   0        0        0     5351 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_down_circle.png
+-rw-rw-rw-   0        0        0     1323 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_down_left.png
+-rw-rw-rw-   0        0        0     5196 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_down_left_circle.png
+-rw-rw-rw-   0        0        0     1286 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_down_right.png
+-rw-rw-rw-   0        0        0     5187 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_down_right_circle.png
+-rw-rw-rw-   0        0        0     2127 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_forward.png
+-rw-rw-rw-   0        0        0     2192 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_forward_up.png
+-rw-rw-rw-   0        0        0     1233 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_left.png
+-rw-rw-rw-   0        0        0     5185 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_left_circle.png
+-rw-rw-rw-   0        0        0     1317 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_down.png
+-rw-rw-rw-   0        0        0     1146 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_left.png
+-rw-rw-rw-   0        0        0     1054 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_right.png
+-rw-rw-rw-   0        0        0     1300 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_up.png
+-rw-rw-rw-   0        0        0     1135 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_right.png
+-rw-rw-rw-   0        0        0     5108 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_right_circle.png
+-rw-rw-rw-   0        0        0     1398 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_up.png
+-rw-rw-rw-   0        0        0     5368 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_up_circle.png
+-rw-rw-rw-   0        0        0     1328 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_up_left.png
+-rw-rw-rw-   0        0        0     5186 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_up_left_circle.png
+-rw-rw-rw-   0        0        0     1329 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_up_right.png
+-rw-rw-rw-   0        0        0     5188 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_up_right_circle.png
+-rw-rw-rw-   0        0        0     1774 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrows_diagonal.png
+-rw-rw-rw-   0        0        0     1751 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrows_diagonal_2.png
+-rw-rw-rw-   0        0        0     1461 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrows_horizontal.png
+-rw-rw-rw-   0        0        0     2792 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrows_maximize.png
+-rw-rw-rw-   0        0        0     2746 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrows_minimize.png
+-rw-rw-rw-   0        0        0     2179 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrows_sort.png
+-rw-rw-rw-   0        0        0     1793 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrows_vertical.png
+-rw-rw-rw-   0        0        0     2160 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/artboard.png
+-rw-rw-rw-   0        0        0     5971 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/at.png
+-rw-rw-rw-   0        0        0     5172 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/award.png
+-rw-rw-rw-   0        0        0     2218 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/backspace.png
+-rw-rw-rw-   0        0        0     2707 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/box.png
+-rw-rw-rw-   0        0        0     3272 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/braces.png
+-rw-rw-rw-   0        0        0     1386 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/brackets.png
+-rw-rw-rw-   0        0        0     1020 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/caret_down.png
+-rw-rw-rw-   0        0        0     1268 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/caret_left.png
+-rw-rw-rw-   0        0        0     1245 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/caret_right.png
+-rw-rw-rw-   0        0        0     1037 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/caret_up.png
+-rw-rw-rw-   0        0        0     1132 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/check.png
+-rw-rw-rw-   0        0        0     2598 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/checkbox.png
+-rw-rw-rw-   0        0        0     1543 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/checks.png
+-rw-rw-rw-   0        0        0     1062 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevron_down.png
+-rw-rw-rw-   0        0        0      995 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevron_left.png
+-rw-rw-rw-   0        0        0      952 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevron_right.png
+-rw-rw-rw-   0        0        0     1001 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevron_up.png
+-rw-rw-rw-   0        0        0     1627 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevrons_down.png
+-rw-rw-rw-   0        0        0     1410 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevrons_left.png
+-rw-rw-rw-   0        0        0     1302 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevrons_right.png
+-rw-rw-rw-   0        0        0     1515 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevrons_up.png
+-rw-rw-rw-   0        0        0     4478 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/circle.png
+-rw-rw-rw-   0        0        0     5101 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/circle_check.png
+-rw-rw-rw-   0        0        0     4738 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/circle_minus.png
+-rw-rw-rw-   0        0        0     4975 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/circle_plus.png
+-rw-rw-rw-   0        0        0     5221 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/circle_x.png
+-rw-rw-rw-   0        0        0     3038 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/click.png
+-rw-rw-rw-   0        0        0     2538 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/clipboard.png
+-rw-rw-rw-   0        0        0     3280 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/clipboard_check.png
+-rw-rw-rw-   0        0        0     3267 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/clipboard_list.png
+-rw-rw-rw-   0        0        0     3445 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/clipboard_x.png
+-rw-rw-rw-   0        0        0     4938 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/clock.png
+-rw-rw-rw-   0        0        0     3766 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/cloud.png
+-rw-rw-rw-   0        0        0     4512 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/cloud_download.png
+-rw-rw-rw-   0        0        0     4632 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/cloud_upload.png
+-rw-rw-rw-   0        0        0     2371 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/code.png
+-rw-rw-rw-   0        0        0     2076 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/color_picker.png
+-rw-rw-rw-   0        0        0     4107 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/color_swatch.png
+-rw-rw-rw-   0        0        0     2358 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/command.png
+-rw-rw-rw-   0        0        0     2731 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/copy.png
+-rw-rw-rw-   0        0        0     5801 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/copyright.png
+-rw-rw-rw-   0        0        0     1733 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_down_left.png
+-rw-rw-rw-   0        0        0     1696 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_down_right.png
+-rw-rw-rw-   0        0        0     1798 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_left_down.png
+-rw-rw-rw-   0        0        0     1783 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_left_up.png
+-rw-rw-rw-   0        0        0     1801 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_right_down.png
+-rw-rw-rw-   0        0        0     1774 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_right_up.png
+-rw-rw-rw-   0        0        0     1774 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_up_left.png
+-rw-rw-rw-   0        0        0     1639 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_up_right.png
+-rw-rw-rw-   0        0        0     1477 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/crop.png
+-rw-rw-rw-   0        0        0     3425 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/cut.png
+-rw-rw-rw-   0        0        0     4739 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/dashboard.png
+-rw-rw-rw-   0        0        0     4530 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/database.png
+-rw-rw-rw-   0        0        0     1646 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_desktop.png
+-rw-rw-rw-   0        0        0     3025 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_floppy.png
+-rw-rw-rw-   0        0        0     2580 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_gamepad.png
+-rw-rw-rw-   0        0        0     1558 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_laptop.png
+-rw-rw-rw-   0        0        0     1772 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_mobile.png
+-rw-rw-rw-   0        0        0     1979 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_tablet.png
+-rw-rw-rw-   0        0        0     2281 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_tv.png
+-rw-rw-rw-   0        0        0     2493 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_watch.png
+-rw-rw-rw-   0        0        0     1980 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/devices.png
+-rw-rw-rw-   0        0        0     1364 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/direction.png
+-rw-rw-rw-   0        0        0     1182 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/direction_horizontal.png
+-rw-rw-rw-   0        0        0      948 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/dots.png
+-rw-rw-rw-   0        0        0     4827 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/dots_circle_horizontal.png
+-rw-rw-rw-   0        0        0     1563 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/dots_diagonal.png
+-rw-rw-rw-   0        0        0     1563 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/dots_diagonal_2.png
+-rw-rw-rw-   0        0        0     1601 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/dots_vertical.png
+-rw-rw-rw-   0        0        0     2248 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/download.png
+-rw-rw-rw-   0        0        0     3797 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/drag_drop.png
+-rw-rw-rw-   0        0        0     2810 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/drag_drop_2.png
+-rw-rw-rw-   0        0        0     3169 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/edit.png
+-rw-rw-rw-   0        0        0     1975 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/eraser.png
+-rw-rw-rw-   0        0        0     4115 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/exchange.png
+-rw-rw-rw-   0        0        0     2649 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/external_link.png
+-rw-rw-rw-   0        0        0     2136 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file.png
+-rw-rw-rw-   0        0        0     2875 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_check.png
+-rw-rw-rw-   0        0        0     3175 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_code.png
+-rw-rw-rw-   0        0        0     3005 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_download.png
+-rw-rw-rw-   0        0        0     2065 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_horizontal.png
+-rw-rw-rw-   0        0        0     2878 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_invoice.png
+-rw-rw-rw-   0        0        0     2450 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_minus.png
+-rw-rw-rw-   0        0        0     3003 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_music.png
+-rw-rw-rw-   0        0        0     2676 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_plus.png
+-rw-rw-rw-   0        0        0     2335 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_shredder.png
+-rw-rw-rw-   0        0        0     2965 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_text.png
+-rw-rw-rw-   0        0        0     3042 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_x.png
+-rw-rw-rw-   0        0        0     1969 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/filter.png
+-rw-rw-rw-   0        0        0     3138 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/flag.png
+-rw-rw-rw-   0        0        0     3368 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/flame.png
+-rw-rw-rw-   0        0        0     2170 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/flask.png
+-rw-rw-rw-   0        0        0     1852 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/flip_horizontal.png
+-rw-rw-rw-   0        0        0     2407 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/flip_vertical.png
+-rw-rw-rw-   0        0        0     2931 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/floppy_disk.png
+-rw-rw-rw-   0        0        0     4886 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/focus.png
+-rw-rw-rw-   0        0        0     4412 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/focus_2.png
+-rw-rw-rw-   0        0        0     1998 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/folder.png
+-rw-rw-rw-   0        0        0     2312 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/folder_minus.png
+-rw-rw-rw-   0        0        0     2502 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/folder_plus.png
+-rw-rw-rw-   0        0        0     2871 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/folder_x.png
+-rw-rw-rw-   0        0        0     2819 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/folders.png
+-rw-rw-rw-   0        0        0     4968 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/forbid.png
+-rw-rw-rw-   0        0        0     4970 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/forbid_2.png
+-rw-rw-rw-   0        0        0     1521 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/frame.png
+-rw-rw-rw-   0        0        0     3231 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/friends.png
+-rw-rw-rw-   0        0        0     3562 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/gift.png
+-rw-rw-rw-   0        0        0     2900 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/git_branch.png
+-rw-rw-rw-   0        0        0     1916 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/git_commit.png
+-rw-rw-rw-   0        0        0     3512 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/git_compare.png
+-rw-rw-rw-   0        0        0     2566 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/git_fork.png
+-rw-rw-rw-   0        0        0     2789 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/git_merge.png
+-rw-rw-rw-   0        0        0     2908 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/git_pull_request.png
+-rw-rw-rw-   0        0        0     1924 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/grid.png
+-rw-rw-rw-   0        0        0     2101 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/grid_dots.png
+-rw-rw-rw-   0        0        0     1522 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/grip_horizontal.png
+-rw-rw-rw-   0        0        0     1924 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/grip_vertical.png
+-rw-rw-rw-   0        0        0     3118 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/hand_stop.png
+-rw-rw-rw-   0        0        0     2221 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/hash.png
+-rw-rw-rw-   0        0        0     5570 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/help.png
+-rw-rw-rw-   0        0        0     3495 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/hexagon.png
+-rw-rw-rw-   0        0        0     5131 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/history.png
+-rw-rw-rw-   0        0        0     2712 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/home.png
+-rw-rw-rw-   0        0        0     2363 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/home_2.png
+-rw-rw-rw-   0        0        0     1745 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/indent_decrease.png
+-rw-rw-rw-   0        0        0     1694 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/indent_increase.png
+-rw-rw-rw-   0        0        0     3729 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/infinity.png
+-rw-rw-rw-   0        0        0     5031 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/info_circle.png
+-rw-rw-rw-   0        0        0     2571 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/info_square.png
+-rw-rw-rw-   0        0        0     2794 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/keyboard.png
+-rw-rw-rw-   0        0        0     3306 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/language.png
+-rw-rw-rw-   0        0        0     3161 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layers_difference.png
+-rw-rw-rw-   0        0        0     2959 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layers_intersect.png
+-rw-rw-rw-   0        0        0     2716 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layers_subtract.png
+-rw-rw-rw-   0        0        0     2572 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layers_union.png
+-rw-rw-rw-   0        0        0     3445 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout.png
+-rw-rw-rw-   0        0        0     2909 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_2.png
+-rw-rw-rw-   0        0        0     1977 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_align_bottom.png
+-rw-rw-rw-   0        0        0     2077 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_align_center.png
+-rw-rw-rw-   0        0        0     2124 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_align_left.png
+-rw-rw-rw-   0        0        0     1979 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_align_middle.png
+-rw-rw-rw-   0        0        0     2158 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_align_right.png
+-rw-rw-rw-   0        0        0     1962 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_align_top.png
+-rw-rw-rw-   0        0        0     1924 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_bottombar.png
+-rw-rw-rw-   0        0        0     2462 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_cards.png
+-rw-rw-rw-   0        0        0     1958 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_columns.png
+-rw-rw-rw-   0        0        0     2207 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_distribute_horizontal.png
+-rw-rw-rw-   0        0        0     2287 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_distribute_vertical.png
+-rw-rw-rw-   0        0        0     2845 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_list.png
+-rw-rw-rw-   0        0        0     1925 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_navbar.png
+-rw-rw-rw-   0        0        0     1924 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_rows.png
+-rw-rw-rw-   0        0        0     1937 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_sidebar.png
+-rw-rw-rw-   0        0        0     1972 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_sidebar_right.png
+-rw-rw-rw-   0        0        0     2907 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/license.png
+-rw-rw-rw-   0        0        0     2457 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/line_height.png
+-rw-rw-rw-   0        0        0     3800 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/link.png
+-rw-rw-rw-   0        0        0     1650 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/list.png
+-rw-rw-rw-   0        0        0     2543 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/list_check.png
+-rw-rw-rw-   0        0        0     3414 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/location.png
+-rw-rw-rw-   0        0        0     3313 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/lock.png
+-rw-rw-rw-   0        0        0     3463 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/lock_open.png
+-rw-rw-rw-   0        0        0     2726 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/login.png
+-rw-rw-rw-   0        0        0     2681 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/logout.png
+-rw-rw-rw-   0        0        0     2912 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/magnet.png
+-rw-rw-rw-   0        0        0     2557 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/mail.png
+-rw-rw-rw-   0        0        0     2911 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/mail_opened.png
+-rw-rw-rw-   0        0        0     2019 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/man.png
+-rw-rw-rw-   0        0        0     1960 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/map.png
+-rw-rw-rw-   0        0        0     4351 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/map_2.png
+-rw-rw-rw-   0        0        0     4932 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/map_pin.png
+-rw-rw-rw-   0        0        0     2493 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/math.png
+-rw-rw-rw-   0        0        0     1910 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/maximize.png
+-rw-rw-rw-   0        0        0     3895 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/medical_cross.png
+-rw-rw-rw-   0        0        0      915 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/menu.png
+-rw-rw-rw-   0        0        0     2725 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/message.png
+-rw-rw-rw-   0        0        0     3050 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/message_2.png
+-rw-rw-rw-   0        0        0     4720 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/message_circle.png
+-rw-rw-rw-   0        0        0     2452 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/message_dots.png
+-rw-rw-rw-   0        0        0     2335 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/messages.png
+-rw-rw-rw-   0        0        0     4047 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/microphone.png
+-rw-rw-rw-   0        0        0     1945 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/minimize.png
+-rw-rw-rw-   0        0        0      653 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/minus.png
+-rw-rw-rw-   0        0        0      616 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/minus_red.png
+-rw-rw-rw-   0        0        0     1885 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/mist.png
+-rw-rw-rw-   0        0        0     2866 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/mouse.png
+-rw-rw-rw-   0        0        0     2049 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/movie.png
+-rw-rw-rw-   0        0        0     2559 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/mug.png
+-rw-rw-rw-   0        0        0     2201 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/music.png
+-rw-rw-rw-   0        0        0     2429 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/new_section.png
+-rw-rw-rw-   0        0        0     2932 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/news.png
+-rw-rw-rw-   0        0        0     2147 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/note.png
+-rw-rw-rw-   0        0        0     2352 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/notebook.png
+-rw-rw-rw-   0        0        0     2825 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/notes.png
+-rw-rw-rw-   0        0        0     2840 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/notification.png
+-rw-rw-rw-   0        0        0     2470 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/outlet.png
+-rw-rw-rw-   0        0        0     2914 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/package.png
+-rw-rw-rw-   0        0        0     3173 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/paint.png
+-rw-rw-rw-   0        0        0     3946 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/palette.png
+-rw-rw-rw-   0        0        0     4342 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/paperclip.png
+-rw-rw-rw-   0        0        0     3625 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/parentheses.png
+-rw-rw-rw-   0        0        0     2107 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/pencil.png
+-rw-rw-rw-   0        0        0     3572 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/photo.png
+-rw-rw-rw-   0        0        0     2200 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/plug.png
+-rw-rw-rw-   0        0        0     1165 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/plus.png
+-rw-rw-rw-   0        0        0     1004 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/plus_green.png
+-rw-rw-rw-   0        0        0     2402 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/point.png
+-rw-rw-rw-   0        0        0     4075 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/power.png
+-rw-rw-rw-   0        0        0     2708 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/presentation.png
+-rw-rw-rw-   0        0        0     3534 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/printer.png
+-rw-rw-rw-   0        0        0     1208 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/prompt.png
+-rw-rw-rw-   0        0        0     2848 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/puzzle.png
+-rw-rw-rw-   0        0        0     3046 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/qrcode.png
+-rw-rw-rw-   0        0        0     1800 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/record_mail.png
+-rw-rw-rw-   0        0        0     4501 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/recycle.png
+-rw-rw-rw-   0        0        0     4309 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/refresh.png
+-rw-rw-rw-   0        0        0     5443 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/registered.png
+-rw-rw-rw-   0        0        0     2582 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/repeat.png
+-rw-rw-rw-   0        0        0     2934 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/repeat_once.png
+-rw-rw-rw-   0        0        0     3597 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/replace.png
+-rw-rw-rw-   0        0        0     4342 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/rotate.png
+-rw-rw-rw-   0        0        0     3966 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/rotate_2.png
+-rw-rw-rw-   0        0        0     4334 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/rotate_clockwise.png
+-rw-rw-rw-   0        0        0     4017 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/rotate_clockwise_2.png
+-rw-rw-rw-   0        0        0     3008 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/rotate_rectangle.png
+-rw-rw-rw-   0        0        0     3880 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/route.png
+-rw-rw-rw-   0        0        0     4099 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/router.png
+-rw-rw-rw-   0        0        0     4103 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/rss.png
+-rw-rw-rw-   0        0        0     2384 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/ruler.png
+-rw-rw-rw-   0        0        0     3453 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/scale.png
+-rw-rw-rw-   0        0        0     2169 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/scan.png
+-rw-rw-rw-   0        0        0     3249 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/scissors.png
+-rw-rw-rw-   0        0        0     3948 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/search.png
+-rw-rw-rw-   0        0        0     1460 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/selector.png
+-rw-rw-rw-   0        0        0     3627 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/send.png
+-rw-rw-rw-   0        0        0      853 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/separator.png
+-rw-rw-rw-   0        0        0     3689 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/server.png
+-rw-rw-rw-   0        0        0     2059 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/servicemark.png
+-rw-rw-rw-   0        0        0     4623 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/settings.png
+-rw-rw-rw-   0        0        0     2160 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/shape.png
+-rw-rw-rw-   0        0        0     4054 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/share.png
+-rw-rw-rw-   0        0        0     4377 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/shield.png
+-rw-rw-rw-   0        0        0     4912 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/shield_check.png
+-rw-rw-rw-   0        0        0     5078 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/shield_x.png
+-rw-rw-rw-   0        0        0     2900 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/shopping_cart.png
+-rw-rw-rw-   0        0        0     2957 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/sitemap.png
+-rw-rw-rw-   0        0        0     3768 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/slideshow.png
+-rw-rw-rw-   0        0        0     3111 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/social.png
+-rw-rw-rw-   0        0        0     1983 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/sort_ascending.png
+-rw-rw-rw-   0        0        0     2027 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/sort_descending.png
+-rw-rw-rw-   0        0        0      935 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/space.png
+-rw-rw-rw-   0        0        0     1919 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/square.png
+-rw-rw-rw-   0        0        0     2664 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/square_check.png
+-rw-rw-rw-   0        0        0     2210 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/square_minus.png
+-rw-rw-rw-   0        0        0     2413 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/square_plus.png
+-rw-rw-rw-   0        0        0     2789 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/square_x.png
+-rw-rw-rw-   0        0        0     2173 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/stack.png
+-rw-rw-rw-   0        0        0     4785 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/star.png
+-rw-rw-rw-   0        0        0     4379 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/sticker.png
+-rw-rw-rw-   0        0        0     2789 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/strikethrough.png
+-rw-rw-rw-   0        0        0     2617 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/subscript.png
+-rw-rw-rw-   0        0        0     2687 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/superscript.png
+-rw-rw-rw-   0        0        0     2410 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/switch.png
+-rw-rw-rw-   0        0        0     1790 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/switch_horizontal.png
+-rw-rw-rw-   0        0        0     2016 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/switch_vertical.png
+-rw-rw-rw-   0        0        0     1968 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/table.png
+-rw-rw-rw-   0        0        0     2903 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/tag.png
+-rw-rw-rw-   0        0        0     6690 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/target.png
+-rw-rw-rw-   0        0        0     3594 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/tax.png
+-rw-rw-rw-   0        0        0     2588 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/template.png
+-rw-rw-rw-   0        0        0     1213 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/terminal.png
+-rw-rw-rw-   0        0        0     2898 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/terminal_2.png
+-rw-rw-rw-   0        0        0     2381 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/text_wrap.png
+-rw-rw-rw-   0        0        0     2707 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/ticket.png
+-rw-rw-rw-   0        0        0     4053 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/toggle_left.png
+-rw-rw-rw-   0        0        0     4077 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/toggle_right.png
+-rw-rw-rw-   0        0        0     3045 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/tool.png
+-rw-rw-rw-   0        0        0     3601 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/tools.png
+-rw-rw-rw-   0        0        0     2994 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/trash.png
+-rw-rw-rw-   0        0        0     4060 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/trees.png
+-rw-rw-rw-   0        0        0     1629 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/trending_down.png
+-rw-rw-rw-   0        0        0     1658 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/trending_up.png
+-rw-rw-rw-   0        0        0     2827 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/triangle.png
+-rw-rw-rw-   0        0        0     3275 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/trophy.png
+-rw-rw-rw-   0        0        0     2051 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/underline.png
+-rw-rw-rw-   0        0        0     4631 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/unlink.png
+-rw-rw-rw-   0        0        0     2204 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/upload.png
+-rw-rw-rw-   0        0        0     3148 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/urgent.png
+-rw-rw-rw-   0        0        0     3568 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/user.png
+-rw-rw-rw-   0        0        0     4047 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/user_check.png
+-rw-rw-rw-   0        0        0     4029 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/user_exclamation.png
+-rw-rw-rw-   0        0        0     3816 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/user_minus.png
+-rw-rw-rw-   0        0        0     4132 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/user_plus.png
+-rw-rw-rw-   0        0        0     4198 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/user_x.png
+-rw-rw-rw-   0        0        0     5017 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/users.png
+-rw-rw-rw-   0        0        0     5251 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/viewfinder.png
+-rw-rw-rw-   0        0        0     2214 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/viewport_narrow.png
+-rw-rw-rw-   0        0        0     2266 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/viewport_wide.png
+-rw-rw-rw-   0        0        0     4312 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/virus.png
+-rw-rw-rw-   0        0        0     4418 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/volume.png
+-rw-rw-rw-   0        0        0     3153 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/volume_2.png
+-rw-rw-rw-   0        0        0     2954 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/volume_3.png
+-rw-rw-rw-   0        0        0     2539 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/wallet.png
+-rw-rw-rw-   0        0        0     2761 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/wand.png
+-rw-rw-rw-   0        0        0     3742 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/wifi.png
+-rw-rw-rw-   0        0        0      549 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/wifi_0.png
+-rw-rw-rw-   0        0        0     1307 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/wifi_1.png
+-rw-rw-rw-   0        0        0     2399 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/wifi_2.png
+-rw-rw-rw-   0        0        0     3913 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/wind.png
+-rw-rw-rw-   0        0        0     2280 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/woman.png
+-rw-rw-rw-   0        0        0     5571 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/world.png
+-rw-rw-rw-   0        0        0     1505 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/x.png
+-rw-rw-rw-   0        0        0     6512 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/yin_yang.png
+-rw-rw-rw-   0        0        0     4478 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/zoom_in.png
+-rw-rw-rw-   0        0        0     4180 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/zoom_out.png
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/logo/
+-rw-rw-rw-   0        0        0   148555 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/logo/amulet_logo.png
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/
+-rw-rw-rw-   0        0        0      629 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_array.png
+-rw-rw-rw-   0        0        0      609 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_byte.png
+-rw-rw-rw-   0        0        0      664 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_compound.png
+-rw-rw-rw-   0        0        0      597 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_double.png
+-rw-rw-rw-   0        0        0      558 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_float.png
+-rw-rw-rw-   0        0        0      574 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_int.png
+-rw-rw-rw-   0        0        0      666 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_list.png
+-rw-rw-rw-   0        0        0      554 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_long.png
+-rw-rw-rw-   0        0        0      601 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_short.png
+-rw-rw-rw-   0        0        0      604 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_string.png
+-rw-rw-rw-   0        0        0     4503 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/lang.py
+-rw-rw-rw-   0        0        0      646 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/logging.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/
+-rw-rw-rw-   0        0        0      835 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/camera/
+-rw-rw-rw-   0        0        0      213 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/camera/__init__.py
+-rw-rw-rw-   0        0        0    12019 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/camera/camera.py
+-rw-rw-rw-   0        0        0     1356 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/camera/controllable_camera.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/canvas/
+-rw-rw-rw-   0        0        0       71 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/canvas/__init__.py
+-rw-rw-rw-   0        0        0     1898 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/canvas/canvas.py
+-rw-rw-rw-   0        0        0     2004 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/canvas/event_canvas.py
+-rw-rw-rw-   0        0        0      477 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/canvas_container.py
+-rw-rw-rw-   0        0        0      293 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/context_manager.py
+-rw-rw-rw-   0        0        0      229 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/data_types.py
+-rw-rw-rw-   0        0        0      289 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/drawable.py
+-rw-rw-rw-   0        0        0      308 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/events.py
+-rw-rw-rw-   0        0        0     1661 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/matrix.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/
+-rw-rw-rw-   0        0        0       64 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level/
+-rw-rw-rw-   0        0        0       32 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level/chunk/
+-rw-rw-rw-   0        0        0       32 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level/chunk/__init__.py
+-rw-rw-rw-   0        0        0    11030 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level/chunk/chunk.py
+-rw-rw-rw-   0        0        0    10527 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level/chunk/chunk_builder.py
+-rw-rw-rw-   0        0        0    11879 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level/level.py
+-rw-rw-rw-   0        0        0    11257 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level/region.py
+-rw-rw-rw-   0        0        0      468 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level/selection.py
+-rw-rw-rw-   0        0        0     7037 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level_group.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/
+-rw-rw-rw-   0        0        0      165 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/box/
+-rw-rw-rw-   0        0        0      185 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/box/__init__.py
+-rw-rw-rw-   0        0        0      243 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/box/colours.json
+-rw-rw-rw-   0        0        0      506 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/box/colours.py
+-rw-rw-rw-   0        0        0     9498 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/box/render_selection.py
+-rw-rw-rw-   0        0        0    11559 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/box/render_selection_editable.py
+-rw-rw-rw-   0        0        0     1921 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/box/render_selection_highlightable.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/group/
+-rw-rw-rw-   0        0        0      143 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/group/__init__.py
+-rw-rw-rw-   0        0        0     2243 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/group/render_selection_group.py
+-rw-rw-rw-   0        0        0      914 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/group/render_selection_group_highlightable.py
+-rw-rw-rw-   0        0        0     2881 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/sky_box.py
+-rw-rw-rw-   0        0        0     6237 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/tri_mesh.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/resource_pack/
+-rw-rw-rw-   0        0        0      158 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/resource_pack/__init__.py
+-rw-rw-rw-   0        0        0     6890 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/resource_pack/resource_pack.py
+-rw-rw-rw-   0        0        0     1166 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/resource_pack/resource_pack_manager.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/shaders/
+-rw-rw-rw-   0        0        0     2196 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/shaders/__init__.py
+-rw-rw-rw-   0        0        0      436 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/shaders/render_chunk_120.frag
+-rw-rw-rw-   0        0        0      504 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/shaders/render_chunk_120.vert
+-rw-rw-rw-   0        0        0      437 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/shaders/render_chunk_330.frag
+-rw-rw-rw-   0        0        0      437 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/shaders/render_chunk_330.vert
+-rw-rw-rw-   0        0        0    10315 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/textureatlas.py
+-rw-rw-rw-   0        0        0     1930 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/thread_generator.py
+-rw-rw-rw-   0        0        0     3099 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/resources.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/
+-rw-rw-rw-   0        0        0        0 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/
+-rw-rw-rw-   0        0        0        0 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/__init__.py
+-rw-rw-rw-   0        0        0     3361 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/base_define.py
+-rw-rw-rw-   0        0        0     7850 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/base_select.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/biome_select/
+-rw-rw-rw-   0        0        0       39 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/biome_select/__init__.py
+-rw-rw-rw-   0        0        0     1967 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/biome_select/biome_define.py
+-rw-rw-rw-   0        0        0      920 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/biome_select/biome_select.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/block_select/
+-rw-rw-rw-   0        0        0      191 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/block_select/__init__.py
+-rw-rw-rw-   0        0        0     5646 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/block_select/block_define.py
+-rw-rw-rw-   0        0        0     1804 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/block_select/block_select.py
+-rw-rw-rw-   0        0        0     6907 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/block_select/multi_block_define.py
+-rw-rw-rw-   0        0        0    13667 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/block_select/properties.py
+-rw-rw-rw-   0        0        0    14216 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/nbt_editor.py
+-rw-rw-rw-   0        0        0    12102 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/select_world.py
+-rw-rw-rw-   0        0        0     5947 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/simple.py
+-rw-rw-rw-   0        0        0     2706 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/traceback_dialog.py
+-rw-rw-rw-   0        0        0     9009 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/version_select.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/util/
+-rw-rw-rw-   0        0        0        0 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/util/__init__.py
+-rw-rw-rw-   0        0        0     9141 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/util/button_input.py
+-rw-rw-rw-   0        0        0    16783 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/util/key_config.py
+-rw-rw-rw-   0        0        0     5204 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/util/mouse_movement.py
+-rw-rw-rw-   0        0        0     2350 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/util/ui_preferences.py
+-rw-rw-rw-   0        0        0     1062 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/util/validators.py
+-rw-rw-rw-   0        0        0      457 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/api/wx/util/window_container.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/lang/
+-rw-rw-rw-   0        0        0    16234 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/lang/cs.lang
+-rw-rw-rw-   0        0        0    14748 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/lang/de.lang
+-rw-rw-rw-   0        0        0    15730 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/lang/en.lang
+-rw-rw-rw-   0        0        0    17293 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/lang/fr.lang
+-rw-rw-rw-   0        0        0    13212 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/lang/id.lang
+-rw-rw-rw-   0        0        0    18609 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/lang/ja.lang
+-rw-rw-rw-   0        0        0    14396 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/lang/ko.lang
+-rw-rw-rw-   0        0        0    22815 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/lang/ru.lang
+-rw-rw-rw-   0        0        0    18106 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/lang/vi.lang
+-rw-rw-rw-   0        0        0    13331 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/lang/zh_CN.lang
+-rw-rw-rw-   0        0        0    12652 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/lang/zh_TW.lang
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/
+-rw-rw-rw-   0        0        0        0 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/convert/
+-rw-rw-rw-   0        0        0      158 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/convert/__init__.py
+-rw-rw-rw-   0        0        0     6439 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/convert/convert.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/
+-rw-rw-rw-   0        0        0      255 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/
+-rw-rw-rw-   0        0        0     6950 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/down.png
+-rw-rw-rw-   0        0        0    36091 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/east.png
+-rw-rw-rw-   0        0        0    29789 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/north.png
+-rw-rw-rw-   0        0        0    41677 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/south.png
+-rw-rw-rw-   0        0        0    36204 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/up.png
+-rw-rw-rw-   0        0        0    36917 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/west.png
+-rw-rw-rw-   0        0        0     1292 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/selection.png
+-rw-rw-rw-   0        0        0     1383 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/translucent_white.png
+-rw-rw-rw-   0        0        0      540 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/manifest.json
+-rw-rw-rw-   0        0        0     1337 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/pack_icon.png
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/textures/
+-rw-rw-rw-   0        0        0      340 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/textures/terrain_texture.json
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/
+-rw-rw-rw-   0        0        0     6950 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/down.png
+-rw-rw-rw-   0        0        0    36091 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/east.png
+-rw-rw-rw-   0        0        0    29789 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/north.png
+-rw-rw-rw-   0        0        0    41677 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/south.png
+-rw-rw-rw-   0        0        0    36204 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/up.png
+-rw-rw-rw-   0        0        0    36917 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/west.png
+-rw-rw-rw-   0        0        0     1292 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/selection.png
+-rw-rw-rw-   0        0        0     1383 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/translucent_white.png
+-rw-rw-rw-   0        0        0       94 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/pack.mcmeta
+-rw-rw-rw-   0        0        0     1337 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/pack.png
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/
+-rw-rw-rw-   0        0        0       88 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/
+-rw-rw-rw-   0        0        0      536 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/__init__.py
+-rw-rw-rw-   0        0        0      611 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/base_behaviour.py
+-rw-rw-rw-   0        0        0    22005 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/block_selection_behaviour.py
+-rw-rw-rw-   0        0        0     7819 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/camera_behaviour.py
+-rw-rw-rw-   0        0        0     6820 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/chunk_selection_behaviour.py
+-rw-rw-rw-   0        0        0     4184 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/inspect_block_behaviour.py
+-rw-rw-rw-   0        0        0     3377 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/pointer_behaviour.py
+-rw-rw-rw-   0        0        0     9545 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/raycast_behaviour.py
+-rw-rw-rw-   0        0        0     1415 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/static_selection_behaviour.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/canvas/
+-rw-rw-rw-   0        0        0       37 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/canvas/__init__.py
+-rw-rw-rw-   0        0        0    11000 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/canvas/base_edit_canvas.py
+-rw-rw-rw-   0        0        0    11712 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/canvas/edit_canvas.py
+-rw-rw-rw-   0        0        0     1238 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/chunk_generator.py
+-rw-rw-rw-   0        0        0      554 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/edit_canvas_container.py
+-rw-rw-rw-   0        0        0     1061 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/events.py
+-rw-rw-rw-   0        0        0     4661 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/key_config.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/
+-rw-rw-rw-   0        0        0      256 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/base/
+-rw-rw-rw-   0        0        0      110 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/base/__init__.py
+-rw-rw-rw-   0        0        0     2420 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/base/default_operation_ui.py
+-rw-rw-rw-   0        0        0     3192 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/base/operation_ui.py
+-rw-rw-rw-   0        0        0      956 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/errors.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/manager/
+-rw-rw-rw-   0        0        0      189 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/manager/loader/
+-rw-rw-rw-   0        0        0      155 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/manager/loader/__init__.py
+-rw-rw-rw-   0        0        0     1735 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/manager/loader/base_operation_loader.py
+-rw-rw-rw-   0        0        0     1588 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/manager/loader/operation_loader.py
+-rw-rw-rw-   0        0        0     3643 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/manager/loader/ui_operation_loader.py
+-rw-rw-rw-   0        0        0     5907 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/manager/operation_manager.py
+-rw-rw-rw-   0        0        0      356 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/manager/util.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/ui/
+-rw-rw-rw-   0        0        0        0 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/ui/__init__.py
+-rw-rw-rw-   0        0        0     8343 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/ui/fixed_pipeline.py
+-rw-rw-rw-   0        0        0     1495 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/ui/simple_operation_panel.py
+-rw-rw-rw-   0        0        0     8718 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/renderer.py
+-rw-rw-rw-   0        0        0     5795 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/selection.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/
+-rw-rw-rw-   0        0        0        2 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/__init__.py
+-rw-rw-rw-   0        0        0      839 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/canvas_toggle_element.py
+-rw-rw-rw-   0        0        0     6779 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/file.py
+-rw-rw-rw-   0        0        0     4790 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/goto.py
+-rw-rw-rw-   0        0        0     3507 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/nudge_button.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/select_location/
+-rw-rw-rw-   0        0        0      326 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/select_location/__init__.py
+-rw-rw-rw-   0        0        0     3062 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/select_location/events.py
+-rw-rw-rw-   0        0        0     4202 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/select_location/select_location.py
+-rw-rw-rw-   0        0        0     2995 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/select_location/select_transform.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/tool/
+-rw-rw-rw-   0        0        0      153 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/tool/__init__.py
+-rw-rw-rw-   0        0        0     6306 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/tool/base_operation_choice.py
+-rw-rw-rw-   0        0        0     1162 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/tool/base_tool_ui.py
+-rw-rw-rw-   0        0        0     3174 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/tool/default_base_tool_ui.py
+-rw-rw-rw-   0        0        0     4614 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/tool_manager.py
+-rw-rw-rw-   0        0        0    12624 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/edit.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/
+-rw-rw-rw-   0        0        0        0 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/
+-rw-rw-rw-   0        0        0        0 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/examples/
+-rw-rw-rw-   0        0        0     1251 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/examples/1_fixed_function_pipeline.py
+-rw-rw-rw-   0        0        0     1148 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/examples/2_fixed_function_pipeline.py
+-rw-rw-rw-   0        0        0     3420 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/examples/3_fixed_function_pipeline.py
+-rw-rw-rw-   0        0        0        0 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/
+-rw-rw-rw-   0        0        0        0 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/
+-rw-rw-rw-   0        0        0        0 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/__init__.py
+-rw-rw-rw-   0        0        0     3717 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/construction.py
+-rw-rw-rw-   0        0        0     3929 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/mcstructure.py
+-rw-rw-rw-   0        0        0     4303 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/schematic.py
+-rw-rw-rw-   0        0        0     3926 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/sponge_schematic.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/
+-rw-rw-rw-   0        0        0       74 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/__init__.py
+-rw-rw-rw-   0        0        0      896 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/copy.py
+-rw-rw-rw-   0        0        0      973 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/cut.py
+-rw-rw-rw-   0        0        0      801 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/delete.py
+-rw-rw-rw-   0        0        0      865 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/prune_chunks.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/
+-rw-rw-rw-   0        0        0        0 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/__init__.py
+-rw-rw-rw-   0        0        0     1204 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/clone.py
+-rw-rw-rw-   0        0        0     3198 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/fill.py
+-rw-rw-rw-   0        0        0     7354 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/replace.py
+-rw-rw-rw-   0        0        0     6007 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/set_biome.py
+-rw-rw-rw-   0        0        0    10932 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/waterlog.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/tools/
+-rw-rw-rw-   0        0        0      204 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/tools/__init__.py
+-rw-rw-rw-   0        0        0    10143 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/tools/chunk.py
+-rw-rw-rw-   0        0        0      249 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/tools/export_tool.py
+-rw-rw-rw-   0        0        0     2945 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/tools/import_tool.py
+-rw-rw-rw-   0        0        0      248 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/tools/operation.py
+-rw-rw-rw-   0        0        0    23618 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/tools/paste.py
+-rw-rw-rw-   0        0        0    13768 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/tools/select.py
+drwxrwxrwx   0        0        0        0 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor.egg-info/
+-rw-rw-rw-   0        0        0      429 2022-06-21 09:03:45.000000 amulet-map-editor-0.9.6/amulet_map_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    34995 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      190 2022-06-21 09:03:45.000000 amulet-map-editor-0.9.6/amulet_map_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2022-06-21 09:03:46.000000 amulet-map-editor-0.9.6/amulet_map_editor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4076 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/icon.ico
+-rw-rw-rw-   0        0        0      175 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/pyproject.toml
+-rw-rw-rw-   0        0        0      263 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/requirements.txt
+-rw-rw-rw-   0        0        0      925 2022-06-21 09:03:47.000000 amulet-map-editor-0.9.6/setup.cfg
+-rw-rw-rw-   0        0        0     4441 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/setup.py
+-rw-rw-rw-   0        0        0    70636 2022-06-21 09:02:52.000000 amulet-map-editor-0.9.6/versioneer.py
```

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/__main__.py` & `amulet-map-editor-0.9.6/amulet_map_editor/__main__.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/_version.py` & `amulet-map-editor-0.9.6/amulet_map_editor/_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 
 version_json = '''
 {
  "date": "2022-05-24T09:05:37+0100",
  "dirty": false,
  "error": null,
  "full-revisionid": "9e4adb214a4f2040a89ee3c0a77b60ba818399c6",
- "version": "0.9.5"
+ "version": "0.9.6"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/config.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/config.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/framework/amulet_ui.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/framework/amulet_ui.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/framework/app.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/framework/app.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/framework/pages/main_menu.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/framework/pages/main_menu.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/framework/pages/world_page.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/framework/pages/world_page.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/framework/programs/about_program.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/framework/programs/about_program.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/framework/programs/base_program.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/framework/programs/base_program.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/framework/update_check.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/framework/update_check.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/__init__.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/__init__.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/accessible.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/accessible.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/adjustments.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/adjustments.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/alert_circle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/alert_circle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/alert_triangle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/alert_triangle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/align_center.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/align_center.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/align_justified.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/align_justified.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/align_left.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/align_left.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/align_right.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/align_right.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/anchor.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/anchor.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/aperture.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/aperture.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/apps.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/apps.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/archive.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/archive.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_back.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_back.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_back_up.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_back_up.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_bar_down.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_bar_down.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_bar_left.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_bar_left.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_bar_right.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_bar_right.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_bar_up.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_bar_up.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_down.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_down.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_down_circle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_down_circle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_down_left.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_down_left.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_down_left_circle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_down_left_circle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_down_right.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_down_right.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_down_right_circle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_down_right_circle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_forward.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_forward.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_forward_up.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_forward_up.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_left.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_left.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_left_circle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_left_circle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_down.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_down.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_left.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_left.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_right.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_right.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_up.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_narrow_up.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_right.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_right.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_right_circle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_right_circle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_up.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_up.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_up_circle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_up_circle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_up_left.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_up_left.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_up_left_circle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_up_left_circle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_up_right.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_up_right.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrow_up_right_circle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrow_up_right_circle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrows_diagonal.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrows_diagonal.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrows_diagonal_2.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrows_diagonal_2.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrows_horizontal.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrows_horizontal.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrows_maximize.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrows_maximize.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrows_minimize.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrows_minimize.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrows_sort.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrows_sort.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/arrows_vertical.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/arrows_vertical.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/artboard.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/artboard.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/at.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/at.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/award.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/award.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/backspace.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/backspace.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/box.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/box.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/braces.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/braces.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/brackets.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/brackets.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/caret_down.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/caret_down.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/caret_left.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/caret_left.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/caret_right.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/caret_right.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/caret_up.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/caret_up.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/check.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/check.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/checkbox.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/checkbox.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/checks.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/checks.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevron_down.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevron_down.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevron_left.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevron_left.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevron_right.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevron_right.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevron_up.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevron_up.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevrons_down.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevrons_down.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevrons_left.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevrons_left.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevrons_right.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevrons_right.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/chevrons_up.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/chevrons_up.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/circle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/circle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/circle_check.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/circle_check.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/circle_minus.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/circle_minus.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/circle_plus.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/circle_plus.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/circle_x.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/circle_x.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/click.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/click.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/clipboard.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/clipboard.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/clipboard_check.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/clipboard_check.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/clipboard_list.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/clipboard_list.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/clipboard_x.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/clipboard_x.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/clock.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/clock.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/cloud.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/cloud.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/cloud_download.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/cloud_download.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/cloud_upload.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/cloud_upload.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/code.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/code.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/color_picker.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/color_picker.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/color_swatch.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/color_swatch.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/command.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/command.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/copy.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/copy.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/copyright.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/copyright.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_down_left.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_down_left.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_down_right.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_down_right.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_left_down.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_left_down.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_left_up.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_left_up.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_right_down.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_right_down.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_right_up.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_right_up.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_up_left.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_up_left.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/corner_up_right.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/corner_up_right.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/crop.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/crop.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/cut.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/cut.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/dashboard.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/dashboard.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/database.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/database.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_desktop.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_desktop.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_floppy.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_floppy.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_gamepad.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_gamepad.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_laptop.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_laptop.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_mobile.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_mobile.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_tablet.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_tablet.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_tv.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_tv.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/device_watch.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/device_watch.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/devices.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/devices.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/direction.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/direction.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/direction_horizontal.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/direction_horizontal.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/dots.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/dots.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/dots_circle_horizontal.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/dots_circle_horizontal.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/dots_diagonal.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/dots_diagonal.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/dots_diagonal_2.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/dots_diagonal_2.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/dots_vertical.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/dots_vertical.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/download.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/download.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/drag_drop.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/drag_drop.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/drag_drop_2.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/drag_drop_2.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/edit.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/edit.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/eraser.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/eraser.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/exchange.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/exchange.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/external_link.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/external_link.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_check.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_check.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_code.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_code.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_download.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_download.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_horizontal.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_horizontal.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_invoice.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_invoice.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_minus.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_minus.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_music.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_music.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_plus.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_plus.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_shredder.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_shredder.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_text.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_text.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/file_x.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/file_x.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/filter.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/filter.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/flag.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/flag.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/flame.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/flame.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/flask.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/flask.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/flip_horizontal.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/flip_horizontal.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/flip_vertical.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/flip_vertical.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/floppy_disk.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/floppy_disk.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/focus.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/focus.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/focus_2.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/focus_2.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/folder.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/folder.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/folder_minus.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/folder_minus.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/folder_plus.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/folder_plus.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/folder_x.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/folder_x.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/folders.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/folders.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/forbid.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/forbid.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/forbid_2.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/forbid_2.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/frame.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/frame.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/friends.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/friends.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/gift.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/gift.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/git_branch.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/git_branch.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/git_commit.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/git_commit.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/git_compare.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/git_compare.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/git_fork.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/git_fork.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/git_merge.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/git_merge.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/git_pull_request.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/git_pull_request.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/grid.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/grid.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/grid_dots.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/grid_dots.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/grip_horizontal.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/grip_horizontal.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/grip_vertical.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/grip_vertical.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/hand_stop.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/hand_stop.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/hash.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/hash.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/help.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/help.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/hexagon.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/hexagon.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/history.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/history.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/home.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/home.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/home_2.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/home_2.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/indent_decrease.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/indent_decrease.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/indent_increase.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/indent_increase.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/infinity.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/infinity.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/info_circle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/info_circle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/info_square.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/info_square.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/keyboard.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/keyboard.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/language.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/language.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layers_difference.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layers_difference.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layers_intersect.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layers_intersect.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layers_subtract.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layers_subtract.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layers_union.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layers_union.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_2.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_2.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_align_bottom.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_align_bottom.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_align_center.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_align_center.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_align_left.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_align_left.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_align_middle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_align_middle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_align_right.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_align_right.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_align_top.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_align_top.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_bottombar.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_bottombar.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_cards.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_cards.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_columns.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_columns.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_distribute_horizontal.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_distribute_horizontal.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_distribute_vertical.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_distribute_vertical.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_list.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_list.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_navbar.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_navbar.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_rows.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_rows.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_sidebar.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_sidebar.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/layout_sidebar_right.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/layout_sidebar_right.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/license.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/license.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/line_height.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/line_height.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/link.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/link.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/list.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/list.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/list_check.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/list_check.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/location.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/location.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/lock.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/lock.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/lock_open.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/lock_open.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/login.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/login.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/logout.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/logout.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/magnet.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/magnet.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/mail.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/mail.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/mail_opened.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/mail_opened.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/man.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/man.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/map.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/map.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/map_2.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/map_2.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/map_pin.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/map_pin.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/math.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/math.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/maximize.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/maximize.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/medical_cross.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/medical_cross.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/menu.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/menu.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/message.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/message.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/message_2.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/message_2.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/message_circle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/message_circle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/message_dots.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/message_dots.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/messages.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/messages.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/microphone.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/microphone.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/minimize.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/minimize.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/minus.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/minus.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/minus_red.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/minus_red.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/mist.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/mist.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/mouse.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/mouse.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/movie.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/movie.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/mug.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/mug.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/music.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/music.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/new_section.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/new_section.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/news.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/news.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/note.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/note.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/notebook.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/notebook.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/notes.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/notes.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/notification.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/notification.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/outlet.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/outlet.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/package.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/package.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/paint.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/paint.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/palette.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/palette.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/paperclip.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/paperclip.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/parentheses.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/parentheses.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/pencil.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/pencil.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/photo.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/photo.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/plug.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/plug.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/plus.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/plus.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/plus_green.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/plus_green.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/point.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/point.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/power.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/power.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/presentation.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/presentation.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/printer.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/printer.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/prompt.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/prompt.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/puzzle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/puzzle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/qrcode.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/qrcode.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/record_mail.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/record_mail.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/recycle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/recycle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/refresh.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/refresh.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/registered.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/registered.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/repeat.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/repeat.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/repeat_once.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/repeat_once.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/replace.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/replace.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/rotate.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/rotate.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/rotate_2.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/rotate_2.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/rotate_clockwise.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/rotate_clockwise.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/rotate_clockwise_2.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/rotate_clockwise_2.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/rotate_rectangle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/rotate_rectangle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/route.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/route.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/router.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/router.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/rss.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/rss.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/ruler.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/ruler.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/scale.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/scale.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/scan.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/scan.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/scissors.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/scissors.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/search.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/search.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/selector.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/selector.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/send.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/send.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/separator.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/separator.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/server.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/server.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/servicemark.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/servicemark.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/settings.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/settings.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/shape.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/shape.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/share.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/share.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/shield.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/shield.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/shield_check.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/shield_check.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/shield_x.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/shield_x.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/shopping_cart.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/shopping_cart.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/sitemap.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/sitemap.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/slideshow.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/slideshow.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/social.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/social.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/sort_ascending.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/sort_ascending.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/sort_descending.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/sort_descending.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/space.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/space.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/square.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/square.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/square_check.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/square_check.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/square_minus.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/square_minus.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/square_plus.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/square_plus.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/square_x.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/square_x.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/stack.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/stack.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/star.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/star.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/sticker.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/sticker.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/strikethrough.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/strikethrough.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/subscript.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/subscript.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/superscript.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/superscript.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/switch.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/switch.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/switch_horizontal.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/switch_horizontal.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/switch_vertical.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/switch_vertical.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/table.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/table.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/tag.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/tag.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/target.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/target.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/tax.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/tax.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/template.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/template.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/terminal.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/terminal.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/terminal_2.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/terminal_2.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/text_wrap.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/text_wrap.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/ticket.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/ticket.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/toggle_left.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/toggle_left.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/toggle_right.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/toggle_right.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/tool.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/tool.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/tools.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/tools.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/trash.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/trash.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/trees.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/trees.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/trending_down.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/trending_down.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/trending_up.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/trending_up.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/triangle.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/triangle.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/trophy.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/trophy.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/underline.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/underline.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/unlink.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/unlink.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/upload.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/upload.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/urgent.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/urgent.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/user.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/user.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/user_check.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/user_check.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/user_exclamation.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/user_exclamation.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/user_minus.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/user_minus.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/user_plus.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/user_plus.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/user_x.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/user_x.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/users.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/users.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/viewfinder.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/viewfinder.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/viewport_narrow.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/viewport_narrow.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/viewport_wide.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/viewport_wide.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/virus.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/virus.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/volume.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/volume.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/volume_2.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/volume_2.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/volume_3.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/volume_3.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/wallet.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/wallet.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/wand.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/wand.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/wifi.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/wifi.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/wifi_0.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/wifi_0.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/wifi_1.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/wifi_1.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/wifi_2.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/wifi_2.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/wind.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/wind.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/woman.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/woman.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/world.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/world.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/x.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/x.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/yin_yang.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/yin_yang.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/zoom_in.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/zoom_in.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/icon/tablericons/zoom_out.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/icon/tablericons/zoom_out.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/logo/amulet_logo.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/logo/amulet_logo.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_array.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_array.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_byte.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_byte.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_compound.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_compound.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_double.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_double.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_float.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_float.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_int.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_int.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_list.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_list.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_long.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_long.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_short.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_short.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/image/nbt/nbt_tag_string.png` & `amulet-map-editor-0.9.6/amulet_map_editor/api/image/nbt/nbt_tag_string.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/lang.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/lang.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/logging.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/logging.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/__init__.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/__init__.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/camera/camera.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/camera/camera.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/camera/controllable_camera.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/camera/controllable_camera.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/canvas/canvas.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/canvas/event_canvas.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/canvas/event_canvas.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/matrix.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/matrix.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level/chunk/chunk.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level/chunk/chunk.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level/chunk/chunk_builder.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level/chunk/chunk_builder.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level/level.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level/level.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level/region.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level/region.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/level_group.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/level_group.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/box/render_selection.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/box/render_selection.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/box/render_selection_editable.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/box/render_selection_editable.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/box/render_selection_highlightable.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/box/render_selection_highlightable.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/group/render_selection_group.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/group/render_selection_group.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/selection/group/render_selection_group_highlightable.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/selection/group/render_selection_group_highlightable.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/sky_box.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/sky_box.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/mesh/tri_mesh.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/mesh/tri_mesh.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/resource_pack/resource_pack.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/resource_pack/resource_pack.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/resource_pack/resource_pack_manager.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/resource_pack/resource_pack_manager.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/shaders/__init__.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/shaders/__init__.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/textureatlas.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/textureatlas.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/opengl/thread_generator.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/opengl/thread_generator.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/resources.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/resources.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/base_define.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/base_define.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/base_select.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/base_select.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/biome_select/biome_define.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/biome_select/biome_define.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/biome_select/biome_select.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/biome_select/biome_select.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/block_select/block_define.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/block_select/block_define.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/block_select/block_select.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/block_select/block_select.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/block_select/multi_block_define.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/block_select/multi_block_define.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/block_select/properties.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/block_select/properties.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/nbt_editor.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/nbt_editor.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/select_world.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/select_world.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/simple.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/simple.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/traceback_dialog.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/traceback_dialog.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/ui/version_select.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/ui/version_select.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/util/button_input.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/util/button_input.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/util/key_config.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/util/key_config.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/util/mouse_movement.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/util/mouse_movement.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/util/ui_preferences.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/util/ui_preferences.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/api/wx/util/validators.py` & `amulet-map-editor-0.9.6/amulet_map_editor/api/wx/util/validators.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/lang/cs.lang` & `amulet-map-editor-0.9.6/amulet_map_editor/lang/cs.lang`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/lang/de.lang` & `amulet-map-editor-0.9.6/amulet_map_editor/lang/de.lang`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/lang/en.lang` & `amulet-map-editor-0.9.6/amulet_map_editor/lang/en.lang`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/lang/fr.lang` & `amulet-map-editor-0.9.6/amulet_map_editor/lang/fr.lang`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/lang/id.lang` & `amulet-map-editor-0.9.6/amulet_map_editor/lang/id.lang`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/lang/ja.lang` & `amulet-map-editor-0.9.6/amulet_map_editor/lang/ja.lang`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/lang/ko.lang` & `amulet-map-editor-0.9.6/amulet_map_editor/lang/ko.lang`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/lang/ru.lang` & `amulet-map-editor-0.9.6/amulet_map_editor/lang/ru.lang`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/lang/vi.lang` & `amulet-map-editor-0.9.6/amulet_map_editor/lang/vi.lang`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/lang/zh_CN.lang` & `amulet-map-editor-0.9.6/amulet_map_editor/lang/zh_CN.lang`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/lang/zh_TW.lang` & `amulet-map-editor-0.9.6/amulet_map_editor/lang/zh_TW.lang`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/convert/convert.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/convert/convert.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/down.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/down.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/east.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/east.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/north.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/north.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/south.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/south.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/up.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/up.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/west.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/cubemap/west.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/selection.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/selection.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/translucent_white.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/amulet_ui/translucent_white.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/manifest.json` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/manifest.json`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/pack_icon.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/bedrock/pack_icon.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/down.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/down.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/east.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/east.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/north.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/north.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/south.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/south.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/up.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/up.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/west.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/cubemap/west.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/selection.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/selection.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/translucent_white.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/assets/amulet/textures/amulet_ui/translucent_white.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/amulet_resource_pack/java/pack.png` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/amulet_resource_pack/java/pack.png`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/__init__.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/__init__.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/base_behaviour.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/base_behaviour.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/block_selection_behaviour.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/block_selection_behaviour.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/camera_behaviour.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/camera_behaviour.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/chunk_selection_behaviour.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/chunk_selection_behaviour.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/inspect_block_behaviour.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/inspect_block_behaviour.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/pointer_behaviour.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/pointer_behaviour.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/raycast_behaviour.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/raycast_behaviour.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/behaviour/static_selection_behaviour.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/behaviour/static_selection_behaviour.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/canvas/base_edit_canvas.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/canvas/base_edit_canvas.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/canvas/edit_canvas.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/canvas/edit_canvas.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/chunk_generator.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/chunk_generator.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/edit_canvas_container.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/edit_canvas_container.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/events.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/events.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/key_config.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/key_config.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/base/default_operation_ui.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/base/default_operation_ui.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/base/operation_ui.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/base/operation_ui.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/errors.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/errors.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/manager/loader/base_operation_loader.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/manager/loader/base_operation_loader.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/manager/loader/operation_loader.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/manager/loader/operation_loader.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/manager/loader/ui_operation_loader.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/manager/loader/ui_operation_loader.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/manager/operation_manager.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/manager/operation_manager.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/ui/fixed_pipeline.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/ui/fixed_pipeline.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/operations/ui/simple_operation_panel.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/operations/ui/simple_operation_panel.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/renderer.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/renderer.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/selection.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/selection.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/canvas_toggle_element.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/canvas_toggle_element.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/file.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/file.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/goto.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/goto.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/nudge_button.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/nudge_button.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/select_location/events.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/select_location/events.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/select_location/select_location.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/select_location/select_location.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/select_location/select_transform.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/select_location/select_transform.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/tool/base_operation_choice.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/tool/base_operation_choice.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/tool/base_tool_ui.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/tool/base_tool_ui.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/tool/default_base_tool_ui.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/tool/default_base_tool_ui.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/api/ui/tool_manager.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/api/ui/tool_manager.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/edit.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/edit.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/examples/1_fixed_function_pipeline.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/examples/1_fixed_function_pipeline.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/examples/2_fixed_function_pipeline.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/examples/2_fixed_function_pipeline.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/examples/3_fixed_function_pipeline.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/examples/3_fixed_function_pipeline.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/construction.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/construction.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/mcstructure.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/mcstructure.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/schematic.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/schematic.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/sponge_schematic.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/export_operations/sponge_schematic.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/copy.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/copy.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/cut.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/cut.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/delete.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/delete.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/prune_chunks.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/internal_operations/prune_chunks.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/clone.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/clone.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/fill.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/fill.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/replace.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/replace.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/set_biome.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/set_biome.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/waterlog.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/operations/stock_plugins/operations/waterlog.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/tools/chunk.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/tools/chunk.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/tools/import_tool.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/tools/import_tool.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/tools/paste.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/tools/paste.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor/programs/edit/plugins/tools/select.py` & `amulet-map-editor-0.9.6/amulet_map_editor/programs/edit/plugins/tools/select.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/amulet_map_editor.egg-info/SOURCES.txt` & `amulet-map-editor-0.9.6/amulet_map_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/icon.ico` & `amulet-map-editor-0.9.6/icon.ico`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/setup.cfg` & `amulet-map-editor-0.9.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/setup.py` & `amulet-map-editor-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `amulet-map-editor-0.9.5/versioneer.py` & `amulet-map-editor-0.9.6/versioneer.py`

 * *Files identical despite different names*

