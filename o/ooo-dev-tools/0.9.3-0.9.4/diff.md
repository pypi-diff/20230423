# Comparing `tmp/ooo_dev_tools-0.9.3.tar.gz` & `tmp/ooo_dev_tools-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooo_dev_tools-0.9.3.tar", max compression
+gzip compressed data, was "ooo_dev_tools-0.9.4.tar", max compression
```

## Comparing `ooo_dev_tools-0.9.3.tar` & `ooo_dev_tools-0.9.4.tar`

### file list

```diff
@@ -1,805 +1,985 @@
--rw-r--r--   0        0        0    10174 2022-06-09 05:52:04.135315 ooo_dev_tools-0.9.3/LICENSE
--rw-r--r--   0        0        0      272 2023-04-07 18:11:57.908882 ooo_dev_tools-0.9.3/ooodev/__init__.py
--rw-r--r--   0        0        0        0 2022-11-29 00:27:48.235332 ooo_dev_tools-0.9.3/ooodev/adapter/__init__.py
--rw-r--r--   0        0        0     1806 2022-11-29 00:27:48.236329 ooo_dev_tools-0.9.3/ooodev/adapter/adapter_base.py
--rw-r--r--   0        0        0        0 2022-11-29 00:27:48.236329 ooo_dev_tools-0.9.3/ooodev/adapter/awt/__init__.py
--rw-r--r--   0        0        0     3451 2022-12-03 04:37:37.329802 ooo_dev_tools-0.9.3/ooodev/adapter/awt/top_window_listener.py
--rw-r--r--   0        0        0        0 2022-11-29 00:27:48.238329 ooo_dev_tools-0.9.3/ooodev/adapter/frame/__init__.py
--rw-r--r--   0        0        0     2711 2022-12-03 04:37:37.330805 ooo_dev_tools-0.9.3/ooodev/adapter/frame/terminate_listener.py
--rw-r--r--   0        0        0        0 2022-11-29 00:27:48.239328 ooo_dev_tools-0.9.3/ooodev/adapter/lang/__init__.py
--rw-r--r--   0        0        0     1543 2022-12-03 04:37:37.330805 ooo_dev_tools-0.9.3/ooodev/adapter/lang/event_listener.py
--rw-r--r--   0        0        0        0 2022-11-29 00:27:48.240329 ooo_dev_tools-0.9.3/ooodev/adapter/util/__init__.py
--rw-r--r--   0        0        0     2336 2022-12-03 04:37:37.331804 ooo_dev_tools-0.9.3/ooodev/adapter/util/modify_listener.py
--rw-r--r--   0        0        0        0 2022-11-29 00:27:48.241329 ooo_dev_tools-0.9.3/ooodev/adapter/view/__init__.py
--rw-r--r--   0        0        0     2628 2023-04-06 02:13:08.626094 ooo_dev_tools-0.9.3/ooodev/adapter/view/selection_change_listener.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.785323 ooo_dev_tools-0.9.3/ooodev/cfg/__init__.py
--rw-r--r--   0        0        0       89 2022-10-27 15:27:12.042995 ooo_dev_tools-0.9.3/ooodev/cfg/config.json
--rw-r--r--   0        0        0     2012 2022-10-27 15:27:12.042995 ooo_dev_tools-0.9.3/ooodev/cfg/config.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.786382 ooo_dev_tools-0.9.3/ooodev/conn/__init__.py
--rw-r--r--   0        0        0     5699 2022-07-14 20:40:23.787320 ooo_dev_tools-0.9.3/ooodev/conn/cache.py
--rw-r--r--   0        0        0    18466 2023-04-06 02:13:08.627093 ooo_dev_tools-0.9.3/ooodev/conn/connect.py
--rw-r--r--   0        0        0     6968 2022-12-20 23:59:58.431481 ooo_dev_tools-0.9.3/ooodev/conn/connectors.py
--rw-r--r--   0        0        0        0 2022-10-27 15:27:12.043993 ooo_dev_tools-0.9.3/ooodev/dialog/__init__.py
--rw-r--r--   0        0        0     3161 2022-11-05 19:29:24.377395 ooo_dev_tools-0.9.3/ooodev/dialog/input.py
--rw-r--r--   0        0        0     2297 2022-11-13 02:25:58.183785 ooo_dev_tools-0.9.3/ooodev/dialog/msgbox.py
--rw-r--r--   0        0        0     2019 2022-10-27 15:27:12.045993 ooo_dev_tools-0.9.3/ooodev/dialog/tk_input.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.789060 ooo_dev_tools-0.9.3/ooodev/events/__init__.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.789342 ooo_dev_tools-0.9.3/ooodev/events/args/__init__.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.789342 ooo_dev_tools-0.9.3/ooodev/events/args/calc/__init__.py
--rw-r--r--   0        0        0     1371 2023-04-02 18:09:12.324621 ooo_dev_tools-0.9.3/ooodev/events/args/calc/cell_args.py
--rw-r--r--   0        0        0     1461 2023-04-02 18:09:12.325621 ooo_dev_tools-0.9.3/ooodev/events/args/calc/cell_cancel_args.py
--rw-r--r--   0        0        0     1590 2023-04-02 18:09:12.326621 ooo_dev_tools-0.9.3/ooodev/events/args/calc/sheet_args.py
--rw-r--r--   0        0        0     1575 2023-04-02 18:09:12.327740 ooo_dev_tools-0.9.3/ooodev/events/args/calc/sheet_cancel_args.py
--rw-r--r--   0        0        0     1451 2023-04-02 18:09:12.328623 ooo_dev_tools-0.9.3/ooodev/events/args/cancel_event_args.py
--rw-r--r--   0        0        0     1163 2023-04-02 18:09:12.328745 ooo_dev_tools-0.9.3/ooodev/events/args/dispatch_args.py
--rw-r--r--   0        0        0     1450 2023-04-02 18:09:12.329620 ooo_dev_tools-0.9.3/ooodev/events/args/dispatch_cancel_args.py
--rw-r--r--   0        0        0     4051 2023-04-06 02:13:08.628097 ooo_dev_tools-0.9.3/ooodev/events/args/event_args.py
--rw-r--r--   0        0        0      640 2022-11-29 00:27:48.243330 ooo_dev_tools-0.9.3/ooodev/events/args/generic_args.py
--rw-r--r--   0        0        0     1366 2023-04-02 18:09:12.330620 ooo_dev_tools-0.9.3/ooodev/events/args/key_val_args.py
--rw-r--r--   0        0        0     1608 2023-04-02 18:09:12.331622 ooo_dev_tools-0.9.3/ooodev/events/args/key_val_cancel_args.py
--rw-r--r--   0        0        0     5995 2023-04-02 18:09:12.332622 ooo_dev_tools-0.9.3/ooodev/events/calc_named_event.py
--rw-r--r--   0        0        0      391 2022-11-29 00:27:48.244327 ooo_dev_tools-0.9.3/ooodev/events/command.py
--rw-r--r--   0        0        0      312 2023-04-02 18:09:12.332622 ooo_dev_tools-0.9.3/ooodev/events/draw_named_event.py
--rw-r--r--   0        0        0     4247 2023-04-02 18:09:12.333621 ooo_dev_tools-0.9.3/ooodev/events/event_singleton.py
--rw-r--r--   0        0        0     3594 2023-04-06 02:13:08.629097 ooo_dev_tools-0.9.3/ooodev/events/format_named_event.py
--rw-r--r--   0        0        0      210 2023-04-02 18:09:12.334621 ooo_dev_tools-0.9.3/ooodev/events/gbl_named_event.py
--rw-r--r--   0        0        0     9544 2023-04-02 18:09:12.335620 ooo_dev_tools-0.9.3/ooodev/events/lo_events.py
--rw-r--r--   0        0        0     3082 2023-04-02 18:09:12.336620 ooo_dev_tools-0.9.3/ooodev/events/lo_named_event.py
--rw-r--r--   0        0        0      728 2023-04-02 18:09:12.336620 ooo_dev_tools-0.9.3/ooodev/events/props_named_event.py
--rw-r--r--   0        0        0     5175 2023-04-02 18:09:12.337911 ooo_dev_tools-0.9.3/ooodev/events/write_named_event.py
--rw-r--r--   0        0        0        0 2022-06-09 05:52:04.175567 ooo_dev_tools-0.9.3/ooodev/exceptions/__init__.py
--rw-r--r--   0        0        0     9928 2023-04-06 02:13:08.630095 ooo_dev_tools-0.9.3/ooodev/exceptions/ex.py
--rw-r--r--   0        0        0      160 2023-04-06 02:13:08.630095 ooo_dev_tools-0.9.3/ooodev/format/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.339621 ooo_dev_tools-0.9.3/ooodev/format/calc/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.339621 ooo_dev_tools-0.9.3/ooodev/format/calc/direct/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.631093 ooo_dev_tools-0.9.3/ooodev/format/calc/direct/cell/__init__.py
--rw-r--r--   0        0        0      812 2023-04-06 02:13:48.174066 ooo_dev_tools-0.9.3/ooodev/format/calc/direct/cell/alignment/__init__.py
--rw-r--r--   0        0        0      108 2023-04-06 02:13:08.632095 ooo_dev_tools-0.9.3/ooodev/format/calc/direct/cell/background/__init__.py
--rw-r--r--   0        0        0      782 2023-04-07 18:06:32.190987 ooo_dev_tools-0.9.3/ooodev/format/calc/direct/cell/borders/__init__.py
--rw-r--r--   0        0        0      139 2023-04-06 02:13:08.633094 ooo_dev_tools-0.9.3/ooodev/format/calc/direct/cell/cell_protection/__init__.py
--rw-r--r--   0        0        0     1379 2023-04-06 02:13:08.634096 ooo_dev_tools-0.9.3/ooodev/format/calc/direct/cell/font/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.634096 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.634096 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/cell/__init__.py
--rw-r--r--   0        0        0     1376 2023-04-06 02:13:08.635093 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/cell/alignment/__init__.py
--rw-r--r--   0        0        0      291 2023-04-06 02:13:08.635093 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/cell/background/__init__.py
--rw-r--r--   0        0        0      852 2023-04-07 18:06:32.191986 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/cell/borders/__init__.py
--rw-r--r--   0        0        0      375 2023-04-06 02:13:08.636101 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/cell/cell_protection/__init__.py
--rw-r--r--   0        0        0     1245 2023-04-06 02:13:08.637094 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/cell/font/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.637094 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/__init__.py
--rw-r--r--   0        0        0     1123 2023-04-06 02:13:08.638093 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/area/__init__.py
--rw-r--r--   0        0        0     1019 2023-04-06 02:13:08.638093 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/borders/__init__.py
--rw-r--r--   0        0        0      276 2023-04-06 02:13:08.639095 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/footer/__init__.py
--rw-r--r--   0        0        0     1100 2023-04-06 02:13:08.639095 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/footer/area/__init__.py
--rw-r--r--   0        0        0     1005 2023-04-06 02:13:08.640095 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/footer/borders/__init__.py
--rw-r--r--   0        0        0      290 2023-04-06 02:13:08.640095 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/header/__init__.py
--rw-r--r--   0        0        0     1235 2023-04-06 02:13:08.641104 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/header/area/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-06 02:13:08.641104 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/header/borders/__init__.py
--rw-r--r--   0        0        0     1162 2023-04-06 02:13:08.642093 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/page/__init__.py
--rw-r--r--   0        0        0      708 2023-04-06 02:13:08.642093 ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/sheet/__init__.py
--rw-r--r--   0        0        0      254 2023-04-06 02:13:48.198066 ooo_dev_tools-0.9.3/ooodev/format/calc/style/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.643095 ooo_dev_tools-0.9.3/ooodev/format/calc/style/cell/__init__.py
--rw-r--r--   0        0        0     4313 2023-04-06 02:13:48.198066 ooo_dev_tools-0.9.3/ooodev/format/calc/style/cell/cell.py
--rw-r--r--   0        0        0       60 2023-04-06 02:13:08.644094 ooo_dev_tools-0.9.3/ooodev/format/calc/style/cell/kind/__init__.py
--rw-r--r--   0        0        0      588 2023-04-06 02:13:08.645093 ooo_dev_tools-0.9.3/ooodev/format/calc/style/cell/kind/style_cell_kind.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.645093 ooo_dev_tools-0.9.3/ooodev/format/calc/style/page/__init__.py
--rw-r--r--   0        0        0       73 2023-04-06 02:13:08.645093 ooo_dev_tools-0.9.3/ooodev/format/calc/style/page/kind/__init__.py
--rw-r--r--   0        0        0      207 2023-04-06 02:13:08.646094 ooo_dev_tools-0.9.3/ooodev/format/calc/style/page/kind/calc_style_page_kind.py
--rw-r--r--   0        0        0     4101 2023-04-06 02:13:48.199068 ooo_dev_tools-0.9.3/ooodev/format/calc/style/page/page.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.403612 ooo_dev_tools-0.9.3/ooodev/format/draw/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.404613 ooo_dev_tools-0.9.3/ooodev/format/draw/direct/__init__.py
--rw-r--r--   0        0        0     1401 2023-04-07 18:06:32.193000 ooo_dev_tools-0.9.3/ooodev/format/draw/direct/area/__init__.py
--rw-r--r--   0        0        0      641 2023-04-06 02:13:08.648096 ooo_dev_tools-0.9.3/ooodev/format/draw/direct/transparency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.405614 ooo_dev_tools-0.9.3/ooodev/format/draw/modify/__init__.py
--rw-r--r--   0        0        0      945 2023-04-06 02:13:08.675095 ooo_dev_tools-0.9.3/ooodev/format/draw/modify/area/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.406613 ooo_dev_tools-0.9.3/ooodev/format/draw/style/__init__.py
--rw-r--r--   0        0        0      277 2023-04-02 18:09:12.406613 ooo_dev_tools-0.9.3/ooodev/format/draw/style/kind/__init__.py
--rw-r--r--   0        0        0     2652 2023-04-02 18:09:12.407617 ooo_dev_tools-0.9.3/ooodev/format/draw/style/lookup/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.408612 ooo_dev_tools-0.9.3/ooodev/format/impress/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.408612 ooo_dev_tools-0.9.3/ooodev/format/impress/modify/__init__.py
--rw-r--r--   0        0        0      945 2023-04-06 02:13:08.676094 ooo_dev_tools-0.9.3/ooodev/format/impress/modify/area/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.677093 ooo_dev_tools-0.9.3/ooodev/format/inner/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.677093 ooo_dev_tools-0.9.3/ooodev/format/inner/common/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.677093 ooo_dev_tools-0.9.3/ooodev/format/inner/common/abstract/__init__.py
--rw-r--r--   0        0        0     3954 2023-04-06 02:13:08.678094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/abstract/abstract_document.py
--rw-r--r--   0        0        0     4577 2023-04-06 02:13:48.214066 ooo_dev_tools-0.9.3/ooodev/format/inner/common/abstract/abstract_fill_color.py
--rw-r--r--   0        0        0    16076 2023-04-06 02:13:48.251066 ooo_dev_tools-0.9.3/ooodev/format/inner/common/abstract/abstract_hf.py
--rw-r--r--   0        0        0     7849 2023-04-06 02:13:08.680093 ooo_dev_tools-0.9.3/ooodev/format/inner/common/abstract/abstract_line_number.py
--rw-r--r--   0        0        0    11818 2023-04-06 02:13:08.681095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/abstract/abstract_padding.py
--rw-r--r--   0        0        0    10284 2023-04-06 02:13:08.682094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/abstract/abstract_sides.py
--rw-r--r--   0        0        0     4323 2023-04-06 02:13:08.683094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/border_width_impl.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.683094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/format_types/__init__.py
--rw-r--r--   0        0        0      262 2023-04-06 02:13:08.684096 ooo_dev_tools-0.9.3/ooodev/format/inner/common/format_types/offset_column.py
--rw-r--r--   0        0        0      256 2023-04-06 02:13:08.684096 ooo_dev_tools-0.9.3/ooodev/format/inner/common/format_types/offset_row.py
--rw-r--r--   0        0        0      252 2023-04-06 02:13:08.685095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/format_types/size_percent.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.685095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/__init__.py
--rw-r--r--   0        0        0      318 2023-04-06 02:13:08.685095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/area_gradient_props.py
--rw-r--r--   0        0        0      324 2023-04-06 02:13:08.686095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/area_hatch_props.py
--rw-r--r--   0        0        0      531 2023-04-06 02:13:08.686095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/area_img_props.py
--rw-r--r--   0        0        0      294 2023-04-06 02:13:08.687092 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/area_pattern_props.py
--rw-r--r--   0        0        0      187 2023-04-06 02:13:08.687092 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/border_props.py
--rw-r--r--   0        0        0      181 2023-04-06 02:13:08.688095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/cell_background_color_props.py
--rw-r--r--   0        0        0      650 2023-04-06 02:13:08.688095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/cell_borders_props.py
--rw-r--r--   0        0        0      499 2023-04-06 02:13:08.689094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/cell_style_borders_props.py
--rw-r--r--   0        0        0      238 2023-04-06 02:13:08.689094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/cell_text_align_props.py
--rw-r--r--   0        0        0      197 2023-04-06 02:13:08.690093 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/cell_text_orientation_props.py
--rw-r--r--   0        0        0      203 2023-04-06 02:13:08.690093 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/cell_text_properties_props.py
--rw-r--r--   0        0        0      288 2023-04-06 02:13:08.691092 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/fill_color_props.py
--rw-r--r--   0        0        0      179 2023-04-06 02:13:08.691092 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/font_only_props.py
--rw-r--r--   0        0        0      176 2023-04-06 02:13:08.692095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/frame_options_align_props.py
--rw-r--r--   0        0        0      196 2023-04-06 02:13:08.692095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/frame_options_names_props.py
--rw-r--r--   0        0        0      239 2023-04-06 02:13:08.693095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/frame_options_properties.py
--rw-r--r--   0        0        0      244 2023-04-06 02:13:08.693095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/frame_options_protect_props.py
--rw-r--r--   0        0        0      166 2023-04-06 02:13:08.694094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/frame_type_anchor_props.py
--rw-r--r--   0        0        0      445 2023-04-06 02:13:08.695094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/frame_type_positon_props.py
--rw-r--r--   0        0        0      449 2023-04-06 02:13:08.695094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/frame_type_size_props.py
--rw-r--r--   0        0        0      231 2023-04-06 02:13:08.696094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/frame_wrap_options_props.py
--rw-r--r--   0        0        0      165 2023-04-06 02:13:08.696094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/frame_wrap_settings_props.py
--rw-r--r--   0        0        0      628 2023-04-06 02:13:08.697094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/hf_props.py
--rw-r--r--   0        0        0      313 2023-04-06 02:13:08.697094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/hyperlink_props.py
--rw-r--r--   0        0        0      263 2023-04-06 02:13:08.698096 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/image_crop_props.py
--rw-r--r--   0        0        0      253 2023-04-06 02:13:08.698096 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/image_flip_props.py
--rw-r--r--   0        0        0      209 2023-04-06 02:13:08.699094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/image_options_names_props.py
--rw-r--r--   0        0        0      168 2023-04-06 02:13:08.699094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/image_options_properties.py
--rw-r--r--   0        0        0      154 2023-04-06 02:13:08.700095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/image_rotation_props.py
--rw-r--r--   0        0        0      218 2023-04-06 02:13:08.700095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/img_para_area_props.py
--rw-r--r--   0        0        0      178 2023-04-06 02:13:08.701096 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/list_style_props.py
--rw-r--r--   0        0        0      207 2023-04-06 02:13:08.701096 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/page_margin_props.py
--rw-r--r--   0        0        0      157 2023-04-06 02:13:08.702098 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/prop_pair.py
--rw-r--r--   0        0        0      329 2023-04-06 02:13:08.702098 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/shape_shadow_props.py
--rw-r--r--   0        0        0      319 2023-04-06 02:13:08.703097 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/struct_border_table_props.py
--rw-r--r--   0        0        0      266 2023-04-06 02:13:08.703097 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/struct_cell_protection_props.py
--rw-r--r--   0        0        0      235 2023-04-06 02:13:08.704097 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/struct_crop_props.py
--rw-r--r--   0        0        0      208 2023-04-06 02:13:08.704097 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/struct_size_props.py
--rw-r--r--   0        0        0      333 2023-04-06 02:13:08.705094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/struct_table_border_distances_props.py
--rw-r--r--   0        0        0      443 2023-04-06 02:13:08.705094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/table_borders_props.py
--rw-r--r--   0        0        0      281 2023-04-06 02:13:08.706095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/table_properties_props.py
--rw-r--r--   0        0        0      279 2023-04-06 02:13:08.706095 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/transparent_gradient_props.py
--rw-r--r--   0        0        0      188 2023-04-06 02:13:08.707094 ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/transparent_transparency_props.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.707094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.747094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.783096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/alignment/__init__.py
--rw-r--r--   0        0        0     6882 2023-04-06 02:13:08.785095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/alignment/properties.py
--rw-r--r--   0        0        0     8619 2023-04-06 02:13:08.786095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/alignment/text_align.py
--rw-r--r--   0        0        0     6213 2023-04-06 02:13:08.786095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/alignment/text_orientation.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.787101 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/background/__init__.py
--rw-r--r--   0        0        0     5291 2023-04-06 02:13:48.252066 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/background/color.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.788097 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/border/__init__.py
--rw-r--r--   0        0        0    21534 2023-04-07 18:06:32.194988 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/border/borders.py
--rw-r--r--   0        0        0     3026 2023-04-06 02:13:08.789097 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/border/padding.py
--rw-r--r--   0        0        0      759 2023-04-06 02:13:08.790094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/border/shadow.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.790094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/cell_protection/__init__.py
--rw-r--r--   0        0        0      340 2023-04-06 02:13:08.790094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/cell_protection/cell_protection.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.791094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/page/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.791094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/page/page/__init__.py
--rw-r--r--   0        0        0     6479 2023-04-06 02:13:08.792095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/page/page/layout_settings.py
--rw-r--r--   0        0        0     7798 2023-04-06 02:13:08.792095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/page/page/margins.py
--rw-r--r--   0        0        0        0 2023-04-07 18:06:32.194988 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/draw/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 18:06:32.195989 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/draw/fill/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 18:06:32.195989 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/draw/fill/area/__init__.py
--rw-r--r--   0        0        0      229 2023-04-07 18:06:32.196990 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/draw/fill/area/color.py
--rw-r--r--   0        0        0      288 2023-04-07 18:06:32.197988 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/draw/fill/area/gradient.py
--rw-r--r--   0        0        0      249 2023-04-07 18:06:32.198989 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/draw/fill/area/hatch.py
--rw-r--r--   0        0        0      266 2023-04-07 18:06:32.199988 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/draw/fill/area/img.py
--rw-r--r--   0        0        0      250 2023-04-07 18:06:32.200989 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/draw/fill/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.793096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/__init__.py
--rw-r--r--   0        0        0     9315 2023-04-06 02:13:48.258068 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/cell_protection_struct.py
--rw-r--r--   0        0        0    11233 2023-04-06 02:13:48.260066 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/crop_struct.py
--rw-r--r--   0        0        0    10183 2023-04-06 02:13:48.262067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/drop_cap_struct.py
--rw-r--r--   0        0        0    14839 2023-04-06 02:13:48.264068 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/gradient_struct.py
--rw-r--r--   0        0        0     8274 2023-04-06 02:13:48.266068 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/hatch_struct.py
--rw-r--r--   0        0        0    10085 2023-04-06 02:13:48.267067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/line_spacing_struct.py
--rw-r--r--   0        0        0    31720 2023-04-06 02:13:48.269067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/locale_struct.py
--rw-r--r--   0        0        0    11857 2023-04-06 02:13:48.276066 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/shadow_struct.py
--rw-r--r--   0        0        0    25317 2023-04-06 02:13:48.277068 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/side.py
--rw-r--r--   0        0        0     8523 2023-04-06 02:13:48.279067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/size_struct.py
--rw-r--r--   0        0        0      640 2023-04-06 02:13:08.801095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/struct_base.py
--rw-r--r--   0        0        0    13991 2023-04-06 02:13:48.280068 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/tab_stop_struct.py
--rw-r--r--   0        0        0    13469 2023-04-06 02:13:48.281067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/table_border_distances_struct.py
--rw-r--r--   0        0        0    20841 2023-04-06 02:13:48.282066 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/table_border_struct.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.803095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.803095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.804095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/border/__init__.py
--rw-r--r--   0        0        0    10508 2023-04-06 02:13:08.805096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/border/borders.py
--rw-r--r--   0        0        0     2322 2023-04-06 02:13:08.805096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/border/padding.py
--rw-r--r--   0        0        0     1239 2023-04-06 02:13:08.806095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/border/shadow.py
--rw-r--r--   0        0        0     1766 2023-04-06 02:13:08.806095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/border/sides.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.807104 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/font/__init__.py
--rw-r--r--   0        0        0    34693 2023-04-07 18:06:32.201988 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/font/font.py
--rw-r--r--   0        0        0    26969 2023-04-06 02:13:48.315067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/font/font_effects.py
--rw-r--r--   0        0        0    21397 2023-04-06 02:13:48.316067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/font/font_only.py
--rw-r--r--   0        0        0    21143 2023-04-06 02:13:08.809094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/font/font_position.py
--rw-r--r--   0        0        0        1 2023-04-06 02:13:08.810097 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/highlight/__init__.py
--rw-r--r--   0        0        0     5150 2023-04-06 02:13:48.317067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/highlight/highlight.py
--rw-r--r--   0        0        0        1 2023-04-06 02:13:08.811097 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/hyperlink/__init__.py
--rw-r--r--   0        0        0     5042 2023-04-06 02:13:08.812096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/hyperlink/hyperlink.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.812096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.812096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/area/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-06 02:13:08.813095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/area/fill_color.py
--rw-r--r--   0        0        0    12826 2023-04-06 02:13:48.319068 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/area/gradient.py
--rw-r--r--   0        0        0    13085 2023-04-06 02:13:48.320066 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/area/hatch.py
--rw-r--r--   0        0        0    18242 2023-04-06 02:13:08.816096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/area/img.py
--rw-r--r--   0        0        0    10260 2023-04-06 02:13:48.321066 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.837095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/transparent/__init__.py
--rw-r--r--   0        0        0    11815 2023-04-06 02:13:08.839095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/transparent/gradient.py
--rw-r--r--   0        0        0     4966 2023-04-06 02:13:08.840097 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/transparent/transparency.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.852094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.852094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/frame_type/__init__.py
--rw-r--r--   0        0        0     4866 2023-04-06 02:13:08.853094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/frame_type/anchor.py
--rw-r--r--   0        0        0    18717 2023-04-06 02:13:08.866093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/frame_type/position.py
--rw-r--r--   0        0        0     6874 2023-04-06 02:13:08.867093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/frame_type/size.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.867093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/hyperlink/__init__.py
--rw-r--r--   0        0        0     4026 2023-04-06 02:13:08.868093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/hyperlink/image_map_options.py
--rw-r--r--   0        0        0     5997 2023-04-06 02:13:08.869093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/hyperlink/link_to.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.869093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/options/__init__.py
--rw-r--r--   0        0        0     4913 2023-04-06 02:13:08.870096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/options/align.py
--rw-r--r--   0        0        0     8725 2023-04-06 02:13:08.871096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/options/names.py
--rw-r--r--   0        0        0     9653 2023-04-06 02:13:08.871096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/options/properties.py
--rw-r--r--   0        0        0     4781 2023-04-06 02:13:08.872094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/options/protect.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.872094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/wrap/__init__.py
--rw-r--r--   0        0        0     7691 2023-04-06 02:13:08.873093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/wrap/options.py
--rw-r--r--   0        0        0     3655 2023-04-06 02:13:08.873093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/wrap/settings.py
--rw-r--r--   0        0        0     1796 2023-04-06 02:13:08.874109 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/wrap/spacing.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.874109 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.874109 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/crop/__init__.py
--rw-r--r--   0        0        0    18759 2023-04-06 02:13:48.323067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/crop/crop.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.875093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/image/__init__.py
--rw-r--r--   0        0        0     5201 2023-04-06 02:13:08.876094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/image/flip.py
--rw-r--r--   0        0        0     3716 2023-04-06 02:13:08.876094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/image/rotation.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.877095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/image_type/__init__.py
--rw-r--r--   0        0        0    11093 2023-04-06 02:13:08.877095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/image_type/size.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.878097 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/options/__init__.py
--rw-r--r--   0        0        0     2718 2023-04-06 02:13:08.878097 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/options/names.py
--rw-r--r--   0        0        0     3786 2023-04-06 02:13:08.879093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/options/properties.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.879093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:48.323067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/footer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:48.324069 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/footer/area/__init__.py
--rw-r--r--   0        0        0      961 2023-04-06 02:13:48.325067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/footer/area/color.py
--rw-r--r--   0        0        0     1247 2023-04-06 02:13:48.325067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/footer/area/gradient.py
--rw-r--r--   0        0        0     1302 2023-04-06 02:13:48.326069 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/footer/area/hatch.py
--rw-r--r--   0        0        0     1505 2023-04-06 02:13:48.326069 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/footer/area/img.py
--rw-r--r--   0        0        0     1226 2023-04-06 02:13:48.327067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/footer/area/pattern.py
--rw-r--r--   0        0        0     1432 2023-04-06 02:13:48.328065 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/footer/footer.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:48.328065 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/header/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:48.329080 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/header/area/__init__.py
--rw-r--r--   0        0        0     1376 2023-04-06 02:13:48.329080 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/header/area/color.py
--rw-r--r--   0        0        0     1679 2023-04-06 02:13:48.359068 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/header/area/gradient.py
--rw-r--r--   0        0        0     1815 2023-04-06 02:13:48.360070 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/header/area/hatch.py
--rw-r--r--   0        0        0     1962 2023-04-06 02:13:48.361065 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/header/area/img.py
--rw-r--r--   0        0        0     1683 2023-04-06 02:13:48.362067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/header/area/pattern.py
--rw-r--r--   0        0        0     1432 2023-04-06 02:13:48.413067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/header/header.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.879093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/page/__init__.py
--rw-r--r--   0        0        0     6554 2023-04-06 02:13:08.880098 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/page/layout_settings.py
--rw-r--r--   0        0        0     3103 2023-04-06 02:13:08.881093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/page/margins.py
--rw-r--r--   0        0        0     5382 2023-04-06 02:13:08.882094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/page/paper_format.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.882094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/__init__.py
--rw-r--r--   0        0        0      389 2023-04-06 02:13:08.883094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/align/__init__.py
--rw-r--r--   0        0        0    14994 2023-04-06 02:13:08.885097 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/align/alignment.py
--rw-r--r--   0        0        0     8097 2023-04-06 02:13:08.886093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/align/writing_mode.py
--rw-r--r--   0        0        0        1 2023-04-06 02:13:08.886093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/area/__init__.py
--rw-r--r--   0        0        0     1910 2023-04-06 02:13:08.887093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/area/color.py
--rw-r--r--   0        0        0    15216 2023-04-06 02:13:48.416068 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/area/hatch.py
--rw-r--r--   0        0        0    12082 2023-04-06 02:13:08.888094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/area/img.py
--rw-r--r--   0        0        0     6846 2023-04-06 02:13:48.416068 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/area/pattern.py
--rw-r--r--   0        0        0      471 2023-04-06 02:13:08.889093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/border/__init__.py
--rw-r--r--   0        0        0    11804 2023-04-06 02:13:08.890095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/border/borders.py
--rw-r--r--   0        0        0     2524 2023-04-06 02:13:08.890095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/border/padding.py
--rw-r--r--   0        0        0      834 2023-04-06 02:13:08.891093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/border/shadow.py
--rw-r--r--   0        0        0     2025 2023-04-06 02:13:08.892093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/border/sides.py
--rw-r--r--   0        0        0        1 2023-04-06 02:13:08.892093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/drop_cap/__init__.py
--rw-r--r--   0        0        0     9056 2023-04-06 02:13:08.893095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/drop_cap/drop_caps.py
--rw-r--r--   0        0        0      303 2023-04-06 02:13:08.894096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/indent_space/__init__.py
--rw-r--r--   0        0        0     9615 2023-04-06 02:13:08.894096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/indent_space/indent.py
--rw-r--r--   0        0        0     8011 2023-04-06 02:13:08.895096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/indent_space/indent_spacing.py
--rw-r--r--   0        0        0     7564 2023-04-06 02:13:48.417068 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/indent_space/line_spacing.py
--rw-r--r--   0        0        0     8377 2023-04-06 02:13:08.916093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/indent_space/spacing.py
--rw-r--r--   0        0        0      368 2023-04-06 02:13:08.917097 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/outline_list/__init__.py
--rw-r--r--   0        0        0      879 2023-04-06 02:13:08.917097 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/outline_list/line_num.py
--rw-r--r--   0        0        0     9905 2023-04-06 02:13:48.418067 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/outline_list/list_style.py
--rw-r--r--   0        0        0     7452 2023-04-06 02:13:08.918095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/outline_list/outline.py
--rw-r--r--   0        0        0     7022 2023-04-06 02:13:48.419065 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/outline_list/outline_list.py
--rw-r--r--   0        0        0     2936 2023-04-06 02:13:08.920094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/padding.py
--rw-r--r--   0        0        0      191 2023-04-06 02:13:08.920094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/tabs/__init__.py
--rw-r--r--   0        0        0     8574 2023-04-06 02:13:08.921095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/tabs/tabs.py
--rw-r--r--   0        0        0      261 2023-04-06 02:13:08.921095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/text_flow/__init__.py
--rw-r--r--   0        0        0     6402 2023-04-06 02:13:08.922096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/text_flow/breaks.py
--rw-r--r--   0        0        0    10238 2023-04-06 02:13:08.923093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/text_flow/flow_options.py
--rw-r--r--   0        0        0    10123 2023-04-06 02:13:08.924094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/text_flow/hyphenation.py
--rw-r--r--   0        0        0     7387 2023-04-06 02:13:08.924094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/text_flow/text_flow.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.924094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/transparent/__init__.py
--rw-r--r--   0        0        0     3859 2023-04-06 02:13:08.925095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/transparent/gradient.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.925095 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/shape/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.926092 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/shape/area/__init__.py
--rw-r--r--   0        0        0    16356 2023-04-06 02:13:48.420065 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/shape/area/shadow.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.927094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/table/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.927094 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/table/background/__init__.py
--rw-r--r--   0        0        0     1127 2023-04-06 02:13:08.928093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/table/background/color.py
--rw-r--r--   0        0        0     2513 2023-04-06 02:13:08.928093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/table/background/img.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.929096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/table/borders/__init__.py
--rw-r--r--   0        0        0    18684 2023-04-06 02:13:08.929096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/table/borders/borders.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.929096 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/table/props/__init__.py
--rw-r--r--   0        0        0    74782 2023-04-06 02:13:08.931093 ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/table/props/table_properties.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.931093 ooo_dev_tools-0.9.3/ooodev/format/inner/kind/__init__.py
--rw-r--r--   0        0        0      231 2023-04-06 02:13:08.932094 ooo_dev_tools-0.9.3/ooodev/format/inner/kind/border_kind.py
--rw-r--r--   0        0        0      509 2023-04-06 02:13:48.421066 ooo_dev_tools-0.9.3/ooodev/format/inner/kind/format_kind.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.932094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.933097 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.933097 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/alignment/__init__.py
--rw-r--r--   0        0        0     3747 2023-04-06 02:13:08.934097 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/alignment/properties.py
--rw-r--r--   0        0        0     3809 2023-04-06 02:13:08.935098 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/alignment/text_align.py
--rw-r--r--   0        0        0     3655 2023-04-06 02:13:08.935098 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/alignment/text_orientation.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.935098 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/background/__init__.py
--rw-r--r--   0        0        0     3261 2023-04-06 02:13:48.422065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/background/color.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.936097 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/border/__init__.py
--rw-r--r--   0        0        0    23992 2023-04-07 18:06:32.203989 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/border/borders.py
--rw-r--r--   0        0        0      172 2023-04-07 18:06:32.209987 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/border/padding.py
--rw-r--r--   0        0        0      166 2023-04-07 18:06:32.210989 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/border/shadow.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.937094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/cell_protection/__init__.py
--rw-r--r--   0        0        0     4681 2023-04-06 02:13:08.938093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/cell_protection/cell_protection.py
--rw-r--r--   0        0        0     3739 2023-04-06 02:13:08.938093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/cell_style_base.py
--rw-r--r--   0        0        0      820 2023-04-06 02:13:08.939094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/cell_style_base_multi.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.939094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/font/__init__.py
--rw-r--r--   0        0        0     6013 2023-04-06 02:13:48.425066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/font/font_effects.py
--rw-r--r--   0        0        0     4325 2023-04-06 02:13:08.941096 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/font/font_only.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.941096 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.941096 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/area/__init__.py
--rw-r--r--   0        0        0     4943 2023-04-06 02:13:48.426066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/area/color.py
--rw-r--r--   0        0        0     5808 2023-04-06 02:13:08.942093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/area/img.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.943095 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/border/__init__.py
--rw-r--r--   0        0        0     5359 2023-04-06 02:13:08.943095 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/border/padding.py
--rw-r--r--   0        0        0     4973 2023-04-06 02:13:48.426066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/border/shadow.py
--rw-r--r--   0        0        0     5300 2023-04-06 02:13:08.945095 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/border/sides.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.945095 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.945095 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/area/__init__.py
--rw-r--r--   0        0        0     1028 2023-04-06 02:13:48.427066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/area/color.py
--rw-r--r--   0        0        0     1943 2023-04-06 02:13:48.428066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/area/img.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.947095 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/border/__init__.py
--rw-r--r--   0        0        0     1095 2023-04-06 02:13:48.429066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/border/padding.py
--rw-r--r--   0        0        0      917 2023-04-06 02:13:48.429066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/border/shadow.py
--rw-r--r--   0        0        0     1092 2023-04-06 02:13:48.430065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/border/sides.py
--rw-r--r--   0        0        0     1116 2023-04-06 02:13:48.431066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/footer.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.982094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.982094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/area/__init__.py
--rw-r--r--   0        0        0     5283 2023-04-06 02:13:48.431066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/area/color.py
--rw-r--r--   0        0        0     7094 2023-04-06 02:13:48.432068 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/area/img.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.984094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/border/__init__.py
--rw-r--r--   0        0        0     6626 2023-04-06 02:13:48.433067 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/border/padding.py
--rw-r--r--   0        0        0     6045 2023-04-06 02:13:48.434070 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/border/shadow.py
--rw-r--r--   0        0        0     6289 2023-04-06 02:13:48.434070 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/border/sides.py
--rw-r--r--   0        0        0     7271 2023-04-06 02:13:48.435066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/header.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.986093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/page/__init__.py
--rw-r--r--   0        0        0     3819 2023-04-06 02:13:08.987094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/page/layout_settings.py
--rw-r--r--   0        0        0     3565 2023-04-06 02:13:08.987094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/page/margins.py
--rw-r--r--   0        0        0     4332 2023-04-06 02:13:08.988093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/page/paper_format.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.988093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/sheet/__init__.py
--rw-r--r--   0        0        0     4051 2023-04-06 02:13:08.989095 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/sheet/order.py
--rw-r--r--   0        0        0     7444 2023-04-06 02:13:08.989095 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/sheet/printing.py
--rw-r--r--   0        0        0     3418 2023-04-06 02:13:08.990094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/sheet/scale_num_of_pages.py
--rw-r--r--   0        0        0     4164 2023-04-06 02:13:08.991094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/sheet/scale_pages_width_height.py
--rw-r--r--   0        0        0     3543 2023-04-06 02:13:08.991094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/sheet/scale_reduce_enlarge.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.991094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.992093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.992093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/border/__init__.py
--rw-r--r--   0        0        0     3830 2023-04-06 02:13:08.993104 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/border/padding.py
--rw-r--r--   0        0        0     3881 2023-04-06 02:13:48.436066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/border/shadow.py
--rw-r--r--   0        0        0     3905 2023-04-06 02:13:08.994096 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/border/sides.py
--rw-r--r--   0        0        0      701 2023-04-06 02:13:08.994096 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/char_style_base_multi.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.995093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/font/__init__.py
--rw-r--r--   0        0        0     5324 2023-04-06 02:13:48.437065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/font/font_effects.py
--rw-r--r--   0        0        0     3778 2023-04-06 02:13:08.996095 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/font/font_only.py
--rw-r--r--   0        0        0     4855 2023-04-06 02:13:08.997094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/font/font_position.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.997094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/highlight/__init__.py
--rw-r--r--   0        0        0     3099 2023-04-06 02:13:48.438068 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/highlight/highlight.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.998094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/fill/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.999094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/fill/area/__init__.py
--rw-r--r--   0        0        0     5010 2023-04-06 02:13:48.439067 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/fill/area/img.py
--rw-r--r--   0        0        0      686 2023-04-06 02:13:09.000093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/fill/fill_style_base_multi.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.001095 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.001095 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/area/__init__.py
--rw-r--r--   0        0        0     3731 2023-04-06 02:13:48.440068 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/area/color.py
--rw-r--r--   0        0        0     6551 2023-04-06 02:13:48.441068 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/area/gradient.py
--rw-r--r--   0        0        0     5763 2023-04-06 02:13:48.442065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/area/hatch.py
--rw-r--r--   0        0        0     6033 2023-04-06 02:13:09.004092 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/area/img.py
--rw-r--r--   0        0        0     5246 2023-04-06 02:13:48.442065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.005095 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/border/__init__.py
--rw-r--r--   0        0        0     4498 2023-04-06 02:13:09.006094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/border/padding.py
--rw-r--r--   0        0        0     4409 2023-04-06 02:13:48.443065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/border/shadow.py
--rw-r--r--   0        0        0     4309 2023-04-06 02:13:09.007094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/border/sides.py
--rw-r--r--   0        0        0      742 2023-04-06 02:13:09.008093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/frame_style_base_multi.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.009094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/frame_type/__init__.py
--rw-r--r--   0        0        0     3280 2023-04-06 02:13:09.009094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/frame_type/anchor.py
--rw-r--r--   0        0        0     3895 2023-04-06 02:13:09.010094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/frame_type/position.py
--rw-r--r--   0        0        0     3568 2023-04-06 02:13:09.011093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/frame_type/size.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.011093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/options/__init__.py
--rw-r--r--   0        0        0     3294 2023-04-06 02:13:09.012094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/options/align.py
--rw-r--r--   0        0        0     3551 2023-04-06 02:13:09.012094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/options/properties.py
--rw-r--r--   0        0        0     3335 2023-04-06 02:13:09.013101 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/options/protect.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.013101 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/transparent/__init__.py
--rw-r--r--   0        0        0     4635 2023-04-06 02:13:09.040094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/transparent/gradient.py
--rw-r--r--   0        0        0     3782 2023-04-06 02:13:09.041093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/transparent/transparency.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.041093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/wrap/__init__.py
--rw-r--r--   0        0        0     3838 2023-04-06 02:13:09.042094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/wrap/options.py
--rw-r--r--   0        0        0     3185 2023-04-06 02:13:09.043094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/wrap/settings.py
--rw-r--r--   0        0        0     3864 2023-04-06 02:13:09.043094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/wrap/spacing.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.044094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.044094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/area/__init__.py
--rw-r--r--   0        0        0     4253 2023-04-06 02:13:48.444065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/area/color.py
--rw-r--r--   0        0        0     6171 2023-04-06 02:13:48.444065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/area/gradient.py
--rw-r--r--   0        0        0     5020 2023-04-06 02:13:48.445065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/area/hatch.py
--rw-r--r--   0        0        0     5914 2023-04-06 02:13:09.046093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/area/img.py
--rw-r--r--   0        0        0     4802 2023-04-06 02:13:48.446066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.047093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/border/__init__.py
--rw-r--r--   0        0        0     3905 2023-04-06 02:13:09.048094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/border/padding.py
--rw-r--r--   0        0        0     5049 2023-04-06 02:13:48.447065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/border/shadow.py
--rw-r--r--   0        0        0     3829 2023-04-06 02:13:09.049093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/border/sides.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.049093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.049093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/area/__init__.py
--rw-r--r--   0        0        0      892 2023-04-06 02:13:48.447065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/area/color.py
--rw-r--r--   0        0        0     1072 2023-04-06 02:13:48.448067 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/area/gradient.py
--rw-r--r--   0        0        0     1007 2023-04-06 02:13:48.449065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/area/hatch.py
--rw-r--r--   0        0        0     1346 2023-04-06 02:13:48.449065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/area/img.py
--rw-r--r--   0        0        0     1077 2023-04-06 02:13:48.450068 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.052094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/border/__init__.py
--rw-r--r--   0        0        0     1052 2023-04-06 02:13:48.510066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/border/padding.py
--rw-r--r--   0        0        0      976 2023-04-06 02:13:48.511066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/border/shadow.py
--rw-r--r--   0        0        0      971 2023-04-06 02:13:48.511066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/border/sides.py
--rw-r--r--   0        0        0     1176 2023-04-06 02:13:48.512066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/footer.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.055093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/transparency/__init__.py
--rw-r--r--   0        0        0     1095 2023-04-06 02:13:48.513065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/transparency/gradient.py
--rw-r--r--   0        0        0      994 2023-04-06 02:13:48.513065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/transparency/transparency.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.056092 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.057094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/area/__init__.py
--rw-r--r--   0        0        0     5331 2023-04-06 02:13:48.514066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/area/color.py
--rw-r--r--   0        0        0     7596 2023-04-06 02:13:48.515074 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/area/gradient.py
--rw-r--r--   0        0        0     6455 2023-04-06 02:13:48.515074 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/area/hatch.py
--rw-r--r--   0        0        0     7602 2023-04-06 02:13:48.516066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/area/img.py
--rw-r--r--   0        0        0     6295 2023-04-06 02:13:48.517067 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.060095 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/border/__init__.py
--rw-r--r--   0        0        0     6729 2023-04-06 02:13:48.517067 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/border/padding.py
--rw-r--r--   0        0        0     6148 2023-04-06 02:13:48.518065 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/border/shadow.py
--rw-r--r--   0        0        0     6403 2023-04-06 02:13:48.519066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/border/sides.py
--rw-r--r--   0        0        0     7279 2023-04-06 02:13:48.519066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/header.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.063098 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/transparency/__init__.py
--rw-r--r--   0        0        0     5959 2023-04-06 02:13:48.520064 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/transparency/gradient.py
--rw-r--r--   0        0        0     4560 2023-04-06 02:13:48.521067 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/transparency/transparency.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.064093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/page/__init__.py
--rw-r--r--   0        0        0     4052 2023-04-06 02:13:09.065093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/page/layout_settings.py
--rw-r--r--   0        0        0     3750 2023-04-06 02:13:09.066093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/page/margins.py
--rw-r--r--   0        0        0     4359 2023-04-06 02:13:09.066093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/page/paper_format.py
--rw-r--r--   0        0        0      778 2023-04-06 02:13:09.066093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/page_style_base_multi.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.067093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/transparency/__init__.py
--rw-r--r--   0        0        0     3751 2023-04-06 02:13:09.068093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/transparency/gradient.py
--rw-r--r--   0        0        0     3261 2023-04-06 02:13:09.069094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/transparency/transparency.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.069094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.069094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/align/__init__.py
--rw-r--r--   0        0        0     4517 2023-04-06 02:13:09.070093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/align/alignment.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.070093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/area/__init__.py
--rw-r--r--   0        0        0     2740 2023-04-06 02:13:48.522066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/area/color.py
--rw-r--r--   0        0        0     5562 2023-04-06 02:13:48.523066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/area/gradient.py
--rw-r--r--   0        0        0     5340 2023-04-06 02:13:48.523066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/area/hatch.py
--rw-r--r--   0        0        0     5005 2023-04-06 02:13:48.524066 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/area/img.py
--rw-r--r--   0        0        0     4841 2023-04-06 02:13:09.073094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.073094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/border/__init__.py
--rw-r--r--   0        0        0     4484 2023-04-06 02:13:09.085094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/border/borders.py
--rw-r--r--   0        0        0     3853 2023-04-06 02:13:09.086093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/border/padding.py
--rw-r--r--   0        0        0     3916 2023-04-06 02:13:48.525067 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/border/shadow.py
--rw-r--r--   0        0        0     3752 2023-04-06 02:13:09.087092 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/border/sides.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.087092 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/drop_cap/__init__.py
--rw-r--r--   0        0        0     3892 2023-04-06 02:13:09.088093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/drop_cap/drop_caps.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.088093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/font/__init__.py
--rw-r--r--   0        0        0     5359 2023-04-06 02:13:48.565068 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/font/font_effects.py
--rw-r--r--   0        0        0     3722 2023-04-06 02:13:09.089094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/font/font_only.py
--rw-r--r--   0        0        0     4933 2023-04-06 02:13:09.090093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/font/font_position.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.090093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/highlight/__init__.py
--rw-r--r--   0        0        0     3162 2023-04-06 02:13:48.570063 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/highlight/highlight.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.091092 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/indent_space/__init__.py
--rw-r--r--   0        0        0     3715 2023-04-06 02:13:09.092093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/indent_space/indent.py
--rw-r--r--   0        0        0     4124 2023-04-06 02:13:48.592064 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/indent_space/line_spacing.py
--rw-r--r--   0        0        0     3555 2023-04-06 02:13:09.093094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/indent_space/spacing.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.093094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/outline_list/__init__.py
--rw-r--r--   0        0        0     4065 2023-04-06 02:13:09.094093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/outline_list/line_num.py
--rw-r--r--   0        0        0     8129 2023-04-06 02:13:09.095094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/outline_list/list_style.py
--rw-r--r--   0        0        0     3214 2023-04-06 02:13:09.095094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/outline_list/outline.py
--rw-r--r--   0        0        0      837 2023-04-06 02:13:09.096093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/para_style_base_multi.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.096093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/tabs/__init__.py
--rw-r--r--   0        0        0     5372 2023-04-06 02:13:09.097093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/tabs/tabs.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.097093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/text_flow/__init__.py
--rw-r--r--   0        0        0     3288 2023-04-06 02:13:09.099100 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/text_flow/breaks.py
--rw-r--r--   0        0        0     3449 2023-04-06 02:13:09.110092 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/text_flow/flow_options.py
--rw-r--r--   0        0        0     3577 2023-04-06 02:13:09.110092 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/text_flow/hyphenation.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.111094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/transparent/__init__.py
--rw-r--r--   0        0        0     3765 2023-04-06 02:13:09.111094 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/transparent/gradient.py
--rw-r--r--   0        0        0     3230 2023-04-06 02:13:09.112093 ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/transparent/transparency.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.112093 ooo_dev_tools-0.9.3/ooodev/format/inner/preset/__init__.py
--rw-r--r--   0        0        0     8819 2023-04-06 02:13:48.593066 ooo_dev_tools-0.9.3/ooodev/format/inner/preset/preset_gradient.py
--rw-r--r--   0        0        0     7403 2023-04-06 02:13:48.594065 ooo_dev_tools-0.9.3/ooodev/format/inner/preset/preset_hatch.py
--rw-r--r--   0        0        0  1674033 2023-04-06 02:13:09.129092 ooo_dev_tools-0.9.3/ooodev/format/inner/preset/preset_image.py
--rw-r--r--   0        0        0     1257 2023-04-06 02:13:09.135093 ooo_dev_tools-0.9.3/ooodev/format/inner/preset/preset_paper_format.py
--rw-r--r--   0        0        0     5884 2023-04-06 02:13:09.137094 ooo_dev_tools-0.9.3/ooodev/format/inner/preset/preset_pattern.py
--rw-r--r--   0        0        0    51848 2023-04-06 02:13:48.596069 ooo_dev_tools-0.9.3/ooodev/format/inner/style_base.py
--rw-r--r--   0        0        0    12917 2023-04-06 02:13:09.174092 ooo_dev_tools-0.9.3/ooodev/format/readme.md
--rw-r--r--   0        0        0      738 2023-04-06 02:13:09.175094 ooo_dev_tools-0.9.3/ooodev/format/styler.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.738588 ooo_dev_tools-0.9.3/ooodev/format/writer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.738588 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.739586 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/char/__init__.py
--rw-r--r--   0        0        0      957 2023-04-06 02:13:09.175094 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/char/borders/__init__.py
--rw-r--r--   0        0        0     1686 2023-04-06 02:13:09.176093 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/char/font/__init__.py
--rw-r--r--   0        0        0      129 2023-04-06 02:13:09.177094 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/char/highlight/__init__.py
--rw-r--r--   0        0        0      238 2023-04-06 02:13:09.178103 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/char/hyperlink/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.741673 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/frame/__init__.py
--rw-r--r--   0        0        0     2001 2023-04-06 02:13:09.178103 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/frame/area/__init__.py
--rw-r--r--   0        0        0      636 2023-04-06 02:13:09.180093 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/frame/borders/__init__.py
--rw-r--r--   0        0        0      349 2023-04-06 02:13:09.181096 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/frame/hyperlink/__init__.py
--rw-r--r--   0        0        0      653 2023-04-06 02:13:09.183092 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/frame/options/__init__.py
--rw-r--r--   0        0        0      584 2023-04-06 02:13:09.184095 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/frame/transparency/__init__.py
--rw-r--r--   0        0        0     1471 2023-04-06 02:13:09.184095 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/frame/type/__init__.py
--rw-r--r--   0        0        0      378 2023-04-06 02:13:09.185094 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/frame/wrap/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.753585 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/image/__init__.py
--rw-r--r--   0        0        0     2001 2023-04-06 02:13:09.186092 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/image/area/__init__.py
--rw-r--r--   0        0        0      636 2023-04-06 02:13:09.187095 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/image/borders/__init__.py
--rw-r--r--   0        0        0      313 2023-04-06 02:13:09.188095 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/image/crop/__init__.py
--rw-r--r--   0        0        0      351 2023-04-06 02:13:09.188095 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/image/hyperlink/__init__.py
--rw-r--r--   0        0        0      289 2023-04-06 02:13:09.189094 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/image/image/__init__.py
--rw-r--r--   0        0        0      318 2023-04-06 02:13:09.190093 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/image/options/__init__.py
--rw-r--r--   0        0        0      584 2023-04-06 02:13:09.191094 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/image/transparency/__init__.py
--rw-r--r--   0        0        0     1471 2023-04-06 02:13:09.191094 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/image/type/__init__.py
--rw-r--r--   0        0        0      378 2023-04-06 02:13:09.192094 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/image/wrap/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.758699 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/obj/__init__.py
--rw-r--r--   0        0        0     2001 2023-04-06 02:13:09.193093 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/obj/area/__init__.py
--rw-r--r--   0        0        0      636 2023-04-06 02:13:09.194093 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/obj/borders/__init__.py
--rw-r--r--   0        0        0      349 2023-04-06 02:13:09.194093 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/obj/hyperlink/__init__.py
--rw-r--r--   0        0        0      318 2023-04-06 02:13:09.196094 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/obj/options/__init__.py
--rw-r--r--   0        0        0      584 2023-04-06 02:13:09.197093 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/obj/transparency/__init__.py
--rw-r--r--   0        0        0     1471 2023-04-06 02:13:09.198094 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/obj/type/__init__.py
--rw-r--r--   0        0        0      378 2023-04-06 02:13:09.198094 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/obj/wrap/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:48.596069 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/page/__init__.py
--rw-r--r--   0        0        0      114 2023-04-06 02:13:48.597066 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/page/footer/__init__.py
--rw-r--r--   0        0        0     1743 2023-04-06 02:13:48.598067 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/page/footer/area/__init__.py
--rw-r--r--   0        0        0      114 2023-04-06 02:13:48.598067 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/page/header/__init__.py
--rw-r--r--   0        0        0     1743 2023-04-06 02:13:48.599067 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/page/header/area/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.766787 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/__init__.py
--rw-r--r--   0        0        0      596 2023-04-06 02:13:09.199097 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/alignment/__init__.py
--rw-r--r--   0        0        0     2067 2023-04-06 02:13:09.202093 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/area/__init__.py
--rw-r--r--   0        0        0      838 2023-04-06 02:13:09.203094 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/borders/__init__.py
--rw-r--r--   0        0        0      205 2023-04-06 02:13:09.204094 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/drop_caps/__init__.py
--rw-r--r--   0        0        0      439 2023-04-06 02:13:09.205092 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/indent_space/__init__.py
--rw-r--r--   0        0        0      517 2023-04-06 02:13:09.205092 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/outline_list/__init__.py
--rw-r--r--   0        0        0      269 2023-04-06 02:13:09.206092 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/tabs/__init__.py
--rw-r--r--   0        0        0      406 2023-04-06 02:13:09.207091 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/text_flow/__init__.py
--rw-r--r--   0        0        0      536 2023-04-06 02:13:09.207091 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/transparency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.773090 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/shape/__init__.py
--rw-r--r--   0        0        0     1828 2023-04-06 02:13:09.222095 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/shape/area/__init__.py
--rw-r--r--   0        0        0      396 2023-04-06 02:13:09.223094 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/shape/shadow/__init__.py
--rw-r--r--   0        0        0      584 2023-04-06 02:13:09.223094 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/shape/transparency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.775216 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/table/__init__.py
--rw-r--r--   0        0        0     1223 2023-04-06 02:13:09.224095 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/table/background/__init__.py
--rw-r--r--   0        0        0      828 2023-04-06 02:13:09.225093 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/table/borders/__init__.py
--rw-r--r--   0        0        0      265 2023-04-06 02:13:09.226093 ooo_dev_tools-0.9.3/ooodev/format/writer/direct/table/properties/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.776595 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.777629 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/char/__init__.py
--rw-r--r--   0        0        0     1134 2023-04-06 02:13:09.228094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/char/borders/__init__.py
--rw-r--r--   0        0        0     1683 2023-04-06 02:13:09.229095 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/char/font/__init__.py
--rw-r--r--   0        0        0      346 2023-04-06 02:13:09.230094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/char/highlight/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.779585 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/frame/__init__.py
--rw-r--r--   0        0        0     2421 2023-04-06 02:13:09.231100 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/frame/area/__init__.py
--rw-r--r--   0        0        0     1091 2023-04-06 02:13:09.232094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/frame/borders/__init__.py
--rw-r--r--   0        0        0     1034 2023-04-06 02:13:09.233093 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/frame/options/__init__.py
--rw-r--r--   0        0        0      818 2023-04-06 02:13:09.233093 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/frame/transparency/__init__.py
--rw-r--r--   0        0        0     1911 2023-04-06 02:13:09.234094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/frame/type/__init__.py
--rw-r--r--   0        0        0      805 2023-04-06 02:13:09.235094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/frame/wrap/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.783676 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/__init__.py
--rw-r--r--   0        0        0     2427 2023-04-06 02:13:48.600068 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/area/__init__.py
--rw-r--r--   0        0        0     1105 2023-04-06 02:13:09.236092 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/borders/__init__.py
--rw-r--r--   0        0        0      321 2023-04-06 02:13:09.237093 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/footer/__init__.py
--rw-r--r--   0        0        0     2535 2023-04-06 02:13:09.237093 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/footer/area/__init__.py
--rw-r--r--   0        0        0     1147 2023-04-06 02:13:09.238094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/footer/borders/__init__.py
--rw-r--r--   0        0        0      995 2023-04-06 02:13:09.239092 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/footer/transparency/__init__.py
--rw-r--r--   0        0        0      321 2023-04-06 02:13:09.239092 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/header/__init__.py
--rw-r--r--   0        0        0     2535 2023-04-06 02:13:09.240096 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/header/area/__init__.py
--rw-r--r--   0        0        0     1148 2023-04-06 02:13:09.241093 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/header/borders/__init__.py
--rw-r--r--   0        0        0      995 2023-04-06 02:13:09.241093 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/header/transparency/__init__.py
--rw-r--r--   0        0        0     1293 2023-04-06 02:13:09.242093 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/page/__init__.py
--rw-r--r--   0        0        0     3526 2023-04-06 02:13:09.243093 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/page_style_base.py
--rw-r--r--   0        0        0     3939 2023-04-06 02:13:09.246092 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/page_style_base_multi.py
--rw-r--r--   0        0        0      958 2023-04-06 02:13:09.247094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/transparency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.792731 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/__init__.py
--rw-r--r--   0        0        0      794 2023-04-06 02:13:09.249093 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/alignment/__init__.py
--rw-r--r--   0        0        0     2297 2023-04-06 02:13:09.250094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/area/__init__.py
--rw-r--r--   0        0        0     1347 2023-04-06 02:13:09.250094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/borders/__init__.py
--rw-r--r--   0        0        0      402 2023-04-06 02:13:09.251094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/drop_caps/__init__.py
--rw-r--r--   0        0        0     1685 2023-04-06 02:13:09.252093 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/font/__init__.py
--rw-r--r--   0        0        0      319 2023-04-06 02:13:09.252093 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/highlight/__init__.py
--rw-r--r--   0        0        0      880 2023-04-06 02:13:09.253094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/indent_space/__init__.py
--rw-r--r--   0        0        0      955 2023-04-06 02:13:09.255094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/outline_list/__init__.py
--rw-r--r--   0        0        0      446 2023-04-06 02:13:09.257094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/tabs/__init__.py
--rw-r--r--   0        0        0      855 2023-04-06 02:13:09.257094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/text_flow/__init__.py
--rw-r--r--   0        0        0      839 2023-04-06 02:13:09.258094 ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/transparency/__init__.py
--rw-r--r--   0        0        0      750 2023-04-06 02:13:09.300094 ooo_dev_tools-0.9.3/ooodev/format/writer/style/__init__.py
--rw-r--r--   0        0        0      110 2023-04-02 18:09:12.799670 ooo_dev_tools-0.9.3/ooodev/format/writer/style/bullet_list/__init__.py
--rw-r--r--   0        0        0     4239 2023-04-06 02:13:48.601065 ooo_dev_tools-0.9.3/ooodev/format/writer/style/bullet_list/bullet_list.py
--rw-r--r--   0        0        0      107 2023-04-02 18:09:12.800581 ooo_dev_tools-0.9.3/ooodev/format/writer/style/char/__init__.py
--rw-r--r--   0        0        0     6741 2023-04-06 02:13:48.602067 ooo_dev_tools-0.9.3/ooodev/format/writer/style/char/char.py
--rw-r--r--   0        0        0       60 2023-04-02 18:09:12.802395 ooo_dev_tools-0.9.3/ooodev/format/writer/style/char/kind/__init__.py
--rw-r--r--   0        0        0     1135 2023-04-06 02:13:09.303093 ooo_dev_tools-0.9.3/ooodev/format/writer/style/char/kind/style_char_kind.py
--rw-r--r--   0        0        0       97 2023-04-06 02:13:09.304092 ooo_dev_tools-0.9.3/ooodev/format/writer/style/frame/__init__.py
--rw-r--r--   0        0        0     3704 2023-04-06 02:13:48.603067 ooo_dev_tools-0.9.3/ooodev/format/writer/style/frame/frame.py
--rw-r--r--   0        0        0      353 2023-04-06 02:13:09.305109 ooo_dev_tools-0.9.3/ooodev/format/writer/style/frame/style_frame_kind.py
--rw-r--r--   0        0        0       60 2023-04-02 18:09:12.804657 ooo_dev_tools-0.9.3/ooodev/format/writer/style/lst/__init__.py
--rw-r--r--   0        0        0      791 2023-04-06 02:13:09.306094 ooo_dev_tools-0.9.3/ooodev/format/writer/style/lst/style_list_kind.py
--rw-r--r--   0        0        0      115 2023-04-06 02:13:09.307094 ooo_dev_tools-0.9.3/ooodev/format/writer/style/page/__init__.py
--rw-r--r--   0        0        0       79 2023-04-06 02:13:09.308096 ooo_dev_tools-0.9.3/ooodev/format/writer/style/page/kind/__init__.py
--rw-r--r--   0        0        0      412 2023-04-06 02:13:09.309094 ooo_dev_tools-0.9.3/ooodev/format/writer/style/page/kind/writer_style_page_kind.py
--rw-r--r--   0        0        0     4711 2023-04-06 02:13:48.605068 ooo_dev_tools-0.9.3/ooodev/format/writer/style/page/page.py
--rw-r--r--   0        0        0       91 2023-04-03 22:12:05.347628 ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/__init__.py
--rw-r--r--   0        0        0      579 2023-04-02 18:09:12.808625 ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/__init__.py
--rw-r--r--   0        0        0      335 2023-04-06 02:13:09.310097 ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/style_chapter_kind.py
--rw-r--r--   0        0        0      260 2023-04-06 02:13:09.311093 ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/style_para_cond_kind.py
--rw-r--r--   0        0        0     1225 2023-04-06 02:13:09.312094 ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/style_para_html_kind.py
--rw-r--r--   0        0        0     2105 2023-04-06 02:13:09.312094 ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/style_para_index_kind.py
--rw-r--r--   0        0        0     4274 2023-04-06 02:13:09.313095 ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/style_para_kind.py
--rw-r--r--   0        0        0     2492 2023-04-06 02:13:09.314095 ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/style_para_list_kind.py
--rw-r--r--   0        0        0     1139 2023-04-06 02:13:09.316093 ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/style_para_special_kind.py
--rw-r--r--   0        0        0     1278 2023-04-06 02:13:09.317099 ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/style_para_text_kind.py
--rw-r--r--   0        0        0    11249 2023-04-06 02:13:48.607067 ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/para.py
--rw-r--r--   0        0        0      218 2022-11-22 00:28:23.283709 ooo_dev_tools-0.9.3/ooodev/formatters/__init__.py
--rw-r--r--   0        0        0     1185 2022-11-22 00:28:23.284709 ooo_dev_tools-0.9.3/ooodev/formatters/format_list_item.py
--rw-r--r--   0        0        0     1101 2022-11-22 00:28:23.284709 ooo_dev_tools-0.9.3/ooodev/formatters/format_string.py
--rw-r--r--   0        0        0     2540 2022-11-22 00:28:23.285710 ooo_dev_tools-0.9.3/ooodev/formatters/format_table_item.py
--rw-r--r--   0        0        0     3182 2022-11-22 00:28:23.285710 ooo_dev_tools-0.9.3/ooodev/formatters/formatter_list.py
--rw-r--r--   0        0        0    10394 2023-04-06 02:13:09.319094 ooo_dev_tools-0.9.3/ooodev/formatters/formatter_table.py
--rw-r--r--   0        0        0      130 2022-11-22 00:28:23.287709 ooo_dev_tools-0.9.3/ooodev/formatters/only_ignore_kind.py
--rw-r--r--   0        0        0      196 2022-11-22 00:28:23.287709 ooo_dev_tools-0.9.3/ooodev/formatters/string_kind.py
--rw-r--r--   0        0        0      720 2022-11-22 00:28:23.288717 ooo_dev_tools-0.9.3/ooodev/formatters/table_item_kind.py
--rw-r--r--   0        0        0     4482 2022-11-22 00:28:23.289713 ooo_dev_tools-0.9.3/ooodev/formatters/table_item_processer.py
--rw-r--r--   0        0        0      336 2022-11-22 00:28:23.290711 ooo_dev_tools-0.9.3/ooodev/formatters/table_rule_kind.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.797175 ooo_dev_tools-0.9.3/ooodev/lazy/__init__.py
--rw-r--r--   0        0        0     1551 2022-07-24 03:34:34.541590 ooo_dev_tools-0.9.3/ooodev/lazy/lazy_import.py
--rw-r--r--   0        0        0        0 2022-06-09 05:52:04.176192 ooo_dev_tools-0.9.3/ooodev/listeners/__init__.py
--rw-r--r--   0        0        0     1130 2022-07-20 01:40:32.577461 ooo_dev_tools-0.9.3/ooodev/listeners/x_event_adapter.py
--rw-r--r--   0        0        0     1402 2022-07-20 01:40:32.578458 ooo_dev_tools-0.9.3/ooodev/listeners/x_modify_adapter.py
--rw-r--r--   0        0        0     1355 2022-08-23 05:01:45.222321 ooo_dev_tools-0.9.3/ooodev/listeners/x_selection_change_adapter.py
--rw-r--r--   0        0        0     1827 2022-07-20 01:40:32.580453 ooo_dev_tools-0.9.3/ooodev/listeners/x_terminate_adapter.py
--rw-r--r--   0        0        0     2034 2022-07-20 01:40:32.581450 ooo_dev_tools-0.9.3/ooodev/listeners/x_top_window_adapter.py
--rw-r--r--   0        0        0        0 2022-06-09 05:52:04.177777 ooo_dev_tools-0.9.3/ooodev/meta/__init__.py
--rw-r--r--   0        0        0      518 2023-04-02 18:09:12.815585 ooo_dev_tools-0.9.3/ooodev/meta/class_property_readonly.py
--rw-r--r--   0        0        0      545 2023-04-02 18:09:12.820755 ooo_dev_tools-0.9.3/ooodev/meta/deleted_attrib.py
--rw-r--r--   0        0        0     1617 2023-04-02 18:09:12.821833 ooo_dev_tools-0.9.3/ooodev/meta/deleted_enum_meta.py
--rw-r--r--   0        0        0      915 2023-04-02 18:09:12.822581 ooo_dev_tools-0.9.3/ooodev/meta/disabled_method.py
--rw-r--r--   0        0        0      241 2022-07-14 20:40:23.800284 ooo_dev_tools-0.9.3/ooodev/meta/singleton.py
--rw-r--r--   0        0        0     2135 2023-01-10 14:23:45.008570 ooo_dev_tools-0.9.3/ooodev/meta/static_meta.py
--rw-r--r--   0        0        0      518 2023-04-02 18:09:12.822581 ooo_dev_tools-0.9.3/ooodev/meta/static_prop.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.801281 ooo_dev_tools-0.9.3/ooodev/mock/__init__.py
--rw-r--r--   0        0        0      559 2022-07-14 20:40:23.801281 ooo_dev_tools-0.9.3/ooodev/mock/mock_g.py
--rw-r--r--   0        0        0      579 2022-10-04 00:14:04.239070 ooo_dev_tools-0.9.3/ooodev/mock/unohelper.py
--rw-r--r--   0        0        0        0 2022-06-09 05:51:34.370860 ooo_dev_tools-0.9.3/ooodev/office/__init__.py
--rw-r--r--   0        0        0   264405 2023-04-06 02:13:48.628067 ooo_dev_tools-0.9.3/ooodev/office/calc.py
--rw-r--r--   0        0        0    45621 2023-04-06 02:13:09.324093 ooo_dev_tools-0.9.3/ooodev/office/chart.py
--rw-r--r--   0        0        0    86455 2023-04-06 02:13:48.630066 ooo_dev_tools-0.9.3/ooodev/office/chart2.py
--rw-r--r--   0        0        0   135614 2023-04-06 02:13:48.632065 ooo_dev_tools-0.9.3/ooodev/office/draw.py
--rw-r--r--   0        0        0   149589 2023-04-06 02:13:48.634064 ooo_dev_tools-0.9.3/ooodev/office/write.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.805270 ooo_dev_tools-0.9.3/ooodev/proto/__init__.py
--rw-r--r--   0        0        0      626 2023-04-06 02:13:09.329093 ooo_dev_tools-0.9.3/ooodev/proto/dispatch_shape.py
--rw-r--r--   0        0        0     1453 2023-04-06 02:13:09.329093 ooo_dev_tools-0.9.3/ooodev/proto/event_observer.py
--rw-r--r--   0        0        0      450 2023-04-06 02:13:09.330101 ooo_dev_tools-0.9.3/ooodev/proto/size_obj.py
--rw-r--r--   0        0        0     2394 2023-04-06 02:13:09.331094 ooo_dev_tools-0.9.3/ooodev/proto/style_obj.py
--rw-r--r--   0        0        0      636 2023-04-06 02:13:48.635066 ooo_dev_tools-0.9.3/ooodev/theme/__init__.py
--rw-r--r--   0        0        0     1604 2023-04-07 18:06:32.211989 ooo_dev_tools-0.9.3/ooodev/theme/theme.py
--rw-r--r--   0        0        0     2212 2023-04-06 02:13:48.638067 ooo_dev_tools-0.9.3/ooodev/theme/theme_basic.py
--rw-r--r--   0        0        0     4152 2023-04-06 02:13:48.639065 ooo_dev_tools-0.9.3/ooodev/theme/theme_calc.py
--rw-r--r--   0        0        0      865 2023-04-06 02:13:48.640067 ooo_dev_tools-0.9.3/ooodev/theme/theme_draw.py
--rw-r--r--   0        0        0     4342 2023-04-06 02:13:48.640067 ooo_dev_tools-0.9.3/ooodev/theme/theme_general.py
--rw-r--r--   0        0        0     1416 2023-04-06 02:13:48.641076 ooo_dev_tools-0.9.3/ooodev/theme/theme_html.py
--rw-r--r--   0        0        0     3982 2023-04-06 02:13:48.641076 ooo_dev_tools-0.9.3/ooodev/theme/theme_rpt_builder.py
--rw-r--r--   0        0        0     2215 2023-04-06 02:13:48.642067 ooo_dev_tools-0.9.3/ooodev/theme/theme_sql.py
--rw-r--r--   0        0        0     4975 2023-04-06 02:13:48.642067 ooo_dev_tools-0.9.3/ooodev/theme/theme_text_doc.py
--rw-r--r--   0        0        0      768 2023-04-06 02:13:48.643065 ooo_dev_tools-0.9.3/ooodev/units/__init__.py
--rw-r--r--   0        0        0     8844 2023-04-06 02:13:09.334092 ooo_dev_tools-0.9.3/ooodev/units/unit_convert.py
--rw-r--r--   0        0        0     4704 2023-04-06 02:13:09.335095 ooo_dev_tools-0.9.3/ooodev/units/unit_inch.py
--rw-r--r--   0        0        0     4727 2023-04-06 02:13:09.369091 ooo_dev_tools-0.9.3/ooodev/units/unit_inch10.py
--rw-r--r--   0        0        0     4760 2023-04-06 02:13:09.369091 ooo_dev_tools-0.9.3/ooodev/units/unit_inch100.py
--rw-r--r--   0        0        0     5384 2023-04-06 02:13:09.370092 ooo_dev_tools-0.9.3/ooodev/units/unit_inch1000.py
--rw-r--r--   0        0        0     5238 2023-04-06 02:13:09.371091 ooo_dev_tools-0.9.3/ooodev/units/unit_mm.py
--rw-r--r--   0        0        0     5460 2023-04-06 02:13:09.372094 ooo_dev_tools-0.9.3/ooodev/units/unit_mm10.py
--rw-r--r--   0        0        0     5988 2023-04-06 02:13:09.373093 ooo_dev_tools-0.9.3/ooodev/units/unit_mm100.py
--rw-r--r--   0        0        0     1329 2023-04-06 02:13:48.644066 ooo_dev_tools-0.9.3/ooodev/units/unit_obj.py
--rw-r--r--   0        0        0     5041 2023-04-06 02:13:09.374093 ooo_dev_tools-0.9.3/ooodev/units/unit_pt.py
--rw-r--r--   0        0        0     5301 2023-04-06 02:13:09.374093 ooo_dev_tools-0.9.3/ooodev/units/unit_px.py
--rw-r--r--   0        0        0     1907 2022-07-14 20:40:23.806682 ooo_dev_tools-0.9.3/ooodev/utils/__init__.py
--rw-r--r--   0        0        0    26819 2023-04-06 02:13:48.645065 ooo_dev_tools-0.9.3/ooodev/utils/color.py
--rw-r--r--   0        0        0        0 2022-10-27 15:27:12.052996 ooo_dev_tools-0.9.3/ooodev/utils/data_type/__init__.py
--rw-r--r--   0        0        0     2758 2023-04-02 18:09:12.852582 ooo_dev_tools-0.9.3/ooodev/utils/data_type/angle.py
--rw-r--r--   0        0        0     3820 2022-12-17 01:13:14.728078 ooo_dev_tools-0.9.3/ooodev/utils/data_type/base_float_value.py
--rw-r--r--   0        0        0     3785 2023-04-02 18:09:12.853581 ooo_dev_tools-0.9.3/ooodev/utils/data_type/base_int_value.py
--rw-r--r--   0        0        0     1280 2023-04-02 18:09:12.874577 ooo_dev_tools-0.9.3/ooodev/utils/data_type/byte.py
--rw-r--r--   0        0        0     1298 2023-04-02 18:09:12.875872 ooo_dev_tools-0.9.3/ooodev/utils/data_type/byte_signed.py
--rw-r--r--   0        0        0    14993 2023-04-02 18:09:12.876578 ooo_dev_tools-0.9.3/ooodev/utils/data_type/cell_obj.py
--rw-r--r--   0        0        0     3298 2023-04-02 18:09:12.877797 ooo_dev_tools-0.9.3/ooodev/utils/data_type/cell_values.py
--rw-r--r--   0        0        0    10497 2023-04-06 02:13:09.375094 ooo_dev_tools-0.9.3/ooodev/utils/data_type/col_obj.py
--rw-r--r--   0        0        0      522 2023-04-02 18:09:12.879580 ooo_dev_tools-0.9.3/ooodev/utils/data_type/color_range.py
--rw-r--r--   0        0        0      195 2022-11-13 02:25:58.188785 ooo_dev_tools-0.9.3/ooodev/utils/data_type/dialog_title.py
--rw-r--r--   0        0        0     1020 2023-04-02 18:09:12.880576 ooo_dev_tools-0.9.3/ooodev/utils/data_type/image_offset.py
--rw-r--r--   0        0        0     1290 2023-04-02 18:09:12.882575 ooo_dev_tools-0.9.3/ooodev/utils/data_type/intensity.py
--rw-r--r--   0        0        0      880 2023-04-06 02:13:09.376093 ooo_dev_tools-0.9.3/ooodev/utils/data_type/intensity_range.py
--rw-r--r--   0        0        0      209 2023-04-02 18:09:12.884666 ooo_dev_tools-0.9.3/ooodev/utils/data_type/offset.py
--rw-r--r--   0        0        0      431 2023-04-02 18:09:12.884666 ooo_dev_tools-0.9.3/ooodev/utils/data_type/point.py
--rw-r--r--   0        0        0      482 2023-04-02 18:09:12.885575 ooo_dev_tools-0.9.3/ooodev/utils/data_type/point_positive.py
--rw-r--r--   0        0        0     1282 2023-04-02 18:09:12.886577 ooo_dev_tools-0.9.3/ooodev/utils/data_type/poly_sides.py
--rw-r--r--   0        0        0    22190 2023-04-06 02:13:09.377092 ooo_dev_tools-0.9.3/ooodev/utils/data_type/range_obj.py
--rw-r--r--   0        0        0    15997 2023-04-06 02:13:09.402093 ooo_dev_tools-0.9.3/ooodev/utils/data_type/range_values.py
--rw-r--r--   0        0        0     7314 2023-04-02 18:09:12.888579 ooo_dev_tools-0.9.3/ooodev/utils/data_type/row_obj.py
--rw-r--r--   0        0        0     1993 2023-04-06 02:13:09.403093 ooo_dev_tools-0.9.3/ooodev/utils/data_type/size.py
--rw-r--r--   0        0        0     3154 2023-04-06 02:13:09.404094 ooo_dev_tools-0.9.3/ooodev/utils/data_type/size_mm.py
--rw-r--r--   0        0        0     1126 2023-04-02 18:09:12.890576 ooo_dev_tools-0.9.3/ooodev/utils/data_type/width_height_fraction.py
--rw-r--r--   0        0        0      935 2023-04-02 18:09:12.891577 ooo_dev_tools-0.9.3/ooodev/utils/data_type/width_height_percent.py
--rw-r--r--   0        0        0      270 2022-11-13 02:25:58.189784 ooo_dev_tools-0.9.3/ooodev/utils/data_type/window_title.py
--rw-r--r--   0        0        0     5657 2022-12-10 17:01:36.559035 ooo_dev_tools-0.9.3/ooodev/utils/date_time_util.py
--rw-r--r--   0        0        0        0 2022-10-27 15:27:12.055992 ooo_dev_tools-0.9.3/ooodev/utils/decorator/__init__.py
--rw-r--r--   0        0        0     2736 2022-10-27 15:27:12.055992 ooo_dev_tools-0.9.3/ooodev/utils/decorator/enforce.py
--rw-r--r--   0        0        0    24793 2023-04-06 02:13:09.404094 ooo_dev_tools-0.9.3/ooodev/utils/dialogs.py
--rw-r--r--   0        0        0        0 2022-10-27 15:27:12.056992 ooo_dev_tools-0.9.3/ooodev/utils/dispatch/__init__.py
--rw-r--r--   0        0        0     3178 2022-10-27 15:27:12.057993 ooo_dev_tools-0.9.3/ooodev/utils/dispatch/draw_drawing_dispatch.py
--rw-r--r--   0        0        0     2806 2022-10-27 15:27:12.058992 ooo_dev_tools-0.9.3/ooodev/utils/dispatch/draw_view_dispatch.py
--rw-r--r--   0        0        0     3180 2022-10-27 15:27:12.059993 ooo_dev_tools-0.9.3/ooodev/utils/dispatch/global_edit_dispatch.py
--rw-r--r--   0        0        0     9772 2022-10-27 15:27:12.059993 ooo_dev_tools-0.9.3/ooodev/utils/dispatch/global_format_dispatch.py
--rw-r--r--   0        0        0     2911 2022-10-27 15:27:12.060992 ooo_dev_tools-0.9.3/ooodev/utils/dispatch/global_view_dispatch.py
--rw-r--r--   0        0        0    11843 2022-11-08 11:09:51.358105 ooo_dev_tools-0.9.3/ooodev/utils/dispatch/shape_dispatch_kind.py
--rw-r--r--   0        0        0     1562 2022-07-24 03:34:47.720953 ooo_dev_tools-0.9.3/ooodev/utils/enum_helper.py
--rw-r--r--   0        0        0    21457 2022-11-30 23:26:32.117139 ooo_dev_tools-0.9.3/ooodev/utils/file_io.py
--rw-r--r--   0        0        0    44086 2023-04-06 02:13:48.646066 ooo_dev_tools-0.9.3/ooodev/utils/forms.py
--rw-r--r--   0        0        0    21957 2023-04-02 18:09:12.895589 ooo_dev_tools-0.9.3/ooodev/utils/gallery.py
--rw-r--r--   0        0        0     7438 2023-04-02 18:09:12.897956 ooo_dev_tools-0.9.3/ooodev/utils/gen_util.py
--rw-r--r--   0        0        0    58911 2023-04-06 02:13:09.406094 ooo_dev_tools-0.9.3/ooodev/utils/gui.py
--rw-r--r--   0        0        0     2062 2022-07-14 20:40:23.810268 ooo_dev_tools-0.9.3/ooodev/utils/image_transferable.py
--rw-r--r--   0        0        0     3745 2022-07-24 03:34:34.555553 ooo_dev_tools-0.9.3/ooodev/utils/images.py
--rw-r--r--   0        0        0    15354 2023-04-06 02:13:48.647065 ooo_dev_tools-0.9.3/ooodev/utils/images_lo.py
--rw-r--r--   0        0        0    76912 2023-04-06 02:13:48.648067 ooo_dev_tools-0.9.3/ooodev/utils/info.py
--rw-r--r--   0        0        0        0 2022-10-27 15:27:12.066994 ooo_dev_tools-0.9.3/ooodev/utils/kind/__init__.py
--rw-r--r--   0        0        0      658 2022-11-05 19:28:56.359598 ooo_dev_tools-0.9.3/ooodev/utils/kind/axis_kind.py
--rw-r--r--   0        0        0     2943 2022-11-05 19:28:56.360598 ooo_dev_tools-0.9.3/ooodev/utils/kind/chart2_data_role_kind.py
--rw-r--r--   0        0        0     7423 2022-12-17 01:13:14.740079 ooo_dev_tools-0.9.3/ooodev/utils/kind/chart2_types.py
--rw-r--r--   0        0        0     1061 2022-11-05 19:28:56.361599 ooo_dev_tools-0.9.3/ooodev/utils/kind/chart_diagram_kind.py
--rw-r--r--   0        0        0     1979 2022-11-05 19:28:56.361599 ooo_dev_tools-0.9.3/ooodev/utils/kind/curve_kind.py
--rw-r--r--   0        0        0      893 2022-11-05 19:28:56.362600 ooo_dev_tools-0.9.3/ooodev/utils/kind/data_point_label_type_kind.py
--rw-r--r--   0        0        0      922 2022-11-05 19:28:56.363598 ooo_dev_tools-0.9.3/ooodev/utils/kind/data_point_lable_placement_kind.py
--rw-r--r--   0        0        0     1921 2022-11-05 19:28:56.364600 ooo_dev_tools-0.9.3/ooodev/utils/kind/drawing_bitmap_kind.py
--rw-r--r--   0        0        0     1510 2022-11-05 19:28:56.364600 ooo_dev_tools-0.9.3/ooodev/utils/kind/drawing_gradient_kind.py
--rw-r--r--   0        0        0     1781 2022-11-05 19:28:56.365599 ooo_dev_tools-0.9.3/ooodev/utils/kind/drawing_hatching_kind.py
--rw-r--r--   0        0        0     1053 2022-11-05 19:28:56.366599 ooo_dev_tools-0.9.3/ooodev/utils/kind/drawing_layer_kind.py
--rw-r--r--   0        0        0     1343 2022-11-05 19:28:56.367602 ooo_dev_tools-0.9.3/ooodev/utils/kind/drawing_name_space_kind.py
--rw-r--r--   0        0        0     2298 2022-11-05 19:28:56.368600 ooo_dev_tools-0.9.3/ooodev/utils/kind/drawing_shape_kind.py
--rw-r--r--   0        0        0     1123 2022-11-05 19:28:56.369599 ooo_dev_tools-0.9.3/ooodev/utils/kind/drawing_slide_show_kind.py
--rw-r--r--   0        0        0     2482 2022-11-05 19:28:56.370602 ooo_dev_tools-0.9.3/ooodev/utils/kind/form_component_kind.py
--rw-r--r--   0        0        0     1778 2022-11-05 19:28:56.371600 ooo_dev_tools-0.9.3/ooodev/utils/kind/form_control_kind.py
--rw-r--r--   0        0        0     1309 2022-11-05 19:28:56.371600 ooo_dev_tools-0.9.3/ooodev/utils/kind/gallery_kind.py
--rw-r--r--   0        0        0      945 2022-11-05 19:28:56.372599 ooo_dev_tools-0.9.3/ooodev/utils/kind/gallery_search_by_kind.py
--rw-r--r--   0        0        0      812 2022-11-05 19:28:56.373599 ooo_dev_tools-0.9.3/ooodev/utils/kind/glue_points_kind.py
--rw-r--r--   0        0        0     2878 2022-11-08 11:08:31.782891 ooo_dev_tools-0.9.3/ooodev/utils/kind/graphic_arrow_style_kind.py
--rw-r--r--   0        0        0     2131 2022-11-05 19:28:56.374601 ooo_dev_tools-0.9.3/ooodev/utils/kind/graphic_style_kind.py
--rw-r--r--   0        0        0     1526 2022-11-30 23:26:32.119139 ooo_dev_tools-0.9.3/ooodev/utils/kind/info_paths_kind.py
--rw-r--r--   0        0        0      209 2022-10-27 15:27:12.079996 ooo_dev_tools-0.9.3/ooodev/utils/kind/kind_base.py
--rw-r--r--   0        0        0     2389 2022-11-13 02:25:58.191785 ooo_dev_tools-0.9.3/ooodev/utils/kind/kind_helper.py
--rw-r--r--   0        0        0     1260 2022-11-05 19:28:56.376599 ooo_dev_tools-0.9.3/ooodev/utils/kind/line_style_name_kind.py
--rw-r--r--   0        0        0     2202 2022-11-05 19:28:56.377600 ooo_dev_tools-0.9.3/ooodev/utils/kind/presentation_kind.py
--rw-r--r--   0        0        0     1898 2022-11-13 02:25:58.191785 ooo_dev_tools-0.9.3/ooodev/utils/kind/presentation_layout_kind.py
--rw-r--r--   0        0        0     1146 2022-11-05 19:28:56.377600 ooo_dev_tools-0.9.3/ooodev/utils/kind/search_match_kind.py
--rw-r--r--   0        0        0      820 2022-11-05 19:28:56.378600 ooo_dev_tools-0.9.3/ooodev/utils/kind/shape_comb_kind.py
--rw-r--r--   0        0        0    99082 2023-04-06 02:13:48.650068 ooo_dev_tools-0.9.3/ooodev/utils/lo.py
--rw-r--r--   0        0        0     2783 2022-07-24 03:34:34.561536 ooo_dev_tools-0.9.3/ooodev/utils/lo_util.py
--rw-r--r--   0        0        0     8437 2022-11-25 03:43:11.801371 ooo_dev_tools-0.9.3/ooodev/utils/paths.py
--rw-r--r--   0        0        0    54910 2023-04-06 02:13:09.412095 ooo_dev_tools-0.9.3/ooodev/utils/props.py
--rw-r--r--   0        0        0     1896 2022-07-20 01:40:32.607380 ooo_dev_tools-0.9.3/ooodev/utils/script_context.py
--rw-r--r--   0        0        0    25588 2023-04-02 18:09:12.906574 ooo_dev_tools-0.9.3/ooodev/utils/selection.py
--rw-r--r--   0        0        0     6400 2022-10-31 22:59:24.504932 ooo_dev_tools-0.9.3/ooodev/utils/session.py
--rw-r--r--   0        0        0      727 2022-10-29 21:44:16.952005 ooo_dev_tools-0.9.3/ooodev/utils/sys_info.py
--rw-r--r--   0        0        0    26396 2023-04-02 18:09:12.907574 ooo_dev_tools-0.9.3/ooodev/utils/table_helper.py
--rw-r--r--   0        0        0     2023 2022-07-14 20:40:23.817443 ooo_dev_tools-0.9.3/ooodev/utils/text_transferable.py
--rw-r--r--   0        0        0     1453 2022-07-24 03:34:34.568523 ooo_dev_tools-0.9.3/ooodev/utils/type_var.py
--rw-r--r--   0        0        0     3478 2022-07-14 20:40:23.818235 ooo_dev_tools-0.9.3/ooodev/utils/uno_const.py
--rw-r--r--   0        0        0     6513 2022-10-04 00:14:04.247070 ooo_dev_tools-0.9.3/ooodev/utils/uno_enum.py
--rw-r--r--   0        0        0      562 2022-10-27 15:27:12.084993 ooo_dev_tools-0.9.3/ooodev/utils/validation.py
--rw-r--r--   0        0        0    11180 2022-11-25 03:43:11.802373 ooo_dev_tools-0.9.3/ooodev/utils/view_state.py
--rw-r--r--   0        0        0    18910 2022-07-24 03:34:47.735913 ooo_dev_tools-0.9.3/ooodev/utils/xml_util.py
--rw-r--r--   0        0        0        0 2022-07-16 02:19:46.806983 ooo_dev_tools-0.9.3/ooodev/wrapper/__init__.py
--rw-r--r--   0        0        0      929 2022-08-23 05:01:45.230317 ooo_dev_tools-0.9.3/ooodev/wrapper/break_context.py
--rw-r--r--   0        0        0     2342 2023-04-07 18:11:57.909888 ooo_dev_tools-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     5220 2023-04-07 18:06:32.049984 ooo_dev_tools-0.9.3/README.rst
--rw-r--r--   0        0        0     6770 1970-01-01 00:00:00.000000 ooo_dev_tools-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    10174 2022-06-09 05:52:04.135315 ooo_dev_tools-0.9.4/LICENSE
+-rw-r--r--   0        0        0      272 2023-04-21 22:38:52.804812 ooo_dev_tools-0.9.4/ooodev/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-29 00:27:48.235332 ooo_dev_tools-0.9.4/ooodev/adapter/__init__.py
+-rw-r--r--   0        0        0     1806 2022-11-29 00:27:48.236329 ooo_dev_tools-0.9.4/ooodev/adapter/adapter_base.py
+-rw-r--r--   0        0        0        0 2022-11-29 00:27:48.236329 ooo_dev_tools-0.9.4/ooodev/adapter/awt/__init__.py
+-rw-r--r--   0        0        0     3451 2022-12-03 04:37:37.329802 ooo_dev_tools-0.9.4/ooodev/adapter/awt/top_window_listener.py
+-rw-r--r--   0        0        0        0 2022-11-29 00:27:48.238329 ooo_dev_tools-0.9.4/ooodev/adapter/frame/__init__.py
+-rw-r--r--   0        0        0     2711 2022-12-03 04:37:37.330805 ooo_dev_tools-0.9.4/ooodev/adapter/frame/terminate_listener.py
+-rw-r--r--   0        0        0        0 2022-11-29 00:27:48.239328 ooo_dev_tools-0.9.4/ooodev/adapter/lang/__init__.py
+-rw-r--r--   0        0        0     1543 2022-12-03 04:37:37.330805 ooo_dev_tools-0.9.4/ooodev/adapter/lang/event_listener.py
+-rw-r--r--   0        0        0        0 2022-11-29 00:27:48.240329 ooo_dev_tools-0.9.4/ooodev/adapter/util/__init__.py
+-rw-r--r--   0        0        0     2336 2022-12-03 04:37:37.331804 ooo_dev_tools-0.9.4/ooodev/adapter/util/modify_listener.py
+-rw-r--r--   0        0        0        0 2022-11-29 00:27:48.241329 ooo_dev_tools-0.9.4/ooodev/adapter/view/__init__.py
+-rw-r--r--   0        0        0     2628 2023-04-06 02:13:08.626094 ooo_dev_tools-0.9.4/ooodev/adapter/view/selection_change_listener.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.785323 ooo_dev_tools-0.9.4/ooodev/cfg/__init__.py
+-rw-r--r--   0        0        0       89 2022-10-27 15:27:12.042995 ooo_dev_tools-0.9.4/ooodev/cfg/config.json
+-rw-r--r--   0        0        0     2012 2022-10-27 15:27:12.042995 ooo_dev_tools-0.9.4/ooodev/cfg/config.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.786382 ooo_dev_tools-0.9.4/ooodev/conn/__init__.py
+-rw-r--r--   0        0        0     5699 2022-07-14 20:40:23.787320 ooo_dev_tools-0.9.4/ooodev/conn/cache.py
+-rw-r--r--   0        0        0    18466 2023-04-06 02:13:08.627093 ooo_dev_tools-0.9.4/ooodev/conn/connect.py
+-rw-r--r--   0        0        0     6968 2022-12-20 23:59:58.431481 ooo_dev_tools-0.9.4/ooodev/conn/connectors.py
+-rw-r--r--   0        0        0        0 2022-10-27 15:27:12.043993 ooo_dev_tools-0.9.4/ooodev/dialog/__init__.py
+-rw-r--r--   0        0        0     3161 2022-11-05 19:29:24.377395 ooo_dev_tools-0.9.4/ooodev/dialog/input.py
+-rw-r--r--   0        0        0     2297 2022-11-13 02:25:58.183785 ooo_dev_tools-0.9.4/ooodev/dialog/msgbox.py
+-rw-r--r--   0        0        0     2019 2022-10-27 15:27:12.045993 ooo_dev_tools-0.9.4/ooodev/dialog/tk_input.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.789060 ooo_dev_tools-0.9.4/ooodev/events/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.789342 ooo_dev_tools-0.9.4/ooodev/events/args/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.789342 ooo_dev_tools-0.9.4/ooodev/events/args/calc/__init__.py
+-rw-r--r--   0        0        0     1371 2023-04-02 18:09:12.324621 ooo_dev_tools-0.9.4/ooodev/events/args/calc/cell_args.py
+-rw-r--r--   0        0        0     1461 2023-04-02 18:09:12.325621 ooo_dev_tools-0.9.4/ooodev/events/args/calc/cell_cancel_args.py
+-rw-r--r--   0        0        0     1590 2023-04-02 18:09:12.326621 ooo_dev_tools-0.9.4/ooodev/events/args/calc/sheet_args.py
+-rw-r--r--   0        0        0     1575 2023-04-02 18:09:12.327740 ooo_dev_tools-0.9.4/ooodev/events/args/calc/sheet_cancel_args.py
+-rw-r--r--   0        0        0     1451 2023-04-02 18:09:12.328623 ooo_dev_tools-0.9.4/ooodev/events/args/cancel_event_args.py
+-rw-r--r--   0        0        0     1163 2023-04-02 18:09:12.328745 ooo_dev_tools-0.9.4/ooodev/events/args/dispatch_args.py
+-rw-r--r--   0        0        0     1450 2023-04-02 18:09:12.329620 ooo_dev_tools-0.9.4/ooodev/events/args/dispatch_cancel_args.py
+-rw-r--r--   0        0        0     4051 2023-04-06 02:13:08.628097 ooo_dev_tools-0.9.4/ooodev/events/args/event_args.py
+-rw-r--r--   0        0        0      640 2022-11-29 00:27:48.243330 ooo_dev_tools-0.9.4/ooodev/events/args/generic_args.py
+-rw-r--r--   0        0        0     1366 2023-04-02 18:09:12.330620 ooo_dev_tools-0.9.4/ooodev/events/args/key_val_args.py
+-rw-r--r--   0        0        0     1608 2023-04-02 18:09:12.331622 ooo_dev_tools-0.9.4/ooodev/events/args/key_val_cancel_args.py
+-rw-r--r--   0        0        0     5995 2023-04-02 18:09:12.332622 ooo_dev_tools-0.9.4/ooodev/events/calc_named_event.py
+-rw-r--r--   0        0        0      863 2023-04-21 22:38:52.805814 ooo_dev_tools-0.9.4/ooodev/events/chart2_named_event.py
+-rw-r--r--   0        0        0      391 2022-11-29 00:27:48.244327 ooo_dev_tools-0.9.4/ooodev/events/command.py
+-rw-r--r--   0        0        0      312 2023-04-02 18:09:12.332622 ooo_dev_tools-0.9.4/ooodev/events/draw_named_event.py
+-rw-r--r--   0        0        0     4247 2023-04-02 18:09:12.333621 ooo_dev_tools-0.9.4/ooodev/events/event_singleton.py
+-rw-r--r--   0        0        0     3816 2023-04-21 22:38:52.807813 ooo_dev_tools-0.9.4/ooodev/events/format_named_event.py
+-rw-r--r--   0        0        0      210 2023-04-02 18:09:12.334621 ooo_dev_tools-0.9.4/ooodev/events/gbl_named_event.py
+-rw-r--r--   0        0        0     9544 2023-04-02 18:09:12.335620 ooo_dev_tools-0.9.4/ooodev/events/lo_events.py
+-rw-r--r--   0        0        0     3082 2023-04-02 18:09:12.336620 ooo_dev_tools-0.9.4/ooodev/events/lo_named_event.py
+-rw-r--r--   0        0        0     1022 2023-04-21 22:38:52.808814 ooo_dev_tools-0.9.4/ooodev/events/props_named_event.py
+-rw-r--r--   0        0        0     5175 2023-04-02 18:09:12.337911 ooo_dev_tools-0.9.4/ooodev/events/write_named_event.py
+-rw-r--r--   0        0        0        0 2022-06-09 05:52:04.175567 ooo_dev_tools-0.9.4/ooodev/exceptions/__init__.py
+-rw-r--r--   0        0        0     9928 2023-04-06 02:13:08.630095 ooo_dev_tools-0.9.4/ooodev/exceptions/ex.py
+-rw-r--r--   0        0        0      160 2023-04-06 02:13:08.630095 ooo_dev_tools-0.9.4/ooodev/format/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.339621 ooo_dev_tools-0.9.4/ooodev/format/calc/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.339621 ooo_dev_tools-0.9.4/ooodev/format/calc/direct/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.631093 ooo_dev_tools-0.9.4/ooodev/format/calc/direct/cell/__init__.py
+-rw-r--r--   0        0        0      812 2023-04-06 02:13:48.174066 ooo_dev_tools-0.9.4/ooodev/format/calc/direct/cell/alignment/__init__.py
+-rw-r--r--   0        0        0      108 2023-04-06 02:13:08.632095 ooo_dev_tools-0.9.4/ooodev/format/calc/direct/cell/background/__init__.py
+-rw-r--r--   0        0        0      782 2023-04-07 18:06:32.190987 ooo_dev_tools-0.9.4/ooodev/format/calc/direct/cell/borders/__init__.py
+-rw-r--r--   0        0        0      139 2023-04-06 02:13:08.633094 ooo_dev_tools-0.9.4/ooodev/format/calc/direct/cell/cell_protection/__init__.py
+-rw-r--r--   0        0        0     1376 2023-04-21 22:38:52.810814 ooo_dev_tools-0.9.4/ooodev/format/calc/direct/cell/font/__init__.py
+-rw-r--r--   0        0        0      281 2023-04-21 22:38:52.810814 ooo_dev_tools-0.9.4/ooodev/format/calc/direct/cell/numbers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.634096 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.634096 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/cell/__init__.py
+-rw-r--r--   0        0        0     1376 2023-04-06 02:13:08.635093 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/cell/alignment/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-06 02:13:08.635093 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/cell/background/__init__.py
+-rw-r--r--   0        0        0      852 2023-04-07 18:06:32.191986 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/cell/borders/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-06 02:13:08.636101 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/cell/cell_protection/__init__.py
+-rw-r--r--   0        0        0     1245 2023-04-06 02:13:08.637094 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/cell/font/__init__.py
+-rw-r--r--   0        0        0      530 2023-04-21 22:38:52.811812 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/cell/numbers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.637094 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/__init__.py
+-rw-r--r--   0        0        0     1123 2023-04-06 02:13:08.638093 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/area/__init__.py
+-rw-r--r--   0        0        0     1019 2023-04-06 02:13:08.638093 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/borders/__init__.py
+-rw-r--r--   0        0        0      276 2023-04-06 02:13:08.639095 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/footer/__init__.py
+-rw-r--r--   0        0        0     1100 2023-04-06 02:13:08.639095 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/footer/area/__init__.py
+-rw-r--r--   0        0        0     1005 2023-04-06 02:13:08.640095 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/footer/borders/__init__.py
+-rw-r--r--   0        0        0      290 2023-04-06 02:13:08.640095 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/header/__init__.py
+-rw-r--r--   0        0        0     1235 2023-04-06 02:13:08.641104 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/header/area/__init__.py
+-rw-r--r--   0        0        0     1112 2023-04-06 02:13:08.641104 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/header/borders/__init__.py
+-rw-r--r--   0        0        0     1162 2023-04-06 02:13:08.642093 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/page/__init__.py
+-rw-r--r--   0        0        0      708 2023-04-06 02:13:08.642093 ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/sheet/__init__.py
+-rw-r--r--   0        0        0      254 2023-04-06 02:13:48.198066 ooo_dev_tools-0.9.4/ooodev/format/calc/style/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.643095 ooo_dev_tools-0.9.4/ooodev/format/calc/style/cell/__init__.py
+-rw-r--r--   0        0        0     4313 2023-04-06 02:13:48.198066 ooo_dev_tools-0.9.4/ooodev/format/calc/style/cell/cell.py
+-rw-r--r--   0        0        0       60 2023-04-06 02:13:08.644094 ooo_dev_tools-0.9.4/ooodev/format/calc/style/cell/kind/__init__.py
+-rw-r--r--   0        0        0      588 2023-04-06 02:13:08.645093 ooo_dev_tools-0.9.4/ooodev/format/calc/style/cell/kind/style_cell_kind.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.645093 ooo_dev_tools-0.9.4/ooodev/format/calc/style/page/__init__.py
+-rw-r--r--   0        0        0       73 2023-04-06 02:13:08.645093 ooo_dev_tools-0.9.4/ooodev/format/calc/style/page/kind/__init__.py
+-rw-r--r--   0        0        0      207 2023-04-06 02:13:08.646094 ooo_dev_tools-0.9.4/ooodev/format/calc/style/page/kind/calc_style_page_kind.py
+-rw-r--r--   0        0        0     4101 2023-04-06 02:13:48.199068 ooo_dev_tools-0.9.4/ooodev/format/calc/style/page/page.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.812811 ooo_dev_tools-0.9.4/ooodev/format/chart2/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.812811 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.813814 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/axis/__init__.py
+-rw-r--r--   0        0        0     1096 2023-04-21 22:38:52.814813 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/axis/font/__init__.py
+-rw-r--r--   0        0        0      683 2023-04-21 22:38:52.815813 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/axis/label/__init__.py
+-rw-r--r--   0        0        0      305 2023-04-21 22:38:52.816814 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/axis/line/__init__.py
+-rw-r--r--   0        0        0      338 2023-04-21 22:38:52.816814 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/axis/numbers/__init__.py
+-rw-r--r--   0        0        0      887 2023-04-21 22:38:52.817814 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/axis/positioning/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.817814 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/general/__init__.py
+-rw-r--r--   0        0        0     1809 2023-04-21 22:38:52.846813 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/general/area/__init__.py
+-rw-r--r--   0        0        0      309 2023-04-21 22:38:52.847813 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/general/borders/__init__.py
+-rw-r--r--   0        0        0      339 2023-04-21 22:38:52.848815 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/general/numbers/__init__.py
+-rw-r--r--   0        0        0      212 2023-04-21 22:38:52.849814 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/general/position_size/__init__.py
+-rw-r--r--   0        0        0      519 2023-04-21 22:38:52.849814 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/general/transparency/__init__.py
+-rw-r--r--   0        0        0      309 2023-04-21 22:38:52.850816 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/grid/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.851814 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/legend/__init__.py
+-rw-r--r--   0        0        0     1812 2023-04-21 22:38:52.852816 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/legend/area/__init__.py
+-rw-r--r--   0        0        0      310 2023-04-21 22:38:52.853814 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/legend/borders/__init__.py
+-rw-r--r--   0        0        0     1280 2023-04-21 22:38:52.854812 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/legend/font/__init__.py
+-rw-r--r--   0        0        0      314 2023-04-21 22:38:52.855812 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/legend/position_size/__init__.py
+-rw-r--r--   0        0        0      521 2023-04-21 22:38:52.856812 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/legend/transparency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.856812 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/series/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.856812 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/series/data_labels/__init__.py
+-rw-r--r--   0        0        0      331 2023-04-21 22:38:52.857812 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/series/data_labels/borders/__init__.py
+-rw-r--r--   0        0        0     1314 2023-04-21 22:38:52.858810 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/series/data_labels/data_labels/__init__.py
+-rw-r--r--   0        0        0     1124 2023-04-21 22:38:52.858810 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/series/data_labels/font/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.859810 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/series/data_series/__init__.py
+-rw-r--r--   0        0        0     1874 2023-04-21 22:38:52.860814 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/series/data_series/area/__init__.py
+-rw-r--r--   0        0        0      331 2023-04-21 22:38:52.861814 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/series/data_series/borders/__init__.py
+-rw-r--r--   0        0        0     1085 2023-04-21 22:38:52.862812 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/series/data_series/options/__init__.py
+-rw-r--r--   0        0        0      545 2023-04-21 22:38:52.863814 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/series/data_series/transparency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.863814 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/title/__init__.py
+-rw-r--r--   0        0        0      357 2023-04-21 22:38:52.865811 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/title/alignment/__init__.py
+-rw-r--r--   0        0        0     1807 2023-04-21 22:38:52.866813 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/title/area/__init__.py
+-rw-r--r--   0        0        0      309 2023-04-21 22:38:52.867810 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/title/borders/__init__.py
+-rw-r--r--   0        0        0     1277 2023-04-21 22:38:52.868812 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/title/font/__init__.py
+-rw-r--r--   0        0        0      132 2023-04-21 22:38:52.870811 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/title/position_size/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.870811 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/wall/__init__.py
+-rw-r--r--   0        0        0     1804 2023-04-21 22:38:52.872811 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/wall/area/__init__.py
+-rw-r--r--   0        0        0      308 2023-04-21 22:38:52.873814 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/wall/borders/__init__.py
+-rw-r--r--   0        0        0      517 2023-04-21 22:38:52.874826 ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/wall/transparency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.403612 ooo_dev_tools-0.9.4/ooodev/format/draw/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.404613 ooo_dev_tools-0.9.4/ooodev/format/draw/direct/__init__.py
+-rw-r--r--   0        0        0     1401 2023-04-07 18:06:32.193000 ooo_dev_tools-0.9.4/ooodev/format/draw/direct/area/__init__.py
+-rw-r--r--   0        0        0      641 2023-04-06 02:13:08.648096 ooo_dev_tools-0.9.4/ooodev/format/draw/direct/transparency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.405614 ooo_dev_tools-0.9.4/ooodev/format/draw/modify/__init__.py
+-rw-r--r--   0        0        0      945 2023-04-06 02:13:08.675095 ooo_dev_tools-0.9.4/ooodev/format/draw/modify/area/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.406613 ooo_dev_tools-0.9.4/ooodev/format/draw/style/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-02 18:09:12.406613 ooo_dev_tools-0.9.4/ooodev/format/draw/style/kind/__init__.py
+-rw-r--r--   0        0        0     2652 2023-04-02 18:09:12.407617 ooo_dev_tools-0.9.4/ooodev/format/draw/style/lookup/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.408612 ooo_dev_tools-0.9.4/ooodev/format/impress/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.408612 ooo_dev_tools-0.9.4/ooodev/format/impress/modify/__init__.py
+-rw-r--r--   0        0        0      945 2023-04-06 02:13:08.676094 ooo_dev_tools-0.9.4/ooodev/format/impress/modify/area/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.677093 ooo_dev_tools-0.9.4/ooodev/format/inner/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.677093 ooo_dev_tools-0.9.4/ooodev/format/inner/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.677093 ooo_dev_tools-0.9.4/ooodev/format/inner/common/abstract/__init__.py
+-rw-r--r--   0        0        0     3954 2023-04-06 02:13:08.678094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/abstract/abstract_document.py
+-rw-r--r--   0        0        0     4577 2023-04-06 02:13:48.214066 ooo_dev_tools-0.9.4/ooodev/format/inner/common/abstract/abstract_fill_color.py
+-rw-r--r--   0        0        0    16076 2023-04-06 02:13:48.251066 ooo_dev_tools-0.9.4/ooodev/format/inner/common/abstract/abstract_hf.py
+-rw-r--r--   0        0        0     7849 2023-04-06 02:13:08.680093 ooo_dev_tools-0.9.4/ooodev/format/inner/common/abstract/abstract_line_number.py
+-rw-r--r--   0        0        0    11818 2023-04-06 02:13:08.681095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/abstract/abstract_padding.py
+-rw-r--r--   0        0        0    10284 2023-04-06 02:13:08.682094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/abstract/abstract_sides.py
+-rw-r--r--   0        0        0     5204 2023-04-21 22:38:52.877812 ooo_dev_tools-0.9.4/ooodev/format/inner/common/abstract/abstract_writing_mode.py
+-rw-r--r--   0        0        0     4323 2023-04-06 02:13:08.683094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/border_width_impl.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.683094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/format_types/__init__.py
+-rw-r--r--   0        0        0      262 2023-04-06 02:13:08.684096 ooo_dev_tools-0.9.4/ooodev/format/inner/common/format_types/offset_column.py
+-rw-r--r--   0        0        0      256 2023-04-06 02:13:08.684096 ooo_dev_tools-0.9.4/ooodev/format/inner/common/format_types/offset_row.py
+-rw-r--r--   0        0        0      252 2023-04-06 02:13:08.685095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/format_types/size_percent.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.685095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-06 02:13:08.685095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/area_gradient_props.py
+-rw-r--r--   0        0        0      324 2023-04-06 02:13:08.686095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/area_hatch_props.py
+-rw-r--r--   0        0        0      531 2023-04-06 02:13:08.686095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/area_img_props.py
+-rw-r--r--   0        0        0      294 2023-04-06 02:13:08.687092 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/area_pattern_props.py
+-rw-r--r--   0        0        0      187 2023-04-06 02:13:08.687092 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/border_props.py
+-rw-r--r--   0        0        0      181 2023-04-06 02:13:08.688095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/cell_background_color_props.py
+-rw-r--r--   0        0        0      650 2023-04-06 02:13:08.688095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/cell_borders_props.py
+-rw-r--r--   0        0        0      499 2023-04-06 02:13:08.689094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/cell_style_borders_props.py
+-rw-r--r--   0        0        0      238 2023-04-06 02:13:08.689094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/cell_text_align_props.py
+-rw-r--r--   0        0        0      197 2023-04-06 02:13:08.690093 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/cell_text_orientation_props.py
+-rw-r--r--   0        0        0      203 2023-04-06 02:13:08.690093 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/cell_text_properties_props.py
+-rw-r--r--   0        0        0      288 2023-04-06 02:13:08.691092 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/fill_color_props.py
+-rw-r--r--   0        0        0      179 2023-04-06 02:13:08.691092 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/font_only_props.py
+-rw-r--r--   0        0        0      176 2023-04-06 02:13:08.692095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/frame_options_align_props.py
+-rw-r--r--   0        0        0      196 2023-04-06 02:13:08.692095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/frame_options_names_props.py
+-rw-r--r--   0        0        0      239 2023-04-06 02:13:08.693095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/frame_options_properties.py
+-rw-r--r--   0        0        0      244 2023-04-06 02:13:08.693095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/frame_options_protect_props.py
+-rw-r--r--   0        0        0      166 2023-04-06 02:13:08.694094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/frame_type_anchor_props.py
+-rw-r--r--   0        0        0      445 2023-04-06 02:13:08.695094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/frame_type_positon_props.py
+-rw-r--r--   0        0        0      449 2023-04-06 02:13:08.695094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/frame_type_size_props.py
+-rw-r--r--   0        0        0      231 2023-04-06 02:13:08.696094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/frame_wrap_options_props.py
+-rw-r--r--   0        0        0      165 2023-04-06 02:13:08.696094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/frame_wrap_settings_props.py
+-rw-r--r--   0        0        0      628 2023-04-06 02:13:08.697094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/hf_props.py
+-rw-r--r--   0        0        0      313 2023-04-06 02:13:08.697094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/hyperlink_props.py
+-rw-r--r--   0        0        0      263 2023-04-06 02:13:08.698096 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/image_crop_props.py
+-rw-r--r--   0        0        0      253 2023-04-06 02:13:08.698096 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/image_flip_props.py
+-rw-r--r--   0        0        0      209 2023-04-06 02:13:08.699094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/image_options_names_props.py
+-rw-r--r--   0        0        0      168 2023-04-06 02:13:08.699094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/image_options_properties.py
+-rw-r--r--   0        0        0      154 2023-04-06 02:13:08.700095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/image_rotation_props.py
+-rw-r--r--   0        0        0      218 2023-04-06 02:13:08.700095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/img_para_area_props.py
+-rw-r--r--   0        0        0      178 2023-04-06 02:13:08.701096 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/list_style_props.py
+-rw-r--r--   0        0        0      207 2023-04-06 02:13:08.701096 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/page_margin_props.py
+-rw-r--r--   0        0        0      157 2023-04-06 02:13:08.702098 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/prop_pair.py
+-rw-r--r--   0        0        0      329 2023-04-06 02:13:08.702098 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/shape_shadow_props.py
+-rw-r--r--   0        0        0      319 2023-04-06 02:13:08.703097 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/struct_border_table_props.py
+-rw-r--r--   0        0        0      266 2023-04-06 02:13:08.703097 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/struct_cell_protection_props.py
+-rw-r--r--   0        0        0      235 2023-04-06 02:13:08.704097 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/struct_crop_props.py
+-rw-r--r--   0        0        0      349 2023-04-21 22:38:52.878811 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/struct_data_point_label_props.py
+-rw-r--r--   0        0        0      208 2023-04-06 02:13:08.704097 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/struct_size_props.py
+-rw-r--r--   0        0        0      333 2023-04-06 02:13:08.705094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/struct_table_border_distances_props.py
+-rw-r--r--   0        0        0      443 2023-04-06 02:13:08.705094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/table_borders_props.py
+-rw-r--r--   0        0        0      281 2023-04-06 02:13:08.706095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/table_properties_props.py
+-rw-r--r--   0        0        0      181 2023-04-21 22:38:52.879811 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/title_alignment_orientation_props.py
+-rw-r--r--   0        0        0      279 2023-04-06 02:13:08.706095 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/transparent_gradient_props.py
+-rw-r--r--   0        0        0      188 2023-04-06 02:13:08.707094 ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/transparent_transparency_props.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.707094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.747094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.783096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/alignment/__init__.py
+-rw-r--r--   0        0        0     6882 2023-04-06 02:13:08.785095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/alignment/properties.py
+-rw-r--r--   0        0        0     8619 2023-04-06 02:13:08.786095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/alignment/text_align.py
+-rw-r--r--   0        0        0     6213 2023-04-06 02:13:08.786095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/alignment/text_orientation.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.787101 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/background/__init__.py
+-rw-r--r--   0        0        0     5291 2023-04-06 02:13:48.252066 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/background/color.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.788097 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/border/__init__.py
+-rw-r--r--   0        0        0    21534 2023-04-07 18:06:32.194988 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/border/borders.py
+-rw-r--r--   0        0        0     3026 2023-04-06 02:13:08.789097 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/border/padding.py
+-rw-r--r--   0        0        0      759 2023-04-06 02:13:08.790094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/border/shadow.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.790094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/cell_protection/__init__.py
+-rw-r--r--   0        0        0      340 2023-04-06 02:13:08.790094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/cell_protection/cell_protection.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.879811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/char/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.880812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/char/font/__init__.py
+-rw-r--r--   0        0        0      737 2023-04-21 22:38:52.901810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/char/font/font.py
+-rw-r--r--   0        0        0      483 2023-04-21 22:38:52.902812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/char/font/font_effects.py
+-rw-r--r--   0        0        0      414 2023-04-21 22:38:52.903809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/char/font/font_only.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.903809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/numbers/__init__.py
+-rw-r--r--   0        0        0    13621 2023-04-21 22:38:52.905810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/numbers/numbers.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.791094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/page/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.791094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/page/page/__init__.py
+-rw-r--r--   0        0        0     6479 2023-04-06 02:13:08.792095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/page/page/layout_settings.py
+-rw-r--r--   0        0        0     7798 2023-04-06 02:13:08.792095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/page/page/margins.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.905810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.905810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.905810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/font/__init__.py
+-rw-r--r--   0        0        0      829 2023-04-21 22:38:52.906811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/font/font_effects.py
+-rw-r--r--   0        0        0     2473 2023-04-21 22:38:52.908813 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/font/font_only.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.908813 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/label/__init__.py
+-rw-r--r--   0        0        0     1727 2023-04-21 22:38:52.909824 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/label/order.py
+-rw-r--r--   0        0        0     3433 2023-04-21 22:38:52.910812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/label/orientation.py
+-rw-r--r--   0        0        0     1539 2023-04-21 22:38:52.911811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/label/show.py
+-rw-r--r--   0        0        0     2158 2023-04-21 22:38:52.912812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/label/text_flow.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.913810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/line/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-21 22:38:52.914812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/line/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.914812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/numbers/__init__.py
+-rw-r--r--   0        0        0      590 2023-04-21 22:38:52.915810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/numbers/numbers.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.916813 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/positioning/__init__.py
+-rw-r--r--   0        0        0     3064 2023-04-21 22:38:52.917813 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/positioning/axis_line.py
+-rw-r--r--   0        0        0     3481 2023-04-21 22:38:52.918812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/positioning/interval_marks.py
+-rw-r--r--   0        0        0     1757 2023-04-21 22:38:52.919811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/positioning/label_position.py
+-rw-r--r--   0        0        0     3043 2023-04-21 22:38:52.920814 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/axis/positioning/position_axis.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.920814 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/chart/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.920814 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/chart/area/__init__.py
+-rw-r--r--   0        0        0      895 2023-04-21 22:38:52.921812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/chart/area/color.py
+-rw-r--r--   0        0        0     7146 2023-04-21 22:38:52.923809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/chart/area/gradient.py
+-rw-r--r--   0        0        0     9958 2023-04-21 22:38:52.924811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/chart/area/hatch.py
+-rw-r--r--   0        0        0     7581 2023-04-21 22:38:52.925810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/chart/area/img.py
+-rw-r--r--   0        0        0     5901 2023-04-21 22:38:52.927811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/chart/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.927811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/chart/borders/__init__.py
+-rw-r--r--   0        0        0     4771 2023-04-21 22:38:52.928813 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/chart/borders/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.928813 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/chart/numbers/__init__.py
+-rw-r--r--   0        0        0     6352 2023-04-21 22:38:52.929814 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/chart/numbers/numbers.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.930811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/chart/transparent/__init__.py
+-rw-r--r--   0        0        0     5650 2023-04-21 22:38:52.931811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/chart/transparent/gradient.py
+-rw-r--r--   0        0        0     1173 2023-04-21 22:38:52.932812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/chart/transparent/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.932812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/grid/__init__.py
+-rw-r--r--   0        0        0     1542 2023-04-21 22:38:52.933812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/grid/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.934812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.934812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/area/__init__.py
+-rw-r--r--   0        0        0      213 2023-04-21 22:38:52.964809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/area/color.py
+-rw-r--r--   0        0        0      285 2023-04-21 22:38:52.965810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/area/gradient.py
+-rw-r--r--   0        0        0      224 2023-04-21 22:38:52.966812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/area/hatch.py
+-rw-r--r--   0        0        0      253 2023-04-21 22:38:52.968811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/area/img.py
+-rw-r--r--   0        0        0      236 2023-04-21 22:38:52.968811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.969809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/borders/__init__.py
+-rw-r--r--   0        0        0      279 2023-04-21 22:38:52.970810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/borders/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.970810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/font/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-21 22:38:52.971810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/font/font.py
+-rw-r--r--   0        0        0      561 2023-04-21 22:38:52.972810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/font/font_effects.py
+-rw-r--r--   0        0        0      465 2023-04-21 22:38:52.974809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/font/font_only.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.974809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/position/__init__.py
+-rw-r--r--   0        0        0     5243 2023-04-21 22:38:52.977808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/position/position.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.977808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/transparent/__init__.py
+-rw-r--r--   0        0        0      372 2023-04-21 22:38:52.978807 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/transparent/gradient.py
+-rw-r--r--   0        0        0      288 2023-04-21 22:38:52.980810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/legend/transparent/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.980810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/position_size/__init__.py
+-rw-r--r--   0        0        0     4171 2023-04-21 22:38:52.982808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/position_size/position.py
+-rw-r--r--   0        0        0     4066 2023-04-21 22:38:52.984808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/position_size/size.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.984808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/__index__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.985808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_labels/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.985808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_labels/borders/__init__.py
+-rw-r--r--   0        0        0     3112 2023-04-21 22:38:52.987811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_labels/borders/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.988809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/__init__.py
+-rw-r--r--   0        0        0     3326 2023-04-21 22:38:52.989811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/attrib_options.py
+-rw-r--r--   0        0        0     6717 2023-04-21 22:38:52.990810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/number_format.py
+-rw-r--r--   0        0        0     4193 2023-04-21 22:38:52.991808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/orientation.py
+-rw-r--r--   0        0        0     7580 2023-04-21 22:38:52.992811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/percent_format.py
+-rw-r--r--   0        0        0      250 2023-04-21 22:38:52.993811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/text_attribs.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:52.993811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_labels/font/__init__.py
+-rw-r--r--   0        0        0      867 2023-04-21 22:38:52.995812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_labels/font/font_effects.py
+-rw-r--r--   0        0        0     2511 2023-04-21 22:38:53.013808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_labels/font/font_only.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.013808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.014812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/area/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-21 22:38:53.015814 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/area/color.py
+-rw-r--r--   0        0        0      292 2023-04-21 22:38:53.015814 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/area/gradient.py
+-rw-r--r--   0        0        0      231 2023-04-21 22:38:53.016809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/area/hatch.py
+-rw-r--r--   0        0        0      260 2023-04-21 22:38:53.044807 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/area/img.py
+-rw-r--r--   0        0        0      243 2023-04-21 22:38:53.045811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.045811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/borders/__init__.py
+-rw-r--r--   0        0        0     5492 2023-04-21 22:38:53.047807 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/borders/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.047807 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/options/__init__.py
+-rw-r--r--   0        0        0     4504 2023-04-21 22:38:53.048812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/options/align_series.py
+-rw-r--r--   0        0        0     2841 2023-04-21 22:38:53.049809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/options/legend_entry.py
+-rw-r--r--   0        0        0     5033 2023-04-21 22:38:53.050813 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/options/orientation.py
+-rw-r--r--   0        0        0     2126 2023-04-21 22:38:53.051811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/options/plot.py
+-rw-r--r--   0        0        0     3329 2023-04-21 22:38:53.052811 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/options/plot_simple.py
+-rw-r--r--   0        0        0     6823 2023-04-21 22:38:53.053806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/options/settings.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.053806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/transparent/__init__.py
+-rw-r--r--   0        0        0      304 2023-04-21 22:38:53.054812 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/transparent/gradient.py
+-rw-r--r--   0        0        0      286 2023-04-21 22:38:53.055819 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/series/data_series/transparent/transparency.py
+-rw-r--r--   0        0        0     4171 2023-04-21 22:38:53.058807 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/alignment/direction.py
+-rw-r--r--   0        0        0     4313 2023-04-21 22:38:53.059809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/alignment/orientation.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.059809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/area/__init__.py
+-rw-r--r--   0        0        0      213 2023-04-21 22:38:53.060810 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/area/color.py
+-rw-r--r--   0        0        0      285 2023-04-21 22:38:53.061806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/area/gradient.py
+-rw-r--r--   0        0        0      224 2023-04-21 22:38:53.061806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/area/hatch.py
+-rw-r--r--   0        0        0      253 2023-04-21 22:38:53.062808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/area/img.py
+-rw-r--r--   0        0        0      236 2023-04-21 22:38:53.063805 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.063805 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/borders/__init__.py
+-rw-r--r--   0        0        0      278 2023-04-21 22:38:53.064808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/borders/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.064808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/font/__init__.py
+-rw-r--r--   0        0        0     6359 2023-04-21 22:38:53.066806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/font/font.py
+-rw-r--r--   0        0        0      918 2023-04-21 22:38:53.067808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/font/font_effects.py
+-rw-r--r--   0        0        0     2312 2023-04-21 22:38:53.068806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/font/font_only.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.068806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/position_size/__init__.py
+-rw-r--r--   0        0        0      880 2023-04-21 22:38:53.069809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/title/position_size/position.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.070809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/wall/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.070809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/wall/area/__init__.py
+-rw-r--r--   0        0        0      657 2023-04-21 22:38:53.071808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/wall/area/color.py
+-rw-r--r--   0        0        0      712 2023-04-21 22:38:53.072806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/wall/area/gradient.py
+-rw-r--r--   0        0        0      658 2023-04-21 22:38:53.073808 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/wall/area/hatch.py
+-rw-r--r--   0        0        0      686 2023-04-21 22:38:53.074804 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/wall/area/img.py
+-rw-r--r--   0        0        0      670 2023-04-21 22:38:53.075818 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/wall/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.075818 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/wall/borders/__init__.py
+-rw-r--r--   0        0        0      719 2023-04-21 22:38:53.076809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/wall/borders/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.077809 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/wall/transparent/__init__.py
+-rw-r--r--   0        0        0      725 2023-04-21 22:38:53.128803 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/wall/transparent/gradient.py
+-rw-r--r--   0        0        0     1040 2023-04-21 22:38:53.129807 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/chart2/wall/transparent/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:06:32.194988 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/draw/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:06:32.195989 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/draw/fill/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:06:32.195989 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/draw/fill/area/__init__.py
+-rw-r--r--   0        0        0      229 2023-04-07 18:06:32.196990 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/draw/fill/area/color.py
+-rw-r--r--   0        0        0      288 2023-04-07 18:06:32.197988 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/draw/fill/area/gradient.py
+-rw-r--r--   0        0        0      249 2023-04-07 18:06:32.198989 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/draw/fill/area/hatch.py
+-rw-r--r--   0        0        0      266 2023-04-07 18:06:32.199988 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/draw/fill/area/img.py
+-rw-r--r--   0        0        0      250 2023-04-07 18:06:32.200989 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/draw/fill/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.130807 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/draw/shape/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.130807 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/draw/shape/position_size/__init__.py
+-rw-r--r--   0        0        0     3378 2023-04-21 22:38:53.132806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/draw/shape/position_size/position.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.793096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/__init__.py
+-rw-r--r--   0        0        0     9315 2023-04-06 02:13:48.258068 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/cell_protection_struct.py
+-rw-r--r--   0        0        0    11233 2023-04-06 02:13:48.260066 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/crop_struct.py
+-rw-r--r--   0        0        0    11148 2023-04-21 22:38:53.133804 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/data_point_label_struct.py
+-rw-r--r--   0        0        0    10183 2023-04-06 02:13:48.262067 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/drop_cap_struct.py
+-rw-r--r--   0        0        0    14924 2023-04-21 22:38:53.134806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/gradient_struct.py
+-rw-r--r--   0        0        0     8274 2023-04-06 02:13:48.266068 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/hatch_struct.py
+-rw-r--r--   0        0        0    10085 2023-04-06 02:13:48.267067 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/line_spacing_struct.py
+-rw-r--r--   0        0        0    31720 2023-04-06 02:13:48.269067 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/locale_struct.py
+-rw-r--r--   0        0        0     7412 2023-04-21 22:38:53.135804 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/point_struct.py
+-rw-r--r--   0        0        0    11772 2023-04-21 22:38:53.137802 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/shadow_struct.py
+-rw-r--r--   0        0        0    25317 2023-04-06 02:13:48.277068 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/side.py
+-rw-r--r--   0        0        0     8482 2023-04-21 22:38:53.138806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/size_struct.py
+-rw-r--r--   0        0        0      640 2023-04-06 02:13:08.801095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/struct_base.py
+-rw-r--r--   0        0        0    13991 2023-04-06 02:13:48.280068 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/tab_stop_struct.py
+-rw-r--r--   0        0        0    13469 2023-04-06 02:13:48.281067 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/table_border_distances_struct.py
+-rw-r--r--   0        0        0    20841 2023-04-06 02:13:48.282066 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/table_border_struct.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.803095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.803095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.804095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/border/__init__.py
+-rw-r--r--   0        0        0    10508 2023-04-06 02:13:08.805096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/border/borders.py
+-rw-r--r--   0        0        0     2322 2023-04-06 02:13:08.805096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/border/padding.py
+-rw-r--r--   0        0        0     1239 2023-04-06 02:13:08.806095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/border/shadow.py
+-rw-r--r--   0        0        0     1766 2023-04-06 02:13:08.806095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/border/sides.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.807104 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/font/__init__.py
+-rw-r--r--   0        0        0    34693 2023-04-07 18:06:32.201988 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/font/font.py
+-rw-r--r--   0        0        0    26717 2023-04-21 22:38:53.140806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/font/font_effects.py
+-rw-r--r--   0        0        0    21095 2023-04-21 22:38:53.142806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/font/font_only.py
+-rw-r--r--   0        0        0    21143 2023-04-06 02:13:08.809094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/font/font_position.py
+-rw-r--r--   0        0        0        1 2023-04-06 02:13:08.810097 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/highlight/__init__.py
+-rw-r--r--   0        0        0     5150 2023-04-06 02:13:48.317067 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/highlight/highlight.py
+-rw-r--r--   0        0        0        1 2023-04-06 02:13:08.811097 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/hyperlink/__init__.py
+-rw-r--r--   0        0        0     5042 2023-04-06 02:13:08.812096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/hyperlink/hyperlink.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.812096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.812096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/area/__init__.py
+-rw-r--r--   0        0        0     2482 2023-04-06 02:13:08.813095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/area/fill_color.py
+-rw-r--r--   0        0        0    14136 2023-04-21 22:38:53.143807 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/area/gradient.py
+-rw-r--r--   0        0        0    13254 2023-04-21 22:38:53.145806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/area/hatch.py
+-rw-r--r--   0        0        0    18444 2023-04-21 22:38:53.147805 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/area/img.py
+-rw-r--r--   0        0        0    10537 2023-04-21 22:38:53.148807 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.837095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/transparent/__init__.py
+-rw-r--r--   0        0        0    12939 2023-04-21 22:38:53.150806 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/transparent/gradient.py
+-rw-r--r--   0        0        0     4966 2023-04-06 02:13:08.840097 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/transparent/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.852094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.852094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/frame_type/__init__.py
+-rw-r--r--   0        0        0     4866 2023-04-06 02:13:08.853094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/frame_type/anchor.py
+-rw-r--r--   0        0        0    18717 2023-04-06 02:13:08.866093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/frame_type/position.py
+-rw-r--r--   0        0        0     6874 2023-04-06 02:13:08.867093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/frame_type/size.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.867093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/hyperlink/__init__.py
+-rw-r--r--   0        0        0     4026 2023-04-06 02:13:08.868093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/hyperlink/image_map_options.py
+-rw-r--r--   0        0        0     5997 2023-04-06 02:13:08.869093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/hyperlink/link_to.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.869093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/options/__init__.py
+-rw-r--r--   0        0        0     4913 2023-04-06 02:13:08.870096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/options/align.py
+-rw-r--r--   0        0        0     8725 2023-04-06 02:13:08.871096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/options/names.py
+-rw-r--r--   0        0        0     9653 2023-04-06 02:13:08.871096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/options/properties.py
+-rw-r--r--   0        0        0     4781 2023-04-06 02:13:08.872094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/options/protect.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.872094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/wrap/__init__.py
+-rw-r--r--   0        0        0     7691 2023-04-06 02:13:08.873093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/wrap/options.py
+-rw-r--r--   0        0        0     3655 2023-04-06 02:13:08.873093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/wrap/settings.py
+-rw-r--r--   0        0        0     1796 2023-04-06 02:13:08.874109 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/wrap/spacing.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.874109 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.874109 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/crop/__init__.py
+-rw-r--r--   0        0        0    18759 2023-04-06 02:13:48.323067 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/crop/crop.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.875093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/image/__init__.py
+-rw-r--r--   0        0        0     5201 2023-04-06 02:13:08.876094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/image/flip.py
+-rw-r--r--   0        0        0     3716 2023-04-06 02:13:08.876094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/image/rotation.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.877095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/image_type/__init__.py
+-rw-r--r--   0        0        0    11093 2023-04-06 02:13:08.877095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/image_type/size.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.878097 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/options/__init__.py
+-rw-r--r--   0        0        0     2718 2023-04-06 02:13:08.878097 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/options/names.py
+-rw-r--r--   0        0        0     3786 2023-04-06 02:13:08.879093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/options/properties.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.879093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:48.323067 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/footer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:48.324069 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/footer/area/__init__.py
+-rw-r--r--   0        0        0      961 2023-04-06 02:13:48.325067 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/footer/area/color.py
+-rw-r--r--   0        0        0     1247 2023-04-06 02:13:48.325067 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/footer/area/gradient.py
+-rw-r--r--   0        0        0     1302 2023-04-06 02:13:48.326069 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/footer/area/hatch.py
+-rw-r--r--   0        0        0     1505 2023-04-06 02:13:48.326069 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/footer/area/img.py
+-rw-r--r--   0        0        0     1226 2023-04-06 02:13:48.327067 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/footer/area/pattern.py
+-rw-r--r--   0        0        0     1432 2023-04-06 02:13:48.328065 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/footer/footer.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:48.328065 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/header/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:48.329080 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/header/area/__init__.py
+-rw-r--r--   0        0        0     1376 2023-04-06 02:13:48.329080 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/header/area/color.py
+-rw-r--r--   0        0        0     1679 2023-04-06 02:13:48.359068 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/header/area/gradient.py
+-rw-r--r--   0        0        0     1815 2023-04-06 02:13:48.360070 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/header/area/hatch.py
+-rw-r--r--   0        0        0     1962 2023-04-06 02:13:48.361065 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/header/area/img.py
+-rw-r--r--   0        0        0     1683 2023-04-06 02:13:48.362067 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/header/area/pattern.py
+-rw-r--r--   0        0        0     1432 2023-04-06 02:13:48.413067 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/header/header.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.879093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/page/__init__.py
+-rw-r--r--   0        0        0     6554 2023-04-06 02:13:08.880098 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/page/layout_settings.py
+-rw-r--r--   0        0        0     3103 2023-04-06 02:13:08.881093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/page/margins.py
+-rw-r--r--   0        0        0     5382 2023-04-06 02:13:08.882094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/page/paper_format.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.882094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/__init__.py
+-rw-r--r--   0        0        0      389 2023-04-06 02:13:08.883094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/align/__init__.py
+-rw-r--r--   0        0        0    14994 2023-04-06 02:13:08.885097 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/align/alignment.py
+-rw-r--r--   0        0        0     3563 2023-04-21 22:38:53.151805 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/align/writing_mode.py
+-rw-r--r--   0        0        0        1 2023-04-06 02:13:08.886093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/area/__init__.py
+-rw-r--r--   0        0        0     1910 2023-04-06 02:13:08.887093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/area/color.py
+-rw-r--r--   0        0        0    15216 2023-04-06 02:13:48.416068 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/area/hatch.py
+-rw-r--r--   0        0        0    12082 2023-04-06 02:13:08.888094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/area/img.py
+-rw-r--r--   0        0        0     6846 2023-04-06 02:13:48.416068 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/area/pattern.py
+-rw-r--r--   0        0        0      471 2023-04-06 02:13:08.889093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/border/__init__.py
+-rw-r--r--   0        0        0    11804 2023-04-06 02:13:08.890095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/border/borders.py
+-rw-r--r--   0        0        0     2524 2023-04-06 02:13:08.890095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/border/padding.py
+-rw-r--r--   0        0        0      834 2023-04-06 02:13:08.891093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/border/shadow.py
+-rw-r--r--   0        0        0     2025 2023-04-06 02:13:08.892093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/border/sides.py
+-rw-r--r--   0        0        0        1 2023-04-06 02:13:08.892093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/drop_cap/__init__.py
+-rw-r--r--   0        0        0     9056 2023-04-06 02:13:08.893095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/drop_cap/drop_caps.py
+-rw-r--r--   0        0        0      303 2023-04-06 02:13:08.894096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/indent_space/__init__.py
+-rw-r--r--   0        0        0     9615 2023-04-06 02:13:08.894096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/indent_space/indent.py
+-rw-r--r--   0        0        0     8011 2023-04-06 02:13:08.895096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/indent_space/indent_spacing.py
+-rw-r--r--   0        0        0     7564 2023-04-06 02:13:48.417068 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/indent_space/line_spacing.py
+-rw-r--r--   0        0        0     8377 2023-04-06 02:13:08.916093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/indent_space/spacing.py
+-rw-r--r--   0        0        0      368 2023-04-06 02:13:08.917097 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/outline_list/__init__.py
+-rw-r--r--   0        0        0      879 2023-04-06 02:13:08.917097 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/outline_list/line_num.py
+-rw-r--r--   0        0        0     9905 2023-04-06 02:13:48.418067 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/outline_list/list_style.py
+-rw-r--r--   0        0        0     7452 2023-04-06 02:13:08.918095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/outline_list/outline.py
+-rw-r--r--   0        0        0     7022 2023-04-06 02:13:48.419065 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/outline_list/outline_list.py
+-rw-r--r--   0        0        0     2936 2023-04-06 02:13:08.920094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/padding.py
+-rw-r--r--   0        0        0      191 2023-04-06 02:13:08.920094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/tabs/__init__.py
+-rw-r--r--   0        0        0     8574 2023-04-06 02:13:08.921095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/tabs/tabs.py
+-rw-r--r--   0        0        0      261 2023-04-06 02:13:08.921095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/text_flow/__init__.py
+-rw-r--r--   0        0        0     6402 2023-04-06 02:13:08.922096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/text_flow/breaks.py
+-rw-r--r--   0        0        0    10238 2023-04-06 02:13:08.923093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/text_flow/flow_options.py
+-rw-r--r--   0        0        0    10123 2023-04-06 02:13:08.924094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/text_flow/hyphenation.py
+-rw-r--r--   0        0        0     7387 2023-04-06 02:13:08.924094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/text_flow/text_flow.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.924094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/transparent/__init__.py
+-rw-r--r--   0        0        0     3859 2023-04-06 02:13:08.925095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/transparent/gradient.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.925095 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/shape/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.926092 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/shape/area/__init__.py
+-rw-r--r--   0        0        0    16356 2023-04-06 02:13:48.420065 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/shape/area/shadow.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.927094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/table/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.927094 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/table/background/__init__.py
+-rw-r--r--   0        0        0     1127 2023-04-06 02:13:08.928093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/table/background/color.py
+-rw-r--r--   0        0        0     2513 2023-04-06 02:13:08.928093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/table/background/img.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.929096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/table/borders/__init__.py
+-rw-r--r--   0        0        0    18684 2023-04-06 02:13:08.929096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/table/borders/borders.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.929096 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/table/props/__init__.py
+-rw-r--r--   0        0        0    74782 2023-04-06 02:13:08.931093 ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/table/props/table_properties.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.931093 ooo_dev_tools-0.9.4/ooodev/format/inner/kind/__init__.py
+-rw-r--r--   0        0        0      231 2023-04-06 02:13:08.932094 ooo_dev_tools-0.9.4/ooodev/format/inner/kind/border_kind.py
+-rw-r--r--   0        0        0      509 2023-04-06 02:13:48.421066 ooo_dev_tools-0.9.4/ooodev/format/inner/kind/format_kind.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.932094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.933097 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.933097 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/alignment/__init__.py
+-rw-r--r--   0        0        0     3747 2023-04-06 02:13:08.934097 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/alignment/properties.py
+-rw-r--r--   0        0        0     3809 2023-04-06 02:13:08.935098 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/alignment/text_align.py
+-rw-r--r--   0        0        0     3655 2023-04-06 02:13:08.935098 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/alignment/text_orientation.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.935098 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/background/__init__.py
+-rw-r--r--   0        0        0     3261 2023-04-06 02:13:48.422065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/background/color.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.936097 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/border/__init__.py
+-rw-r--r--   0        0        0    23992 2023-04-07 18:06:32.203989 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/border/borders.py
+-rw-r--r--   0        0        0      172 2023-04-07 18:06:32.209987 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/border/padding.py
+-rw-r--r--   0        0        0      166 2023-04-07 18:06:32.210989 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/border/shadow.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.937094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/cell_protection/__init__.py
+-rw-r--r--   0        0        0     4681 2023-04-06 02:13:08.938093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/cell_protection/cell_protection.py
+-rw-r--r--   0        0        0     3739 2023-04-06 02:13:08.938093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/cell_style_base.py
+-rw-r--r--   0        0        0      820 2023-04-06 02:13:08.939094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/cell_style_base_multi.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.939094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/font/__init__.py
+-rw-r--r--   0        0        0     6013 2023-04-06 02:13:48.425066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/font/font_effects.py
+-rw-r--r--   0        0        0     4325 2023-04-06 02:13:08.941096 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/font/font_only.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:38:53.152804 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/numbers/__index__.py
+-rw-r--r--   0        0        0     4733 2023-04-21 22:38:53.153806 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/numbers/numbers.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.941096 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.941096 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/area/__init__.py
+-rw-r--r--   0        0        0     4943 2023-04-06 02:13:48.426066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/area/color.py
+-rw-r--r--   0        0        0     5808 2023-04-06 02:13:08.942093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/area/img.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.943095 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/border/__init__.py
+-rw-r--r--   0        0        0     5359 2023-04-06 02:13:08.943095 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/border/padding.py
+-rw-r--r--   0        0        0     4973 2023-04-06 02:13:48.426066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/border/shadow.py
+-rw-r--r--   0        0        0     5300 2023-04-06 02:13:08.945095 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/border/sides.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.945095 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.945095 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/area/__init__.py
+-rw-r--r--   0        0        0     1028 2023-04-06 02:13:48.427066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/area/color.py
+-rw-r--r--   0        0        0     1943 2023-04-06 02:13:48.428066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/area/img.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.947095 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/border/__init__.py
+-rw-r--r--   0        0        0     1095 2023-04-06 02:13:48.429066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/border/padding.py
+-rw-r--r--   0        0        0      917 2023-04-06 02:13:48.429066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/border/shadow.py
+-rw-r--r--   0        0        0     1092 2023-04-06 02:13:48.430065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/border/sides.py
+-rw-r--r--   0        0        0     1116 2023-04-06 02:13:48.431066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/footer.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.982094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.982094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/area/__init__.py
+-rw-r--r--   0        0        0     5283 2023-04-06 02:13:48.431066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/area/color.py
+-rw-r--r--   0        0        0     7094 2023-04-06 02:13:48.432068 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/area/img.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.984094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/border/__init__.py
+-rw-r--r--   0        0        0     6626 2023-04-06 02:13:48.433067 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/border/padding.py
+-rw-r--r--   0        0        0     6045 2023-04-06 02:13:48.434070 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/border/shadow.py
+-rw-r--r--   0        0        0     6289 2023-04-06 02:13:48.434070 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/border/sides.py
+-rw-r--r--   0        0        0     7271 2023-04-06 02:13:48.435066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/header.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.986093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/page/__init__.py
+-rw-r--r--   0        0        0     3819 2023-04-06 02:13:08.987094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/page/layout_settings.py
+-rw-r--r--   0        0        0     3565 2023-04-06 02:13:08.987094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/page/margins.py
+-rw-r--r--   0        0        0     4332 2023-04-06 02:13:08.988093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/page/paper_format.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.988093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/sheet/__init__.py
+-rw-r--r--   0        0        0     4051 2023-04-06 02:13:08.989095 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/sheet/order.py
+-rw-r--r--   0        0        0     7444 2023-04-06 02:13:08.989095 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/sheet/printing.py
+-rw-r--r--   0        0        0     3418 2023-04-06 02:13:08.990094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/sheet/scale_num_of_pages.py
+-rw-r--r--   0        0        0     4164 2023-04-06 02:13:08.991094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/sheet/scale_pages_width_height.py
+-rw-r--r--   0        0        0     3543 2023-04-06 02:13:08.991094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/sheet/scale_reduce_enlarge.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.991094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.992093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.992093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/border/__init__.py
+-rw-r--r--   0        0        0     3830 2023-04-06 02:13:08.993104 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/border/padding.py
+-rw-r--r--   0        0        0     3881 2023-04-06 02:13:48.436066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/border/shadow.py
+-rw-r--r--   0        0        0     3905 2023-04-06 02:13:08.994096 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/border/sides.py
+-rw-r--r--   0        0        0      701 2023-04-06 02:13:08.994096 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/char_style_base_multi.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.995093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/font/__init__.py
+-rw-r--r--   0        0        0     5324 2023-04-06 02:13:48.437065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/font/font_effects.py
+-rw-r--r--   0        0        0     3778 2023-04-06 02:13:08.996095 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/font/font_only.py
+-rw-r--r--   0        0        0     4855 2023-04-06 02:13:08.997094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/font/font_position.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.997094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/highlight/__init__.py
+-rw-r--r--   0        0        0     3099 2023-04-06 02:13:48.438068 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/highlight/highlight.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.998094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/fill/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.999094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/fill/area/__init__.py
+-rw-r--r--   0        0        0     5010 2023-04-06 02:13:48.439067 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/fill/area/img.py
+-rw-r--r--   0        0        0      686 2023-04-06 02:13:09.000093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/fill/fill_style_base_multi.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.001095 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.001095 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/area/__init__.py
+-rw-r--r--   0        0        0     3731 2023-04-06 02:13:48.440068 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/area/color.py
+-rw-r--r--   0        0        0     6551 2023-04-06 02:13:48.441068 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/area/gradient.py
+-rw-r--r--   0        0        0     5763 2023-04-06 02:13:48.442065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/area/hatch.py
+-rw-r--r--   0        0        0     6033 2023-04-06 02:13:09.004092 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/area/img.py
+-rw-r--r--   0        0        0     5246 2023-04-06 02:13:48.442065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.005095 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/border/__init__.py
+-rw-r--r--   0        0        0     4498 2023-04-06 02:13:09.006094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/border/padding.py
+-rw-r--r--   0        0        0     4409 2023-04-06 02:13:48.443065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/border/shadow.py
+-rw-r--r--   0        0        0     4309 2023-04-06 02:13:09.007094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/border/sides.py
+-rw-r--r--   0        0        0      742 2023-04-06 02:13:09.008093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/frame_style_base_multi.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.009094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/frame_type/__init__.py
+-rw-r--r--   0        0        0     3280 2023-04-06 02:13:09.009094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/frame_type/anchor.py
+-rw-r--r--   0        0        0     3895 2023-04-06 02:13:09.010094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/frame_type/position.py
+-rw-r--r--   0        0        0     3568 2023-04-06 02:13:09.011093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/frame_type/size.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.011093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/options/__init__.py
+-rw-r--r--   0        0        0     3294 2023-04-06 02:13:09.012094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/options/align.py
+-rw-r--r--   0        0        0     3551 2023-04-06 02:13:09.012094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/options/properties.py
+-rw-r--r--   0        0        0     3335 2023-04-06 02:13:09.013101 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/options/protect.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.013101 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/transparent/__init__.py
+-rw-r--r--   0        0        0     4635 2023-04-06 02:13:09.040094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/transparent/gradient.py
+-rw-r--r--   0        0        0     3782 2023-04-06 02:13:09.041093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/transparent/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.041093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/wrap/__init__.py
+-rw-r--r--   0        0        0     3838 2023-04-06 02:13:09.042094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/wrap/options.py
+-rw-r--r--   0        0        0     3185 2023-04-06 02:13:09.043094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/wrap/settings.py
+-rw-r--r--   0        0        0     3864 2023-04-06 02:13:09.043094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/wrap/spacing.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.044094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.044094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/area/__init__.py
+-rw-r--r--   0        0        0     4253 2023-04-06 02:13:48.444065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/area/color.py
+-rw-r--r--   0        0        0     6171 2023-04-06 02:13:48.444065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/area/gradient.py
+-rw-r--r--   0        0        0     5020 2023-04-06 02:13:48.445065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/area/hatch.py
+-rw-r--r--   0        0        0     5914 2023-04-06 02:13:09.046093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/area/img.py
+-rw-r--r--   0        0        0     4802 2023-04-06 02:13:48.446066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.047093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/border/__init__.py
+-rw-r--r--   0        0        0     3905 2023-04-06 02:13:09.048094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/border/padding.py
+-rw-r--r--   0        0        0     5049 2023-04-06 02:13:48.447065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/border/shadow.py
+-rw-r--r--   0        0        0     3829 2023-04-06 02:13:09.049093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/border/sides.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.049093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.049093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/area/__init__.py
+-rw-r--r--   0        0        0      892 2023-04-06 02:13:48.447065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/area/color.py
+-rw-r--r--   0        0        0     1072 2023-04-06 02:13:48.448067 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/area/gradient.py
+-rw-r--r--   0        0        0     1007 2023-04-06 02:13:48.449065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/area/hatch.py
+-rw-r--r--   0        0        0     1346 2023-04-06 02:13:48.449065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/area/img.py
+-rw-r--r--   0        0        0     1077 2023-04-06 02:13:48.450068 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.052094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/border/__init__.py
+-rw-r--r--   0        0        0     1052 2023-04-06 02:13:48.510066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/border/padding.py
+-rw-r--r--   0        0        0      976 2023-04-06 02:13:48.511066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/border/shadow.py
+-rw-r--r--   0        0        0      971 2023-04-06 02:13:48.511066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/border/sides.py
+-rw-r--r--   0        0        0     1176 2023-04-06 02:13:48.512066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/footer.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.055093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/transparency/__init__.py
+-rw-r--r--   0        0        0     1095 2023-04-06 02:13:48.513065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/transparency/gradient.py
+-rw-r--r--   0        0        0      994 2023-04-06 02:13:48.513065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/transparency/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.056092 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.057094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/area/__init__.py
+-rw-r--r--   0        0        0     5331 2023-04-06 02:13:48.514066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/area/color.py
+-rw-r--r--   0        0        0     7596 2023-04-06 02:13:48.515074 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/area/gradient.py
+-rw-r--r--   0        0        0     6455 2023-04-06 02:13:48.515074 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/area/hatch.py
+-rw-r--r--   0        0        0     7602 2023-04-06 02:13:48.516066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/area/img.py
+-rw-r--r--   0        0        0     6295 2023-04-06 02:13:48.517067 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.060095 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/border/__init__.py
+-rw-r--r--   0        0        0     6729 2023-04-06 02:13:48.517067 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/border/padding.py
+-rw-r--r--   0        0        0     6148 2023-04-06 02:13:48.518065 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/border/shadow.py
+-rw-r--r--   0        0        0     6403 2023-04-06 02:13:48.519066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/border/sides.py
+-rw-r--r--   0        0        0     7279 2023-04-06 02:13:48.519066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/header.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.063098 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/transparency/__init__.py
+-rw-r--r--   0        0        0     5959 2023-04-06 02:13:48.520064 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/transparency/gradient.py
+-rw-r--r--   0        0        0     4560 2023-04-06 02:13:48.521067 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/transparency/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.064093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/page/__init__.py
+-rw-r--r--   0        0        0     4052 2023-04-06 02:13:09.065093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/page/layout_settings.py
+-rw-r--r--   0        0        0     3750 2023-04-06 02:13:09.066093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/page/margins.py
+-rw-r--r--   0        0        0     4359 2023-04-06 02:13:09.066093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/page/paper_format.py
+-rw-r--r--   0        0        0      778 2023-04-06 02:13:09.066093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/page_style_base_multi.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.067093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/transparency/__init__.py
+-rw-r--r--   0        0        0     3751 2023-04-06 02:13:09.068093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/transparency/gradient.py
+-rw-r--r--   0        0        0     3261 2023-04-06 02:13:09.069094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/transparency/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.069094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.069094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/align/__init__.py
+-rw-r--r--   0        0        0     4517 2023-04-06 02:13:09.070093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/align/alignment.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.070093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/area/__init__.py
+-rw-r--r--   0        0        0     2740 2023-04-06 02:13:48.522066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/area/color.py
+-rw-r--r--   0        0        0     5562 2023-04-06 02:13:48.523066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/area/gradient.py
+-rw-r--r--   0        0        0     5340 2023-04-06 02:13:48.523066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/area/hatch.py
+-rw-r--r--   0        0        0     5005 2023-04-06 02:13:48.524066 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/area/img.py
+-rw-r--r--   0        0        0     4841 2023-04-06 02:13:09.073094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.073094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/border/__init__.py
+-rw-r--r--   0        0        0     4484 2023-04-06 02:13:09.085094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/border/borders.py
+-rw-r--r--   0        0        0     3853 2023-04-06 02:13:09.086093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/border/padding.py
+-rw-r--r--   0        0        0     3916 2023-04-06 02:13:48.525067 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/border/shadow.py
+-rw-r--r--   0        0        0     3752 2023-04-06 02:13:09.087092 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/border/sides.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.087092 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/drop_cap/__init__.py
+-rw-r--r--   0        0        0     3892 2023-04-06 02:13:09.088093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/drop_cap/drop_caps.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.088093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/font/__init__.py
+-rw-r--r--   0        0        0     5359 2023-04-06 02:13:48.565068 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/font/font_effects.py
+-rw-r--r--   0        0        0     3722 2023-04-06 02:13:09.089094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/font/font_only.py
+-rw-r--r--   0        0        0     4933 2023-04-06 02:13:09.090093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/font/font_position.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.090093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/highlight/__init__.py
+-rw-r--r--   0        0        0     3162 2023-04-06 02:13:48.570063 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/highlight/highlight.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.091092 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/indent_space/__init__.py
+-rw-r--r--   0        0        0     3715 2023-04-06 02:13:09.092093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/indent_space/indent.py
+-rw-r--r--   0        0        0     4124 2023-04-06 02:13:48.592064 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/indent_space/line_spacing.py
+-rw-r--r--   0        0        0     3555 2023-04-06 02:13:09.093094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/indent_space/spacing.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.093094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/outline_list/__init__.py
+-rw-r--r--   0        0        0     4065 2023-04-06 02:13:09.094093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/outline_list/line_num.py
+-rw-r--r--   0        0        0     8129 2023-04-06 02:13:09.095094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/outline_list/list_style.py
+-rw-r--r--   0        0        0     3214 2023-04-06 02:13:09.095094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/outline_list/outline.py
+-rw-r--r--   0        0        0      837 2023-04-06 02:13:09.096093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/para_style_base_multi.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.096093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/tabs/__init__.py
+-rw-r--r--   0        0        0     5372 2023-04-06 02:13:09.097093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/tabs/tabs.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.097093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/text_flow/__init__.py
+-rw-r--r--   0        0        0     3288 2023-04-06 02:13:09.099100 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/text_flow/breaks.py
+-rw-r--r--   0        0        0     3449 2023-04-06 02:13:09.110092 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/text_flow/flow_options.py
+-rw-r--r--   0        0        0     3577 2023-04-06 02:13:09.110092 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/text_flow/hyphenation.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.111094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/transparent/__init__.py
+-rw-r--r--   0        0        0     3765 2023-04-06 02:13:09.111094 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/transparent/gradient.py
+-rw-r--r--   0        0        0     3230 2023-04-06 02:13:09.112093 ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/transparent/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.112093 ooo_dev_tools-0.9.4/ooodev/format/inner/preset/__init__.py
+-rw-r--r--   0        0        0    28652 2023-04-21 22:38:53.154803 ooo_dev_tools-0.9.4/ooodev/format/inner/preset/preset_border_line.py
+-rw-r--r--   0        0        0     8819 2023-04-06 02:13:48.593066 ooo_dev_tools-0.9.4/ooodev/format/inner/preset/preset_gradient.py
+-rw-r--r--   0        0        0     7403 2023-04-06 02:13:48.594065 ooo_dev_tools-0.9.4/ooodev/format/inner/preset/preset_hatch.py
+-rw-r--r--   0        0        0  1674033 2023-04-06 02:13:09.129092 ooo_dev_tools-0.9.4/ooodev/format/inner/preset/preset_image.py
+-rw-r--r--   0        0        0     1257 2023-04-06 02:13:09.135093 ooo_dev_tools-0.9.4/ooodev/format/inner/preset/preset_paper_format.py
+-rw-r--r--   0        0        0     5884 2023-04-06 02:13:09.137094 ooo_dev_tools-0.9.4/ooodev/format/inner/preset/preset_pattern.py
+-rw-r--r--   0        0        0    53215 2023-04-21 22:38:53.155805 ooo_dev_tools-0.9.4/ooodev/format/inner/style_base.py
+-rw-r--r--   0        0        0    17583 2023-04-21 23:05:47.303361 ooo_dev_tools-0.9.4/ooodev/format/readme.md
+-rw-r--r--   0        0        0      738 2023-04-06 02:13:09.175094 ooo_dev_tools-0.9.4/ooodev/format/styler.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.738588 ooo_dev_tools-0.9.4/ooodev/format/writer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.738588 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.739586 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/char/__init__.py
+-rw-r--r--   0        0        0      957 2023-04-06 02:13:09.175094 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/char/borders/__init__.py
+-rw-r--r--   0        0        0     1687 2023-04-21 22:38:53.157803 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/char/font/__init__.py
+-rw-r--r--   0        0        0      129 2023-04-06 02:13:09.177094 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/char/highlight/__init__.py
+-rw-r--r--   0        0        0      238 2023-04-06 02:13:09.178103 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/char/hyperlink/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.741673 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/frame/__init__.py
+-rw-r--r--   0        0        0     2001 2023-04-06 02:13:09.178103 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/frame/area/__init__.py
+-rw-r--r--   0        0        0      636 2023-04-06 02:13:09.180093 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/frame/borders/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-06 02:13:09.181096 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/frame/hyperlink/__init__.py
+-rw-r--r--   0        0        0      653 2023-04-06 02:13:09.183092 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/frame/options/__init__.py
+-rw-r--r--   0        0        0      584 2023-04-06 02:13:09.184095 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/frame/transparency/__init__.py
+-rw-r--r--   0        0        0     1471 2023-04-06 02:13:09.184095 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/frame/type/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-06 02:13:09.185094 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/frame/wrap/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.753585 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/image/__init__.py
+-rw-r--r--   0        0        0     2001 2023-04-06 02:13:09.186092 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/image/area/__init__.py
+-rw-r--r--   0        0        0      636 2023-04-06 02:13:09.187095 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/image/borders/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-06 02:13:09.188095 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/image/crop/__init__.py
+-rw-r--r--   0        0        0      351 2023-04-06 02:13:09.188095 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/image/hyperlink/__init__.py
+-rw-r--r--   0        0        0      289 2023-04-06 02:13:09.189094 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/image/image/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-06 02:13:09.190093 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/image/options/__init__.py
+-rw-r--r--   0        0        0      584 2023-04-06 02:13:09.191094 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/image/transparency/__init__.py
+-rw-r--r--   0        0        0     1471 2023-04-06 02:13:09.191094 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/image/type/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-06 02:13:09.192094 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/image/wrap/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.758699 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/obj/__init__.py
+-rw-r--r--   0        0        0     2001 2023-04-06 02:13:09.193093 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/obj/area/__init__.py
+-rw-r--r--   0        0        0      636 2023-04-06 02:13:09.194093 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/obj/borders/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-06 02:13:09.194093 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/obj/hyperlink/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-06 02:13:09.196094 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/obj/options/__init__.py
+-rw-r--r--   0        0        0      584 2023-04-06 02:13:09.197093 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/obj/transparency/__init__.py
+-rw-r--r--   0        0        0     1471 2023-04-06 02:13:09.198094 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/obj/type/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-06 02:13:09.198094 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/obj/wrap/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:48.596069 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/page/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-06 02:13:48.597066 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/page/footer/__init__.py
+-rw-r--r--   0        0        0     1743 2023-04-06 02:13:48.598067 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/page/footer/area/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-06 02:13:48.598067 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/page/header/__init__.py
+-rw-r--r--   0        0        0     1743 2023-04-06 02:13:48.599067 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/page/header/area/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.766787 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/__init__.py
+-rw-r--r--   0        0        0      596 2023-04-06 02:13:09.199097 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/alignment/__init__.py
+-rw-r--r--   0        0        0     2067 2023-04-06 02:13:09.202093 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/area/__init__.py
+-rw-r--r--   0        0        0      838 2023-04-06 02:13:09.203094 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/borders/__init__.py
+-rw-r--r--   0        0        0      205 2023-04-06 02:13:09.204094 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/drop_caps/__init__.py
+-rw-r--r--   0        0        0      439 2023-04-06 02:13:09.205092 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/indent_space/__init__.py
+-rw-r--r--   0        0        0      517 2023-04-06 02:13:09.205092 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/outline_list/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-06 02:13:09.206092 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/tabs/__init__.py
+-rw-r--r--   0        0        0      406 2023-04-06 02:13:09.207091 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/text_flow/__init__.py
+-rw-r--r--   0        0        0      536 2023-04-06 02:13:09.207091 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/transparency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.773090 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/shape/__init__.py
+-rw-r--r--   0        0        0     1828 2023-04-21 22:38:53.158803 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/shape/area/__init__.py
+-rw-r--r--   0        0        0      396 2023-04-06 02:13:09.223094 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/shape/shadow/__init__.py
+-rw-r--r--   0        0        0      584 2023-04-06 02:13:09.223094 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/shape/transparency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.775216 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/table/__init__.py
+-rw-r--r--   0        0        0     1223 2023-04-06 02:13:09.224095 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/table/background/__init__.py
+-rw-r--r--   0        0        0      828 2023-04-06 02:13:09.225093 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/table/borders/__init__.py
+-rw-r--r--   0        0        0      265 2023-04-06 02:13:09.226093 ooo_dev_tools-0.9.4/ooodev/format/writer/direct/table/properties/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.776595 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.777629 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/char/__init__.py
+-rw-r--r--   0        0        0     1134 2023-04-06 02:13:09.228094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/char/borders/__init__.py
+-rw-r--r--   0        0        0     1683 2023-04-06 02:13:09.229095 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/char/font/__init__.py
+-rw-r--r--   0        0        0      346 2023-04-06 02:13:09.230094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/char/highlight/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.779585 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/frame/__init__.py
+-rw-r--r--   0        0        0     2421 2023-04-06 02:13:09.231100 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/frame/area/__init__.py
+-rw-r--r--   0        0        0     1091 2023-04-06 02:13:09.232094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/frame/borders/__init__.py
+-rw-r--r--   0        0        0     1034 2023-04-06 02:13:09.233093 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/frame/options/__init__.py
+-rw-r--r--   0        0        0      818 2023-04-06 02:13:09.233093 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/frame/transparency/__init__.py
+-rw-r--r--   0        0        0     1911 2023-04-06 02:13:09.234094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/frame/type/__init__.py
+-rw-r--r--   0        0        0      805 2023-04-06 02:13:09.235094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/frame/wrap/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.783676 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/__init__.py
+-rw-r--r--   0        0        0     2427 2023-04-06 02:13:48.600068 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/area/__init__.py
+-rw-r--r--   0        0        0     1105 2023-04-06 02:13:09.236092 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/borders/__init__.py
+-rw-r--r--   0        0        0      321 2023-04-06 02:13:09.237093 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/footer/__init__.py
+-rw-r--r--   0        0        0     2535 2023-04-06 02:13:09.237093 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/footer/area/__init__.py
+-rw-r--r--   0        0        0     1147 2023-04-06 02:13:09.238094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/footer/borders/__init__.py
+-rw-r--r--   0        0        0      995 2023-04-06 02:13:09.239092 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/footer/transparency/__init__.py
+-rw-r--r--   0        0        0      321 2023-04-06 02:13:09.239092 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/header/__init__.py
+-rw-r--r--   0        0        0     2535 2023-04-06 02:13:09.240096 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/header/area/__init__.py
+-rw-r--r--   0        0        0     1148 2023-04-06 02:13:09.241093 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/header/borders/__init__.py
+-rw-r--r--   0        0        0      995 2023-04-06 02:13:09.241093 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/header/transparency/__init__.py
+-rw-r--r--   0        0        0     1293 2023-04-06 02:13:09.242093 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/page/__init__.py
+-rw-r--r--   0        0        0     3526 2023-04-06 02:13:09.243093 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/page_style_base.py
+-rw-r--r--   0        0        0     3939 2023-04-06 02:13:09.246092 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/page_style_base_multi.py
+-rw-r--r--   0        0        0      958 2023-04-06 02:13:09.247094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/transparency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.792731 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/__init__.py
+-rw-r--r--   0        0        0      794 2023-04-06 02:13:09.249093 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/alignment/__init__.py
+-rw-r--r--   0        0        0     2297 2023-04-06 02:13:09.250094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/area/__init__.py
+-rw-r--r--   0        0        0     1347 2023-04-06 02:13:09.250094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/borders/__init__.py
+-rw-r--r--   0        0        0      402 2023-04-06 02:13:09.251094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/drop_caps/__init__.py
+-rw-r--r--   0        0        0     1685 2023-04-06 02:13:09.252093 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/font/__init__.py
+-rw-r--r--   0        0        0      319 2023-04-06 02:13:09.252093 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/highlight/__init__.py
+-rw-r--r--   0        0        0      880 2023-04-06 02:13:09.253094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/indent_space/__init__.py
+-rw-r--r--   0        0        0      955 2023-04-06 02:13:09.255094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/outline_list/__init__.py
+-rw-r--r--   0        0        0      446 2023-04-06 02:13:09.257094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/tabs/__init__.py
+-rw-r--r--   0        0        0      855 2023-04-06 02:13:09.257094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/text_flow/__init__.py
+-rw-r--r--   0        0        0      839 2023-04-06 02:13:09.258094 ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/transparency/__init__.py
+-rw-r--r--   0        0        0      750 2023-04-06 02:13:09.300094 ooo_dev_tools-0.9.4/ooodev/format/writer/style/__init__.py
+-rw-r--r--   0        0        0      110 2023-04-02 18:09:12.799670 ooo_dev_tools-0.9.4/ooodev/format/writer/style/bullet_list/__init__.py
+-rw-r--r--   0        0        0     4239 2023-04-06 02:13:48.601065 ooo_dev_tools-0.9.4/ooodev/format/writer/style/bullet_list/bullet_list.py
+-rw-r--r--   0        0        0      107 2023-04-02 18:09:12.800581 ooo_dev_tools-0.9.4/ooodev/format/writer/style/char/__init__.py
+-rw-r--r--   0        0        0     6741 2023-04-06 02:13:48.602067 ooo_dev_tools-0.9.4/ooodev/format/writer/style/char/char.py
+-rw-r--r--   0        0        0       60 2023-04-02 18:09:12.802395 ooo_dev_tools-0.9.4/ooodev/format/writer/style/char/kind/__init__.py
+-rw-r--r--   0        0        0     1135 2023-04-06 02:13:09.303093 ooo_dev_tools-0.9.4/ooodev/format/writer/style/char/kind/style_char_kind.py
+-rw-r--r--   0        0        0       97 2023-04-06 02:13:09.304092 ooo_dev_tools-0.9.4/ooodev/format/writer/style/frame/__init__.py
+-rw-r--r--   0        0        0     3704 2023-04-06 02:13:48.603067 ooo_dev_tools-0.9.4/ooodev/format/writer/style/frame/frame.py
+-rw-r--r--   0        0        0      353 2023-04-06 02:13:09.305109 ooo_dev_tools-0.9.4/ooodev/format/writer/style/frame/style_frame_kind.py
+-rw-r--r--   0        0        0       60 2023-04-02 18:09:12.804657 ooo_dev_tools-0.9.4/ooodev/format/writer/style/lst/__init__.py
+-rw-r--r--   0        0        0      791 2023-04-06 02:13:09.306094 ooo_dev_tools-0.9.4/ooodev/format/writer/style/lst/style_list_kind.py
+-rw-r--r--   0        0        0      115 2023-04-06 02:13:09.307094 ooo_dev_tools-0.9.4/ooodev/format/writer/style/page/__init__.py
+-rw-r--r--   0        0        0       79 2023-04-06 02:13:09.308096 ooo_dev_tools-0.9.4/ooodev/format/writer/style/page/kind/__init__.py
+-rw-r--r--   0        0        0      412 2023-04-06 02:13:09.309094 ooo_dev_tools-0.9.4/ooodev/format/writer/style/page/kind/writer_style_page_kind.py
+-rw-r--r--   0        0        0     4711 2023-04-06 02:13:48.605068 ooo_dev_tools-0.9.4/ooodev/format/writer/style/page/page.py
+-rw-r--r--   0        0        0       91 2023-04-03 22:12:05.347628 ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/__init__.py
+-rw-r--r--   0        0        0      579 2023-04-02 18:09:12.808625 ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/__init__.py
+-rw-r--r--   0        0        0      335 2023-04-06 02:13:09.310097 ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/style_chapter_kind.py
+-rw-r--r--   0        0        0      260 2023-04-06 02:13:09.311093 ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/style_para_cond_kind.py
+-rw-r--r--   0        0        0     1225 2023-04-06 02:13:09.312094 ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/style_para_html_kind.py
+-rw-r--r--   0        0        0     2105 2023-04-06 02:13:09.312094 ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/style_para_index_kind.py
+-rw-r--r--   0        0        0     4274 2023-04-06 02:13:09.313095 ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/style_para_kind.py
+-rw-r--r--   0        0        0     2492 2023-04-06 02:13:09.314095 ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/style_para_list_kind.py
+-rw-r--r--   0        0        0     1139 2023-04-06 02:13:09.316093 ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/style_para_special_kind.py
+-rw-r--r--   0        0        0     1278 2023-04-06 02:13:09.317099 ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/style_para_text_kind.py
+-rw-r--r--   0        0        0    11249 2023-04-06 02:13:48.607067 ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/para.py
+-rw-r--r--   0        0        0      218 2022-11-22 00:28:23.283709 ooo_dev_tools-0.9.4/ooodev/formatters/__init__.py
+-rw-r--r--   0        0        0     1185 2022-11-22 00:28:23.284709 ooo_dev_tools-0.9.4/ooodev/formatters/format_list_item.py
+-rw-r--r--   0        0        0     1101 2022-11-22 00:28:23.284709 ooo_dev_tools-0.9.4/ooodev/formatters/format_string.py
+-rw-r--r--   0        0        0     2540 2022-11-22 00:28:23.285710 ooo_dev_tools-0.9.4/ooodev/formatters/format_table_item.py
+-rw-r--r--   0        0        0     3182 2022-11-22 00:28:23.285710 ooo_dev_tools-0.9.4/ooodev/formatters/formatter_list.py
+-rw-r--r--   0        0        0    10394 2023-04-06 02:13:09.319094 ooo_dev_tools-0.9.4/ooodev/formatters/formatter_table.py
+-rw-r--r--   0        0        0      130 2022-11-22 00:28:23.287709 ooo_dev_tools-0.9.4/ooodev/formatters/only_ignore_kind.py
+-rw-r--r--   0        0        0      196 2022-11-22 00:28:23.287709 ooo_dev_tools-0.9.4/ooodev/formatters/string_kind.py
+-rw-r--r--   0        0        0      720 2022-11-22 00:28:23.288717 ooo_dev_tools-0.9.4/ooodev/formatters/table_item_kind.py
+-rw-r--r--   0        0        0     4482 2022-11-22 00:28:23.289713 ooo_dev_tools-0.9.4/ooodev/formatters/table_item_processer.py
+-rw-r--r--   0        0        0      336 2022-11-22 00:28:23.290711 ooo_dev_tools-0.9.4/ooodev/formatters/table_rule_kind.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.797175 ooo_dev_tools-0.9.4/ooodev/lazy/__init__.py
+-rw-r--r--   0        0        0     1551 2022-07-24 03:34:34.541590 ooo_dev_tools-0.9.4/ooodev/lazy/lazy_import.py
+-rw-r--r--   0        0        0        0 2022-06-09 05:52:04.176192 ooo_dev_tools-0.9.4/ooodev/listeners/__init__.py
+-rw-r--r--   0        0        0     1130 2022-07-20 01:40:32.577461 ooo_dev_tools-0.9.4/ooodev/listeners/x_event_adapter.py
+-rw-r--r--   0        0        0     1402 2022-07-20 01:40:32.578458 ooo_dev_tools-0.9.4/ooodev/listeners/x_modify_adapter.py
+-rw-r--r--   0        0        0     1355 2022-08-23 05:01:45.222321 ooo_dev_tools-0.9.4/ooodev/listeners/x_selection_change_adapter.py
+-rw-r--r--   0        0        0     1827 2022-07-20 01:40:32.580453 ooo_dev_tools-0.9.4/ooodev/listeners/x_terminate_adapter.py
+-rw-r--r--   0        0        0     2034 2022-07-20 01:40:32.581450 ooo_dev_tools-0.9.4/ooodev/listeners/x_top_window_adapter.py
+-rw-r--r--   0        0        0        0 2022-06-09 05:52:04.177777 ooo_dev_tools-0.9.4/ooodev/meta/__init__.py
+-rw-r--r--   0        0        0      518 2023-04-02 18:09:12.815585 ooo_dev_tools-0.9.4/ooodev/meta/class_property_readonly.py
+-rw-r--r--   0        0        0      545 2023-04-02 18:09:12.820755 ooo_dev_tools-0.9.4/ooodev/meta/deleted_attrib.py
+-rw-r--r--   0        0        0     1617 2023-04-02 18:09:12.821833 ooo_dev_tools-0.9.4/ooodev/meta/deleted_enum_meta.py
+-rw-r--r--   0        0        0      915 2023-04-02 18:09:12.822581 ooo_dev_tools-0.9.4/ooodev/meta/disabled_method.py
+-rw-r--r--   0        0        0      241 2022-07-14 20:40:23.800284 ooo_dev_tools-0.9.4/ooodev/meta/singleton.py
+-rw-r--r--   0        0        0     2135 2023-01-10 14:23:45.008570 ooo_dev_tools-0.9.4/ooodev/meta/static_meta.py
+-rw-r--r--   0        0        0      518 2023-04-02 18:09:12.822581 ooo_dev_tools-0.9.4/ooodev/meta/static_prop.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.801281 ooo_dev_tools-0.9.4/ooodev/mock/__init__.py
+-rw-r--r--   0        0        0      559 2022-07-14 20:40:23.801281 ooo_dev_tools-0.9.4/ooodev/mock/mock_g.py
+-rw-r--r--   0        0        0      579 2022-10-04 00:14:04.239070 ooo_dev_tools-0.9.4/ooodev/mock/unohelper.py
+-rw-r--r--   0        0        0        0 2022-06-09 05:51:34.370860 ooo_dev_tools-0.9.4/ooodev/office/__init__.py
+-rw-r--r--   0        0        0   265485 2023-04-21 22:38:53.162807 ooo_dev_tools-0.9.4/ooodev/office/calc.py
+-rw-r--r--   0        0        0    45621 2023-04-06 02:13:09.324093 ooo_dev_tools-0.9.4/ooodev/office/chart.py
+-rw-r--r--   0        0        0   114364 2023-04-22 15:05:38.537084 ooo_dev_tools-0.9.4/ooodev/office/chart2.py
+-rw-r--r--   0        0        0   135614 2023-04-06 02:13:48.632065 ooo_dev_tools-0.9.4/ooodev/office/draw.py
+-rw-r--r--   0        0        0   149599 2023-04-21 22:38:53.222801 ooo_dev_tools-0.9.4/ooodev/office/write.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.805270 ooo_dev_tools-0.9.4/ooodev/proto/__init__.py
+-rw-r--r--   0        0        0      626 2023-04-06 02:13:09.329093 ooo_dev_tools-0.9.4/ooodev/proto/dispatch_shape.py
+-rw-r--r--   0        0        0     1453 2023-04-06 02:13:09.329093 ooo_dev_tools-0.9.4/ooodev/proto/event_observer.py
+-rw-r--r--   0        0        0      450 2023-04-06 02:13:09.330101 ooo_dev_tools-0.9.4/ooodev/proto/size_obj.py
+-rw-r--r--   0        0        0     2394 2023-04-06 02:13:09.331094 ooo_dev_tools-0.9.4/ooodev/proto/style_obj.py
+-rw-r--r--   0        0        0      636 2023-04-06 02:13:48.635066 ooo_dev_tools-0.9.4/ooodev/theme/__init__.py
+-rw-r--r--   0        0        0     1604 2023-04-07 18:06:32.211989 ooo_dev_tools-0.9.4/ooodev/theme/theme.py
+-rw-r--r--   0        0        0     2212 2023-04-06 02:13:48.638067 ooo_dev_tools-0.9.4/ooodev/theme/theme_basic.py
+-rw-r--r--   0        0        0     4152 2023-04-06 02:13:48.639065 ooo_dev_tools-0.9.4/ooodev/theme/theme_calc.py
+-rw-r--r--   0        0        0      865 2023-04-06 02:13:48.640067 ooo_dev_tools-0.9.4/ooodev/theme/theme_draw.py
+-rw-r--r--   0        0        0     4342 2023-04-06 02:13:48.640067 ooo_dev_tools-0.9.4/ooodev/theme/theme_general.py
+-rw-r--r--   0        0        0     1416 2023-04-06 02:13:48.641076 ooo_dev_tools-0.9.4/ooodev/theme/theme_html.py
+-rw-r--r--   0        0        0     3982 2023-04-06 02:13:48.641076 ooo_dev_tools-0.9.4/ooodev/theme/theme_rpt_builder.py
+-rw-r--r--   0        0        0     2215 2023-04-06 02:13:48.642067 ooo_dev_tools-0.9.4/ooodev/theme/theme_sql.py
+-rw-r--r--   0        0        0     4975 2023-04-06 02:13:48.642067 ooo_dev_tools-0.9.4/ooodev/theme/theme_text_doc.py
+-rw-r--r--   0        0        0      820 2023-04-21 22:38:53.223801 ooo_dev_tools-0.9.4/ooodev/units/__init__.py
+-rw-r--r--   0        0        0     5979 2023-04-21 22:38:53.224804 ooo_dev_tools-0.9.4/ooodev/units/unit_cm.py
+-rw-r--r--   0        0        0     8844 2023-04-06 02:13:09.334092 ooo_dev_tools-0.9.4/ooodev/units/unit_convert.py
+-rw-r--r--   0        0        0     5352 2023-04-21 22:38:53.225808 ooo_dev_tools-0.9.4/ooodev/units/unit_inch.py
+-rw-r--r--   0        0        0     5394 2023-04-21 22:38:53.228802 ooo_dev_tools-0.9.4/ooodev/units/unit_inch10.py
+-rw-r--r--   0        0        0     5447 2023-04-21 22:38:53.230802 ooo_dev_tools-0.9.4/ooodev/units/unit_inch100.py
+-rw-r--r--   0        0        0     6082 2023-04-21 22:38:53.231801 ooo_dev_tools-0.9.4/ooodev/units/unit_inch1000.py
+-rw-r--r--   0        0        0     5897 2023-04-21 22:38:53.233802 ooo_dev_tools-0.9.4/ooodev/units/unit_mm.py
+-rw-r--r--   0        0        0     6131 2023-04-21 22:38:53.234804 ooo_dev_tools-0.9.4/ooodev/units/unit_mm10.py
+-rw-r--r--   0        0        0     6677 2023-04-21 22:38:53.235804 ooo_dev_tools-0.9.4/ooodev/units/unit_mm100.py
+-rw-r--r--   0        0        0     1329 2023-04-06 02:13:48.644066 ooo_dev_tools-0.9.4/ooodev/units/unit_obj.py
+-rw-r--r--   0        0        0     5700 2023-04-21 22:38:53.237801 ooo_dev_tools-0.9.4/ooodev/units/unit_pt.py
+-rw-r--r--   0        0        0     5960 2023-04-21 22:38:53.238801 ooo_dev_tools-0.9.4/ooodev/units/unit_px.py
+-rw-r--r--   0        0        0     1907 2022-07-14 20:40:23.806682 ooo_dev_tools-0.9.4/ooodev/utils/__init__.py
+-rw-r--r--   0        0        0    26819 2023-04-06 02:13:48.645065 ooo_dev_tools-0.9.4/ooodev/utils/color.py
+-rw-r--r--   0        0        0        0 2022-10-27 15:27:12.052996 ooo_dev_tools-0.9.4/ooodev/utils/data_type/__init__.py
+-rw-r--r--   0        0        0     2758 2023-04-02 18:09:12.852582 ooo_dev_tools-0.9.4/ooodev/utils/data_type/angle.py
+-rw-r--r--   0        0        0     3820 2022-12-17 01:13:14.728078 ooo_dev_tools-0.9.4/ooodev/utils/data_type/base_float_value.py
+-rw-r--r--   0        0        0     3785 2023-04-02 18:09:12.853581 ooo_dev_tools-0.9.4/ooodev/utils/data_type/base_int_value.py
+-rw-r--r--   0        0        0     1280 2023-04-02 18:09:12.874577 ooo_dev_tools-0.9.4/ooodev/utils/data_type/byte.py
+-rw-r--r--   0        0        0     1298 2023-04-02 18:09:12.875872 ooo_dev_tools-0.9.4/ooodev/utils/data_type/byte_signed.py
+-rw-r--r--   0        0        0    14993 2023-04-02 18:09:12.876578 ooo_dev_tools-0.9.4/ooodev/utils/data_type/cell_obj.py
+-rw-r--r--   0        0        0     3298 2023-04-02 18:09:12.877797 ooo_dev_tools-0.9.4/ooodev/utils/data_type/cell_values.py
+-rw-r--r--   0        0        0    10497 2023-04-06 02:13:09.375094 ooo_dev_tools-0.9.4/ooodev/utils/data_type/col_obj.py
+-rw-r--r--   0        0        0      522 2023-04-02 18:09:12.879580 ooo_dev_tools-0.9.4/ooodev/utils/data_type/color_range.py
+-rw-r--r--   0        0        0      195 2022-11-13 02:25:58.188785 ooo_dev_tools-0.9.4/ooodev/utils/data_type/dialog_title.py
+-rw-r--r--   0        0        0     1020 2023-04-02 18:09:12.880576 ooo_dev_tools-0.9.4/ooodev/utils/data_type/image_offset.py
+-rw-r--r--   0        0        0     1290 2023-04-02 18:09:12.882575 ooo_dev_tools-0.9.4/ooodev/utils/data_type/intensity.py
+-rw-r--r--   0        0        0      880 2023-04-06 02:13:09.376093 ooo_dev_tools-0.9.4/ooodev/utils/data_type/intensity_range.py
+-rw-r--r--   0        0        0      209 2023-04-02 18:09:12.884666 ooo_dev_tools-0.9.4/ooodev/utils/data_type/offset.py
+-rw-r--r--   0        0        0      431 2023-04-02 18:09:12.884666 ooo_dev_tools-0.9.4/ooodev/utils/data_type/point.py
+-rw-r--r--   0        0        0      482 2023-04-02 18:09:12.885575 ooo_dev_tools-0.9.4/ooodev/utils/data_type/point_positive.py
+-rw-r--r--   0        0        0     1282 2023-04-02 18:09:12.886577 ooo_dev_tools-0.9.4/ooodev/utils/data_type/poly_sides.py
+-rw-r--r--   0        0        0    22190 2023-04-06 02:13:09.377092 ooo_dev_tools-0.9.4/ooodev/utils/data_type/range_obj.py
+-rw-r--r--   0        0        0    15997 2023-04-06 02:13:09.402093 ooo_dev_tools-0.9.4/ooodev/utils/data_type/range_values.py
+-rw-r--r--   0        0        0     7314 2023-04-02 18:09:12.888579 ooo_dev_tools-0.9.4/ooodev/utils/data_type/row_obj.py
+-rw-r--r--   0        0        0     1993 2023-04-06 02:13:09.403093 ooo_dev_tools-0.9.4/ooodev/utils/data_type/size.py
+-rw-r--r--   0        0        0     3154 2023-04-06 02:13:09.404094 ooo_dev_tools-0.9.4/ooodev/utils/data_type/size_mm.py
+-rw-r--r--   0        0        0     1126 2023-04-02 18:09:12.890576 ooo_dev_tools-0.9.4/ooodev/utils/data_type/width_height_fraction.py
+-rw-r--r--   0        0        0      935 2023-04-02 18:09:12.891577 ooo_dev_tools-0.9.4/ooodev/utils/data_type/width_height_percent.py
+-rw-r--r--   0        0        0      270 2022-11-13 02:25:58.189784 ooo_dev_tools-0.9.4/ooodev/utils/data_type/window_title.py
+-rw-r--r--   0        0        0     5657 2022-12-10 17:01:36.559035 ooo_dev_tools-0.9.4/ooodev/utils/date_time_util.py
+-rw-r--r--   0        0        0        0 2022-10-27 15:27:12.055992 ooo_dev_tools-0.9.4/ooodev/utils/decorator/__init__.py
+-rw-r--r--   0        0        0     2736 2022-10-27 15:27:12.055992 ooo_dev_tools-0.9.4/ooodev/utils/decorator/enforce.py
+-rw-r--r--   0        0        0    24793 2023-04-06 02:13:09.404094 ooo_dev_tools-0.9.4/ooodev/utils/dialogs.py
+-rw-r--r--   0        0        0        0 2022-10-27 15:27:12.056992 ooo_dev_tools-0.9.4/ooodev/utils/dispatch/__init__.py
+-rw-r--r--   0        0        0     3178 2022-10-27 15:27:12.057993 ooo_dev_tools-0.9.4/ooodev/utils/dispatch/draw_drawing_dispatch.py
+-rw-r--r--   0        0        0     2806 2022-10-27 15:27:12.058992 ooo_dev_tools-0.9.4/ooodev/utils/dispatch/draw_view_dispatch.py
+-rw-r--r--   0        0        0     3180 2022-10-27 15:27:12.059993 ooo_dev_tools-0.9.4/ooodev/utils/dispatch/global_edit_dispatch.py
+-rw-r--r--   0        0        0     9772 2022-10-27 15:27:12.059993 ooo_dev_tools-0.9.4/ooodev/utils/dispatch/global_format_dispatch.py
+-rw-r--r--   0        0        0     2911 2022-10-27 15:27:12.060992 ooo_dev_tools-0.9.4/ooodev/utils/dispatch/global_view_dispatch.py
+-rw-r--r--   0        0        0    11843 2022-11-08 11:09:51.358105 ooo_dev_tools-0.9.4/ooodev/utils/dispatch/shape_dispatch_kind.py
+-rw-r--r--   0        0        0     1562 2022-07-24 03:34:47.720953 ooo_dev_tools-0.9.4/ooodev/utils/enum_helper.py
+-rw-r--r--   0        0        0    21457 2022-11-30 23:26:32.117139 ooo_dev_tools-0.9.4/ooodev/utils/file_io.py
+-rw-r--r--   0        0        0    44086 2023-04-06 02:13:48.646066 ooo_dev_tools-0.9.4/ooodev/utils/forms.py
+-rw-r--r--   0        0        0    21957 2023-04-02 18:09:12.895589 ooo_dev_tools-0.9.4/ooodev/utils/gallery.py
+-rw-r--r--   0        0        0     7499 2023-04-21 22:38:53.239802 ooo_dev_tools-0.9.4/ooodev/utils/gen_util.py
+-rw-r--r--   0        0        0    58911 2023-04-06 02:13:09.406094 ooo_dev_tools-0.9.4/ooodev/utils/gui.py
+-rw-r--r--   0        0        0     2062 2022-07-14 20:40:23.810268 ooo_dev_tools-0.9.4/ooodev/utils/image_transferable.py
+-rw-r--r--   0        0        0     3745 2022-07-24 03:34:34.555553 ooo_dev_tools-0.9.4/ooodev/utils/images.py
+-rw-r--r--   0        0        0    15354 2023-04-06 02:13:48.647065 ooo_dev_tools-0.9.4/ooodev/utils/images_lo.py
+-rw-r--r--   0        0        0    79006 2023-04-21 22:38:53.242801 ooo_dev_tools-0.9.4/ooodev/utils/info.py
+-rw-r--r--   0        0        0        0 2022-10-27 15:27:12.066994 ooo_dev_tools-0.9.4/ooodev/utils/kind/__init__.py
+-rw-r--r--   0        0        0      658 2022-11-05 19:28:56.359598 ooo_dev_tools-0.9.4/ooodev/utils/kind/axis_kind.py
+-rw-r--r--   0        0        0     2943 2022-11-05 19:28:56.360598 ooo_dev_tools-0.9.4/ooodev/utils/kind/chart2_data_role_kind.py
+-rw-r--r--   0        0        0     7423 2022-12-17 01:13:14.740079 ooo_dev_tools-0.9.4/ooodev/utils/kind/chart2_types.py
+-rw-r--r--   0        0        0     1061 2022-11-05 19:28:56.361599 ooo_dev_tools-0.9.4/ooodev/utils/kind/chart_diagram_kind.py
+-rw-r--r--   0        0        0     1979 2022-11-05 19:28:56.361599 ooo_dev_tools-0.9.4/ooodev/utils/kind/curve_kind.py
+-rw-r--r--   0        0        0      893 2022-11-05 19:28:56.362600 ooo_dev_tools-0.9.4/ooodev/utils/kind/data_point_label_type_kind.py
+-rw-r--r--   0        0        0      922 2022-11-05 19:28:56.363598 ooo_dev_tools-0.9.4/ooodev/utils/kind/data_point_lable_placement_kind.py
+-rw-r--r--   0        0        0     1921 2022-11-05 19:28:56.364600 ooo_dev_tools-0.9.4/ooodev/utils/kind/drawing_bitmap_kind.py
+-rw-r--r--   0        0        0     1510 2022-11-05 19:28:56.364600 ooo_dev_tools-0.9.4/ooodev/utils/kind/drawing_gradient_kind.py
+-rw-r--r--   0        0        0     1781 2022-11-05 19:28:56.365599 ooo_dev_tools-0.9.4/ooodev/utils/kind/drawing_hatching_kind.py
+-rw-r--r--   0        0        0     1053 2022-11-05 19:28:56.366599 ooo_dev_tools-0.9.4/ooodev/utils/kind/drawing_layer_kind.py
+-rw-r--r--   0        0        0     1343 2022-11-05 19:28:56.367602 ooo_dev_tools-0.9.4/ooodev/utils/kind/drawing_name_space_kind.py
+-rw-r--r--   0        0        0     2298 2022-11-05 19:28:56.368600 ooo_dev_tools-0.9.4/ooodev/utils/kind/drawing_shape_kind.py
+-rw-r--r--   0        0        0     1123 2022-11-05 19:28:56.369599 ooo_dev_tools-0.9.4/ooodev/utils/kind/drawing_slide_show_kind.py
+-rw-r--r--   0        0        0     2482 2022-11-05 19:28:56.370602 ooo_dev_tools-0.9.4/ooodev/utils/kind/form_component_kind.py
+-rw-r--r--   0        0        0     1778 2022-11-05 19:28:56.371600 ooo_dev_tools-0.9.4/ooodev/utils/kind/form_control_kind.py
+-rw-r--r--   0        0        0     1309 2022-11-05 19:28:56.371600 ooo_dev_tools-0.9.4/ooodev/utils/kind/gallery_kind.py
+-rw-r--r--   0        0        0      945 2022-11-05 19:28:56.372599 ooo_dev_tools-0.9.4/ooodev/utils/kind/gallery_search_by_kind.py
+-rw-r--r--   0        0        0      812 2022-11-05 19:28:56.373599 ooo_dev_tools-0.9.4/ooodev/utils/kind/glue_points_kind.py
+-rw-r--r--   0        0        0     2878 2022-11-08 11:08:31.782891 ooo_dev_tools-0.9.4/ooodev/utils/kind/graphic_arrow_style_kind.py
+-rw-r--r--   0        0        0     2131 2022-11-05 19:28:56.374601 ooo_dev_tools-0.9.4/ooodev/utils/kind/graphic_style_kind.py
+-rw-r--r--   0        0        0     1526 2022-11-30 23:26:32.119139 ooo_dev_tools-0.9.4/ooodev/utils/kind/info_paths_kind.py
+-rw-r--r--   0        0        0      209 2022-10-27 15:27:12.079996 ooo_dev_tools-0.9.4/ooodev/utils/kind/kind_base.py
+-rw-r--r--   0        0        0     2389 2022-11-13 02:25:58.191785 ooo_dev_tools-0.9.4/ooodev/utils/kind/kind_helper.py
+-rw-r--r--   0        0        0     1260 2022-11-05 19:28:56.376599 ooo_dev_tools-0.9.4/ooodev/utils/kind/line_style_name_kind.py
+-rw-r--r--   0        0        0     2202 2022-11-05 19:28:56.377600 ooo_dev_tools-0.9.4/ooodev/utils/kind/presentation_kind.py
+-rw-r--r--   0        0        0     1898 2022-11-13 02:25:58.191785 ooo_dev_tools-0.9.4/ooodev/utils/kind/presentation_layout_kind.py
+-rw-r--r--   0        0        0     1146 2022-11-05 19:28:56.377600 ooo_dev_tools-0.9.4/ooodev/utils/kind/search_match_kind.py
+-rw-r--r--   0        0        0     1183 2023-04-21 22:38:53.243803 ooo_dev_tools-0.9.4/ooodev/utils/kind/shape_base_point_kind.py
+-rw-r--r--   0        0        0      820 2022-11-05 19:28:56.378600 ooo_dev_tools-0.9.4/ooodev/utils/kind/shape_comb_kind.py
+-rw-r--r--   0        0        0    99082 2023-04-21 22:38:53.245804 ooo_dev_tools-0.9.4/ooodev/utils/lo.py
+-rw-r--r--   0        0        0     2783 2022-07-24 03:34:34.561536 ooo_dev_tools-0.9.4/ooodev/utils/lo_util.py
+-rw-r--r--   0        0        0     8437 2022-11-25 03:43:11.801371 ooo_dev_tools-0.9.4/ooodev/utils/paths.py
+-rw-r--r--   0        0        0    57557 2023-04-21 22:38:53.248801 ooo_dev_tools-0.9.4/ooodev/utils/props.py
+-rw-r--r--   0        0        0     1896 2022-07-20 01:40:32.607380 ooo_dev_tools-0.9.4/ooodev/utils/script_context.py
+-rw-r--r--   0        0        0    25545 2023-04-21 22:38:53.250802 ooo_dev_tools-0.9.4/ooodev/utils/selection.py
+-rw-r--r--   0        0        0     6400 2022-10-31 22:59:24.504932 ooo_dev_tools-0.9.4/ooodev/utils/session.py
+-rw-r--r--   0        0        0      727 2022-10-29 21:44:16.952005 ooo_dev_tools-0.9.4/ooodev/utils/sys_info.py
+-rw-r--r--   0        0        0    26396 2023-04-02 18:09:12.907574 ooo_dev_tools-0.9.4/ooodev/utils/table_helper.py
+-rw-r--r--   0        0        0     2023 2022-07-14 20:40:23.817443 ooo_dev_tools-0.9.4/ooodev/utils/text_transferable.py
+-rw-r--r--   0        0        0     1453 2022-07-24 03:34:34.568523 ooo_dev_tools-0.9.4/ooodev/utils/type_var.py
+-rw-r--r--   0        0        0     3478 2022-07-14 20:40:23.818235 ooo_dev_tools-0.9.4/ooodev/utils/uno_const.py
+-rw-r--r--   0        0        0     6513 2022-10-04 00:14:04.247070 ooo_dev_tools-0.9.4/ooodev/utils/uno_enum.py
+-rw-r--r--   0        0        0      562 2022-10-27 15:27:12.084993 ooo_dev_tools-0.9.4/ooodev/utils/validation.py
+-rw-r--r--   0        0        0    11180 2022-11-25 03:43:11.802373 ooo_dev_tools-0.9.4/ooodev/utils/view_state.py
+-rw-r--r--   0        0        0    18910 2022-07-24 03:34:47.735913 ooo_dev_tools-0.9.4/ooodev/utils/xml_util.py
+-rw-r--r--   0        0        0        0 2022-07-16 02:19:46.806983 ooo_dev_tools-0.9.4/ooodev/wrapper/__init__.py
+-rw-r--r--   0        0        0      929 2022-08-23 05:01:45.230317 ooo_dev_tools-0.9.4/ooodev/wrapper/break_context.py
+-rw-r--r--   0        0        0     2366 2023-04-21 22:38:53.304799 ooo_dev_tools-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     5220 2023-04-07 18:06:32.049984 ooo_dev_tools-0.9.4/README.rst
+-rw-r--r--   0        0        0     6770 1970-01-01 00:00:00.000000 ooo_dev_tools-0.9.4/PKG-INFO
```

### Comparing `ooo_dev_tools-0.9.3/LICENSE` & `ooo_dev_tools-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/adapter/adapter_base.py` & `ooo_dev_tools-0.9.4/ooodev/adapter/adapter_base.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/adapter/awt/top_window_listener.py` & `ooo_dev_tools-0.9.4/ooodev/adapter/awt/top_window_listener.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/adapter/frame/terminate_listener.py` & `ooo_dev_tools-0.9.4/ooodev/adapter/frame/terminate_listener.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/adapter/lang/event_listener.py` & `ooo_dev_tools-0.9.4/ooodev/adapter/lang/event_listener.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/adapter/util/modify_listener.py` & `ooo_dev_tools-0.9.4/ooodev/adapter/util/modify_listener.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/adapter/view/selection_change_listener.py` & `ooo_dev_tools-0.9.4/ooodev/adapter/view/selection_change_listener.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/cfg/config.py` & `ooo_dev_tools-0.9.4/ooodev/cfg/config.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/conn/cache.py` & `ooo_dev_tools-0.9.4/ooodev/conn/cache.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/conn/connect.py` & `ooo_dev_tools-0.9.4/ooodev/conn/connect.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/conn/connectors.py` & `ooo_dev_tools-0.9.4/ooodev/conn/connectors.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/dialog/input.py` & `ooo_dev_tools-0.9.4/ooodev/dialog/input.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/dialog/msgbox.py` & `ooo_dev_tools-0.9.4/ooodev/dialog/msgbox.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/dialog/tk_input.py` & `ooo_dev_tools-0.9.4/ooodev/dialog/tk_input.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/args/calc/cell_args.py` & `ooo_dev_tools-0.9.4/ooodev/events/args/calc/cell_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/args/calc/cell_cancel_args.py` & `ooo_dev_tools-0.9.4/ooodev/events/args/calc/cell_cancel_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/args/calc/sheet_args.py` & `ooo_dev_tools-0.9.4/ooodev/events/args/calc/sheet_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/args/calc/sheet_cancel_args.py` & `ooo_dev_tools-0.9.4/ooodev/events/args/calc/sheet_cancel_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/args/cancel_event_args.py` & `ooo_dev_tools-0.9.4/ooodev/events/args/cancel_event_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/args/dispatch_args.py` & `ooo_dev_tools-0.9.4/ooodev/events/args/dispatch_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/args/dispatch_cancel_args.py` & `ooo_dev_tools-0.9.4/ooodev/events/args/dispatch_cancel_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/args/event_args.py` & `ooo_dev_tools-0.9.4/ooodev/events/args/event_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/args/generic_args.py` & `ooo_dev_tools-0.9.4/ooodev/events/args/generic_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/args/key_val_args.py` & `ooo_dev_tools-0.9.4/ooodev/events/args/key_val_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/args/key_val_cancel_args.py` & `ooo_dev_tools-0.9.4/ooodev/events/args/key_val_cancel_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/calc_named_event.py` & `ooo_dev_tools-0.9.4/ooodev/events/calc_named_event.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/event_singleton.py` & `ooo_dev_tools-0.9.4/ooodev/events/event_singleton.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/format_named_event.py` & `ooo_dev_tools-0.9.4/ooodev/events/format_named_event.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,19 @@
     Triggers for each property being set on an UNO Object.
     """
     STYLE_PROPERTY_APPLIED = "format_style_prop_applied"
     """
     Style Property Applied. Event when property has been applied to an object.
     Triggers for each property that has been set on an UNO Object.
     """
+    STYLE_PROPERTY_ERROR = "format_style_prop_error"
+    """
+    Style Property Error. Event when property has failed to be applied for an object.
+    Triggers for each property that has been set on an UNO Object.
+    """
     STYLE_BACKING_UP = "format_style_backing_up"
     """Style Backing up"""
     STYLE_BACKED_UP = "format_style_backed_up"
     """Style Backed up"""
     STYLE_PROPERTY_RESTORING = "format_style_prop_restoring"
     """Style Restoring up"""
     STYLE_PROPERTY_RESTORED = "format_style_prop_restored"
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/lo_events.py` & `ooo_dev_tools-0.9.4/ooodev/events/lo_events.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/lo_named_event.py` & `ooo_dev_tools-0.9.4/ooodev/events/lo_named_event.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/props_named_event.py` & `ooo_dev_tools-0.9.4/ooodev/events/props_named_event.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 
 class PropsNamedEvent(NamedTuple):
     """
     Named events for utils.lo.LO class
     """
 
     PROP_SETTING = "props_setting"
-    """Prop setting command see :py:meth:`Props.set() <.utils.props.Props.set>`"""
+    """Prop setting command. See :py:meth:`Props.set() <.utils.props.Props.set>`"""
     PROP_SET = "props_set"
-    """Prop set command see :py:meth:`Props.set() <.utils.props.Props.set>`"""
+    """Prop set command. See :py:meth:`Props.set() <.utils.props.Props.set>`"""
+    PROP_SET_ERROR = "props_set_error"
+    """Prop set command error. See :py:meth:`Props.set() <.utils.props.Props.set>`"""
 
     PROP_DEFAULT_SETTING = "props_default_setting"
-    """Prop setting default command see :py:meth:`Props.set_default() <.utils.props.Props.set_default>`"""
+    """Prop setting default command. See :py:meth:`Props.set_default() <.utils.props.Props.set_default>`"""
     PROP_DEFAULT_SET = "props_default_set"
-    """Prop set default command see :py:meth:`Props.set_default() <.utils.props.Props.set_default>`"""
+    """Prop setting default command. See :py:meth:`Props.set_default() <.utils.props.Props.set_default>`"""
+    PROP_SET_DEFAULT_ERROR = "props_default_set_error"
+    """Prop setting command error. See :py:meth:`Props.set_default() <.utils.props.Props.set_default>`"""
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/events/write_named_event.py` & `ooo_dev_tools-0.9.4/ooodev/events/write_named_event.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/exceptions/ex.py` & `ooo_dev_tools-0.9.4/ooodev/exceptions/ex.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/direct/cell/alignment/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/direct/cell/alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/direct/cell/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/direct/cell/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/direct/cell/font/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/chart2/direct/title/font/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import uno
 from ooo.dyn.awt.char_set import CharSetEnum as CharSetEnum
+from ooo.dyn.awt.font_family import FontFamilyEnum as FontFamilyEnum
 from ooo.dyn.awt.font_relief import FontReliefEnum as FontReliefEnum
 from ooo.dyn.awt.font_slant import FontSlant as FontSlant
 from ooo.dyn.awt.font_strikeout import FontStrikeoutEnum as FontStrikeoutEnum
 from ooo.dyn.awt.font_underline import FontUnderlineEnum as FontUnderlineEnum
 from ooo.dyn.awt.font_weight import FontWeightEnum as FontWeightEnum
 from ooo.dyn.style.case_map import CaseMapEnum as CaseMapEnum
 from ooo.dyn.table.shadow_format import ShadowFormat as ShadowFormat
 from ooo.dyn.table.shadow_location import ShadowLocation as ShadowLocation
-from ooodev.utils.data_type.intensity import Intensity as Intensity
-from ooodev.format.inner.direct.write.char.font.font import Font as Font
-from ooodev.format.inner.direct.write.char.font.font_effects import FontEffects as FontEffects
+
+from ooodev.format.inner.direct.chart2.title.font.font import Font as Font
+from ooodev.format.inner.direct.chart2.title.font.font_effects import FontEffects as FontEffects
+from ooodev.format.inner.direct.chart2.title.font.font_only import FontOnly as FontOnly
 from ooodev.format.inner.direct.write.char.font.font_effects import FontLine as FontLine
 from ooodev.format.inner.direct.write.char.font.font_only import FontLang as FontLang
-from ooodev.format.inner.direct.write.char.font.font_only import FontOnly as FontOnly
-from ooodev.format.inner.direct.write.char.font.font_position import CharSpacingKind as CharSpacingKind
-from ooodev.format.inner.direct.write.char.font.font_position import FontScriptKind as FontScriptKind
+from ooodev.format.writer.style.char.kind.style_char_kind import StyleCharKind as StyleCharKind
 
 __all__ = ["Font", "FontEffects", "FontOnly"]
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/modify/cell/alignment/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/modify/cell/alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/modify/cell/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/modify/cell/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/modify/cell/font/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/modify/cell/font/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/footer/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/footer/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/footer/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/footer/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/header/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/header/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/header/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/header/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/page/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/page/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/modify/page/sheet/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/modify/page/sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/style/cell/cell.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/style/cell/cell.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/style/cell/kind/style_cell_kind.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/style/cell/kind/style_cell_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/calc/style/page/page.py` & `ooo_dev_tools-0.9.4/ooodev/format/calc/style/page/page.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/draw/direct/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/draw/direct/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/draw/direct/transparency/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/draw/direct/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/draw/modify/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/draw/modify/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/draw/style/lookup/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/draw/style/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/impress/modify/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/impress/modify/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/common/abstract/abstract_document.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/common/abstract/abstract_document.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/common/abstract/abstract_fill_color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/common/abstract/abstract_fill_color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/common/abstract/abstract_hf.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/common/abstract/abstract_hf.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/common/abstract/abstract_line_number.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/common/abstract/abstract_line_number.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/common/abstract/abstract_padding.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/common/abstract/abstract_padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/common/abstract/abstract_sides.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/common/abstract/abstract_sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/common/border_width_impl.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/common/border_width_impl.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/area_img_props.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/area_img_props.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/cell_borders_props.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/cell_borders_props.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/common/props/hf_props.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/common/props/hf_props.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/alignment/properties.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/alignment/properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/alignment/text_align.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/alignment/text_align.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/alignment/text_orientation.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/alignment/text_orientation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/background/color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/background/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/border/borders.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/border/borders.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/border/padding.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/border/shadow.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/page/page/layout_settings.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/page/page/layout_settings.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/calc/page/page/margins.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/calc/page/page/margins.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/cell_protection_struct.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/cell_protection_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/crop_struct.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/crop_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/drop_cap_struct.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/drop_cap_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/gradient_struct.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/gradient_struct.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,17 @@
         Args:
             obj (object): UNO object.
 
         Returns:
             None:
         """
         # override_dv
+        p_name = self._get_property_name()
+        if not p_name:
+            return
         if not mProps.Props.has(obj, self._get_property_name()):
             self._print_not_valid_srv("apply")
             return
 
         grad = self.get_uno_struct()
         props = {self._get_property_name(): grad}
         super().apply(obj=obj, override_dv=props)
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/hatch_struct.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/hatch_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/line_spacing_struct.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/line_spacing_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/locale_struct.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/locale_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/shadow_struct.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/shadow_struct.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-"""
-Module for Shadow format (``ShadowFormat``) struct.
-
-.. versionadded:: 0.9.0
-"""
 # region Import
 from __future__ import annotations
 from typing import Any, Dict, Tuple, Type, cast, overload, TypeVar
 
 import uno
 from ooo.dyn.table.shadow_format import ShadowFormat as ShadowFormat
 from ooo.dyn.table.shadow_location import ShadowLocation as ShadowLocation
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/side.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/side.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/size_struct.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/size_struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-"""
-Module for Image Crop (``GraphicCrop``) struct
-
-.. versionadded:: 0.9.0
-"""
 # region Import
 from __future__ import annotations
 from typing import Tuple, Type, cast, overload, TypeVar
 
 from ooo.dyn.awt.size import Size
 
 from ooodev.exceptions import ex as mEx
@@ -116,20 +111,23 @@
 
         Args:
             obj (object): UNO object.
 
         Returns:
             None:
         """
-        if not mProps.Props.has(obj, self._get_property_name()):
+        name = self._get_property_name()
+        if not name:
+            return
+        if not mProps.Props.has(obj, name):
             self._print_not_valid_srv("apply")
             return
 
         grad = self.get_uno_struct()
-        props = {self._get_property_name(): grad}
+        props = {name: grad}
         super().apply(obj=obj, override_dv=props)
 
     # endregion apply()
 
     # endregion overrides methods
 
     # region static methods
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/struct_base.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/struct_base.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/tab_stop_struct.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/tab_stop_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/table_border_distances_struct.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/table_border_distances_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/structs/table_border_struct.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/table_border_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/border/borders.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/border/borders.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/border/padding.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/border/shadow.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/border/sides.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/font/font.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/font/font.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/font/font_effects.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/font/font_effects.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,15 @@
             return self._supported_services_values
         except AttributeError:
             self._supported_services_values = (
                 "com.sun.star.style.CharacterProperties",
                 "com.sun.star.style.CharacterStyle",
                 "com.sun.star.style.ParagraphStyle",
                 "com.sun.star.drawing.ControlShape",
+                "com.sun.star.chart2.Legend",
             )
         return self._supported_services_values
 
     def _on_modifying(self, source: Any, event: CancelEventArgs) -> None:
         if self._is_default_inst:
             raise ValueError("Modifying a default instance is not allowed")
         return super()._on_modifying(source, event)
@@ -178,22 +179,14 @@
             obj (object): UNO object that has supports ``com.sun.star.style.CharacterProperties`` service.
 
         Returns:
             None:
         """
         super().apply(obj, **kwargs)
 
-    def _props_set(self, obj: object, **kwargs: Any) -> None:
-        try:
-            super()._props_set(obj, **kwargs)
-        except mEx.MultiError as e:
-            mLo.Lo.print(f"Font.apply(): Unable to set Property")
-            for err in e.errors:
-                mLo.Lo.print(f"  {err}")
-
     # endregion apply()
     # region from_obj()
     @overload
     @classmethod
     def from_obj(cls: Type[_TFontEffects], obj: object) -> _TFontEffects:
         ...
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/font/font_only.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/font/font_only.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,22 +202,14 @@
             obj (object): UNO object that has supports ``com.sun.star.style.CharacterProperties`` service.
 
         Returns:
             None:
         """
         super().apply(obj, **kwargs)
 
-    def _props_set(self, obj: object, **kwargs: Any) -> None:
-        try:
-            super()._props_set(obj, **kwargs)
-        except mEx.MultiError as e:
-            mLo.Lo.print(f"FontOnly.apply(): Unable to set Property")
-            for err in e.errors:
-                mLo.Lo.print(f"  {err}")
-
     # endregion apply()
 
     # endregion Overrides
 
     # region Internal Methods
 
     def _set_fd_style(self, name: str | None, style: str | None) -> None:
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/font/font_position.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/font/font_position.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/highlight/highlight.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/highlight/highlight.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/char/hyperlink/hyperlink.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/char/hyperlink/hyperlink.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/area/fill_color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/area/fill_color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/area/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/area/gradient.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 from ooodev.utils.data_type.angle import Angle as Angle
 from ooodev.utils.data_type.color_range import ColorRange as ColorRange
 from ooodev.utils.data_type.intensity import Intensity as Intensity
 from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
 from ooodev.utils.data_type.offset import Offset as Offset
 from ooodev.format.inner.kind.format_kind import FormatKind
 from ooodev.format.inner.preset import preset_gradient
-from ooodev.format.inner.preset.preset_gradient import PresetGradientKind as PresetGradientKind
+from ooodev.format.inner.preset.preset_gradient import (
+    PresetGradientKind as PresetGradientKind,
+)
 from ooodev.format.inner.style_base import StyleMulti
 from ooodev.format.inner.common.props.area_gradient_props import AreaGradientProps
 from ooodev.format.inner.direct.structs.gradient_struct import GradientStruct
 
 # endregion Import
 
 _TGradient = TypeVar(name="_TGradient", bound="Gradient")
@@ -65,26 +67,25 @@
                 Defaults to ``0``.
             grad_color (ColorRange, optional): Specifies the color at the start point and stop point of the gradient.
                 Defaults to ``ColorRange(Color(0), Color(16777215))``.
             grad_intensity (IntensityRange, optional): Specifies the intensity at the start point and stop point of the
                 gradient. Defaults to ``IntensityRange(100, 100)``.
             name (str, optional): Specifies the Fill Gradient Name.
         """
-        fs = GradientStruct(
+        fs = self._get_inner_class(
             style=style,
             step_count=step_count,
             x_offset=offset.x,
             y_offset=offset.y,
             angle=angle,
             border=border,
             start_color=grad_color.start,
             start_intensity=grad_intensity.start,
             end_color=grad_color.end,
             end_intensity=grad_intensity.end,
-            _cattribs=self._get_gradient_struct_cattrib(),
         )
         super().__init__()
         self._name = name
 
         self._set(self._props.style, FillStyle.GRADIENT)
         self._set(self._props.step_count, step_count)
         if name == "__constructor_default__":
@@ -92,60 +93,100 @@
             self._set(self._props.name, "Gradient 9999")
             self._set_style("fill_style", fs, *fs.get_attrs())
         else:
             fill_struct = self._get_fill_struct(fill_struct=fs, name=name, auto_name=False)
             self._set(self._props.name, self._name)
             self._set_style("fill_style", fill_struct, *fill_struct.get_attrs())
 
+    # region Internal Methods
+    def _container_get_default_name(self) -> str:
+        return "Gradient"
+
     def _get_gradient_struct_cattrib(self) -> dict:
         return {
             "_property_name": "FillGradient",
             "_supported_services_values": self._supported_services(),
             "_format_kind_prop": self.prop_format_kind,
         }
 
+    def _get_gradient_from_uno_struct(self, value: UNOGradient, **kwargs) -> GradientStruct:
+        return GradientStruct.from_uno_struct(value, **kwargs)
+
     def _get_fill_struct(self, fill_struct: GradientStruct | None, name: str, auto_name: bool) -> GradientStruct:
         # if the name passed in already exist in the Gradient Table then it is returned.
         # Otherwise, the Gradient is added to the Gradient Table and then returned.
         # after Gradient is added to table all other subsequent call of this name will return
         # that Gradient from the Table. Except auto_name which will force a new entry
         # into the Table each time.
         self._name = name
         if name:
             if PresetGradientKind.is_preset(name):
                 return fill_struct
         else:
             auto_name = True
-            name = "Gradient"
+            name = self._container_get_default_name()
         nc = self._container_get_inst()
         if auto_name:
             name = name.rstrip() + " "  # add a space after name before getting unique name
             self._name = self._container_get_unique_el_name(name, nc)
 
         grad = self._container_get_value(self._name, nc)  # raises value error if name is empty
         if not grad is None:
-            return GradientStruct.from_uno_struct(grad, _cattribs=self._get_gradient_struct_cattrib())
+            return self._get_gradient_from_uno_struct(grad, _cattribs=self._get_gradient_struct_cattrib())
         if fill_struct is None:
             raise ValueError(
                 f'No Gradient could be found in container for "{name}". In this case a Gradient is required.'
             )
         self._container_add_value(name=self._name, obj=fill_struct.get_uno_struct(), allow_update=False, nc=nc)
-        return GradientStruct.from_uno_struct(
-            self._container_get_value(self._name, nc), _cattribs=self._get_gradient_struct_cattrib()
+        return self._get_gradient_from_uno_struct(
+            self._container_get_value(self._name, nc),
+            _cattribs=self._get_gradient_struct_cattrib(),
+        )
+
+    def _get_inner_class(
+        self,
+        style: GradientStyle,
+        step_count: int,
+        x_offset: Intensity | int,
+        y_offset: Intensity | int,
+        angle: Angle | int,
+        border: Intensity | int,
+        start_color: Color,
+        start_intensity: Intensity | int,
+        end_color: Color,
+        end_intensity: Intensity | int,
+    ) -> GradientStruct:
+        fs = GradientStruct(
+            style=style,
+            step_count=step_count,
+            x_offset=x_offset,
+            y_offset=y_offset,
+            angle=angle,
+            border=border,
+            start_color=start_color,
+            start_intensity=start_intensity,
+            end_color=end_color,
+            end_intensity=end_intensity,
+            _cattribs=self._get_gradient_struct_cattrib(),
         )
+        return fs
 
+    # endregion Internal Methods
+
+    # region override methods
     def _container_get_service_name(self) -> str:
         # https://github.com/LibreOffice/core/blob/d9e044f04ac11b76b9a3dac575f4e9155b67490e/chart2/source/tools/PropertyHelper.cxx#L229
         return "com.sun.star.drawing.GradientTable"
 
     def _supported_services(self) -> Tuple[str, ...]:
         try:
             return self._supported_services_values
         except AttributeError:
             self._supported_services_values = (
+                "com.sun.star.beans.PropertySet",
                 "com.sun.star.drawing.FillProperties",
                 "com.sun.star.style.PageStyle",
                 "com.sun.star.style.ParagraphStyle",
                 "com.sun.star.text.BaseFrame",
                 "com.sun.star.text.TextContent",
                 "com.sun.star.text.TextEmbeddedObject",
                 "com.sun.star.text.TextGraphicObject",
@@ -169,29 +210,33 @@
     def copy(self: _TGradient, **kwargs) -> _TGradient:
         """Gets a copy of instance as a new instance"""
         cp = super().copy(**kwargs)
         cp._name = self._name
         return cp
 
     # endregion copy()
+    # endregion override methods
+
+    # region Static Methods
+
     # region from_obj()
     @overload
     @classmethod
     def from_obj(cls: Type[_TGradient], obj: object) -> _TGradient:
         ...
 
     @overload
     @classmethod
     def from_obj(cls: Type[_TGradient], obj: object, **kwargs) -> _TGradient:
         ...
 
     @classmethod
     def from_obj(cls: Type[_TGradient], obj: object, **kwargs) -> _TGradient:
         """
-        Gets instance from object
+        Gets instance from object.
 
         Args:
             obj (object): UNO object.
 
         Raises:
             NotSupportedError: If ``obj`` is not supported.
 
@@ -270,14 +315,16 @@
         """
         args = preset_gradient.get_preset(preset)
         args.update(kwargs)
         return cls(**args)
 
     # endregion from_preset()
 
+    # endregion Static Methods
+
     @property
     def prop_format_kind(self) -> FormatKind:
         """Gets the kind of style"""
         try:
             return self._format_kind_prop
         except AttributeError:
             self._format_kind_prop = FormatKind.PARA | FormatKind.TXT_CONTENT
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/area/hatch.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/area/hatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,23 +60,15 @@
             angle (Angle, int, optional): Specifies angle of the hatch in degrees. Default to ``0``.
             bg_color(Color, optionl): Specifies the background Color. Set this ``-1`` (default) for no background color.
 
         Returns:
             None:
         """
 
-        hatch = HatchStruct(
-            style=style,
-            color=color,
-            distance=space,
-            angle=angle,
-            _cattribs=self._get_hatch_cattribs(),
-        )
-        hatch._prop_parent = self
-        # hatch._struct_property_name = self._props.hatch_prop
+        hatch = self._get_inner_class(style=style, color=color, distance=space, angle=angle)
 
         # create event just to listen to fill color init
         bk_color = FillColor(color=bg_color, _cattribs=self._get_fill_color_cattribs())
         bk_color._prop_parent = self
         # FillStyle is set by this class
         bk_color._remove(self._props.style)
         # add event listener to prevent FillStyle from being set
@@ -143,14 +135,25 @@
                 mLo.Lo.print(f"  {err}")
 
     # endregion apply()
 
     # endregion Overrides
 
     # region Internal Methods
+    def _get_inner_class(self, style, color, distance, angle) -> HatchStruct:
+        hatch = HatchStruct(
+            style=style,
+            color=color,
+            distance=distance,
+            angle=angle,
+            _cattribs=self._get_hatch_cattribs(),
+        )
+        hatch._prop_parent = self
+        return hatch
+
     def _get_hatch_cattribs(self) -> dict:
         return {
             "_supported_services_values": self._supported_services(),
             "_format_kind_prop": self.prop_format_kind,
             "_property_name": self._props.hatch_prop,
         }
 
@@ -194,15 +197,15 @@
 
     @classmethod
     def from_preset(cls: Type[_THatch], preset: PresetHatchKind, **kwargs) -> _THatch:
         """
         Gets an instance from a preset.
 
         Args:
-            preset (PresetHatchKind): Preset.
+            preset (~.format.inner.preset.preset_hatch.PresetHatchKind): Preset.
 
         Returns:
             Hatch: Instance from preset.
         """
         kargs = mPreset.get_preset(preset)
         kargs.update(kwargs)
         return cls(**kargs)
@@ -241,14 +244,15 @@
         hatch = cast(UnoHatch, mProps.Props.get(obj, nu._props.hatch_prop))
         fc = FillColor.from_obj(obj, _cattribs=nu._get_fill_color_cattribs())
 
         if hatch.Angle > 0:
             angle = round(hatch.Angle / 10)
         else:
             angle = 0
+
         return cls(
             style=hatch.Style,
             color=hatch.Color,
             space=UnitConvert.convert_mm100_mm(hatch.Distance),
             angle=angle,
             bg_color=fc.prop_color,
             **kwargs,
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/area/img.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/area/img.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 # region Imports
 from __future__ import annotations
 from typing import Any, Tuple, cast, overload, Type, TypeVar, TYPE_CHECKING
 from enum import Enum
 
 from com.sun.star.awt import XBitmap
 
-from ooo.dyn.drawing.fill_style import FillStyle as FillStyle
 from ooo.dyn.drawing.bitmap_mode import BitmapMode
+from ooo.dyn.drawing.fill_style import FillStyle as FillStyle
 from ooo.dyn.drawing.rectangle_point import RectanglePoint as RectanglePoint
 
 from ooodev.events.args.key_val_cancel_args import KeyValCancelArgs
 from ooodev.exceptions import ex as mEx
-from ooodev.utils import lo as mLo
-from ooodev.utils import props as mProps
-from ooodev.utils.data_type.offset import Offset as Offset
-from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
-from ooodev.units.unit_convert import UnitConvert
-from ooodev.format.inner.kind.format_kind import FormatKind
-from ooodev.format.inner.preset import preset_image as mImage
-from ooodev.format.inner.preset.preset_image import PresetImageKind as PresetImageKind
-from ooodev.format.inner.style_base import StyleBase
 from ooodev.format.inner.common.format_types.offset_column import OffsetColumn as OffsetColumn
 from ooodev.format.inner.common.format_types.offset_row import OffsetRow as OffsetRow
 from ooodev.format.inner.common.format_types.size_percent import SizePercent as SizePercent
 from ooodev.format.inner.common.props.area_img_props import AreaImgProps
+from ooodev.format.inner.kind.format_kind import FormatKind
+from ooodev.format.inner.preset import preset_image as mImage
+from ooodev.format.inner.preset.preset_image import PresetImageKind as PresetImageKind
+from ooodev.format.inner.style_base import StyleBase
+from ooodev.units.unit_convert import UnitConvert
+from ooodev.utils import lo as mLo
+from ooodev.utils import props as mProps
+from ooodev.utils.data_type.offset import Offset as Offset
+from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 
 # endregion Imports
 
 if TYPE_CHECKING:
     pass
 
 # https://github.com/LibreOffice/core/blob/6379414ca34527fbe69df2035d49d651655317cd/vcl/source/filter/ipict/ipict.cxx#L92
@@ -108,16 +108,17 @@
         init_vals = {}
         bmap = None
         try:
             # if bitmap or name is passed in then get the bitmap
             bmap = self._get_bitmap(bitmap, name, auto_name)
         except Exception:
             pass
-        if not bmap is None:
-            init_vals[self._props.bitmap] = bmap
+        if bmap is not None:
+            if self._props.bitmap:
+                init_vals[self._props.bitmap] = bmap
             init_vals[self._props.name] = self._name
             init_vals[self._props.style] = FillStyle.BITMAP
 
         super().__init__(**init_vals)
         self.prop_mode = mode
         self.prop_size = size
         self.prop_posiion = position
@@ -201,15 +202,16 @@
         Args:
             obj (object): UNO object that has supports ``com.sun.star.style.FillProperties``
                 or ``com.sun.star.beans.PropertySet`` service.
 
         Returns:
             None:
         """
-        if not self._has(self._props.bitmap):
+
+        if self._props.bitmap and not self._has(self._props.bitmap):
             mLo.Lo.print("Img.apply(): There is nothing to apply.")
             return
         super().apply(obj, **kwargs)
 
     def _props_set(self, obj: object, **kwargs: Any) -> None:
         try:
             super()._props_set(obj, **kwargs)
@@ -217,15 +219,15 @@
             mLo.Lo.print(f"Img.apply(): Unable to set Property")
             for err in e.errors:
                 mLo.Lo.print(f"  {err}")
 
     # endregion apply()
 
     def on_property_restore_setting(self, source: Any, event_args: KeyValCancelArgs) -> None:
-        if event_args.key == self._props.bitmap:
+        if self._props.bitmap and event_args.key == self._props.bitmap:
             if event_args.value is None:
                 event_args.default = True
         elif event_args.key == self._props.name:
             if not event_args.value:
                 event_args.default = True
         return super().on_property_restore_setting(source, event_args)
 
@@ -245,15 +247,15 @@
 
     @classmethod
     def from_preset(cls: Type[_TImg], preset: PresetImageKind, **kwargs) -> _TImg:
         """
         Gets an instance from a preset.
 
         Args:
-            preset (PresetImageKind): Preset.
+            preset (~.preset.preset_image.PresetImageKind): Preset.
 
         Returns:
             Img: Instance from preset.
         """
         name = str(preset)
         nu = cls(**kwargs)
 
@@ -315,15 +317,16 @@
             val = mProps.Props.get(obj, key, None)
             if not val is None:
                 fp._set(key, val)
 
         name = mProps.Props.get(obj, inst._props.name)
         inst._name = name
         inst._set(inst._props.name, name)
-        set_prop(inst._props.bitmap, inst)
+        if inst._props.bitmap:
+            set_prop(inst._props.bitmap, inst)
         set_prop(inst._props.mode, inst)
         set_prop(inst._props.offset_x, inst)
         set_prop(inst._props.offset_y, inst)
         set_prop(inst._props.pos_x, inst)
         set_prop(inst._props.pos_y, inst)
         set_prop(inst._props.point, inst)
         set_prop(inst._props.size_x, inst)
@@ -348,14 +351,16 @@
         except AttributeError:
             self._format_kind_prop = FormatKind.TXT_CONTENT | FormatKind.FILL
         return self._format_kind_prop
 
     @property
     def prop_bitmap(self) -> XBitmap | None:
         """Gets bitmap"""
+        if not self._props.bitmap:
+            return None
         pv = self._get(self._props.bitmap)
         if pv is None:
             return None
         return pv
 
     @property
     def prop_mode(self) -> ImgStyleKind | None:
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/area/pattern.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/area/pattern.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,25 +58,30 @@
         Note:
             If ``auto_name`` is ``False`` then a bitmap for a given name is only required the first call.
             All subsequent call of the same name will retrieve the bitmap form the LibreOffice Bitmap Table.
         """
 
         init_vals = {}
         # if bitmap or name is passed in then get the bitmap
-        init_vals[self._props.tile] = tile
-        init_vals[self._props.stretch] = stretch
+        if self._props.tile:
+            init_vals[self._props.tile] = tile
+        if self._props.stretch:
+            init_vals[self._props.stretch] = stretch
         bmap = None
         try:
             bmap = self._get_bitmap(bitmap, name, auto_name)
         except Exception:
             pass
         if not bmap is None:
-            init_vals[self._props.bitmap] = bmap
-            init_vals[self._props.name] = self._name
-            init_vals[self._props.style] = FillStyle.BITMAP
+            if self._props.bitmap:
+                init_vals[self._props.bitmap] = bmap
+            if self._props.name:
+                init_vals[self._props.name] = self._name
+            if self._props.style:
+                init_vals[self._props.style] = FillStyle.BITMAP
 
         super().__init__(**init_vals)
 
     # region Internal Methods
     def _get_bitmap(self, bitmap: XBitmap | None, name: str, auto_name: bool) -> XBitmap:
         # if the name passed in already exist in the Bitmap Table then it is returned.
         # Otherwise the bitmap is added to the Bitmap Table and then returned.
@@ -150,15 +155,15 @@
 
         Args:
             obj (object): UNO object that has supports ``com.sun.star.style.FillProperties`` or ``com.sun.star.beans.PropertySet`` service.
 
         Returns:
             None:
         """
-        if not self._has(self._props.bitmap):
+        if self._props.bitmap and not self._has(self._props.bitmap):
             mLo.Lo.print("Pattern.apply(): There is nothing to apply.")
             return
         super().apply(obj, **kwargs)
 
     def _props_set(self, obj: object, **kwargs: Any) -> None:
         try:
             super()._props_set(obj, **kwargs)
@@ -194,15 +199,15 @@
 
     @classmethod
     def from_preset(cls: Type[_TPattern], preset: PresetPatternKind, **kwargs) -> _TPattern:
         """
         Gets an instance from a preset.
 
         Args:
-            preset (PresetPatternKind): Preset.
+            preset (~.preset.preset_pattern.PresetPatternKind): Preset.
 
         Returns:
             Pattern: ``Pattern`` instance from preset.
         """
         name = str(preset)
         nu = cls(**kwargs)
 
@@ -241,14 +246,16 @@
         """
         inst = cls(**kwargs)
         if not inst._is_valid_obj(obj):
             raise mEx.NotSupportedError(f'Object is not supported for conversion to "{cls.__name__}"')
 
         def set_prop(key: str, fp: Pattern):
             nonlocal obj
+            if not key:
+                return
             val = mProps.Props.get(obj, key, None)
             if not val is None:
                 fp._set(key, val)
 
         name = mProps.Props.get(obj, inst._props.name)
         inst._name = name
         inst._set(inst._props.name, name)
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/transparent/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/transparent/gradient.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Module for Fill Gradient Color.
 
 .. versionadded:: 0.9.0
 """
 # region Import
 from __future__ import annotations
-from typing import Any, Tuple, cast, Type, TypeVar, overload
+from typing import Any, Tuple, cast, Type, TypeVar, overload, TYPE_CHECKING
 from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
-from ooo.dyn.awt.gradient import Gradient as UNOGradient
 
 from ooodev.events.args.cancel_event_args import CancelEventArgs
 from ooodev.events.args.key_val_cancel_args import KeyValCancelArgs
 from ooodev.exceptions import ex as mEx
 from ooodev.utils import color as mColor
 from ooodev.utils import lo as mLo
 from ooodev.utils import props as mProps
@@ -20,14 +19,17 @@
 from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
 from ooodev.utils.data_type.offset import Offset as Offset
 from ooodev.format.inner.kind.format_kind import FormatKind
 from ooodev.format.inner.style_base import StyleMulti
 from ooodev.format.inner.direct.structs.gradient_struct import GradientStruct
 from ooodev.format.inner.common.props.transparent_gradient_props import TransparentGradientProps
 
+if TYPE_CHECKING:
+    from ooo.dyn.awt.gradient import Gradient as UNOGradient
+
 # endregion Import
 
 # from ooo.dyn.drawing.fill_style import FillStyle
 
 # See Also:
 # https://wiki.documentfoundation.org/Documentation/BASIC_Guide#Color_Gradient
 # https://github.com/LibreOffice/core/blob/d57836db76fcf3133e6eb54d264c774911015e08/chart2/source/controller/itemsetwrapper/GraphicPropertyItemConverter.cxx
@@ -71,72 +73,106 @@
         """
 
         start_color = int(mColor.get_gray_rgb(grad_intensity.start))
         end_color = int(mColor.get_gray_rgb(grad_intensity.end))
         # start_color = 4144959
         # end_color = 16777215
 
-        fs = GradientStruct(
+        fs = self._get_inner_class(
             style=style,
             step_count=0,
             x_offset=offset.x,
             y_offset=offset.y,
             angle=angle,
             border=border,
             start_color=start_color,
             start_intensity=grad_intensity.start,
             end_color=end_color,
             end_intensity=grad_intensity.end,
-            _cattribs=self._get_inner_cattribs(),
         )
 
         super().__init__()
         # gradient
         self._set_fill_tp(fs, kwargs.get("transparency_name", ""))
         # self._set("FillStyle", FillStyle.SOLID)
         # Fill Transparence is always zero when Gradient Transparency is applied
         self._set(self._props.transparence, 0)
 
     # region Internal Methods
+    def _get_inner_class(
+        self,
+        style: GradientStyle,
+        step_count: int,
+        x_offset: Intensity | int,
+        y_offset: Intensity | int,
+        angle: Angle | int,
+        border: Intensity | int,
+        start_color: int,
+        start_intensity: Intensity | int,
+        end_color: int,
+        end_intensity: Intensity | int,
+    ) -> GradientStruct:
+        fs = GradientStruct(
+            style=style,
+            step_count=step_count,
+            x_offset=x_offset,
+            y_offset=y_offset,
+            angle=angle,
+            border=border,
+            start_color=start_color,
+            start_intensity=start_intensity,
+            end_color=end_color,
+            end_intensity=end_intensity,
+            _cattribs=self._get_inner_cattribs(),
+        )
+        return fs
+
     def _get_inner_cattribs(self) -> dict:
         return {
             "_supported_services_values": self._supported_services(),
             "_format_kind_prop": self.prop_format_kind,
             "_property_name": self._props.struct_prop,
         }
 
     def _set_fill_tp(self, fill_tp: GradientStruct, name: str = "") -> None:
         fs = self._get_fill_tp(fill_tp, name)
         fs._prop_parent = self
 
         self._set(self._props.name, self._name)
         self._set_style("fill_style", fs, *fs.get_attrs())
 
+    def _container_get_default_name(self) -> str:
+        return "Transparency"
+
+    def _get_gradient_from_uno_struct(self, value: "UNOGradient", **kwargs) -> GradientStruct:
+        return GradientStruct.from_uno_struct(value, **kwargs)
+
     def _get_fill_tp(self, fill_tp: GradientStruct, name: str) -> GradientStruct:
         # if the name passed in already exist in the TransparencyGradientTable Table then it is returned.
-        # Otherwise, the struc is added to the TransparencyGradientTable Table and then returned.
+        # Otherwise, the struct is added to the TransparencyGradientTable Table and then returned.
         # after struct is added to table all other subsequent call of this name will return
         # that struc from the Table. Except auto_name which will force a new entry
         # into the Table each time.
         # see: https://github.com/LibreOffice/core/blob/d9e044f04ac11b76b9a3dac575f4e9155b67490e/chart2/source/tools/PropertyHelper.cxx#L212
         nc = self._container_get_inst()
         if name:
             struct = self._container_get_value(name, nc)  # raises value error if name is empty
             if struct is not None:
                 self._name = name
-                return GradientStruct.from_uno_struct(value=struct, _cattribs=self._get_inner_cattribs())
+                return self._get_gradient_from_uno_struct(value=struct, _cattribs=self._get_inner_cattribs())
 
-        name = "Transparency "
+        name = self._container_get_default_name()
+        name = name.strip() + " "
         self._name = self._container_get_unique_el_name(name, nc)
         struct = self._container_get_value(self._name, nc)  # raises value error if name is empty
         if struct is not None:
-            return GradientStruct.from_uno_struct(value=struct, _cattribs=self._get_inner_cattribs())
+            return self._get_gradient_from_uno_struct(value=struct, _cattribs=self._get_inner_cattribs())
         struct = fill_tp.get_uno_struct()
         self._container_add_value(name=self._name, obj=struct, allow_update=False, nc=nc)
-        return GradientStruct.from_uno_struct(
+        return self._get_gradient_from_uno_struct(
             value=self._container_get_value(self._name, nc), _cattribs=self._get_inner_cattribs()
         )
 
     # endregion Internal Methods
 
     # region Overrides
     # region copy()
@@ -229,15 +265,15 @@
             Gradient: Instance that represents Gradient color.
         """
         # this nu is only used to get Property Name
         nu = cls(**kwargs)
         if not nu._is_valid_obj(obj):
             raise mEx.NotSupportedError(f'Object is not supported for conversion to "{cls.__name__}"')
 
-        grad_fill = cast(UNOGradient, mProps.Props.get(obj, nu._props.struct_prop))
+        grad_fill = cast("UNOGradient", mProps.Props.get(obj, nu._props.struct_prop))
         fill_gradient_name = cast(str, mProps.Props.get(obj, nu._props.name, ""))
         if grad_fill.Angle == 0:
             angle = 0
         else:
             angle = round(grad_fill.Angle / 10)
         return cls(
             style=grad_fill.Style,
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/fill/transparent/transparency.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/fill/transparent/transparency.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/frame_type/anchor.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/frame_type/anchor.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/frame_type/position.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/frame_type/position.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/frame_type/size.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/frame_type/size.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/hyperlink/image_map_options.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/hyperlink/image_map_options.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/hyperlink/link_to.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/hyperlink/link_to.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/options/align.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/options/align.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/options/names.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/options/names.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/options/properties.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/options/properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/options/protect.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/options/protect.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/wrap/options.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/wrap/options.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/wrap/settings.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/wrap/settings.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/frame/wrap/spacing.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/frame/wrap/spacing.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/crop/crop.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/crop/crop.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/image/flip.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/image/flip.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/image/rotation.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/image/rotation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/image_type/size.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/image_type/size.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/options/names.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/options/names.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/image/options/properties.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/image/options/properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/footer/area/color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/footer/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/footer/area/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/footer/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/footer/area/hatch.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/footer/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/footer/area/img.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/footer/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/footer/area/pattern.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/footer/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/footer/footer.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/footer/footer.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/header/area/color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/header/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/header/area/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/header/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/header/area/hatch.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/header/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/header/area/img.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/header/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/header/area/pattern.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/header/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/header/header.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/header/header.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/page/layout_settings.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/page/layout_settings.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/page/margins.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/page/margins.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/page/page/paper_format.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/page/page/paper_format.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/align/alignment.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/align/alignment.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/align/writing_mode.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/structs/point_struct.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,281 +1,280 @@
-"""
-Module for managing paragraph Writing Mode.
-
-.. versionadded:: 0.9.0
-"""
+# region Import
 from __future__ import annotations
-from typing import Any, Tuple, cast, overload, Type, TypeVar
+from typing import Tuple, Type, cast, overload, TypeVar
 
-from ooo.dyn.text.writing_mode2 import WritingMode2Enum as WritingMode2Enum
+import uno
+from ooo.dyn.awt.point import Point
 
-from ooodev.events.args.cancel_event_args import CancelEventArgs
 from ooodev.exceptions import ex as mEx
-from ooodev.utils import lo as mLo
 from ooodev.utils import props as mProps
+from ooodev.units import UnitObj
+from ooodev.units import UnitMM
+from ooodev.units import UnitConvert
 from ooodev.format.inner.kind.format_kind import FormatKind
-from ooodev.format.inner.style_base import StyleBase
+from ...common.props.struct_size_props import StructSizeProps
+from .struct_base import StructBase
 
+# endregion Import
 
-_TWritingMode = TypeVar(name="_TWritingMode", bound="WritingMode")
+_TPointStruct = TypeVar(name="_TPointStruct", bound="PointStruct")
 
 
-class WritingMode(StyleBase):
+class PointStruct(StructBase):
     """
-    Paragraph Writing Mode
+    Point struct.
 
     Any properties starting with ``prop_`` set or get current instance values.
 
-    All methods starting with ``fmt_`` can be used to chain together properties.
-
-    .. versionadded:: 0.9.0
+    All methods starting with ``fmt_`` can be used to chain together Border Table properties.
     """
 
     # region init
 
-    def __init__(self, mode: WritingMode2Enum | None = None) -> None:
+    def __init__(self, x: int = 0, y: int = 0) -> None:
         """
         Constructor
 
         Args:
-            mode (WritingMode2Enum, optional): Determines the writing direction
-
-        Returns:
-            None:
+            x (int, optional): Specifies X coordinate. Default ``0``.
+            y (int, optional): Specifies Y coordinate. Default ``0``.
         """
-        # https://api.libreoffice.org/docs/idl/ref/servicecom_1_1sun_1_1star_1_1style_1_1ParagraphProperties-members.html
-        init_vals = {}
-
-        if mode is not None:
-            init_vals[self._get_property_name()] = mode.value
-
-        super().__init__(**init_vals)
+        super().__init__()
+        self.prop_x = x
+        self.prop_y = y
 
     # endregion init
 
-    # region methods
+    # region internal methods
     def _get_property_name(self) -> str:
         try:
             return self._property_name
         except AttributeError:
-            self._property_name = "WritingMode"
+            self._property_name = "Position"
         return self._property_name
 
+    # endregion internal methods
+
+    # region dunder methods
+    def __eq__(self, oth: object) -> bool:
+        obj2 = None
+        if isinstance(oth, PointStruct):
+            obj2 = oth.get_uno_struct()
+        if getattr(oth, "typeName", None) == "com.sun.star.awt.Point":
+            obj2 = cast(PointStruct, oth)
+        if obj2:
+            obj1 = self.get_uno_struct()
+            return obj1.X == obj2.X and obj1.Y == obj2.Y
+        return NotImplemented
+
+    # endregion dunder methods
+
+    # region methods
+    def get_uno_struct(self) -> Point:
+        """
+        Gets UNO ``Point`` from instance.
+
+        Returns:
+            Point: ``Point`` instance
+        """
+        x = self._get(self._props.width)
+        y = self._get(self._props.height)
+        inst = Point(X=x, Y=y)
+        return inst
+
+    # endregion methods
+
+    # region overrides methods
+
     def _supported_services(self) -> Tuple[str, ...]:
         try:
             return self._supported_services_values
         except AttributeError:
-            self._supported_services_values = (
-                "com.sun.star.style.ParagraphPropertiesComplex",
-                "com.sun.star.style.ParagraphStyle",
-            )
+            self._supported_services_values = ("com.sun.star.drawing.Shape",)
         return self._supported_services_values
 
-    def _on_modifying(self, source: Any, event: CancelEventArgs) -> None:
-        if self._is_default_inst:
-            raise ValueError("Modifying a default instance is not allowed")
-        return super()._on_modifying(source, event)
-
     # region apply()
 
     @overload
     def apply(self, obj: object) -> None:
         ...
 
     def apply(self, obj: object, **kwargs) -> None:
         """
-        Applies writing mode to ``obj``
+        Applies tab properties to ``obj``
 
         Args:
-            obj (object): UNO object that supports ``com.sun.star.style.ParagraphPropertiesComplex`` service.
+            obj (object): UNO object.
 
         Returns:
             None:
         """
-        try:
-            super().apply(obj, **kwargs)
-        except mEx.MultiError as e:
-            mLo.Lo.print(f"{self.__class__.__name__}.apply(): Unable to set Property")
-            for err in e.errors:
-                mLo.Lo.print(f"  {err}")
+        name = self._get_property_name()
+        if not name:
+            return
+        if not mProps.Props.has(obj, name):
+            self._print_not_valid_srv("apply")
+            return
+
+        struct = self.get_uno_struct()
+        props = {name: struct}
+        super().apply(obj=obj, override_dv=props)
 
     # endregion apply()
 
-    # region from_obj()
+    # endregion overrides methods
+
+    # region static methods
+
+    # region from_uno_struct()
     @overload
     @classmethod
-    def from_obj(cls: Type[_TWritingMode], obj: object) -> _TWritingMode:
+    def from_uno_struct(cls: Type[_TPointStruct], value: Point) -> _TPointStruct:
         ...
 
     @overload
     @classmethod
-    def from_obj(cls: Type[_TWritingMode], obj: object, **kwargs) -> _TWritingMode:
+    def from_uno_struct(cls: Type[_TPointStruct], value: Point, **kwargs) -> _TPointStruct:
         ...
 
     @classmethod
-    def from_obj(cls: Type[_TWritingMode], obj: object, **kwargs) -> _TWritingMode:
+    def from_uno_struct(cls: Type[_TPointStruct], value: Point, **kwargs) -> _TPointStruct:
         """
-        Gets instance from object
+        Converts a ``Point`` instance to a ``PointStruct``.
 
         Args:
-            obj (object): UNO object.
-
-        Raises:
-            NotSupportedError: If ``obj`` is not supported.
+            value (Point): UNO ``Point``.
 
         Returns:
-            WritingMode: ``WritingMode`` instance that represents ``obj`` writing mode.
+            PointStruct: ``PointStruct`` set with ``Point`` properties.
         """
         inst = cls(**kwargs)
-        if not inst._is_valid_obj(obj):
-            raise mEx.NotSupportedError(f'Object is not supported for conversion to "{cls.__name__}"')
-
-        inst._set("WritingMode", int(mProps.Props.get(obj, inst._get_property_name())))
+        inst._set(inst._props.height, value.Height)
+        inst._set(inst._props.width, value.Width)
         return inst
 
-    # endregion from_obj()
+    # endregion from_uno_struct()
 
-    # endregion methods
+    # region from_obj()
+    @overload
+    @classmethod
+    def from_obj(cls: Type[_TPointStruct], obj: object) -> _TPointStruct:
+        ...
+
+    @overload
+    @classmethod
+    def from_obj(cls: Type[_TPointStruct], obj: object, **kwargs) -> _TPointStruct:
+        ...
 
-    # region style methods
-    def fmt_mode(self: _TWritingMode, value: WritingMode2Enum | None) -> _TWritingMode:
+    @classmethod
+    def from_obj(cls: Type[_TPointStruct], obj: object, **kwargs) -> _TPointStruct:
         """
-        Gets copy of instance with writing mode set or removed
+        Gets instance from object
 
         Args:
-            value (WritingMode2Enum | None): mode value
+            obj (object): UNO object
+
+        Raises:
+            PropertyNotFoundError: If ``obj`` does not have required property
 
         Returns:
-            WritingMode: ``WritingMode`` instance
+            PointStruct: ``PointStruct`` instance that represents ``obj`` Point properties.
         """
-        cp = self.copy()
-        cp.prop_align = value
-        return cp
+        # this nu is only used to get Property Name
+        nu = cls(**kwargs)
+        prop_name = nu._get_property_name()
 
-    # endregion style methods
+        try:
+            point = cast(PointStruct, mProps.Props.get(obj, prop_name))
+        except mEx.PropertyNotFoundError:
+            raise mEx.PropertyNotFoundError(prop_name, f"from_obj() obj as no {prop_name} property")
 
-    # region Style Properties
-    @property
-    def bt_lr(self: _TWritingMode) -> _TWritingMode:
-        """
-        Gets instance.
+        return cls.from_uno_struct(point, **kwargs)
 
-        Text within a line is written bottom-to-top.
-        Lines and blocks are placed left-to-right.
-        """
-        cp = self.copy()
-        cp.prop_mode = WritingMode2Enum.BT_LR
-        return cp
+    # endregion from_obj()
 
-    @property
-    def lr_tb(self: _TWritingMode) -> _TWritingMode:
-        """
-        Gets instance.
+    # endregion static methods
 
-        Text within lines is written left-to-right.
-        Lines and blocks are placed top-to-bottom.
-        Typically, this is the writing mode for normal ``alphabetic`` text.
+    # region Style methods
+    def fmt_all(self: _TPointStruct, value: int) -> _TPointStruct:
         """
-        cp = self.copy()
-        cp.prop_mode = WritingMode2Enum.LR_TB
-        return cp
+        Gets copy of instance with width and height set.
 
-    @property
-    def rl_tb(self: _TWritingMode) -> _TWritingMode:
-        """
-        Gets instance.
+        Args:
+            value (float, UnitObj): Specifies ``x`` and ``y`` values.
 
-        Text within a line are written right-to-left.
-        Lines and blocks are placed top-to-bottom.
-        Typically, this writing mode is used in Arabic and Hebrew text.
+        Returns:
+            PointStruct: Border Table
         """
         cp = self.copy()
-        cp.prop_mode = WritingMode2Enum.RL_TB
+        cp.prop_y = value
+        cp.prop_x = value
         return cp
 
-    @property
-    def tb_rl(self: _TWritingMode) -> _TWritingMode:
-        """
-        Gets instance.
-
-        Text within a line is written top-to-bottom.
-        Lines and blocks are placed right-to-left.
-        Typically, this writing mode is used in Chinese and Japanese text.
+    def fmt_x(self: _TPointStruct, value: int) -> _TPointStruct:
         """
-        cp = self.copy()
-        cp.prop_mode = WritingMode2Enum.TB_RL
-        return cp
+        Gets a copy of instance with height set.
 
-    @property
-    def tb_lr(self: _TWritingMode) -> _TWritingMode:
-        """
-        Gets instance.
+        Args:
+            value (float, UnitObj): Specifies ``x`` value.
 
-        Text within a line is written top-to-bottom.
-        Lines and blocks are placed left-to-right.
-        Typically, this writing mode is used in Mongolian text.
+        Returns:
+            PointStruct:
         """
         cp = self.copy()
-        cp.prop_mode = WritingMode2Enum.TB_LR
+        cp.prop_x = value
         return cp
 
-    @property
-    def page(self: _TWritingMode) -> _TWritingMode:
-        """
-        Gets instance.
-
-        Obtain writing mode from the current page.
-        May not be used in page styles.
+    def fmt_y(self: _TPointStruct, value: int) -> _TPointStruct:
         """
-        cp = self.copy()
-        cp.prop_mode = WritingMode2Enum.PAGE
-        return cp
+        Gets a copy of instance with width set.
 
-    @property
-    def context(self: _TWritingMode) -> _TWritingMode:
-        """
-        Gets instance.
+        Args:
+            value (float, UnitObj): Specifies ``y`` value.
 
-        Obtain actual writing mode from the context of the object.
+        Returns:
+            PointStruct:
         """
         cp = self.copy()
-        cp.prop_mode = WritingMode2Enum.CONTEXT
+        cp.prop_y = value
         return cp
 
-    # endregion Style Properties
+    # endregion Style methods
+
+    # region Properties
 
-    # region properties
     @property
     def prop_format_kind(self) -> FormatKind:
         """Gets the kind of style"""
         try:
             return self._format_kind_prop
         except AttributeError:
-            self._format_kind_prop = FormatKind.PARA | FormatKind.PARA_COMPLEX
+            self._format_kind_prop = FormatKind.STRUCT
         return self._format_kind_prop
 
     @property
-    def prop_mode(self) -> WritingMode2Enum | None:
-        """Gets/Sets writing mode of a paragraph."""
-        pv = cast(int, self._get(self._get_property_name()))
-        if pv is None:
-            return None
-        return WritingMode2Enum(pv)
-
-    @prop_mode.setter
-    def prop_mode(self, value: WritingMode2Enum | None):
-        if value is None:
-            self._remove(self._get_property_name())
-            return
-        self._set(self._get_property_name(), value.value)
+    def prop_x(self) -> int:
+        """Gets/Sets x value"""
+        return self._get(self._props.width)
+
+    @prop_x.setter
+    def prop_x(self, value: int) -> None:
+        self._set(self._props.width, value)
+
+    @property
+    def prop_y(self) -> int:
+        """Gets/Sets y value."""
+        return self._get(self._props.height)
+
+    @prop_y.setter
+    def prop_y(self, value: int) -> None:
+        self._set(self._props.height, value)
 
     @property
-    def default(self: _TWritingMode) -> _TWritingMode:
-        """Gets ``WritingMode`` default."""
+    def _props(self) -> StructSizeProps:
         try:
-            return self._default_inst
+            return self._props_internal_attributes
         except AttributeError:
-            self._default_inst = self.__class__(mode=WritingMode2Enum.PAGE, _cattribs=self._get_internal_cattribs())
-            self._default_inst._is_default_inst = True
-        return self._default_inst
+            self._props_internal_attributes = StructSizeProps(width="X", height="Y")
+        return self._props_internal_attributes
 
-    # endregion properties
+    # endregion Properties
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/area/color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/area/hatch.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/area/img.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/area/pattern.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/border/borders.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/border/borders.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/border/padding.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/border/shadow.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/border/sides.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/drop_cap/drop_caps.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/drop_cap/drop_caps.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/indent_space/indent.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/indent_space/indent.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/indent_space/indent_spacing.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/indent_space/indent_spacing.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/indent_space/line_spacing.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/indent_space/line_spacing.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/indent_space/spacing.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/indent_space/spacing.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/outline_list/line_num.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/outline_list/line_num.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/outline_list/list_style.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/outline_list/list_style.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/outline_list/outline.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/outline_list/outline.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/outline_list/outline_list.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/outline_list/outline_list.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/padding.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/tabs/tabs.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/tabs/tabs.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/text_flow/breaks.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/text_flow/breaks.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/text_flow/flow_options.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/text_flow/flow_options.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/text_flow/hyphenation.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/text_flow/hyphenation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/text_flow/text_flow.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/text_flow/text_flow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/para/transparent/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/para/transparent/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/shape/area/shadow.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/shape/area/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/table/background/color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/table/background/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/table/background/img.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/table/background/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/table/borders/borders.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/table/borders/borders.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/direct/write/table/props/table_properties.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/direct/write/table/props/table_properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/alignment/properties.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/alignment/properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/alignment/text_align.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/alignment/text_align.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/alignment/text_orientation.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/alignment/text_orientation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/background/color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/background/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/border/borders.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/border/borders.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/cell_protection/cell_protection.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/cell_protection/cell_protection.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/cell_style_base.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/cell_style_base.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/cell_style_base_multi.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/cell_style_base_multi.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/font/font_effects.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/font/font_effects.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/font/font_only.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/font/font_only.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/area/color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/area/img.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/border/padding.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/border/shadow.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/border/sides.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/area/color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/area/img.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/border/padding.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/border/shadow.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/border/sides.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/footer/footer.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/footer/footer.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/area/color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/area/img.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/border/padding.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/border/shadow.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/border/sides.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/header/header.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/header/header.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/page/layout_settings.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/page/layout_settings.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/page/margins.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/page/margins.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/page/paper_format.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/page/paper_format.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/sheet/order.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/sheet/order.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/sheet/printing.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/sheet/printing.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/sheet/scale_num_of_pages.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/sheet/scale_num_of_pages.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/sheet/scale_pages_width_height.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/sheet/scale_pages_width_height.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/calc/page/sheet/scale_reduce_enlarge.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/calc/page/sheet/scale_reduce_enlarge.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/border/padding.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/border/shadow.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/border/sides.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/char_style_base_multi.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/char_style_base_multi.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/font/font_effects.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/font/font_effects.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/font/font_only.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/font/font_only.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/font/font_position.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/font/font_position.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/char/highlight/highlight.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/char/highlight/highlight.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/fill/area/img.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/fill/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/fill/fill_style_base_multi.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/fill/fill_style_base_multi.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/area/color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/area/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/area/hatch.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/area/img.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/area/pattern.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/border/padding.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/border/shadow.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/border/sides.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/frame_style_base_multi.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/frame_style_base_multi.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/frame_type/anchor.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/frame_type/anchor.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/frame_type/position.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/frame_type/position.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/frame_type/size.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/frame_type/size.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/options/align.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/options/align.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/options/properties.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/options/properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/options/protect.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/options/protect.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/transparent/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/transparent/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/transparent/transparency.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/transparent/transparency.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/wrap/options.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/wrap/options.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/wrap/settings.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/wrap/settings.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/frame/wrap/spacing.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/frame/wrap/spacing.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/area/color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/area/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/area/hatch.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/area/img.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/area/pattern.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/border/padding.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/border/shadow.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/border/sides.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/area/color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/area/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/area/hatch.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/area/img.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/area/pattern.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/border/padding.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/border/shadow.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/border/sides.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/footer.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/footer.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/transparency/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/transparency/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/footer/transparency/transparency.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/footer/transparency/transparency.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/area/color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/area/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/area/hatch.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/area/img.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/area/pattern.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/border/padding.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/border/shadow.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/border/sides.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/header.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/header.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/transparency/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/transparency/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/header/transparency/transparency.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/header/transparency/transparency.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/page/layout_settings.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/page/layout_settings.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/page/margins.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/page/margins.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/page/paper_format.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/page/paper_format.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/page_style_base_multi.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/page_style_base_multi.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/transparency/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/transparency/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/page/transparency/transparency.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/page/transparency/transparency.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/align/alignment.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/align/alignment.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/area/color.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/area/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/area/hatch.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/area/img.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/area/pattern.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/border/borders.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/border/borders.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/border/padding.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/border/shadow.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/border/sides.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/drop_cap/drop_caps.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/drop_cap/drop_caps.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/font/font_effects.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/font/font_effects.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/font/font_only.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/font/font_only.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/font/font_position.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/font/font_position.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/highlight/highlight.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/highlight/highlight.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/indent_space/indent.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/indent_space/indent.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/indent_space/line_spacing.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/indent_space/line_spacing.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/indent_space/spacing.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/indent_space/spacing.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/outline_list/line_num.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/outline_list/line_num.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/outline_list/list_style.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/outline_list/list_style.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/outline_list/outline.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/outline_list/outline.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/para_style_base_multi.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/para_style_base_multi.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/tabs/tabs.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/tabs/tabs.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/text_flow/breaks.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/text_flow/breaks.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/text_flow/flow_options.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/text_flow/flow_options.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/text_flow/hyphenation.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/text_flow/hyphenation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/transparent/gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/transparent/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/modify/write/para/transparent/transparency.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/modify/write/para/transparent/transparency.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/preset/preset_gradient.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/preset/preset_gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/preset/preset_hatch.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/preset/preset_hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/preset/preset_image.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/preset/preset_image.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/preset/preset_paper_format.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/preset/preset_paper_format.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/preset/preset_pattern.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/preset/preset_pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/inner/style_base.py` & `ooo_dev_tools-0.9.4/ooodev/format/inner/style_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # region Imports
 from __future__ import annotations
 from typing import Any, Dict, NamedTuple, Tuple, TYPE_CHECKING, Type, TypeVar, cast, overload
 import uno
-from com.sun.star.container import XNameContainer
 from com.sun.star.beans import XPropertySet
+from com.sun.star.container import XNameContainer
+from com.sun.star.lang import XMultiServiceFactory
 
 # import random
 # import string
 
 from ooodev.utils import props as mProps
 from ooodev.utils import info as mInfo
 from ooodev.utils import lo as mLo
@@ -346,15 +347,20 @@
 
     # endregion Services
 
     # region Internal Methods
     def _props_set(self, obj: object, **kwargs: Any) -> None:
         # set properties. Can be overriden in child classes
         # may be usful to wrap in try statements in child classes
-        mProps.Props.set(obj, **kwargs)
+        try:
+            mProps.Props.set(obj, **kwargs)
+        except mEx.MultiError as e:
+            mLo.Lo.print(f"{self.__class__.__name__}.apply(): Unable to set Property")
+            for err in e.errors:
+                mLo.Lo.print(f"  {err}")
 
     def _copy_missing_attribs(self, src: TStyleBase, dst: TStyleBase, *args: str) -> None:
         """
         Copies attribs from source to dst if dst does not already have the attrib.
 
         Args:
             src (TStyleBase): Source
@@ -402,39 +408,44 @@
 
         Args:
             obj (object): UNO Object that styles are to be applied.
             kwargs (Any, optional): Expandable list of key value pairs that may be used in child classes.
 
         Keyword Arguments:
             override_dv (Dic[str, Any], optional): if passed in this dictionary is used to set properties instead of internal dictionary of property values.
+            validate (bool, optional): if ``False`` then ``obj`` is not validated. Defaults to ``True``.
 
         :events:
             .. cssclass:: lo_event
 
                 - :py:attr:`~.events.format_named_event.FormatNamedEvent.STYLE_APPLYING` :eventref:`src-docs-event-cancel`
                 - :py:attr:`~.events.format_named_event.FormatNamedEvent.STYLE_APPLYED` :eventref:`src-docs-event`
 
         Returns:
             None:
+
+        .. versionchanged:: 0.9.4
+            Added ``validate`` keyword arguments.
         """
+        validate = bool(kwargs.get("validate", True))
         if "override_dv" in kwargs:
             dv = kwargs["override_dv"]
         else:
             dv = self._get_properties()
         if len(dv) > 0:
-            if self._is_valid_obj(obj):
+            if validate is False or self._is_valid_obj(obj):
                 cargs = CancelEventArgs(source=f"{self.apply.__qualname__}")
                 cargs.event_data = self
                 self._events.trigger(FormatNamedEvent.STYLE_APPLYING, cargs)
                 if cargs.cancel:
                     return
                 events = Events(source=self)
                 events.on(PropsNamedEvent.PROP_SETTING, _on_props_setting)
                 events.on(PropsNamedEvent.PROP_SET, _on_props_set)
-                # mProps.Props.set(obj, **dv)
+                events.on(PropsNamedEvent.PROP_SET_ERROR, _on_props_set_error)
                 self._props_set(obj, **dv)
                 events = None
                 eargs = EventArgs.from_args(cargs)
                 self._events.trigger(FormatNamedEvent.STYLE_APPLIED, eargs)
             else:
                 self._print_not_valid_srv("apply")
 
@@ -625,26 +636,37 @@
             event_args (KeyValueCancelArgs): Event Args
         """
         # can be overriden in child classes.
         pass
 
     def on_property_set(self, source: Any, event_args: KeyValArgs) -> None:
         """
-        Triggers for each property that is set
+        Triggers for each property that is set.
+
+        Args:
+            source (Any): Event Source.
+            event_args (KeyValArgs): Event Args
+        """
+        # can be overriden in child classes.
+        pass
+
+    def on_property_set_error(self, source: Any, event_args: KeyValCancelArgs) -> None:
+        """
+        Triggers for each property that fails to set.
 
         Args:
             source (Any): Event Source.
             event_args (KeyValArgs): Event Args
         """
         # can be overriden in child classes.
         pass
 
     def on_property_backing_up(self, source: Any, event_args: KeyValCancelArgs) -> None:
         """
-        Triggers before each property that is about to be backup up during backup
+        Triggers before each property that is about to be backup up during backup.
 
         Args:
             source (Any): Event Source.
             event_args (KeyValueCancelArgs): Event Args.
         """
         # can be overriden in child classes.
         pass
@@ -727,17 +749,25 @@
 
     # region Named Container Methods
 
     def _container_get_service_name(self) -> str:
         raise NotImplementedError
 
     def _container_get_inst(self) -> XNameContainer:
-        container = mLo.Lo.create_instance_msf(XNameContainer, self._container_get_service_name(), raise_err=True)
+        container = mLo.Lo.create_instance_msf(
+            XNameContainer,
+            service_name=self._container_get_service_name(),
+            msf=self._container_get_msf(),
+            raise_err=True,
+        )
         return container
 
+    def _container_get_msf(self) -> XMultiServiceFactory | None:
+        return None
+
     def _container_add_value(
         self, name: str, obj: object, allow_update: bool = True, nc: XNameContainer | None = None
     ) -> None:
         if nc is None:
             nc = self._container_get_inst()
         if nc.hasByName(name):
             if allow_update:
@@ -1269,15 +1299,14 @@
             p = mLo.Lo.qi(XPropertySet, obj)
             if p is None:
                 mLo.Lo.print(
                     f"{self.__class__.__name__}.apply(): Not a UNO Object for style. Unable to set Style Properties"
                 )
                 return
         else:
-
             if not self._is_valid_doc(obj):
                 mLo.Lo.print(
                     f"{self.__class__.__name__}.apply(): Not a UNO Object for style. Unable to set Style Properties"
                 )
                 return
             p = self.get_style_props(obj)
         super().apply(p, **kwargs)
@@ -1518,14 +1547,20 @@
 
 def _on_props_set(source: Any, event_args: KeyValArgs, *args, **kwargs) -> None:
     instance = cast(StyleBase, event_args.event_source)
     instance.on_property_set(source, event_args)
     instance._events.trigger(FormatNamedEvent.STYLE_PROPERTY_APPLIED, event_args)
 
 
+def _on_props_set_error(source: Any, event_args: KeyValCancelArgs, *args, **kwargs) -> None:
+    instance = cast(StyleBase, event_args.event_source)
+    instance.on_property_set_error(source, event_args)
+    instance._events.trigger(FormatNamedEvent.STYLE_PROPERTY_ERROR, event_args)
+
+
 def _on_props_restore_setting(source: Any, event_args: KeyValCancelArgs, *args, **kwargs) -> None:
     instance = cast(StyleBase, event_args.event_source)
     instance.on_property_restore_setting(source, event_args)
     instance._events.trigger(FormatNamedEvent.STYLE_PROPERTY_RESTORING, event_args)
 
 
 def _on_props_restore_set(source: Any, event_args: KeyValArgs, *args, **kwargs) -> None:
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/readme.md` & `ooo_dev_tools-0.9.4/ooodev/format/readme.md`

 * *Files 22% similar despite different names*

```diff
@@ -295,35 +295,48 @@
                 id{{BulletList}}
                 id{{Char}}
                 id{{Frame}}
                 id{{page}}
                 id{{Para}}
         calc
             [direct]
-                borders
-                    id{{Borders}}
-                    id{{Padding}}
-                    id{{Shadow}}
-                font
-                    id{{Font}}
-                    id{{FontOnly}}
-                    id{{FontEffects}}
+                cell
+                    alignment
+                        id{{TextAlign}}
+                        id{{TextOrientation}}
+                        id{{Properties}}
+                    borders
+                        id{{Borders}}
+                        id{{Padding}}
+                        id{{Shadow}}
+                    font
+                        id{{Font}}
+                        id{{FontOnly}}
+                        id{{FontEffects}}
+                    background
+                        id{{Color}}
+                    cell_protection
+                        id{{CellProtection}}
+                    numbers
+                        id{{Numbers}}
             [modify]
                 cell
                     alignment
                         id{{TextAlign}}
                         id{{TextOrientation}}
                         id{{Properties}}
                     background
                         id{{Color}}
                     borders
                         id{{Borders}}
                     font
                         id{{FontOnly}}
                         id{{FontEffects}}
+                    numbers
+                        id{{Numbers}}
                 page
                     background
                         id{{Color}}
                         id{{Img}}
                     borders
                         id{{Padding}}
                         id{{Sides}}
@@ -355,14 +368,129 @@
                         id{{Printing}}
                         id{{ScaleReduceEnlarge}}
                         id{{ScaleNumOfPages}}
                         id{{ScalePagesWidthHeight}}
             [style]
                 id{{Cell}}
                 id{{Page}}
+        chart2
+            [direct]
+                axis
+                    numbers
+                        id{{Numbers}}
+                    font
+                        id{{FontEffects}}
+                        id{{FontOnly}}
+                    line
+                        id{{LineProperties}}
+                    positioning
+                        id{{AxisLine}}
+                        id{{IntervalMarks}}
+                        id{{LabelPosition}}
+                        id{{PositionAxis}}
+                general
+                    area
+                        id{{Color}}
+                        id{{Gradient}}
+                        id{{Img}}
+                        id{{Pattern}}
+                        id{{Hatch}}
+                    borders
+                        id{{LineProperties}}
+                    position_size
+                        id{{Position}}
+                        id{{Size}}
+                    transparency
+                        id{{Gradient}}
+                        id{{Transparency}}
+                    numbers
+                        id{{Numbers}}
+                grid
+                    id{{LineProperties}}
+                legend
+                    area
+                        id{{Color}}
+                        id{{Gradient}}
+                        id{{Img}}
+                        id{{Pattern}}
+                        id{{Hatch}}
+                    borders
+                        id{{LineProperties}}
+                    font
+                        id{{Font}}
+                        id{{FontEffects}}
+                        id{{FontOnly}}
+                    position_size
+                        id{{Position}}
+                    transparency
+                        id{{Gradient}}
+                        id{{Transparency}}
+                series
+                    data_series
+                        area
+                            id{{Color}}
+                            id{{Gradient}}
+                            id{{Img}}
+                            id{{Pattern}}
+                            id{{Hatch}}
+                        borders
+                            id{{LineProperties}}
+                        options
+                            id{{AlignSeries}}
+                            id{{LegendEntry}}
+                            id{{Orientation}}
+                            id{{Plot}}
+                            id{{PlotSimple}}
+                            id{{Settings}}
+                            id{{Orientation}}
+                        transparency
+                            id{{Gradient}}
+                            id{{Transparency}}
+                    data_labels
+                        data_labels
+                            id{{AttribOptions}}
+                            id{{NumberFormat}}
+                            id{{Orientation}}
+                            id{{PercentFormat}}
+                            id{{TextAttribs}}
+                        borders
+                            id{{LineProperties}}
+                        font
+                            id{{FontEffects}}
+                            id{{FontOnly}}
+                title
+                    alignment
+                        id{{Direction}}
+                        id{{Orientation}}
+                    area
+                        id{{Color}}
+                        id{{Gradient}}
+                        id{{Img}}
+                        id{{Pattern}}
+                        id{{Hatch}}
+                    borders
+                        id{{LineProperties}}
+                    font
+                        id{{Font}}
+                        id{{FontEffects}}
+                        id{{FontOnly}}
+                    position_size
+                        id{{Position}}
+                wall
+                    area
+                        id{{Color}}
+                        id{{Gradient}}
+                        id{{Img}}
+                        id{{Pattern}}
+                        id{{Hatch}}
+                    borders
+                        id{{LineProperties}}
+                    transparency
+                        id{{Gradient}}
+                        id{{Transparency}}
         draw
             [direct]
                 area
                     id{{Img}}
                     id{{Pattern}}
                     id{{Hatch}}
                 transparency
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/styler.py` & `ooo_dev_tools-0.9.4/ooodev/format/styler.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/char/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/char/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/char/font/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/char/font/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 from ooo.dyn.awt.font_slant import FontSlant as FontSlant
 from ooo.dyn.awt.font_strikeout import FontStrikeoutEnum as FontStrikeoutEnum
 from ooo.dyn.awt.font_underline import FontUnderlineEnum as FontUnderlineEnum
 from ooo.dyn.awt.font_weight import FontWeightEnum as FontWeightEnum
 from ooo.dyn.style.case_map import CaseMapEnum as CaseMapEnum
 from ooo.dyn.table.shadow_format import ShadowFormat as ShadowFormat
 from ooo.dyn.table.shadow_location import ShadowLocation as ShadowLocation
-from ooodev.format.writer.style.char.kind.style_char_kind import StyleCharKind as StyleCharKind
-from ooodev.format.inner.direct.write.char.font.font_position import FontPosition as FontPosition
-from ooodev.format.inner.direct.write.char.font.font_position import FontScriptKind as FontScriptKind
-from ooodev.format.inner.direct.write.char.font.font_position import CharSpacingKind as CharSpacingKind
+
 from ooodev.format.inner.direct.write.char.font.font import Font as Font
 from ooodev.format.inner.direct.write.char.font.font_effects import FontEffects as FontEffects
 from ooodev.format.inner.direct.write.char.font.font_effects import FontLine as FontLine
-from ooodev.format.inner.direct.write.char.font.font_only import FontOnly as FontOnly
 from ooodev.format.inner.direct.write.char.font.font_only import FontLang as FontLang
+from ooodev.format.inner.direct.write.char.font.font_only import FontOnly as FontOnly
+from ooodev.format.inner.direct.write.char.font.font_position import CharSpacingKind as CharSpacingKind
+from ooodev.format.inner.direct.write.char.font.font_position import FontPosition as FontPosition
+from ooodev.format.inner.direct.write.char.font.font_position import FontScriptKind as FontScriptKind
+from ooodev.format.writer.style.char.kind.style_char_kind import StyleCharKind as StyleCharKind
 
 __all__ = [
     "FontPosition",
     "FontScriptKind",
     "CharSpacingKind",
     "Font",
     "FontEffects",
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/frame/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/frame/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/frame/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/frame/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/frame/options/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/frame/options/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/frame/transparency/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/frame/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/frame/type/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/frame/type/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/image/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/image/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/image/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/image/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/image/transparency/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/image/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/image/type/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/image/type/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/obj/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/obj/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/obj/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/obj/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/obj/transparency/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/obj/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/obj/type/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/obj/type/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/page/footer/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/page/footer/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/page/header/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/page/header/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/alignment/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/outline_list/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/outline_list/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/para/transparency/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/para/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/shape/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/shape/area/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import uno
 from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
 from ooo.dyn.drawing.hatch_style import HatchStyle as HatchStyle
 from ooo.dyn.drawing.rectangle_point import RectanglePoint as RectanglePoint
 
-from ooodev.utils.data_type.angle import Angle as Angle
-from ooodev.utils.data_type.color_range import ColorRange as ColorRange
-from ooodev.utils.data_type.intensity import Intensity as Intensity
-from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
-from ooodev.utils.data_type.offset import Offset as Offset
 from ooodev.format.inner.common.format_types.offset_column import OffsetColumn as OffsetColumn
 from ooodev.format.inner.common.format_types.offset_row import OffsetRow as OffsetRow
-from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 from ooodev.format.inner.common.format_types.size_percent import SizePercent as SizePercent
-from ooodev.format.inner.direct.write.fill.area.img import ImgStyleKind as ImgStyleKind
-from ooodev.format.inner.preset.preset_gradient import PresetGradientKind as PresetGradientKind
-from ooodev.format.inner.preset.preset_hatch import PresetHatchKind as PresetHatchKind
-from ooodev.format.inner.preset.preset_image import PresetImageKind as PresetImageKind
-from ooodev.format.inner.preset.preset_pattern import PresetPatternKind as PresetPatternKind
 from ooodev.format.inner.direct.write.fill.area.fill_color import FillColor as Color
 from ooodev.format.inner.direct.write.fill.area.gradient import Gradient as Gradient
 from ooodev.format.inner.direct.write.fill.area.hatch import Hatch as Hatch
 from ooodev.format.inner.direct.write.fill.area.img import Img as Img
+from ooodev.format.inner.direct.write.fill.area.img import ImgStyleKind as ImgStyleKind
 from ooodev.format.inner.direct.write.fill.area.pattern import Pattern as Pattern
+from ooodev.format.inner.preset.preset_gradient import PresetGradientKind as PresetGradientKind
+from ooodev.format.inner.preset.preset_hatch import PresetHatchKind as PresetHatchKind
+from ooodev.format.inner.preset.preset_image import PresetImageKind as PresetImageKind
+from ooodev.format.inner.preset.preset_pattern import PresetPatternKind as PresetPatternKind
+from ooodev.utils.data_type.angle import Angle as Angle
+from ooodev.utils.data_type.color_range import ColorRange as ColorRange
+from ooodev.utils.data_type.intensity import Intensity as Intensity
+from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
+from ooodev.utils.data_type.offset import Offset as Offset
+from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 
 __all__ = [
     "Color",
     "Gradient",
     "Hatch",
     "Img",
     "Pattern",
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/shape/transparency/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/shape/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/table/background/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/table/background/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/direct/table/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/direct/table/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/char/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/char/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/char/font/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/char/font/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/frame/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/frame/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/frame/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/frame/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/frame/options/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/frame/options/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/frame/transparency/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/frame/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/frame/type/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/frame/type/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/frame/wrap/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/frame/wrap/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/footer/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/footer/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/footer/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/footer/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/footer/transparency/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/footer/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/header/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/header/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/header/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/header/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/header/transparency/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/header/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/page/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/page/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/page_style_base.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/page_style_base.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/page_style_base_multi.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/page_style_base_multi.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/page/transparency/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/page/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/alignment/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/area/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/borders/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/font/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/font/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/indent_space/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/indent_space/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/outline_list/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/outline_list/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/text_flow/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/text_flow/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/modify/para/transparency/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/modify/para/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/bullet_list/bullet_list.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/bullet_list/bullet_list.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/char/char.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/char/char.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/char/kind/style_char_kind.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/char/kind/style_char_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/frame/frame.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/frame/frame.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/lst/style_list_kind.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/lst/style_list_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/page/page.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/page/page.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/style_para_html_kind.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/style_para_html_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/style_para_index_kind.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/style_para_index_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/style_para_kind.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/style_para_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/style_para_list_kind.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/style_para_list_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/style_para_special_kind.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/style_para_special_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/kind/style_para_text_kind.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/kind/style_para_text_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/format/writer/style/para/para.py` & `ooo_dev_tools-0.9.4/ooodev/format/writer/style/para/para.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/formatters/format_list_item.py` & `ooo_dev_tools-0.9.4/ooodev/formatters/format_list_item.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/formatters/format_string.py` & `ooo_dev_tools-0.9.4/ooodev/formatters/format_string.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/formatters/format_table_item.py` & `ooo_dev_tools-0.9.4/ooodev/formatters/format_table_item.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/formatters/formatter_list.py` & `ooo_dev_tools-0.9.4/ooodev/formatters/formatter_list.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/formatters/formatter_table.py` & `ooo_dev_tools-0.9.4/ooodev/formatters/formatter_table.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/formatters/table_item_kind.py` & `ooo_dev_tools-0.9.4/ooodev/formatters/table_item_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/formatters/table_item_processer.py` & `ooo_dev_tools-0.9.4/ooodev/formatters/table_item_processer.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/lazy/lazy_import.py` & `ooo_dev_tools-0.9.4/ooodev/lazy/lazy_import.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/listeners/x_event_adapter.py` & `ooo_dev_tools-0.9.4/ooodev/listeners/x_event_adapter.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/listeners/x_modify_adapter.py` & `ooo_dev_tools-0.9.4/ooodev/listeners/x_modify_adapter.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/listeners/x_selection_change_adapter.py` & `ooo_dev_tools-0.9.4/ooodev/listeners/x_selection_change_adapter.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/listeners/x_terminate_adapter.py` & `ooo_dev_tools-0.9.4/ooodev/listeners/x_terminate_adapter.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/listeners/x_top_window_adapter.py` & `ooo_dev_tools-0.9.4/ooodev/listeners/x_top_window_adapter.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/meta/class_property_readonly.py` & `ooo_dev_tools-0.9.4/ooodev/meta/class_property_readonly.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/meta/deleted_attrib.py` & `ooo_dev_tools-0.9.4/ooodev/meta/deleted_attrib.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/meta/deleted_enum_meta.py` & `ooo_dev_tools-0.9.4/ooodev/meta/deleted_enum_meta.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/meta/disabled_method.py` & `ooo_dev_tools-0.9.4/ooodev/meta/disabled_method.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/meta/static_meta.py` & `ooo_dev_tools-0.9.4/ooodev/meta/static_meta.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/meta/static_prop.py` & `ooo_dev_tools-0.9.4/ooodev/meta/static_prop.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/mock/mock_g.py` & `ooo_dev_tools-0.9.4/ooodev/mock/mock_g.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/mock/unohelper.py` & `ooo_dev_tools-0.9.4/ooodev/mock/unohelper.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/office/calc.py` & `ooo_dev_tools-0.9.4/ooodev/office/calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Python conversion of Calc.java by Andrew Davison, ad@fivedots.coe.psu.ac.th
 # See Also: https://fivedots.coe.psu.ac.th/~ad/jlop/
 # region Imports
 from __future__ import annotations
 from enum import IntEnum, IntFlag, Enum
 import numbers
 import re
-from typing import Any, Iterable, List, Tuple, cast, overload, Sequence, TYPE_CHECKING
+from typing import Any, List, Tuple, cast, overload, Sequence, TYPE_CHECKING
 import uno
 
 # from ..mock import mock_g
 
 # if not mock_g.DOCS_BUILDING:
 # not importing for doc building just result in short import name for
 # args that use these.
@@ -87,14 +87,16 @@
 from ooo.dyn.table.cell_content_type import CellContentType
 from ooo.dyn.table.cell_hori_justify import CellHoriJustify
 from ooo.dyn.table.cell_vert_justify2 import CellVertJustify2
 
 from ..exceptions import ex as mEx
 from ..formatters.formatter_table import FormatterTable
 from ..proto.style_obj import StyleObj
+from ..units import UnitObj
+from ..units import UnitConvert
 from ..utils import gui as mGui
 from ..utils import info as mInfo
 from ..utils import lo as mLo
 from ..utils import props as mProps
 from ..utils import table_helper as mTblHelper
 from ..utils import view_state as mViewState
 from ..utils.color import CommonColor, Color
@@ -2223,15 +2225,15 @@
     # endregion clear_cells()
 
     # endregion ------------ insert/remove rows, columns, cells -----
 
     # region --------------- set/get values in cells -------------------
     # region    set_val()
     @staticmethod
-    def _set_val_by_cell(value: object, cell: XCell, styles: Iterable[StyleObj] = None) -> None:
+    def _set_val_by_cell(value: object, cell: XCell, styles: Sequence[StyleObj] = None) -> None:
         if isinstance(value, numbers.Number):
             cell.setValue(float(value))
         elif isinstance(value, str):
             cell.setFormula(str(value))
         else:
             mLo.Lo.print(f"Value is not a number or string: {value}")
         if styles is None:
@@ -2245,81 +2247,81 @@
         )
         for style in styles:
             if style.support_service(*supported_styles):
                 style.apply(cell)
 
     @classmethod
     def _set_val_by_cell_name(
-        cls, value: object, sheet: XSpreadsheet, cell_name: str, styles: Iterable[StyleObj] = None
+        cls, value: object, sheet: XSpreadsheet, cell_name: str, styles: Sequence[StyleObj] = None
     ) -> None:
         pos = cls.get_cell_position(cell_name)
         cls._set_val_by_col_row(value=value, sheet=sheet, col=pos.X, row=pos.Y, styles=styles)
 
     @classmethod
     def _set_val_by_col_row(
-        cls, value: object, sheet: XSpreadsheet, col: int, row: int, styles: Iterable[StyleObj] = None
+        cls, value: object, sheet: XSpreadsheet, col: int, row: int, styles: Sequence[StyleObj] = None
     ) -> None:
         cell = cls.get_cell(sheet=sheet, col=col, row=row)
         cls._set_val_by_cell(value=value, cell=cell, styles=styles)
 
     @overload
     @classmethod
     def set_val(cls, value: object, cell: XCell) -> None:
         ...
 
     @overload
     @classmethod
-    def set_val(cls, value: object, cell: XCell, *, styles: Iterable[StyleObj]) -> None:
+    def set_val(cls, value: object, cell: XCell, *, styles: Sequence[StyleObj]) -> None:
         ...
 
     @overload
     @classmethod
     def set_val(cls, value: object, sheet: XSpreadsheet, cell_name: str) -> None:
         ...
 
     @overload
     @classmethod
-    def set_val(cls, value: object, sheet: XSpreadsheet, cell_name: str, *, styles: Iterable[StyleObj]) -> None:
+    def set_val(cls, value: object, sheet: XSpreadsheet, cell_name: str, *, styles: Sequence[StyleObj]) -> None:
         ...
 
     @overload
     @classmethod
     def set_val(cls, value: object, sheet: XSpreadsheet, cell_obj: mCellObj.CellObj) -> None:
         ...
 
     @overload
     @classmethod
     def set_val(
-        cls, value: object, sheet: XSpreadsheet, cell_obj: mCellObj.CellObj, *, styles: Iterable[StyleObj]
+        cls, value: object, sheet: XSpreadsheet, cell_obj: mCellObj.CellObj, *, styles: Sequence[StyleObj]
     ) -> None:
         ...
 
     @overload
     @classmethod
     def set_val(cls, value: object, sheet: XSpreadsheet, col: int, row: int) -> None:
         ...
 
     @overload
     @classmethod
-    def set_val(cls, value: object, sheet: XSpreadsheet, col: int, row: int, *, styles: Iterable[StyleObj]) -> None:
+    def set_val(cls, value: object, sheet: XSpreadsheet, col: int, row: int, *, styles: Sequence[StyleObj]) -> None:
         ...
 
     @classmethod
     def set_val(cls, *args, **kwargs) -> None:
         """
         Sets the value of a cell
 
         Args:
             value (object): Value for cell
             cell (XCell): Cell to assign value
             sheet (XSpreadsheet): Spreadsheet
             cell_name (str): Name of cell to set value of such as 'B4'
             col (int): Cell column as zero-based integer
             row (int): Cell row as zero-based integer
-            styles (Iterable[StyleObj], optional): One or more styles to apply to cell.
+            styles (Sequence[StyleObj], optional): One or more styles to apply to cell.
 
         Returns:
             None:
 
         .. versionchanged:: 0.9.1
             Added overloads for styles.
         """
@@ -2754,15 +2756,15 @@
     # endregion ------------ set/get values in cells -----------------
 
     # region --------------- set/get values in 2D array ----------------
 
     # region    set_array()
     @classmethod
     def _set_array_doc_addr(
-        cls, values: Table, doc: XSpreadsheetDocument, addr: CellAddress, styles: Iterable[StyleObj] = None
+        cls, values: Table, doc: XSpreadsheetDocument, addr: CellAddress, styles: Sequence[StyleObj] = None
     ) -> None:
         v_len = len(values)
         if v_len == 0:
             mLo.Lo.print("Values has not data")
             return
         sheet = cls._get_sheet_index(doc=doc, index=addr.Sheet)
         col_end = addr.Column + (len(values[0]) - 1)
@@ -2775,60 +2777,60 @@
     @overload
     @classmethod
     def set_array(cls, values: Table, cell_range: XCellRange) -> None:
         ...
 
     @overload
     @classmethod
-    def set_array(cls, values: Table, cell_range: XCellRange, *, styles: Iterable[StyleObj]) -> None:
+    def set_array(cls, values: Table, cell_range: XCellRange, *, styles: Sequence[StyleObj]) -> None:
         ...
 
     @overload
     @classmethod
     def set_array(cls, values: Table, sheet: XSpreadsheet, name: str) -> None:
         ...
 
     @overload
     @classmethod
-    def set_array(cls, values: Table, sheet: XSpreadsheet, name: str, *, styles: Iterable[StyleObj]) -> None:
+    def set_array(cls, values: Table, sheet: XSpreadsheet, name: str, *, styles: Sequence[StyleObj]) -> None:
         ...
 
     @overload
     @classmethod
     def set_array(cls, values: Table, sheet: XSpreadsheet, range_obj: mRngObj.RangeObj) -> None:
         ...
 
     @overload
     @classmethod
     def set_array(
-        cls, values: Table, sheet: XSpreadsheet, range_obj: mRngObj.RangeObj, *, styles: Iterable[StyleObj]
+        cls, values: Table, sheet: XSpreadsheet, range_obj: mRngObj.RangeObj, *, styles: Sequence[StyleObj]
     ) -> None:
         ...
 
     @overload
     @classmethod
     def set_array(cls, values: Table, sheet: XSpreadsheet, cell_obj: mCellObj.CellObj) -> None:
         ...
 
     @overload
     @classmethod
     def set_array(
-        cls, values: Table, sheet: XSpreadsheet, cell_obj: mCellObj.CellObj, *, styles: Iterable[StyleObj]
+        cls, values: Table, sheet: XSpreadsheet, cell_obj: mCellObj.CellObj, *, styles: Sequence[StyleObj]
     ) -> None:
         ...
 
     @overload
     @classmethod
     def set_array(cls, values: Table, doc: XSpreadsheetDocument, addr: CellAddress) -> None:
         ...
 
     @overload
     @classmethod
     def set_array(
-        cls, values: Table, doc: XSpreadsheetDocument, addr: CellAddress, *, styles: Iterable[StyleObj]
+        cls, values: Table, doc: XSpreadsheetDocument, addr: CellAddress, *, styles: Sequence[StyleObj]
     ) -> None:
         ...
 
     @overload
     @classmethod
     def set_array(
         cls,
@@ -2848,15 +2850,15 @@
         values: Table,
         sheet: XSpreadsheet,
         col_start: int,
         row_start: int,
         col_end: int,
         row_end: int,
         *,
-        styles: Iterable[StyleObj],
+        styles: Sequence[StyleObj],
     ) -> None:
         ...
 
     @classmethod
     def set_array(cls, *args, **kwargs) -> None:
         """
         Inserts array of data into spreadsheet
@@ -2870,15 +2872,15 @@
             cell_obj (CellObj): Cell Object
             doc (XSpreadsheetDocument): Spreadsheet Document
             addr (CellAddress): Address to insert data.
             col_start (int): Zero-base Start Column
             row_start (int): Zero-base Start Row
             col_end (int): Zero-base End Column
             row_end (int): Zero-base End Row
-            styles (Iterable[StyleObj], optional): One or more styles to apply to cell range.
+            styles (Sequence[StyleObj], optional): One or more styles to apply to cell range.
 
         Returns:
             None:
 
         .. versionchanged:: 0.9.1
             Added overloads for styles.
         """
@@ -2969,24 +2971,24 @@
 
     # endregion set_array()
 
     # region set_array_range()
 
     @classmethod
     def _set_array_range(
-        cls, sheet: XSpreadsheet, range_name: str | mRngObj.RangeObj, values: Table, styles: Iterable[StyleObj] = None
+        cls, sheet: XSpreadsheet, range_name: str | mRngObj.RangeObj, values: Table, styles: Sequence[StyleObj] = None
     ) -> None:
         """
         Inserts array of data into spreadsheet
 
         Args:
             sheet (XSpreadsheet): Spreadsheet
             range_name (str): Range to insert data such as 'A1:E12'
             values (Table): A 2-Dimensional array of value such as a list of list or tuple of tuples.
-            styles (Iterable[StyleObj], optional): One or more styles to apply to cell range.
+            styles (Sequence[StyleObj], optional): One or more styles to apply to cell range.
 
         Returns:
             None:
         """
         v_len = len(values)
         if v_len == 0:
             mLo.Lo.print("Values has not data")
@@ -2998,41 +3000,41 @@
     @classmethod
     def set_array_range(cls, sheet: XSpreadsheet, range_name: str, values: Table) -> None:
         ...
 
     @overload
     @classmethod
     def set_array_range(
-        cls, sheet: XSpreadsheet, range_name: str, values: Table, *, styles: Iterable[StyleObj]
+        cls, sheet: XSpreadsheet, range_name: str, values: Table, *, styles: Sequence[StyleObj]
     ) -> None:
         ...
 
     @overload
     @classmethod
     def set_array_range(cls, sheet: XSpreadsheet, range_obj: mRngObj.RangeObj, values: Table) -> None:
         ...
 
     @overload
     @classmethod
     def set_array_range(
-        cls, sheet: XSpreadsheet, range_obj: mRngObj.RangeObj, values: Table, *, styles: Iterable[StyleObj]
+        cls, sheet: XSpreadsheet, range_obj: mRngObj.RangeObj, values: Table, *, styles: Sequence[StyleObj]
     ) -> None:
         ...
 
     @classmethod
     def set_array_range(cls, *args, **kwargs) -> None:
         """
         Inserts array of data into spreadsheet
 
         Args:
             sheet (XSpreadsheet): Spreadsheet
             range_name (str): Range to insert data such as 'A1:E12'
             range_obj (RangeObj): Range Object
             values (Table): A 2-Dimensional array of value such as a list of list or tuple of tuples.
-            styles (Iterable[StyleObj], optional): One or more styles to apply to cell range.
+            styles (Sequence[StyleObj], optional): One or more styles to apply to cell range.
 
         Returns:
             None:
 
         .. versionchanged:: 0.9.1
             Added overloads for styles.
         """
@@ -3073,26 +3075,26 @@
     @overload
     @staticmethod
     def set_cell_range_array(cell_range: XCellRange, values: Table) -> None:
         ...
 
     @overload
     @staticmethod
-    def set_cell_range_array(cell_range: XCellRange, values: Table, styles: Iterable[StyleObj]) -> None:
+    def set_cell_range_array(cell_range: XCellRange, values: Table, styles: Sequence[StyleObj]) -> None:
         ...
 
     @staticmethod
-    def set_cell_range_array(cell_range: XCellRange, values: Table, styles: Iterable[StyleObj] = None) -> None:
+    def set_cell_range_array(cell_range: XCellRange, values: Table, styles: Sequence[StyleObj] = None) -> None:
         """
         Inserts array of data into spreadsheet
 
         Args:
             cell_range (XCellRange): Cell Range
             values (Table): A 2-Dimensional array of value such as a list of list or tuple of tuples.
-            styles (Iterable[StyleObj], optional): One or more styles to apply to cell range.
+            styles (Sequence[StyleObj], optional): One or more styles to apply to cell range.
 
         Returns:
             None:
 
         .. versionchanged:: 0.9.1
             Added overloads for styles.
         """
@@ -3121,24 +3123,24 @@
 
     # endregion set_cell_range_array()
 
     # region set_array_cell()
 
     @classmethod
     def _set_array_cell(
-        cls, sheet: XSpreadsheet, cell_name: str | mCellObj.CellObj, values: Table, styles: Iterable[StyleObj] = None
+        cls, sheet: XSpreadsheet, cell_name: str | mCellObj.CellObj, values: Table, styles: Sequence[StyleObj] = None
     ) -> None:
         """
         Inserts array of data into spreadsheet
 
         Args:
             sheet (XSpreadsheet): Spreadsheet
             cell_name (str): Cell Name such as 'A1'
             values (Table): A 2-Dimensional array of value such as a list of list or tuple of tuples.
-            styles (Iterable[StyleObj], optional): One or more styles to apply to cell range.
+            styles (Sequence[StyleObj], optional): One or more styles to apply to cell range.
         """
         v_len = len(values)
         if v_len == 0:
             mLo.Lo.print("Values has not data")
             return
         pos = cls.get_cell_position(cell_name)
         col_end = pos.X + (len(values[0]) - 1)
@@ -3152,22 +3154,22 @@
     @classmethod
     def set_array_cell(cls, sheet: XSpreadsheet, range_name: str, values: Table) -> None:
         ...
 
     @overload
     @classmethod
     def set_array_cell(
-        cls, sheet: XSpreadsheet, range_name: str, values: Table, *, styles: Iterable[StyleObj]
+        cls, sheet: XSpreadsheet, range_name: str, values: Table, *, styles: Sequence[StyleObj]
     ) -> None:
         ...
 
     @overload
     @classmethod
     def set_array_cell(
-        cls, sheet: XSpreadsheet, cell_obj: mCellObj.CellObj, values: Table, *, styles: Iterable[StyleObj]
+        cls, sheet: XSpreadsheet, cell_obj: mCellObj.CellObj, values: Table, *, styles: Sequence[StyleObj]
     ) -> None:
         ...
 
     @overload
     @classmethod
     def set_array_cell(cls, sheet: XSpreadsheet, cell_obj: mCellObj.CellObj, values: Table) -> None:
         ...
@@ -3178,15 +3180,15 @@
         Inserts array of data into spreadsheet
 
         Args:
             sheet (XSpreadsheet): Spreadsheet
             range_name (str): Range to insert data such as 'A1:E12'
             cell_obj (CellObj): Range Object
             values (Table): A 2-Dimensional array of value such as a list of list or tuple of tuples.
-            styles (Iterable[StyleObj], optional): One or more styles to apply to cell range.
+            styles (Sequence[StyleObj], optional): One or more styles to apply to cell range.
 
         .. versionchanged:: 0.9.1
             Added overloads for styles.
         """
         styles = kwargs.pop("styles", None)
         ordered_keys = (1, 2, 3)
         kargs_len = len(kwargs)
@@ -6987,21 +6989,21 @@
         cls._set_val_by_cell(value=cargs.event_data["headline"], cell=first_cell)
         _Events().trigger(CalcNamedEvent.CELLS_HIGH_LIGHTED, CellArgs.from_args(cargs))
         return first_cell
 
     # endregion highlight_range()
 
     @classmethod
-    def set_col_width(cls, sheet: XSpreadsheet, width: int, idx: int) -> XCellRange:
+    def set_col_width(cls, sheet: XSpreadsheet, width: int | UnitObj, idx: int) -> XCellRange:
         """
         Sets column width. width is in ``mm``, e.g. 6
 
         Args:
             sheet (XSpreadsheet): Spreadsheet
-            width (int): Width in mm
+            width (int, UnitObj): Width in ``mm`` units or :ref:`proto_unit_obj`.
             idx (int): Index of column
 
         Raises:
             CancelEventError: If SHEET_COL_WIDTH_SETTING event is canceled.
 
         Returns:
             XCellRange: Column cell range that width is applied on
@@ -7009,44 +7011,52 @@
         :events:
             .. cssclass:: lo_event
 
                 - :py:attr:`~.events.calc_named_event.CalcNamedEvent.SHEET_COL_WIDTH_SETTING` :eventref:`src-docs-sheet-event-col-width-setting`
                 - :py:attr:`~.events.calc_named_event.CalcNamedEvent.SHEET_COL_WIDTH_SET` :eventref:`src-docs-sheet-event-col-width-set`
 
         Note:
-            Event args ``index`` is set to ``idx`` value, ``event_data`` is set to ``width`` value.
+            Event args ``index`` is set to ``idx`` value, ``event_data`` is set to ``width`` value (``mm100`` units).
+
+        .. versionchanged:: 0.9.4
+            width can now also be ``UnitObj``
         """
+        try:
+            col_width = width.get_value_mm100()
+        except AttributeError:
+            col_width = UnitConvert.convert_mm_mm100(width)
         cargs = SheetCancelArgs(Calc.set_col_width.__qualname__)
         cargs.sheet = sheet
         cargs.index = idx
-        cargs.event_data = width
+        cargs.event_data = col_width
         _Events().trigger(CalcNamedEvent.SHEET_COL_WIDTH_SETTING, cargs)
         if cargs.cancel:
             raise mEx.CancelEventError(cargs)
-        if width <= 0:
+        col_width = cargs.event_data
+        if col_width <= 0:
             mLo.Lo.print("Width must be greater then 0")
             return None
         cell_range = cls.get_col_range(sheet=cargs.sheet, idx=cargs.index)
-        mProps.Props.set(cell_range, Width=(width * 100))
+        mProps.Props.set(cell_range, Width=col_width)
         _Events().trigger(CalcNamedEvent.SHEET_COL_WIDTH_SET, SheetArgs.from_args(cargs))
         return cell_range
 
     @classmethod
     def set_row_height(
         cls,
         sheet: XSpreadsheet,
-        height: int,
+        height: int | UnitObj,
         idx: int,
     ) -> XCellRange:
         """
         Sets column width. height is in ``mm``, e.g. 6
 
         Args:
             sheet (XSpreadsheet): Spreadsheet
-            height (int): Width in mm
+            height (int, UnitObj): Width in ``mm`` units or :ref:`proto_unit_obj`.
             idx (int): Index of Row
 
         Raises:
             CancelEventError: If SHEET_ROW_HEIGHT_SETTING event is canceled.
 
         Returns:
             XCellRange: Row cell range that height is applied on
@@ -7054,31 +7064,38 @@
         :events:
             .. cssclass:: lo_event
 
                 - :py:attr:`~.events.calc_named_event.CalcNamedEvent.SHEET_ROW_HEIGHT_SETTING` :eventref:`src-docs-sheet-event-row-height-setting`
                 - :py:attr:`~.events.calc_named_event.CalcNamedEvent.SHEET_ROW_HEIGHT_SET` :eventref:`src-docs-sheet-event-row-height-set`
 
         Note:
-            Event args ``index`` is set to ``idx`` value, ``event_data`` is set to ``height`` value.
+            Event args ``index`` is set to ``idx`` value, ``event_data`` is set to ``height`` value (``mm100`` units).
+
+        .. versionchanged:: 0.9.4
+            width can now also be ``UnitObj``
         """
+        try:
+            row_height = height.get_value_mm100()
+        except AttributeError:
+            row_height = UnitConvert.convert_mm_mm100(height)
         cargs = SheetCancelArgs(Calc.set_row_height.__qualname__)
         cargs.sheet = sheet
         cargs.index = idx
-        cargs.event_data = height
+        cargs.event_data = row_height
         _Events().trigger(CalcNamedEvent.SHEET_ROW_HEIGHT_SETTING, cargs)
         if cargs.cancel:
             raise mEx.CancelEventError(cargs)
         idx = cargs.index
-        height = cargs.event_data
-        if height <= 0:
+        row_height = cargs.event_data
+        if row_height <= 0:
             mLo.Lo.print("Height must be greater then 0")
             return None
         cell_range = cls.get_row_range(sheet=cargs.sheet, idx=idx)
         # mInfo.Info.show_services(obj_name="Cell range for a row", obj=cell_range)
-        mProps.Props.set(cell_range, Height=(height * 100))
+        mProps.Props.set(cell_range, Height=row_height)
         _Events().trigger(CalcNamedEvent.SHEET_ROW_HEIGHT_SET, SheetArgs.from_args(cargs))
         return cell_range
 
     # endregion ------------ cell decoration ---------------------------
 
     # region --------------- scenarios ---------------------------------
 
@@ -7814,54 +7831,54 @@
 
     # endregion --------------- headers /footers -----------------------
 
     # region --------------- styles ------------------------------------
     # region set_style_range()
     @overload
     @classmethod
-    def set_style_range(cls, sheet: XSpreadsheet, range_name: str, *, styles: Iterable[StyleObj]) -> XCellRange:
+    def set_style_range(cls, sheet: XSpreadsheet, range_name: str, *, styles: Sequence[StyleObj]) -> XCellRange:
         ...
 
     @overload
     @classmethod
     def set_style_range(
-        cls, sheet: XSpreadsheet, range_obj: mRngObj.RangeObj, *, styles: Iterable[StyleObj]
+        cls, sheet: XSpreadsheet, range_obj: mRngObj.RangeObj, *, styles: Sequence[StyleObj]
     ) -> XCellRange:
         ...
 
     @overload
     @classmethod
     def set_style_range(
-        cls, sheet: XSpreadsheet, cell_obj: mCellObj.CellObj, *, styles: Iterable[StyleObj]
+        cls, sheet: XSpreadsheet, cell_obj: mCellObj.CellObj, *, styles: Sequence[StyleObj]
     ) -> XCellRange:
         ...
 
     @overload
     @classmethod
     def set_style_range(
-        cls, sheet: XSpreadsheet, cr_addr: CellRangeAddress, *, styles: Iterable[StyleObj]
+        cls, sheet: XSpreadsheet, cr_addr: CellRangeAddress, *, styles: Sequence[StyleObj]
     ) -> XCellRange:
         ...
 
     @overload
     @classmethod
-    def set_style_range(cls, cell_range: XCellRange, *, styles: Iterable[StyleObj]) -> XCellRange:
+    def set_style_range(cls, cell_range: XCellRange, *, styles: Sequence[StyleObj]) -> XCellRange:
         ...
 
     @overload
     @classmethod
     def set_style_range(
         cls,
         sheet: XSpreadsheet,
         col_start: int,
         row_start: int,
         col_end: int,
         row_end: int,
         *,
-        styles: Iterable[StyleObj],
+        styles: Sequence[StyleObj],
     ) -> XCellRange:
         ...
 
     @classmethod
     def set_style_range(cls, *args, **kwargs) -> None:
         """
         Set style/formatting on cell range
@@ -7873,22 +7890,22 @@
             cell_obj (CellObj): Cell Object
             cr_addr (CellRangeAddress): Cell range Address
             cell_range (XCellRange): Cell Range. If passed in then the same instance is returned.
             col_start (int): Start Column
             row_start (int): Start Row
             col_end (int): End Column
             row_end (int): End Row
-            styles (Iterable[StyleObj], optional): One or more styles to apply to cell range.
+            styles (Sequence[StyleObj], optional): One or more styles to apply to cell range.
 
         Returns:
             None:
 
         .. versionadded:: 0.9.2
         """
-        styles = cast(Iterable[StyleObj], kwargs.pop("styles", None))
+        styles = cast(Sequence[StyleObj], kwargs.pop("styles", None))
         if styles is None:
             return
         cell_range = cls.get_cell_range(*args, **kwargs)
         supported_styles = (
             "com.sun.star.style.CharacterProperties",
             "com.sun.star.style.ParagraphProperties",
             "com.sun.star.table.CellProperties",
@@ -7901,40 +7918,40 @@
                 style.apply(cell_range)
 
     # endregion set_style_range()
 
     # region set_style_cell()
     @overload
     @classmethod
-    def set_style_cell(cls, sheet: XSpreadsheet, addr: CellAddress, *, styles: Iterable[StyleObj]) -> XCell:
+    def set_style_cell(cls, sheet: XSpreadsheet, addr: CellAddress, *, styles: Sequence[StyleObj]) -> XCell:
         ...
 
     @overload
     @classmethod
-    def set_style_cell(cls, sheet: XSpreadsheet, cell_name: str, *, styles: Iterable[StyleObj]) -> XCell:
+    def set_style_cell(cls, sheet: XSpreadsheet, cell_name: str, *, styles: Sequence[StyleObj]) -> XCell:
         ...
 
     @overload
     @classmethod
-    def set_style_cell(cls, sheet: XSpreadsheet, cell_obj: mCellObj.CellObj, *, styles: Iterable[StyleObj]) -> XCell:
+    def set_style_cell(cls, sheet: XSpreadsheet, cell_obj: mCellObj.CellObj, *, styles: Sequence[StyleObj]) -> XCell:
         ...
 
     @overload
     @classmethod
-    def set_style_cell(cls, sheet: XSpreadsheet, col: int, row: int, *, styles: Iterable[StyleObj]) -> XCell:
+    def set_style_cell(cls, sheet: XSpreadsheet, col: int, row: int, *, styles: Sequence[StyleObj]) -> XCell:
         ...
 
     @overload
     @classmethod
-    def set_style_cell(cls, cell_range: XCellRange, *, styles: Iterable[StyleObj]) -> XCell:
+    def set_style_cell(cls, cell_range: XCellRange, *, styles: Sequence[StyleObj]) -> XCell:
         ...
 
     @overload
     @classmethod
-    def set_style_cell(cls, cell_range: XCellRange, col: int, row: int, *, styles: Iterable[StyleObj]) -> XCell:
+    def set_style_cell(cls, cell_range: XCellRange, col: int, row: int, *, styles: Sequence[StyleObj]) -> XCell:
         ...
 
     @classmethod
     def set_style_cell(cls, *args, **kwargs) -> None:
         """
         Set style/formatting on cell
 
@@ -7942,22 +7959,22 @@
             sheet (XSpreadsheet): Spreadsheet
             addr (CellAddress): Cell Address
             cell_name (str): Cell Name such as 'A1'
             cell_obj: (CellObj): Cell object
             cell_range (XCellRange): Cell Range
             col (int): Cell column
             row (int): cell row
-            styles (Iterable[StyleObj], optional): One or more styles to apply to cell range.
+            styles (Sequence[StyleObj], optional): One or more styles to apply to cell range.
 
         Returns:
             None:
 
         .. versionadded:: 0.9.2
         """
-        styles = cast(Iterable[StyleObj], kwargs.pop("styles", None))
+        styles = cast(Sequence[StyleObj], kwargs.pop("styles", None))
         if styles is None:
             return
         cell = cls.get_cell(*args, **kwargs)
         supported_styles = (
             "com.sun.star.style.CharacterProperties",
             "com.sun.star.style.ParagraphProperties",
             "com.sun.star.table.CellProperties",
@@ -7967,7 +7984,19 @@
 
         for style in styles:
             if style.support_service(*supported_styles):
                 style.apply(cell)
 
     # endregion set_style_cell()
     # endregion ------------ styles ------------------------------------
+
+    # region --------------- dispatch ----------------------------------
+    @staticmethod
+    def dispatch_recalculate() -> None:
+        """
+        Dispatches recalculate command to the current sheet.
+
+        .. versionadded:: 0.9.4
+        """
+        mLo.Lo.dispatch_cmd("Calculate")
+
+    # endregion ------------ dispatch ----------------------------------
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/office/chart.py` & `ooo_dev_tools-0.9.4/ooodev/office/chart.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/office/chart2.py` & `ooo_dev_tools-0.9.4/ooodev/office/chart2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # region Imports
 from __future__ import annotations
 from random import random
-from typing import List, Tuple, cast, overload, TYPE_CHECKING
+from typing import List, Sequence, Tuple, cast, overload, TYPE_CHECKING
 
 import uno
 
-# XChartTypeTemplate import error in LO 7.4.0 to 7.4.3
+# XChartTypeTemplate import error in LO 7.4.0 to 7.4.3, Corrected in Lo 7.5
 from com.sun.star.beans import XPropertySet
 from com.sun.star.chart2 import XAxis
 from com.sun.star.chart2 import XChartDocument
 from com.sun.star.chart2 import XChartType
 from com.sun.star.chart2 import XChartTypeContainer
 from com.sun.star.chart2 import XChartTypeTemplate
 from com.sun.star.chart2 import XCoordinateSystem
@@ -40,16 +40,21 @@
 from com.sun.star.lang import XMultiServiceFactory
 from com.sun.star.sheet import XSpreadsheet
 from com.sun.star.sheet import XSpreadsheetDocument
 from com.sun.star.table import XTableChart
 from com.sun.star.table import XTableChartsSupplier
 from com.sun.star.util import XNumberFormatsSupplier
 
+from ooodev.events.event_singleton import _Events
+
 
 from . import calc as mCalc
+from ..events.args.cancel_event_args import CancelEventArgs
+from ..events.args.event_args import EventArgs
+from ..events.chart2_named_event import Chart2NamedEvent
 from ..exceptions import ex as mEx
 from ..proto.style_obj import StyleObj
 from ..utils import color as mColor
 from ..utils import file_io as mFileIo
 from ..utils import gui as mGui
 from ..utils import images_lo as mImgLo
 from ..utils import info as mInfo
@@ -65,25 +70,27 @@
 
 from ooo.dyn.awt.rectangle import Rectangle
 from ooo.dyn.chart.chart_data_row_source import ChartDataRowSource
 from ooo.dyn.chart.error_bar_style import ErrorBarStyle
 from ooo.dyn.chart2.axis_orientation import AxisOrientation
 from ooo.dyn.chart2.axis_type import AxisTypeEnum as AxisTypeKind
 from ooo.dyn.chart2.data_point_geometry3_d import DataPointGeometry3DEnum as DataPointGeometry3DEnum
-from ooo.dyn.chart2.data_point_label import DataPointLabel
 from ooo.dyn.drawing.fill_style import FillStyle as FillStyle
 from ooo.dyn.drawing.line_style import LineStyle as LineStyle
 from ooo.dyn.lang.locale import Locale
 from ooo.dyn.table.cell_range_address import CellRangeAddress
 
 if TYPE_CHECKING:
     from ooo.lo.chart2.data_point_properties import DataPointProperties
-
+    from com.sun.star.drawing import OLE2Shape
+    from com.sun.star.chart2 import DataPointLabel
 # endregion Imports
 
+# https://wiki.documentfoundation.org/Documentation/DevGuide/Charts
+
 
 class Chart2:
     """Chart 2 Class"""
 
     _CHART_NAME = "chart$$_"
 
     # region insert/remove a chart
@@ -125,14 +132,17 @@
         Returns:
             XChartDocument: Chart Document that was created and inserted
 
         Note:
             **Keyword Arguments** are to mostly be ignored.
             If finer control over chart creation is needed then **Keyword Arguments** can be used.
 
+        Note:
+            See **Open Office Wiki** - `The Structure of Charts <https://wiki.openoffice.org/wiki/Documentation/BASIC_Guide/Structure_of_Charts>`__ for more information.
+
         See Also:
             :py:class:`~.color.CommonColor`
 
         Hint:
             .. include:: ../../resources/utils/chart2_lookup_chart_tmpl.rst
 
         .. versionchanged:: 0.8.1
@@ -462,72 +472,93 @@
         except Exception as e:
             raise mEx.ChartError("Error getting chart templates") from e
 
     # endregion get a chart
 
     # region titles
     @classmethod
-    def set_title(cls, chart_doc: XChartDocument, title: str) -> XTitle:
+    def set_title(cls, chart_doc: XChartDocument, title: str, styles: Sequence[StyleObj] = None) -> XTitle:
         """
         Sets the title of chart
 
         Args:
             chart_doc (XChartDocument): Chart Document.
-            title (str): Title as string
+            title (str): Title as string.
+            styles (Sequence[StyleObj], optional): Styles to apply to title.
 
         Raises:
             ChartError: If error occurs.
 
         Returns:
             XTitle: Title Object
 
         Note:
-            The title is set to a font size of ``14`` and the font applied is
-            the font returned by :py:meth:`.Info.get_font_general_name`
+            The title has a default font size of ``14`` and the font name applied is
+            the font returned by :py:meth:`.Info.get_font_general_name`.
 
         Hint:
-            The returned Title object can be passed to :py:meth:`~.Chart2.set_x_title_font` to
-            change default font.
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>` subpackages.
         """
         try:
             # return XTilte so it may have futher styles applied
             titled = mLo.Lo.qi(XTitled, chart_doc, True)
-            xtitle = cls.create_title(title)
+            xtitle = cls._create_title(title, 14, styles)
             titled.setTitleObject(xtitle)
-            fname = mInfo.Info.get_font_general_name()
-            cls.set_x_title_font(xtitle, fname, 14)
+
             return xtitle
         except Exception as e:
             raise mEx.ChartError("Error setting title for chart") from e
 
-    @staticmethod
-    def create_title(title: str) -> XTitle:
+    @classmethod
+    def _create_title(cls, title: str, font_size: int, styles: Sequence[StyleObj] = None) -> XTitle:
+        try:
+            xtitle = mLo.Lo.create_instance_mcf(XTitle, "com.sun.star.chart2.Title", raise_err=True)
+            xtitle_str = mLo.Lo.create_instance_mcf(
+                XFormattedString, "com.sun.star.chart2.FormattedString", raise_err=True
+            )
+            xtitle_str.setString(title)
+
+            # set default font. Styles can override the default.
+            fname = mInfo.Info.get_font_general_name()
+            cls.set_x_title_font(xtitle, fname, font_size)
+
+            title_arr = (xtitle_str,)
+            xtitle.setText(title_arr)
+            # Shape style will not be applied. Need to use style_title() after title is created.
+            if styles:
+                title_styles = [style for style in styles if not style.support_service("com.sun.star.drawing.Shape")]
+                cls._style_title(xtitle=xtitle, styles=title_styles)
+
+            return xtitle
+        except Exception as e:
+            raise mEx.ChartError(f'Error creating title for: "{title}"') from e
+
+    @classmethod
+    def create_title(cls, title: str, styles: Sequence[StyleObj] = None) -> XTitle:
         """
         Creates a title object
 
         Args:
             title (str): Title text.
+            styles (Sequence[StyleObj], optional): Styles to apply to title.
 
         Raises:
             ChartError: If error occurs.
 
         Returns:
             XTitle: Title object.
+
+        Note:
+            The title has a default font size of ``14`` and the font name applied is
+            the font returned by :py:meth:`.Info.get_font_general_name`.
+
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>` subpackages.
         """
-        try:
-            xtitle = mLo.Lo.create_instance_mcf(XTitle, "com.sun.star.chart2.Title", raise_err=True)
-            xtitle_str = mLo.Lo.create_instance_mcf(
-                XFormattedString, "com.sun.star.chart2.FormattedString", raise_err=True
-            )
-            xtitle_str.setString(title)
-            title_arr = (xtitle_str,)
-            xtitle.setText(title_arr)
-            return xtitle
-        except Exception as e:
-            raise mEx.ChartError(f'Error creating title for: "{title}"') from e
+        return cls._create_title(title, 14, styles)
 
     @staticmethod
     def set_x_title_font(xtitle: XTitle, font_name: str, pt_size: int) -> None:
         """
         Sets X title font.
 
         Args:
@@ -569,43 +600,41 @@
         try:
             xtilted = mLo.Lo.qi(XTitled, chart_doc, True)
             return xtilted.getTitleObject()
         except Exception as e:
             raise mEx.ChartError("Error getting title from chart") from e
 
     @classmethod
-    def set_subtitle(cls, chart_doc: XChartDocument, subtitle: str) -> XTitle:
+    def set_subtitle(cls, chart_doc: XChartDocument, subtitle: str, styles: Sequence[StyleObj] = None) -> XTitle:
         """
         Gets subtitle
 
         Args:
             chart_doc (XChartDocument): Chart Document.
             subtitle (str): Subtitle text.
+            styles (Sequence[StyleObj], optional): Styles to apply to subtitle.
 
         Raises:
             ChartError: If error occurs
 
         Returns:
             XTitle: Title object
 
         Note:
             The subtitle is set to a font size of ``12`` and the font applied is
             the font returned by :py:meth:`.Info.get_font_general_name`
 
         Hint:
-            The returned Title object can be passed to :py:meth:`~.Chart2.set_x_title_font` to
-            change default font.
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>` subpackages.
         """
         try:
             diagram = chart_doc.getFirstDiagram()
             titled = mLo.Lo.qi(XTitled, diagram, True)
-            title = cls.create_title(subtitle)
+            title = cls._create_title(title=subtitle, font_size=12, styles=styles)
             titled.setTitleObject(title)
-            fname = mInfo.Info.get_font_general_name()
-            cls.set_x_title_font(title, fname, 12)
             return title
         except mEx.ChartError:
             raise
         except Exception as e:
             raise mEx.ChartError(f'Error setting subtitle "{subtitle}" for chart') from e
 
     @staticmethod
@@ -732,121 +761,139 @@
 
         See Also:
             :py:meth:`~.Chart2.get_axis`
         """
         return cls.get_axis(chart_doc=chart_doc, axis_val=AxisKind.Y, idx=1)
 
     @classmethod
-    def set_axis_title(cls, chart_doc: XChartDocument, title: str, axis_val: AxisKind, idx: int) -> XTitle:
+    def set_axis_title(
+        cls, chart_doc: XChartDocument, title: str, axis_val: AxisKind, idx: int, styles: Sequence[StyleObj] = None
+    ) -> XTitle:
         """
         Sets axis title.
 
         Args:
             chart_doc (XChartDocument): Chart Document.
             title (str): Title text.
             axis_val (AxisKind): Axis kind.
             idx (int): Index
+            styles (Sequence[StyleObj], optional): Styles to apply to title.
 
         Raises:
             ChartError: If error occurs.
 
         Returns:
             XTitle: Axis Title.
 
         Note:
             The title is set to a font size of ``12`` and the font applied is
             the font returned by :py:meth:`.Info.get_font_general_name`
 
         Hint:
-            The returned Title object can be passed to :py:meth:`~.Chart2.set_x_title_font` to
-            change default font.
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>` subpackages.
 
         See Also:
             :py:meth:`~.Chart2.get_axis`
         """
         try:
             axis = cls.get_axis(chart_doc=chart_doc, axis_val=axis_val, idx=idx)
             titled_axis = mLo.Lo.qi(XTitled, axis, True)
-            xtitle = cls.create_title(title)
+            xtitle = cls._create_title(title=title, font_size=12, styles=styles)
             titled_axis.setTitleObject(xtitle)
             fname = mInfo.Info.get_font_general_name()
             cls.set_x_title_font(xtitle, fname, 12)
             return xtitle
         except mEx.ChartError:
             raise
         except Exception as e:
             raise mEx.ChartError(f'Error setting axis tile: "{title}" for chart') from e
 
     @classmethod
-    def set_x_axis_title(cls, chart_doc: XChartDocument, title: str) -> XTitle:
+    def set_x_axis_title(cls, chart_doc: XChartDocument, title: str, styles: Sequence[StyleObj] = None) -> XTitle:
         """
         Sets X axis Title
 
         Args:
             chart_doc (XChartDocument): Chart Document.
-            title (str): Title Text
+            title (str): Title Text.
+            styles (Sequence[StyleObj], optional): Styles to apply to title.
 
         Returns:
             XTitle: Title object
 
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>` subpackages.
+
         See Also:
             :py:meth:`~.Chart2.set_axis_title`
         """
-        return cls.set_axis_title(chart_doc=chart_doc, title=title, axis_val=AxisKind.X, idx=0)
+        return cls.set_axis_title(chart_doc=chart_doc, title=title, axis_val=AxisKind.X, idx=0, styles=styles)
 
     @classmethod
-    def set_y_axis_title(cls, chart_doc: XChartDocument, title: str) -> XTitle:
+    def set_y_axis_title(cls, chart_doc: XChartDocument, title: str, styles: Sequence[StyleObj] = None) -> XTitle:
         """
         Sets Y axis Title
 
         Args:
             chart_doc (XChartDocument): Chart Document.
-            title (str): Title Text
+            title (str): Title Text.
+            styles (Sequence[StyleObj], optional): Styles to apply to title.
 
         Returns:
             XTitle: Title object
 
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>` subpackages.
+
         See Also:
             :py:meth:`~.Chart2.set_axis_title`
         """
-        return cls.set_axis_title(chart_doc=chart_doc, title=title, axis_val=AxisKind.Y, idx=0)
+        return cls.set_axis_title(chart_doc=chart_doc, title=title, axis_val=AxisKind.Y, idx=0, styles=styles)
 
     @classmethod
-    def set_x_axis2_title(cls, chart_doc: XChartDocument, title: str) -> XTitle:
+    def set_x_axis2_title(cls, chart_doc: XChartDocument, title: str, styles: Sequence[StyleObj] = None) -> XTitle:
         """
         Sets X axis2 Title
 
         Args:
             chart_doc (XChartDocument): Chart Document.
-            title (str): Title Text
+            title (str): Title Text.
+            styles (Sequence[StyleObj], optional): Styles to apply to title.
 
         Returns:
             XTitle: Title object
 
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>` subpackages.
+
         See Also:
             :py:meth:`~.Chart2.set_axis_title`
         """
-        return cls.set_axis_title(chart_doc=chart_doc, title=title, axis_val=AxisKind.X, idx=1)
+        return cls.set_axis_title(chart_doc=chart_doc, title=title, axis_val=AxisKind.X, idx=1, styles=styles)
 
     @classmethod
-    def set_y_axis2_title(cls, chart_doc: XChartDocument, title: str) -> XTitle:
+    def set_y_axis2_title(cls, chart_doc: XChartDocument, title: str, styles: Sequence[StyleObj] = None) -> XTitle:
         """
         Sets Y axis2 Title
 
         Args:
             chart_doc (XChartDocument): Chart Document.
-            title (str): Title Text
+            title (str): Title Text.
+            styles (Sequence[StyleObj], optional): Styles to apply to title.
 
         Returns:
             XTitle: Title object
 
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>` subpackages.
+
         See Also:
             :py:meth:`~.Chart2.set_axis_title`
         """
-        return cls.set_axis_title(chart_doc=chart_doc, title=title, axis_val=AxisKind.Y, idx=1)
+        return cls.set_axis_title(chart_doc=chart_doc, title=title, axis_val=AxisKind.Y, idx=1, styles=styles)
 
     @classmethod
     def get_axis_title(cls, chart_doc: XChartDocument, axis_val: AxisKind, idx: int) -> XTitle:
         """
         Gets axis Title
 
         Args:
@@ -948,106 +995,107 @@
 
         See Also:
             :py:meth:`~.Chart2.get_axis_title`
         """
         return cls.get_axis_title(chart_doc=chart_doc, axis_val=AxisKind.Y, idx=1)
 
     @classmethod
-    def rotate_axis_title(cls, chart_doc: XChartDocument, axis_val: AxisKind, idx: int, angle: Angle) -> None:
+    def rotate_axis_title(cls, chart_doc: XChartDocument, axis_val: AxisKind, idx: int, angle: Angle | int) -> None:
         """
         Rotates axis title.
 
         Args:
             chart_doc (XChartDocument): Chart Document.
             axis_val (AxisKind): Axis kind.
             idx (int): Index
-            angle (Angle): Angle
+            angle (Angle, int): Angle
 
         Raises:
             ChartError: If error occurs.
 
         Returns:
             None:
         """
         try:
+            rotation = Angle(int(angle))
             xtitle = cls.get_axis_title(chart_doc=chart_doc, axis_val=axis_val, idx=idx)
-            mProps.Props.set(xtitle, TextRotation=angle.value)
+            mProps.Props.set(xtitle, TextRotation=rotation.value)
         except mEx.ChartError:
             raise
         except Exception as e:
             raise mEx.ChartError("Error while trying to rotate axis title") from e
 
     @classmethod
-    def rotate_x_axis_title(cls, chart_doc: XChartDocument, angle: Angle) -> None:
+    def rotate_x_axis_title(cls, chart_doc: XChartDocument, angle: Angle | int) -> None:
         """
         Rotates X axis title.
 
         Args:
             chart_doc (XChartDocument): Chart Document.
-            angle (Angle): Angle
+            angle (Angle, int): Angle
 
         Raises:
             ChartError: If error occurs.
 
         Returns:
             None:
 
         See Also:
             :py:meth:`~.Chart2.rotate_axis_title`
         """
         cls.rotate_axis_title(chart_doc=chart_doc, axis_val=AxisKind.X, idx=0, angle=angle)
 
     @classmethod
-    def rotate_y_axis_title(cls, chart_doc: XChartDocument, angle: Angle) -> None:
+    def rotate_y_axis_title(cls, chart_doc: XChartDocument, angle: Angle | int) -> None:
         """
         Rotates Y axis title.
 
         Args:
             chart_doc (XChartDocument): Chart Document.
-            angle (Angle): Angle
+            angle (Angle, int): Angle
 
         Raises:
             ChartError: If error occurs.
 
         Returns:
             None:
 
         See Also:
             :py:meth:`~.Chart2.rotate_axis_title`
         """
         cls.rotate_axis_title(chart_doc=chart_doc, axis_val=AxisKind.Y, idx=0, angle=angle)
 
     @classmethod
-    def rotate_x_axis2_title(cls, chart_doc: XChartDocument, angle: Angle) -> None:
+    def rotate_x_axis2_title(cls, chart_doc: XChartDocument, angle: Angle | int) -> None:
         """
         Rotates X axis2 title.
 
         Args:
             chart_doc (XChartDocument): Chart Document.
-            angle (Angle): Angle
+            angle (Angle, int): Angle
 
         Raises:
             ChartError: If error occurs.
 
         Returns:
             None:
 
         See Also:
             :py:meth:`~.Chart2.rotate_axis_title`
         """
         cls.rotate_axis_title(chart_doc=chart_doc, axis_val=AxisKind.X, idx=1, angle=angle)
 
     @classmethod
-    def rotate_y_axis2_title(cls, chart_doc: XChartDocument, angle: Angle) -> None:
+    def rotate_y_axis2_title(cls, chart_doc: XChartDocument, angle: Angle | int) -> None:
         """
         Rotates Y axis2 title.
 
         Args:
             chart_doc (XChartDocument): Chart Document.
-            angle (Angle): Angle
+            angle (Angle, int): Angle
 
         Raises:
             ChartError: If error occurs.
 
         Returns:
             None:
 
@@ -1313,38 +1361,61 @@
     @overload
     @classmethod
     def set_grid_lines(cls, chart_doc: XChartDocument, axis_val: AxisKind) -> XPropertySet:
         ...
 
     @overload
     @classmethod
+    def set_grid_lines(
+        cls, chart_doc: XChartDocument, axis_val: AxisKind, *, styles: Sequence[StyleObj]
+    ) -> XPropertySet:
+        ...
+
+    @overload
+    @classmethod
     def set_grid_lines(cls, chart_doc: XChartDocument, axis_val: AxisKind, idx: int) -> XPropertySet:
         ...
 
+    @overload
     @classmethod
-    def set_grid_lines(cls, chart_doc: XChartDocument, axis_val: AxisKind, idx: int = 0) -> XPropertySet:
+    def set_grid_lines(
+        cls, chart_doc: XChartDocument, axis_val: AxisKind, idx: int, styles: Sequence[StyleObj]
+    ) -> XPropertySet:
+        ...
+
+    @classmethod
+    def set_grid_lines(
+        cls, chart_doc: XChartDocument, axis_val: AxisKind, idx: int = 0, styles: Sequence[StyleObj] = None
+    ) -> XPropertySet:
         """
         Set the grid lines for a chart.
 
         Args:
             chart_doc (XChartDocument): Chart Document.
             axis_val (AxisKind): Axis kind.
-            idx (int, optional): Index. Defaults to 0.
+            idx (int, optional): Index. Defaults to ``0``.
+            styles (Sequence[StyleObj], optional): Styles to apply.
 
         Raises:
             ChartError: If error occurs.
 
         Returns:
             XPropertySet: Property Set of Grid Properties.
+
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.grid </src/format/ooodev.format.chart2.direct.grid>`.
         """
         try:
             axis = cls.get_axis(chart_doc=chart_doc, axis_val=axis_val, idx=idx)
             props = axis.getGridProperties()
             mProps.Props.set_property(props, "LineStyle", LineStyle.DASH)
             mProps.Props.set_property(props, "LineDashName", str(LineStyleNameKind.FINE_DOTTED))
+            if styles:
+                for style in styles:
+                    style.apply(props)
             return props
         except mEx.ChartError:
             raise
         except Exception as e:
             raise mEx.ChartError("Error setting gird lines for chart") from e
 
     # endregion set_grid_lines()
@@ -1375,77 +1446,530 @@
                 mProps.Props.set(leg, LineStyle=LineStyle.NONE, FillStyle=FillStyle.SOLID, FillTransparence=100)
                 diagram.setLegend(leg)
 
             mProps.Props.set(leg, Show=is_visible)
         except Exception as e:
             raise mEx.ChartError("Error while setting legend visibility") from e
 
+    @staticmethod
+    def get_legend(chart_doc: XChartDocument) -> XLegend | None:
+        """
+        Gets chart legend.
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+
+        Raises:
+            ChartError: If error occurs.
+
+        Returns:
+            XLegend: Legend object or ``None`` if no legend exists.
+
+        .. versionadded:: 0.9.4
+        """
+        try:
+            diagram = chart_doc.getFirstDiagram()
+            return diagram.getLegend()
+        except Exception as e:
+            raise mEx.ChartError("Error while getting legend") from e
+
     # endregion legend
 
     # region Styles
+    @classmethod
+    def style_grid(
+        cls, chart_doc: XChartDocument, axis_val: AxisKind, styles: Sequence[StyleObj], idx: int = 0
+    ) -> None:
+        """
+        Style Grid
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+            axis_val (AxisKind): Axis kind.
+            styles (Sequence[StyleObj]): Styles to apply.
+            idx (int, optional): Index. Defaults to ``0``.
+
+        Returns:
+            None:
+
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.grid </src/format/ooodev.format.chart2.direct.grid>`.
+        """
+        try:
+            axis = cls.get_axis(chart_doc=chart_doc, axis_val=axis_val, idx=idx)
+            props = axis.getGridProperties()
+
+            if props is None:
+                return
+
+            for style in styles:
+                style.apply(props)
+        except Exception as e:
+            pass
 
     @staticmethod
-    def style_background(chart_doc: XChartDocument, *styles: StyleObj) -> None:
+    def style_background(chart_doc: XChartDocument, styles: Sequence[StyleObj]) -> None:
         """
         Styles background of chart
 
         Args:
             chart_doc (XChartDocument): Chart Document.
-            styles: Expandable list of styles to apply to chart background
+            styles (Sequence[StyleObj]): One or more styles to apply chart background.
 
         Returns:
             None:
 
+        Hint:
+            Styles that can be applied are found in the following:
+
+                - :doc:`ooodev.format.chart2.direct.general.area </src/format/ooodev.format.chart2.direct.general.area>`
+                - :doc:`ooodev.format.chart2.direct.general.borders </src/format/ooodev.format.chart2.direct.general.borders>`
+                - :doc:`ooodev.format.chart2.direct.general.transparency </src/format/ooodev.format.chart2.direct.general.transparency>`
+
         .. versionadded:: 0.9.0
         """
         bg_ps = chart_doc.getPageBackground()
         for style in styles:
             style.apply(bg_ps)
 
     @staticmethod
-    def style_wall(chart_doc: XChartDocument, *styles: StyleObj) -> None:
+    def style_wall(chart_doc: XChartDocument, styles: Sequence[StyleObj]) -> None:
         """
         Styles Wall of chart
 
         Args:
             chart_doc (XChartDocument): Chart Document.
-            styles: Expandable list of styles to apply to chart background
+            styles (Sequence[StyleObj]): One or more styles to apply chart wall.
 
         Returns:
             None:
 
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.wall </src/format/ooodev.format.chart2.direct.wall>` subpackages.
+
         .. versionadded:: 0.9.0
         """
         wall = chart_doc.getFirstDiagram().getWall()
-        for style in styles:
-            style.apply(wall)
+        if wall:
+            for style in styles:
+                style.apply(wall)
 
     @staticmethod
-    def style_data_point(chart_doc: XChartDocument, series_idx: int, idx: int, *styles: StyleObj) -> None:
+    def style_floor(chart_doc: XChartDocument, styles: Sequence[StyleObj]) -> None:
+        """
+        Styles Floor of 3D chart.
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+            styles (Sequence[StyleObj]): One or more styles to apply chart floor.
+
+        Returns:
+            None:
+
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.wall </src/format/ooodev.format.chart2.direct.wall>` subpackages.
+
+        .. versionadded:: 0.9.4
+        """
+        floor = chart_doc.getFirstDiagram().getFloor()
+        if floor:
+            for style in styles:
+                style.apply(floor)
+
+    @classmethod
+    def style_data_point(
+        cls, chart_doc: XChartDocument, series_idx: int, idx: int, styles: Sequence[StyleObj]
+    ) -> None:
         """
         Styles a data point of chart
 
         Args:
             chart_doc (XChartDocument): Chart Document.
             series_idx (int): Series Index.
             idx (int): Index to extract from the datapoints data.
                 If ``idx=-1`` then the last data point is styled.
-            styles: Expandable list of styles to apply to chart background
+            styles (Sequence[StyleObj]): One or more styles to apply chart data point.
 
         Returns:
             None:
 
+        Hint:
+            Styles that can be applied are found in the following packages.
+
+                - :doc:`ooodev.format.chart2.direct.series.data_series </src/format/ooodev.format.chart2.direct.series.data_series>`
+                - :doc:`ooodev.format.chart2.direct.series.data_labels </src/format/ooodev.format.chart2.direct.series.data_labels>`
+
         .. versionadded:: 0.9.0
         """
 
-        pp = Chart2.get_data_point_props(chart_doc=chart_doc, series_idx=series_idx, idx=idx)
+        pp = cls.get_data_point_props(chart_doc=chart_doc, series_idx=series_idx, idx=idx)
 
         for style in styles:
             style.apply(pp)
 
+    @classmethod
+    def style_data_series(cls, chart_doc: XChartDocument, styles: Sequence[StyleObj], idx: int = -1) -> None:
+        """
+        Styles one or more data series of chart.
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+            styles (Sequence[StyleObj]): One or more styles to apply chart data series.
+            idx (int, optional): Zero based series index. If value is ``-1`` then styles all data series are styled,
+                Otherwise only data series specified by index is styled. Defaults to ``-1``.
+
+        Returns:
+            None:
+
+        Hint:
+            Styles that can be applied are found in the following packages.
+
+                - :doc:`ooodev.format.chart2.direct.series.data_series </src/format/ooodev.format.chart2.direct.series.data_series>`
+                - :doc:`ooodev.format.chart2.direct.series.data_labels </src/format/ooodev.format.chart2.direct.series.data_labels>`
+
+        .. versionadded:: 0.9.4
+        """
+        if idx < 0:
+            idx = -1
+
+        series = cls.get_data_series(chart_doc=chart_doc)
+        if idx == -1:
+            for itm in series:
+                for style in styles:
+                    style.apply(itm)
+        else:
+            if idx < 0 or idx >= len(series):
+                raise IndexError(f"Index value of {idx} is out of of range")
+            itm = series[idx]
+            for style in styles:
+                style.apply(itm)
+
+    @classmethod
+    def style_legend(cls, chart_doc: XChartDocument, styles: Sequence[StyleObj]) -> None:
+        """
+        Styles legend of chart.
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+            styles (Sequence[StyleObj]): One or more styles to apply chart legend.
+
+        Returns:
+            None:
+
+        Hint:
+            Styles that can be applied are found in the following packages.
+
+                - :doc:`ooodev.format.chart2.direct.legend </src/format/ooodev.format.chart2.direct.legend>`
+                - :doc:`ooodev.format.chart2.direct.general.position_size </src/format/ooodev.format.chart2.direct.general.position_size>`
+
+        .. versionadded:: 0.9.0
+        """
+        applied_styles = 0
+        legend_shape = None
+        for style in styles:
+            if style.support_service("com.sun.star.drawing.Shape"):
+                legend_shape = chart_doc.getLegend()
+                break
+        if legend_shape:
+            for style in styles:
+                if style.support_service("com.sun.star.drawing.Shape"):
+                    style.apply(legend_shape)
+                    applied_styles += 1
+        if len(styles) == applied_styles:
+            return
+        legend = cls.get_legend(chart_doc=chart_doc)
+        if legend:
+            for style in styles:
+                if not style.support_service("com.sun.star.drawing.Shape"):
+                    style.apply(legend)
+
+    @classmethod
+    def _style_title(cls, xtitle: XTitle, styles: Sequence[StyleObj]) -> None:
+        title_styles = [style for style in styles if not style.support_service("com.sun.star.drawing.Shape")]
+        applied_styles = 0
+        if title_styles:
+            for style in title_styles:
+                if style.support_service("com.sun.star.chart2.Title"):
+                    style.apply(xtitle)
+                    applied_styles += 1
+            if len(title_styles) == applied_styles:
+                return
+            fo_strs = xtitle.getText()
+            if fo_strs:
+                fo_first = fo_strs[0]
+                for style in title_styles:
+                    if not style.support_service("com.sun.star.chart2.Title"):
+                        style.apply(fo_first)
+
+    @classmethod
+    def style_title(cls, chart_doc: XChartDocument, styles: Sequence[StyleObj]) -> None:
+        """
+        Styles title of chart.
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+            styles (Sequence[StyleObj]): One or more styles to apply chart title.
+
+        Returns:
+            None:
+
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>` subpackages.
+
+        .. versionadded:: 0.9.4
+        """
+        title_styles = [style for style in styles if not style.support_service("com.sun.star.drawing.Shape")]
+        shape_styles = [style for style in styles if style.support_service("com.sun.star.drawing.Shape")]
+        if shape_styles:
+            title_shape = chart_doc.getTitle()
+            if title_shape:
+                for style in shape_styles:
+                    style.apply(title_shape)
+
+        if title_styles:
+            xtitle = cls.get_title(chart_doc=chart_doc)
+            if xtitle is None:
+                return
+            cls._style_title(xtitle=xtitle, styles=title_styles)
+
+    @classmethod
+    def style_subtitle(cls, chart_doc: XChartDocument, styles: Sequence[StyleObj]) -> None:
+        """
+        Styles subtitle of chart.
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+            styles (Sequence[StyleObj]): One or more styles to apply chart subtitle.
+
+        Returns:
+            None:
+
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>` subpackages.
+
+        .. versionadded:: 0.9.4
+        """
+        title_styles = [style for style in styles if not style.support_service("com.sun.star.drawing.Shape")]
+        shape_styles = [style for style in styles if style.support_service("com.sun.star.drawing.Shape")]
+        if shape_styles:
+            subtitle_shape = chart_doc.getSubTitle()
+            if subtitle_shape:
+                for style in shape_styles:
+                    style.apply(subtitle_shape)
+
+        if title_styles:
+            xtitle = cls.get_subtitle(chart_doc=chart_doc)
+            if xtitle:
+                cls._style_title(xtitle=xtitle, styles=title_styles)
+
+    @classmethod
+    def style_x_axis(cls, chart_doc: XChartDocument, styles: Sequence[StyleObj]) -> None:
+        """
+        Styles X axis of chart.
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+            styles (Sequence[StyleObj]): One or more styles to apply chart X axis.
+
+        Returns:
+            None:
+
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.axis </src/format/ooodev.format.chart2.direct.axis>` subpackages.
+
+        .. versionadded:: 0.9.4
+        """
+        try:
+            axis = cls.get_x_axis(chart_doc=chart_doc)
+        except mEx.ChartError:
+            return
+
+        for style in styles:
+            style.apply(axis)
+
+    @classmethod
+    def style_x_axis2(cls, chart_doc: XChartDocument, styles: Sequence[StyleObj]) -> None:
+        """
+        Styles X axis2 of chart.
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+            styles (Sequence[StyleObj]): One or more styles to apply chart X axis2.
+
+        Returns:
+            None:
+
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.axis </src/format/ooodev.format.chart2.direct.axis>` subpackages.
+
+        .. versionadded:: 0.9.4
+        """
+        try:
+            axis = cls.get_x_axis2(chart_doc=chart_doc)
+        except mEx.ChartError:
+            return
+
+        for style in styles:
+            style.apply(axis)
+
+    @classmethod
+    def style_y_axis(cls, chart_doc: XChartDocument, styles: Sequence[StyleObj]) -> None:
+        """
+        Styles Y axis of chart.
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+            styles (Sequence[StyleObj]): One or more styles to apply chart Y axis.
+
+        Returns:
+            None:
+
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.axis </src/format/ooodev.format.chart2.direct.axis>` subpackages.
+
+        .. versionadded:: 0.9.4
+        """
+        try:
+            axis = cls.get_y_axis(chart_doc=chart_doc)
+        except mEx.ChartError:
+            return
+
+        for style in styles:
+            style.apply(axis)
+
+    @classmethod
+    def style_y_axis2(cls, chart_doc: XChartDocument, styles: Sequence[StyleObj]) -> None:
+        """
+        Styles Y axis2 of chart.
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+            styles (Sequence[StyleObj]): One or more styles to apply chart Y axis2.
+
+        Returns:
+            None:
+
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.axis </src/format/ooodev.format.chart2.direct.axis>` subpackages.
+
+        .. versionadded:: 0.9.4
+        """
+        try:
+            axis = cls.get_y_axis2(chart_doc=chart_doc)
+        except mEx.ChartError:
+            return
+
+        for style in styles:
+            style.apply(axis)
+
+    @classmethod
+    def style_x_axis_title(cls, chart_doc: XChartDocument, styles: Sequence[StyleObj]) -> None:
+        """
+        Styles X axis title of chart.
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+            styles (Sequence[StyleObj]): One or more styles to apply chart X axis title.
+
+        Returns:
+            None:
+
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>` subpackages.
+
+        .. versionadded:: 0.9.4
+        """
+        title_styles = [style for style in styles if not style.support_service("com.sun.star.drawing.Shape")]
+        shape_styles = [style for style in styles if style.support_service("com.sun.star.drawing.Shape")]
+        if shape_styles:
+            diagram = chart_doc.getDiagram()
+            title_shape = diagram.getXAxisTitle()
+            if title_shape:
+                for style in shape_styles:
+                    style.apply(title_shape)
+        if title_styles:
+            xtitle = cls.get_x_axis_title(chart_doc=chart_doc)
+            if xtitle:
+                cls._style_title(xtitle=xtitle, styles=title_styles)
+
+    @classmethod
+    def style_y_axis_title(cls, chart_doc: XChartDocument, styles: Sequence[StyleObj]) -> None:
+        """
+        Styles X axis title of chart.
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+            styles (Sequence[StyleObj]): One or more styles to apply chart Y axis title.
+
+        Returns:
+            None:
+
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>` subpackages.
+
+        .. versionadded:: 0.9.4
+        """
+
+        title_styles = [style for style in styles if not style.support_service("com.sun.star.drawing.Shape")]
+        shape_styles = [style for style in styles if style.support_service("com.sun.star.drawing.Shape")]
+        if shape_styles:
+            diagram = chart_doc.getDiagram()
+            title_shape = diagram.getYAxisTitle()
+            if title_shape:
+                for style in shape_styles:
+                    style.apply(title_shape)
+        if title_styles:
+            xtitle = cls.get_y_axis_title(chart_doc=chart_doc)
+            if xtitle:
+                cls._style_title(xtitle=xtitle, styles=title_styles)
+
+    @classmethod
+    def style_x_axis2_title(cls, chart_doc: XChartDocument, styles: Sequence[StyleObj]) -> None:
+        """
+        Styles X axis2 title of chart.
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+            styles (Sequence[StyleObj]): One or more styles to apply chart X axis2 title.
+
+        Returns:
+            None:
+
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>` subpackages.
+
+        .. versionadded:: 0.9.4
+        """
+        xtitle = cls.get_x_axis2_title(chart_doc=chart_doc)
+        if xtitle is None:
+            return
+        cls._style_title(xtitle=xtitle, styles=styles)
+
+    @classmethod
+    def style_y_axis2_title(cls, chart_doc: XChartDocument, styles: Sequence[StyleObj]) -> None:
+        """
+        Styles X axis2 title of chart.
+
+        Args:
+            chart_doc (XChartDocument): Chart Document.
+            styles (Sequence[StyleObj]): One or more styles to apply chart Y axis2 title.
+
+        Returns:
+            None:
+
+        Hint:
+            Styles that can be applied are found in :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>` subpackages.
+
+        .. versionadded:: 0.9.4
+        """
+        xtitle = cls.get_y_axis2_title(chart_doc=chart_doc)
+        if xtitle is None:
+            return
+        cls._style_title(xtitle=xtitle, styles=styles)
+
     # endregion Styles
 
     # region background colors
 
     @staticmethod
     def set_background_colors(chart_doc: XChartDocument, bg_color: mColor.Color, wall_color: mColor.Color) -> None:
         """
@@ -1645,15 +2169,15 @@
         try:
             diagram = chart_doc.getFirstDiagram()
             coord_sys_con = mLo.Lo.qi(XCoordinateSystemContainer, diagram, True)
             coord_sys = coord_sys_con.getCoordinateSystems()
             if coord_sys:
                 if len(coord_sys) > 1:
                     mLo.Lo.print(f"No. of coord systems: {len(coord_sys)}; using first.")
-            return coord_sys[0]  # will raise error if coord_sys is empyt or none
+            return coord_sys[0]  # will raise error if coord_sys is empty or none
         except Exception as e:
             raise mEx.ChartError("Error unable to get coord_system") from e
 
     @classmethod
     def get_chart_types(cls, chart_doc: XChartDocument) -> Tuple[XChartType, ...]:
         """
         Gets chart types for a chart.
@@ -1896,14 +2420,18 @@
 
         Raises:
             IndexError: If idx is out of range.
 
         Returns:
             List[XPropertySet]: Property set list.
         """
+        # BUG: there is a bug in the API, getDataPointByIndex() is suppose to return XPropertySet,
+        #   which is does, however, it does not properly implement the XPropertySet interface.
+        #   setPropertyValue() and getPropertyValue() are not implemented.
+        #   The Props.set() method can handle this because is has a fallback to set attributes using the setattr() method of python.
         data_series_arr = cls.get_data_series(chart_doc=chart_doc)
         if idx < 0 or idx >= len(data_series_arr):
             raise IndexError(f"Index value of {idx} is out of of range")
 
         props_lst: List[XPropertySet] = []
         i = 0
         while True:
@@ -1913,16 +2441,16 @@
                     props_lst.append(props)
                 i += 1
             except Exception:
                 props = None
 
             if props is None:
                 break
-        if len(props_lst) > 0:
-            mLo.Lo.print(f"No Series at index {idx}")
+        if len(props_lst) == 0:
+            mLo.Lo.print(f"No Data Series at index {idx}")
         return props_lst
 
     @classmethod
     def get_data_point_props(cls, chart_doc: XChartDocument, series_idx: int, idx: int) -> XPropertySet:
         """
         Get the proprieties for a specific index within the data points.
 
@@ -1949,15 +2477,17 @@
         if not props:
             raise mEx.NotFoundError("No Datapoints found to get XPropertySet from")
 
         if idx == -1:
             return props.pop()
 
         if idx < 0 or idx >= len(props):
-            raise IndexError(f"Index value of {idx} is out of of range")
+            raise IndexError(
+                f"Index value of {idx} is out of of range; use 0 to {len(props) - 1} or -1 for last item."
+            )
 
         return props[idx]
 
     @classmethod
     def set_data_point_labels(cls, chart_doc: XChartDocument, label_type: DataPointLabelTypeKind) -> None:
         """
         Sets the data point label of a chart
@@ -1971,15 +2501,15 @@
 
         Returns:
             None:
         """
         try:
             data_series_arr = cls.get_data_series(chart_doc=chart_doc)
             for data_series in data_series_arr:
-                dp_label = cast(DataPointLabel, mProps.Props.get_property(data_series, "Label"))
+                dp_label = cast("DataPointLabel", mProps.Props.get_property(data_series, "Label"))
                 dp_label.ShowNumber = False
                 dp_label.ShowCategoryName = False
                 dp_label.ShowLegendSymbol = False
                 if label_type == DataPointLabelTypeKind.NUMBER:
                     dp_label.ShowNumber = True
                 elif label_type == DataPointLabelTypeKind.PERCENT:
                     dp_label.ShowNumber = True
@@ -2109,41 +2639,64 @@
         try:
             rc = mLo.Lo.create_instance_mcf(XRegressionCurve, curve_kind.to_namespace(), raise_err=True)
             return rc
         except Exception as e:
             raise mEx.ChartError("Error creating curve") from e
 
     @classmethod
-    def draw_regression_curve(cls, chart_doc: XChartDocument, curve_kind: CurveKind) -> None:
+    def draw_regression_curve(
+        cls, chart_doc: XChartDocument, curve_kind: CurveKind, styles: Sequence[StyleObj] | None = None
+    ) -> XPropertySet:
         """
         Draws a regression curve.
 
         Args:
             chart_doc (XChartDocument): Chart Document
             curve_kind (CurveKind): Curve kind.
+            styles (Sequence[StyleObj], optional): Styles to apply to the curve. Defaults to ``None``.
 
         Raises:
             ChartError: If error occurs.
 
         Returns:
-            None:
+            XPropertySet: Regression curve property set.
+
+        Hint:
+            Styles that can be applied are found in the following subpackages:
+
+                - :doc:`ooodev.format.chart2.direct.title </src/format/ooodev.format.chart2.direct.title>`
+                - :doc:`ooodev.format.chart2.direct.general.numbers </src/format/ooodev.format.chart2.direct.general.numbers>`
+
+        .. versionchanged:: 0.9.4
+            Added ``styles`` argument, and now returns the regression curve property set.
         """
         try:
             data_series_arr = cls.get_data_series(chart_doc=chart_doc)
             rc_con = mLo.Lo.qi(XRegressionCurveContainer, data_series_arr[0], True)
             curve = cls.create_curve(curve_kind)
             rc_con.addRegressionCurve(curve)
 
             ps = curve.getEquationProperties()
-            mProps.Props.set_property(ps, "ShowCorrelationCoefficient", True)
-            mProps.Props.set_property(ps, "ShowEquation", True)
+            mProps.Props.set(ps, ShowCorrelationCoefficient=True, ShowEquation=True)
 
             key = cls.get_number_format_key(chart_doc=chart_doc, nf_str="0.00")  # 2 dp
             if key != -1:
-                mProps.Props.set_property(ps, "NumberFormat", key)
+                mProps.Props.set(ps, NumberFormat=key)
+            if styles:
+                supported = (
+                    "com.sun.star.chart2.RegressionEquation",
+                    "com.sun.star.drawing.FillProperties",
+                    "com.sun.star.drawing.LineProperties",
+                    "com.sun.star.style.CharacterProperties",
+                )
+
+                for style in styles:
+                    if style.support_service(*supported):
+                        style.apply(ps)
+            return ps
         except mEx.ChartError:
             raise
         except Exception as e:
             raise mEx.ChartError("Error drawing regression curve") from e
 
     @staticmethod
     def get_number_format_key(chart_doc: XChartDocument, nf_str: str) -> int:
@@ -2165,15 +2718,18 @@
             The string-to-key conversion is straight forward if you know what number format string to use,
             but there's little documentation on them. Probably the best approach is to use the Format
             Cells menu item in a spreadsheet document, and examine the dialog
         """
         try:
             xfs = mLo.Lo.qi(XNumberFormatsSupplier, chart_doc, True)
             n_formats = xfs.getNumberFormats()
-            key = int(n_formats.queryKey(nf_str, Locale("en", "us", ""), False))
+            # locale = Locale("en", "us", "")
+            # locale = mInfo.Info.language_locale
+            # note the empty locale for default locale
+            key = int(n_formats.queryKey(nf_str, Locale(), False))
             if key == -1:
                 mLo.Lo.print(f'Could not access key for number format: "{nf_str}"')
             return key
         except Exception as e:
             raise mEx.ChartError("Error getting number format key") from e
 
     @staticmethod
@@ -2445,124 +3001,263 @@
         except Exception as e:
             raise mEx.ChartError("Error adding category lables") from e
 
     # endregion add data to a chart
 
     # region chart shape and image
     @staticmethod
-    def get_chart_shape(sheet: XSpreadsheet) -> XShape:
+    def get_chart_shape(sheet: XSpreadsheet, chart_name: str = "") -> XShape:
         """
         Gets chart shape
 
         Args:
             sheet (XSpreadsheet): Spreadsheet
+            chart_name (str, optional): Chart name. Defaults to "". If ``""`` then first chart is returned.
 
         Raises:
             ShapeMissingError: If shape is ``None``.
             ShapeError: If any other error occurs.
 
         Returns:
             XShape: Shape object.
+
+        .. versionchanged:: 0.9.4
+            Added chart_name parameter.
         """
         shape = None
+        if chart_name:
+            chart_name = chart_name.casefold()
         try:
             page_supp = mLo.Lo.qi(XDrawPageSupplier, sheet, True)
             draw_page = page_supp.getDrawPage()
             num_shapes = draw_page.getCount()
             chart_classid = mLo.Lo.CLSID.CHART.value
             for i in range(num_shapes):
                 try:
-                    shape = mLo.Lo.qi(XShape, draw_page.getByIndex(i), True)
+                    shape = cast("OLE2Shape", mLo.Lo.qi(XShape, draw_page.getByIndex(i), True))
                     classid = str(mProps.Props.get(shape, "CLSID")).lower()
-                    if classid == chart_classid:
-                        break
+                    if chart_name:
+                        if classid == chart_classid and chart_name == shape.PersistName.casefold():
+                            break
+                    else:
+                        if classid == chart_classid:
+                            break
                 except Exception:
                     shape = None
                     # continue on, just because got an error does not mean shape will not be found
         except Exception as e:
             raise mEx.ShapeError("Error getting shape from sheet") from e
         if shape is None:
             raise mEx.ShapeMissingError("Unalbe to find Chart Shape")
         return shape
 
     @classmethod
-    def copy_chart(cls, ssdoc: XSpreadsheetDocument, sheet: XSpreadsheet) -> None:
+    def copy_chart(cls, ssdoc: XSpreadsheetDocument, sheet: XSpreadsheet, chart_name: str = "") -> None:
         """
         Copies a chart using a dispatch command.
 
         Args:
-            ssdoc (XSpreadsheetDocument): Spreadsheet Document
-            sheet (XSpreadsheet): Spreadsheet
+            ssdoc (XSpreadsheetDocument): Spreadsheet Document.
+            sheet (XSpreadsheet): Spreadsheet.
+            chart_name (str, optional): Chart name. Defaults to "". If ``""`` then first chart is copied.
 
         Raises:
             ChartError: If error occurs.
 
         Returns:
             None:
+
+        .. versionchanged:: 0.9.4
+            Added chart_name parameter.
         """
         try:
-            chart_shape = cls.get_chart_shape(sheet=sheet)
+            chart_shape = cls.get_chart_shape(sheet=sheet, chart_name=chart_name)
             doc = mLo.Lo.qi(XComponent, ssdoc, True)
             supp = mGui.GUI.get_selection_supplier(doc)
             supp.select(chart_shape)
             mLo.Lo.dispatch_cmd("Copy")
         except Exception as e:
             raise mEx.ChartError("Error in attempt to copy chart") from e
 
     @classmethod
-    def get_chart_draw_page(cls, sheet: XSpreadsheet) -> XDrawPage:
+    def get_chart_draw_page(cls, sheet: XSpreadsheet, chart_name: str = "") -> XDrawPage:
         """
         Gets chart draw page.
 
         Args:
             sheet (XSpreadsheet): Spreadsheet
+            chart_name (str, optional): Chart name. Defaults to "". If ``""`` then first chart Draw Page is returned.
 
         Raises:
             ChartError: If error occurs.
 
         Returns:
             XDrawPage: Draw Page object
+
+        .. versionchanged:: 0.9.4
+            Added chart_name parameter.
         """
         try:
-            chart_shape = cls.get_chart_shape(sheet)
+            chart_shape = cls.get_chart_shape(sheet=sheet, chart_name=chart_name)
             embedded_chart = mLo.Lo.qi(XEmbeddedObject, mProps.Props.get_property(chart_shape, "EmbeddedObject"), True)
             comp_supp = mLo.Lo.qi(XComponentSupplier, embedded_chart, True)
             xclosable = comp_supp.getComponent()
             supp_page = mLo.Lo.qi(XDrawPageSupplier, xclosable, True)
             result = supp_page.getDrawPage()
             if result is None:
                 raise mEx.UnKnownError("None Value: getDrawPage() returned a value of None")
             return result
         except Exception as e:
             raise mEx.ChartError("Error getting chart draw page") from e
 
     @classmethod
-    def get_chart_image(cls, sheet: XSpreadsheet) -> XGraphic:
+    def get_chart_image(cls, sheet: XSpreadsheet, chart_name: str = "") -> XGraphic:
         """
         Get chart image as ``XGraphic``.
 
         Args:
-            sheet (XSpreadsheet): Spreadsheet
+            sheet (XSpreadsheet): Spreadsheet.
+            chart_name (str, optional): Chart name. Defaults to "". If ``""`` then first chart image is returned.
 
         Raises:
             ChartError: If error occurs.
 
         Returns:
             XGraphic: Graphic object
+
+        .. versionchanged:: 0.9.4
+            Added chart_name parameter.
         """
         try:
-            chart_shape = cls.get_chart_shape(sheet)
+            chart_shape = cls.get_chart_shape(sheet=sheet, chart_name=chart_name)
 
             graphic = mLo.Lo.qi(XGraphic, mProps.Props.get(chart_shape, "Graphic"), True)
 
             tmp_fnm = mFileIo.FileIO.create_temp_file("png")
             mImgLo.ImagesLo.save_graphic(pic=graphic, fnm=tmp_fnm, im_format="png")
             im = mImgLo.ImagesLo.load_graphic_file(tmp_fnm)
             mFileIo.FileIO.delete_file(tmp_fnm)
             return im
         except Exception as e:
             raise mEx.ChartError("Error getting chart image") from e
 
     # endregion chart shape and image
 
+    # region Lock Controllers
+
+    @classmethod
+    def lock_controllers(cls, chart_doc: XChartDocument) -> bool:
+        """
+        Suspends some notifications to the controllers which are used for display updates.
+
+        The calls to :py:meth:`~.chart2.Chart2.lock_controllers` and :py:meth:`~.chart2.Chart2.unlock_controllers`
+        may be nested and even overlapping, but they must be in pairs.
+        While there is at least one lock remaining, some notifications for
+        display updates are not broadcast.
+
+        Returns:
+            bool: False if ``CONTROLERS_LOCKING`` event is canceled; Otherwise, True
+
+         :events:
+            .. cssclass:: lo_event
+
+                - :py:attr:`~.events.chart2_named_event.Chart2NamedEvent.CONTROLERS_LOCKING` :eventref:`src-docs-event-cancel`
+                - :py:attr:`~.events.chart2_named_event.Chart2NamedEvent.CONTROLERS_LOCKED` :eventref:`src-docs-event`
+
+        See Also:
+
+            - :py:class:`~.chart2.Chart2ControllerLock`
+            - :py:meth:`~.chart2.Chart2.unlock_controllers`
+
+        .. versionadded:: 0.9.4
+        """
+        # much faster updates as screen is basically suspended
+        cargs = CancelEventArgs(Chart2.lock_controllers.__qualname__)
+        _Events().trigger(Chart2NamedEvent.CONTROLERS_LOCKING, cargs)
+        if cargs.cancel:
+            return False
+        chart_doc.lockControllers()
+        _Events().trigger(Chart2NamedEvent.CONTROLERS_LOCKED, EventArgs(cls))
+        return True
+
+    @staticmethod
+    def unlock_controllers(chart_doc: XChartDocument) -> bool:
+        """
+        Resumes the notifications which were suspended by :py:meth:`~.chart2.Chart2.lock_controllers`.
+
+        The calls to :py:meth:`~.chart2.Chart2.lock_controllers` and :py:meth:`~.chart2.Chart2.unlock_controllers`
+        may be nested and even overlapping, but they must be in pairs.
+        While there is at least one lock remaining, some notifications for
+        display updates are not broadcast.
+
+        Returns:
+            bool: False if ``CONTROLERS_UNLOCKING`` event is canceled; Otherwise, True
+
+        :events:
+            .. cssclass:: lo_event
+
+                - :py:attr:`~.events.chart2_named_event.Chart2NamedEvent.CONTROLERS_UNLOCKING` :eventref:`src-docs-event-cancel`
+                - :py:attr:`~.events.chart2_named_event.Chart2NamedEvent.CONTROLERS_UNLOCKED` :eventref:`src-docs-event`
+
+        See Also:
+
+            - :py:class:`~.chart2.Chart2ControllerLock`
+            - :py:meth:`~.chart2.Chart2.lock_controllers`
+
+        .. versionadded:: 0.9.4
+        """
+        cargs = CancelEventArgs(Chart2.unlock_controllers.__qualname__)
+        _Events().trigger(Chart2NamedEvent.CONTROLERS_UNLOCKING, cargs)
+        if cargs.cancel:
+            return False
+        if chart_doc.hasControllersLocked():
+            chart_doc.unlockControllers()
+        _Events().trigger(Chart2NamedEvent.CONTROLERS_UNLOCKED, EventArgs.from_args(cargs))
+        return True
+
+    # endregion Lock Controllers
+
+
+class Chart2ControllerLock:
+    """
+    Context manager for Locking Chart2 Controller
+
+    In the following example ControllerLock is called using ``with``.
+
+    All code inside the ``with Chart2ControllerLock.ControllerLock(chart_doc)`` block is updated
+    with controller locked. This means the ui will not update chart until the block is done.
+    A soon as the block is processed the controller is unlocked and the ui is updated.
+
+    Example:
+
+        .. code::
+
+            from ooodev.utils.color import CommonColor
+            from ooodev.office.chart2 import Chart2
+            from ooodev.office.chart2 import Chart2ControllerLock
+            from ooodev.format.chart2.direct.title.area import Color as ChartTitleBgColor
+            from ooodev.format.chart2.direct.title.font import Font as TitleFont
+            from ooodev.format.chart2.direct.title.borders import LineProperties as TitleBorderLineProperties, BorderLineKind
+            # ... other imports
+
+            with Chart2ControllerLock.ControllerLock(chart_doc):
+                title_area_bg_color = ChartTitleBgColor(CommonColor.LIGHT_YELLOW)
+                title_font = TitleFont(b=True, size=14, color=CommonColor.DARK_GREEN)
+                title_border = TitleBorderLineProperties(style=BorderLineKind.DASH_DOT, width=1.0, color=CommonColor.DARK_RED)
+                Chart2.style_title(chart_doc=chart_doc, styles=[title_area_bg_color, title_font, title_border])
+                # ... other code
+
+    .. versionadded:: 0.9.4
+    """
+
+    def __init__(self, chart_doc: XChartDocument):
+        self._chart_doc = chart_doc
+        Chart2.lock_controllers(chart_doc=self._chart_doc)
+
+    def __enter__(self) -> XChartDocument:
+        return self._chart_doc
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        Chart2.unlock_controllers(self._chart_doc)
+
 
-__all__ = ("Chart2",)
+__all__ = ("Chart2", "Chart2ControllerLock")
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/office/draw.py` & `ooo_dev_tools-0.9.4/ooodev/office/draw.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/office/write.py` & `ooo_dev_tools-0.9.4/ooodev/office/write.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 # Python conversion of Write.java by Andrew Davison, ad@fivedots.coe.psu.ac.th
 # See Also: https://fivedots.coe.psu.ac.th/~ad/jlop/
 # region Imports
 from __future__ import annotations
-from typing import TYPE_CHECKING, Iterable, List, cast, overload, Union
+from typing import TYPE_CHECKING, Iterable, List, Sequence, cast, overload, Union
 import re
 import uno
 from com.sun.star.awt import FontWeight
 from com.sun.star.beans import XPropertySet
 from com.sun.star.container import XEnumerationAccess
 from com.sun.star.container import XNamed
 from com.sun.star.document import XDocumentInsertable
@@ -790,15 +790,15 @@
     # region    append()
     @classmethod
     def _append_text(cls, cursor: XTextCursor, text: str) -> None:
         cursor.setString(text)
         cursor.gotoEnd(False)
 
     @classmethod
-    def _append_text_style(cls, cursor: XTextCursor, text: str, styles: Iterable[StyleObj]) -> None:
+    def _append_text_style(cls, cursor: XTextCursor, text: str, styles: Sequence[StyleObj]) -> None:
         s_len = len(text)
         if s_len == 0:
             return
 
         cursor.setString(text)
         cursor.gotoEnd(False)
         style_srv = (
@@ -853,15 +853,15 @@
     @overload
     @classmethod
     def append(cls, cursor: XTextCursor, text: str) -> None:
         ...
 
     @overload
     @classmethod
-    def append(cls, cursor: XTextCursor, text: str, styles: Iterable[StyleObj]) -> None:
+    def append(cls, cursor: XTextCursor, text: str, styles: Sequence[StyleObj]) -> None:
         ...
 
     @overload
     @classmethod
     def append(cls, cursor: XTextCursor, ctl_char: ControlCharacterEnum) -> None:
         ...
 
@@ -874,15 +874,15 @@
     def append(cls, *args, **kwargs) -> None:
         """
         Append content to cursor
 
         Args:
             cursor (XTextCursor): Text Cursor
             text (str): Text to append
-            styles (Iterable[StyleObj]):One or more styles to apply to text.
+            styles (Sequence[StyleObj]):One or more styles to apply to text.
             ctl_char (int): Control Char (like a paragraph break or a hard space)
             text_content (XTextContent): Text content, such as a text table, text frame or text field.
 
         Returns:
             None:
 
         :events:
@@ -893,15 +893,15 @@
                 - :py:attr:`~.events.write_named_event.WriteNamedEvent.STYLING` :eventref:`src-docs-event-cancel`
                 - :py:attr:`~.events.write_named_event.WriteNamedEvent.STYLED` :eventref:`src-docs-event`
 
         See Also:
             `API ControlCharacter <https://api.libreoffice.org/docs/idl/ref/namespacecom_1_1sun_1_1star_1_1text_1_1ControlCharacter.html>`_
 
         .. versionchanged:: 0.9.0
-            Added ``append(cursor: XTextCursor, text: str, styles: Iterable[StyleObj])`` overload.
+            Added ``append(cursor: XTextCursor, text: str, styles: Sequence[StyleObj])`` overload.
 
             Added Events.
         """
         ordered_keys = (1, 2, 3)
         kargs_len = len(kwargs)
         count = len(args) + kargs_len
 
@@ -956,37 +956,37 @@
     @overload
     @classmethod
     def append_line(cls, cursor: XTextCursor, text: str) -> None:
         ...
 
     @overload
     @classmethod
-    def append_line(cls, cursor: XTextCursor, text: str, styles: Iterable[StyleObj]) -> None:
+    def append_line(cls, cursor: XTextCursor, text: str, styles: Sequence[StyleObj]) -> None:
         ...
 
     @classmethod
-    def append_line(cls, cursor: XTextCursor, text: str = "", styles: Iterable[StyleObj] = None) -> None:
+    def append_line(cls, cursor: XTextCursor, text: str = "", styles: Sequence[StyleObj] = None) -> None:
         """
         Appends a new Line
 
         Args:
             cursor (XTextCursor): Text Cursor
             text (str, optional): text to append before new line is inserted.
-            styles (Iterable[StyleObj]): One or more styles to apply to text. If ``text`` is omitted then this argument is ignored.
+            styles (Sequence[StyleObj]): One or more styles to apply to text. If ``text`` is omitted then this argument is ignored.
 
         :events:
             If using styles then the following events are triggered for each style.
 
             .. cssclass:: lo_event
 
                 - :py:attr:`~.events.write_named_event.WriteNamedEvent.STYLING` :eventref:`src-docs-event-cancel`
                 - :py:attr:`~.events.write_named_event.WriteNamedEvent.STYLED` :eventref:`src-docs-event`
 
         .. versionchanged:: 0.9.0
-            Added overload ``append_line(cursor: XTextCursor, text: str, styles: Iterable[StyleObj])``.
+            Added overload ``append_line(cursor: XTextCursor, text: str, styles: Sequence[StyleObj])``.
 
             Added events.
         """
         if text:
             if styles is None:
                 cls._append_text(cursor=cursor, text=text)
             else:
@@ -1027,37 +1027,37 @@
     @overload
     @classmethod
     def append_para(cls, cursor: XTextCursor, text: str) -> None:
         ...
 
     @overload
     @classmethod
-    def append_para(cls, cursor: XTextCursor, text: str, styles: Iterable[StyleObj]) -> None:
+    def append_para(cls, cursor: XTextCursor, text: str, styles: Sequence[StyleObj]) -> None:
         ...
 
     @classmethod
-    def append_para(cls, cursor: XTextCursor, text: str = "", styles: Iterable[StyleObj] = None) -> None:
+    def append_para(cls, cursor: XTextCursor, text: str = "", styles: Sequence[StyleObj] = None) -> None:
         """
         Appends text (if present) and then a paragraph break.
 
         Args:
             cursor (XTextCursor): Text Cursor
             text (str, optional): Text to append
-            styles (Iterable[StyleObj]): One or more styles to apply to text. If ``text`` is empty then this argument is ignored.
+            styles (Sequence[StyleObj]): One or more styles to apply to text. If ``text`` is empty then this argument is ignored.
 
         :events:
             If using styles then the following events are triggered for each style.
 
             .. cssclass:: lo_event
 
                 - :py:attr:`~.events.write_named_event.WriteNamedEvent.STYLING` :eventref:`src-docs-event-cancel`
                 - :py:attr:`~.events.write_named_event.WriteNamedEvent.STYLED` :eventref:`src-docs-event`
 
         .. versionchanged:: 0.9.0
-            Added overload ``append_para(cursor: XTextCursor, text: str, styles: Iterable[StyleObj])``.
+            Added overload ``append_para(cursor: XTextCursor, text: str, styles: Sequence[StyleObj])``.
 
             Added Events.
         """
 
         # paragraph styles need to capture the current pargarph setting and restore them.
         # other styles are handeled by _append_text_style().
 
@@ -1352,15 +1352,15 @@
         cursor.goRight(pos, False)
         cursor.goRight(distance, True)
         mProps.Props.set(cursor, **{prop_name: prop_val})
         cursor.gotoEnd(False)
         _Events().trigger(WriteNamedEvent.STYLED, KeyValArgs.from_args(cargs))
 
     @classmethod
-    def _style_style(cls, pos: int, distance: int, styles: Iterable[StyleObj], cursor: XTextCursor = None) -> None:
+    def _style_style(cls, pos: int, distance: int, styles: Sequence[StyleObj], cursor: XTextCursor = None) -> None:
         if cursor is None:
             cursor = cls.get_cursor()
         # cursor.collapseToEnd()
         cursor.gotoStart(False)
         cursor.goRight(pos, False)
         cursor.goRight(distance, True)
 
@@ -1381,20 +1381,20 @@
                 continue
             style.apply(cursor)
             _Events().trigger(WriteNamedEvent.STYLED, EventArgs.from_args(cargs))
         cursor.gotoEnd(False)
 
     @overload
     @classmethod
-    def style(cls, pos: int, length: int, styles: Iterable[StyleObj]) -> None:
+    def style(cls, pos: int, length: int, styles: Sequence[StyleObj]) -> None:
         ...
 
     @overload
     @classmethod
-    def style(cls, pos: int, length: int, styles: Iterable[StyleObj], cursor: XTextCursor) -> None:
+    def style(cls, pos: int, length: int, styles: Sequence[StyleObj], cursor: XTextCursor) -> None:
         ...
 
     @overload
     @classmethod
     def style(cls, pos: int, length: int, prop_name: str, prop_val: object) -> None:
         ...
 
@@ -1407,15 +1407,15 @@
     def style(cls, *args, **kwargs) -> None:
         """
         Styles. From position styles right by distance amount.
 
         Args:
             pos (int): Position style start.
             length (int): The distance from ``pos`` to apply style.
-            styles (Iterable[StyleObj]):One or more styles to apply to text.
+            styles (Sequence[StyleObj]):One or more styles to apply to text.
             prop_name (str): Property Name such as ``CharHeight``
             prop_val (object): Property Value such as ``10``
             cursor (XTextCursor): Text Cursor
 
         Returns:
             None:
 
@@ -1499,15 +1499,15 @@
             cursor.goRight(amt, False)
             mProps.Props.set(cursor, **{prop_name: old_val})
         else:
             cursor.goRight(0, False)
         _Events().trigger(WriteNamedEvent.STYLED, KeyValArgs.from_args(cargs))
 
     @classmethod
-    def _style_left_style(cls, cursor: XTextCursor, pos: int, styles: Iterable[StyleObj]) -> None:
+    def _style_left_style(cls, cursor: XTextCursor, pos: int, styles: Sequence[StyleObj]) -> None:
         # store properties about to be changed
 
         if pos == 0:
             cursor.goLeft(0, True)
             amt = 0
         else:
             curr_pos = mSel.Selection.get_position(cursor)
@@ -1552,15 +1552,15 @@
             _Events().trigger(WriteNamedEvent.STYLED, EventArgs.from_args(cargs))
 
         if pos <= 0:
             cursor.goRight(0, False)
 
     @overload
     @classmethod
-    def style_left(cls, cursor: XTextCursor, pos: int, styles: Iterable[StyleObj]) -> None:
+    def style_left(cls, cursor: XTextCursor, pos: int, styles: Sequence[StyleObj]) -> None:
         ...
 
     @overload
     @classmethod
     def style_left(cls, cursor: XTextCursor, pos: int, prop_name: str, prop_val: object) -> None:
         ...
 
@@ -1568,18 +1568,18 @@
     def style_left(cls, *args, **kwargs) -> None:
         """
         Styles left. From current cursor position to left by pos amount.
 
         Args:
             cursor (XTextCursor): Text Cursor
             pos (int): Positions to style left
-            styles (Iterable[StyleObj]):One or more styles to apply to text.
+            styles (Sequence[StyleObj]):One or more styles to apply to text.
             prop_name (str): Property Name such as ``CharHeight``
             prop_val (object): Property Value such as ``10``
-            styles (Iterable[StyleObj], optional): One or more styles to apply.
+            styles (Sequence[StyleObj], optional): One or more styles to apply.
 
         Returns:
             None:
 
         :events:
             If using styles then the following events are triggered for each style.
 
@@ -1600,15 +1600,15 @@
 
         Note:
             This method restores the style properties to their original state after the style is applied.
             This is done so applied style properties are reset before next text is appended.
             This is not the case for :py:meth:`~.Write.style` method.
 
         .. versionchanged:: 0.9.0
-            Added ``style_left(cursor: XTextCursor, pos: int, styles: Iterable[StyleObj])`` overload.
+            Added ``style_left(cursor: XTextCursor, pos: int, styles: Sequence[StyleObj])`` overload.
 
             Added Events.
         """
         ordered_keys = (1, 2, 3, 4)
         kargs_len = len(kwargs)
         count = len(args) + kargs_len
 
@@ -1721,15 +1721,15 @@
         cursor.gotoNextParagraph(False)
         mProps.Props.set(cursor, **{prop_name: old_val})
         eargs = KeyValArgs.from_args(cargs)
         _Events().trigger(WriteNamedEvent.STYLED, eargs)
         _Events().trigger(WriteNamedEvent.STYLE_PREV_PARA_PROP_SET, eargs)
 
     @classmethod
-    def _style_prev_paragraph_style(cls, cursor: XTextCursor | XParagraphCursor, styles: Iterable[StyleObj]) -> None:
+    def _style_prev_paragraph_style(cls, cursor: XTextCursor | XParagraphCursor, styles: Sequence[StyleObj]) -> None:
         if not styles:
             return
         c_styles_args = CancelEventArgs("Write._style_prev_paragraph_style")
         c_styles_args.event_data = styles
         _Events().trigger(WriteNamedEvent.STYLE_PREV_PARA_STYLES_SETTING, c_styles_args)
         if c_styles_args.cancel:
             return
@@ -1737,15 +1737,15 @@
             "com.sun.star.style.CharacterProperties",
             "com.sun.star.style.ParagraphProperties",
             "com.sun.star.drawing.FillProperties",
         )
 
         style_lst: List[StyleObj] = []
         fill_lst: List[StyleObj] = []
-        style_data = cast(Iterable[StyleObj], c_styles_args.event_data)
+        style_data = cast(Sequence[StyleObj], c_styles_args.event_data)
         for style in style_data:
             if not style.support_service(*style_srv):
                 mLo.Lo.print(
                     f"style_prev_paragraph(), Supported services are {style_srv}. Not Supported style: {style}"
                 )
                 continue
             if FormatKind.TXT_CONTENT in style.prop_format_kind and FormatKind.PARA in style.prop_format_kind:
@@ -1790,15 +1790,15 @@
                 para_c.gotoNextParagraph(False)
 
         e_style_args = EventArgs.from_args(c_styles_args)
         _Events().trigger(WriteNamedEvent.STYLE_PREV_PARA_STYLES_SET, e_style_args)
 
     @overload
     @classmethod
-    def style_prev_paragraph(cls, cursor: XTextCursor, styles: Iterable[StyleObj]) -> None:
+    def style_prev_paragraph(cls, cursor: XTextCursor, styles: Sequence[StyleObj]) -> None:
         ...
 
     @overload
     @classmethod
     def style_prev_paragraph(cls, cursor: XTextCursor, prop_val: object) -> None:
         ...
 
@@ -1810,15 +1810,15 @@
     @classmethod
     def style_prev_paragraph(cls, *args, **kwargs) -> None:
         """
         Style previous paragraph
 
         Args:
             cursor (XTextCursor): Text Cursor
-            styles (Iterable[StyleObj]): One or more styles to apply to text.
+            styles (Sequence[StyleObj]): One or more styles to apply to text.
             prop_val (object): Property value
             prop_name (str): Property Name
 
         :events:
             If using styles then the following events are triggered for each style.
 
             .. cssclass:: lo_event
@@ -1840,15 +1840,15 @@
 
             .. code-block:: python
 
                 cursor = Write.get_cursor(doc)
                 Write.style_prev_paragraph(cursor=cursor, prop_val=ParagraphAdjust.CENTER, prop_name="ParaAdjust")
 
         .. versionchanged:: 0.9.0
-            Added overload ``style_prev_paragraph(cursor: XTextCursor, styles: Iterable[StyleObj])``
+            Added overload ``style_prev_paragraph(cursor: XTextCursor, styles: Sequence[StyleObj])``
         """
         ordered_keys = (1, 2, 3)
         kargs_len = len(kwargs)
         count = len(args) + kargs_len
 
         def get_kwargs() -> dict:
             ka = {}
@@ -1879,35 +1879,35 @@
 
         if count == 3:
             cls._style_prev_paragraph_prop(cursor=kargs[1], prop_val=kargs[2], prop_name=kargs[3])
             return
 
         # count == 2
         arg2 = kargs[2]
-        # arg2 must be string or Iterable[StyleObj]
+        # arg2 must be string or Sequence[StyleObj]
         # ParaStyleName can only be set a string value
         if isinstance(arg2, str):
             cls._style_prev_paragraph_prop(cursor=kargs[1], prop_val=arg2, prop_name="ParaStyleName")
         else:
             cls._style_prev_paragraph_style(cursor=kargs[1], styles=arg2)
 
     # endregion style_prev_paragraph()
 
     # endregion ---------- text cursor property methods ----------------
 
     # region ------------- style methods -------------------------------
     @staticmethod
-    def create_style_para(text_doc: XTextDocument, style_name: str, styles: Iterable[StyleObj] = None) -> XStyle:
+    def create_style_para(text_doc: XTextDocument, style_name: str, styles: Sequence[StyleObj] = None) -> XStyle:
         """
         Creates a paragraph style and adds it to document paragraph styles.
 
         Args:
             text_doc (XTextDocument): Text Document
             style_name (str): The name of the paragraph style.
-            styles (Iterable[StyleObj], optional): One or more styles to apply.
+            styles (Sequence[StyleObj], optional): One or more styles to apply.
 
         Returns:
             XStyle: Newly created style
 
         .. versionadded:: 0.9.2
         """
         para_styles = mInfo.Info.get_style_container(doc=text_doc, family_style_name="ParagraphStyles")
@@ -1921,22 +1921,22 @@
                 style.apply(props)
 
         # add the style to Document
         para_styles.insertByName(style_name, props)
         return para_styles
 
     @staticmethod
-    def create_style_char(text_doc: XTextDocument, style_name: str, styles: Iterable[StyleObj] = None) -> XStyle:
+    def create_style_char(text_doc: XTextDocument, style_name: str, styles: Sequence[StyleObj] = None) -> XStyle:
         """
         Creates a character style and adds it to document character styles.
 
         Args:
             text_doc (XTextDocument): Text Document
             style_name (str): The name of the character style.
-            styles (Iterable[StyleObj], optional): One or more styles to apply.
+            styles (Sequence[StyleObj], optional): One or more styles to apply.
 
         Returns:
             XStyle: Newly created style
 
         .. versionadded:: 0.9.2
         """
         char_styles = mInfo.Info.get_style_container(doc=text_doc, family_style_name="CharacterStyles")
@@ -2172,15 +2172,15 @@
         """
         pc_field = mLo.Lo.create_instance_msf(XTextField, "com.sun.star.text.TextField.PageCount")
         mProps.Props.set(pc_field, NumberingType=NumberingType.ARABIC)
         return pc_field
 
     @staticmethod
     def _set_header_footer(
-        text_doc: XTextDocument, text: str, kind: str = "h", styles: Iterable[StyleObj] = None
+        text_doc: XTextDocument, text: str, kind: str = "h", styles: Sequence[StyleObj] = None
     ) -> None:
         props = mInfo.Info.get_style_props(doc=text_doc, family_style_name="PageStyles", prop_set_nm="Standard")
         if props is None:
             raise mEx.PropertiesError("Could not access the standard page style container")
         try:
             # header or footer must be turned on in the document
             if kind == "h":
@@ -2222,24 +2222,24 @@
                         style.apply(text_doc)
                     else:
                         style.apply(props)
         except Exception as e:
             raise Exception("Unable to set header text") from e
 
     @classmethod
-    def set_header(cls, text_doc: XTextDocument, text: str, styles: Iterable[StyleObj] = None) -> None:
+    def set_header(cls, text_doc: XTextDocument, text: str, styles: Sequence[StyleObj] = None) -> None:
         """
         Modify the header via the page style for the document.
         Put the text on the right hand side in the header in
         a general font of 10pt.
 
         Args:
             text_doc (XTextDocument): Text Document
             text (str): Header Text
-            styles (Iterable[StyleObj]): Styles to apply to the text.
+            styles (Sequence[StyleObj]): Styles to apply to the text.
 
         Raises:
             PropertiesError: If unable to access properties
             Exception: If unable to set header text
 
         See Also:
             :py:meth:`~.wrtie.Write.set_footer`
@@ -2249,24 +2249,24 @@
 
         .. versionchanged:: 0.9.2
             Added styles parameter
         """
         cls._set_header_footer(text_doc=text_doc, text=text, kind="h", styles=styles)
 
     @classmethod
-    def set_footer(cls, text_doc: XTextDocument, text: str, styles: Iterable[StyleObj] = None) -> None:
+    def set_footer(cls, text_doc: XTextDocument, text: str, styles: Sequence[StyleObj] = None) -> None:
         """
         Modify the footer via the page style for the document.
         Put the text on the right hand side in the header in
         a general font of 10pt.
 
         Args:
             text_doc (XTextDocument): Text Document
             text (str): Header Text
-            styles (Iterable[StyleObj]): Styles to apply to the text.
+            styles (Sequence[StyleObj]): Styles to apply to the text.
 
         Raises:
             PropertiesError: If unable to access properties
             Exception: If unable to set header text
 
         See Also:
             :py:meth:`~.wrtie.Write.set_header`
@@ -2303,26 +2303,26 @@
     @overload
     @classmethod
     def add_formula(cls, cursor: XTextCursor, formula: str) -> XTextContent:
         ...
 
     @overload
     @classmethod
-    def add_formula(cls, cursor: XTextCursor, formula: str, styles: Iterable[StyleObj] = None) -> XTextContent:
+    def add_formula(cls, cursor: XTextCursor, formula: str, styles: Sequence[StyleObj] = None) -> XTextContent:
         ...
 
     @classmethod
-    def add_formula(cls, cursor: XTextCursor, formula: str, styles: Iterable[StyleObj] = None) -> XTextContent:
+    def add_formula(cls, cursor: XTextCursor, formula: str, styles: Sequence[StyleObj] = None) -> XTextContent:
         """
         Adds a formula
 
         Args:
             cursor (XTextCursor): Cursor
             formula (str): formula
-            styles (Iterable[StyleObj]): One or more styles to apply to frame. Only styles that support ``com.sun.star.text.TextEmbeddedObject`` service are applied.
+            styles (Sequence[StyleObj]): One or more styles to apply to frame. Only styles that support ``com.sun.star.text.TextEmbeddedObject`` service are applied.
 
         Raises:
             CreateInstanceMsfError: If unable to create text.TextEmbeddedObject
             Exception: If unable to add formula
 
         Returns:
             XTextContent: Embedded Object.
@@ -2515,29 +2515,29 @@
         text: str = "",
         ypos: int | UnitObj = 300,
         width: int | UnitObj = 5000,
         height: int | UnitObj = 5000,
         page_num: int = 1,
         border_color: Color | None = None,
         background_color: Color | None = None,
-        styles: Iterable[StyleObj] = None,
+        styles: Sequence[StyleObj] = None,
     ) -> XTextFrame:
         """
         Adds a text frame.
 
         Args:
             cursor (XTextCursor): Text Cursor
             text (str, optional): Frame Text
             ypos (int, UnitObj. optional): Frame Y pos in ``1/100th mm`` or :ref:`proto_unit_obj`. Default ``300``.
             width (int, UnitObj, optional): Width in ``1/100th mm`` or :ref:`proto_unit_obj`.
             height (int, UnitObj, optional): Height in ``1/100th mm`` or :ref:`proto_unit_obj`.
             page_num (int, optional): Page Number to add text frame. If ``0`` Then Frame is anchored to paragraph. Default ``1``.
             border_color (:py:data:`~.utils.color.Color`, optional):.color.Color`, optional): Border Color.
             background_color (:py:data:`~.utils.color.Color`, optional): Background Color.
-            styles (Iterable[StyleObj]): One or more styles to apply to frame. Only styles that support ``com.sun.star.text.TextFrame`` service are applied.
+            styles (Sequence[StyleObj]): One or more styles to apply to frame. Only styles that support ``com.sun.star.text.TextFrame`` service are applied.
 
         Raises:
             CreateInstanceMsfError: If unable to create text.TextFrame
             Exception: If unable to add text frame
 
         Returns:
             XTextFrame: Text frame that is added to document.
@@ -2715,15 +2715,15 @@
         cursor: XTextCursor,
         table_data: Table,
         header_bg_color: Color | None = CommonColor.DARK_BLUE,
         header_fg_color: Color | None = CommonColor.WHITE,
         tbl_bg_color: Color | None = CommonColor.LIGHT_BLUE,
         tbl_fg_color: Color | None = CommonColor.BLACK,
         first_row_header: bool = True,
-        styles: Iterable[StyleObj] = None,
+        styles: Sequence[StyleObj] = None,
     ) -> XTextTable:
         """
         Adds a table.
 
         Each row becomes a row of the table. The first row is treated as a header.
 
         Args:
@@ -2734,15 +2734,15 @@
             header_fg_color (:py:data:`~.utils.color.Color`, optional): Table header foreground color.
                 Set to None to ignore header color. Defaults to ``CommonColor.WHITE``.
             tbl_bg_color (:py:data:`~.utils.color.Color`, optional): Table background color.
                 Set to None to ignore background color. Defaults to ``CommonColor.LIGHT_BLUE``.
             tbl_fg_color (:py:data:`~.utils.color.Color`, optional): Table background color.
                 Set to None to ignore background color. Defaults to ``CommonColor.BLACK``.
             first_row_header (bool, optional): If ``True`` First row is treated as header data. Default ``True``.
-            styles (Iterable[StyleObj], optional): One or more styles to apply to frame.
+            styles (Sequence[StyleObj], optional): One or more styles to apply to frame.
                 Only styles that support ``com.sun.star.text.TextTable`` service are applied.
 
         Raises:
             ValueError: If table_data is empty
             CreateInstanceMsfError: If unable to create instance of text.TextTable
             Exception: If unable to add table
 
@@ -2890,15 +2890,15 @@
             fnm (PathOrStr): Image path
 
         Returns:
             bool: True if image link is added; Otherwise, False
         """
         ...
 
-    # style: Iterable[StyleObj] = None
+    # style: Sequence[StyleObj] = None
     @overload
     @classmethod
     def add_image_link(
         cls, doc: XTextDocument, cursor: XTextCursor, fnm: PathOrStr, width: int | UnitObj, height: int | UnitObj
     ) -> XTextContent | None:
         """
         Add Image Link
@@ -2918,24 +2918,24 @@
     @classmethod
     def add_image_link(
         cls,
         doc: XTextDocument,
         cursor: XTextCursor,
         fnm: PathOrStr,
         *,
-        styles: Iterable[StyleObj],
+        styles: Sequence[StyleObj],
     ) -> XTextContent | None:
         """
         Add Image Link
 
         Args:
             doc (XTextDocument): Text Document
             cursor (XTextCursor): Text Cursor
             fnm (PathOrStr): Image path
-            styles (Iterable[StyleObj]): One or more styles to apply to frame. Only styles that support ``com.sun.star.text.TextGraphicObject`` service are applied.
+            styles (Sequence[StyleObj]): One or more styles to apply to frame. Only styles that support ``com.sun.star.text.TextGraphicObject`` service are applied.
 
         Returns:
             XTextContent: Image Link on success; Otherwise, ``None``
         """
         ...
 
     @overload
@@ -2943,26 +2943,26 @@
     def add_image_link(
         cls,
         doc: XTextDocument,
         cursor: XTextCursor,
         fnm: PathOrStr,
         width: int | UnitObj,
         height: int | UnitObj,
-        styles: Iterable[StyleObj],
+        styles: Sequence[StyleObj],
     ) -> XTextContent | None:
         """
         Add Image Link
 
         Args:
             doc (XTextDocument): Text Document
             cursor (XTextCursor): Text Cursor
             fnm (PathOrStr): Image path
             width (int, UnitObj): Width in ``1/100th mm`` or ``UnitObj``.
             height (int, UnitObj): Height in ``1/100th mm`` or ``UnitObj``.
-            styles (Iterable[StyleObj]): One or more styles to apply to frame. Only styles that support ``com.sun.star.text.TextGraphicObject`` service are applied.
+            styles (Sequence[StyleObj]): One or more styles to apply to frame. Only styles that support ``com.sun.star.text.TextGraphicObject`` service are applied.
 
         Returns:
             XTextContent: Image Link on success; Otherwise, ``None``
         """
         ...
 
     @classmethod
@@ -2970,26 +2970,26 @@
         cls,
         doc: XTextDocument,
         cursor: XTextCursor,
         fnm: PathOrStr,
         *,
         width: int | UnitObj = 0,
         height: int | UnitObj = 0,
-        styles: Iterable[StyleObj] = None,
+        styles: Sequence[StyleObj] = None,
     ) -> XTextContent | None:
         """
         Add Image Link
 
         Args:
             doc (XTextDocument): Text Document
             cursor (XTextCursor): Text Cursor
             fnm (PathOrStr): Image path
             width (int, UnitObj): Width in ``1/100th mm`` or :ref:`proto_unit_obj`.
             height (int, UnitObj): Height in ``1/100th mm`` or :ref:`proto_unit_obj`.
-            styles (Iterable[StyleObj]): One or more styles to apply to frame. Only styles that support ``com.sun.star.text.TextGraphicObject`` service are applied.
+            styles (Sequence[StyleObj]): One or more styles to apply to frame. Only styles that support ``com.sun.star.text.TextGraphicObject`` service are applied.
 
         Raises:
             CreateInstanceMsfError: If Unable to create text.TextGraphicObject
             MissingInterfaceError: If unable to obtain XPropertySet interface
             Exception: If unable to add image
 
         Returns:
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/proto/dispatch_shape.py` & `ooo_dev_tools-0.9.4/ooodev/proto/dispatch_shape.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/proto/event_observer.py` & `ooo_dev_tools-0.9.4/ooodev/proto/event_observer.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/proto/style_obj.py` & `ooo_dev_tools-0.9.4/ooodev/proto/style_obj.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/theme/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/theme/theme.py` & `ooo_dev_tools-0.9.4/ooodev/theme/theme.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/theme/theme_basic.py` & `ooo_dev_tools-0.9.4/ooodev/theme/theme_basic.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/theme/theme_calc.py` & `ooo_dev_tools-0.9.4/ooodev/theme/theme_calc.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/theme/theme_draw.py` & `ooo_dev_tools-0.9.4/ooodev/theme/theme_draw.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/theme/theme_general.py` & `ooo_dev_tools-0.9.4/ooodev/theme/theme_general.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/theme/theme_html.py` & `ooo_dev_tools-0.9.4/ooodev/theme/theme_html.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/theme/theme_rpt_builder.py` & `ooo_dev_tools-0.9.4/ooodev/theme/theme_rpt_builder.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/theme/theme_sql.py` & `ooo_dev_tools-0.9.4/ooodev/theme/theme_sql.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/theme/theme_text_doc.py` & `ooo_dev_tools-0.9.4/ooodev/theme/theme_text_doc.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/units/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/units/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 from .unit_inch100 import UnitInch100 as UnitInch100
 from .unit_inch1000 import UnitInch1000 as UnitInch1000
 from .unit_mm import UnitMM as UnitMM
 from .unit_mm10 import UnitMM10 as UnitMM10
 from .unit_mm100 import UnitMM100 as UnitMM100
 from .unit_pt import UnitPT as UnitPT
 from .unit_px import UnitPX as UnitPX
+from .unit_cm import UnitCM as UnitCM
 
 __all__ = [
     "UnitConvert",
     "UnitLength",
     "UnitObj",
     "UnitInch",
     "UnitInch10",
     "UnitInch100",
     "UnitInch1000",
     "UnitMM",
     "UnitMM10",
     "UnitMM100",
     "UnitPT",
     "UnitPX",
+    "UnitCM",
 ]
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/units/unit_convert.py` & `ooo_dev_tools-0.9.4/ooodev/units/unit_convert.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/units/unit_inch.py` & `ooo_dev_tools-0.9.4/ooodev/units/unit_inch.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,23 @@
         :ref:`proto_unit_obj`
     """
 
     def __post_init__(self):
         if not isinstance(self.value, float):
             object.__setattr__(self, "value", float(self.value))
 
+    def get_value_cm(self) -> float:
+        """
+        Gets instance value converted to ``cm`` units.
+
+        Returns:
+            int: Value in ``cm`` units.
+        """
+        return UnitConvert.convert(num=self.value, frm=UnitLength.IN, to=UnitLength.CM)
+
     def get_value_pt(self) -> float:
         """
         Gets instance value converted to Size in ``pt`` (points) units.
 
         Returns:
             int: Value in ``pt`` units.
         """
@@ -126,39 +135,54 @@
         Args:
             value (int): ``1/10th in`` value.
 
         Returns:
             UnitInch:
         """
         inst = super(UnitInch, cls).__new__(cls)
-        inst.__init__(round(UnitConvert.convert(num=value, frm=UnitLength.IN10, to=UnitLength.IN)))
+        inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.IN10, to=UnitLength.IN))
         return inst
 
     @classmethod
     def from_inch100(cls: Type[_TUnitInch], value: float) -> _TUnitInch:
         """
         Get instance from ``1/100th in`` (inch) value.
 
         Args:
             value (int): ``1/100th in`` value.
 
         Returns:
             UnitInch:
         """
         inst = super(UnitInch, cls).__new__(cls)
-        inst.__init__(round(UnitConvert.convert(num=value, frm=UnitLength.IN100, to=UnitLength.IN)))
+        inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.IN100, to=UnitLength.IN))
         return inst
 
     @classmethod
     def from_inch1000(cls: Type[_TUnitInch], value: float) -> _TUnitInch:
         """
         Get instance from ``1/1,000th in`` (inch) value.
 
         Args:
             value (int): ``1/1,000th in`` value.
 
         Returns:
             UnitInch:
         """
         inst = super(UnitInch, cls).__new__(cls)
-        inst.__init__(round(UnitConvert.convert(num=value, frm=UnitLength.IN1000, to=UnitLength.IN)))
+        inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.IN1000, to=UnitLength.IN))
+        return inst
+
+    @classmethod
+    def from_cm(cls: Type[_TUnitInch], value: float) -> _TUnitInch:
+        """
+        Get instance from ``cm`` value.
+
+        Args:
+            value (float): ``cm`` value.
+
+        Returns:
+            UnitInch:
+        """
+        inst = super(UnitInch, cls).__new__(cls)
+        inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.CM, to=UnitLength.IN))
         return inst
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/units/unit_inch10.py` & `ooo_dev_tools-0.9.4/ooodev/units/unit_inch10.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,23 @@
         :ref:`proto_unit_obj`
     """
 
     def __post_init__(self):
         if not isinstance(self.value, float):
             object.__setattr__(self, "value", float(self.value))
 
+    def get_value_cm(self) -> float:
+        """
+        Gets instance value converted to ``cm`` units.
+
+        Returns:
+            int: Value in ``cm`` units.
+        """
+        return UnitConvert.convert(num=self.value, frm=UnitLength.IN10, to=UnitLength.CM)
+
     def get_value_mm(self) -> float:
         """
         Gets instance value converted to ``mm`` units.
 
         Returns:
             int: Value in ``mm`` units.
         """
@@ -141,24 +150,39 @@
         Args:
             value (int): ``1/100th in`` value.
 
         Returns:
             UnitInch10:
         """
         inst = super(UnitInch10, cls).__new__(cls)
-        inst.__init__(round(UnitConvert.convert(num=value, frm=UnitLength.IN100, to=UnitLength.IN10)))
+        inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.IN100, to=UnitLength.IN10))
         return inst
 
     @classmethod
     def from_inch1000(cls: Type[_TUnitInch10], value: float) -> _TUnitInch10:
         """
         Get instance from ``1/1,000th in`` (inch) value.
 
         Args:
             value (int): ``1/1,000th in`` value.
 
         Returns:
             UnitInch10:
         """
         inst = super(UnitInch10, cls).__new__(cls)
-        inst.__init__(round(UnitConvert.convert(num=value, frm=UnitLength.IN1000, to=UnitLength.IN10)))
+        inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.IN1000, to=UnitLength.IN10))
+        return inst
+
+    @classmethod
+    def from_cm(cls: Type[_TUnitInch10], value: float) -> _TUnitInch10:
+        """
+        Get instance from ``cm`` value.
+
+        Args:
+            value (float): ``cm`` value.
+
+        Returns:
+            UnitInch10:
+        """
+        inst = super(UnitInch10, cls).__new__(cls)
+        inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.CM, to=UnitLength.IN10))
         return inst
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/units/unit_inch100.py` & `ooo_dev_tools-0.9.4/ooodev/units/unit_inch100.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,23 @@
         :ref:`proto_unit_obj`
     """
 
     def __post_init__(self):
         if not isinstance(self.value, float):
             object.__setattr__(self, "value", float(self.value))
 
+    def get_value_cm(self) -> float:
+        """
+        Gets instance value converted to ``cm`` units.
+
+        Returns:
+            int: Value in ``cm`` units.
+        """
+        return UnitConvert.convert(num=self.value, frm=UnitLength.IN100, to=UnitLength.CM)
+
     def get_value_mm(self) -> float:
         """
         Gets instance value converted to Size in ``mm`` units.
 
         Returns:
             int: Value in ``mm`` units.
         """
@@ -158,7 +167,22 @@
 
         Returns:
             UnitInch100:
         """
         inst = super(UnitInch100, cls).__new__(cls)
         inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.IN1000, to=UnitLength.IN100))
         return inst
+
+    @classmethod
+    def from_cm(cls: Type[_TUnitInch100], value: float) -> _TUnitInch100:
+        """
+        Get instance from ``cm`` value.
+
+        Args:
+            value (float): ``cm`` value.
+
+        Returns:
+            UnitInch100:
+        """
+        inst = super(UnitInch100, cls).__new__(cls)
+        inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.CM, to=UnitLength.IN100))
+        return inst
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/units/unit_inch1000.py` & `ooo_dev_tools-0.9.4/ooodev/units/unit_inch1000.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,23 @@
         # I suspect this is due to this class being a dataclass.
         try:
             i = int(other)
             return i == self.value
         except Exception as e:
             return False
 
+    def get_value_cm(self) -> float:
+        """
+        Gets instance value converted to ``cm`` units.
+
+        Returns:
+            int: Value in ``cm`` units.
+        """
+        return UnitConvert.convert(num=self.value, frm=UnitLength.IN1000, to=UnitLength.CM)
+
     def get_value_mm(self) -> float:
         """
         Gets instance value converted to ``mm`` units.
 
         Returns:
             int: Value in ``mm`` units.
         """
@@ -172,7 +181,22 @@
 
         Returns:
             UnitInch1000:
         """
         inst = super(UnitInch1000, cls).__new__(cls)
         inst.__init__(value)
         return inst
+
+    @classmethod
+    def from_cm(cls: Type[_TUnitInch1000], value: float) -> _TUnitInch1000:
+        """
+        Get instance from ``cm`` value.
+
+        Args:
+            value (int): ``cm`` value.
+
+        Returns:
+            UnitInch1000:
+        """
+        inst = super(UnitInch1000, cls).__new__(cls)
+        inst.__init__(round(UnitConvert.convert(num=value, frm=UnitLength.CM, to=UnitLength.IN1000)))
+        return inst
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/units/unit_mm.py` & `ooo_dev_tools-0.9.4/ooodev/units/unit_mm.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,23 @@
         :ref:`proto_unit_obj`
     """
 
     def __post_init__(self):
         if not isinstance(self.value, float):
             object.__setattr__(self, "value", float(self.value))
 
+    def get_value_cm(self) -> float:
+        """
+        Gets instance value converted to ``cm`` units.
+
+        Returns:
+            int: Value in ``cm`` units.
+        """
+        return UnitConvert.convert(num=self.value, frm=UnitLength.MM, to=UnitLength.CM)
+
     def get_value_mm100(self) -> int:
         """
         Gets instance value converted to Size in ``1/100th mm`` units.
 
         Returns:
             int: Value in ``1/100th mm`` units.
         """
@@ -188,7 +197,22 @@
 
         Returns:
             UnitMM:
         """
         inst = super(UnitMM, cls).__new__(cls)
         inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.IN1000, to=UnitLength.MM))
         return inst
+
+    @classmethod
+    def from_cm(cls: Type[_TUnitMM], value: float) -> _TUnitMM:
+        """
+        Get instance from ``cm`` value.
+
+        Args:
+            value (int): ``cm`` value.
+
+        Returns:
+            UnitMM:
+        """
+        inst = super(UnitMM, cls).__new__(cls)
+        inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.CM, to=UnitLength.MM))
+        return inst
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/units/unit_mm10.py` & `ooo_dev_tools-0.9.4/ooodev/units/unit_mm10.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,23 @@
         :ref:`proto_unit_obj`
     """
 
     def __post_init__(self):
         if not isinstance(self.value, float):
             object.__setattr__(self, "value", float(self.value))
 
+    def get_value_cm(self) -> float:
+        """
+        Gets instance value converted to ``cm`` units.
+
+        Returns:
+            int: Value in ``cm`` units.
+        """
+        return UnitConvert.convert(num=self.value, frm=UnitLength.MM10, to=UnitLength.CM)
+
     def get_value_mm(self) -> float:
         """
         Gets instance value converted to ``mm`` units.
 
         Returns:
             int: Value in ``mm`` units.
         """
@@ -188,7 +197,22 @@
 
         Returns:
             UnitMM10:
         """
         inst = super(UnitMM10, cls).__new__(cls)
         inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.IN1000, to=UnitLength.MM10))
         return inst
+
+    @classmethod
+    def from_cm(cls: Type[_TUnitMM10], value: float) -> _TUnitMM10:
+        """
+        Get instance from ``cm`` value.
+
+        Args:
+            value (int): ``cm`` value.
+
+        Returns:
+            UnitMM10:
+        """
+        inst = super(UnitMM10, cls).__new__(cls)
+        inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.CM, to=UnitLength.MM10))
+        return inst
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/units/unit_mm100.py` & `ooo_dev_tools-0.9.4/ooodev/units/unit_mm100.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,23 @@
         # I suspect this is due to this class being a dataclass.
         try:
             i = int(other)
             return i == self.value
         except Exception as e:
             return False
 
+    def get_value_cm(self) -> float:
+        """
+        Gets instance value converted to ``cm`` units.
+
+        Returns:
+            int: Value in ``cm`` units.
+        """
+        return UnitConvert.convert(num=self.value, frm=UnitLength.MM100, to=UnitLength.CM)
+
     def get_value_mm(self) -> float:
         """
         Gets instance value converted to ``mm`` units.
 
         Returns:
             int: Value in ``mm`` units.
         """
@@ -110,15 +119,15 @@
         Args:
             value (int): ``1/100th mm`` value.
 
         Returns:
             UnitMM100:
         """
         inst = super(UnitMM100, cls).__new__(cls)
-        inst.__init__(value)
+        inst.__init__(int(value))
         return inst
 
     @classmethod
     def from_pt(cls: Type[_TUnitMM100], value: float) -> _TUnitMM100:
         """
         Get instance from ``pt`` (points) value.
 
@@ -202,7 +211,22 @@
 
         Returns:
             UnitMM100:
         """
         inst = super(UnitMM100, cls).__new__(cls)
         inst.__init__(round(UnitConvert.convert(num=value, frm=UnitLength.IN1000, to=UnitLength.MM100)))
         return inst
+
+    @classmethod
+    def from_cm(cls: Type[_TUnitMM100], value: float) -> _TUnitMM100:
+        """
+        Get instance from ``cm`` value.
+
+        Args:
+            value (int): ``cm`` value.
+
+        Returns:
+            UnitMM100:
+        """
+        inst = super(UnitMM100, cls).__new__(cls)
+        inst.__init__(round(UnitConvert.convert(num=value, frm=UnitLength.CM, to=UnitLength.MM100)))
+        return inst
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/units/unit_obj.py` & `ooo_dev_tools-0.9.4/ooodev/units/unit_obj.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/units/unit_pt.py` & `ooo_dev_tools-0.9.4/ooodev/units/unit_pt.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,23 @@
         :ref:`proto_unit_obj`
     """
 
     def __post_init__(self) -> None:
         if not isinstance(self.value, float):
             object.__setattr__(self, "value", float(self.value))
 
+    def get_value_cm(self) -> float:
+        """
+        Gets instance value converted to ``cm`` units.
+
+        Returns:
+            int: Value in ``cm`` units.
+        """
+        return UnitConvert.convert(num=self.value, frm=UnitLength.PT, to=UnitLength.CM)
+
     def get_value_mm(self) -> float:
         """
         Gets instance value converted to ``mm`` units.
 
         Returns:
             int: Value in ``mm`` units.
         """
@@ -179,7 +188,22 @@
 
         Returns:
             UnitPT:
         """
         inst = super(UnitPT, cls).__new__(cls)
         inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.IN1000, to=UnitLength.PT))
         return inst
+
+    @classmethod
+    def from_cm(cls: Type[_TUnitPT], value: float) -> _TUnitPT:
+        """
+        Get instance from ``cm`` value.
+
+        Args:
+            value (int): ``cm`` value.
+
+        Returns:
+            UnitPT:
+        """
+        inst = super(UnitPT, cls).__new__(cls)
+        inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.CM, to=UnitLength.PT))
+        return inst
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/units/unit_px.py` & `ooo_dev_tools-0.9.4/ooodev/units/unit_px.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,23 @@
         :ref:`proto_unit_obj`
     """
 
     def __post_init__(self) -> None:
         if not isinstance(self.value, float):
             object.__setattr__(self, "value", float(self.value))
 
+    def get_value_cm(self) -> float:
+        """
+        Gets instance value converted to ``cm`` units.
+
+        Returns:
+            int: Value in ``cm`` units.
+        """
+        return UnitConvert.convert(num=self.value, frm=UnitLength.PX, to=UnitLength.CM)
+
     def get_value_mm(self) -> float:
         """
         Gets instance value converted to ``mm`` units.
 
         Returns:
             int: Value in ``mm`` units.
         """
@@ -188,7 +197,22 @@
 
         Returns:
             UnitPX:
         """
         inst = super(UnitPX, cls).__new__(cls)
         inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.IN1000, to=UnitLength.PX))
         return inst
+
+    @classmethod
+    def from_cm(cls: Type[_TUnitPX], value: float) -> _TUnitPX:
+        """
+        Get instance from ``cm`` value.
+
+        Args:
+            value (int): ``cm`` value.
+
+        Returns:
+            UnitPX:
+        """
+        inst = super(UnitPX, cls).__new__(cls)
+        inst.__init__(UnitConvert.convert(num=value, frm=UnitLength.CM, to=UnitLength.PX))
+        return inst
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/__init__.py` & `ooo_dev_tools-0.9.4/ooodev/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/color.py` & `ooo_dev_tools-0.9.4/ooodev/utils/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/angle.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/angle.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/base_float_value.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/base_float_value.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/base_int_value.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/base_int_value.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/byte.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/byte.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/byte_signed.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/byte_signed.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/cell_obj.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/cell_obj.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/cell_values.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/cell_values.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/col_obj.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/col_obj.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/color_range.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/color_range.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/image_offset.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/image_offset.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/intensity.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/intensity.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/intensity_range.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/intensity_range.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/poly_sides.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/poly_sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/range_obj.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/range_obj.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/range_values.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/range_values.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/row_obj.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/row_obj.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/size.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/size.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/size_mm.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/size_mm.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/width_height_fraction.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/width_height_fraction.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/data_type/width_height_percent.py` & `ooo_dev_tools-0.9.4/ooodev/utils/data_type/width_height_percent.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/date_time_util.py` & `ooo_dev_tools-0.9.4/ooodev/utils/date_time_util.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/decorator/enforce.py` & `ooo_dev_tools-0.9.4/ooodev/utils/decorator/enforce.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/dialogs.py` & `ooo_dev_tools-0.9.4/ooodev/utils/dialogs.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/dispatch/draw_drawing_dispatch.py` & `ooo_dev_tools-0.9.4/ooodev/utils/dispatch/draw_drawing_dispatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/dispatch/draw_view_dispatch.py` & `ooo_dev_tools-0.9.4/ooodev/utils/dispatch/draw_view_dispatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/dispatch/global_edit_dispatch.py` & `ooo_dev_tools-0.9.4/ooodev/utils/dispatch/global_edit_dispatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/dispatch/global_format_dispatch.py` & `ooo_dev_tools-0.9.4/ooodev/utils/dispatch/global_format_dispatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/dispatch/global_view_dispatch.py` & `ooo_dev_tools-0.9.4/ooodev/utils/dispatch/global_view_dispatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/dispatch/shape_dispatch_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/dispatch/shape_dispatch_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/enum_helper.py` & `ooo_dev_tools-0.9.4/ooodev/utils/enum_helper.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/file_io.py` & `ooo_dev_tools-0.9.4/ooodev/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/forms.py` & `ooo_dev_tools-0.9.4/ooodev/utils/forms.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/gallery.py` & `ooo_dev_tools-0.9.4/ooodev/utils/gallery.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/gen_util.py` & `ooo_dev_tools-0.9.4/ooodev/utils/gen_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # coding: utf-8
 """General Utilities"""
 from __future__ import annotations
 import re
-from typing import Iterable, Iterator, NamedTuple, Any
+from typing import Iterable, Iterator, NamedTuple, Any, Type, TypeVar
 from inspect import isclass
 
 # match:
 #   Any uppercase character that is not at the start of a line
 #   Any Number that is preceeded by a Upper or Lower case character
 _REG_TO_SNAKE = re.compile(r"(?<!^)(?=[A-Z])|(?<=[A-zA-Z])(?=[0-9])")  # re.compile(r"(?<!^)(?=[A-Z])")
 _REG_LETTER_AFTER_NUMBER = re.compile(r"(?<=\d)(?=[a-zA-Z])")
 
 NULL_OBJ = object()
 """Null Object uses with None is not an option"""
 
+TNullObj = TypeVar("TNullObj", bound=object)
+
 
 class ArgsHelper:
     "Args Helper"
 
     class NameValue(NamedTuple):
         "Name Value pair"
         name: str
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/gui.py` & `ooo_dev_tools-0.9.4/ooodev/utils/gui.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/image_transferable.py` & `ooo_dev_tools-0.9.4/ooodev/utils/image_transferable.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/images.py` & `ooo_dev_tools-0.9.4/ooodev/utils/images.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/images_lo.py` & `ooo_dev_tools-0.9.4/ooodev/utils/images_lo.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/info.py` & `ooo_dev_tools-0.9.4/ooodev/utils/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     from com.sun.star.beans import XPropertyContainer
     from com.sun.star.document import XDocumentProperties
     from com.sun.star.reflection import XIdlMethod
 
 from ooo.dyn.beans.property_value import PropertyValue
 from ooo.dyn.beans.property_concept import PropertyConceptEnum
 from ooo.dyn.beans.the_introspection import theIntrospection
+from ooo.dyn.lang.locale import Locale  # struct
 
 from . import date_time_util as mDate
 from . import file_io as mFileIO
 from . import lo as mLo
 from . import props as mProps
 from ..units import unit_convert as mConvert
 from ..events.args.event_args import EventArgs
@@ -2229,36 +2230,97 @@
         if hasattr(obj, "__ooo_full_ns__"):
             # ooouno object
             return obj.__ooo_full_ns__
         if hasattr(obj, "__pyunointerface__"):
             return obj.__pyunointerface__
         return None
 
+    @classmethod
+    def parse_languange_code(cls, lang_code: str) -> Locale:
+        """
+        Parses a language code into a ``Locale`` object.
+
+        Args:
+            lang_code (str): Language code such as ``"en-US"``
+
+        Returns:
+            Locale: ``Locale`` object
+
+        Raises:
+            ValueError: If ``lang_code`` is not valid.
+        """
+        if not lang_code:
+            raise ValueError("lang_code cannot be empty")
+        lang_code = lang_code.lower()
+        if "-" in lang_code:
+            parts = lang_code.split("-", maxsplit=2)
+            if len(parts) == 2:
+                lang, country = parts
+                variant = ""
+            elif len(parts) == 3:
+                lang, country, variant = parts
+        else:
+            lang = lang_code
+            country = ""
+            variant = ""
+        if len(lang) != 2:
+            raise ValueError(f"Invalid language code: {lang_code}")
+        if country and len(country) != 2:
+            raise ValueError(f"Invalid country code: {lang_code}")
+        return Locale(lang, country.upper(), variant)
+
     @classproperty
     def language(cls) -> str:
         """
         Gets the Current Language of the LibreOffice Instance
 
         Returns:
-            str: First two chars of language in lower case such as 'en-US'
+            str: Language string such as 'en-US'
         """
 
         try:
             return cls._language
         except AttributeError:
-            lang = cls.get_config(node_str="ooLocale")
+            lang = cls.get_config(node_str="ooLocale", node_path="/org.openoffice.Setup/L10N")
+            if not lang:
+                lang = cls.get_config(node_str="ooSetupSystemLocale", node_path="/org.openoffice.Setup/L10N")
+            if not lang:
+                # default to en-us
+                lang = "en-US"
             cls._language = str(lang)
         return cls._language
 
     @language.setter
     def language(cls, value) -> None:
         # raise error on set. Not really necessary but gives feedback.
         raise AttributeError("Attempt to modify read-only class property '%s'." % cls.__name__)
 
     @classproperty
+    def language_locale(cls) -> Locale:
+        """
+        Gets the Current Language ``Locale`` of the LibreOffice Instance.
+
+        Returns:
+            Locale: ``Locale`` object.
+
+        .. versionadded:: 0.9.4
+        """
+
+        try:
+            return cls._language_locale
+        except AttributeError:
+            cls._language_locale = cls.parse_languange_code(cls.language)
+        return cls._language_locale
+
+    @language_locale.setter
+    def language_locale(cls, value) -> None:
+        # raise error on set. Not really necessary but gives feedback.
+        raise AttributeError("Attempt to modify read-only class property '%s'." % cls.__name__)
+
+    @classproperty
     def version(cls) -> str:
         """
         Gets the running LibreOffice version
 
         Returns:
             str: version as string such as ``"7.3.4.2"``
 
@@ -2302,15 +2364,15 @@
     def version_info(cls, value) -> None:
         # raise error on set. Not really necessary but gives feedback.
         raise AttributeError("Attempt to modify read-only class property '%s'." % cls.__name__)
 
 
 def _del_cache_attrs(source: object, e: EventArgs) -> None:
     # clears Write Attributes that are dynamically created
-    dattrs = ("_language", "_version", "_version_info")
+    dattrs = ("_language", "_language_locale", "_version", "_version_info")
     for attr in dattrs:
         if hasattr(Info, attr):
             delattr(Info, attr)
 
 
 # subscribe to events that warrant clearing cached attribs
 _Events().on(LoNamedEvent.RESET, _del_cache_attrs)
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/axis_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/axis_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/chart2_data_role_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/chart2_data_role_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/chart2_types.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/chart2_types.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/chart_diagram_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/chart_diagram_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/curve_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/curve_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/data_point_label_type_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/data_point_label_type_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/data_point_lable_placement_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/data_point_lable_placement_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/drawing_bitmap_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/drawing_bitmap_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/drawing_gradient_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/drawing_gradient_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/drawing_hatching_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/drawing_hatching_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/drawing_layer_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/drawing_layer_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/drawing_name_space_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/drawing_name_space_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/drawing_shape_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/drawing_shape_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/drawing_slide_show_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/drawing_slide_show_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/form_component_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/form_component_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/form_control_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/form_control_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/gallery_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/gallery_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/gallery_search_by_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/gallery_search_by_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/glue_points_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/glue_points_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/graphic_arrow_style_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/graphic_arrow_style_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/graphic_style_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/graphic_style_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/info_paths_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/info_paths_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/kind_helper.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/kind_helper.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/line_style_name_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/line_style_name_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/presentation_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/presentation_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/presentation_layout_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/presentation_layout_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/search_match_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/search_match_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/kind/shape_comb_kind.py` & `ooo_dev_tools-0.9.4/ooodev/utils/kind/shape_comb_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/lo.py` & `ooo_dev_tools-0.9.4/ooodev/utils/lo.py`

 * *Files 0% similar despite different names*

```diff
@@ -2062,19 +2062,19 @@
 
         Note:
             There are many dispatch command constants that can be found in :ref:`utils_dispatch` Namespace
 
             | ``DISPATCHING`` Event args data contains any properties passed in via ``props``.
             | ``DISPATCHED`` Event args data contains any results from the dispatch commands.
 
-
         See Also:
             - :ref:`ch04_dispatching`
             - `LibreOffice Dispatch Commands <https://wiki.documentfoundation.org/Development/DispatchCommands>`_
         """
+
         if not cmd:
             raise mEx.DispatchError("cmd must not be empty or None")
         try:
             str_cmd = str(cmd)  # make sure and enum or other lookup did not get passed by mistake
             cargs = DispatchCancelArgs(Lo.dispatch_cmd.__qualname__, str_cmd)
             cargs.event_data = props
             _Events().trigger(LoNamedEvent.DISPATCHING, cargs)
@@ -2561,28 +2561,28 @@
             return False
         xmodel = cls.qi(XModel, cls._doc, True)
         xmodel.lockControllers()
         _Events().trigger(LoNamedEvent.CONTROLERS_LOCKED, EventArgs(cls))
         return True
 
     @classmethod
-    def unlock_controllers(cls) -> uno.Bool:
+    def unlock_controllers(cls) -> bool:
         """
         Resumes the notifications which were suspended by :py:meth:`~.lo.Lo.lock_controllers`.
 
         The calls to :py:meth:`~.lo.Lo.lock_controllers` and :py:meth:`~.lo.Lo.unlock_controllers`
         may be nested and even overlapping, but they must be in pairs.
         While there is at least one lock remaining, some notifications for
         display updates are not broadcast.
 
         Raises:
             MissingInterfaceError: If unable to obtain XModel interface.
 
         Returns:
-            bool: False if CONTROLERS_UNLOCKING event is canceled; Otherwise, True
+            bool: False if ``CONTROLERS_UNLOCKING`` event is canceled; Otherwise, True
 
         :events:
             .. cssclass:: lo_event
 
                 - :py:attr:`~.events.lo_named_event.LoNamedEvent.CONTROLERS_UNLOCKING` :eventref:`src-docs-event-cancel`
                 - :py:attr:`~.events.lo_named_event.LoNamedEvent.CONTROLERS_UNLOCKED` :eventref:`src-docs-event`
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/lo_util.py` & `ooo_dev_tools-0.9.4/ooodev/utils/lo_util.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/paths.py` & `ooo_dev_tools-0.9.4/ooodev/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/props.py` & `ooo_dev_tools-0.9.4/ooodev/utils/props.py`

 * *Files 2% similar despite different names*

```diff
@@ -738,28 +738,35 @@
             None:
 
         :events:
             .. cssclass:: lo_event
 
                 - :py:attr:`~.events.props_named_event.PropsNamedEvent.PROP_SETTING` :eventref:`src-docs-props-event-setting`
                 - :py:attr:`~.events.props_named_event.PropsNamedEvent.PROP_SET` :eventref:`src-docs-props-event-set`
+                - :py:attr:`~.events.props_named_event.PropsNamedEvent.PROP_SET_ERROR` :eventref:`src-docs-props-event-set-error`
 
         Note:
             If a Event is canceled then that property is not set. No error occurs.
 
             If ``MultiError`` occurs only the properties that raised an error is part of the error object.
             The remaining properties will still be set.
 
             If ``KeyValCancelArgs.default`` is set to true then property is set to Default
 
+        Note:
+            If an error occurs a ``PROP_SET_ERROR`` is raised. If the event args are set to ``cancel`` or ``handled`` then the error is ignored.
+
         See Also:
             :py:meth:`~.props.Props.set_default`
 
         .. versionchanged:: 0.9.0
             Setting ``KeyValCancelArgs.default=False`` will set a property to its default.
+
+        .. versionchanged:: 0.9.4
+            Now event is raised if a property fails to set.
         """
         if len(kwargs) == 0:
             return
         if mInfo.Info.is_type_interface(obj, "com.sun.star.beans.XPropertySet"):
             ps = cast(XPropertySet, obj)
         else:
             ps = mLo.Lo.qi(XPropertySet, obj, True)
@@ -774,35 +781,46 @@
             try:
                 if cargs.default:
                     cls.set_default(obj, cargs.key)
                 else:
                     if cargs.key == "":
                         continue
                     ps.setPropertyValue(cargs.key, cargs.value)
-            except AttributeError as e:
+            except (AttributeError, UnknownPropertyException) as e:
                 # handle a LibreOffice bug
-                if not cls._set_by_attribute(obj, cargs.key, cargs.value):
-                    errs.append(
-                        mEx.UnKnownError(
-                            f'Something went wrong. Could not find setPropertyValue attribute on property set. Tried setting "{key}" manually but failed'
-                        )
-                    )
+                try:
+                    if not cls._set_by_attribute(obj, cargs.key, cargs.value):
+                        raise e
+                except Exception as ex:
                     has_error = True
-                    errs.append(e)
+                    if type(ex).__name__ == "com.sun.star.beans.UnknownPropertyException":
+                        errs.append(mEx.PropertyNotFoundError(key, ex))
+                    else:
+                        errs.append(
+                            mEx.UnKnownError(
+                                f'Something went wrong. Could not find setPropertyValue attribute on property set. Tried setting "{key}" manually but failed'
+                            )
+                        )
 
             except PropertyVetoException as e:
                 has_error = True
                 errs.append(mEx.PropertySetError(f'Could not set readonly-property "{key}"', e))
-            except UnknownPropertyException as e:
-                has_error = True
-                errs.append(mEx.PropertyNotFoundError(key, e))
             except Exception as e:
                 has_error = True
                 errs.append(Exception(f'Could not set property "{key}"', e))
-            if not has_error:
+            if has_error:
+                error_args = KeyValCancelArgs.from_args(cargs)
+                error_args.cancel = False
+                error_args.handled = False
+                _Events().trigger(PropsNamedEvent.PROP_SET_ERROR, error_args)
+                if error_args.handled or error_args.cancel:
+                    # remove the last error
+                    if errs:
+                        _ = errs.pop()
+            else:
                 _Events().trigger(PropsNamedEvent.PROP_SET, KeyValArgs.from_args(cargs))
         if len(errs) > 0:
             raise mEx.MultiError(errs)
 
     @classmethod
     def set_default(cls, obj: object, *prop_names: str) -> None:
         """
@@ -820,38 +838,54 @@
             None:
 
         :events:
             .. cssclass:: lo_event
 
                 - :py:attr:`~.events.props_named_event.PropsNamedEvent.PROP_DEFAULT_SETTING` :eventref:`src-docs-event-cancel`
                 - :py:attr:`~.events.props_named_event.PropsNamedEvent.PROP_DEFAULT_SET` :eventref:`src-docs-event`
+                - :py:attr:`~.events.props_named_event.PropsNamedEvent.PROP_SET_DEFAULT_ERROR` :eventref:`src-docs-event-cancel`
 
         Note:
+            Event data  is a dictionary of ``{"obj": obj, "name": name}`` with name being the property name currently being set.
+
             If a Event is canceled then that property is not set. No error occurs.
 
             If ``MultiError`` occurs only the properties that raised an error is part of the error object.
             The remaining properties will still be set to default.
 
         .. versionadded:: 0.9.0
+
+        .. versionchanged:: 0.9.4
+            Now event is raised if a property fails to set default.
         """
         ps = mLo.Lo.qi(XPropertyState, obj, True)
         errs = []
         for name in prop_names:
             has_error = False
             cargs = CancelEventArgs(Props.set.__qualname__)
-            cargs.event_data = name
+            cargs.event_data = {"obj": obj, "name": name}
             _Events().trigger(PropsNamedEvent.PROP_DEFAULT_SETTING, cargs)
             if cargs.cancel:
                 continue
+            prop_name = cargs.event_data["name"]
             try:
-                ps.setPropertyToDefault(name)
+                ps.setPropertyToDefault(prop_name)
             except Exception as e:
                 has_error = True
-                errs.append(Exception(f'Could not set property Default "{name}"', e))
-            if not has_error:
+                errs.append(Exception(f'Could not set property Default "{prop_name}"', e))
+            if has_error:
+                error_args = CancelEventArgs.from_args(cargs)
+                cargs.cancel = False
+                cargs.handled = False
+                _Events().trigger(PropsNamedEvent.PROP_SET_DEFAULT_ERROR, error_args)
+                if error_args.handled or error_args.cancel:
+                    # remove the last error
+                    if errs:
+                        _ = errs.pop()
+            else:
                 _Events().trigger(PropsNamedEvent.PROP_DEFAULT_SET, EventArgs.from_args(cargs))
         if len(errs) > 0:
             raise mEx.MultiError(errs)
 
     # endregion ---------------- set properties -----------------------
 
     # region ------------------- get properties ------------------------
@@ -918,36 +952,47 @@
         try:
             if mInfo.Info.is_type_interface(obj, "com.sun.star.beans.XPropertySet"):
                 ps = cast(XPropertySet, obj)
             else:
                 ps = mLo.Lo.qi(XPropertySet, obj, True)
             try:
                 val = ps.getPropertyValue(name)
-            except AttributeError as e:
+            except (AttributeError, UnknownPropertyException) as e:
                 # handle a LibreOffice bug
-                success, val = cls._get_by_attribute(ps, name)
+                success = False
+                try:
+                    success, val = cls._get_by_attribute(ps, name)
+                except Exception as ex:
+                    if type(e).__name__ == "com.sun.star.beans.UnknownPropertyException":
+                        raise e
+                    raise mEx.UnKnownError(
+                        f'Something went wrong. Could not find getPropertyValue attribute on property set. Tried getting "{name}" manually but failed.'
+                    ) from ex
+
                 if not success:
+                    if type(e).__name__ == "com.sun.star.beans.UnknownPropertyException":
+                        raise e
                     raise mEx.UnKnownError(
                         f'Something went wrong. Could not find getPropertyValue attribute on property set. Tried getting "{name}" manually but failed.'
                     )
             # it is perfeclty fine for a property to have a value of None
             if val is None and default is not gUtil.NULL_OBJ:
                 return default
             return val
         except UnknownPropertyException:
             # the property name is not in the property set
             if default is not gUtil.NULL_OBJ:
                 return default
             raise mEx.PropertyNotFoundError(name)
         except mEx.UnKnownError:
             raise
-        except Exception as e:
+        except Exception as exx:
             if default is not gUtil.NULL_OBJ:
                 return default
-            raise mEx.PropertyError(f'Error getting property: "{name}"') from e
+            raise mEx.PropertyError(f'Error getting property: "{name}"') from exx
 
     # endregion get()
 
     # region    get_property()
     @overload
     @classmethod
     def get_property(cls, obj: object, name: str) -> object:
@@ -1459,15 +1504,20 @@
 
         Returns:
             bool: True if obj contains Property that matches name; Otherwise, False
         """
         prop_set = mLo.Lo.qi(XPropertySet, obj)
         if prop_set is None:
             return False
-        return prop_set.getPropertySetInfo().hasPropertyByName(name)
+        try:
+            return prop_set.getPropertySetInfo().hasPropertyByName(name)
+        except AttributeError:
+            # some object such as a chart data point seem to not properly implement XPropertySet
+            # and does not have a getPropertySetInfo() method
+            return hasattr(obj, name)
 
     has_property = has
 
     @classmethod
     def show_doc_type_props(cls, type: str) -> None:
         """
         Prints doc type info to console
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/script_context.py` & `ooo_dev_tools-0.9.4/ooodev/utils/script_context.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/selection.py` & `ooo_dev_tools-0.9.4/ooodev/utils/selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,14 @@
         i = 0
         if o_sel.isCollapsed():
             return i
         o_text = mLo.Lo.qi(XText, text_doc, True)
         l_cursor = cls.get_left_cursor(o_sel=o_sel, o_text=o_text)
         r_cursor = cls.get_right_cursor(o_sel=o_sel, o_text=o_text)
         if cls.compare_cursor_ends(c1=l_cursor, c2=r_cursor) < cls.CompareEnum.EQUAL:
-
             while cls.compare_cursor_ends(c1=l_cursor, c2=r_cursor) != cls.CompareEnum.EQUAL:
                 l_cursor.goRight(1, False)
                 i += 1
         return i
 
     # region ------------- model cursor methods ------------------------
 
@@ -657,20 +656,19 @@
         Returns:
             int: The number of words
         """
         if word_type is None:
             word_type = WordTypeEnum.WORD_COUNT
         # https://forum.openoffice.org/en/forum/viewtopic.php?f=20&t=82678
         next_wd = Boundary()
-        local = Locale()
-        # local.Language = "en"
-        if locale_lang is None:
-            local.Language = mInfo.Info.language
+        if locale_lang:
+            local = mInfo.Info.parse_languange_code(locale_lang)
         else:
-            local.Language = locale_lang
+            local = mInfo.Info.language_locale
+
         num_words = 0
         start_pos = 0
         if word_type > WordTypeEnum.ANY_WORD:
             # intensionally pad the start and end of the string to guarantee we get the first word and clean break on last word
             st = f" {text} "
         else:
             # ANY_WORD
```

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/session.py` & `ooo_dev_tools-0.9.4/ooodev/utils/session.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/sys_info.py` & `ooo_dev_tools-0.9.4/ooodev/utils/sys_info.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/table_helper.py` & `ooo_dev_tools-0.9.4/ooodev/utils/table_helper.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/text_transferable.py` & `ooo_dev_tools-0.9.4/ooodev/utils/text_transferable.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/type_var.py` & `ooo_dev_tools-0.9.4/ooodev/utils/type_var.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/uno_const.py` & `ooo_dev_tools-0.9.4/ooodev/utils/uno_const.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/uno_enum.py` & `ooo_dev_tools-0.9.4/ooodev/utils/uno_enum.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/validation.py` & `ooo_dev_tools-0.9.4/ooodev/utils/validation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/view_state.py` & `ooo_dev_tools-0.9.4/ooodev/utils/view_state.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/utils/xml_util.py` & `ooo_dev_tools-0.9.4/ooodev/utils/xml_util.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/ooodev/wrapper/break_context.py` & `ooo_dev_tools-0.9.4/ooodev/wrapper/break_context.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/pyproject.toml` & `ooo_dev_tools-0.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ooo-dev-tools"
-version = "0.9.3"
+version = "0.9.4"
 description = "LibreOffice Developer Tools"
 license = "Apache Software License"
 readme = "README.rst"
 authors = [
     ":Barry-Thomas-Paul: Moss <bigbytetech@gmail.com>"
 ]
 keywords = ["odev", "libreoffice", "openoffice", "macro", "uno", "ooouno", "pyuno"]
@@ -50,28 +50,29 @@
 hypothesis = ">=6.56.4"
 thefuzz = ">=0.19.0"
 python-Levenshtein = ">=0.20.7"
 lo-dev-search = {version = ">=2.0.2", platform = "linux"}
 ruff = ">=0.0.254"
 black = {extras = ["d"], version = ">=23.1.0"}
 oooenv = ">=0.1.1"
+pytest-mock = ">=3.10"
 
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^5.3"
 sphinx-toolbox = ">=3.2.0"
 sphinx-tabs = ">=3.4.1"
 sphinx-rtd-dark-mode = ">=1.2.4"
 sphinx-autodoc-typehints = ">=1.19.4"
 sphinxcontrib-spelling = ">=8.0.0"
 sphinx_design = ">=0.3.0"
 sphinxcontrib-apidoc = ">=0.3.0"
 esbonio = ">=0.16.1"
 # pygls = {version = ">=0.12.4,<1.0", python = ">=3.7,<3.12"}
-sphinx-substitution-extensions = "^2022.2.16"
+sphinx-substitution-extensions = ">=2022.2.16"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
 markers = [
     "skip_headless: skips a test in headless mode",
```

### Comparing `ooo_dev_tools-0.9.3/README.rst` & `ooo_dev_tools-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.3/PKG-INFO` & `ooo_dev_tools-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooo-dev-tools
-Version: 0.9.3
+Version: 0.9.4
 Summary: LibreOffice Developer Tools
 Home-page: https://github.com/Amourspirit/python_ooo_dev_tools
 License: Apache Software License
 Keywords: odev,libreoffice,openoffice,macro,uno,ooouno,pyuno
 Author: :Barry-Thomas-Paul: Moss
 Author-email: bigbytetech@gmail.com
 Requires-Python: >=3.7,<4.0
```

