# Comparing `tmp/gehomesdk-0.5.8.tar.gz` & `tmp/gehomesdk-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gehomesdk-0.5.8.tar", last modified: Mon Jan 23 01:17:08 2023, max compression
+gzip compressed data, was "gehomesdk-0.5.9.tar", last modified: Sun Apr 23 03:33:40 2023, max compression
```

## Comparing `gehomesdk-0.5.8.tar` & `gehomesdk-0.5.9.tar`

### file list

```diff
@@ -1,329 +1,329 @@
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:08.560553 gehomesdk-0.5.8/
--rw-rw-rw-   0        0        0     1077 2021-05-17 02:36:34.000000 gehomesdk-0.5.8/LICENSE
--rw-rw-rw-   0        0        0       17 2020-12-29 21:45:43.000000 gehomesdk-0.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0    13841 2023-01-23 01:17:08.558174 gehomesdk-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0    13358 2022-08-13 17:11:40.000000 gehomesdk-0.5.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:04.389872 gehomesdk-0.5.8/gehomesdk/
--rw-rw-rw-   0        0        0      148 2023-01-23 01:07:49.000000 gehomesdk-0.5.8/gehomesdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:04.617830 gehomesdk-0.5.8/gehomesdk/clients/
--rw-rw-rw-   0        0        0      788 2022-02-19 19:34:32.000000 gehomesdk-0.5.8/gehomesdk/clients/__init__.py
--rw-rw-rw-   0        0        0      752 2021-06-26 14:57:09.000000 gehomesdk-0.5.8/gehomesdk/clients/async_helpers.py
--rw-rw-rw-   0        0        0     8590 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/clients/async_login_flows.py
--rw-rw-rw-   0        0        0    11886 2022-02-05 04:27:48.000000 gehomesdk-0.5.8/gehomesdk/clients/base_client.py
--rw-rw-rw-   0        0        0     1290 2022-02-05 05:12:15.000000 gehomesdk-0.5.8/gehomesdk/clients/const.py
--rw-rw-rw-   0        0        0     4264 2021-01-10 01:53:36.000000 gehomesdk-0.5.8/gehomesdk/clients/ge_client_xmpp.py
--rw-rw-rw-   0        0        0      347 2021-01-10 00:21:42.000000 gehomesdk-0.5.8/gehomesdk/clients/states.py
--rw-rw-rw-   0        0        0    19845 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/clients/websocket_client.py
--rw-rw-rw-   0        0        0    12645 2022-02-05 04:19:17.000000 gehomesdk-0.5.8/gehomesdk/clients/xmpp_client.py
--rw-rw-rw-   0        0        0      661 2022-08-13 16:48:04.000000 gehomesdk-0.5.8/gehomesdk/entry_points.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:04.710824 gehomesdk-0.5.8/gehomesdk/erd/
--rw-rw-rw-   0        0        0      208 2021-12-11 04:47:31.000000 gehomesdk-0.5.8/gehomesdk/erd/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:04.742121 gehomesdk-0.5.8/gehomesdk/erd/converters/
--rw-rw-rw-   0        0        0      419 2022-09-04 02:27:39.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/__init__.py
--rw-rw-rw-   0        0        0     1254 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/abstract.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:04.864407 gehomesdk-0.5.8/gehomesdk/erd/converters/ac/
--rw-rw-rw-   0        0        0      639 2021-08-18 02:20:48.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/ac/__init__.py
--rw-rw-rw-   0        0        0      487 2021-08-03 18:00:00.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/ac/erd_ac_fan_setting_converter.py
--rw-rw-rw-   0        0        0      402 2021-08-03 17:57:08.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/ac/erd_ac_filter_status_converter.py
--rw-rw-rw-   0        0        0      505 2021-08-03 17:59:56.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/ac/erd_ac_operation_mode_converter.py
--rw-rw-rw-   0        0        0      414 2021-08-03 17:59:59.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/ac/erd_ac_target_temperature_converter.py
--rw-rw-rw-   0        0        0      503 2021-08-18 02:20:48.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/ac/erd_sac_available_modes_converter.py
--rw-rw-rw-   0        0        0      655 2021-08-03 18:18:36.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/ac/erd_sac_target_temperature_range_converter.py
--rw-rw-rw-   0        0        0      359 2021-08-03 17:54:35.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/ac/erd_wac_demand_response_power_converter.py
--rw-rw-rw-   0        0        0      448 2021-08-03 17:54:38.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/ac/erd_wac_demand_response_state_converter.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:05.025659 gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/
--rw-rw-rw-   0        0        0      826 2021-06-19 16:58:37.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/__init__.py
--rw-rw-rw-   0        0        0     2711 2021-08-05 20:08:00.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_cook_setting_converter.py
--rw-rw-rw-   0        0        0     1669 2021-06-16 04:35:18.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_cook_status_converter.py
--rw-rw-rw-   0        0        0      317 2021-06-13 18:48:25.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_cook_time_adjust_converter.py
--rw-rw-rw-   0        0        0     1449 2021-08-05 20:07:39.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_cook_time_min_max_converter.py
--rw-rw-rw-   0        0        0      505 2021-08-05 20:06:57.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_cook_time_remaining_converter.py
--rw-rw-rw-   0        0        0      551 2021-08-05 20:06:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_kitchen_timer_min_max_converter.py
--rw-rw-rw-   0        0        0      905 2021-08-05 20:06:33.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_microwave_min_max_converter.py
--rw-rw-rw-   0        0        0     1075 2021-08-05 20:06:04.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_precision_min_max_converter.py
--rw-rw-rw-   0        0        0      899 2021-06-16 14:29:30.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_remote_cook_mode_config_converter.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:05.086752 gehomesdk-0.5.8/gehomesdk/erd/converters/coffee_maker/
--rw-rw-rw-   0        0        0      235 2021-12-11 14:28:26.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/coffee_maker/__init__.py
--rw-rw-rw-   0        0        0     1118 2021-12-11 14:28:26.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/coffee_maker/erd_ccm_brew_settings_converter.py
--rw-rw-rw-   0        0        0      394 2021-12-11 14:28:26.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/coffee_maker/erd_ccm_brew_strength_converter.py
--rw-rw-rw-   0        0        0      948 2021-12-11 14:28:26.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/coffee_maker/erd_ccm_brew_temperature_range_converter.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:05.230553 gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/
--rw-rw-rw-   0        0        0      861 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/__init__.py
--rw-rw-rw-   0        0        0      297 2020-12-30 01:26:28.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/cycle_name_converter.py
--rw-rw-rw-   0        0        0      902 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/erd_cycle_count_converter.py
--rw-rw-rw-   0        0        0      740 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/erd_cycle_state_converter.py
--rw-rw-rw-   0        0        0      638 2021-06-19 17:35:21.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/erd_dishwasher_door_status_converter.py
--rw-rw-rw-   0        0        0      775 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/erd_error_converter.py
--rw-rw-rw-   0        0        0      851 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/erd_reminders_converter.py
--rw-rw-rw-   0        0        0     4845 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/erd_user_setting_converter.py
--rw-rw-rw-   0        0        0      712 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/operating_mode_converter.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:05.391252 gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/
--rw-rw-rw-   0        0        0      657 2021-10-08 00:57:29.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/__init__.py
--rw-rw-rw-   0        0        0      546 2021-10-08 00:56:59.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/erd_convertable_drawer_mode_converter.py
--rw-rw-rw-   0        0        0      738 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/erd_filter_status_converter.py
--rw-rw-rw-   0        0        0     1441 2021-09-11 18:16:18.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/fridge_door_status_converter.py
--rw-rw-rw-   0        0        0     1550 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/fridge_ice_bucket_status_converter.py
--rw-rw-rw-   0        0        0      938 2021-10-07 02:41:20.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/fridge_model_info_converter.py
--rw-rw-rw-   0        0        0      573 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/fridge_set_point_limits_converter.py
--rw-rw-rw-   0        0        0      582 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/fridge_set_points_converter.py
--rw-rw-rw-   0        0        0     1672 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/hot_water_status_converter.py
--rw-rw-rw-   0        0        0      822 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/ice_maker_control_status_converter.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:05.460517 gehomesdk-0.5.8/gehomesdk/erd/converters/hood/
--rw-rw-rw-   0        0        0      326 2021-08-21 02:20:56.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/hood/__init__.py
--rw-rw-rw-   0        0        0      661 2021-08-21 02:20:10.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/hood/erd_hood_fan_speed_availability_converter.py
--rw-rw-rw-   0        0        0      472 2021-08-21 02:18:59.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/hood/erd_hood_fan_speed_converter.py
--rw-rw-rw-   0        0        0      604 2021-08-21 01:47:52.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/hood/erd_hood_light_level_availability_converter.py
--rw-rw-rw-   0        0        0      484 2021-08-21 02:19:06.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/hood/erd_hood_light_level_converter.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:05.513425 gehomesdk-0.5.8/gehomesdk/erd/converters/ice_maker/
--rw-rw-rw-   0        0        0      203 2021-10-18 00:21:14.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/ice_maker/__init__.py
--rw-rw-rw-   0        0        0      391 2021-10-18 00:18:37.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/ice_maker/erd_oim_filter_status_converter.py
--rw-rw-rw-   0        0        0      483 2021-10-18 00:24:35.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/ice_maker/erd_oim_light_level_converter.py
--rw-rw-rw-   0        0        0      361 2021-10-18 00:20:13.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/ice_maker/erd_oim_status_converter.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:05.740494 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/
--rw-rw-rw-   0        0        0     1074 2021-07-21 03:46:17.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/__init__.py
--rw-rw-rw-   0        0        0      937 2021-07-08 16:46:22.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/dryness_level_converter.py
--rw-rw-rw-   0        0        0      584 2021-07-08 16:46:34.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/ecodry_status_converter.py
--rw-rw-rw-   0        0        0      508 2021-07-08 16:24:56.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/laundry_cycle_converter.py
--rw-rw-rw-   0        0        0      538 2021-07-08 18:16:25.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/laundry_door_status_converter.py
--rw-rw-rw-   0        0        0      529 2021-07-08 16:30:46.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/laundry_sub_cycle_converter.py
--rw-rw-rw-   0        0        0      580 2021-07-08 16:47:05.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/machine_state_converter.py
--rw-rw-rw-   0        0        0      502 2021-07-08 16:43:52.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/rinse_option_converter.py
--rw-rw-rw-   0        0        0     1196 2022-04-30 23:37:45.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/sheet_usage_configuration_converter.py
--rw-rw-rw-   0        0        0      986 2021-07-21 03:46:17.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/smart_dispense_converter.py
--rw-rw-rw-   0        0        0      574 2021-07-21 03:46:17.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/smart_dispense_tank_status_converter.py
--rw-rw-rw-   0        0        0      490 2021-07-08 16:39:10.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/soil_level_converter.py
--rw-rw-rw-   0        0        0      514 2021-07-08 16:45:02.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/spintime_level_converter.py
--rw-rw-rw-   0        0        0      508 2021-07-08 16:45:35.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/tank_selected_converter.py
--rw-rw-rw-   0        0        0     1022 2021-07-08 16:46:03.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/temperature_option_converter.py
--rw-rw-rw-   0        0        0      514 2021-07-08 16:51:06.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/tumble_status_converter.py
--rw-rw-rw-   0        0        0      589 2021-06-30 02:11:43.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/washtemp_level_converter.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:05.803357 gehomesdk-0.5.8/gehomesdk/erd/converters/microwave/
--rw-rw-rw-   0        0        0      323 2021-10-18 03:43:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/microwave/__init__.py
--rw-rw-rw-   0        0        0      793 2021-10-18 02:18:28.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/microwave/erd_microwave_available_modes_converter.py
--rw-rw-rw-   0        0        0     1398 2022-04-24 02:15:52.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/microwave/erd_microwave_cook_setting_converter.py
--rw-rw-rw-   0        0        0      798 2021-12-12 17:24:18.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/microwave/erd_microwave_cook_timer_converter.py
--rw-rw-rw-   0        0        0     1340 2021-12-12 17:06:01.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/microwave/erd_microwave_state_converter.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:06.007350 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/
--rw-rw-rw-   0        0        0     1199 2021-12-11 17:34:53.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/__init__.py
--rw-rw-rw-   0        0        0     1105 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/cooktop_status_converter.py
--rw-rw-rw-   0        0        0     1062 2021-09-12 02:26:03.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_available_cook_mode_converter.py
--rw-rw-rw-   0        0        0      571 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_cooktop_config_converter.py
--rw-rw-rw-   0        0        0      644 2021-08-19 23:52:33.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_extended_cook_mode_converter.py
--rw-rw-rw-   0        0        0      664 2021-12-11 17:24:55.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_oven_light_level_availability_converter.py
--rw-rw-rw-   0        0        0      494 2021-12-11 17:58:40.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_oven_light_level_converter.py
--rw-rw-rw-   0        0        0     1344 2021-08-19 21:11:03.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_oven_state_converter.py
--rw-rw-rw-   0        0        0      668 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_precision_cooking_app_probe_control_mode_converter.py
--rw-rw-rw-   0        0        0      659 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_precision_cooking_probe_battery_status_converter.py
--rw-rw-rw-   0        0        0      677 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_precision_cooking_probe_target_time_reached_converter.py
--rw-rw-rw-   0        0        0      733 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_precision_cooking_start_sous_vide_timer_active_status_converter.py
--rw-rw-rw-   0        0        0      916 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/oven_configuration_converter.py
--rw-rw-rw-   0        0        0     2098 2021-09-12 02:14:51.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/oven_cook_mode_converter.py
--rw-rw-rw-   0        0        0      504 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/oven/oven_ranges_converter.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:06.112375 gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/
--rw-rw-rw-   0        0        0      724 2021-08-05 20:08:43.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/__init__.py
--rw-rw-rw-   0        0        0     1127 2020-12-27 18:07:39.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/erd_bool_converter.py
--rw-rw-rw-   0        0        0      911 2020-12-27 18:08:19.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/erd_bytes_converter.py
--rw-rw-rw-   0        0        0     1167 2021-07-21 03:17:07.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/erd_int_converter.py
--rw-rw-rw-   0        0        0     1279 2020-12-27 18:11:14.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/erd_signed_byte_converter.py
--rw-rw-rw-   0        0        0     1145 2020-12-27 18:11:02.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/erd_string_converter.py
--rw-rw-rw-   0        0        0     2399 2022-09-04 02:27:39.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/erd_time_span_converter.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:06.260224 gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/
--rw-rw-rw-   0        0        0      646 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/__init__.py
--rw-rw-rw-   0        0        0      987 2022-08-13 16:20:42.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/erd_appliance_type_converter.py
--rw-rw-rw-   0        0        0      382 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/erd_clock_format_converter.py
--rw-rw-rw-   0        0        0      525 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/erd_end_tone_converter.py
--rw-rw-rw-   0        0        0     1085 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/erd_locked_converter.py
--rw-rw-rw-   0        0        0      422 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/erd_measurement_units_converter.py
--rw-rw-rw-   0        0        0      535 2020-12-27 16:50:31.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/erd_model_serial_converter.py
--rw-rw-rw-   0        0        0      423 2021-08-01 02:00:52.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/erd_on_off_converter.py
--rw-rw-rw-   0        0        0      467 2020-12-27 16:49:34.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/erd_software_version_converter.py
--rw-rw-rw-   0        0        0      443 2021-05-17 02:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/erd_sound_level_converter.py
--rw-rw-rw-   0        0        0      506 2021-08-10 17:18:26.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/erd_unit_type_converter.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:06.404868 gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/
--rw-rw-rw-   0        0        0      654 2021-07-09 02:55:38.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/__init__.py
--rw-rw-rw-   0        0        0      579 2021-07-08 21:27:05.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/erd_alert_settings_converter.py
--rw-rw-rw-   0        0        0      324 2021-07-08 21:27:00.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/erd_alert_state_converter.py
--rw-rw-rw-   0        0        0      423 2021-07-08 21:26:54.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/erd_filter_manual_mode_converter.py
--rw-rw-rw-   0        0        0      400 2021-07-09 02:54:54.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/erd_filter_mode_converter.py
--rw-rw-rw-   0        0        0      743 2021-07-21 03:14:09.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/erd_filter_position_converter.py
--rw-rw-rw-   0        0        0      448 2021-07-09 02:55:01.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/erd_filter_valve_state_converter.py
--rw-rw-rw-   0        0        0      432 2021-07-09 02:55:03.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/erd_leak_validity_converter.py
--rw-rw-rw-   0        0        0      358 2021-07-20 01:01:24.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/erd_waterfilter_flow_converter.py
--rw-rw-rw-   0        0        0      804 2021-07-20 01:13:48.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/erd_waterfilter_life_converter.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:06.508004 gehomesdk-0.5.8/gehomesdk/erd/converters/water_heater/
--rw-rw-rw-   0        0        0      321 2022-09-17 15:06:16.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_heater/__init__.py
--rw-rw-rw-   0        0        0      989 2022-09-17 15:06:16.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_heater/erd_waterheater_min_max_temperature.py
--rw-rw-rw-   0        0        0      495 2022-09-04 02:27:39.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_heater/erd_waterheater_mode.py
--rw-rw-rw-   0        0        0      609 2022-09-04 02:27:39.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_heater/erd_waterheater_mode_hours_remaining.py
--rw-rw-rw-   0        0        0      459 2022-09-04 20:53:15.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_heater/erd_waterheater_temperature.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:06.573148 gehomesdk-0.5.8/gehomesdk/erd/converters/water_softener/
--rw-rw-rw-   0        0        0      266 2021-12-04 20:18:35.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_softener/__init__.py
--rw-rw-rw-   0        0        0      446 2021-12-04 20:09:57.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_softener/erd_softener_error_code_converter.py
--rw-rw-rw-   0        0        0      426 2021-12-04 20:18:49.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_softener/erd_softener_salt_level_converter.py
--rw-rw-rw-   0        0        0      873 2021-12-04 20:04:15.000000 gehomesdk-0.5.8/gehomesdk/erd/converters/water_softener/erd_softener_shutoff_valve_state_converter.py
--rw-rw-rw-   0        0        0     1039 2022-09-04 02:27:39.000000 gehomesdk-0.5.8/gehomesdk/erd/erd_code_class.py
--rw-rw-rw-   0        0        0    13726 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/erd_codes.py
--rw-rw-rw-   0        0        0    28490 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/erd_configuration.py
--rw-rw-rw-   0        0        0      218 2021-12-11 04:31:01.000000 gehomesdk-0.5.8/gehomesdk/erd/erd_data_type.py
--rw-rw-rw-   0        0        0     5162 2023-01-23 01:12:08.000000 gehomesdk-0.5.8/gehomesdk/erd/erd_encoder.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:06.579196 gehomesdk-0.5.8/gehomesdk/erd/values/
--rw-rw-rw-   0        0        0      360 2022-09-04 02:27:39.000000 gehomesdk-0.5.8/gehomesdk/erd/values/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:06.636573 gehomesdk-0.5.8/gehomesdk/erd/values/ac/
--rw-rw-rw-   0        0        0       79 2021-08-05 18:46:56.000000 gehomesdk-0.5.8/gehomesdk/erd/values/ac/__init__.py
--rw-rw-rw-   0        0        0      855 2021-08-07 00:13:47.000000 gehomesdk-0.5.8/gehomesdk/erd/values/ac/common_enums.py
--rw-rw-rw-   0        0        0      506 2021-08-08 14:50:33.000000 gehomesdk-0.5.8/gehomesdk/erd/values/ac/sac_enums.py
--rw-rw-rw-   0        0        0      323 2021-08-05 18:46:22.000000 gehomesdk-0.5.8/gehomesdk/erd/values/ac/wac_enums.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:06.818441 gehomesdk-0.5.8/gehomesdk/erd/values/advantium/
--rw-rw-rw-   0        0        0      718 2021-07-17 00:04:53.000000 gehomesdk-0.5.8/gehomesdk/erd/values/advantium/__init__.py
--rw-rw-rw-   0        0        0      539 2021-07-17 02:27:43.000000 gehomesdk-0.5.8/gehomesdk/erd/values/advantium/advantium_cook_setting.py
--rw-rw-rw-   0        0        0     1660 2021-08-07 00:14:11.000000 gehomesdk-0.5.8/gehomesdk/erd/values/advantium/advantium_enums.py
--rw-rw-rw-   0        0        0      807 2021-07-17 00:07:56.000000 gehomesdk-0.5.8/gehomesdk/erd/values/advantium/advantium_operation_mode.py
--rw-rw-rw-   0        0        0     2070 2021-07-17 02:27:38.000000 gehomesdk-0.5.8/gehomesdk/erd/values/advantium/advantium_operation_mode_mapping.py
--rw-rw-rw-   0        0        0      765 2021-06-19 16:52:09.000000 gehomesdk-0.5.8/gehomesdk/erd/values/advantium/erd_advantium_cook_setting.py
--rw-rw-rw-   0        0        0      714 2021-06-15 19:24:07.000000 gehomesdk-0.5.8/gehomesdk/erd/values/advantium/erd_advantium_cook_status.py
--rw-rw-rw-   0        0        0      568 2021-06-19 18:17:09.000000 gehomesdk-0.5.8/gehomesdk/erd/values/advantium/erd_advantium_cook_time_min_max.py
--rw-rw-rw-   0        0        0      258 2021-06-19 18:16:29.000000 gehomesdk-0.5.8/gehomesdk/erd/values/advantium/erd_advantium_kitchen_timer_min_max.py
--rw-rw-rw-   0        0        0      341 2021-06-19 18:18:28.000000 gehomesdk-0.5.8/gehomesdk/erd/values/advantium/erd_advantium_microwave_min_max.py
--rw-rw-rw-   0        0        0      422 2021-06-19 18:18:36.000000 gehomesdk-0.5.8/gehomesdk/erd/values/advantium/erd_advantium_precision_min_max.py
--rw-rw-rw-   0        0        0     5218 2021-06-16 14:28:30.000000 gehomesdk-0.5.8/gehomesdk/erd/values/advantium/erd_advantium_remote_cook_mode_config.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:06.837959 gehomesdk-0.5.8/gehomesdk/erd/values/coffee_maker/
--rw-rw-rw-   0        0        0       27 2021-12-11 14:28:26.000000 gehomesdk-0.5.8/gehomesdk/erd/values/coffee_maker/__init__.py
--rw-rw-rw-   0        0        0      836 2021-12-11 14:28:26.000000 gehomesdk-0.5.8/gehomesdk/erd/values/coffee_maker/common_enums.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:06.956449 gehomesdk-0.5.8/gehomesdk/erd/values/common/
--rw-rw-rw-   0        0        0      380 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/values/common/__init__.py
--rw-rw-rw-   0        0        0      842 2022-09-04 02:59:53.000000 gehomesdk-0.5.8/gehomesdk/erd/values/common/erd_appliance_type.py
--rw-rw-rw-   0        0        0      139 2020-12-26 14:45:00.000000 gehomesdk-0.5.8/gehomesdk/erd/values/common/erd_clock_format.py
--rw-rw-rw-   0        0        0      117 2020-12-26 14:45:46.000000 gehomesdk-0.5.8/gehomesdk/erd/values/common/erd_end_tone.py
--rw-rw-rw-   0        0        0      111 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/values/common/erd_locked.py
--rw-rw-rw-   0        0        0      102 2020-12-26 14:47:25.000000 gehomesdk-0.5.8/gehomesdk/erd/values/common/erd_measurement_units.py
--rw-rw-rw-   0        0        0      213 2021-08-07 00:14:17.000000 gehomesdk-0.5.8/gehomesdk/erd/values/common/erd_on_off.py
--rw-rw-rw-   0        0        0      116 2020-12-26 14:46:06.000000 gehomesdk-0.5.8/gehomesdk/erd/values/common/erd_present.py
--rw-rw-rw-   0        0        0      118 2020-12-26 14:45:14.000000 gehomesdk-0.5.8/gehomesdk/erd/values/common/erd_sound_level.py
--rw-rw-rw-   0        0        0      311 2021-08-10 17:21:14.000000 gehomesdk-0.5.8/gehomesdk/erd/values/common/erd_unit_type.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:07.109874 gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/
--rw-rw-rw-   0        0        0      732 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/__init__.py
--rw-rw-rw-   0        0        0      174 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/cycle_count.py
--rw-rw-rw-   0        0        0     1246 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/cycle_state_mapping.py
--rw-rw-rw-   0        0        0      814 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/erd_cycle_state.py
--rw-rw-rw-   0        0        0      527 2021-08-07 00:14:24.000000 gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/erd_dishwasher_door_status.py
--rw-rw-rw-   0        0        0      384 2021-01-04 22:51:42.000000 gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/erd_operating_mode.py
--rw-rw-rw-   0        0        0      202 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/erd_reminders.py
--rw-rw-rw-   0        0        0     1299 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/erd_user_setting.py
--rw-rw-rw-   0        0        0      152 2023-01-23 01:07:26.000000 gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/error_state.py
--rw-rw-rw-   0        0        0      515 2021-09-11 01:57:54.000000 gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/operating_mode.py
--rw-rw-rw-   0        0        0     1065 2021-01-04 22:53:18.000000 gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/operating_mode_mapping.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:07.336754 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/
--rw-rw-rw-   0        0        0      672 2021-10-08 00:53:06.000000 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/__init__.py
--rw-rw-rw-   0        0        0      380 2021-10-08 01:51:36.000000 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/erd_convertable_drawer_mode.py
--rw-rw-rw-   0        0        0      490 2021-08-07 00:15:01.000000 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/erd_door_status.py
--rw-rw-rw-   0        0        0      354 2021-07-16 00:58:21.000000 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/erd_filter_status.py
--rw-rw-rw-   0        0        0      284 2021-08-07 00:15:07.000000 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/erd_full_not_full.py
--rw-rw-rw-   0        0        0      203 2020-12-26 15:17:44.000000 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/erd_hot_water_status.py
--rw-rw-rw-   0        0        0      114 2020-12-26 15:18:04.000000 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/erd_pod_status.py
--rw-rw-rw-   0        0        0      574 2021-07-20 20:43:01.000000 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/fridge_door_status.py
--rw-rw-rw-   0        0        0      703 2020-12-28 16:02:04.000000 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/fridge_ice_bucket_status.py
--rw-rw-rw-   0        0        0      184 2020-12-29 17:47:46.000000 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/fridge_model_info.py
--rw-rw-rw-   0        0        0      158 2020-12-26 15:22:45.000000 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/fridge_set_point_limits.py
--rw-rw-rw-   0        0        0      104 2020-12-26 15:23:19.000000 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/fridge_set_points.py
--rw-rw-rw-   0        0        0      691 2020-12-29 16:37:18.000000 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/hot_water_status.py
--rw-rw-rw-   0        0        0      165 2020-12-26 15:26:00.000000 gehomesdk-0.5.8/gehomesdk/erd/values/fridge/ice_maker_control_status.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:07.404012 gehomesdk-0.5.8/gehomesdk/erd/values/hood/
--rw-rw-rw-   0        0        0      179 2021-08-21 02:16:53.000000 gehomesdk-0.5.8/gehomesdk/erd/values/hood/__init__.py
--rw-rw-rw-   0        0        0      560 2021-08-21 15:29:12.000000 gehomesdk-0.5.8/gehomesdk/erd/values/hood/common_enums.py
--rw-rw-rw-   0        0        0      522 2021-08-21 15:56:41.000000 gehomesdk-0.5.8/gehomesdk/erd/values/hood/erd_hood_fan_speed_availability.py
--rw-rw-rw-   0        0        0      384 2021-08-21 15:57:34.000000 gehomesdk-0.5.8/gehomesdk/erd/values/hood/erd_hood_light_level_availability.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:07.423430 gehomesdk-0.5.8/gehomesdk/erd/values/ice_maker/
--rw-rw-rw-   0        0        0       27 2021-10-18 00:13:39.000000 gehomesdk-0.5.8/gehomesdk/erd/values/ice_maker/__init__.py
--rw-rw-rw-   0        0        0      794 2021-10-18 00:24:03.000000 gehomesdk-0.5.8/gehomesdk/erd/values/ice_maker/common_enums.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:07.604358 gehomesdk-0.5.8/gehomesdk/erd/values/laundry/
--rw-rw-rw-   0        0        0      567 2021-07-08 17:15:12.000000 gehomesdk-0.5.8/gehomesdk/erd/values/laundry/__init__.py
--rw-rw-rw-   0        0        0      254 2021-07-08 16:52:40.000000 gehomesdk-0.5.8/gehomesdk/erd/values/laundry/dryness_level.py
--rw-rw-rw-   0        0        0      774 2021-06-30 02:11:43.000000 gehomesdk-0.5.8/gehomesdk/erd/values/laundry/dryness_level_mapping.py
--rw-rw-rw-   0        0        0      217 2021-07-08 16:25:30.000000 gehomesdk-0.5.8/gehomesdk/erd/values/laundry/ecodry_status.py
--rw-rw-rw-   0        0        0      339 2021-06-30 02:11:43.000000 gehomesdk-0.5.8/gehomesdk/erd/values/laundry/ecodry_status_mapping.py
--rw-rw-rw-   0        0        0     5942 2021-08-07 00:15:41.000000 gehomesdk-0.5.8/gehomesdk/erd/values/laundry/laundry_enums.py
--rw-rw-rw-   0        0        0      530 2021-07-08 16:26:13.000000 gehomesdk-0.5.8/gehomesdk/erd/values/laundry/machine_state.py
--rw-rw-rw-   0        0        0      856 2021-06-30 02:11:43.000000 gehomesdk-0.5.8/gehomesdk/erd/values/laundry/machine_state_mapping.py
--rw-rw-rw-   0        0        0      253 2021-07-08 16:41:48.000000 gehomesdk-0.5.8/gehomesdk/erd/values/laundry/temperature_option.py
--rw-rw-rw-   0        0        0      898 2021-06-30 02:11:43.000000 gehomesdk-0.5.8/gehomesdk/erd/values/laundry/temperature_option_mapping.py
--rw-rw-rw-   0        0        0      287 2021-07-08 16:50:43.000000 gehomesdk-0.5.8/gehomesdk/erd/values/laundry/washtemp_level.py
--rw-rw-rw-   0        0        0      784 2021-07-08 16:55:53.000000 gehomesdk-0.5.8/gehomesdk/erd/values/laundry/washtemp_level_mapping.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:07.689201 gehomesdk-0.5.8/gehomesdk/erd/values/microwave/
--rw-rw-rw-   0        0        0      220 2021-10-18 03:39:01.000000 gehomesdk-0.5.8/gehomesdk/erd/values/microwave/__init__.py
--rw-rw-rw-   0        0        0      247 2021-10-18 03:02:22.000000 gehomesdk-0.5.8/gehomesdk/erd/values/microwave/erd_microwave_available_modes.py
--rw-rw-rw-   0        0        0      242 2021-10-18 03:41:50.000000 gehomesdk-0.5.8/gehomesdk/erd/values/microwave/erd_microwave_cook_setting.py
--rw-rw-rw-   0        0        0      376 2021-12-12 17:14:52.000000 gehomesdk-0.5.8/gehomesdk/erd/values/microwave/erd_microwave_state.py
--rw-rw-rw-   0        0        0      912 2021-12-12 17:13:53.000000 gehomesdk-0.5.8/gehomesdk/erd/values/microwave/microwave_enums.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:08.093742 gehomesdk-0.5.8/gehomesdk/erd/values/oven/
--rw-rw-rw-   0        0        0     1272 2021-12-11 17:31:40.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/__init__.py
--rw-rw-rw-   0        0        0      233 2020-12-26 15:08:43.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/available_cook_mode.py
--rw-rw-rw-   0        0        0     1158 2020-12-29 18:37:42.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/burner.py
--rw-rw-rw-   0        0        0     1264 2021-08-19 23:56:38.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/const.py
--rw-rw-rw-   0        0        0     1485 2020-12-29 19:04:34.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/cooktop_status.py
--rw-rw-rw-   0        0        0     7538 2021-09-12 02:28:00.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_available_cook_mode.py
--rw-rw-rw-   0        0        0      239 2020-12-27 05:55:10.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_closed_loop_cooking_configuration.py
--rw-rw-rw-   0        0        0     2057 2020-12-27 05:55:20.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_closed_loop_cooking_devices_status.py
--rw-rw-rw-   0        0        0      285 2020-12-26 16:43:26.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_cooktop_config.py
--rw-rw-rw-   0        0        0      112 2020-12-27 02:12:53.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_cooktop_status.py
--rw-rw-rw-   0        0        0      368 2021-08-19 23:48:09.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_extended_cook_mode.py
--rw-rw-rw-   0        0        0      251 2020-12-26 15:10:14.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_oven_configuration.py
--rw-rw-rw-   0        0        0     2179 2021-09-11 16:41:41.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_oven_cook_mode.py
--rw-rw-rw-   0        0        0      320 2021-12-11 17:30:12.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_oven_light_level.py
--rw-rw-rw-   0        0        0      465 2021-12-12 01:07:17.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_oven_light_level_availability.py
--rw-rw-rw-   0        0        0     2391 2021-08-19 21:09:42.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_oven_state.py
--rw-rw-rw-   0        0        0      135 2020-12-27 05:20:05.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_precision_cooking_app_probe_control_mode.py
--rw-rw-rw-   0        0        0      122 2020-12-27 04:46:36.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_precision_cooking_probe_battery_status.py
--rw-rw-rw-   0        0        0      231 2020-12-27 05:55:42.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_precision_cooking_probe_target_time_reached.py
--rw-rw-rw-   0        0        0      145 2020-12-27 01:14:52.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_precision_cooking_start_sous_vide_timer_active_status.py
--rw-rw-rw-   0        0        0      319 2020-12-26 15:10:51.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/oven_configuration.py
--rw-rw-rw-   0        0        0      346 2020-12-26 15:04:29.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/oven_cook_mode.py
--rw-rw-rw-   0        0        0     7341 2021-09-11 16:41:13.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/oven_cook_mode_mapping.py
--rw-rw-rw-   0        0        0     1700 2021-09-11 16:27:29.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/oven_cook_setting.py
--rw-rw-rw-   0        0        0     2990 2021-08-20 00:19:46.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/oven_display_state_mapping.py
--rw-rw-rw-   0        0        0       98 2020-12-26 15:04:53.000000 gehomesdk-0.5.8/gehomesdk/erd/values/oven/oven_ranges.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:08.235646 gehomesdk-0.5.8/gehomesdk/erd/values/water_filter/
--rw-rw-rw-   0        0        0      581 2021-07-08 21:45:12.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_filter/__init__.py
--rw-rw-rw-   0        0        0      374 2021-06-30 17:14:52.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_filter/erd_waterfilter_alert_settings.py
--rw-rw-rw-   0        0        0      913 2021-07-09 03:25:38.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_filter/erd_waterfilter_alert_state.py
--rw-rw-rw-   0        0        0      204 2021-07-09 03:25:45.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_filter/erd_waterfilter_flowrate.py
--rw-rw-rw-   0        0        0      238 2021-08-07 00:16:11.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_filter/erd_waterfilter_leak_validity.py
--rw-rw-rw-   0        0        0      252 2021-07-20 01:12:34.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_filter/erd_waterfilter_life.py
--rw-rw-rw-   0        0        0      336 2021-08-07 00:16:20.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_filter/erd_waterfilter_manual_mode.py
--rw-rw-rw-   0        0        0      328 2021-07-16 00:58:21.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_filter/erd_waterfilter_mode.py
--rw-rw-rw-   0        0        0      256 2021-07-08 21:28:04.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_filter/erd_waterfilter_position.py
--rw-rw-rw-   0        0        0      314 2021-07-08 21:28:08.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_filter/erd_waterfilter_valve_state.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:08.322919 gehomesdk-0.5.8/gehomesdk/erd/values/water_heater/
--rw-rw-rw-   0        0        0      371 2022-09-17 15:06:16.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_heater/__init__.py
--rw-rw-rw-   0        0        0      117 2022-09-17 15:06:16.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_heater/erd_waterheater_min_max_temperature.py
--rw-rw-rw-   0        0        0      380 2022-09-04 02:27:39.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_heater/erd_waterheater_mode.py
--rw-rw-rw-   0        0        0      193 2022-09-04 02:27:39.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_heater/erd_waterheater_mode_hours_remaining.py
--rw-rw-rw-   0        0        0      207 2022-09-04 02:27:39.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_heater/erd_waterheater_set_temperature.py
--rw-rw-rw-   0        0        0      210 2022-09-04 02:27:39.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_heater/erd_waterheater_target_temperature.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:08.387192 gehomesdk-0.5.8/gehomesdk/erd/values/water_softener/
--rw-rw-rw-   0        0        0      224 2021-12-04 20:17:44.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_softener/__init__.py
--rw-rw-rw-   0        0        0      545 2021-12-04 19:31:11.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_softener/erd_watersoftener_error_code.py
--rw-rw-rw-   0        0        0      329 2021-12-04 20:17:05.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_softener/erd_watersoftener_salt_level.py
--rw-rw-rw-   0        0        0      274 2021-12-04 19:44:04.000000 gehomesdk-0.5.8/gehomesdk/erd/values/water_softener/erd_watersoftener_shutoff_valve_state.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:08.555068 gehomesdk-0.5.8/gehomesdk/exception/
--rw-rw-rw-   0        0        0      643 2021-05-17 02:50:39.000000 gehomesdk-0.5.8/gehomesdk/exception/__init__.py
--rw-rw-rw-   0        0        0      153 2020-12-27 18:53:39.000000 gehomesdk-0.5.8/gehomesdk/exception/ge_auth_failed_error.py
--rw-rw-rw-   0        0        0      154 2020-12-27 18:54:19.000000 gehomesdk-0.5.8/gehomesdk/exception/ge_client_disconnected_error.py
--rw-rw-rw-   0        0        0      174 2021-01-08 02:28:45.000000 gehomesdk-0.5.8/gehomesdk/exception/ge_duplicate_appliance_error.py
--rw-rw-rw-   0        0        0       95 2020-12-27 15:39:37.000000 gehomesdk-0.5.8/gehomesdk/exception/ge_exception.py
--rw-rw-rw-   0        0        0      166 2020-12-27 18:58:18.000000 gehomesdk-0.5.8/gehomesdk/exception/ge_general_server_error.py
--rw-rw-rw-   0        0        0      159 2021-01-08 01:42:19.000000 gehomesdk-0.5.8/gehomesdk/exception/ge_needs_reauthentication_error.py
--rw-rw-rw-   0        0        0      157 2020-12-27 18:53:12.000000 gehomesdk-0.5.8/gehomesdk/exception/ge_not_authenticated_error.py
--rw-rw-rw-   0        0        0      516 2021-01-04 01:56:47.000000 gehomesdk-0.5.8/gehomesdk/exception/ge_request_error.py
--rw-rw-rw-   0        0        0      445 2020-12-27 15:48:13.000000 gehomesdk-0.5.8/gehomesdk/exception/ge_set_erd_not_allowed_error.py
--rw-rw-rw-   0        0        0      166 2020-12-27 15:42:50.000000 gehomesdk-0.5.8/gehomesdk/exception/ge_unsupported_operation_error.py
--rw-rw-rw-   0        0        0     2113 2022-08-13 16:41:20.000000 gehomesdk-0.5.8/gehomesdk/gather_data.py
--rw-rw-rw-   0        0        0     8656 2021-12-12 00:03:38.000000 gehomesdk-0.5.8/gehomesdk/ge_appliance.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:17:04.481393 gehomesdk-0.5.8/gehomesdk.egg-info/
--rw-rw-rw-   0        0        0    13841 2023-01-23 01:17:04.000000 gehomesdk-0.5.8/gehomesdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    16222 2023-01-23 01:17:04.000000 gehomesdk-0.5.8/gehomesdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-23 01:17:04.000000 gehomesdk-0.5.8/gehomesdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-01-23 01:17:04.000000 gehomesdk-0.5.8/gehomesdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2023-01-23 01:17:04.000000 gehomesdk-0.5.8/gehomesdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-23 01:17:04.000000 gehomesdk-0.5.8/gehomesdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-23 01:17:08.561248 gehomesdk-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0     1550 2022-08-13 16:47:54.000000 gehomesdk-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.614214 gehomesdk-0.5.9/
+-rw-rw-rw-   0        0        0     1077 2021-05-17 02:36:34.000000 gehomesdk-0.5.9/LICENSE
+-rw-rw-rw-   0        0        0       17 2020-12-29 21:45:43.000000 gehomesdk-0.5.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    13848 2023-04-23 03:33:40.612213 gehomesdk-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0    13358 2022-08-13 17:11:40.000000 gehomesdk-0.5.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:39.936501 gehomesdk-0.5.9/gehomesdk/
+-rw-rw-rw-   0        0        0      148 2023-04-23 03:31:21.000000 gehomesdk-0.5.9/gehomesdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:39.999989 gehomesdk-0.5.9/gehomesdk/clients/
+-rw-rw-rw-   0        0        0      788 2022-02-19 19:34:32.000000 gehomesdk-0.5.9/gehomesdk/clients/__init__.py
+-rw-rw-rw-   0        0        0      773 2023-04-23 03:18:05.000000 gehomesdk-0.5.9/gehomesdk/clients/async_helpers.py
+-rw-rw-rw-   0        0        0     8590 2023-01-23 02:42:25.000000 gehomesdk-0.5.9/gehomesdk/clients/async_login_flows.py
+-rw-rw-rw-   0        0        0    12047 2023-04-23 03:24:32.000000 gehomesdk-0.5.9/gehomesdk/clients/base_client.py
+-rw-rw-rw-   0        0        0     1290 2022-02-05 05:12:15.000000 gehomesdk-0.5.9/gehomesdk/clients/const.py
+-rw-rw-rw-   0        0        0     4264 2021-01-10 01:53:36.000000 gehomesdk-0.5.9/gehomesdk/clients/ge_client_xmpp.py
+-rw-rw-rw-   0        0        0      347 2021-01-10 00:21:42.000000 gehomesdk-0.5.9/gehomesdk/clients/states.py
+-rw-rw-rw-   0        0        0    19845 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/clients/websocket_client.py
+-rw-rw-rw-   0        0        0    12645 2022-02-05 04:19:17.000000 gehomesdk-0.5.9/gehomesdk/clients/xmpp_client.py
+-rw-rw-rw-   0        0        0      661 2022-08-13 16:48:04.000000 gehomesdk-0.5.9/gehomesdk/entry_points.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.011988 gehomesdk-0.5.9/gehomesdk/erd/
+-rw-rw-rw-   0        0        0      208 2021-12-11 04:47:31.000000 gehomesdk-0.5.9/gehomesdk/erd/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.014990 gehomesdk-0.5.9/gehomesdk/erd/converters/
+-rw-rw-rw-   0        0        0      419 2022-09-04 02:27:39.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/__init__.py
+-rw-rw-rw-   0        0        0     1254 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/abstract.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.038990 gehomesdk-0.5.9/gehomesdk/erd/converters/ac/
+-rw-rw-rw-   0        0        0      639 2021-08-18 02:20:48.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/ac/__init__.py
+-rw-rw-rw-   0        0        0      487 2021-08-03 18:00:00.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/ac/erd_ac_fan_setting_converter.py
+-rw-rw-rw-   0        0        0      402 2021-08-03 17:57:08.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/ac/erd_ac_filter_status_converter.py
+-rw-rw-rw-   0        0        0      505 2021-08-03 17:59:56.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/ac/erd_ac_operation_mode_converter.py
+-rw-rw-rw-   0        0        0      414 2021-08-03 17:59:59.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/ac/erd_ac_target_temperature_converter.py
+-rw-rw-rw-   0        0        0      503 2021-08-18 02:20:48.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/ac/erd_sac_available_modes_converter.py
+-rw-rw-rw-   0        0        0      655 2021-08-03 18:18:36.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/ac/erd_sac_target_temperature_range_converter.py
+-rw-rw-rw-   0        0        0      359 2021-08-03 17:54:35.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/ac/erd_wac_demand_response_power_converter.py
+-rw-rw-rw-   0        0        0      448 2021-08-03 17:54:38.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/ac/erd_wac_demand_response_state_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.060988 gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/
+-rw-rw-rw-   0        0        0      826 2021-06-19 16:58:37.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/__init__.py
+-rw-rw-rw-   0        0        0     2711 2021-08-05 20:08:00.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_cook_setting_converter.py
+-rw-rw-rw-   0        0        0     1669 2021-06-16 04:35:18.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_cook_status_converter.py
+-rw-rw-rw-   0        0        0      317 2021-06-13 18:48:25.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_cook_time_adjust_converter.py
+-rw-rw-rw-   0        0        0     1449 2021-08-05 20:07:39.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_cook_time_min_max_converter.py
+-rw-rw-rw-   0        0        0      505 2021-08-05 20:06:57.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_cook_time_remaining_converter.py
+-rw-rw-rw-   0        0        0      551 2021-08-05 20:06:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_kitchen_timer_min_max_converter.py
+-rw-rw-rw-   0        0        0      905 2021-08-05 20:06:33.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_microwave_min_max_converter.py
+-rw-rw-rw-   0        0        0     1075 2021-08-05 20:06:04.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_precision_min_max_converter.py
+-rw-rw-rw-   0        0        0      899 2021-06-16 14:29:30.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_remote_cook_mode_config_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.068989 gehomesdk-0.5.9/gehomesdk/erd/converters/coffee_maker/
+-rw-rw-rw-   0        0        0      235 2021-12-11 14:28:26.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/coffee_maker/__init__.py
+-rw-rw-rw-   0        0        0     1118 2021-12-11 14:28:26.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/coffee_maker/erd_ccm_brew_settings_converter.py
+-rw-rw-rw-   0        0        0      394 2021-12-11 14:28:26.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/coffee_maker/erd_ccm_brew_strength_converter.py
+-rw-rw-rw-   0        0        0      948 2021-12-11 14:28:26.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/coffee_maker/erd_ccm_brew_temperature_range_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.089172 gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/
+-rw-rw-rw-   0        0        0      861 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/__init__.py
+-rw-rw-rw-   0        0        0      297 2020-12-30 01:26:28.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/cycle_name_converter.py
+-rw-rw-rw-   0        0        0      902 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/erd_cycle_count_converter.py
+-rw-rw-rw-   0        0        0      740 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/erd_cycle_state_converter.py
+-rw-rw-rw-   0        0        0      638 2021-06-19 17:35:21.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/erd_dishwasher_door_status_converter.py
+-rw-rw-rw-   0        0        0      775 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/erd_error_converter.py
+-rw-rw-rw-   0        0        0      851 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/erd_reminders_converter.py
+-rw-rw-rw-   0        0        0     4845 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/erd_user_setting_converter.py
+-rw-rw-rw-   0        0        0      712 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/operating_mode_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.111694 gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/
+-rw-rw-rw-   0        0        0      657 2021-10-08 00:57:29.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/__init__.py
+-rw-rw-rw-   0        0        0      546 2021-10-08 00:56:59.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/erd_convertable_drawer_mode_converter.py
+-rw-rw-rw-   0        0        0      738 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/erd_filter_status_converter.py
+-rw-rw-rw-   0        0        0     1441 2021-09-11 18:16:18.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/fridge_door_status_converter.py
+-rw-rw-rw-   0        0        0     1550 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/fridge_ice_bucket_status_converter.py
+-rw-rw-rw-   0        0        0      938 2021-10-07 02:41:20.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/fridge_model_info_converter.py
+-rw-rw-rw-   0        0        0      573 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/fridge_set_point_limits_converter.py
+-rw-rw-rw-   0        0        0      582 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/fridge_set_points_converter.py
+-rw-rw-rw-   0        0        0     1672 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/hot_water_status_converter.py
+-rw-rw-rw-   0        0        0      822 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/ice_maker_control_status_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.122696 gehomesdk-0.5.9/gehomesdk/erd/converters/hood/
+-rw-rw-rw-   0        0        0      326 2021-08-21 02:20:56.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/hood/__init__.py
+-rw-rw-rw-   0        0        0      661 2021-08-21 02:20:10.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/hood/erd_hood_fan_speed_availability_converter.py
+-rw-rw-rw-   0        0        0      472 2021-08-21 02:18:59.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/hood/erd_hood_fan_speed_converter.py
+-rw-rw-rw-   0        0        0      604 2021-08-21 01:47:52.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/hood/erd_hood_light_level_availability_converter.py
+-rw-rw-rw-   0        0        0      484 2021-08-21 02:19:06.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/hood/erd_hood_light_level_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.131696 gehomesdk-0.5.9/gehomesdk/erd/converters/ice_maker/
+-rw-rw-rw-   0        0        0      203 2021-10-18 00:21:14.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/ice_maker/__init__.py
+-rw-rw-rw-   0        0        0      391 2021-10-18 00:18:37.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/ice_maker/erd_oim_filter_status_converter.py
+-rw-rw-rw-   0        0        0      483 2021-10-18 00:24:35.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/ice_maker/erd_oim_light_level_converter.py
+-rw-rw-rw-   0        0        0      361 2021-10-18 00:20:13.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/ice_maker/erd_oim_status_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.171695 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/
+-rw-rw-rw-   0        0        0     1074 2021-07-21 03:46:17.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/__init__.py
+-rw-rw-rw-   0        0        0      937 2021-07-08 16:46:22.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/dryness_level_converter.py
+-rw-rw-rw-   0        0        0      584 2021-07-08 16:46:34.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/ecodry_status_converter.py
+-rw-rw-rw-   0        0        0      508 2021-07-08 16:24:56.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/laundry_cycle_converter.py
+-rw-rw-rw-   0        0        0      538 2021-07-08 18:16:25.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/laundry_door_status_converter.py
+-rw-rw-rw-   0        0        0      529 2021-07-08 16:30:46.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/laundry_sub_cycle_converter.py
+-rw-rw-rw-   0        0        0      580 2021-07-08 16:47:05.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/machine_state_converter.py
+-rw-rw-rw-   0        0        0      502 2021-07-08 16:43:52.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/rinse_option_converter.py
+-rw-rw-rw-   0        0        0     1196 2022-04-30 23:37:45.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/sheet_usage_configuration_converter.py
+-rw-rw-rw-   0        0        0      986 2021-07-21 03:46:17.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/smart_dispense_converter.py
+-rw-rw-rw-   0        0        0      574 2021-07-21 03:46:17.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/smart_dispense_tank_status_converter.py
+-rw-rw-rw-   0        0        0      490 2021-07-08 16:39:10.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/soil_level_converter.py
+-rw-rw-rw-   0        0        0      514 2021-07-08 16:45:02.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/spintime_level_converter.py
+-rw-rw-rw-   0        0        0      508 2021-07-08 16:45:35.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/tank_selected_converter.py
+-rw-rw-rw-   0        0        0     1022 2021-07-08 16:46:03.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/temperature_option_converter.py
+-rw-rw-rw-   0        0        0      514 2021-07-08 16:51:06.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/tumble_status_converter.py
+-rw-rw-rw-   0        0        0      589 2021-06-30 02:11:43.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/washtemp_level_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.184696 gehomesdk-0.5.9/gehomesdk/erd/converters/microwave/
+-rw-rw-rw-   0        0        0      323 2021-10-18 03:43:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/microwave/__init__.py
+-rw-rw-rw-   0        0        0      793 2021-10-18 02:18:28.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/microwave/erd_microwave_available_modes_converter.py
+-rw-rw-rw-   0        0        0     1398 2022-04-24 02:15:52.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/microwave/erd_microwave_cook_setting_converter.py
+-rw-rw-rw-   0        0        0      798 2021-12-12 17:24:18.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/microwave/erd_microwave_cook_timer_converter.py
+-rw-rw-rw-   0        0        0     1340 2021-12-12 17:06:01.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/microwave/erd_microwave_state_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.226701 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/
+-rw-rw-rw-   0        0        0     1199 2021-12-11 17:34:53.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/__init__.py
+-rw-rw-rw-   0        0        0     1105 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/cooktop_status_converter.py
+-rw-rw-rw-   0        0        0     1062 2021-09-12 02:26:03.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_available_cook_mode_converter.py
+-rw-rw-rw-   0        0        0      571 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_cooktop_config_converter.py
+-rw-rw-rw-   0        0        0      644 2021-08-19 23:52:33.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_extended_cook_mode_converter.py
+-rw-rw-rw-   0        0        0      664 2021-12-11 17:24:55.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_oven_light_level_availability_converter.py
+-rw-rw-rw-   0        0        0      494 2021-12-11 17:58:40.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_oven_light_level_converter.py
+-rw-rw-rw-   0        0        0     1344 2021-08-19 21:11:03.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_oven_state_converter.py
+-rw-rw-rw-   0        0        0      668 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_precision_cooking_app_probe_control_mode_converter.py
+-rw-rw-rw-   0        0        0      659 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_precision_cooking_probe_battery_status_converter.py
+-rw-rw-rw-   0        0        0      677 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_precision_cooking_probe_target_time_reached_converter.py
+-rw-rw-rw-   0        0        0      733 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_precision_cooking_start_sous_vide_timer_active_status_converter.py
+-rw-rw-rw-   0        0        0      916 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/oven_configuration_converter.py
+-rw-rw-rw-   0        0        0     2098 2021-09-12 02:14:51.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/oven_cook_mode_converter.py
+-rw-rw-rw-   0        0        0      504 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/oven/oven_ranges_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.244699 gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/
+-rw-rw-rw-   0        0        0      724 2021-08-05 20:08:43.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/__init__.py
+-rw-rw-rw-   0        0        0     1127 2020-12-27 18:07:39.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/erd_bool_converter.py
+-rw-rw-rw-   0        0        0      911 2020-12-27 18:08:19.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/erd_bytes_converter.py
+-rw-rw-rw-   0        0        0     1167 2021-07-21 03:17:07.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/erd_int_converter.py
+-rw-rw-rw-   0        0        0     1279 2020-12-27 18:11:14.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/erd_signed_byte_converter.py
+-rw-rw-rw-   0        0        0     1145 2020-12-27 18:11:02.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/erd_string_converter.py
+-rw-rw-rw-   0        0        0     2399 2022-09-04 02:27:39.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/erd_time_span_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.275125 gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/
+-rw-rw-rw-   0        0        0      646 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/__init__.py
+-rw-rw-rw-   0        0        0      987 2022-08-13 16:20:42.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/erd_appliance_type_converter.py
+-rw-rw-rw-   0        0        0      382 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/erd_clock_format_converter.py
+-rw-rw-rw-   0        0        0      525 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/erd_end_tone_converter.py
+-rw-rw-rw-   0        0        0     1085 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/erd_locked_converter.py
+-rw-rw-rw-   0        0        0      422 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/erd_measurement_units_converter.py
+-rw-rw-rw-   0        0        0      535 2020-12-27 16:50:31.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/erd_model_serial_converter.py
+-rw-rw-rw-   0        0        0      423 2021-08-01 02:00:52.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/erd_on_off_converter.py
+-rw-rw-rw-   0        0        0      467 2020-12-27 16:49:34.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/erd_software_version_converter.py
+-rw-rw-rw-   0        0        0      443 2021-05-17 02:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/erd_sound_level_converter.py
+-rw-rw-rw-   0        0        0      506 2021-08-10 17:18:26.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/erd_unit_type_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.300126 gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/
+-rw-rw-rw-   0        0        0      654 2021-07-09 02:55:38.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/__init__.py
+-rw-rw-rw-   0        0        0      579 2021-07-08 21:27:05.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/erd_alert_settings_converter.py
+-rw-rw-rw-   0        0        0      324 2021-07-08 21:27:00.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/erd_alert_state_converter.py
+-rw-rw-rw-   0        0        0      423 2021-07-08 21:26:54.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/erd_filter_manual_mode_converter.py
+-rw-rw-rw-   0        0        0      400 2021-07-09 02:54:54.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/erd_filter_mode_converter.py
+-rw-rw-rw-   0        0        0      743 2021-07-21 03:14:09.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/erd_filter_position_converter.py
+-rw-rw-rw-   0        0        0      448 2021-07-09 02:55:01.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/erd_filter_valve_state_converter.py
+-rw-rw-rw-   0        0        0      432 2021-07-09 02:55:03.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/erd_leak_validity_converter.py
+-rw-rw-rw-   0        0        0      358 2021-07-20 01:01:24.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/erd_waterfilter_flow_converter.py
+-rw-rw-rw-   0        0        0      804 2021-07-20 01:13:48.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/erd_waterfilter_life_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.315054 gehomesdk-0.5.9/gehomesdk/erd/converters/water_heater/
+-rw-rw-rw-   0        0        0      321 2022-09-17 15:06:16.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_heater/__init__.py
+-rw-rw-rw-   0        0        0      989 2022-09-17 15:06:16.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_heater/erd_waterheater_min_max_temperature.py
+-rw-rw-rw-   0        0        0      495 2022-09-04 02:27:39.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_heater/erd_waterheater_mode.py
+-rw-rw-rw-   0        0        0      609 2022-09-04 02:27:39.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_heater/erd_waterheater_mode_hours_remaining.py
+-rw-rw-rw-   0        0        0      459 2022-09-04 20:53:15.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_heater/erd_waterheater_temperature.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.325955 gehomesdk-0.5.9/gehomesdk/erd/converters/water_softener/
+-rw-rw-rw-   0        0        0      266 2021-12-04 20:18:35.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_softener/__init__.py
+-rw-rw-rw-   0        0        0      446 2021-12-04 20:09:57.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_softener/erd_softener_error_code_converter.py
+-rw-rw-rw-   0        0        0      426 2021-12-04 20:18:49.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_softener/erd_softener_salt_level_converter.py
+-rw-rw-rw-   0        0        0      873 2021-12-04 20:04:15.000000 gehomesdk-0.5.9/gehomesdk/erd/converters/water_softener/erd_softener_shutoff_valve_state_converter.py
+-rw-rw-rw-   0        0        0     1039 2022-09-04 02:27:39.000000 gehomesdk-0.5.9/gehomesdk/erd/erd_code_class.py
+-rw-rw-rw-   0        0        0    13726 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/erd_codes.py
+-rw-rw-rw-   0        0        0    28490 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/erd_configuration.py
+-rw-rw-rw-   0        0        0      218 2021-12-11 04:31:01.000000 gehomesdk-0.5.9/gehomesdk/erd/erd_data_type.py
+-rw-rw-rw-   0        0        0     5162 2023-01-23 01:12:08.000000 gehomesdk-0.5.9/gehomesdk/erd/erd_encoder.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.327953 gehomesdk-0.5.9/gehomesdk/erd/values/
+-rw-rw-rw-   0        0        0      360 2022-09-04 02:27:39.000000 gehomesdk-0.5.9/gehomesdk/erd/values/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.335957 gehomesdk-0.5.9/gehomesdk/erd/values/ac/
+-rw-rw-rw-   0        0        0       79 2021-08-05 18:46:56.000000 gehomesdk-0.5.9/gehomesdk/erd/values/ac/__init__.py
+-rw-rw-rw-   0        0        0      855 2021-08-07 00:13:47.000000 gehomesdk-0.5.9/gehomesdk/erd/values/ac/common_enums.py
+-rw-rw-rw-   0        0        0      506 2021-08-08 14:50:33.000000 gehomesdk-0.5.9/gehomesdk/erd/values/ac/sac_enums.py
+-rw-rw-rw-   0        0        0      323 2021-08-05 18:46:22.000000 gehomesdk-0.5.9/gehomesdk/erd/values/ac/wac_enums.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.362953 gehomesdk-0.5.9/gehomesdk/erd/values/advantium/
+-rw-rw-rw-   0        0        0      718 2021-07-17 00:04:53.000000 gehomesdk-0.5.9/gehomesdk/erd/values/advantium/__init__.py
+-rw-rw-rw-   0        0        0      539 2021-07-17 02:27:43.000000 gehomesdk-0.5.9/gehomesdk/erd/values/advantium/advantium_cook_setting.py
+-rw-rw-rw-   0        0        0     1660 2021-08-07 00:14:11.000000 gehomesdk-0.5.9/gehomesdk/erd/values/advantium/advantium_enums.py
+-rw-rw-rw-   0        0        0      807 2021-07-17 00:07:56.000000 gehomesdk-0.5.9/gehomesdk/erd/values/advantium/advantium_operation_mode.py
+-rw-rw-rw-   0        0        0     2070 2021-07-17 02:27:38.000000 gehomesdk-0.5.9/gehomesdk/erd/values/advantium/advantium_operation_mode_mapping.py
+-rw-rw-rw-   0        0        0      765 2021-06-19 16:52:09.000000 gehomesdk-0.5.9/gehomesdk/erd/values/advantium/erd_advantium_cook_setting.py
+-rw-rw-rw-   0        0        0      714 2021-06-15 19:24:07.000000 gehomesdk-0.5.9/gehomesdk/erd/values/advantium/erd_advantium_cook_status.py
+-rw-rw-rw-   0        0        0      568 2021-06-19 18:17:09.000000 gehomesdk-0.5.9/gehomesdk/erd/values/advantium/erd_advantium_cook_time_min_max.py
+-rw-rw-rw-   0        0        0      258 2021-06-19 18:16:29.000000 gehomesdk-0.5.9/gehomesdk/erd/values/advantium/erd_advantium_kitchen_timer_min_max.py
+-rw-rw-rw-   0        0        0      341 2021-06-19 18:18:28.000000 gehomesdk-0.5.9/gehomesdk/erd/values/advantium/erd_advantium_microwave_min_max.py
+-rw-rw-rw-   0        0        0      422 2021-06-19 18:18:36.000000 gehomesdk-0.5.9/gehomesdk/erd/values/advantium/erd_advantium_precision_min_max.py
+-rw-rw-rw-   0        0        0     5218 2021-06-16 14:28:30.000000 gehomesdk-0.5.9/gehomesdk/erd/values/advantium/erd_advantium_remote_cook_mode_config.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.366955 gehomesdk-0.5.9/gehomesdk/erd/values/coffee_maker/
+-rw-rw-rw-   0        0        0       27 2021-12-11 14:28:26.000000 gehomesdk-0.5.9/gehomesdk/erd/values/coffee_maker/__init__.py
+-rw-rw-rw-   0        0        0      836 2021-12-11 14:28:26.000000 gehomesdk-0.5.9/gehomesdk/erd/values/coffee_maker/common_enums.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.384956 gehomesdk-0.5.9/gehomesdk/erd/values/common/
+-rw-rw-rw-   0        0        0      380 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/values/common/__init__.py
+-rw-rw-rw-   0        0        0      842 2022-09-04 02:59:53.000000 gehomesdk-0.5.9/gehomesdk/erd/values/common/erd_appliance_type.py
+-rw-rw-rw-   0        0        0      139 2020-12-26 14:45:00.000000 gehomesdk-0.5.9/gehomesdk/erd/values/common/erd_clock_format.py
+-rw-rw-rw-   0        0        0      117 2020-12-26 14:45:46.000000 gehomesdk-0.5.9/gehomesdk/erd/values/common/erd_end_tone.py
+-rw-rw-rw-   0        0        0      111 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/values/common/erd_locked.py
+-rw-rw-rw-   0        0        0      102 2020-12-26 14:47:25.000000 gehomesdk-0.5.9/gehomesdk/erd/values/common/erd_measurement_units.py
+-rw-rw-rw-   0        0        0      213 2021-08-07 00:14:17.000000 gehomesdk-0.5.9/gehomesdk/erd/values/common/erd_on_off.py
+-rw-rw-rw-   0        0        0      116 2020-12-26 14:46:06.000000 gehomesdk-0.5.9/gehomesdk/erd/values/common/erd_present.py
+-rw-rw-rw-   0        0        0      118 2020-12-26 14:45:14.000000 gehomesdk-0.5.9/gehomesdk/erd/values/common/erd_sound_level.py
+-rw-rw-rw-   0        0        0      311 2021-08-10 17:21:14.000000 gehomesdk-0.5.9/gehomesdk/erd/values/common/erd_unit_type.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.406958 gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/
+-rw-rw-rw-   0        0        0      732 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/__init__.py
+-rw-rw-rw-   0        0        0      174 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/cycle_count.py
+-rw-rw-rw-   0        0        0     1246 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/cycle_state_mapping.py
+-rw-rw-rw-   0        0        0      814 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/erd_cycle_state.py
+-rw-rw-rw-   0        0        0      527 2021-08-07 00:14:24.000000 gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/erd_dishwasher_door_status.py
+-rw-rw-rw-   0        0        0      384 2021-01-04 22:51:42.000000 gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/erd_operating_mode.py
+-rw-rw-rw-   0        0        0      202 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/erd_reminders.py
+-rw-rw-rw-   0        0        0     1299 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/erd_user_setting.py
+-rw-rw-rw-   0        0        0      152 2023-01-23 01:07:26.000000 gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/error_state.py
+-rw-rw-rw-   0        0        0      515 2021-09-11 01:57:54.000000 gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/operating_mode.py
+-rw-rw-rw-   0        0        0     1065 2021-01-04 22:53:18.000000 gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/operating_mode_mapping.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.434957 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/
+-rw-rw-rw-   0        0        0      672 2021-10-08 00:53:06.000000 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/__init__.py
+-rw-rw-rw-   0        0        0      380 2021-10-08 01:51:36.000000 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/erd_convertable_drawer_mode.py
+-rw-rw-rw-   0        0        0      490 2021-08-07 00:15:01.000000 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/erd_door_status.py
+-rw-rw-rw-   0        0        0      354 2021-07-16 00:58:21.000000 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/erd_filter_status.py
+-rw-rw-rw-   0        0        0      284 2021-08-07 00:15:07.000000 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/erd_full_not_full.py
+-rw-rw-rw-   0        0        0      203 2020-12-26 15:17:44.000000 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/erd_hot_water_status.py
+-rw-rw-rw-   0        0        0      114 2020-12-26 15:18:04.000000 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/erd_pod_status.py
+-rw-rw-rw-   0        0        0      574 2021-07-20 20:43:01.000000 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/fridge_door_status.py
+-rw-rw-rw-   0        0        0      703 2020-12-28 16:02:04.000000 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/fridge_ice_bucket_status.py
+-rw-rw-rw-   0        0        0      184 2020-12-29 17:47:46.000000 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/fridge_model_info.py
+-rw-rw-rw-   0        0        0      158 2020-12-26 15:22:45.000000 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/fridge_set_point_limits.py
+-rw-rw-rw-   0        0        0      104 2020-12-26 15:23:19.000000 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/fridge_set_points.py
+-rw-rw-rw-   0        0        0      691 2020-12-29 16:37:18.000000 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/hot_water_status.py
+-rw-rw-rw-   0        0        0      165 2020-12-26 15:26:00.000000 gehomesdk-0.5.9/gehomesdk/erd/values/fridge/ice_maker_control_status.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.441955 gehomesdk-0.5.9/gehomesdk/erd/values/hood/
+-rw-rw-rw-   0        0        0      179 2021-08-21 02:16:53.000000 gehomesdk-0.5.9/gehomesdk/erd/values/hood/__init__.py
+-rw-rw-rw-   0        0        0      560 2021-08-21 15:29:12.000000 gehomesdk-0.5.9/gehomesdk/erd/values/hood/common_enums.py
+-rw-rw-rw-   0        0        0      522 2021-08-21 15:56:41.000000 gehomesdk-0.5.9/gehomesdk/erd/values/hood/erd_hood_fan_speed_availability.py
+-rw-rw-rw-   0        0        0      384 2021-08-21 15:57:34.000000 gehomesdk-0.5.9/gehomesdk/erd/values/hood/erd_hood_light_level_availability.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.445954 gehomesdk-0.5.9/gehomesdk/erd/values/ice_maker/
+-rw-rw-rw-   0        0        0       27 2021-10-18 00:13:39.000000 gehomesdk-0.5.9/gehomesdk/erd/values/ice_maker/__init__.py
+-rw-rw-rw-   0        0        0      794 2021-10-18 00:24:03.000000 gehomesdk-0.5.9/gehomesdk/erd/values/ice_maker/common_enums.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.468955 gehomesdk-0.5.9/gehomesdk/erd/values/laundry/
+-rw-rw-rw-   0        0        0      567 2021-07-08 17:15:12.000000 gehomesdk-0.5.9/gehomesdk/erd/values/laundry/__init__.py
+-rw-rw-rw-   0        0        0      254 2021-07-08 16:52:40.000000 gehomesdk-0.5.9/gehomesdk/erd/values/laundry/dryness_level.py
+-rw-rw-rw-   0        0        0      774 2021-06-30 02:11:43.000000 gehomesdk-0.5.9/gehomesdk/erd/values/laundry/dryness_level_mapping.py
+-rw-rw-rw-   0        0        0      217 2021-07-08 16:25:30.000000 gehomesdk-0.5.9/gehomesdk/erd/values/laundry/ecodry_status.py
+-rw-rw-rw-   0        0        0      339 2021-06-30 02:11:43.000000 gehomesdk-0.5.9/gehomesdk/erd/values/laundry/ecodry_status_mapping.py
+-rw-rw-rw-   0        0        0     5942 2021-08-07 00:15:41.000000 gehomesdk-0.5.9/gehomesdk/erd/values/laundry/laundry_enums.py
+-rw-rw-rw-   0        0        0      530 2021-07-08 16:26:13.000000 gehomesdk-0.5.9/gehomesdk/erd/values/laundry/machine_state.py
+-rw-rw-rw-   0        0        0      856 2021-06-30 02:11:43.000000 gehomesdk-0.5.9/gehomesdk/erd/values/laundry/machine_state_mapping.py
+-rw-rw-rw-   0        0        0      253 2021-07-08 16:41:48.000000 gehomesdk-0.5.9/gehomesdk/erd/values/laundry/temperature_option.py
+-rw-rw-rw-   0        0        0      898 2021-06-30 02:11:43.000000 gehomesdk-0.5.9/gehomesdk/erd/values/laundry/temperature_option_mapping.py
+-rw-rw-rw-   0        0        0      287 2021-07-08 16:50:43.000000 gehomesdk-0.5.9/gehomesdk/erd/values/laundry/washtemp_level.py
+-rw-rw-rw-   0        0        0      784 2021-07-08 16:55:53.000000 gehomesdk-0.5.9/gehomesdk/erd/values/laundry/washtemp_level_mapping.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.477955 gehomesdk-0.5.9/gehomesdk/erd/values/microwave/
+-rw-rw-rw-   0        0        0      220 2021-10-18 03:39:01.000000 gehomesdk-0.5.9/gehomesdk/erd/values/microwave/__init__.py
+-rw-rw-rw-   0        0        0      247 2021-10-18 03:02:22.000000 gehomesdk-0.5.9/gehomesdk/erd/values/microwave/erd_microwave_available_modes.py
+-rw-rw-rw-   0        0        0      242 2021-10-18 03:41:50.000000 gehomesdk-0.5.9/gehomesdk/erd/values/microwave/erd_microwave_cook_setting.py
+-rw-rw-rw-   0        0        0      376 2021-12-12 17:14:52.000000 gehomesdk-0.5.9/gehomesdk/erd/values/microwave/erd_microwave_state.py
+-rw-rw-rw-   0        0        0      912 2021-12-12 17:13:53.000000 gehomesdk-0.5.9/gehomesdk/erd/values/microwave/microwave_enums.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.526954 gehomesdk-0.5.9/gehomesdk/erd/values/oven/
+-rw-rw-rw-   0        0        0     1272 2021-12-11 17:31:40.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/__init__.py
+-rw-rw-rw-   0        0        0      233 2020-12-26 15:08:43.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/available_cook_mode.py
+-rw-rw-rw-   0        0        0     1158 2020-12-29 18:37:42.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/burner.py
+-rw-rw-rw-   0        0        0     1264 2021-08-19 23:56:38.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/const.py
+-rw-rw-rw-   0        0        0     1485 2020-12-29 19:04:34.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/cooktop_status.py
+-rw-rw-rw-   0        0        0     7538 2021-09-12 02:28:00.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_available_cook_mode.py
+-rw-rw-rw-   0        0        0      239 2020-12-27 05:55:10.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_closed_loop_cooking_configuration.py
+-rw-rw-rw-   0        0        0     2057 2020-12-27 05:55:20.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_closed_loop_cooking_devices_status.py
+-rw-rw-rw-   0        0        0      285 2020-12-26 16:43:26.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_cooktop_config.py
+-rw-rw-rw-   0        0        0      112 2020-12-27 02:12:53.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_cooktop_status.py
+-rw-rw-rw-   0        0        0      368 2021-08-19 23:48:09.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_extended_cook_mode.py
+-rw-rw-rw-   0        0        0      251 2020-12-26 15:10:14.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_oven_configuration.py
+-rw-rw-rw-   0        0        0     2179 2021-09-11 16:41:41.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_oven_cook_mode.py
+-rw-rw-rw-   0        0        0      320 2021-12-11 17:30:12.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_oven_light_level.py
+-rw-rw-rw-   0        0        0      465 2021-12-12 01:07:17.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_oven_light_level_availability.py
+-rw-rw-rw-   0        0        0     2391 2021-08-19 21:09:42.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_oven_state.py
+-rw-rw-rw-   0        0        0      135 2020-12-27 05:20:05.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_precision_cooking_app_probe_control_mode.py
+-rw-rw-rw-   0        0        0      122 2020-12-27 04:46:36.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_precision_cooking_probe_battery_status.py
+-rw-rw-rw-   0        0        0      231 2020-12-27 05:55:42.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_precision_cooking_probe_target_time_reached.py
+-rw-rw-rw-   0        0        0      145 2020-12-27 01:14:52.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_precision_cooking_start_sous_vide_timer_active_status.py
+-rw-rw-rw-   0        0        0      319 2020-12-26 15:10:51.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/oven_configuration.py
+-rw-rw-rw-   0        0        0      346 2020-12-26 15:04:29.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/oven_cook_mode.py
+-rw-rw-rw-   0        0        0     7341 2021-09-11 16:41:13.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/oven_cook_mode_mapping.py
+-rw-rw-rw-   0        0        0     1700 2021-09-11 16:27:29.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/oven_cook_setting.py
+-rw-rw-rw-   0        0        0     2990 2021-08-20 00:19:46.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/oven_display_state_mapping.py
+-rw-rw-rw-   0        0        0       98 2020-12-26 15:04:53.000000 gehomesdk-0.5.9/gehomesdk/erd/values/oven/oven_ranges.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.548956 gehomesdk-0.5.9/gehomesdk/erd/values/water_filter/
+-rw-rw-rw-   0        0        0      581 2021-07-08 21:45:12.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_filter/__init__.py
+-rw-rw-rw-   0        0        0      374 2021-06-30 17:14:52.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_filter/erd_waterfilter_alert_settings.py
+-rw-rw-rw-   0        0        0      913 2021-07-09 03:25:38.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_filter/erd_waterfilter_alert_state.py
+-rw-rw-rw-   0        0        0      204 2021-07-09 03:25:45.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_filter/erd_waterfilter_flowrate.py
+-rw-rw-rw-   0        0        0      238 2021-08-07 00:16:11.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_filter/erd_waterfilter_leak_validity.py
+-rw-rw-rw-   0        0        0      252 2021-07-20 01:12:34.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_filter/erd_waterfilter_life.py
+-rw-rw-rw-   0        0        0      336 2021-08-07 00:16:20.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_filter/erd_waterfilter_manual_mode.py
+-rw-rw-rw-   0        0        0      328 2021-07-16 00:58:21.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_filter/erd_waterfilter_mode.py
+-rw-rw-rw-   0        0        0      256 2021-07-08 21:28:04.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_filter/erd_waterfilter_position.py
+-rw-rw-rw-   0        0        0      314 2021-07-08 21:28:08.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_filter/erd_waterfilter_valve_state.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.566789 gehomesdk-0.5.9/gehomesdk/erd/values/water_heater/
+-rw-rw-rw-   0        0        0      371 2022-09-17 15:06:16.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_heater/__init__.py
+-rw-rw-rw-   0        0        0      117 2022-09-17 15:06:16.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_heater/erd_waterheater_min_max_temperature.py
+-rw-rw-rw-   0        0        0      380 2022-09-04 02:27:39.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_heater/erd_waterheater_mode.py
+-rw-rw-rw-   0        0        0      193 2022-09-04 02:27:39.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_heater/erd_waterheater_mode_hours_remaining.py
+-rw-rw-rw-   0        0        0      207 2022-09-04 02:27:39.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_heater/erd_waterheater_set_temperature.py
+-rw-rw-rw-   0        0        0      210 2022-09-04 02:27:39.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_heater/erd_waterheater_target_temperature.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.575913 gehomesdk-0.5.9/gehomesdk/erd/values/water_softener/
+-rw-rw-rw-   0        0        0      224 2021-12-04 20:17:44.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_softener/__init__.py
+-rw-rw-rw-   0        0        0      545 2021-12-04 19:31:11.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_softener/erd_watersoftener_error_code.py
+-rw-rw-rw-   0        0        0      329 2021-12-04 20:17:05.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_softener/erd_watersoftener_salt_level.py
+-rw-rw-rw-   0        0        0      274 2021-12-04 19:44:04.000000 gehomesdk-0.5.9/gehomesdk/erd/values/water_softener/erd_watersoftener_shutoff_valve_state.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:40.608213 gehomesdk-0.5.9/gehomesdk/exception/
+-rw-rw-rw-   0        0        0      643 2021-05-17 02:50:39.000000 gehomesdk-0.5.9/gehomesdk/exception/__init__.py
+-rw-rw-rw-   0        0        0      153 2020-12-27 18:53:39.000000 gehomesdk-0.5.9/gehomesdk/exception/ge_auth_failed_error.py
+-rw-rw-rw-   0        0        0      154 2020-12-27 18:54:19.000000 gehomesdk-0.5.9/gehomesdk/exception/ge_client_disconnected_error.py
+-rw-rw-rw-   0        0        0      174 2021-01-08 02:28:45.000000 gehomesdk-0.5.9/gehomesdk/exception/ge_duplicate_appliance_error.py
+-rw-rw-rw-   0        0        0       95 2020-12-27 15:39:37.000000 gehomesdk-0.5.9/gehomesdk/exception/ge_exception.py
+-rw-rw-rw-   0        0        0      166 2020-12-27 18:58:18.000000 gehomesdk-0.5.9/gehomesdk/exception/ge_general_server_error.py
+-rw-rw-rw-   0        0        0      159 2021-01-08 01:42:19.000000 gehomesdk-0.5.9/gehomesdk/exception/ge_needs_reauthentication_error.py
+-rw-rw-rw-   0        0        0      157 2020-12-27 18:53:12.000000 gehomesdk-0.5.9/gehomesdk/exception/ge_not_authenticated_error.py
+-rw-rw-rw-   0        0        0      516 2021-01-04 01:56:47.000000 gehomesdk-0.5.9/gehomesdk/exception/ge_request_error.py
+-rw-rw-rw-   0        0        0      445 2020-12-27 15:48:13.000000 gehomesdk-0.5.9/gehomesdk/exception/ge_set_erd_not_allowed_error.py
+-rw-rw-rw-   0        0        0      166 2020-12-27 15:42:50.000000 gehomesdk-0.5.9/gehomesdk/exception/ge_unsupported_operation_error.py
+-rw-rw-rw-   0        0        0     2113 2022-08-13 16:41:20.000000 gehomesdk-0.5.9/gehomesdk/gather_data.py
+-rw-rw-rw-   0        0        0     8656 2021-12-12 00:03:38.000000 gehomesdk-0.5.9/gehomesdk/ge_appliance.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:33:39.968993 gehomesdk-0.5.9/gehomesdk.egg-info/
+-rw-rw-rw-   0        0        0    13848 2023-04-23 03:33:39.000000 gehomesdk-0.5.9/gehomesdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    16222 2023-04-23 03:33:39.000000 gehomesdk-0.5.9/gehomesdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 03:33:39.000000 gehomesdk-0.5.9/gehomesdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-04-23 03:33:39.000000 gehomesdk-0.5.9/gehomesdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-04-23 03:33:39.000000 gehomesdk-0.5.9/gehomesdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 03:33:39.000000 gehomesdk-0.5.9/gehomesdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 03:33:40.614214 gehomesdk-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     1570 2023-04-23 02:08:23.000000 gehomesdk-0.5.9/setup.py
```

### Comparing `gehomesdk-0.5.8/LICENSE` & `gehomesdk-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/PKG-INFO` & `gehomesdk-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: gehomesdk
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python SDK for GE Home Appliances
 Home-page: https://github.com/simbaja/gehome
 Author: Jack Simbach
 Author-email: jack.simbach@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-Provides-Extra: XMPP
 License-File: LICENSE
 
 # gehomesdk
 Python SDK for GE WiFi-enabled (SmartHQ) appliances.
 The primary goal is to use this to power integrations for [Home Assistant](https://www.home-assistant.io/), though that
 will probably need to wait on some new entity types.   
 
@@ -265,9 +264,7 @@
             "0x000a":"03",
             "0x0089":"",
             ...
         }</json>
     </response>
 </body>
 ```
-
-
```

### Comparing `gehomesdk-0.5.8/README.md` & `gehomesdk-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/clients/__init__.py` & `gehomesdk-0.5.9/gehomesdk/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/clients/async_helpers.py` & `gehomesdk-0.5.9/gehomesdk/clients/async_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 async def CancellableAsyncIterator(async_iterator: AsyncIterator, cancellation_event: asyncio.Event) -> AsyncIterator:
     cancellation_task = asyncio.create_task(cancellation_event.wait())
     result_iter = async_iterator.__aiter__()
     while not cancellation_event.is_set():
         done, pending = await asyncio.wait(
-            [cancellation_task, result_iter.__anext__()],
+            [cancellation_task, asyncio.create_task(result_iter.__anext__())],
             return_when=asyncio.FIRST_COMPLETED
         )
         for done_task in done:
             if done_task == cancellation_task:
                 for pending_task in pending:
                     await pending_task
                 break
```

### Comparing `gehomesdk-0.5.8/gehomesdk/clients/async_login_flows.py` & `gehomesdk-0.5.9/gehomesdk/clients/async_login_flows.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/clients/base_client.py` & `gehomesdk-0.5.9/gehomesdk/clients/base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,18 @@
         return self._state == GeClientState.CONNECTED
 
     @property
     def event_handlers(self) -> Dict[str, List[Callable]]:
         return self._event_handlers
 
     async def async_event(self, event: str, *args, **kwargs):
+        _LOGGER.debug(f"received event: {event}, processing callbacks...")
         """Trigger event callbacks sequentially"""
         for cb in self.event_handlers[event]:
+            _LOGGER.debug(f"processing callback: {cb}")
             asyncio.ensure_future(cb(*args, **kwargs), loop=self.loop)
 
     def add_event_handler(self, event: str, callback: Callable, disposable: bool = False):
         if disposable:
             raise NotImplementedError('Support for disposable callbacks not yet implemented')
         self.event_handlers[event].append(callback)
 
@@ -132,15 +134,16 @@
                 _LOGGER.info('Reauthentication needed')
             except GeRequestError as err:
                 _LOGGER.info(f'Error executing request {err}')
             except Exception as err:
                 if not self._has_successful_connect:
                     _LOGGER.warn(f'Unhandled exception on first connect attempt: {err}, disconnecting')
                     break
-                _LOGGER.info(f'Unhandled exception while running client: {err}, ignoring and restarting')  
+                _LOGGER.exception(err)
+                _LOGGER.info(f'Unhandled exception while running client, ignoring and restarting')
             finally:
                 if not self._disconnect_requested.is_set():
                     await self._set_state(GeClientState.DROPPED)
                     await self._set_state(GeClientState.WAITING)
                     _LOGGER.debug('Waiting before reconnecting')
                     await asyncio.sleep(RETRY_INTERVAL)
                     _LOGGER.debug('Refreshing authentication before reconnecting')
```

### Comparing `gehomesdk-0.5.8/gehomesdk/clients/const.py` & `gehomesdk-0.5.9/gehomesdk/clients/const.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/clients/ge_client_xmpp.py` & `gehomesdk-0.5.9/gehomesdk/clients/ge_client_xmpp.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/clients/websocket_client.py` & `gehomesdk-0.5.9/gehomesdk/clients/websocket_client.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/clients/xmpp_client.py` & `gehomesdk-0.5.9/gehomesdk/clients/xmpp_client.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/entry_points.py` & `gehomesdk-0.5.9/gehomesdk/entry_points.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/abstract.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/abstract.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/ac/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/ac/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/ac/erd_sac_target_temperature_range_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/ac/erd_sac_target_temperature_range_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_cook_setting_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_cook_setting_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_cook_status_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_cook_status_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_cook_time_min_max_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_cook_time_min_max_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_kitchen_timer_min_max_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_kitchen_timer_min_max_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_microwave_min_max_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_microwave_min_max_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_precision_min_max_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_precision_min_max_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/advantium/erd_advantium_remote_cook_mode_config_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/advantium/erd_advantium_remote_cook_mode_config_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/coffee_maker/erd_ccm_brew_settings_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/coffee_maker/erd_ccm_brew_settings_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/coffee_maker/erd_ccm_brew_temperature_range_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/coffee_maker/erd_ccm_brew_temperature_range_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/erd_cycle_count_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/erd_cycle_count_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/erd_cycle_state_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/erd_cycle_state_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/erd_dishwasher_door_status_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/erd_dishwasher_door_status_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/erd_error_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/erd_error_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/erd_reminders_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/erd_reminders_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/erd_user_setting_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/erd_user_setting_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/dishwasher/operating_mode_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/dishwasher/operating_mode_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/erd_convertable_drawer_mode_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/erd_convertable_drawer_mode_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/erd_filter_status_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/erd_filter_status_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/fridge_door_status_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/fridge_door_status_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/fridge_ice_bucket_status_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/fridge_ice_bucket_status_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/fridge_model_info_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/fridge_model_info_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/fridge_set_point_limits_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/fridge_set_point_limits_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/fridge_set_points_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/fridge_set_points_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/hot_water_status_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/hot_water_status_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/fridge/ice_maker_control_status_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/fridge/ice_maker_control_status_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/hood/erd_hood_fan_speed_availability_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/hood/erd_hood_fan_speed_availability_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/hood/erd_hood_light_level_availability_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/hood/erd_hood_light_level_availability_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/dryness_level_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/dryness_level_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/ecodry_status_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/ecodry_status_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/laundry_door_status_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/laundry_door_status_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/laundry_sub_cycle_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/laundry_sub_cycle_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/machine_state_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/machine_state_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/sheet_usage_configuration_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/sheet_usage_configuration_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/smart_dispense_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/smart_dispense_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/smart_dispense_tank_status_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/smart_dispense_tank_status_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/spintime_level_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/spintime_level_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/temperature_option_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/temperature_option_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/tumble_status_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/tumble_status_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/laundry/washtemp_level_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/laundry/washtemp_level_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/microwave/erd_microwave_available_modes_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/microwave/erd_microwave_available_modes_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/microwave/erd_microwave_cook_setting_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/microwave/erd_microwave_cook_setting_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/microwave/erd_microwave_cook_timer_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/microwave/erd_microwave_cook_timer_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/microwave/erd_microwave_state_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/microwave/erd_microwave_state_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/oven/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/oven/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/oven/cooktop_status_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/oven/cooktop_status_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_available_cook_mode_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_available_cook_mode_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_cooktop_config_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_cooktop_config_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_extended_cook_mode_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_extended_cook_mode_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_oven_light_level_availability_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_oven_light_level_availability_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_oven_state_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_oven_state_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_precision_cooking_app_probe_control_mode_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_precision_cooking_app_probe_control_mode_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_precision_cooking_probe_battery_status_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_precision_cooking_probe_battery_status_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_precision_cooking_probe_target_time_reached_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_precision_cooking_probe_target_time_reached_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/oven/erd_precision_cooking_start_sous_vide_timer_active_status_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/oven/erd_precision_cooking_start_sous_vide_timer_active_status_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/oven/oven_configuration_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/oven/oven_configuration_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/oven/oven_cook_mode_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/oven/oven_cook_mode_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/erd_bool_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/erd_bool_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/erd_bytes_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/erd_bytes_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/erd_int_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/erd_int_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/erd_signed_byte_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/erd_signed_byte_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/erd_string_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/erd_string_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/primitives/erd_time_span_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/primitives/erd_time_span_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/erd_appliance_type_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/erd_appliance_type_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/erd_end_tone_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/erd_end_tone_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/erd_locked_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/erd_locked_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/specialized/erd_model_serial_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/specialized/erd_model_serial_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/erd_alert_settings_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/erd_alert_settings_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/erd_filter_position_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/erd_filter_position_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/water_filter/erd_waterfilter_life_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/water_filter/erd_waterfilter_life_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/water_heater/erd_waterheater_min_max_temperature.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/water_heater/erd_waterheater_min_max_temperature.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/water_heater/erd_waterheater_mode_hours_remaining.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/water_heater/erd_waterheater_mode_hours_remaining.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/converters/water_softener/erd_softener_shutoff_valve_state_converter.py` & `gehomesdk-0.5.9/gehomesdk/erd/converters/water_softener/erd_softener_shutoff_valve_state_converter.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/erd_code_class.py` & `gehomesdk-0.5.9/gehomesdk/erd/erd_code_class.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/erd_codes.py` & `gehomesdk-0.5.9/gehomesdk/erd/erd_codes.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/erd_configuration.py` & `gehomesdk-0.5.9/gehomesdk/erd/erd_configuration.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/erd_encoder.py` & `gehomesdk-0.5.9/gehomesdk/erd/erd_encoder.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/ac/common_enums.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/ac/common_enums.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/advantium/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/advantium/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/advantium/advantium_cook_setting.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/advantium/advantium_cook_setting.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/advantium/advantium_enums.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/advantium/advantium_enums.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/advantium/advantium_operation_mode.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/advantium/advantium_operation_mode.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/advantium/advantium_operation_mode_mapping.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/advantium/advantium_operation_mode_mapping.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/advantium/erd_advantium_cook_setting.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/advantium/erd_advantium_cook_setting.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/advantium/erd_advantium_cook_status.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/advantium/erd_advantium_cook_status.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/advantium/erd_advantium_cook_time_min_max.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/advantium/erd_advantium_cook_time_min_max.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/advantium/erd_advantium_remote_cook_mode_config.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/advantium/erd_advantium_remote_cook_mode_config.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/coffee_maker/common_enums.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/coffee_maker/common_enums.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/common/erd_appliance_type.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/common/erd_appliance_type.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/cycle_state_mapping.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/cycle_state_mapping.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/erd_cycle_state.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/erd_cycle_state.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/erd_dishwasher_door_status.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/erd_dishwasher_door_status.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/erd_user_setting.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/erd_user_setting.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/operating_mode.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/operating_mode.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/dishwasher/operating_mode_mapping.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/dishwasher/operating_mode_mapping.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/fridge/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/fridge/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/fridge/fridge_door_status.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/fridge/fridge_door_status.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/fridge/fridge_ice_bucket_status.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/fridge/fridge_ice_bucket_status.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/fridge/hot_water_status.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/fridge/hot_water_status.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/hood/common_enums.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/hood/common_enums.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/hood/erd_hood_fan_speed_availability.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/hood/erd_hood_fan_speed_availability.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/ice_maker/common_enums.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/ice_maker/common_enums.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/laundry/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/laundry/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/laundry/dryness_level_mapping.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/laundry/dryness_level_mapping.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/laundry/laundry_enums.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/laundry/laundry_enums.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/laundry/machine_state.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/laundry/machine_state.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/laundry/machine_state_mapping.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/laundry/machine_state_mapping.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/laundry/temperature_option_mapping.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/laundry/temperature_option_mapping.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/laundry/washtemp_level_mapping.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/laundry/washtemp_level_mapping.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/microwave/microwave_enums.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/microwave/microwave_enums.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/oven/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/oven/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/oven/burner.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/oven/burner.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/oven/const.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/oven/const.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/oven/cooktop_status.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/oven/cooktop_status.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_available_cook_mode.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_available_cook_mode.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_closed_loop_cooking_devices_status.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_closed_loop_cooking_devices_status.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_oven_cook_mode.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_oven_cook_mode.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/oven/erd_oven_state.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/oven/erd_oven_state.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/oven/oven_cook_mode_mapping.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/oven/oven_cook_mode_mapping.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/oven/oven_cook_setting.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/oven/oven_cook_setting.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/oven/oven_display_state_mapping.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/oven/oven_display_state_mapping.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/water_filter/__init__.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/water_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/water_filter/erd_waterfilter_alert_state.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/water_filter/erd_waterfilter_alert_state.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/erd/values/water_softener/erd_watersoftener_error_code.py` & `gehomesdk-0.5.9/gehomesdk/erd/values/water_softener/erd_watersoftener_error_code.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/exception/__init__.py` & `gehomesdk-0.5.9/gehomesdk/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/exception/ge_request_error.py` & `gehomesdk-0.5.9/gehomesdk/exception/ge_request_error.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/gather_data.py` & `gehomesdk-0.5.9/gehomesdk/gather_data.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk/ge_appliance.py` & `gehomesdk-0.5.9/gehomesdk/ge_appliance.py`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/gehomesdk.egg-info/PKG-INFO` & `gehomesdk-0.5.9/gehomesdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: gehomesdk
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python SDK for GE Home Appliances
 Home-page: https://github.com/simbaja/gehome
 Author: Jack Simbach
 Author-email: jack.simbach@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-Provides-Extra: XMPP
 License-File: LICENSE
 
 # gehomesdk
 Python SDK for GE WiFi-enabled (SmartHQ) appliances.
 The primary goal is to use this to power integrations for [Home Assistant](https://www.home-assistant.io/), though that
 will probably need to wait on some new entity types.   
 
@@ -265,9 +264,7 @@
             "0x000a":"03",
             "0x0089":"",
             ...
         }</json>
     </response>
 </body>
 ```
-
-
```

### Comparing `gehomesdk-0.5.8/gehomesdk.egg-info/SOURCES.txt` & `gehomesdk-0.5.9/gehomesdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gehomesdk-0.5.8/setup.py` & `gehomesdk-0.5.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
     url="https://github.com/simbaja/gehome",
     author="Jack Simbach",
     author_email="jack.simbach@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     entry_points={
         'console_scripts': [
             'gehome-appliance-data = gehomesdk.entry_points:appliance_data',
         ],
     },    
     packages=find_namespace_packages(include=[base_package, f"{base_package}*"]),
     include_package_data=False,
-    install_requires=["aiohttp", "bidict", "requests", "websockets","humanize"],
-    extras_require={"XMPP": ["slixmpp==1.5.2"]}
+    install_requires=["aiohttp", "bidict", "requests", "websockets","humanize", "lxml", "slixmpp"]
 )
```

