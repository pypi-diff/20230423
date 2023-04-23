# Comparing `tmp/foursight_core-4.1.0.5b12.tar.gz` & `tmp/foursight_core-4.1.0.5b13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.1.0.5b12.tar", max compression
+gzip compressed data, was "foursight_core-4.1.0.5b13.tar", max compression
```

## Comparing `foursight_core-4.1.0.5b12.tar` & `foursight_core-4.1.0.5b13.tar`

### file list

```diff
@@ -1,139 +1,139 @@
--rw-r--r--   0        0        0     1083 2022-09-07 10:08:59.753994 foursight_core-4.1.0.5b12/LICENSE.txt
--rw-r--r--   0        0        0    10825 2022-11-20 13:33:58.544911 foursight_core-4.1.0.5b12/foursight_core/'
--rw-r--r--   0        0        0        0 2022-09-07 10:08:59.760120 foursight_core-4.1.0.5b12/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-03-30 11:22:44.920863 foursight_core-4.1.0.5b12/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0     8523 2023-02-23 17:12:48.834947 foursight_core-4.1.0.5b12/foursight_core/adfasdfad
--rw-r--r--   0        0        0       69 2023-04-16 14:05:52.759877 foursight_core-4.1.0.5b12/foursight_core/app.py
--rw-r--r--   0        0        0   105730 2023-04-16 14:04:58.418881 foursight_core-4.1.0.5b12/foursight_core/app_utils.py
--rw-r--r--   0        0        0   101241 2022-12-02 19:01:09.085977 foursight_core-4.1.0.5b12/foursight_core/app_utils.py---
--rw-r--r--   0        0        0    97799 2022-11-22 14:52:55.397982 foursight_core-4.1.0.5b12/foursight_core/app_utils.py-deb
--rw-r--r--   0        0        0    97949 2022-11-23 13:18:09.708092 foursight_core-4.1.0.5b12/foursight_core/app_utils.py-debug
--rw-r--r--   0        0        0   101943 2023-03-29 22:48:31.801408 foursight_core-4.1.0.5b12/foursight_core/app_utils.py-debugg
--rw-r--r--   0        0        0    12620 2022-11-30 14:04:39.423857 foursight_core-4.1.0.5b12/foursight_core/asdf
--rw-r--r--   0        0        0     2571 2023-03-30 11:22:44.922092 foursight_core-4.1.0.5b12/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2022-09-07 10:08:59.760846 foursight_core-4.1.0.5b12/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2022-09-07 10:08:59.760916 foursight_core-4.1.0.5b12/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-03-31 17:00:42.022944 foursight_core-4.1.0.5b12/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-03-30 11:22:44.922592 foursight_core-4.1.0.5b12/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     4452 2023-04-20 18:26:30.344734 foursight_core-4.1.0.5b12/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-03-31 17:00:42.023738 foursight_core-4.1.0.5b12/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-03-31 17:00:42.024190 foursight_core-4.1.0.5b12/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-03-31 17:00:42.024311 foursight_core-4.1.0.5b12/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2022-09-07 10:08:59.761273 foursight_core-4.1.0.5b12/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-03-30 11:22:44.922849 foursight_core-4.1.0.5b12/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-03-30 11:22:44.923050 foursight_core-4.1.0.5b12/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2022-09-07 10:08:59.761552 foursight_core-4.1.0.5b12/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-03-31 17:00:42.024438 foursight_core-4.1.0.5b12/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-03-31 17:00:42.024598 foursight_core-4.1.0.5b12/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0     1292 2023-04-19 11:31:51.999612 foursight_core-4.1.0.5b12/foursight_core/checks/x
--rw-r--r--   0        0        0    11437 2022-11-20 14:31:38.983954 foursight_core-4.1.0.5b12/foursight_core/d
--rw-r--r--   0        0        0    11929 2023-03-31 17:00:42.024812 foursight_core-4.1.0.5b12/foursight_core/decorators.py
--rw-r--r--   0        0        0    12565 2022-11-28 19:43:36.821773 foursight_core-4.1.0.5b12/foursight_core/decorators.py-new
--rw-r--r--   0        0        0    15050 2023-03-31 17:00:42.025145 foursight_core-4.1.0.5b12/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-04-16 04:32:00.359540 foursight_core-4.1.0.5b12/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-03-31 17:00:42.025932 foursight_core-4.1.0.5b12/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2022-09-07 10:08:59.762246 foursight_core-4.1.0.5b12/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5146 2023-04-10 14:14:30.704795 foursight_core-4.1.0.5b12/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-04-10 14:14:30.705142 foursight_core-4.1.0.5b12/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-03-31 17:00:42.026791 foursight_core-4.1.0.5b12/foursight_core/mapping.json
--rw-r--r--   0        0        0    95074 2022-11-15 14:26:15.846985 foursight_core-4.1.0.5b12/foursight_core/okk
--rw-r--r--   0        0        0     1014 2023-03-30 11:22:44.924884 foursight_core-4.1.0.5b12/foursight_core/package.py
--rw-r--r--   0        0        0     4846 2022-10-18 15:27:01.122701 foursight_core-4.1.0.5b12/foursight_core/react/api/'
--rw-r--r--   0        0        0    26281 2022-12-06 19:54:26.692542 foursight_core-4.1.0.5b12/foursight_core/react/api/:w
--rw-r--r--   0        0        0     5122 2022-10-19 18:25:39.526281 foursight_core-4.1.0.5b12/foursight_core/react/api/]:w
--rw-r--r--   0        0        0        0 2023-04-22 12:48:27.827660 foursight_core-4.1.0.5b12/foursight_core/react/api/a
--rw-r--r--   0        0        0    16866 2022-10-19 15:30:53.424281 foursight_core-4.1.0.5b12/foursight_core/react/api/adsfa
--rw-r--r--   0        0        0    46462 2022-11-19 15:11:20.178519 foursight_core-4.1.0.5b12/foursight_core/react/api/alkd
--rw-r--r--   0        0        0    32044 2022-10-21 15:56:11.928913 foursight_core-4.1.0.5b12/foursight_core/react/api/asav
--rw-r--r--   0        0        0    28883 2022-10-19 18:32:59.913329 foursight_core-4.1.0.5b12/foursight_core/react/api/asdf
--rw-r--r--   0        0        0     2582 2023-04-19 15:51:21.736937 foursight_core-4.1.0.5b12/foursight_core/react/api/asdfasdf
--rw-r--r--   0        0        0    12150 2022-12-08 18:15:25.696290 foursight_core-4.1.0.5b12/foursight_core/react/api/asdff
--rw-r--r--   0        0        0    17014 2023-04-22 17:35:00.396862 foursight_core-4.1.0.5b12/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0    14143 2023-03-31 15:18:53.676413 foursight_core-4.1.0.5b12/foursight_core/react/api/auth.py-deb
--rw-r--r--   0        0        0     7091 2023-04-16 14:14:05.368090 foursight_core-4.1.0.5b12/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0     1163 2022-12-26 13:33:51.355358 foursight_core-4.1.0.5b12/foursight_core/react/api/aws_logs.py
--rw-r--r--   0        0        0    23203 2023-03-31 17:00:42.028111 foursight_core-4.1.0.5b12/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-03-31 17:00:42.028307 foursight_core-4.1.0.5b12/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6315 2023-03-31 17:00:42.028636 foursight_core-4.1.0.5b12/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28316 2023-03-31 17:00:42.029013 foursight_core-4.1.0.5b12/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    30044 2023-01-03 14:40:15.527405 foursight_core-4.1.0.5b12/foursight_core/react/api/checks.py---
--rw-r--r--   0        0        0    28530 2022-12-07 15:57:38.726495 foursight_core-4.1.0.5b12/foursight_core/react/api/checks.py-new
--rw-r--r--   0        0        0    20652 2023-03-31 17:00:42.029767 foursight_core-4.1.0.5b12/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3459 2023-04-18 14:46:47.694282 foursight_core-4.1.0.5b12/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     5745 2023-03-31 17:00:42.030106 foursight_core-4.1.0.5b12/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-03-31 17:00:42.030271 foursight_core-4.1.0.5b12/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-03-31 17:00:42.030388 foursight_core-4.1.0.5b12/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4878 2023-04-21 20:12:47.966508 foursight_core-4.1.0.5b12/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0    58991 2022-12-25 17:24:38.880437 foursight_core-4.1.0.5b12/foursight_core/react/api/foo
--rw-r--r--   0        0        0     3257 2023-03-31 17:00:42.030761 foursight_core-4.1.0.5b12/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0    13097 2022-11-07 19:29:38.049301 foursight_core-4.1.0.5b12/foursight_core/react/api/hama
--rw-r--r--   0        0        0    44446 2022-11-18 16:41:20.868752 foursight_core-4.1.0.5b12/foursight_core/react/api/hmm
--rw-r--r--   0        0        0     3516 2023-03-31 17:00:42.030910 foursight_core-4.1.0.5b12/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9524 2023-03-31 17:00:42.031263 foursight_core-4.1.0.5b12/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0    14646 2022-10-23 19:06:03.352206 foursight_core-4.1.0.5b12/foursight_core/react/api/ok
--rw-r--r--   0        0        0    27126 2022-12-07 16:03:28.375164 foursight_core-4.1.0.5b12/foursight_core/react/api/oklk
--rw-r--r--   0        0        0    17397 2022-10-19 18:57:09.208083 foursight_core-4.1.0.5b12/foursight_core/react/api/okok
--rw-r--r--   0        0        0    15418 2022-10-23 19:08:13.968538 foursight_core-4.1.0.5b12/foursight_core/react/api/okokok
--rw-r--r--   0        0        0    37016 2022-11-12 14:03:53.287757 foursight_core-4.1.0.5b12/foursight_core/react/api/okokokok
--rw-r--r--   0        0        0    39205 2022-11-12 19:00:46.033390 foursight_core-4.1.0.5b12/foursight_core/react/api/okokokokok
--rw-r--r--   0        0        0    29102 2022-12-07 19:03:24.489085 foursight_core-4.1.0.5b12/foursight_core/react/api/ot
--rw-r--r--   0        0        0     3862 2023-04-21 03:15:59.228651 foursight_core-4.1.0.5b12/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    77827 2023-04-21 20:10:16.814770 foursight_core-4.1.0.5b12/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    45701 2022-10-21 14:29:00.904736 foursight_core-4.1.0.5b12/foursight_core/react/api/react_api.py-
--rw-r--r--   0        0        0    30313 2022-10-21 17:36:32.520832 foursight_core-4.1.0.5b12/foursight_core/react/api/react_api.py--
--rw-r--r--   0        0        0    71345 2023-01-23 23:30:44.383522 foursight_core-4.1.0.5b12/foursight_core/react/api/react_api.py----
--rw-r--r--   0        0        0    46990 2022-11-22 14:51:44.189069 foursight_core-4.1.0.5b12/foursight_core/react/api/react_api.py-deb
--rw-r--r--   0        0        0    24458 2022-10-22 23:24:49.505751 foursight_core-4.1.0.5b12/foursight_core/react/api/react_api.py-saaave
--rw-r--r--   0        0        0    11353 2023-04-21 19:21:13.190302 foursight_core-4.1.0.5b12/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0    11721 2023-03-31 15:18:58.965799 foursight_core-4.1.0.5b12/foursight_core/react/api/react_api_base.py-deb
--rw-r--r--   0        0        0    10435 2022-10-22 23:25:02.692255 foursight_core-4.1.0.5b12/foursight_core/react/api/react_app.py-saaave
--rw-r--r--   0        0        0     8025 2023-03-31 17:00:42.033249 foursight_core-4.1.0.5b12/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0     5576 2022-10-19 22:12:16.865537 foursight_core-4.1.0.5b12/foursight_core/react/api/react_route_utils.py-
--rw-r--r--   0        0        0     7471 2022-10-22 19:19:42.543417 foursight_core-4.1.0.5b12/foursight_core/react/api/react_route_utils.py.save
--rw-r--r--   0        0        0    32302 2023-04-20 18:33:16.326327 foursight_core-4.1.0.5b12/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0    12876 2022-10-22 19:00:58.268720 foursight_core-4.1.0.5b12/foursight_core/react/api/react_routes.py.save
--rw-r--r--   0        0        0     4861 2023-03-31 17:00:42.034179 foursight_core-4.1.0.5b12/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0     5027 2022-10-17 22:40:41.733498 foursight_core-4.1.0.5b12/foursight_core/react/api/react_ui.py-bak
--rw-r--r--   0        0        0     4206 2022-10-17 22:47:29.529384 foursight_core-4.1.0.5b12/foursight_core/react/api/react_ui.py-debug
--rw-r--r--   0        0        0    56415 2022-12-15 17:41:55.903970 foursight_core-4.1.0.5b12/foursight_core/react/api/sa
--rw-r--r--   0        0        0    42517 2022-11-15 20:10:51.305457 foursight_core-4.1.0.5b12/foursight_core/react/api/sav
--rw-r--r--   0        0        0    16885 2022-10-19 15:44:40.693752 foursight_core-4.1.0.5b12/foursight_core/react/api/save
--rw-r--r--   0        0        0     1977 2023-04-20 20:15:19.741349 foursight_core-4.1.0.5b12/foursight_core/react/api/x
--rw-r--r--   0        0        0    31785 2022-10-21 15:29:37.208969 foursight_core-4.1.0.5b12/foursight_core/react/api/xx
--rw-r--r--   0        0        0     5648 2023-04-19 14:58:25.494220 foursight_core-4.1.0.5b12/foursight_core/react/api/xxx
--rw-r--r--   0        0        0    56739 2022-12-15 20:17:56.533252 foursight_core-4.1.0.5b12/foursight_core/react/api/xxy
--rw-r--r--   0        0        0     5921 2022-10-21 16:32:06.326758 foursight_core-4.1.0.5b12/foursight_core/react/api/xyz
--rw-r--r--   0        0        0      806 2023-03-31 17:00:42.034293 foursight_core-4.1.0.5b12/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-04-22 15:42:04.085444 foursight_core-4.1.0.5b12/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-04-22 15:42:04.082976 foursight_core-4.1.0.5b12/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-04-22 15:41:55.537258 foursight_core-4.1.0.5b12/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11786 2023-04-22 15:55:41.831738 foursight_core-4.1.0.5b12/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1927830 2023-04-22 15:55:41.838030 foursight_core-4.1.0.5b12/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-03-31 17:00:42.046642 foursight_core-4.1.0.5b12/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-03-31 17:00:42.047578 foursight_core-4.1.0.5b12/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-03-31 17:00:42.047831 foursight_core-4.1.0.5b12/foursight_core/run_result.py
--rw-r--r--   0        0        0    22924 2022-11-21 20:22:40.475142 foursight_core-4.1.0.5b12/foursight_core/run_result.py-deb
--rw-r--r--   0        0        0     6330 2023-03-31 17:00:42.048014 foursight_core-4.1.0.5b12/foursight_core/s3_connection.py
--rw-r--r--   0        0        0    95791 2022-11-15 19:33:17.290307 foursight_core-4.1.0.5b12/foursight_core/sav
--rw-r--r--   0        0        0     5282 2023-03-31 17:00:42.048163 foursight_core-4.1.0.5b12/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     6458 2022-11-04 14:38:30.182413 foursight_core-4.1.0.5b12/foursight_core/schedule_decorator.py-
--rw-r--r--   0        0        0     1402 2023-03-31 17:00:42.048268 foursight_core-4.1.0.5b12/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-03-31 17:00:42.048339 foursight_core-4.1.0.5b12/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0       65 2022-11-14 16:31:57.489442 foursight_core-4.1.0.5b12/foursight_core/scripts/p
--rw-r--r--   0        0        0      797 2022-11-17 17:02:52.436871 foursight_core-4.1.0.5b12/foursight_core/scripts/save/decrypt_accounts_file.py
--rw-r--r--   0        0        0      801 2022-11-17 17:02:55.810728 foursight_core-4.1.0.5b12/foursight_core/scripts/save/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-03-31 17:00:42.048769 foursight_core-4.1.0.5b12/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-03-30 11:23:29.553404 foursight_core-4.1.0.5b12/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-03-30 11:26:56.704948 foursight_core-4.1.0.5b12/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-04-10 14:14:30.716241 foursight_core-4.1.0.5b12/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2022-09-07 10:08:59.763471 foursight_core-4.1.0.5b12/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-03-30 11:28:21.582264 foursight_core-4.1.0.5b12/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2022-09-07 10:08:59.763671 foursight_core-4.1.0.5b12/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-03-30 11:26:56.705625 foursight_core-4.1.0.5b12/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-03-30 11:26:56.705764 foursight_core-4.1.0.5b12/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-03-30 11:26:56.706033 foursight_core-4.1.0.5b12/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-03-30 11:26:56.706216 foursight_core-4.1.0.5b12/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1489 2023-03-29 22:45:57.789020 foursight_core-4.1.0.5b12/foursight_core/x
--rw-r--r--   0        0        0      231 2023-02-23 19:48:15.449939 foursight_core-4.1.0.5b12/foursight_core/x.py]
--rw-r--r--   0        0        0     1549 2023-04-23 14:13:48.228050 foursight_core-4.1.0.5b12/pyproject.toml
--rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 foursight_core-4.1.0.5b12/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-07 10:08:59.753994 foursight_core-4.1.0.5b13/LICENSE.txt
+-rw-r--r--   0        0        0    10825 2022-11-20 13:33:58.544911 foursight_core-4.1.0.5b13/foursight_core/'
+-rw-r--r--   0        0        0        0 2022-09-07 10:08:59.760120 foursight_core-4.1.0.5b13/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-03-30 11:22:44.920863 foursight_core-4.1.0.5b13/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0     8523 2023-02-23 17:12:48.834947 foursight_core-4.1.0.5b13/foursight_core/adfasdfad
+-rw-r--r--   0        0        0       69 2023-04-16 14:05:52.759877 foursight_core-4.1.0.5b13/foursight_core/app.py
+-rw-r--r--   0        0        0   105730 2023-04-16 14:04:58.418881 foursight_core-4.1.0.5b13/foursight_core/app_utils.py
+-rw-r--r--   0        0        0   101241 2022-12-02 19:01:09.085977 foursight_core-4.1.0.5b13/foursight_core/app_utils.py---
+-rw-r--r--   0        0        0    97799 2022-11-22 14:52:55.397982 foursight_core-4.1.0.5b13/foursight_core/app_utils.py-deb
+-rw-r--r--   0        0        0    97949 2022-11-23 13:18:09.708092 foursight_core-4.1.0.5b13/foursight_core/app_utils.py-debug
+-rw-r--r--   0        0        0   101943 2023-03-29 22:48:31.801408 foursight_core-4.1.0.5b13/foursight_core/app_utils.py-debugg
+-rw-r--r--   0        0        0    12620 2022-11-30 14:04:39.423857 foursight_core-4.1.0.5b13/foursight_core/asdf
+-rw-r--r--   0        0        0     2571 2023-03-30 11:22:44.922092 foursight_core-4.1.0.5b13/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2022-09-07 10:08:59.760846 foursight_core-4.1.0.5b13/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2022-09-07 10:08:59.760916 foursight_core-4.1.0.5b13/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-03-31 17:00:42.022944 foursight_core-4.1.0.5b13/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-03-30 11:22:44.922592 foursight_core-4.1.0.5b13/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     4452 2023-04-20 18:26:30.344734 foursight_core-4.1.0.5b13/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-03-31 17:00:42.023738 foursight_core-4.1.0.5b13/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-03-31 17:00:42.024190 foursight_core-4.1.0.5b13/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-03-31 17:00:42.024311 foursight_core-4.1.0.5b13/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2022-09-07 10:08:59.761273 foursight_core-4.1.0.5b13/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-03-30 11:22:44.922849 foursight_core-4.1.0.5b13/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-03-30 11:22:44.923050 foursight_core-4.1.0.5b13/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2022-09-07 10:08:59.761552 foursight_core-4.1.0.5b13/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-03-31 17:00:42.024438 foursight_core-4.1.0.5b13/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-03-31 17:00:42.024598 foursight_core-4.1.0.5b13/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0     1292 2023-04-19 11:31:51.999612 foursight_core-4.1.0.5b13/foursight_core/checks/x
+-rw-r--r--   0        0        0    11437 2022-11-20 14:31:38.983954 foursight_core-4.1.0.5b13/foursight_core/d
+-rw-r--r--   0        0        0    11929 2023-03-31 17:00:42.024812 foursight_core-4.1.0.5b13/foursight_core/decorators.py
+-rw-r--r--   0        0        0    12565 2022-11-28 19:43:36.821773 foursight_core-4.1.0.5b13/foursight_core/decorators.py-new
+-rw-r--r--   0        0        0    15050 2023-03-31 17:00:42.025145 foursight_core-4.1.0.5b13/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-04-16 04:32:00.359540 foursight_core-4.1.0.5b13/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-03-31 17:00:42.025932 foursight_core-4.1.0.5b13/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2022-09-07 10:08:59.762246 foursight_core-4.1.0.5b13/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5146 2023-04-10 14:14:30.704795 foursight_core-4.1.0.5b13/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-04-10 14:14:30.705142 foursight_core-4.1.0.5b13/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-03-31 17:00:42.026791 foursight_core-4.1.0.5b13/foursight_core/mapping.json
+-rw-r--r--   0        0        0    95074 2022-11-15 14:26:15.846985 foursight_core-4.1.0.5b13/foursight_core/okk
+-rw-r--r--   0        0        0     1014 2023-03-30 11:22:44.924884 foursight_core-4.1.0.5b13/foursight_core/package.py
+-rw-r--r--   0        0        0     4846 2022-10-18 15:27:01.122701 foursight_core-4.1.0.5b13/foursight_core/react/api/'
+-rw-r--r--   0        0        0    26281 2022-12-06 19:54:26.692542 foursight_core-4.1.0.5b13/foursight_core/react/api/:w
+-rw-r--r--   0        0        0     5122 2022-10-19 18:25:39.526281 foursight_core-4.1.0.5b13/foursight_core/react/api/]:w
+-rw-r--r--   0        0        0        0 2023-04-22 12:48:27.827660 foursight_core-4.1.0.5b13/foursight_core/react/api/a
+-rw-r--r--   0        0        0    16866 2022-10-19 15:30:53.424281 foursight_core-4.1.0.5b13/foursight_core/react/api/adsfa
+-rw-r--r--   0        0        0    46462 2022-11-19 15:11:20.178519 foursight_core-4.1.0.5b13/foursight_core/react/api/alkd
+-rw-r--r--   0        0        0    32044 2022-10-21 15:56:11.928913 foursight_core-4.1.0.5b13/foursight_core/react/api/asav
+-rw-r--r--   0        0        0    28883 2022-10-19 18:32:59.913329 foursight_core-4.1.0.5b13/foursight_core/react/api/asdf
+-rw-r--r--   0        0        0     2582 2023-04-19 15:51:21.736937 foursight_core-4.1.0.5b13/foursight_core/react/api/asdfasdf
+-rw-r--r--   0        0        0    12150 2022-12-08 18:15:25.696290 foursight_core-4.1.0.5b13/foursight_core/react/api/asdff
+-rw-r--r--   0        0        0    17014 2023-04-22 17:35:00.396862 foursight_core-4.1.0.5b13/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0    14143 2023-03-31 15:18:53.676413 foursight_core-4.1.0.5b13/foursight_core/react/api/auth.py-deb
+-rw-r--r--   0        0        0     7091 2023-04-16 14:14:05.368090 foursight_core-4.1.0.5b13/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0     1163 2022-12-26 13:33:51.355358 foursight_core-4.1.0.5b13/foursight_core/react/api/aws_logs.py
+-rw-r--r--   0        0        0    23203 2023-03-31 17:00:42.028111 foursight_core-4.1.0.5b13/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-03-31 17:00:42.028307 foursight_core-4.1.0.5b13/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6315 2023-03-31 17:00:42.028636 foursight_core-4.1.0.5b13/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28316 2023-03-31 17:00:42.029013 foursight_core-4.1.0.5b13/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    30044 2023-01-03 14:40:15.527405 foursight_core-4.1.0.5b13/foursight_core/react/api/checks.py---
+-rw-r--r--   0        0        0    28530 2022-12-07 15:57:38.726495 foursight_core-4.1.0.5b13/foursight_core/react/api/checks.py-new
+-rw-r--r--   0        0        0    20652 2023-03-31 17:00:42.029767 foursight_core-4.1.0.5b13/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3459 2023-04-18 14:46:47.694282 foursight_core-4.1.0.5b13/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     5745 2023-03-31 17:00:42.030106 foursight_core-4.1.0.5b13/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-03-31 17:00:42.030271 foursight_core-4.1.0.5b13/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-03-31 17:00:42.030388 foursight_core-4.1.0.5b13/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4878 2023-04-21 20:12:47.966508 foursight_core-4.1.0.5b13/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0    58991 2022-12-25 17:24:38.880437 foursight_core-4.1.0.5b13/foursight_core/react/api/foo
+-rw-r--r--   0        0        0     3257 2023-03-31 17:00:42.030761 foursight_core-4.1.0.5b13/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0    13097 2022-11-07 19:29:38.049301 foursight_core-4.1.0.5b13/foursight_core/react/api/hama
+-rw-r--r--   0        0        0    44446 2022-11-18 16:41:20.868752 foursight_core-4.1.0.5b13/foursight_core/react/api/hmm
+-rw-r--r--   0        0        0     3516 2023-03-31 17:00:42.030910 foursight_core-4.1.0.5b13/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9524 2023-03-31 17:00:42.031263 foursight_core-4.1.0.5b13/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0    14646 2022-10-23 19:06:03.352206 foursight_core-4.1.0.5b13/foursight_core/react/api/ok
+-rw-r--r--   0        0        0    27126 2022-12-07 16:03:28.375164 foursight_core-4.1.0.5b13/foursight_core/react/api/oklk
+-rw-r--r--   0        0        0    17397 2022-10-19 18:57:09.208083 foursight_core-4.1.0.5b13/foursight_core/react/api/okok
+-rw-r--r--   0        0        0    15418 2022-10-23 19:08:13.968538 foursight_core-4.1.0.5b13/foursight_core/react/api/okokok
+-rw-r--r--   0        0        0    37016 2022-11-12 14:03:53.287757 foursight_core-4.1.0.5b13/foursight_core/react/api/okokokok
+-rw-r--r--   0        0        0    39205 2022-11-12 19:00:46.033390 foursight_core-4.1.0.5b13/foursight_core/react/api/okokokokok
+-rw-r--r--   0        0        0    29102 2022-12-07 19:03:24.489085 foursight_core-4.1.0.5b13/foursight_core/react/api/ot
+-rw-r--r--   0        0        0     3862 2023-04-21 03:15:59.228651 foursight_core-4.1.0.5b13/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    77827 2023-04-21 20:10:16.814770 foursight_core-4.1.0.5b13/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    45701 2022-10-21 14:29:00.904736 foursight_core-4.1.0.5b13/foursight_core/react/api/react_api.py-
+-rw-r--r--   0        0        0    30313 2022-10-21 17:36:32.520832 foursight_core-4.1.0.5b13/foursight_core/react/api/react_api.py--
+-rw-r--r--   0        0        0    71345 2023-01-23 23:30:44.383522 foursight_core-4.1.0.5b13/foursight_core/react/api/react_api.py----
+-rw-r--r--   0        0        0    46990 2022-11-22 14:51:44.189069 foursight_core-4.1.0.5b13/foursight_core/react/api/react_api.py-deb
+-rw-r--r--   0        0        0    24458 2022-10-22 23:24:49.505751 foursight_core-4.1.0.5b13/foursight_core/react/api/react_api.py-saaave
+-rw-r--r--   0        0        0    11353 2023-04-21 19:21:13.190302 foursight_core-4.1.0.5b13/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0    11721 2023-03-31 15:18:58.965799 foursight_core-4.1.0.5b13/foursight_core/react/api/react_api_base.py-deb
+-rw-r--r--   0        0        0    10435 2022-10-22 23:25:02.692255 foursight_core-4.1.0.5b13/foursight_core/react/api/react_app.py-saaave
+-rw-r--r--   0        0        0     8025 2023-03-31 17:00:42.033249 foursight_core-4.1.0.5b13/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0     5576 2022-10-19 22:12:16.865537 foursight_core-4.1.0.5b13/foursight_core/react/api/react_route_utils.py-
+-rw-r--r--   0        0        0     7471 2022-10-22 19:19:42.543417 foursight_core-4.1.0.5b13/foursight_core/react/api/react_route_utils.py.save
+-rw-r--r--   0        0        0    32302 2023-04-20 18:33:16.326327 foursight_core-4.1.0.5b13/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0    12876 2022-10-22 19:00:58.268720 foursight_core-4.1.0.5b13/foursight_core/react/api/react_routes.py.save
+-rw-r--r--   0        0        0     4861 2023-03-31 17:00:42.034179 foursight_core-4.1.0.5b13/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0     5027 2022-10-17 22:40:41.733498 foursight_core-4.1.0.5b13/foursight_core/react/api/react_ui.py-bak
+-rw-r--r--   0        0        0     4206 2022-10-17 22:47:29.529384 foursight_core-4.1.0.5b13/foursight_core/react/api/react_ui.py-debug
+-rw-r--r--   0        0        0    56415 2022-12-15 17:41:55.903970 foursight_core-4.1.0.5b13/foursight_core/react/api/sa
+-rw-r--r--   0        0        0    42517 2022-11-15 20:10:51.305457 foursight_core-4.1.0.5b13/foursight_core/react/api/sav
+-rw-r--r--   0        0        0    16885 2022-10-19 15:44:40.693752 foursight_core-4.1.0.5b13/foursight_core/react/api/save
+-rw-r--r--   0        0        0     1977 2023-04-20 20:15:19.741349 foursight_core-4.1.0.5b13/foursight_core/react/api/x
+-rw-r--r--   0        0        0    31785 2022-10-21 15:29:37.208969 foursight_core-4.1.0.5b13/foursight_core/react/api/xx
+-rw-r--r--   0        0        0     5648 2023-04-19 14:58:25.494220 foursight_core-4.1.0.5b13/foursight_core/react/api/xxx
+-rw-r--r--   0        0        0    56739 2022-12-15 20:17:56.533252 foursight_core-4.1.0.5b13/foursight_core/react/api/xxy
+-rw-r--r--   0        0        0     5921 2022-10-21 16:32:06.326758 foursight_core-4.1.0.5b13/foursight_core/react/api/xyz
+-rw-r--r--   0        0        0      806 2023-03-31 17:00:42.034293 foursight_core-4.1.0.5b13/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-04-22 15:42:04.085444 foursight_core-4.1.0.5b13/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-04-22 15:42:04.082976 foursight_core-4.1.0.5b13/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-04-22 15:41:55.537258 foursight_core-4.1.0.5b13/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11786 2023-04-22 15:55:41.831738 foursight_core-4.1.0.5b13/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1927830 2023-04-22 15:55:41.838030 foursight_core-4.1.0.5b13/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-03-31 17:00:42.046642 foursight_core-4.1.0.5b13/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-03-31 17:00:42.047578 foursight_core-4.1.0.5b13/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-03-31 17:00:42.047831 foursight_core-4.1.0.5b13/foursight_core/run_result.py
+-rw-r--r--   0        0        0    22924 2022-11-21 20:22:40.475142 foursight_core-4.1.0.5b13/foursight_core/run_result.py-deb
+-rw-r--r--   0        0        0     6330 2023-03-31 17:00:42.048014 foursight_core-4.1.0.5b13/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0    95791 2022-11-15 19:33:17.290307 foursight_core-4.1.0.5b13/foursight_core/sav
+-rw-r--r--   0        0        0     5282 2023-03-31 17:00:42.048163 foursight_core-4.1.0.5b13/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     6458 2022-11-04 14:38:30.182413 foursight_core-4.1.0.5b13/foursight_core/schedule_decorator.py-
+-rw-r--r--   0        0        0     1402 2023-03-31 17:00:42.048268 foursight_core-4.1.0.5b13/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-03-31 17:00:42.048339 foursight_core-4.1.0.5b13/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0       65 2022-11-14 16:31:57.489442 foursight_core-4.1.0.5b13/foursight_core/scripts/p
+-rw-r--r--   0        0        0      797 2022-11-17 17:02:52.436871 foursight_core-4.1.0.5b13/foursight_core/scripts/save/decrypt_accounts_file.py
+-rw-r--r--   0        0        0      801 2022-11-17 17:02:55.810728 foursight_core-4.1.0.5b13/foursight_core/scripts/save/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-03-31 17:00:42.048769 foursight_core-4.1.0.5b13/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-03-30 11:23:29.553404 foursight_core-4.1.0.5b13/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-03-30 11:26:56.704948 foursight_core-4.1.0.5b13/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-04-10 14:14:30.716241 foursight_core-4.1.0.5b13/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2022-09-07 10:08:59.763471 foursight_core-4.1.0.5b13/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-03-30 11:28:21.582264 foursight_core-4.1.0.5b13/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2022-09-07 10:08:59.763671 foursight_core-4.1.0.5b13/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-03-30 11:26:56.705625 foursight_core-4.1.0.5b13/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-03-30 11:26:56.705764 foursight_core-4.1.0.5b13/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-03-30 11:26:56.706033 foursight_core-4.1.0.5b13/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-03-30 11:26:56.706216 foursight_core-4.1.0.5b13/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1489 2023-03-29 22:45:57.789020 foursight_core-4.1.0.5b13/foursight_core/x
+-rw-r--r--   0        0        0      231 2023-02-23 19:48:15.449939 foursight_core-4.1.0.5b13/foursight_core/x.py]
+-rw-r--r--   0        0        0     1549 2023-04-23 14:17:08.351887 foursight_core-4.1.0.5b13/pyproject.toml
+-rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 foursight_core-4.1.0.5b13/PKG-INFO
```

### Comparing `foursight_core-4.1.0.5b12/LICENSE.txt` & `foursight_core-4.1.0.5b13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/'` & `foursight_core-4.1.0.5b13/foursight_core/'`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/abstract_connection.py` & `foursight_core-4.1.0.5b13/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/adfasdfad` & `foursight_core-4.1.0.5b13/foursight_core/adfasdfad`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/app_utils.py` & `foursight_core-4.1.0.5b13/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/app_utils.py---` & `foursight_core-4.1.0.5b13/foursight_core/app_utils.py---`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/app_utils.py-deb` & `foursight_core-4.1.0.5b13/foursight_core/app_utils.py-deb`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/app_utils.py-debug` & `foursight_core-4.1.0.5b13/foursight_core/app_utils.py-debug`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/app_utils.py-debugg` & `foursight_core-4.1.0.5b13/foursight_core/app_utils.py-debugg`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/asdf` & `foursight_core-4.1.0.5b13/foursight_core/asdf`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/buckets.py` & `foursight_core-4.1.0.5b13/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/check_schema.py` & `foursight_core-4.1.0.5b13/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/check_utils.py` & `foursight_core-4.1.0.5b13/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.1.0.5b13/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.1.0.5b13/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/checks/ecs_checks.py` & `foursight_core-4.1.0.5b13/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.1.0.5b13/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.1.0.5b13/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.1.0.5b13/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/checks/scaling_checks.py` & `foursight_core-4.1.0.5b13/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/checks/test_checks.py` & `foursight_core-4.1.0.5b13/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/checks/x` & `foursight_core-4.1.0.5b13/foursight_core/checks/x`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/d` & `foursight_core-4.1.0.5b13/foursight_core/d`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/decorators.py` & `foursight_core-4.1.0.5b13/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/decorators.py-new` & `foursight_core-4.1.0.5b13/foursight_core/decorators.py-new`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/deploy.py` & `foursight_core-4.1.0.5b13/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/environment.py` & `foursight_core-4.1.0.5b13/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/es_connection.py` & `foursight_core-4.1.0.5b13/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/exceptions.py` & `foursight_core-4.1.0.5b13/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/fs_connection.py` & `foursight_core-4.1.0.5b13/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/identity.py` & `foursight_core-4.1.0.5b13/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/mapping.json` & `foursight_core-4.1.0.5b13/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/okk` & `foursight_core-4.1.0.5b13/foursight_core/okk`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/package.py` & `foursight_core-4.1.0.5b13/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/'` & `foursight_core-4.1.0.5b13/foursight_core/react/api/'`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/:w` & `foursight_core-4.1.0.5b13/foursight_core/react/api/:w`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/]:w` & `foursight_core-4.1.0.5b13/foursight_core/react/api/]:w`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/adsfa` & `foursight_core-4.1.0.5b13/foursight_core/react/api/adsfa`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/alkd` & `foursight_core-4.1.0.5b13/foursight_core/react/api/alkd`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/asav` & `foursight_core-4.1.0.5b13/foursight_core/react/api/asav`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/asdf` & `foursight_core-4.1.0.5b13/foursight_core/react/api/asdf`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/asdfasdf` & `foursight_core-4.1.0.5b13/foursight_core/react/api/asdfasdf`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/asdff` & `foursight_core-4.1.0.5b13/foursight_core/react/api/asdff`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/auth.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/auth.py-deb` & `foursight_core-4.1.0.5b13/foursight_core/react/api/auth.py-deb`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/auth0_config.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/aws_logs.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/aws_logs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/aws_network.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/aws_s3.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/checks.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/checks.py---` & `foursight_core-4.1.0.5b13/foursight_core/react/api/checks.py---`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/checks.py-new` & `foursight_core-4.1.0.5b13/foursight_core/react/api/checks.py-new`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/cognito.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/encryption.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/envs.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/foo` & `foursight_core-4.1.0.5b13/foursight_core/react/api/foo`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/gac.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/hama` & `foursight_core-4.1.0.5b13/foursight_core/react/api/hama`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/hmm` & `foursight_core-4.1.0.5b13/foursight_core/react/api/hmm`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/misc_utils.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/ok` & `foursight_core-4.1.0.5b13/foursight_core/react/api/ok`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/oklk` & `foursight_core-4.1.0.5b13/foursight_core/react/api/oklk`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/okok` & `foursight_core-4.1.0.5b13/foursight_core/react/api/okok`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/okokok` & `foursight_core-4.1.0.5b13/foursight_core/react/api/okokok`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/okokokok` & `foursight_core-4.1.0.5b13/foursight_core/react/api/okokokok`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/okokokokok` & `foursight_core-4.1.0.5b13/foursight_core/react/api/okokokokok`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/ot` & `foursight_core-4.1.0.5b13/foursight_core/react/api/ot`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_api.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_api.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_api.py-` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_api.py-`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_api.py--` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_api.py--`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_api.py----` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_api.py----`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_api.py-deb` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_api.py-deb`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_api.py-saaave` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_api.py-saaave`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_api_base.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_api_base.py-deb` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_api_base.py-deb`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_app.py-saaave` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_app.py-saaave`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_route_utils.py-` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_route_utils.py-`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_route_utils.py.save` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_route_utils.py.save`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_routes.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_routes.py.save` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_routes.py.save`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_ui.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_ui.py-bak` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_ui.py-bak`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/react_ui.py-debug` & `foursight_core-4.1.0.5b13/foursight_core/react/api/react_ui.py-debug`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/sa` & `foursight_core-4.1.0.5b13/foursight_core/react/api/sa`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/sav` & `foursight_core-4.1.0.5b13/foursight_core/react/api/sav`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/save` & `foursight_core-4.1.0.5b13/foursight_core/react/api/save`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/x` & `foursight_core-4.1.0.5b13/foursight_core/react/api/x`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/xx` & `foursight_core-4.1.0.5b13/foursight_core/react/api/xx`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/xxx` & `foursight_core-4.1.0.5b13/foursight_core/react/api/xxx`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/xxy` & `foursight_core-4.1.0.5b13/foursight_core/react/api/xxy`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/xyz` & `foursight_core-4.1.0.5b13/foursight_core/react/api/xyz`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.1.0.5b13/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/ui/index.html` & `foursight_core-4.1.0.5b13/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.1.0.5b13/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.1.0.5b13/foursight_core/react/ui/static/js/main.js`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/route_prefixes.py` & `foursight_core-4.1.0.5b13/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/routes.py` & `foursight_core-4.1.0.5b13/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/run_result.py` & `foursight_core-4.1.0.5b13/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/run_result.py-deb` & `foursight_core-4.1.0.5b13/foursight_core/run_result.py-deb`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/s3_connection.py` & `foursight_core-4.1.0.5b13/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/sav` & `foursight_core-4.1.0.5b13/foursight_core/sav`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/schedule_decorator.py` & `foursight_core-4.1.0.5b13/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/schedule_decorator.py-` & `foursight_core-4.1.0.5b13/foursight_core/schedule_decorator.py-`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.1.0.5b13/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.1.0.5b13/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/scripts/save/decrypt_accounts_file.py` & `foursight_core-4.1.0.5b13/foursight_core/scripts/save/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/scripts/save/encrypt_accounts_file.py` & `foursight_core-4.1.0.5b13/foursight_core/scripts/save/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/sqs_utils.py` & `foursight_core-4.1.0.5b13/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/stage.py` & `foursight_core-4.1.0.5b13/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/templates/base.html` & `foursight_core-4.1.0.5b13/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/templates/header.html` & `foursight_core-4.1.0.5b13/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/templates/history.html` & `foursight_core-4.1.0.5b13/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/templates/info.html` & `foursight_core-4.1.0.5b13/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/templates/unused.html` & `foursight_core-4.1.0.5b13/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/templates/user.html` & `foursight_core-4.1.0.5b13/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/templates/users.html` & `foursight_core-4.1.0.5b13/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/templates/view_checks.html` & `foursight_core-4.1.0.5b13/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/templates/view_groups.html` & `foursight_core-4.1.0.5b13/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/foursight_core/x` & `foursight_core-4.1.0.5b13/foursight_core/x`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b12/pyproject.toml` & `foursight_core-4.1.0.5b13/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.1.0.5b12"
+version = "4.1.0.5b13"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.1.0.5b12/PKG-INFO` & `foursight_core-4.1.0.5b13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.1.0.5b12
+Version: 4.1.0.5b13
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

