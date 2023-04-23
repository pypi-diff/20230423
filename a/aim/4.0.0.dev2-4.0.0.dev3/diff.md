# Comparing `tmp/aim-4.0.0.dev2.tar.gz` & `tmp/aim-4.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aim-4.0.0.dev2.tar", last modified: Wed Apr  5 11:38:00 2023, max compression
+gzip compressed data, was "aim-4.0.0.dev3.tar", last modified: Mon Apr 10 17:48:51 2023, max compression
```

## Comparing `aim-4.0.0.dev2.tar` & `aim-4.0.0.dev3.tar`

### file list

```diff
@@ -1,460 +1,460 @@
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.768688 aim-4.0.0.dev2/
--rw-r--r--   0 github     (503) staff       (20)    11347 2022-08-06 00:13:01.000000 aim-4.0.0.dev2/LICENSE
--rw-r--r--   0 github     (503) staff       (20)      185 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/MANIFEST.in
--rw-r--r--   0 github     (503) staff       (20)    37083 2023-04-05 11:38:00.768831 aim-4.0.0.dev2/PKG-INFO
--rw-r--r--   0 github     (503) staff       (20)    36396 2023-03-24 14:18:45.000000 aim-4.0.0.dev2/README.md
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.686277 aim-4.0.0.dev2/aim/
--rw-r--r--   0 github     (503) staff       (20)       10 2023-04-05 11:37:51.000000 aim-4.0.0.dev2/aim/VERSION
--rw-r--r--   0 github     (503) staff       (20)      825 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/__about__.py
--rw-r--r--   0 github     (503) staff       (20)      377 2023-02-01 20:08:30.000000 aim-4.0.0.dev2/aim/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      183 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/__version__.py
--rw-r--r--   0 github     (503) staff       (20)      100 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/acme.py
--rw-r--r--   0 github     (503) staff       (20)       96 2022-05-06 13:59:46.000000 aim-4.0.0.dev2/aim/catboost.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.688501 aim-4.0.0.dev2/aim/cli/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1323 2023-01-24 20:09:40.000000 aim-4.0.0.dev2/aim/cli/cli.py
--rw-r--r--   0 github     (503) staff       (20)      166 2022-06-17 00:13:19.000000 aim-4.0.0.dev2/aim/cli/configs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.688947 aim-4.0.0.dev2/aim/cli/convert/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/convert/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2998 2022-08-20 12:34:00.000000 aim-4.0.0.dev2/aim/cli/convert/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.689946 aim-4.0.0.dev2/aim/cli/convert/processors/
--rw-r--r--   0 github     (503) staff       (20)      113 2022-08-20 12:34:00.000000 aim-4.0.0.dev2/aim/cli/convert/processors/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5914 2022-09-01 19:23:53.000000 aim-4.0.0.dev2/aim/cli/convert/processors/mlflow.py
--rw-r--r--   0 github     (503) staff       (20)    10372 2022-08-06 00:13:01.000000 aim-4.0.0.dev2/aim/cli/convert/processors/tensorboard.py
--rw-r--r--   0 github     (503) staff       (20)     6816 2023-01-04 20:08:59.000000 aim-4.0.0.dev2/aim/cli/convert/processors/wandb.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.690306 aim-4.0.0.dev2/aim/cli/init/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/init/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1592 2023-03-24 14:18:45.000000 aim-4.0.0.dev2/aim/cli/init/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.690650 aim-4.0.0.dev2/aim/cli/manager/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/manager/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3382 2022-08-11 13:58:02.000000 aim-4.0.0.dev2/aim/cli/manager/manager.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.690996 aim-4.0.0.dev2/aim/cli/reindex/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/reindex/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      736 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/cli/reindex/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.691599 aim-4.0.0.dev2/aim/cli/runs/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/runs/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     6621 2023-03-24 14:18:45.000000 aim-4.0.0.dev2/aim/cli/runs/commands.py
--rw-r--r--   0 github     (503) staff       (20)     2570 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/cli/runs/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.691937 aim-4.0.0.dev2/aim/cli/server/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/server/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3709 2023-03-24 14:18:45.000000 aim-4.0.0.dev2/aim/cli/server/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.692267 aim-4.0.0.dev2/aim/cli/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-06-17 00:13:19.000000 aim-4.0.0.dev2/aim/cli/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     7537 2023-03-24 14:18:45.000000 aim-4.0.0.dev2/aim/cli/storage/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.692627 aim-4.0.0.dev2/aim/cli/telemetry/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-24 20:09:40.000000 aim-4.0.0.dev2/aim/cli/telemetry/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      305 2023-01-24 20:09:40.000000 aim-4.0.0.dev2/aim/cli/telemetry/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.693280 aim-4.0.0.dev2/aim/cli/up/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/up/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5953 2023-01-24 20:09:40.000000 aim-4.0.0.dev2/aim/cli/up/commands.py
--rw-r--r--   0 github     (503) staff       (20)     1446 2022-06-21 18:01:08.000000 aim-4.0.0.dev2/aim/cli/up/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.693760 aim-4.0.0.dev2/aim/cli/upgrade/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/upgrade/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.694514 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/
--rw-r--r--   0 github     (503) staff       (20)      258 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      734 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/configs.py
--rw-r--r--   0 github     (503) staff       (20)      448 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/metric_artifact.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.695140 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      263 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/base_pb2.py
--rw-r--r--   0 github     (503) staff       (20)      267 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/metric_pb2.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.695638 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/v3/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/v3/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3396 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/v3/base_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     1919 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/v3/metric_pb2.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.696100 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/v4/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/v4/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1111 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/v4/base_pb2.py
--rw-r--r--   0 github     (503) staff       (20)      969 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/v4/metric_pb2.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.697270 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/repo/
--rw-r--r--   0 github     (503) staff       (20)        1 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/repo/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1722 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/repo/metric.py
--rw-r--r--   0 github     (503) staff       (20)     3722 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/repo/repo.py
--rw-r--r--   0 github     (503) staff       (20)     4062 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/repo/run.py
--rw-r--r--   0 github     (503) staff       (20)     1357 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/repo/trace.py
--rw-r--r--   0 github     (503) staff       (20)     1211 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/repo/utils.py
--rw-r--r--   0 github     (503) staff       (20)     6635 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/upgrade/utils.py
--rw-r--r--   0 github     (503) staff       (20)      370 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.697533 aim-4.0.0.dev2/aim/cli/version/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/version/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      149 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/cli/version/commands.py
--rw-r--r--   0 github     (503) staff       (20)     9960 2023-01-24 20:09:40.000000 aim-4.0.0.dev2/aim/cli/watcher_cli.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.698059 aim-4.0.0.dev2/aim/ext/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/ext/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.698307 aim-4.0.0.dev2/aim/ext/cleanup/
--rw-r--r--   0 github     (503) staff       (20)     3579 2022-11-12 00:14:35.000000 aim-4.0.0.dev2/aim/ext/cleanup/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2021 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/ext/exception_resistant.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.698647 aim-4.0.0.dev2/aim/ext/notebook/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/ext/notebook/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     7314 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/ext/notebook/notebook.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.700767 aim-4.0.0.dev2/aim/ext/notifier/
--rw-r--r--   0 github     (503) staff       (20)      589 2022-08-20 12:34:00.000000 aim-4.0.0.dev2/aim/ext/notifier/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      305 2022-08-20 12:34:00.000000 aim-4.0.0.dev2/aim/ext/notifier/base_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1858 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/ext/notifier/config.py
--rw-r--r--   0 github     (503) staff       (20)      361 2022-08-20 12:34:00.000000 aim-4.0.0.dev2/aim/ext/notifier/config_default.json
--rw-r--r--   0 github     (503) staff       (20)       70 2022-08-20 12:34:00.000000 aim-4.0.0.dev2/aim/ext/notifier/config_empty.json
--rw-r--r--   0 github     (503) staff       (20)      522 2022-08-20 12:34:00.000000 aim-4.0.0.dev2/aim/ext/notifier/logging_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1428 2022-08-20 12:34:00.000000 aim-4.0.0.dev2/aim/ext/notifier/notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1158 2022-08-20 12:34:00.000000 aim-4.0.0.dev2/aim/ext/notifier/notifier_builder.py
--rw-r--r--   0 github     (503) staff       (20)      524 2022-08-20 12:34:00.000000 aim-4.0.0.dev2/aim/ext/notifier/slack_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1034 2022-08-20 12:34:00.000000 aim-4.0.0.dev2/aim/ext/notifier/utils.py
--rw-r--r--   0 github     (503) staff       (20)      862 2022-08-20 12:34:00.000000 aim-4.0.0.dev2/aim/ext/notifier/workplace_notifier.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.702138 aim-4.0.0.dev2/aim/ext/resource/
--rw-r--r--   0 github     (503) staff       (20)       92 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/ext/resource/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      100 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/ext/resource/configs.py
--rw-r--r--   0 github     (503) staff       (20)      726 2022-05-16 21:25:24.000000 aim-4.0.0.dev2/aim/ext/resource/log.py
--rw-r--r--   0 github     (503) staff       (20)     6700 2023-01-04 20:08:59.000000 aim-4.0.0.dev2/aim/ext/resource/stat.py
--rw-r--r--   0 github     (503) staff       (20)     7511 2023-01-04 20:08:59.000000 aim-4.0.0.dev2/aim/ext/resource/tracker.py
--rw-r--r--   0 github     (503) staff       (20)       56 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/ext/resource/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.702417 aim-4.0.0.dev2/aim/ext/sshfs/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/ext/sshfs/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     7768 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/ext/sshfs/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.702686 aim-4.0.0.dev2/aim/ext/task_queue/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/ext/task_queue/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2069 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/ext/task_queue/queue.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.703264 aim-4.0.0.dev2/aim/ext/tensorboard_tracker/
--rw-r--r--   0 github     (503) staff       (20)       48 2023-01-04 20:08:59.000000 aim-4.0.0.dev2/aim/ext/tensorboard_tracker/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      919 2023-01-04 20:08:59.000000 aim-4.0.0.dev2/aim/ext/tensorboard_tracker/run.py
--rw-r--r--   0 github     (503) staff       (20)     7201 2023-01-04 20:08:59.000000 aim-4.0.0.dev2/aim/ext/tensorboard_tracker/tracker.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.706428 aim-4.0.0.dev2/aim/ext/transport/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/ext/transport/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    12932 2023-02-27 08:16:06.000000 aim-4.0.0.dev2/aim/ext/transport/client.py
--rw-r--r--   0 github     (503) staff       (20)      515 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/ext/transport/config.py
--rw-r--r--   0 github     (503) staff       (20)     3298 2023-01-23 20:08:00.000000 aim-4.0.0.dev2/aim/ext/transport/handlers.py
--rw-r--r--   0 github     (503) staff       (20)     5555 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/health.py
--rw-r--r--   0 github     (503) staff       (20)     5616 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/heartbeat.py
--rw-r--r--   0 github     (503) staff       (20)     3347 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/message_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.707755 aim-4.0.0.dev2/aim/ext/transport/proto/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      245 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/health_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     3991 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/health_pb2_grpc.py
--rw-r--r--   0 github     (503) staff       (20)      259 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/remote_router_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     8855 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/remote_router_pb2_grpc.py
--rw-r--r--   0 github     (503) staff       (20)      263 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/remote_tracking_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     9444 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/remote_tracking_pb2_grpc.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.708651 aim-4.0.0.dev2/aim/ext/transport/proto/v3/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/v3/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     6195 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/v3/health_pb2.py
--rw-r--r--   0 github     (503) staff       (20)    25245 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/v3/remote_router_pb2.py
--rw-r--r--   0 github     (503) staff       (20)    37567 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/v3/remote_tracking_pb2.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.709454 aim-4.0.0.dev2/aim/ext/transport/proto/v4/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/v4/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1749 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/v4/health_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     4280 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/v4/remote_router_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     5662 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/proto/v4/remote_tracking_pb2.py
--rw-r--r--   0 github     (503) staff       (20)      428 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/ext/transport/remote_resource.py
--rw-r--r--   0 github     (503) staff       (20)     8078 2023-01-23 10:30:27.000000 aim-4.0.0.dev2/aim/ext/transport/remote_tracking.py
--rw-r--r--   0 github     (503) staff       (20)     3637 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/router.py
--rw-r--r--   0 github     (503) staff       (20)     3728 2022-11-18 00:13:03.000000 aim-4.0.0.dev2/aim/ext/transport/rpc_queue.py
--rw-r--r--   0 github     (503) staff       (20)     4609 2023-01-23 10:30:27.000000 aim-4.0.0.dev2/aim/ext/transport/server.py
--rw-r--r--   0 github     (503) staff       (20)     3419 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/ext/transport/worker.py
--rw-r--r--   0 github     (503) staff       (20)     2103 2022-08-20 12:34:00.000000 aim-4.0.0.dev2/aim/ext/utils.py
--rw-r--r--   0 github     (503) staff       (20)       92 2022-09-25 12:02:15.000000 aim-4.0.0.dev2/aim/fastai.py
--rw-r--r--   0 github     (503) staff       (20)      127 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/hf_dataset.py
--rw-r--r--   0 github     (503) staff       (20)      105 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/hugging_face.py
--rw-r--r--   0 github     (503) staff       (20)      103 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/keras.py
--rw-r--r--   0 github     (503) staff       (20)      103 2022-08-20 12:34:00.000000 aim-4.0.0.dev2/aim/keras_tuner.py
--rw-r--r--   0 github     (503) staff       (20)       98 2022-05-06 13:59:46.000000 aim-4.0.0.dev2/aim/lightgbm.py
--rw-r--r--   0 github     (503) staff       (20)       97 2022-10-04 00:16:28.000000 aim-4.0.0.dev2/aim/mxnet.py
--rw-r--r--   0 github     (503) staff       (20)       98 2022-11-12 00:14:35.000000 aim-4.0.0.dev2/aim/optuna.py
--rw-r--r--   0 github     (503) staff       (20)       99 2022-11-12 00:14:35.000000 aim-4.0.0.dev2/aim/paddle.py
--rw-r--r--   0 github     (503) staff       (20)       93 2023-01-31 20:08:25.000000 aim-4.0.0.dev2/aim/prophet.py
--rw-r--r--   0 github     (503) staff       (20)      115 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/pytorch.py
--rw-r--r--   0 github     (503) staff       (20)      107 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/pytorch_ignite.py
--rw-r--r--   0 github     (503) staff       (20)      113 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/pytorch_lightning.py
--rw-r--r--   0 github     (503) staff       (20)       87 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/aim/sb3.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.717622 aim-4.0.0.dev2/aim/sdk/
--rw-r--r--   0 github     (503) staff       (20)      915 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/sdk/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.721398 aim-4.0.0.dev2/aim/sdk/adapters/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/adapters/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2609 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/adapters/acme.py
--rw-r--r--   0 github     (503) staff       (20)     3371 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/adapters/catboost.py
--rw-r--r--   0 github     (503) staff       (20)     5510 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/adapters/fastai.py
--rw-r--r--   0 github     (503) staff       (20)     5664 2023-03-24 14:18:45.000000 aim-4.0.0.dev2/aim/sdk/adapters/hugging_face.py
--rw-r--r--   0 github     (503) staff       (20)     2579 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/adapters/keras.py
--rw-r--r--   0 github     (503) staff       (20)     1128 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/adapters/keras_mixins.py
--rw-r--r--   0 github     (503) staff       (20)     2805 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/adapters/keras_tuner.py
--rw-r--r--   0 github     (503) staff       (20)     3266 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/adapters/lightgbm.py
--rw-r--r--   0 github     (503) staff       (20)     8261 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/adapters/mxnet.py
--rw-r--r--   0 github     (503) staff       (20)     7159 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/adapters/optuna.py
--rw-r--r--   0 github     (503) staff       (20)     3495 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/adapters/paddle.py
--rw-r--r--   0 github     (503) staff       (20)     2911 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/adapters/prophet.py
--rw-r--r--   0 github     (503) staff       (20)     2458 2022-07-09 00:13:12.000000 aim-4.0.0.dev2/aim/sdk/adapters/pytorch.py
--rw-r--r--   0 github     (503) staff       (20)     9025 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/adapters/pytorch_ignite.py
--rw-r--r--   0 github     (503) staff       (20)     5837 2023-03-24 14:18:45.000000 aim-4.0.0.dev2/aim/sdk/adapters/pytorch_lightning.py
--rw-r--r--   0 github     (503) staff       (20)     4533 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/adapters/sb3.py
--rw-r--r--   0 github     (503) staff       (20)     2600 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/adapters/tensorflow.py
--rw-r--r--   0 github     (503) staff       (20)     2934 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/adapters/xgboost.py
--rw-r--r--   0 github     (503) staff       (20)     5138 2023-03-16 00:07:12.000000 aim-4.0.0.dev2/aim/sdk/base_run.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.722208 aim-4.0.0.dev2/aim/sdk/callbacks/
--rw-r--r--   0 github     (503) staff       (20)      196 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/sdk/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1493 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/sdk/callbacks/caller.py
--rw-r--r--   0 github     (503) staff       (20)      495 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/sdk/callbacks/events.py
--rw-r--r--   0 github     (503) staff       (20)     1416 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/sdk/callbacks/helpers.py
--rw-r--r--   0 github     (503) staff       (20)      253 2022-09-26 00:13:35.000000 aim-4.0.0.dev2/aim/sdk/configs.py
--rw-r--r--   0 github     (503) staff       (20)       22 2022-11-24 20:09:30.000000 aim-4.0.0.dev2/aim/sdk/data_version.py
--rw-r--r--   0 github     (503) staff       (20)      145 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/sdk/errors.py
--rw-r--r--   0 github     (503) staff       (20)     4990 2023-01-23 20:08:00.000000 aim-4.0.0.dev2/aim/sdk/index_manager.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.723248 aim-4.0.0.dev2/aim/sdk/legacy/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/legacy/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      288 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/legacy/deprecation_warning.py
--rw-r--r--   0 github     (503) staff       (20)       94 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/legacy/flush.py
--rw-r--r--   0 github     (503) staff       (20)      185 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/legacy/init.py
--rw-r--r--   0 github     (503) staff       (20)      702 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/legacy/select.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.723718 aim-4.0.0.dev2/aim/sdk/legacy/session/
--rw-r--r--   0 github     (503) staff       (20)       67 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/legacy/session/__init__.py
--rw-r--r--   0 github     (503) staff       (20)       30 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/legacy/session/configs.py
--rw-r--r--   0 github     (503) staff       (20)     4277 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/legacy/session/session.py
--rw-r--r--   0 github     (503) staff       (20)      410 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/legacy/track.py
--rw-r--r--   0 github     (503) staff       (20)     6513 2023-02-01 20:08:30.000000 aim-4.0.0.dev2/aim/sdk/lock_manager.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.724038 aim-4.0.0.dev2/aim/sdk/logging/
--rw-r--r--   0 github     (503) staff       (20)       61 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/sdk/logging/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1863 2023-02-03 15:21:38.000000 aim-4.0.0.dev2/aim/sdk/logging/log_record.py
--rw-r--r--   0 github     (503) staff       (20)      954 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/sdk/maintenance_run.py
--rw-r--r--   0 github     (503) staff       (20)     3397 2023-03-16 00:07:12.000000 aim-4.0.0.dev2/aim/sdk/num_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.725205 aim-4.0.0.dev2/aim/sdk/objects/
--rw-r--r--   0 github     (503) staff       (20)      214 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/objects/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3264 2022-11-11 08:24:45.000000 aim-4.0.0.dev2/aim/sdk/objects/audio.py
--rw-r--r--   0 github     (503) staff       (20)     4232 2023-01-04 20:08:59.000000 aim-4.0.0.dev2/aim/sdk/objects/distribution.py
--rw-r--r--   0 github     (503) staff       (20)     2885 2023-01-04 20:08:59.000000 aim-4.0.0.dev2/aim/sdk/objects/figure.py
--rw-r--r--   0 github     (503) staff       (20)     9914 2023-03-03 20:09:01.000000 aim-4.0.0.dev2/aim/sdk/objects/image.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.725559 aim-4.0.0.dev2/aim/sdk/objects/io/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/objects/io/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    21094 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/objects/io/wavfile.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.726710 aim-4.0.0.dev2/aim/sdk/objects/plugins/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/objects/plugins/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1983 2023-01-23 20:08:00.000000 aim-4.0.0.dev2/aim/sdk/objects/plugins/dvc_metadata.py
--rw-r--r--   0 github     (503) staff       (20)     3648 2023-02-02 20:09:54.000000 aim-4.0.0.dev2/aim/sdk/objects/plugins/hf_datasets_metadata.py
--rw-r--r--   0 github     (503) staff       (20)     1272 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/objects/plugins/hub_dataset.py
--rw-r--r--   0 github     (503) staff       (20)      694 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/objects/text.py
--rw-r--r--   0 github     (503) staff       (20)     6048 2022-09-01 19:23:53.000000 aim-4.0.0.dev2/aim/sdk/query_utils.py
--rw-r--r--   0 github     (503) staff       (20)     1050 2023-01-23 10:30:27.000000 aim-4.0.0.dev2/aim/sdk/remote_repo_proxy.py
--rw-r--r--   0 github     (503) staff       (20)     2171 2023-01-23 10:30:27.000000 aim-4.0.0.dev2/aim/sdk/remote_run_reporter.py
--rw-r--r--   0 github     (503) staff       (20)    34519 2023-03-03 20:09:01.000000 aim-4.0.0.dev2/aim/sdk/repo.py
--rw-r--r--   0 github     (503) staff       (20)     1022 2023-03-16 00:07:12.000000 aim-4.0.0.dev2/aim/sdk/repo_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.727347 aim-4.0.0.dev2/aim/sdk/reporter/
--rw-r--r--   0 github     (503) staff       (20)    31012 2023-01-23 20:08:00.000000 aim-4.0.0.dev2/aim/sdk/reporter/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1832 2023-01-23 10:30:27.000000 aim-4.0.0.dev2/aim/sdk/reporter/file_manager.py
--rw-r--r--   0 github     (503) staff       (20)    30774 2023-03-16 00:07:12.000000 aim-4.0.0.dev2/aim/sdk/run.py
--rw-r--r--   0 github     (503) staff       (20)    13171 2023-02-03 15:21:38.000000 aim-4.0.0.dev2/aim/sdk/run_status_watcher.py
--rw-r--r--   0 github     (503) staff       (20)    12970 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/sequence.py
--rw-r--r--   0 github     (503) staff       (20)     9944 2022-07-21 10:42:47.000000 aim-4.0.0.dev2/aim/sdk/sequence_collection.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.729025 aim-4.0.0.dev2/aim/sdk/sequences/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/sequences/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      458 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/sequences/audio_sequence.py
--rw-r--r--   0 github     (503) staff       (20)      408 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/sequences/distribution_sequence.py
--rw-r--r--   0 github     (503) staff       (20)      452 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/sequences/figure_sequence.py
--rw-r--r--   0 github     (503) staff       (20)      482 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/sequences/image_sequence.py
--rw-r--r--   0 github     (503) staff       (20)     3936 2022-07-09 00:13:12.000000 aim-4.0.0.dev2/aim/sdk/sequences/metric.py
--rw-r--r--   0 github     (503) staff       (20)      458 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/sequences/text_sequence.py
--rw-r--r--   0 github     (503) staff       (20)    10545 2022-09-25 12:02:15.000000 aim-4.0.0.dev2/aim/sdk/tracker.py
--rw-r--r--   0 github     (503) staff       (20)     2202 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/sdk/training_flow.py
--rw-r--r--   0 github     (503) staff       (20)      159 2022-06-18 00:13:24.000000 aim-4.0.0.dev2/aim/sdk/types.py
--rw-r--r--   0 github     (503) staff       (20)     2940 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/sdk/uri_service.py
--rw-r--r--   0 github     (503) staff       (20)     4046 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/sdk/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.742572 aim-4.0.0.dev2/aim/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   439810 2023-04-05 11:37:56.000000 aim-4.0.0.dev2/aim/storage/arrayview.cpp
--rw-r--r--   0 github     (503) staff       (20)      278 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/arrayview.pxd
--rw-r--r--   0 github     (503) staff       (20)     2649 2022-06-15 14:05:59.000000 aim-4.0.0.dev2/aim/storage/arrayview.py
--rw-r--r--   0 github     (503) staff       (20)   844368 2023-04-05 11:37:57.000000 aim-4.0.0.dev2/aim/storage/container.cpp
--rw-r--r--   0 github     (503) staff       (20)      951 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/container.pxd
--rw-r--r--   0 github     (503) staff       (20)    10477 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/container.py
--rw-r--r--   0 github     (503) staff       (20)   912217 2023-04-05 11:37:58.000000 aim-4.0.0.dev2/aim/storage/containertreeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      313 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/containertreeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     6026 2023-01-24 20:09:40.000000 aim-4.0.0.dev2/aim/storage/containertreeview.py
--rw-r--r--   0 github     (503) staff       (20)     1212 2022-06-15 14:05:59.000000 aim-4.0.0.dev2/aim/storage/context.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.744415 aim-4.0.0.dev2/aim/storage/encoding/
--rw-r--r--   0 github     (503) staff       (20)   148655 2023-04-05 11:37:58.000000 aim-4.0.0.dev2/aim/storage/encoding/__init__.cpp
--rw-r--r--   0 github     (503) staff       (20)      155 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/encoding/__init__.pxd
--rw-r--r--   0 github     (503) staff       (20)       95 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/encoding/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   378105 2023-04-05 11:37:58.000000 aim-4.0.0.dev2/aim/storage/encoding/encoding.cpp
--rw-r--r--   0 github     (503) staff       (20)      507 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/encoding/encoding.pxd
--rw-r--r--   0 github     (503) staff       (20)     7373 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/encoding/encoding.pyx
--rw-r--r--   0 github     (503) staff       (20)   353597 2023-04-05 11:37:58.000000 aim-4.0.0.dev2/aim/storage/encoding/encoding_native.cpp
--rw-r--r--   0 github     (503) staff       (20)      930 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/encoding/encoding_native.pxd
--rw-r--r--   0 github     (503) staff       (20)     5974 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/encoding/encoding_native.pyx
--rw-r--r--   0 github     (503) staff       (20)      337 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/env.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.746354 aim-4.0.0.dev2/aim/storage/hashing/
--rw-r--r--   0 github     (503) staff       (20)   141729 2023-04-05 11:37:58.000000 aim-4.0.0.dev2/aim/storage/hashing/__init__.cpp
--rw-r--r--   0 github     (503) staff       (20)       85 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/hashing/__init__.pxd
--rw-r--r--   0 github     (503) staff       (20)       50 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/hashing/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   205598 2023-04-05 11:37:58.000000 aim-4.0.0.dev2/aim/storage/hashing/c_hash.cpp
--rw-r--r--   0 github     (503) staff       (20)      151 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/hashing/c_hash.pxd
--rw-r--r--   0 github     (503) staff       (20)     1077 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/hashing/c_hash.pyx
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.746512 aim-4.0.0.dev2/aim/storage/hashing/hash/
--rw-r--r--   0 github     (503) staff       (20)     1412 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/hashing/hash/hash.h
--rw-r--r--   0 github     (503) staff       (20)   392224 2023-04-05 11:37:58.000000 aim-4.0.0.dev2/aim/storage/hashing/hashing.cpp
--rw-r--r--   0 github     (503) staff       (20)     1009 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/hashing/hashing.pxd
--rw-r--r--   0 github     (503) staff       (20)     5562 2023-01-24 20:09:40.000000 aim-4.0.0.dev2/aim/storage/hashing/hashing.py
--rw-r--r--   0 github     (503) staff       (20)   672756 2023-04-05 11:37:58.000000 aim-4.0.0.dev2/aim/storage/inmemorytreeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      196 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/inmemorytreeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     4341 2023-01-24 20:09:40.000000 aim-4.0.0.dev2/aim/storage/inmemorytreeview.py
--rw-r--r--   0 github     (503) staff       (20)     1322 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/storage/lock_proxy.py
--rw-r--r--   0 github     (503) staff       (20)     6344 2023-03-31 20:11:31.000000 aim-4.0.0.dev2/aim/storage/locking.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.748007 aim-4.0.0.dev2/aim/storage/migrations/
--rw-r--r--   0 github     (503) staff       (20)       38 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/migrations/README
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/migrations/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2218 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/migrations/alembic.ini
--rw-r--r--   0 github     (503) staff       (20)     2215 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/migrations/alembic_dev.ini
--rw-r--r--   0 github     (503) staff       (20)     2339 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/migrations/env.py
--rw-r--r--   0 github     (503) staff       (20)      494 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/migrations/script.py.mako
--rw-r--r--   0 github     (503) staff       (20)      965 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/migrations/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.749109 aim-4.0.0.dev2/aim/storage/migrations/versions/
--rw-r--r--   0 github     (503) staff       (20)     2841 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/migrations/versions/1ecf8222220d_initial_schema.py
--rw-r--r--   0 github     (503) staff       (20)      658 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/migrations/versions/3c4f22db7a46_run_end_time.py
--rw-r--r--   0 github     (503) staff       (20)     1475 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/storage/migrations/versions/46b89d830ad8_.py
--rw-r--r--   0 github     (503) staff       (20)      653 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/migrations/versions/9ba30ab3b2b4_.py
--rw-r--r--   0 github     (503) staff       (20)     1516 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/migrations/versions/b07e7b07c8ce_.py
--rw-r--r--   0 github     (503) staff       (20)      789 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/migrations/versions/fbfe5c4702fb_soft_delete.py
--rw-r--r--   0 github     (503) staff       (20)     1650 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/object.py
--rw-r--r--   0 github     (503) staff       (20)   959785 2023-04-05 11:37:58.000000 aim-4.0.0.dev2/aim/storage/prefixview.cpp
--rw-r--r--   0 github     (503) staff       (20)      770 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/prefixview.pxd
--rw-r--r--   0 github     (503) staff       (20)    11248 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/prefixview.py
--rw-r--r--   0 github     (503) staff       (20)    11648 2022-06-15 14:05:59.000000 aim-4.0.0.dev2/aim/storage/proxy.py
--rw-r--r--   0 github     (503) staff       (20)     4816 2022-07-21 10:42:47.000000 aim-4.0.0.dev2/aim/storage/query.py
--rw-r--r--   0 github     (503) staff       (20)  1056280 2023-04-05 11:37:59.000000 aim-4.0.0.dev2/aim/storage/rockscontainer.cpp
--rw-r--r--   0 github     (503) staff       (20)    18514 2023-01-23 20:08:00.000000 aim-4.0.0.dev2/aim/storage/rockscontainer.pyx
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.749864 aim-4.0.0.dev2/aim/storage/structured/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/structured/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3183 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/structured/db.py
--rw-r--r--   0 github     (503) staff       (20)     5355 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/storage/structured/entities.py
--rw-r--r--   0 github     (503) staff       (20)     2959 2022-11-12 00:14:35.000000 aim-4.0.0.dev2/aim/storage/structured/proxy.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.750980 aim-4.0.0.dev2/aim/storage/structured/sql_engine/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/structured/sql_engine/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    19882 2023-01-25 20:08:55.000000 aim-4.0.0.dev2/aim/storage/structured/sql_engine/entities.py
--rw-r--r--   0 github     (503) staff       (20)     3484 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/structured/sql_engine/factory.py
--rw-r--r--   0 github     (503) staff       (20)     4888 2022-11-25 20:09:54.000000 aim-4.0.0.dev2/aim/storage/structured/sql_engine/models.py
--rw-r--r--   0 github     (503) staff       (20)     4811 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/structured/sql_engine/utils.py
--rw-r--r--   0 github     (503) staff       (20)   697830 2023-04-05 11:37:59.000000 aim-4.0.0.dev2/aim/storage/treearrayview.cpp
--rw-r--r--   0 github     (503) staff       (20)      251 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/treearrayview.pxd
--rw-r--r--   0 github     (503) staff       (20)     3033 2022-08-02 09:43:44.000000 aim-4.0.0.dev2/aim/storage/treearrayview.py
--rw-r--r--   0 github     (503) staff       (20)   722166 2023-04-05 11:37:59.000000 aim-4.0.0.dev2/aim/storage/treeutils.cpp
--rw-r--r--   0 github     (503) staff       (20)     8365 2022-06-15 14:05:59.000000 aim-4.0.0.dev2/aim/storage/treeutils.pyx
--rw-r--r--   0 github     (503) staff       (20)      707 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/treeutils_non_native.py
--rw-r--r--   0 github     (503) staff       (20)   515752 2023-04-05 11:37:59.000000 aim-4.0.0.dev2/aim/storage/treeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      311 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/treeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     2765 2023-01-24 20:09:40.000000 aim-4.0.0.dev2/aim/storage/treeview.py
--rw-r--r--   0 github     (503) staff       (20)     8241 2023-02-27 08:16:06.000000 aim-4.0.0.dev2/aim/storage/treeviewproxy.py
--rw-r--r--   0 github     (503) staff       (20)     1357 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/types.py
--rw-r--r--   0 github     (503) staff       (20)   812526 2023-04-05 11:37:59.000000 aim-4.0.0.dev2/aim/storage/union.cpp
--rw-r--r--   0 github     (503) staff       (20)     7919 2023-01-23 20:08:00.000000 aim-4.0.0.dev2/aim/storage/union.pyx
--rw-r--r--   0 github     (503) staff       (20)   810540 2023-04-05 11:38:00.000000 aim-4.0.0.dev2/aim/storage/utils.cpp
--rw-r--r--   0 github     (503) staff       (20)      469 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/utils.pxd
--rw-r--r--   0 github     (503) staff       (20)     2102 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/storage/utils.py
--rw-r--r--   0 github     (503) staff       (20)      119 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/tensorflow.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.751612 aim-4.0.0.dev2/aim/utils/
--rw-r--r--   0 github     (503) staff       (20)       84 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/aim/utils/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1209 2023-02-01 20:08:30.000000 aim-4.0.0.dev2/aim/utils/deprecation.py
--rw-r--r--   0 github     (503) staff       (20)     4728 2023-02-27 08:16:06.000000 aim-4.0.0.dev2/aim/utils/tracking.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.752481 aim-4.0.0.dev2/aim/web/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.753439 aim-4.0.0.dev2/aim/web/api/
--rw-r--r--   0 github     (503) staff       (20)     3504 2023-01-23 10:30:27.000000 aim-4.0.0.dev2/aim/web/api/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.754340 aim-4.0.0.dev2/aim/web/api/dashboard_apps/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/dashboard_apps/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      939 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/dashboard_apps/models.py
--rw-r--r--   0 github     (503) staff       (20)      542 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/dashboard_apps/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)      445 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/dashboard_apps/serializers.py
--rw-r--r--   0 github     (503) staff       (20)     2974 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/dashboard_apps/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.755231 aim-4.0.0.dev2/aim/web/api/dashboards/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/dashboards/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      667 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/dashboards/models.py
--rw-r--r--   0 github     (503) staff       (20)      652 2022-10-06 00:17:33.000000 aim-4.0.0.dev2/aim/web/api/dashboards/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)      775 2022-10-06 00:17:33.000000 aim-4.0.0.dev2/aim/web/api/dashboards/serializers.py
--rw-r--r--   0 github     (503) staff       (20)     3341 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/dashboards/views.py
--rw-r--r--   0 github     (503) staff       (20)      820 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/db.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.755763 aim-4.0.0.dev2/aim/web/api/experiments/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/experiments/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      974 2022-11-24 20:09:30.000000 aim-4.0.0.dev2/aim/web/api/experiments/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)     8931 2023-01-19 20:08:35.000000 aim-4.0.0.dev2/aim/web/api/experiments/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.756571 aim-4.0.0.dev2/aim/web/api/projects/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/projects/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      735 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/projects/project.py
--rw-r--r--   0 github     (503) staff       (20)      943 2022-10-06 00:17:33.000000 aim-4.0.0.dev2/aim/web/api/projects/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)     5200 2023-01-24 20:09:40.000000 aim-4.0.0.dev2/aim/web/api/projects/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.758053 aim-4.0.0.dev2/aim/web/api/runs/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/runs/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    12969 2022-07-21 10:42:47.000000 aim-4.0.0.dev2/aim/web/api/runs/object_api_utils.py
--rw-r--r--   0 github     (503) staff       (20)     6683 2022-07-21 10:42:47.000000 aim-4.0.0.dev2/aim/web/api/runs/object_views.py
--rw-r--r--   0 github     (503) staff       (20)     4420 2022-12-23 10:19:51.000000 aim-4.0.0.dev2/aim/web/api/runs/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)    15418 2023-02-03 15:21:38.000000 aim-4.0.0.dev2/aim/web/api/runs/utils.py
--rw-r--r--   0 github     (503) staff       (20)    12137 2023-02-03 15:21:38.000000 aim-4.0.0.dev2/aim/web/api/runs/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.758543 aim-4.0.0.dev2/aim/web/api/tags/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/tags/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      871 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/tags/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)     4272 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/tags/views.py
--rw-r--r--   0 github     (503) staff       (20)     1169 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/api/utils.py
--rw-r--r--   0 github     (503) staff       (20)     1589 2022-05-16 21:25:24.000000 aim-4.0.0.dev2/aim/web/api/views.py
--rw-r--r--   0 github     (503) staff       (20)      508 2022-08-11 13:58:02.000000 aim-4.0.0.dev2/aim/web/configs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.758705 aim-4.0.0.dev2/aim/web/middlewares/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/middlewares/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.759049 aim-4.0.0.dev2/aim/web/middlewares/profiler/
--rw-r--r--   0 github     (503) staff       (20)       81 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/middlewares/profiler/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3654 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/middlewares/profiler/profiler.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.759900 aim-4.0.0.dev2/aim/web/migrations/
--rw-r--r--   0 github     (503) staff       (20)       38 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/migrations/README
--rw-r--r--   0 github     (503) staff       (20)      810 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/migrations/alembic.ini
--rw-r--r--   0 github     (503) staff       (20)      807 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/migrations/alembic_dev.ini
--rw-r--r--   0 github     (503) staff       (20)     2792 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/migrations/env.py
--rw-r--r--   0 github     (503) staff       (20)      494 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/migrations/script.py.mako
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.760584 aim-4.0.0.dev2/aim/web/migrations/versions/
--rw-r--r--   0 github     (503) staff       (20)     2183 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/migrations/versions/11672b13f92c_.py
--rw-r--r--   0 github     (503) staff       (20)     1545 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/migrations/versions/517a45b2e62c_.py
--rw-r--r--   0 github     (503) staff       (20)     5592 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/migrations/versions/5ae8371b7481_.py
--rw-r--r--   0 github     (503) staff       (20)     7262 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/migrations/versions/73a3d004c227_.py
--rw-r--r--   0 github     (503) staff       (20)       55 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/run.py
--rw-r--r--   0 github     (503) staff       (20)     3055 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/web/utils.py
--rw-r--r--   0 github     (503) staff       (20)       96 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/aim/xgboost.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.687344 aim-4.0.0.dev2/aim.egg-info/
--rw-r--r--   0 github     (503) staff       (20)    37083 2023-04-05 11:38:00.000000 aim-4.0.0.dev2/aim.egg-info/PKG-INFO
--rw-r--r--   0 github     (503) staff       (20)    11901 2023-04-05 11:38:00.000000 aim-4.0.0.dev2/aim.egg-info/SOURCES.txt
--rw-r--r--   0 github     (503) staff       (20)        1 2023-04-05 11:38:00.000000 aim-4.0.0.dev2/aim.egg-info/dependency_links.txt
--rw-r--r--   0 github     (503) staff       (20)      102 2023-04-05 11:38:00.000000 aim-4.0.0.dev2/aim.egg-info/entry_points.txt
--rw-r--r--   0 github     (503) staff       (20)      422 2023-04-05 11:38:00.000000 aim-4.0.0.dev2/aim.egg-info/requires.txt
--rw-r--r--   0 github     (503) staff       (20)       28 2023-04-05 11:38:00.000000 aim-4.0.0.dev2/aim.egg-info/top_level.txt
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.678887 aim-4.0.0.dev2/performance_tests/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.761949 aim-4.0.0.dev2/performance_tests/sdk/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/performance_tests/sdk/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      469 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/performance_tests/sdk/queries.py
--rw-r--r--   0 github     (503) staff       (20)     1199 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/performance_tests/sdk/test_data_collection.py
--rw-r--r--   0 github     (503) staff       (20)     1134 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/performance_tests/sdk/test_query.py
--rw-r--r--   0 github     (503) staff       (20)     1881 2022-06-18 00:13:24.000000 aim-4.0.0.dev2/performance_tests/sdk/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.762822 aim-4.0.0.dev2/performance_tests/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/performance_tests/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      678 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/performance_tests/storage/test_container_open.py
--rw-r--r--   0 github     (503) staff       (20)      690 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/performance_tests/storage/test_iterative_access.py
--rw-r--r--   0 github     (503) staff       (20)      802 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/performance_tests/storage/test_random_access.py
--rw-r--r--   0 github     (503) staff       (20)     1262 2022-06-18 00:13:24.000000 aim-4.0.0.dev2/performance_tests/storage/utils.py
--rw-r--r--   0 github     (503) staff       (20)       84 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/pyproject.toml
--rw-r--r--   0 github     (503) staff       (20)      336 2023-04-05 11:38:00.769132 aim-4.0.0.dev2/setup.cfg
--rw-r--r--   0 github     (503) staff       (20)     6716 2023-03-02 20:49:40.000000 aim-4.0.0.dev2/setup.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.679152 aim-4.0.0.dev2/tests/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.764587 aim-4.0.0.dev2/tests/api/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/tests/api/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5155 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/tests/api/test_dashboards_api.py
--rw-r--r--   0 github     (503) staff       (20)     4335 2022-09-25 12:02:15.000000 aim-4.0.0.dev2/tests/api/test_project_api.py
--rw-r--r--   0 github     (503) staff       (20)    10653 2023-01-23 10:30:27.000000 aim-4.0.0.dev2/tests/api/test_run_api.py
--rw-r--r--   0 github     (503) staff       (20)    21533 2023-01-23 10:30:27.000000 aim-4.0.0.dev2/tests/api/test_run_images_api.py
--rw-r--r--   0 github     (503) staff       (20)    12787 2023-01-23 10:30:27.000000 aim-4.0.0.dev2/tests/api/test_structured_data_api.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.765352 aim-4.0.0.dev2/tests/integrations/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/tests/integrations/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1167 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/tests/integrations/test_dvc_metadata.py
--rw-r--r--   0 github     (503) staff       (20)     1093 2023-01-13 20:10:23.000000 aim-4.0.0.dev2/tests/integrations/test_hf_datasets.py
--rw-r--r--   0 github     (503) staff       (20)      961 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/tests/integrations/test_hub_dataset.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.767668 aim-4.0.0.dev2/tests/sdk/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/tests/sdk/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2312 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/tests/sdk/test_image_construction.py
--rw-r--r--   0 github     (503) staff       (20)     2665 2022-09-25 12:02:15.000000 aim-4.0.0.dev2/tests/sdk/test_resource_tracker.py
--rw-r--r--   0 github     (503) staff       (20)     1022 2022-11-01 00:13:35.000000 aim-4.0.0.dev2/tests/sdk/test_run_apis.py
--rw-r--r--   0 github     (503) staff       (20)     1147 2022-09-01 19:23:53.000000 aim-4.0.0.dev2/tests/sdk/test_run_creation_checks.py
--rw-r--r--   0 github     (503) staff       (20)     1661 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/tests/sdk/test_run_finalization_time.py
--rw-r--r--   0 github     (503) staff       (20)     1214 2022-11-01 00:13:35.000000 aim-4.0.0.dev2/tests/sdk/test_run_metric_types.py
--rw-r--r--   0 github     (503) staff       (20)     4631 2022-09-25 12:02:15.000000 aim-4.0.0.dev2/tests/sdk/test_run_track_type_checking.py
--rw-r--r--   0 github     (503) staff       (20)    10444 2022-09-25 12:02:15.000000 aim-4.0.0.dev2/tests/sdk/test_run_write_container_data.py
--rw-r--r--   0 github     (503) staff       (20)     4517 2022-06-01 01:05:15.000000 aim-4.0.0.dev2/tests/sdk/test_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-05 11:38:00.768516 aim-4.0.0.dev2/tests/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev2/tests/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5677 2022-09-25 12:02:15.000000 aim-4.0.0.dev2/tests/storage/test_query.py
--rw-r--r--   0 github     (503) staff       (20)     1482 2022-06-18 00:13:24.000000 aim-4.0.0.dev2/tests/storage/test_query_with_epoch_none.py
--rw-r--r--   0 github     (503) staff       (20)     1342 2022-09-25 12:02:15.000000 aim-4.0.0.dev2/tests/storage/test_structured_db.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:51.002742 aim-4.0.0.dev3/
+-rw-r--r--   0 github     (503) staff       (20)    11347 2022-08-06 00:13:01.000000 aim-4.0.0.dev3/LICENSE
+-rw-r--r--   0 github     (503) staff       (20)      185 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/MANIFEST.in
+-rw-r--r--   0 github     (503) staff       (20)    37846 2023-04-10 17:48:51.002914 aim-4.0.0.dev3/PKG-INFO
+-rw-r--r--   0 github     (503) staff       (20)    37159 2023-04-06 20:09:56.000000 aim-4.0.0.dev3/README.md
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.920046 aim-4.0.0.dev3/aim/
+-rw-r--r--   0 github     (503) staff       (20)       10 2023-04-10 17:48:41.000000 aim-4.0.0.dev3/aim/VERSION
+-rw-r--r--   0 github     (503) staff       (20)      825 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/__about__.py
+-rw-r--r--   0 github     (503) staff       (20)      377 2023-02-01 20:08:30.000000 aim-4.0.0.dev3/aim/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      183 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/__version__.py
+-rw-r--r--   0 github     (503) staff       (20)      100 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/acme.py
+-rw-r--r--   0 github     (503) staff       (20)       96 2022-05-06 13:59:46.000000 aim-4.0.0.dev3/aim/catboost.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.921952 aim-4.0.0.dev3/aim/cli/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1323 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/cli/cli.py
+-rw-r--r--   0 github     (503) staff       (20)      166 2022-06-17 00:13:19.000000 aim-4.0.0.dev3/aim/cli/configs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.922333 aim-4.0.0.dev3/aim/cli/convert/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/convert/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2998 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/cli/convert/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.923311 aim-4.0.0.dev3/aim/cli/convert/processors/
+-rw-r--r--   0 github     (503) staff       (20)      113 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/cli/convert/processors/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5914 2022-09-01 19:23:53.000000 aim-4.0.0.dev3/aim/cli/convert/processors/mlflow.py
+-rw-r--r--   0 github     (503) staff       (20)    10372 2022-08-06 00:13:01.000000 aim-4.0.0.dev3/aim/cli/convert/processors/tensorboard.py
+-rw-r--r--   0 github     (503) staff       (20)     6816 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/cli/convert/processors/wandb.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.923653 aim-4.0.0.dev3/aim/cli/init/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/init/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1592 2023-03-24 14:18:45.000000 aim-4.0.0.dev3/aim/cli/init/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.923999 aim-4.0.0.dev3/aim/cli/manager/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/manager/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3382 2022-08-11 13:58:02.000000 aim-4.0.0.dev3/aim/cli/manager/manager.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.924341 aim-4.0.0.dev3/aim/cli/reindex/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/reindex/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      736 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/cli/reindex/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.924958 aim-4.0.0.dev3/aim/cli/runs/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/runs/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     6621 2023-03-24 14:18:45.000000 aim-4.0.0.dev3/aim/cli/runs/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     2570 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/cli/runs/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.925329 aim-4.0.0.dev3/aim/cli/server/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/server/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3709 2023-03-24 14:18:45.000000 aim-4.0.0.dev3/aim/cli/server/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.925658 aim-4.0.0.dev3/aim/cli/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-06-17 00:13:19.000000 aim-4.0.0.dev3/aim/cli/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     7537 2023-03-24 14:18:45.000000 aim-4.0.0.dev3/aim/cli/storage/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.926011 aim-4.0.0.dev3/aim/cli/telemetry/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/cli/telemetry/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      305 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/cli/telemetry/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.926634 aim-4.0.0.dev3/aim/cli/up/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/up/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5953 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/cli/up/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     1446 2022-06-21 18:01:08.000000 aim-4.0.0.dev3/aim/cli/up/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.927090 aim-4.0.0.dev3/aim/cli/upgrade/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.927833 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/
+-rw-r--r--   0 github     (503) staff       (20)      258 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      734 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/configs.py
+-rw-r--r--   0 github     (503) staff       (20)      448 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/metric_artifact.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.928496 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      263 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/base_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)      267 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/metric_pb2.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.928979 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v3/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v3/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3396 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v3/base_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     1919 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v3/metric_pb2.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.929408 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v4/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v4/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1111 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v4/base_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)      969 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v4/metric_pb2.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.930388 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/
+-rw-r--r--   0 github     (503) staff       (20)        1 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1722 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/metric.py
+-rw-r--r--   0 github     (503) staff       (20)     3722 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/repo.py
+-rw-r--r--   0 github     (503) staff       (20)     4062 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/run.py
+-rw-r--r--   0 github     (503) staff       (20)     1357 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/trace.py
+-rw-r--r--   0 github     (503) staff       (20)     1211 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/utils.py
+-rw-r--r--   0 github     (503) staff       (20)     6635 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      370 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.930628 aim-4.0.0.dev3/aim/cli/version/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/version/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      149 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/version/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     9960 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/cli/watcher_cli.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.931264 aim-4.0.0.dev3/aim/ext/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.931537 aim-4.0.0.dev3/aim/ext/cleanup/
+-rw-r--r--   0 github     (503) staff       (20)     3579 2022-11-12 00:14:35.000000 aim-4.0.0.dev3/aim/ext/cleanup/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2021 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/ext/exception_resistant.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.931952 aim-4.0.0.dev3/aim/ext/notebook/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/notebook/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     7314 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/notebook/notebook.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.934341 aim-4.0.0.dev3/aim/ext/notifier/
+-rw-r--r--   0 github     (503) staff       (20)      589 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      305 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/base_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1858 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/ext/notifier/config.py
+-rw-r--r--   0 github     (503) staff       (20)      361 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/config_default.json
+-rw-r--r--   0 github     (503) staff       (20)       70 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/config_empty.json
+-rw-r--r--   0 github     (503) staff       (20)      522 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/logging_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1428 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1158 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/notifier_builder.py
+-rw-r--r--   0 github     (503) staff       (20)      524 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/slack_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1034 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      862 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/workplace_notifier.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.935698 aim-4.0.0.dev3/aim/ext/resource/
+-rw-r--r--   0 github     (503) staff       (20)       92 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/resource/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      100 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/resource/configs.py
+-rw-r--r--   0 github     (503) staff       (20)      726 2022-05-16 21:25:24.000000 aim-4.0.0.dev3/aim/ext/resource/log.py
+-rw-r--r--   0 github     (503) staff       (20)     6700 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/ext/resource/stat.py
+-rw-r--r--   0 github     (503) staff       (20)     7511 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/ext/resource/tracker.py
+-rw-r--r--   0 github     (503) staff       (20)       56 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/resource/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.935961 aim-4.0.0.dev3/aim/ext/sshfs/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/sshfs/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     7768 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/sshfs/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.936228 aim-4.0.0.dev3/aim/ext/task_queue/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/task_queue/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2069 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/task_queue/queue.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.936951 aim-4.0.0.dev3/aim/ext/tensorboard_tracker/
+-rw-r--r--   0 github     (503) staff       (20)       48 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/ext/tensorboard_tracker/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      919 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/ext/tensorboard_tracker/run.py
+-rw-r--r--   0 github     (503) staff       (20)     7201 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/ext/tensorboard_tracker/tracker.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.940530 aim-4.0.0.dev3/aim/ext/transport/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/transport/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    13282 2023-04-06 20:09:56.000000 aim-4.0.0.dev3/aim/ext/transport/client.py
+-rw-r--r--   0 github     (503) staff       (20)      563 2023-04-06 20:09:56.000000 aim-4.0.0.dev3/aim/ext/transport/config.py
+-rw-r--r--   0 github     (503) staff       (20)     3298 2023-01-23 20:08:00.000000 aim-4.0.0.dev3/aim/ext/transport/handlers.py
+-rw-r--r--   0 github     (503) staff       (20)     5555 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/health.py
+-rw-r--r--   0 github     (503) staff       (20)     5616 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/heartbeat.py
+-rw-r--r--   0 github     (503) staff       (20)     3347 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/message_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.941787 aim-4.0.0.dev3/aim/ext/transport/proto/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      245 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/health_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     3991 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/health_pb2_grpc.py
+-rw-r--r--   0 github     (503) staff       (20)      259 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/remote_router_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     8855 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/remote_router_pb2_grpc.py
+-rw-r--r--   0 github     (503) staff       (20)      263 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/remote_tracking_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     9444 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/remote_tracking_pb2_grpc.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.942697 aim-4.0.0.dev3/aim/ext/transport/proto/v3/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v3/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     6195 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v3/health_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)    25245 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v3/remote_router_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)    37567 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v3/remote_tracking_pb2.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.943550 aim-4.0.0.dev3/aim/ext/transport/proto/v4/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v4/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1749 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v4/health_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     4280 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v4/remote_router_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     5662 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v4/remote_tracking_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)      428 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/transport/remote_resource.py
+-rw-r--r--   0 github     (503) staff       (20)     8078 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/aim/ext/transport/remote_tracking.py
+-rw-r--r--   0 github     (503) staff       (20)     3637 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/router.py
+-rw-r--r--   0 github     (503) staff       (20)     3728 2022-11-18 00:13:03.000000 aim-4.0.0.dev3/aim/ext/transport/rpc_queue.py
+-rw-r--r--   0 github     (503) staff       (20)     4609 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/aim/ext/transport/server.py
+-rw-r--r--   0 github     (503) staff       (20)     3419 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/worker.py
+-rw-r--r--   0 github     (503) staff       (20)     2103 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/utils.py
+-rw-r--r--   0 github     (503) staff       (20)       92 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/aim/fastai.py
+-rw-r--r--   0 github     (503) staff       (20)      127 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/hf_dataset.py
+-rw-r--r--   0 github     (503) staff       (20)      105 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/hugging_face.py
+-rw-r--r--   0 github     (503) staff       (20)      103 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/keras.py
+-rw-r--r--   0 github     (503) staff       (20)      103 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/keras_tuner.py
+-rw-r--r--   0 github     (503) staff       (20)       98 2022-05-06 13:59:46.000000 aim-4.0.0.dev3/aim/lightgbm.py
+-rw-r--r--   0 github     (503) staff       (20)       97 2022-10-04 00:16:28.000000 aim-4.0.0.dev3/aim/mxnet.py
+-rw-r--r--   0 github     (503) staff       (20)       98 2022-11-12 00:14:35.000000 aim-4.0.0.dev3/aim/optuna.py
+-rw-r--r--   0 github     (503) staff       (20)       99 2022-11-12 00:14:35.000000 aim-4.0.0.dev3/aim/paddle.py
+-rw-r--r--   0 github     (503) staff       (20)       93 2023-01-31 20:08:25.000000 aim-4.0.0.dev3/aim/prophet.py
+-rw-r--r--   0 github     (503) staff       (20)      115 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/pytorch.py
+-rw-r--r--   0 github     (503) staff       (20)      107 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/pytorch_ignite.py
+-rw-r--r--   0 github     (503) staff       (20)      113 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/pytorch_lightning.py
+-rw-r--r--   0 github     (503) staff       (20)       87 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/sb3.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.952455 aim-4.0.0.dev3/aim/sdk/
+-rw-r--r--   0 github     (503) staff       (20)      915 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.956451 aim-4.0.0.dev3/aim/sdk/adapters/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/adapters/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2609 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/acme.py
+-rw-r--r--   0 github     (503) staff       (20)     3371 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/catboost.py
+-rw-r--r--   0 github     (503) staff       (20)     5510 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/fastai.py
+-rw-r--r--   0 github     (503) staff       (20)     5664 2023-03-24 14:18:45.000000 aim-4.0.0.dev3/aim/sdk/adapters/hugging_face.py
+-rw-r--r--   0 github     (503) staff       (20)     2579 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/keras.py
+-rw-r--r--   0 github     (503) staff       (20)     1128 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/adapters/keras_mixins.py
+-rw-r--r--   0 github     (503) staff       (20)     2805 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/keras_tuner.py
+-rw-r--r--   0 github     (503) staff       (20)     3266 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/lightgbm.py
+-rw-r--r--   0 github     (503) staff       (20)     8261 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/mxnet.py
+-rw-r--r--   0 github     (503) staff       (20)     7159 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/optuna.py
+-rw-r--r--   0 github     (503) staff       (20)     3495 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/paddle.py
+-rw-r--r--   0 github     (503) staff       (20)     2911 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/prophet.py
+-rw-r--r--   0 github     (503) staff       (20)     2458 2022-07-09 00:13:12.000000 aim-4.0.0.dev3/aim/sdk/adapters/pytorch.py
+-rw-r--r--   0 github     (503) staff       (20)     9025 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/pytorch_ignite.py
+-rw-r--r--   0 github     (503) staff       (20)     5837 2023-03-24 14:18:45.000000 aim-4.0.0.dev3/aim/sdk/adapters/pytorch_lightning.py
+-rw-r--r--   0 github     (503) staff       (20)     4533 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/sb3.py
+-rw-r--r--   0 github     (503) staff       (20)     2600 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/tensorflow.py
+-rw-r--r--   0 github     (503) staff       (20)     2934 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/xgboost.py
+-rw-r--r--   0 github     (503) staff       (20)     5138 2023-03-16 00:07:12.000000 aim-4.0.0.dev3/aim/sdk/base_run.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.957257 aim-4.0.0.dev3/aim/sdk/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)      196 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1493 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/callbacks/caller.py
+-rw-r--r--   0 github     (503) staff       (20)      495 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/callbacks/events.py
+-rw-r--r--   0 github     (503) staff       (20)     1416 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/callbacks/helpers.py
+-rw-r--r--   0 github     (503) staff       (20)      253 2022-09-26 00:13:35.000000 aim-4.0.0.dev3/aim/sdk/configs.py
+-rw-r--r--   0 github     (503) staff       (20)       22 2022-11-24 20:09:30.000000 aim-4.0.0.dev3/aim/sdk/data_version.py
+-rw-r--r--   0 github     (503) staff       (20)      145 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/errors.py
+-rw-r--r--   0 github     (503) staff       (20)     4990 2023-01-23 20:08:00.000000 aim-4.0.0.dev3/aim/sdk/index_manager.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.958300 aim-4.0.0.dev3/aim/sdk/legacy/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      288 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/deprecation_warning.py
+-rw-r--r--   0 github     (503) staff       (20)       94 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/flush.py
+-rw-r--r--   0 github     (503) staff       (20)      185 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/init.py
+-rw-r--r--   0 github     (503) staff       (20)      702 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/select.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.958782 aim-4.0.0.dev3/aim/sdk/legacy/session/
+-rw-r--r--   0 github     (503) staff       (20)       67 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/session/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)       30 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/session/configs.py
+-rw-r--r--   0 github     (503) staff       (20)     4277 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/session/session.py
+-rw-r--r--   0 github     (503) staff       (20)      410 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/track.py
+-rw-r--r--   0 github     (503) staff       (20)     6513 2023-02-01 20:08:30.000000 aim-4.0.0.dev3/aim/sdk/lock_manager.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.959117 aim-4.0.0.dev3/aim/sdk/logging/
+-rw-r--r--   0 github     (503) staff       (20)       61 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/logging/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1863 2023-02-03 15:21:38.000000 aim-4.0.0.dev3/aim/sdk/logging/log_record.py
+-rw-r--r--   0 github     (503) staff       (20)      954 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/maintenance_run.py
+-rw-r--r--   0 github     (503) staff       (20)     3397 2023-03-16 00:07:12.000000 aim-4.0.0.dev3/aim/sdk/num_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.960264 aim-4.0.0.dev3/aim/sdk/objects/
+-rw-r--r--   0 github     (503) staff       (20)      214 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/objects/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3264 2022-11-11 08:24:45.000000 aim-4.0.0.dev3/aim/sdk/objects/audio.py
+-rw-r--r--   0 github     (503) staff       (20)     4232 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/sdk/objects/distribution.py
+-rw-r--r--   0 github     (503) staff       (20)     2885 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/sdk/objects/figure.py
+-rw-r--r--   0 github     (503) staff       (20)     9914 2023-03-03 20:09:01.000000 aim-4.0.0.dev3/aim/sdk/objects/image.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.960591 aim-4.0.0.dev3/aim/sdk/objects/io/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/objects/io/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    21094 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/objects/io/wavfile.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.961665 aim-4.0.0.dev3/aim/sdk/objects/plugins/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/objects/plugins/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1983 2023-01-23 20:08:00.000000 aim-4.0.0.dev3/aim/sdk/objects/plugins/dvc_metadata.py
+-rw-r--r--   0 github     (503) staff       (20)     3648 2023-02-02 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/objects/plugins/hf_datasets_metadata.py
+-rw-r--r--   0 github     (503) staff       (20)     1272 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/objects/plugins/hub_dataset.py
+-rw-r--r--   0 github     (503) staff       (20)      694 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/objects/text.py
+-rw-r--r--   0 github     (503) staff       (20)     6048 2022-09-01 19:23:53.000000 aim-4.0.0.dev3/aim/sdk/query_utils.py
+-rw-r--r--   0 github     (503) staff       (20)     1050 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/aim/sdk/remote_repo_proxy.py
+-rw-r--r--   0 github     (503) staff       (20)     2171 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/aim/sdk/remote_run_reporter.py
+-rw-r--r--   0 github     (503) staff       (20)    34519 2023-03-03 20:09:01.000000 aim-4.0.0.dev3/aim/sdk/repo.py
+-rw-r--r--   0 github     (503) staff       (20)     1022 2023-03-16 00:07:12.000000 aim-4.0.0.dev3/aim/sdk/repo_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.962310 aim-4.0.0.dev3/aim/sdk/reporter/
+-rw-r--r--   0 github     (503) staff       (20)    31012 2023-01-23 20:08:00.000000 aim-4.0.0.dev3/aim/sdk/reporter/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1832 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/aim/sdk/reporter/file_manager.py
+-rw-r--r--   0 github     (503) staff       (20)    30774 2023-03-16 00:07:12.000000 aim-4.0.0.dev3/aim/sdk/run.py
+-rw-r--r--   0 github     (503) staff       (20)    13171 2023-02-03 15:21:38.000000 aim-4.0.0.dev3/aim/sdk/run_status_watcher.py
+-rw-r--r--   0 github     (503) staff       (20)    12970 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/sequence.py
+-rw-r--r--   0 github     (503) staff       (20)     9944 2022-07-21 10:42:47.000000 aim-4.0.0.dev3/aim/sdk/sequence_collection.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.963838 aim-4.0.0.dev3/aim/sdk/sequences/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/sequences/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      458 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/sequences/audio_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      408 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/sequences/distribution_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      452 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/sequences/figure_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      482 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/sequences/image_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)     3936 2022-07-09 00:13:12.000000 aim-4.0.0.dev3/aim/sdk/sequences/metric.py
+-rw-r--r--   0 github     (503) staff       (20)      458 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/sequences/text_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)    10545 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/aim/sdk/tracker.py
+-rw-r--r--   0 github     (503) staff       (20)     2202 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/training_flow.py
+-rw-r--r--   0 github     (503) staff       (20)      159 2022-06-18 00:13:24.000000 aim-4.0.0.dev3/aim/sdk/types.py
+-rw-r--r--   0 github     (503) staff       (20)     2940 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/uri_service.py
+-rw-r--r--   0 github     (503) staff       (20)     4046 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.976271 aim-4.0.0.dev3/aim/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   439810 2023-04-10 17:48:47.000000 aim-4.0.0.dev3/aim/storage/arrayview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      278 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/arrayview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     2649 2022-06-15 14:05:59.000000 aim-4.0.0.dev3/aim/storage/arrayview.py
+-rw-r--r--   0 github     (503) staff       (20)   844368 2023-04-10 17:48:47.000000 aim-4.0.0.dev3/aim/storage/container.cpp
+-rw-r--r--   0 github     (503) staff       (20)      951 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/container.pxd
+-rw-r--r--   0 github     (503) staff       (20)    10477 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/container.py
+-rw-r--r--   0 github     (503) staff       (20)   912217 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/containertreeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      313 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/containertreeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     6026 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/storage/containertreeview.py
+-rw-r--r--   0 github     (503) staff       (20)     1212 2022-06-15 14:05:59.000000 aim-4.0.0.dev3/aim/storage/context.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.977728 aim-4.0.0.dev3/aim/storage/encoding/
+-rw-r--r--   0 github     (503) staff       (20)   148655 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/encoding/__init__.cpp
+-rw-r--r--   0 github     (503) staff       (20)      155 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/encoding/__init__.pxd
+-rw-r--r--   0 github     (503) staff       (20)       95 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/encoding/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   378105 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/encoding/encoding.cpp
+-rw-r--r--   0 github     (503) staff       (20)      507 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/encoding/encoding.pxd
+-rw-r--r--   0 github     (503) staff       (20)     7373 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/encoding/encoding.pyx
+-rw-r--r--   0 github     (503) staff       (20)   353597 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/encoding/encoding_native.cpp
+-rw-r--r--   0 github     (503) staff       (20)      930 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/encoding/encoding_native.pxd
+-rw-r--r--   0 github     (503) staff       (20)     5974 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/encoding/encoding_native.pyx
+-rw-r--r--   0 github     (503) staff       (20)      337 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/env.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.979081 aim-4.0.0.dev3/aim/storage/hashing/
+-rw-r--r--   0 github     (503) staff       (20)   141729 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/hashing/__init__.cpp
+-rw-r--r--   0 github     (503) staff       (20)       85 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/hashing/__init__.pxd
+-rw-r--r--   0 github     (503) staff       (20)       50 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/hashing/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   205598 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/hashing/c_hash.cpp
+-rw-r--r--   0 github     (503) staff       (20)      151 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/hashing/c_hash.pxd
+-rw-r--r--   0 github     (503) staff       (20)     1077 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/hashing/c_hash.pyx
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.979189 aim-4.0.0.dev3/aim/storage/hashing/hash/
+-rw-r--r--   0 github     (503) staff       (20)     1412 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/hashing/hash/hash.h
+-rw-r--r--   0 github     (503) staff       (20)   392224 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/hashing/hashing.cpp
+-rw-r--r--   0 github     (503) staff       (20)     1009 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/hashing/hashing.pxd
+-rw-r--r--   0 github     (503) staff       (20)     5562 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/storage/hashing/hashing.py
+-rw-r--r--   0 github     (503) staff       (20)   672756 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/inmemorytreeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      196 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/inmemorytreeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     4341 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/storage/inmemorytreeview.py
+-rw-r--r--   0 github     (503) staff       (20)     1322 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/storage/lock_proxy.py
+-rw-r--r--   0 github     (503) staff       (20)     6344 2023-04-06 20:09:56.000000 aim-4.0.0.dev3/aim/storage/locking.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.981488 aim-4.0.0.dev3/aim/storage/migrations/
+-rw-r--r--   0 github     (503) staff       (20)       38 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/README
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2218 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/alembic.ini
+-rw-r--r--   0 github     (503) staff       (20)     2215 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/alembic_dev.ini
+-rw-r--r--   0 github     (503) staff       (20)     2339 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/env.py
+-rw-r--r--   0 github     (503) staff       (20)      494 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/script.py.mako
+-rw-r--r--   0 github     (503) staff       (20)      965 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.982665 aim-4.0.0.dev3/aim/storage/migrations/versions/
+-rw-r--r--   0 github     (503) staff       (20)     2841 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/versions/1ecf8222220d_initial_schema.py
+-rw-r--r--   0 github     (503) staff       (20)      658 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/versions/3c4f22db7a46_run_end_time.py
+-rw-r--r--   0 github     (503) staff       (20)     1475 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/storage/migrations/versions/46b89d830ad8_.py
+-rw-r--r--   0 github     (503) staff       (20)      653 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/versions/9ba30ab3b2b4_.py
+-rw-r--r--   0 github     (503) staff       (20)     1516 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/versions/b07e7b07c8ce_.py
+-rw-r--r--   0 github     (503) staff       (20)      789 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/versions/fbfe5c4702fb_soft_delete.py
+-rw-r--r--   0 github     (503) staff       (20)     1650 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/object.py
+-rw-r--r--   0 github     (503) staff       (20)   959785 2023-04-10 17:48:49.000000 aim-4.0.0.dev3/aim/storage/prefixview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      770 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/prefixview.pxd
+-rw-r--r--   0 github     (503) staff       (20)    11248 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/prefixview.py
+-rw-r--r--   0 github     (503) staff       (20)    11648 2022-06-15 14:05:59.000000 aim-4.0.0.dev3/aim/storage/proxy.py
+-rw-r--r--   0 github     (503) staff       (20)     4816 2022-07-21 10:42:47.000000 aim-4.0.0.dev3/aim/storage/query.py
+-rw-r--r--   0 github     (503) staff       (20)  1056280 2023-04-10 17:48:49.000000 aim-4.0.0.dev3/aim/storage/rockscontainer.cpp
+-rw-r--r--   0 github     (503) staff       (20)    18514 2023-01-23 20:08:00.000000 aim-4.0.0.dev3/aim/storage/rockscontainer.pyx
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.983441 aim-4.0.0.dev3/aim/storage/structured/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/structured/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3183 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/structured/db.py
+-rw-r--r--   0 github     (503) staff       (20)     5355 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/storage/structured/entities.py
+-rw-r--r--   0 github     (503) staff       (20)     2959 2022-11-12 00:14:35.000000 aim-4.0.0.dev3/aim/storage/structured/proxy.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.984595 aim-4.0.0.dev3/aim/storage/structured/sql_engine/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/structured/sql_engine/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    19882 2023-01-25 20:08:55.000000 aim-4.0.0.dev3/aim/storage/structured/sql_engine/entities.py
+-rw-r--r--   0 github     (503) staff       (20)     3484 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/structured/sql_engine/factory.py
+-rw-r--r--   0 github     (503) staff       (20)     4888 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/storage/structured/sql_engine/models.py
+-rw-r--r--   0 github     (503) staff       (20)     4811 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/structured/sql_engine/utils.py
+-rw-r--r--   0 github     (503) staff       (20)   697830 2023-04-10 17:48:49.000000 aim-4.0.0.dev3/aim/storage/treearrayview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      251 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/treearrayview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     3033 2022-08-02 09:43:44.000000 aim-4.0.0.dev3/aim/storage/treearrayview.py
+-rw-r--r--   0 github     (503) staff       (20)   722166 2023-04-10 17:48:49.000000 aim-4.0.0.dev3/aim/storage/treeutils.cpp
+-rw-r--r--   0 github     (503) staff       (20)     8365 2022-06-15 14:05:59.000000 aim-4.0.0.dev3/aim/storage/treeutils.pyx
+-rw-r--r--   0 github     (503) staff       (20)      707 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/treeutils_non_native.py
+-rw-r--r--   0 github     (503) staff       (20)   515752 2023-04-10 17:48:49.000000 aim-4.0.0.dev3/aim/storage/treeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      311 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/treeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     2765 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/storage/treeview.py
+-rw-r--r--   0 github     (503) staff       (20)     8241 2023-02-27 08:16:06.000000 aim-4.0.0.dev3/aim/storage/treeviewproxy.py
+-rw-r--r--   0 github     (503) staff       (20)     1357 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/types.py
+-rw-r--r--   0 github     (503) staff       (20)   812526 2023-04-10 17:48:49.000000 aim-4.0.0.dev3/aim/storage/union.cpp
+-rw-r--r--   0 github     (503) staff       (20)     7919 2023-01-23 20:08:00.000000 aim-4.0.0.dev3/aim/storage/union.pyx
+-rw-r--r--   0 github     (503) staff       (20)   810540 2023-04-10 17:48:50.000000 aim-4.0.0.dev3/aim/storage/utils.cpp
+-rw-r--r--   0 github     (503) staff       (20)      469 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/utils.pxd
+-rw-r--r--   0 github     (503) staff       (20)     2102 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      119 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/tensorflow.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.985324 aim-4.0.0.dev3/aim/utils/
+-rw-r--r--   0 github     (503) staff       (20)       84 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/utils/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1209 2023-02-01 20:08:30.000000 aim-4.0.0.dev3/aim/utils/deprecation.py
+-rw-r--r--   0 github     (503) staff       (20)     4728 2023-02-27 08:16:06.000000 aim-4.0.0.dev3/aim/utils/tracking.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.986193 aim-4.0.0.dev3/aim/web/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.987139 aim-4.0.0.dev3/aim/web/api/
+-rw-r--r--   0 github     (503) staff       (20)     3504 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/aim/web/api/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.987988 aim-4.0.0.dev3/aim/web/api/dashboard_apps/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboard_apps/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      939 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboard_apps/models.py
+-rw-r--r--   0 github     (503) staff       (20)      542 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboard_apps/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)      445 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboard_apps/serializers.py
+-rw-r--r--   0 github     (503) staff       (20)     2974 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboard_apps/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.988889 aim-4.0.0.dev3/aim/web/api/dashboards/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboards/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      667 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboards/models.py
+-rw-r--r--   0 github     (503) staff       (20)      652 2022-10-06 00:17:33.000000 aim-4.0.0.dev3/aim/web/api/dashboards/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)      775 2022-10-06 00:17:33.000000 aim-4.0.0.dev3/aim/web/api/dashboards/serializers.py
+-rw-r--r--   0 github     (503) staff       (20)     3341 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboards/views.py
+-rw-r--r--   0 github     (503) staff       (20)      820 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/db.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.989400 aim-4.0.0.dev3/aim/web/api/experiments/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/experiments/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      974 2022-11-24 20:09:30.000000 aim-4.0.0.dev3/aim/web/api/experiments/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)     8931 2023-01-19 20:08:35.000000 aim-4.0.0.dev3/aim/web/api/experiments/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.990242 aim-4.0.0.dev3/aim/web/api/projects/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/projects/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      735 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/projects/project.py
+-rw-r--r--   0 github     (503) staff       (20)      943 2022-10-06 00:17:33.000000 aim-4.0.0.dev3/aim/web/api/projects/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)     5200 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/web/api/projects/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.991757 aim-4.0.0.dev3/aim/web/api/runs/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/runs/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    12969 2022-07-21 10:42:47.000000 aim-4.0.0.dev3/aim/web/api/runs/object_api_utils.py
+-rw-r--r--   0 github     (503) staff       (20)     6683 2022-07-21 10:42:47.000000 aim-4.0.0.dev3/aim/web/api/runs/object_views.py
+-rw-r--r--   0 github     (503) staff       (20)     4420 2022-12-23 10:19:51.000000 aim-4.0.0.dev3/aim/web/api/runs/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)    16029 2023-04-06 20:09:56.000000 aim-4.0.0.dev3/aim/web/api/runs/utils.py
+-rw-r--r--   0 github     (503) staff       (20)    12258 2023-04-06 20:09:56.000000 aim-4.0.0.dev3/aim/web/api/runs/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.992319 aim-4.0.0.dev3/aim/web/api/tags/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/tags/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      871 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/tags/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)     4272 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/tags/views.py
+-rw-r--r--   0 github     (503) staff       (20)     1169 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/utils.py
+-rw-r--r--   0 github     (503) staff       (20)     1589 2022-05-16 21:25:24.000000 aim-4.0.0.dev3/aim/web/api/views.py
+-rw-r--r--   0 github     (503) staff       (20)      508 2022-08-11 13:58:02.000000 aim-4.0.0.dev3/aim/web/configs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.992494 aim-4.0.0.dev3/aim/web/middlewares/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/middlewares/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.992857 aim-4.0.0.dev3/aim/web/middlewares/profiler/
+-rw-r--r--   0 github     (503) staff       (20)       81 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/middlewares/profiler/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3654 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/middlewares/profiler/profiler.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.993713 aim-4.0.0.dev3/aim/web/migrations/
+-rw-r--r--   0 github     (503) staff       (20)       38 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/README
+-rw-r--r--   0 github     (503) staff       (20)      810 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/alembic.ini
+-rw-r--r--   0 github     (503) staff       (20)      807 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/alembic_dev.ini
+-rw-r--r--   0 github     (503) staff       (20)     2792 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/env.py
+-rw-r--r--   0 github     (503) staff       (20)      494 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/script.py.mako
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.994443 aim-4.0.0.dev3/aim/web/migrations/versions/
+-rw-r--r--   0 github     (503) staff       (20)     2183 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/versions/11672b13f92c_.py
+-rw-r--r--   0 github     (503) staff       (20)     1545 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/versions/517a45b2e62c_.py
+-rw-r--r--   0 github     (503) staff       (20)     5592 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/versions/5ae8371b7481_.py
+-rw-r--r--   0 github     (503) staff       (20)     7262 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/versions/73a3d004c227_.py
+-rw-r--r--   0 github     (503) staff       (20)       55 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/run.py
+-rw-r--r--   0 github     (503) staff       (20)     3055 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/utils.py
+-rw-r--r--   0 github     (503) staff       (20)       96 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/xgboost.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.921023 aim-4.0.0.dev3/aim.egg-info/
+-rw-r--r--   0 github     (503) staff       (20)    37846 2023-04-10 17:48:50.000000 aim-4.0.0.dev3/aim.egg-info/PKG-INFO
+-rw-r--r--   0 github     (503) staff       (20)    11901 2023-04-10 17:48:50.000000 aim-4.0.0.dev3/aim.egg-info/SOURCES.txt
+-rw-r--r--   0 github     (503) staff       (20)        1 2023-04-10 17:48:50.000000 aim-4.0.0.dev3/aim.egg-info/dependency_links.txt
+-rw-r--r--   0 github     (503) staff       (20)      102 2023-04-10 17:48:50.000000 aim-4.0.0.dev3/aim.egg-info/entry_points.txt
+-rw-r--r--   0 github     (503) staff       (20)      422 2023-04-10 17:48:50.000000 aim-4.0.0.dev3/aim.egg-info/requires.txt
+-rw-r--r--   0 github     (503) staff       (20)       28 2023-04-10 17:48:50.000000 aim-4.0.0.dev3/aim.egg-info/top_level.txt
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.912416 aim-4.0.0.dev3/performance_tests/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.995532 aim-4.0.0.dev3/performance_tests/sdk/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/sdk/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      469 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/sdk/queries.py
+-rw-r--r--   0 github     (503) staff       (20)     1199 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/sdk/test_data_collection.py
+-rw-r--r--   0 github     (503) staff       (20)     1134 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/sdk/test_query.py
+-rw-r--r--   0 github     (503) staff       (20)     1881 2022-06-18 00:13:24.000000 aim-4.0.0.dev3/performance_tests/sdk/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.996390 aim-4.0.0.dev3/performance_tests/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      678 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/storage/test_container_open.py
+-rw-r--r--   0 github     (503) staff       (20)      690 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/storage/test_iterative_access.py
+-rw-r--r--   0 github     (503) staff       (20)      802 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/storage/test_random_access.py
+-rw-r--r--   0 github     (503) staff       (20)     1262 2022-06-18 00:13:24.000000 aim-4.0.0.dev3/performance_tests/storage/utils.py
+-rw-r--r--   0 github     (503) staff       (20)       84 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/pyproject.toml
+-rw-r--r--   0 github     (503) staff       (20)      336 2023-04-10 17:48:51.003221 aim-4.0.0.dev3/setup.cfg
+-rw-r--r--   0 github     (503) staff       (20)     6716 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/setup.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.912679 aim-4.0.0.dev3/tests/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.998347 aim-4.0.0.dev3/tests/api/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/api/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5155 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/api/test_dashboards_api.py
+-rw-r--r--   0 github     (503) staff       (20)     4335 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/tests/api/test_project_api.py
+-rw-r--r--   0 github     (503) staff       (20)    10653 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/tests/api/test_run_api.py
+-rw-r--r--   0 github     (503) staff       (20)    21533 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/tests/api/test_run_images_api.py
+-rw-r--r--   0 github     (503) staff       (20)    12787 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/tests/api/test_structured_data_api.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.999118 aim-4.0.0.dev3/tests/integrations/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/integrations/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1167 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/integrations/test_dvc_metadata.py
+-rw-r--r--   0 github     (503) staff       (20)     1093 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/tests/integrations/test_hf_datasets.py
+-rw-r--r--   0 github     (503) staff       (20)      961 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/integrations/test_hub_dataset.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:51.001562 aim-4.0.0.dev3/tests/sdk/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/sdk/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2312 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/sdk/test_image_construction.py
+-rw-r--r--   0 github     (503) staff       (20)     2665 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/tests/sdk/test_resource_tracker.py
+-rw-r--r--   0 github     (503) staff       (20)     1022 2022-11-01 00:13:35.000000 aim-4.0.0.dev3/tests/sdk/test_run_apis.py
+-rw-r--r--   0 github     (503) staff       (20)     1147 2022-09-01 19:23:53.000000 aim-4.0.0.dev3/tests/sdk/test_run_creation_checks.py
+-rw-r--r--   0 github     (503) staff       (20)     1661 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/sdk/test_run_finalization_time.py
+-rw-r--r--   0 github     (503) staff       (20)     1214 2022-11-01 00:13:35.000000 aim-4.0.0.dev3/tests/sdk/test_run_metric_types.py
+-rw-r--r--   0 github     (503) staff       (20)     4631 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/tests/sdk/test_run_track_type_checking.py
+-rw-r--r--   0 github     (503) staff       (20)    10444 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/tests/sdk/test_run_write_container_data.py
+-rw-r--r--   0 github     (503) staff       (20)     4517 2022-06-01 01:05:15.000000 aim-4.0.0.dev3/tests/sdk/test_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:51.002535 aim-4.0.0.dev3/tests/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5677 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/tests/storage/test_query.py
+-rw-r--r--   0 github     (503) staff       (20)     1482 2022-06-18 00:13:24.000000 aim-4.0.0.dev3/tests/storage/test_query_with_epoch_none.py
+-rw-r--r--   0 github     (503) staff       (20)     1342 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/tests/storage/test_structured_db.py
```

### Comparing `aim-4.0.0.dev2/LICENSE` & `aim-4.0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/PKG-INFO` & `aim-4.0.0.dev3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aim
-Version: 4.0.0.dev2
+Version: 4.0.0.dev3
 Summary: A super-easy way to record, search and compare AI experiments.
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,25 +20,27 @@
     <tbody>
       <tr>
         <td>Drop a star to support Aim ⭐</td>
         <td>
           <a href="https://community.aimstack.io/">Join Aim discord community</a>
           <img width="20px" src="https://user-images.githubusercontent.com/13848158/226759622-063b725d-8b3e-4c75-80c7-11fb04b7adf5.png">
         </td>
+        <td><a href="#-aim-40">🔮 Aim 4.0 - COMING SOON!!</a></td>
       </tr>
     </tbody>
   </table>
 </div>
 
 <div align="center">
   <img src="https://user-images.githubusercontent.com/13848158/225620298-9f9293e9-a138-41fd-bd77-21d53d0490b7.png">
   <h3>
-    An easy-to-use & supercharged open-source experiment tracker
+    An easy-to-use & supercharged open-source AI metadata tracker. 
   </h3>
-  Aim logs your training runs and any AI Metadata, enables a beautiful UI to compare, observe them and an API to query them programmatically.
+  
+  Aim logs all your AI metadata(**experiments**, **prompts**, etc), enables a UI to compare & observe them and SDK to query them programmatically.
 </div>
 
 <br/>
 
 <div align="center">
   
   [![Discord Server](https://dcbadge.vercel.app/api/server/zXq2NfVdtF?compact=true&style=flat)](https://community.aimstack.io/)
@@ -114,24 +116,26 @@
   <a href="#-about"><b>About</b></a> &bull;
   <a href="#-demos"><b>Demos</b></a> &bull;
   <a href="#-ecosystem"><b>Ecosystem</b></a> &bull;
   <a href="#-quick-start"><b>Quick Start</b></a> &bull;
   <a href="https://github.com/aimhubio/aim/tree/main/examples"><b>Examples</b></a> &bull;
   <a href="https://aimstack.readthedocs.io/en/latest/"><b>Documentation</b></a> &bull;
   <a href="#-community"><b>Community</b></a> &bull;
-  <a href="https://aimstack.io/blog"><b>Blog</b></a>
+  <a href="https://aimstack.io/blog"><b>Blog</b></a> &bull;
+  <a href="#-aim-40"><b>COMING SOON!!</b></a>
 </h3>  
 
 ---
 
 # ℹ️ About
 
-Aim is an open-source, self-hosted ML experiment tracking tool designed to handle 10,000s of training runs.
+Aim is an open-source, self-hosted AI Metadata tracking tool designed to handle 100,000s of tracked metadata sequences.
+Two most famous AI metadata applications are: experiment tracking and prompt engineering.
 
-Aim provides a performant and beautiful UI for exploring and comparing training runs.
+Aim provides a performant and beautiful UI for exploring and comparing training runs, prompt sessions.
 Additionally, its SDK enables programmatic access to tracked metadata — perfect for automations and Jupyter Notebook analysis.
 
 <p align="center">
   <strong>Aim's mission is to democratize AI dev tools 🎯 </strong>
 </p>
 
 <div align="center">
@@ -184,14 +188,28 @@
             <li>Runs grouping with tags and experiments</li></ul>
         </td>
       </tr>
     </tbody>
   </table>
 </div>
 
+# 🔮 Aim 4.0
+**Aim 4.0 is coming soon!!**
+
+A major iteration of Aim as the ultimate metadata library to track all your interactions with your models - including experiments, prompts etc.
+
+- Remote first
+- Scalable 
+- Capable of storing and querying 100,000s of metadata sequences
+- Custom UI dashboards and reports
+
+The Aim experiment tracker is not just one-off experiment tracker.
+It's built on top of the metadata library that Aim is. Now you can also do prompt engineering on Aim.
+Stay tuned for more...
+
 # 🎬 Demos
 
 Check out live Aim demos NOW to see it in action.
 
 | [Machine translation experiments](http://play.aimstack.io:10001/metrics?grouping=HQGdK9Xxy35e6sY1CYkCmk1WbWMN2AsCNfJJ3d1RJYLtrVPMoF5UpGiA6CF8bEJnfzRsKpqespf3AEuKSVrhUYvYk9MxzNGA9XZWYUf6phEg8AMbZGLRVDXnAPDuo8tueqsST1ZLizWzQwDYJWHUza6pyB2Eojt9uWqNHUdb858TqDRnCJzqiVJXKXEzFWUyvU8MckJo1qpqWWCTb4GpYN6DUJZx2GXDGR21e2xxd4m7PmNUnbA9B3apLttZoipJF6c3v7tNUKmb6irpqnNB3yc57tqYDa1XZuKfDxkMtyFdQ1x95K4jjsTVwhftEWLze35QNcxNXRCGGS9o9yEfTLG26GUX2zjPZFCjjMGU6vV7z1xRccK8MyoGrLSgAQCbvk68dTGBHpXUBvCRq8N&chart=FviZzVrt4fVQPjpCLr9sVGGrcR5etSroyqambiKpm3nTgpyv4eQxKuwNX9uN8UtKmzYUhUyTMBEANHmtbwjLApkvnYeNbxGNC6PVcoqi65m1XJnSrvgt8WiD89BapFAWRUwAGx6SWD7KZPsk3RQyysU7W7FjD3Q99NusxFGhsEfD6HXc7i8xH9KHDRGjLwh6x9VTtSp4FS8HEvpLSiiJoX7LCTi8pB7dXvrQ8G5w3jPsFz4qXYFdsVaCNL1BpFFZuiqQNkfbnM84gEq7UmiV1VzM4oS3AgQHxADG3kpBVp6eKTey9F1Swd4FcUkFA9QEPjgQgqwRGjkquZ2bdDDVLBnCh7JPvboP2kifCiZZ5MDdV9MMx6PKHp4DusWyWLXiHQYPkpGPWBiuccMUXDsuJaCWJbuABdY7CyiJMv1jdHYkjabygSxehPVyEDefWAtjBfv2vaeM1xv63jadbmpKYFxft7qmuT9HvVxiGvRgs4RQFxy8K4rtFBca3HNs1mDaaY81gy9MGXyw7BS5Fniu92jaJpsWDdg6Y3AQBLZtrpJy2obEZ4yzJaCVT7JUNPAyyCUNLck393VFLoEkaD9CU5npK5R7tj1c1G3gkMNQXnSXy5NpSj8deMmXV5qz3JKu1nq2caGQKcqjzy2gLkExdm674AMFjSg9yFjK6VqASXQ17NKtWRUvaYoxGbHDAFQaMKWKh8QLm22QA9mKT8NksLptWozbgDvafnQLNMvezLU5bvKV5o75PAWYiRB56RcYfEhzaB6YWdgL7TJicyY5rFi6Az8UZ7wqB3N5iMuZdpxhKn5KbZDxyuUMuvVt24i5LVPPmmwQtqxMoJ4aLo48a2YvDW6TAkdQjNjvn6KcEEz6GTixujb1YHhMUD8v4AepWKEwKz1ddEca1P2wLQjbpihCuaqbxeohnuZZLogJdUBojBEDgrnrrVpPBaLLEkGSpkJbtrsKUuEeBo1AF3yNgHftLbynGpobVF5DhmsmddmiA6c8vSTokJxHhjpnW8mAcNHBRtmVJCT7VkdHSAhNypM4Hivwfx5jCccG9LauKmCeRMDzHiA57TX9W6ttcPHSvUyQorARQAd2oeNY4H83hZjHh9Bt8iwKZRt4xK6hrTR8tif7hq8eURXrGH9Ys7TzykXK8FHHWvLNzNnYf3E4a9NkD43MjfKvMM1hj4Q2K8MHbmRCqrmFrHP5kim9shq6mhLPTgwha32nvnrBkfPQVPwpGTzKuwE&select=CdsQ7jVNkogQhRzQR3e28Ek39AZ4Ma2y37k5zJaf9EZmQhMjy8GtGm4LGU6dRFuAVG7mYww5xDrQAE74KHQ3Kk1e6661RmcmNALAUjtHyCmrTVBMCnBGNiuq1y7EzmxoodYHU1BV1rnoefQAw2kTBtbWi11hV1P4LcwFCcXfUWF6rpRC7ehEnUCTqUV4bkGVJPLcmk9mdmiGwa2YgmnSShNGPVGZiEi1rMVECyngSRVdqdZwAeXBGWFLfqF1KbZeCo4MTF4SSmFupJ9zLhYbuojEbopyFWHQ6xs3sq9epPeaQziLM4Js7oFYRmuFWUYdFqnZngmewXWmi7tQAgVqhiT6dMjG2eTdfgX6WuRSuoHALkh2XJhHA6GfZLUcxC5Ni9YyKuBTamtaYarbNNJJ8z15WWvuUkLpjgHdEpE2h924xFdu8aoZNuiQxYGvcndaW1BTGMXS5fTKPqYfe2n8Ky2HWPkcX3hEXtyawu1F9BndKNaXLPgsdAoFBArBZnSe28YtSmTa5LRucKVBAxakvv5MWMXchAmpaGFQbZyYUoMgQLcJd7Y96x6zSR7nhwr5Ar81BrmqYz2WFLuk7osUbwsc9HbSG6CQt8p6Vg2u7DjKaZXW8pjkPHAKrHWtHEDiJPJ5rj6VsdFm3) | [lightweight-GAN experiments](http://play.aimstack.io:10002/images?grouping=E1zQzcmtDR3wibEa1MVysTvCyZEv1T8ixkCxTWExCyMnHtX2HyiF9eszvPgfd2xdJ5TUTKGpSs1bsLVq5tHAV3uWtsZmmckn6HjNtVCMyQDJpwhiEy5tAyw&select=2NEXuD7fFoaLcwRjymjA1wLmUrGs9s3AiXcCW82C367SwJt18CAB6xzkMGowrUDuDwggE1huaPVcQJpQUsmAQx1CnGiqCUBp2jPMd5mMNPX2QKQMcmvu9ZykBNkeBvCQFPd9ERuQD2g1EjWuvyJ3H53mAZTfp94LCXvR9CUsG5ei2CjQUzfZLM6DCyUr1GPaEVnY5f1EwzicNxXuoutkBgqCqaobJ7Do4q4eHAA6ooiWU6ekS3D2sLj6qYwhVTjfGCPfbWwBiH83nFkY3fLExzdeTY2zeUHeeYikQR9S7xHbVD8WvjekdQVp8X4dNLJZxiVmEqHpPRnU3ZrYsMhE7yFAAgjJwPNUzLTt6YFrtZBcmc4rwAC2oyrqysUSEr6gzL6LcJ6yuqDGf9D5tzftHbTLDkhc8B2sCgTS&images=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)|
 |:---:|:---:|
 | <a href="http://play.aimstack.io:10001/metrics?grouping=HQGdK9Xxy35e6sY1CYkCmk1WbWMN2AsCNfJJ3d1RJYLtrVPMoF5UpGiA6CF8bEJnfzRsKpqespf3AEuKSVrhUYvYk9MxzNGA9XZWYUf6phEg8AMbZGLRVDXnAPDuo8tueqsST1ZLizWzQwDYJWHUza6pyB2Eojt9uWqNHUdb858TqDRnCJzqiVJXKXEzFWUyvU8MckJo1qpqWWCTb4GpYN6DUJZx2GXDGR21e2xxd4m7PmNUnbA9B3apLttZoipJF6c3v7tNUKmb6irpqnNB3yc57tqYDa1XZuKfDxkMtyFdQ1x95K4jjsTVwhftEWLze35QNcxNXRCGGS9o9yEfTLG26GUX2zjPZFCjjMGU6vV7z1xRccK8MyoGrLSgAQCbvk68dTGBHpXUBvCRq8N&chart=FviZzVrt4fVQPjpCLr9sVGGrcR5etSroyqambiKpm3nTgpyv4eQxKuwNX9uN8UtKmzYUhUyTMBEANHmtbwjLApkvnYeNbxGNC6PVcoqi65m1XJnSrvgt8WiD89BapFAWRUwAGx6SWD7KZPsk3RQyysU7W7FjD3Q99NusxFGhsEfD6HXc7i8xH9KHDRGjLwh6x9VTtSp4FS8HEvpLSiiJoX7LCTi8pB7dXvrQ8G5w3jPsFz4qXYFdsVaCNL1BpFFZuiqQNkfbnM84gEq7UmiV1VzM4oS3AgQHxADG3kpBVp6eKTey9F1Swd4FcUkFA9QEPjgQgqwRGjkquZ2bdDDVLBnCh7JPvboP2kifCiZZ5MDdV9MMx6PKHp4DusWyWLXiHQYPkpGPWBiuccMUXDsuJaCWJbuABdY7CyiJMv1jdHYkjabygSxehPVyEDefWAtjBfv2vaeM1xv63jadbmpKYFxft7qmuT9HvVxiGvRgs4RQFxy8K4rtFBca3HNs1mDaaY81gy9MGXyw7BS5Fniu92jaJpsWDdg6Y3AQBLZtrpJy2obEZ4yzJaCVT7JUNPAyyCUNLck393VFLoEkaD9CU5npK5R7tj1c1G3gkMNQXnSXy5NpSj8deMmXV5qz3JKu1nq2caGQKcqjzy2gLkExdm674AMFjSg9yFjK6VqASXQ17NKtWRUvaYoxGbHDAFQaMKWKh8QLm22QA9mKT8NksLptWozbgDvafnQLNMvezLU5bvKV5o75PAWYiRB56RcYfEhzaB6YWdgL7TJicyY5rFi6Az8UZ7wqB3N5iMuZdpxhKn5KbZDxyuUMuvVt24i5LVPPmmwQtqxMoJ4aLo48a2YvDW6TAkdQjNjvn6KcEEz6GTixujb1YHhMUD8v4AepWKEwKz1ddEca1P2wLQjbpihCuaqbxeohnuZZLogJdUBojBEDgrnrrVpPBaLLEkGSpkJbtrsKUuEeBo1AF3yNgHftLbynGpobVF5DhmsmddmiA6c8vSTokJxHhjpnW8mAcNHBRtmVJCT7VkdHSAhNypM4Hivwfx5jCccG9LauKmCeRMDzHiA57TX9W6ttcPHSvUyQorARQAd2oeNY4H83hZjHh9Bt8iwKZRt4xK6hrTR8tif7hq8eURXrGH9Ys7TzykXK8FHHWvLNzNnYf3E4a9NkD43MjfKvMM1hj4Q2K8MHbmRCqrmFrHP5kim9shq6mhLPTgwha32nvnrBkfPQVPwpGTzKuwE&select=CdsQ7jVNkogQhRzQR3e28Ek39AZ4Ma2y37k5zJaf9EZmQhMjy8GtGm4LGU6dRFuAVG7mYww5xDrQAE74KHQ3Kk1e6661RmcmNALAUjtHyCmrTVBMCnBGNiuq1y7EzmxoodYHU1BV1rnoefQAw2kTBtbWi11hV1P4LcwFCcXfUWF6rpRC7ehEnUCTqUV4bkGVJPLcmk9mdmiGwa2YgmnSShNGPVGZiEi1rMVECyngSRVdqdZwAeXBGWFLfqF1KbZeCo4MTF4SSmFupJ9zLhYbuojEbopyFWHQ6xs3sq9epPeaQziLM4Js7oFYRmuFWUYdFqnZngmewXWmi7tQAgVqhiT6dMjG2eTdfgX6WuRSuoHALkh2XJhHA6GfZLUcxC5Ni9YyKuBTamtaYarbNNJJ8z15WWvuUkLpjgHdEpE2h924xFdu8aoZNuiQxYGvcndaW1BTGMXS5fTKPqYfe2n8Ky2HWPkcX3hEXtyawu1F9BndKNaXLPgsdAoFBArBZnSe28YtSmTa5LRucKVBAxakvv5MWMXchAmpaGFQbZyYUoMgQLcJd7Y96x6zSR7nhwr5Ar81BrmqYz2WFLuk7osUbwsc9HbSG6CQt8p6Vg2u7DjKaZXW8pjkPHAKrHWtHEDiJPJ5rj6VsdFm3"> <img src="https://user-images.githubusercontent.com/97726819/225964524-0051c2c7-8554-43ae-82b8-adcb77bcf1ba.png"> </a> | <a href="http://play.aimstack.io:10002/images?grouping=E1zQzcmtDR3wibEa1MVysTvCyZEv1T8ixkCxTWExCyMnHtX2HyiF9eszvPgfd2xdJ5TUTKGpSs1bsLVq5tHAV3uWtsZmmckn6HjNtVCMyQDJpwhiEy5tAyw&select=2NEXuD7fFoaLcwRjymjA1wLmUrGs9s3AiXcCW82C367SwJt18CAB6xzkMGowrUDuDwggE1huaPVcQJpQUsmAQx1CnGiqCUBp2jPMd5mMNPX2QKQMcmvu9ZykBNkeBvCQFPd9ERuQD2g1EjWuvyJ3H53mAZTfp94LCXvR9CUsG5ei2CjQUzfZLM6DCyUr1GPaEVnY5f1EwzicNxXuoutkBgqCqaobJ7Do4q4eHAA6ooiWU6ekS3D2sLj6qYwhVTjfGCPfbWwBiH83nFkY3fLExzdeTY2zeUHeeYikQR9S7xHbVD8WvjekdQVp8X4dNLJZxiVmEqHpPRnU3ZrYsMhE7yFAAgjJwPNUzLTt6YFrtZBcmc4rwAC2oyrqysUSEr6gzL6LcJ6yuqDGf9D5tzftHbTLDkhc8B2sCgTS&images=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"> <img src="https://user-images.githubusercontent.com/97726819/225948275-a41946ea-89f4-45f1-bce1-251c84dcddca.png"> </a> |
```

#### html2text {}

```diff
@@ -1,24 +1,27 @@
-Metadata-Version: 2.1 Name: aim Version: 4.0.0.dev2 Summary: A super-easy way
+Metadata-Version: 2.1 Name: aim Version: 4.0.0.dev3 Summary: A super-easy way
 to record, search and compare AI experiments. Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
 Python: >=3.7.0 Description-Content-Type: text/markdown License-File: LICENSE
-                               Join_Aim_discord_community [https://user-
-Drop a star to support Aim â­images.githubusercontent.com/13848158/226759622-
-                               063b725d-8b3e-4c75-80c7-11fb04b7adf5.png]
+                       Join_Aim_discord_community
+                       [https://user-
+Drop a star to support images.githubusercontent.com/ ð®_Aim_4.0_-_COMING
+Aim â­             13848158/226759622-063b725d-  SOON!!
+                       8b3e-4c75-80c7-
+                       11fb04b7adf5.png]
  [https://user-images.githubusercontent.com/13848158/225620298-9f9293e9-a138-
                           41fd-bd77-21d53d0490b7.png]
-    **** An easy-to-use & supercharged open-source experiment tracker ****
-  Aim logs your training runs and any AI Metadata, enables a beautiful UI to
-       compare, observe them and an API to query them programmatically.
+   **** An easy-to-use & supercharged open-source AI metadata tracker. ****
+Aim logs all your AI metadata(**experiments**, **prompts**, etc), enables a UI
+       to compare & observe them and SDK to query them programmatically.
 
            [![Discord Server](https://dcbadge.vercel.app/api/server/
 zXq2NfVdtF?compact=true&style=flat)](https://community.aimstack.io/) [![Twitter
 Follow](https://img.shields.io/twitter/follow/aimstackio?style=social)](https:/
    /twitter.com/aimstackio) [![Medium](https://img.shields.io/badge/Medium-
 12100E?style=flat&logo=medium&logoColor=white)](https://medium.com/aimstack) [!
  [Platform Support](https://img.shields.io/badge/platform-Linux%20%7C%20macOS-
@@ -77,20 +80,21 @@
     bf1bc685477b.png] [https://user-images.githubusercontent.com/97726819/
               225953432-4b27653a-aa12-4fbf-897c-01349afa2ad0.png]
 
     AimStack offers enterprise support that's beyond core Aim. Contact via
                            hello@aimstack.io e-mail.
 ---
    **** About • Demos • Ecosystem • Quick_Start • Examples • Documentation •
-                             Community • Blog ****
---- # â¹ï¸ About Aim is an open-source, self-hosted ML experiment tracking
-tool designed to handle 10,000s of training runs. Aim provides a performant and
-beautiful UI for exploring and comparing training runs. Additionally, its SDK
-enables programmatic access to tracked metadata â perfect for automations and
-Jupyter Notebook analysis.
+                     Community • Blog • COMING_SOON!! ****
+--- # â¹ï¸ About Aim is an open-source, self-hosted AI Metadata tracking tool
+designed to handle 100,000s of tracked metadata sequences. Two most famous AI
+metadata applications are: experiment tracking and prompt engineering. Aim
+provides a performant and beautiful UI for exploring and comparing training
+runs, prompt sessions. Additionally, its SDK enables programmatic access to
+tracked metadata â perfect for automations and Jupyter Notebook analysis.
                Aim's mission is to democratize AI dev tools ð¯
  [https://user-images.githubusercontent.com/13848158/226426018-f7c11c9b-78d9-
     4ee4-b292-df28b3e8eaa6.jpg] [https://user-images.githubusercontent.com/
   13848158/226426005-f7e83923-0f92-44a4-88e4-1735a3d3e119.jpg] [https://user-
    images.githubusercontent.com/13848158/226426015-4f1122d8-c96a-443f-8698-
                                3db942b1972a.jpg]
 Log Metadata Across Your ML Pipeline  Visualize & Compare Metadata via UI ð
@@ -104,16 +108,23 @@
 Run ML Trainings Effectively â¡   Organize Your Experiments ðï¸
     * System info and resource usage      * Detailed run information for easy
       tracking                              debugging
     * Real-time alerting on training      * Centralized dashboard for holistic
       progress                              view
     * Logging and configurable            * Runs grouping with tags and
       notifications                         experiments
-# ð¬ Demos Check out live Aim demos NOW to see it in action. | [Machine
-translation experiments](http://play.aimstack.io:10001/
+# ð® Aim 4.0 **Aim 4.0 is coming soon!!** A major iteration of Aim as the
+ultimate metadata library to track all your interactions with your models -
+including experiments, prompts etc. - Remote first - Scalable - Capable of
+storing and querying 100,000s of metadata sequences - Custom UI dashboards and
+reports The Aim experiment tracker is not just one-off experiment tracker. It's
+built on top of the metadata library that Aim is. Now you can also do prompt
+engineering on Aim. Stay tuned for more... # ð¬ Demos Check out live Aim
+demos NOW to see it in action. | [Machine translation experiments](http://
+play.aimstack.io:10001/
 metrics?grouping=HQGdK9Xxy35e6sY1CYkCmk1WbWMN2AsCNfJJ3d1RJYLtrVPMoF5UpGiA6CF8bEJnfzRsKpqespf3AEuKSVrhUYvYk9MxzNGA9XZWYUf6phEg8AMbZGLRVDXnAPDuo8tueqsST1ZLizWzQwDYJWHUza6pyB2Eojt9uWqNHUdb858TqDRnCJzqiVJXKXEzFWUyvU8MckJo1qpqWWCTb4GpYN6DUJZx2GXDGR21e2xxd4m7PmNUnbA9B3apLttZoipJF6c3v7tNUKmb6irpqnNB3yc57tqYDa1XZuKfDxkMtyFdQ1x95K4jjsTVwhftEWLze35QNcxNXRCGGS9o9yEfTLG26GUX2zjPZFCjjMGU6vV7z1xRccK8MyoGrLSgAQCbvk68dTGBHpXUBvCRq8N&chart=FviZzVrt4fVQPjpCLr9sVGGrcR5etSroyqambiKpm3nTgpyv4eQxKuwNX9uN8UtKmzYUhUyTMBEANHmtbwjLApkvnYeNbxGNC6PVcoqi65m1XJnSrvgt8WiD89BapFAWRUwAGx6SWD7KZPsk3RQyysU7W7FjD3Q99NusxFGhsEfD6HXc7i8xH9KHDRGjLwh6x9VTtSp4FS8HEvpLSiiJoX7LCTi8pB7dXvrQ8G5w3jPsFz4qXYFdsVaCNL1BpFFZuiqQNkfbnM84gEq7UmiV1VzM4oS3AgQHxADG3kpBVp6eKTey9F1Swd4FcUkFA9QEPjgQgqwRGjkquZ2bdDDVLBnCh7JPvboP2kifCiZZ5MDdV9MMx6PKHp4DusWyWLXiHQYPkpGPWBiuccMUXDsuJaCWJbuABdY7CyiJMv1jdHYkjabygSxehPVyEDefWAtjBfv2vaeM1xv63jadbmpKYFxft7qmuT9HvVxiGvRgs4RQFxy8K4rtFBca3HNs1mDaaY81gy9MGXyw7BS5Fniu92jaJpsWDdg6Y3AQBLZtrpJy2obEZ4yzJaCVT7JUNPAyyCUNLck393VFLoEkaD9CU5npK5R7tj1c1G3gkMNQXnSXy5NpSj8deMmXV5qz3JKu1nq2caGQKcqjzy2gLkExdm674AMFjSg9yFjK6VqASXQ17NKtWRUvaYoxGbHDAFQaMKWKh8QLm22QA9mKT8NksLptWozbgDvafnQLNMvezLU5bvKV5o75PAWYiRB56RcYfEhzaB6YWdgL7TJicyY5rFi6Az8UZ7wqB3N5iMuZdpxhKn5KbZDxyuUMuvVt24i5LVPPmmwQtqxMoJ4aLo48a2YvDW6TAkdQjNjvn6KcEEz6GTixujb1YHhMUD8v4AepWKEwKz1ddEca1P2wLQjbpihCuaqbxeohnuZZLogJdUBojBEDgrnrrVpPBaLLEkGSpkJbtrsKUuEeBo1AF3yNgHftLbynGpobVF5DhmsmddmiA6c8vSTokJxHhjpnW8mAcNHBRtmVJCT7VkdHSAhNypM4Hivwfx5jCccG9LauKmCeRMDzHiA57TX9W6ttcPHSvUyQorARQAd2oeNY4H83hZjHh9Bt8iwKZRt4xK6hrTR8tif7hq8eURXrGH9Ys7TzykXK8FHHWvLNzNnYf3E4a9NkD43MjfKvMM1hj4Q2K8MHbmRCqrmFrHP5kim9shq6mhLPTgwha32nvnrBkfPQVPwpGTzKuwE&select=CdsQ7jVNkogQhRzQR3e28Ek39AZ4Ma2y37k5zJaf9EZmQhMjy8GtGm4LGU6dRFuAVG7mYww5xDrQAE74KHQ3Kk1e6661RmcmNALAUjtHyCmrTVBMCnBGNiuq1y7EzmxoodYHU1BV1rnoefQAw2kTBtbWi11hV1P4LcwFCcXfUWF6rpRC7ehEnUCTqUV4bkGVJPLcmk9mdmiGwa2YgmnSShNGPVGZiEi1rMVECyngSRVdqdZwAeXBGWFLfqF1KbZeCo4MTF4SSmFupJ9zLhYbuojEbopyFWHQ6xs3sq9epPeaQziLM4Js7oFYRmuFWUYdFqnZngmewXWmi7tQAgVqhiT6dMjG2eTdfgX6WuRSuoHALkh2XJhHA6GfZLUcxC5Ni9YyKuBTamtaYarbNNJJ8z15WWvuUkLpjgHdEpE2h924xFdu8aoZNuiQxYGvcndaW1BTGMXS5fTKPqYfe2n8Ky2HWPkcX3hEXtyawu1F9BndKNaXLPgsdAoFBArBZnSe28YtSmTa5LRucKVBAxakvv5MWMXchAmpaGFQbZyYUoMgQLcJd7Y96x6zSR7nhwr5Ar81BrmqYz2WFLuk7osUbwsc9HbSG6CQt8p6Vg2u7DjKaZXW8pjkPHAKrHWtHEDiJPJ5rj6VsdFm3)
 | [lightweight-GAN experiments](http://play.aimstack.io:10002/
 images?grouping=E1zQzcmtDR3wibEa1MVysTvCyZEv1T8ixkCxTWExCyMnHtX2HyiF9eszvPgfd2xdJ5TUTKGpSs1bsLVq5tHAV3uWtsZmmckn6HjNtVCMyQDJpwhiEy5tAyw&select=2NEXuD7fFoaLcwRjymjA1wLmUrGs9s3AiXcCW82C367SwJt18CAB6xzkMGowrUDuDwggE1huaPVcQJpQUsmAQx1CnGiqCUBp2jPMd5mMNPX2QKQMcmvu9ZykBNkeBvCQFPd9ERuQD2g1EjWuvyJ3H53mAZTfp94LCXvR9CUsG5ei2CjQUzfZLM6DCyUr1GPaEVnY5f1EwzicNxXuoutkBgqCqaobJ7Do4q4eHAA6ooiWU6ekS3D2sLj6qYwhVTjfGCPfbWwBiH83nFkY3fLExzdeTY2zeUHeeYikQR9S7xHbVD8WvjekdQVp8X4dNLJZxiVmEqHpPRnU3ZrYsMhE7yFAAgjJwPNUzLTt6YFrtZBcmc4rwAC2oyrqysUSEr6gzL6LcJ6yuqDGf9D5tzftHbTLDkhc8B2sCgTS&images=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)|
 |:---:|:---:| | [https://user-images.githubusercontent.com/97726819/225964524-
 0051c2c7-8554-43ae-82b8-adcb77bcf1ba.png] | [https://user-
 images.githubusercontent.com/97726819/225948275-a41946ea-89f4-45f1-bce1-
 251c84dcddca.png] | | Training logs of a neural translation model(from WMT'19
```

### Comparing `aim-4.0.0.dev2/README.md` & `aim-4.0.0.dev3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,27 @@
     <tbody>
       <tr>
         <td>Drop a star to support Aim ⭐</td>
         <td>
           <a href="https://community.aimstack.io/">Join Aim discord community</a>
           <img width="20px" src="https://user-images.githubusercontent.com/13848158/226759622-063b725d-8b3e-4c75-80c7-11fb04b7adf5.png">
         </td>
+        <td><a href="#-aim-40">🔮 Aim 4.0 - COMING SOON!!</a></td>
       </tr>
     </tbody>
   </table>
 </div>
 
 <div align="center">
   <img src="https://user-images.githubusercontent.com/13848158/225620298-9f9293e9-a138-41fd-bd77-21d53d0490b7.png">
   <h3>
-    An easy-to-use & supercharged open-source experiment tracker
+    An easy-to-use & supercharged open-source AI metadata tracker. 
   </h3>
-  Aim logs your training runs and any AI Metadata, enables a beautiful UI to compare, observe them and an API to query them programmatically.
+  
+  Aim logs all your AI metadata(**experiments**, **prompts**, etc), enables a UI to compare & observe them and SDK to query them programmatically.
 </div>
 
 <br/>
 
 <div align="center">
   
   [![Discord Server](https://dcbadge.vercel.app/api/server/zXq2NfVdtF?compact=true&style=flat)](https://community.aimstack.io/)
@@ -97,24 +99,26 @@
   <a href="#-about"><b>About</b></a> &bull;
   <a href="#-demos"><b>Demos</b></a> &bull;
   <a href="#-ecosystem"><b>Ecosystem</b></a> &bull;
   <a href="#-quick-start"><b>Quick Start</b></a> &bull;
   <a href="https://github.com/aimhubio/aim/tree/main/examples"><b>Examples</b></a> &bull;
   <a href="https://aimstack.readthedocs.io/en/latest/"><b>Documentation</b></a> &bull;
   <a href="#-community"><b>Community</b></a> &bull;
-  <a href="https://aimstack.io/blog"><b>Blog</b></a>
+  <a href="https://aimstack.io/blog"><b>Blog</b></a> &bull;
+  <a href="#-aim-40"><b>COMING SOON!!</b></a>
 </h3>  
 
 ---
 
 # ℹ️ About
 
-Aim is an open-source, self-hosted ML experiment tracking tool designed to handle 10,000s of training runs.
+Aim is an open-source, self-hosted AI Metadata tracking tool designed to handle 100,000s of tracked metadata sequences.
+Two most famous AI metadata applications are: experiment tracking and prompt engineering.
 
-Aim provides a performant and beautiful UI for exploring and comparing training runs.
+Aim provides a performant and beautiful UI for exploring and comparing training runs, prompt sessions.
 Additionally, its SDK enables programmatic access to tracked metadata — perfect for automations and Jupyter Notebook analysis.
 
 <p align="center">
   <strong>Aim's mission is to democratize AI dev tools 🎯 </strong>
 </p>
 
 <div align="center">
@@ -167,14 +171,28 @@
             <li>Runs grouping with tags and experiments</li></ul>
         </td>
       </tr>
     </tbody>
   </table>
 </div>
 
+# 🔮 Aim 4.0
+**Aim 4.0 is coming soon!!**
+
+A major iteration of Aim as the ultimate metadata library to track all your interactions with your models - including experiments, prompts etc.
+
+- Remote first
+- Scalable 
+- Capable of storing and querying 100,000s of metadata sequences
+- Custom UI dashboards and reports
+
+The Aim experiment tracker is not just one-off experiment tracker.
+It's built on top of the metadata library that Aim is. Now you can also do prompt engineering on Aim.
+Stay tuned for more...
+
 # 🎬 Demos
 
 Check out live Aim demos NOW to see it in action.
 
 | [Machine translation experiments](http://play.aimstack.io:10001/metrics?grouping=HQGdK9Xxy35e6sY1CYkCmk1WbWMN2AsCNfJJ3d1RJYLtrVPMoF5UpGiA6CF8bEJnfzRsKpqespf3AEuKSVrhUYvYk9MxzNGA9XZWYUf6phEg8AMbZGLRVDXnAPDuo8tueqsST1ZLizWzQwDYJWHUza6pyB2Eojt9uWqNHUdb858TqDRnCJzqiVJXKXEzFWUyvU8MckJo1qpqWWCTb4GpYN6DUJZx2GXDGR21e2xxd4m7PmNUnbA9B3apLttZoipJF6c3v7tNUKmb6irpqnNB3yc57tqYDa1XZuKfDxkMtyFdQ1x95K4jjsTVwhftEWLze35QNcxNXRCGGS9o9yEfTLG26GUX2zjPZFCjjMGU6vV7z1xRccK8MyoGrLSgAQCbvk68dTGBHpXUBvCRq8N&chart=FviZzVrt4fVQPjpCLr9sVGGrcR5etSroyqambiKpm3nTgpyv4eQxKuwNX9uN8UtKmzYUhUyTMBEANHmtbwjLApkvnYeNbxGNC6PVcoqi65m1XJnSrvgt8WiD89BapFAWRUwAGx6SWD7KZPsk3RQyysU7W7FjD3Q99NusxFGhsEfD6HXc7i8xH9KHDRGjLwh6x9VTtSp4FS8HEvpLSiiJoX7LCTi8pB7dXvrQ8G5w3jPsFz4qXYFdsVaCNL1BpFFZuiqQNkfbnM84gEq7UmiV1VzM4oS3AgQHxADG3kpBVp6eKTey9F1Swd4FcUkFA9QEPjgQgqwRGjkquZ2bdDDVLBnCh7JPvboP2kifCiZZ5MDdV9MMx6PKHp4DusWyWLXiHQYPkpGPWBiuccMUXDsuJaCWJbuABdY7CyiJMv1jdHYkjabygSxehPVyEDefWAtjBfv2vaeM1xv63jadbmpKYFxft7qmuT9HvVxiGvRgs4RQFxy8K4rtFBca3HNs1mDaaY81gy9MGXyw7BS5Fniu92jaJpsWDdg6Y3AQBLZtrpJy2obEZ4yzJaCVT7JUNPAyyCUNLck393VFLoEkaD9CU5npK5R7tj1c1G3gkMNQXnSXy5NpSj8deMmXV5qz3JKu1nq2caGQKcqjzy2gLkExdm674AMFjSg9yFjK6VqASXQ17NKtWRUvaYoxGbHDAFQaMKWKh8QLm22QA9mKT8NksLptWozbgDvafnQLNMvezLU5bvKV5o75PAWYiRB56RcYfEhzaB6YWdgL7TJicyY5rFi6Az8UZ7wqB3N5iMuZdpxhKn5KbZDxyuUMuvVt24i5LVPPmmwQtqxMoJ4aLo48a2YvDW6TAkdQjNjvn6KcEEz6GTixujb1YHhMUD8v4AepWKEwKz1ddEca1P2wLQjbpihCuaqbxeohnuZZLogJdUBojBEDgrnrrVpPBaLLEkGSpkJbtrsKUuEeBo1AF3yNgHftLbynGpobVF5DhmsmddmiA6c8vSTokJxHhjpnW8mAcNHBRtmVJCT7VkdHSAhNypM4Hivwfx5jCccG9LauKmCeRMDzHiA57TX9W6ttcPHSvUyQorARQAd2oeNY4H83hZjHh9Bt8iwKZRt4xK6hrTR8tif7hq8eURXrGH9Ys7TzykXK8FHHWvLNzNnYf3E4a9NkD43MjfKvMM1hj4Q2K8MHbmRCqrmFrHP5kim9shq6mhLPTgwha32nvnrBkfPQVPwpGTzKuwE&select=CdsQ7jVNkogQhRzQR3e28Ek39AZ4Ma2y37k5zJaf9EZmQhMjy8GtGm4LGU6dRFuAVG7mYww5xDrQAE74KHQ3Kk1e6661RmcmNALAUjtHyCmrTVBMCnBGNiuq1y7EzmxoodYHU1BV1rnoefQAw2kTBtbWi11hV1P4LcwFCcXfUWF6rpRC7ehEnUCTqUV4bkGVJPLcmk9mdmiGwa2YgmnSShNGPVGZiEi1rMVECyngSRVdqdZwAeXBGWFLfqF1KbZeCo4MTF4SSmFupJ9zLhYbuojEbopyFWHQ6xs3sq9epPeaQziLM4Js7oFYRmuFWUYdFqnZngmewXWmi7tQAgVqhiT6dMjG2eTdfgX6WuRSuoHALkh2XJhHA6GfZLUcxC5Ni9YyKuBTamtaYarbNNJJ8z15WWvuUkLpjgHdEpE2h924xFdu8aoZNuiQxYGvcndaW1BTGMXS5fTKPqYfe2n8Ky2HWPkcX3hEXtyawu1F9BndKNaXLPgsdAoFBArBZnSe28YtSmTa5LRucKVBAxakvv5MWMXchAmpaGFQbZyYUoMgQLcJd7Y96x6zSR7nhwr5Ar81BrmqYz2WFLuk7osUbwsc9HbSG6CQt8p6Vg2u7DjKaZXW8pjkPHAKrHWtHEDiJPJ5rj6VsdFm3) | [lightweight-GAN experiments](http://play.aimstack.io:10002/images?grouping=E1zQzcmtDR3wibEa1MVysTvCyZEv1T8ixkCxTWExCyMnHtX2HyiF9eszvPgfd2xdJ5TUTKGpSs1bsLVq5tHAV3uWtsZmmckn6HjNtVCMyQDJpwhiEy5tAyw&select=2NEXuD7fFoaLcwRjymjA1wLmUrGs9s3AiXcCW82C367SwJt18CAB6xzkMGowrUDuDwggE1huaPVcQJpQUsmAQx1CnGiqCUBp2jPMd5mMNPX2QKQMcmvu9ZykBNkeBvCQFPd9ERuQD2g1EjWuvyJ3H53mAZTfp94LCXvR9CUsG5ei2CjQUzfZLM6DCyUr1GPaEVnY5f1EwzicNxXuoutkBgqCqaobJ7Do4q4eHAA6ooiWU6ekS3D2sLj6qYwhVTjfGCPfbWwBiH83nFkY3fLExzdeTY2zeUHeeYikQR9S7xHbVD8WvjekdQVp8X4dNLJZxiVmEqHpPRnU3ZrYsMhE7yFAAgjJwPNUzLTt6YFrtZBcmc4rwAC2oyrqysUSEr6gzL6LcJ6yuqDGf9D5tzftHbTLDkhc8B2sCgTS&images=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)|
 |:---:|:---:|
 | <a href="http://play.aimstack.io:10001/metrics?grouping=HQGdK9Xxy35e6sY1CYkCmk1WbWMN2AsCNfJJ3d1RJYLtrVPMoF5UpGiA6CF8bEJnfzRsKpqespf3AEuKSVrhUYvYk9MxzNGA9XZWYUf6phEg8AMbZGLRVDXnAPDuo8tueqsST1ZLizWzQwDYJWHUza6pyB2Eojt9uWqNHUdb858TqDRnCJzqiVJXKXEzFWUyvU8MckJo1qpqWWCTb4GpYN6DUJZx2GXDGR21e2xxd4m7PmNUnbA9B3apLttZoipJF6c3v7tNUKmb6irpqnNB3yc57tqYDa1XZuKfDxkMtyFdQ1x95K4jjsTVwhftEWLze35QNcxNXRCGGS9o9yEfTLG26GUX2zjPZFCjjMGU6vV7z1xRccK8MyoGrLSgAQCbvk68dTGBHpXUBvCRq8N&chart=FviZzVrt4fVQPjpCLr9sVGGrcR5etSroyqambiKpm3nTgpyv4eQxKuwNX9uN8UtKmzYUhUyTMBEANHmtbwjLApkvnYeNbxGNC6PVcoqi65m1XJnSrvgt8WiD89BapFAWRUwAGx6SWD7KZPsk3RQyysU7W7FjD3Q99NusxFGhsEfD6HXc7i8xH9KHDRGjLwh6x9VTtSp4FS8HEvpLSiiJoX7LCTi8pB7dXvrQ8G5w3jPsFz4qXYFdsVaCNL1BpFFZuiqQNkfbnM84gEq7UmiV1VzM4oS3AgQHxADG3kpBVp6eKTey9F1Swd4FcUkFA9QEPjgQgqwRGjkquZ2bdDDVLBnCh7JPvboP2kifCiZZ5MDdV9MMx6PKHp4DusWyWLXiHQYPkpGPWBiuccMUXDsuJaCWJbuABdY7CyiJMv1jdHYkjabygSxehPVyEDefWAtjBfv2vaeM1xv63jadbmpKYFxft7qmuT9HvVxiGvRgs4RQFxy8K4rtFBca3HNs1mDaaY81gy9MGXyw7BS5Fniu92jaJpsWDdg6Y3AQBLZtrpJy2obEZ4yzJaCVT7JUNPAyyCUNLck393VFLoEkaD9CU5npK5R7tj1c1G3gkMNQXnSXy5NpSj8deMmXV5qz3JKu1nq2caGQKcqjzy2gLkExdm674AMFjSg9yFjK6VqASXQ17NKtWRUvaYoxGbHDAFQaMKWKh8QLm22QA9mKT8NksLptWozbgDvafnQLNMvezLU5bvKV5o75PAWYiRB56RcYfEhzaB6YWdgL7TJicyY5rFi6Az8UZ7wqB3N5iMuZdpxhKn5KbZDxyuUMuvVt24i5LVPPmmwQtqxMoJ4aLo48a2YvDW6TAkdQjNjvn6KcEEz6GTixujb1YHhMUD8v4AepWKEwKz1ddEca1P2wLQjbpihCuaqbxeohnuZZLogJdUBojBEDgrnrrVpPBaLLEkGSpkJbtrsKUuEeBo1AF3yNgHftLbynGpobVF5DhmsmddmiA6c8vSTokJxHhjpnW8mAcNHBRtmVJCT7VkdHSAhNypM4Hivwfx5jCccG9LauKmCeRMDzHiA57TX9W6ttcPHSvUyQorARQAd2oeNY4H83hZjHh9Bt8iwKZRt4xK6hrTR8tif7hq8eURXrGH9Ys7TzykXK8FHHWvLNzNnYf3E4a9NkD43MjfKvMM1hj4Q2K8MHbmRCqrmFrHP5kim9shq6mhLPTgwha32nvnrBkfPQVPwpGTzKuwE&select=CdsQ7jVNkogQhRzQR3e28Ek39AZ4Ma2y37k5zJaf9EZmQhMjy8GtGm4LGU6dRFuAVG7mYww5xDrQAE74KHQ3Kk1e6661RmcmNALAUjtHyCmrTVBMCnBGNiuq1y7EzmxoodYHU1BV1rnoefQAw2kTBtbWi11hV1P4LcwFCcXfUWF6rpRC7ehEnUCTqUV4bkGVJPLcmk9mdmiGwa2YgmnSShNGPVGZiEi1rMVECyngSRVdqdZwAeXBGWFLfqF1KbZeCo4MTF4SSmFupJ9zLhYbuojEbopyFWHQ6xs3sq9epPeaQziLM4Js7oFYRmuFWUYdFqnZngmewXWmi7tQAgVqhiT6dMjG2eTdfgX6WuRSuoHALkh2XJhHA6GfZLUcxC5Ni9YyKuBTamtaYarbNNJJ8z15WWvuUkLpjgHdEpE2h924xFdu8aoZNuiQxYGvcndaW1BTGMXS5fTKPqYfe2n8Ky2HWPkcX3hEXtyawu1F9BndKNaXLPgsdAoFBArBZnSe28YtSmTa5LRucKVBAxakvv5MWMXchAmpaGFQbZyYUoMgQLcJd7Y96x6zSR7nhwr5Ar81BrmqYz2WFLuk7osUbwsc9HbSG6CQt8p6Vg2u7DjKaZXW8pjkPHAKrHWtHEDiJPJ5rj6VsdFm3"> <img src="https://user-images.githubusercontent.com/97726819/225964524-0051c2c7-8554-43ae-82b8-adcb77bcf1ba.png"> </a> | <a href="http://play.aimstack.io:10002/images?grouping=E1zQzcmtDR3wibEa1MVysTvCyZEv1T8ixkCxTWExCyMnHtX2HyiF9eszvPgfd2xdJ5TUTKGpSs1bsLVq5tHAV3uWtsZmmckn6HjNtVCMyQDJpwhiEy5tAyw&select=2NEXuD7fFoaLcwRjymjA1wLmUrGs9s3AiXcCW82C367SwJt18CAB6xzkMGowrUDuDwggE1huaPVcQJpQUsmAQx1CnGiqCUBp2jPMd5mMNPX2QKQMcmvu9ZykBNkeBvCQFPd9ERuQD2g1EjWuvyJ3H53mAZTfp94LCXvR9CUsG5ei2CjQUzfZLM6DCyUr1GPaEVnY5f1EwzicNxXuoutkBgqCqaobJ7Do4q4eHAA6ooiWU6ekS3D2sLj6qYwhVTjfGCPfbWwBiH83nFkY3fLExzdeTY2zeUHeeYikQR9S7xHbVD8WvjekdQVp8X4dNLJZxiVmEqHpPRnU3ZrYsMhE7yFAAgjJwPNUzLTt6YFrtZBcmc4rwAC2oyrqysUSEr6gzL6LcJ6yuqDGf9D5tzftHbTLDkhc8B2sCgTS&images=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"> <img src="https://user-images.githubusercontent.com/97726819/225948275-a41946ea-89f4-45f1-bce1-251c84dcddca.png"> </a> |
```

#### html2text {}

```diff
@@ -1,15 +1,18 @@
-                               Join_Aim_discord_community [https://user-
-Drop a star to support Aim â­images.githubusercontent.com/13848158/226759622-
-                               063b725d-8b3e-4c75-80c7-11fb04b7adf5.png]
+                       Join_Aim_discord_community
+                       [https://user-
+Drop a star to support images.githubusercontent.com/ ð®_Aim_4.0_-_COMING
+Aim â­             13848158/226759622-063b725d-  SOON!!
+                       8b3e-4c75-80c7-
+                       11fb04b7adf5.png]
  [https://user-images.githubusercontent.com/13848158/225620298-9f9293e9-a138-
                           41fd-bd77-21d53d0490b7.png]
-    **** An easy-to-use & supercharged open-source experiment tracker ****
-  Aim logs your training runs and any AI Metadata, enables a beautiful UI to
-       compare, observe them and an API to query them programmatically.
+   **** An easy-to-use & supercharged open-source AI metadata tracker. ****
+Aim logs all your AI metadata(**experiments**, **prompts**, etc), enables a UI
+       to compare & observe them and SDK to query them programmatically.
 
            [![Discord Server](https://dcbadge.vercel.app/api/server/
 zXq2NfVdtF?compact=true&style=flat)](https://community.aimstack.io/) [![Twitter
 Follow](https://img.shields.io/twitter/follow/aimstackio?style=social)](https:/
    /twitter.com/aimstackio) [![Medium](https://img.shields.io/badge/Medium-
 12100E?style=flat&logo=medium&logoColor=white)](https://medium.com/aimstack) [!
  [Platform Support](https://img.shields.io/badge/platform-Linux%20%7C%20macOS-
@@ -68,20 +71,21 @@
     bf1bc685477b.png] [https://user-images.githubusercontent.com/97726819/
               225953432-4b27653a-aa12-4fbf-897c-01349afa2ad0.png]
 
     AimStack offers enterprise support that's beyond core Aim. Contact via
                            hello@aimstack.io e-mail.
 ---
    **** About • Demos • Ecosystem • Quick_Start • Examples • Documentation •
-                             Community • Blog ****
---- # â¹ï¸ About Aim is an open-source, self-hosted ML experiment tracking
-tool designed to handle 10,000s of training runs. Aim provides a performant and
-beautiful UI for exploring and comparing training runs. Additionally, its SDK
-enables programmatic access to tracked metadata â perfect for automations and
-Jupyter Notebook analysis.
+                     Community • Blog • COMING_SOON!! ****
+--- # â¹ï¸ About Aim is an open-source, self-hosted AI Metadata tracking tool
+designed to handle 100,000s of tracked metadata sequences. Two most famous AI
+metadata applications are: experiment tracking and prompt engineering. Aim
+provides a performant and beautiful UI for exploring and comparing training
+runs, prompt sessions. Additionally, its SDK enables programmatic access to
+tracked metadata â perfect for automations and Jupyter Notebook analysis.
                Aim's mission is to democratize AI dev tools ð¯
  [https://user-images.githubusercontent.com/13848158/226426018-f7c11c9b-78d9-
     4ee4-b292-df28b3e8eaa6.jpg] [https://user-images.githubusercontent.com/
   13848158/226426005-f7e83923-0f92-44a4-88e4-1735a3d3e119.jpg] [https://user-
    images.githubusercontent.com/13848158/226426015-4f1122d8-c96a-443f-8698-
                                3db942b1972a.jpg]
 Log Metadata Across Your ML Pipeline  Visualize & Compare Metadata via UI ð
@@ -95,16 +99,23 @@
 Run ML Trainings Effectively â¡   Organize Your Experiments ðï¸
     * System info and resource usage      * Detailed run information for easy
       tracking                              debugging
     * Real-time alerting on training      * Centralized dashboard for holistic
       progress                              view
     * Logging and configurable            * Runs grouping with tags and
       notifications                         experiments
-# ð¬ Demos Check out live Aim demos NOW to see it in action. | [Machine
-translation experiments](http://play.aimstack.io:10001/
+# ð® Aim 4.0 **Aim 4.0 is coming soon!!** A major iteration of Aim as the
+ultimate metadata library to track all your interactions with your models -
+including experiments, prompts etc. - Remote first - Scalable - Capable of
+storing and querying 100,000s of metadata sequences - Custom UI dashboards and
+reports The Aim experiment tracker is not just one-off experiment tracker. It's
+built on top of the metadata library that Aim is. Now you can also do prompt
+engineering on Aim. Stay tuned for more... # ð¬ Demos Check out live Aim
+demos NOW to see it in action. | [Machine translation experiments](http://
+play.aimstack.io:10001/
 metrics?grouping=HQGdK9Xxy35e6sY1CYkCmk1WbWMN2AsCNfJJ3d1RJYLtrVPMoF5UpGiA6CF8bEJnfzRsKpqespf3AEuKSVrhUYvYk9MxzNGA9XZWYUf6phEg8AMbZGLRVDXnAPDuo8tueqsST1ZLizWzQwDYJWHUza6pyB2Eojt9uWqNHUdb858TqDRnCJzqiVJXKXEzFWUyvU8MckJo1qpqWWCTb4GpYN6DUJZx2GXDGR21e2xxd4m7PmNUnbA9B3apLttZoipJF6c3v7tNUKmb6irpqnNB3yc57tqYDa1XZuKfDxkMtyFdQ1x95K4jjsTVwhftEWLze35QNcxNXRCGGS9o9yEfTLG26GUX2zjPZFCjjMGU6vV7z1xRccK8MyoGrLSgAQCbvk68dTGBHpXUBvCRq8N&chart=FviZzVrt4fVQPjpCLr9sVGGrcR5etSroyqambiKpm3nTgpyv4eQxKuwNX9uN8UtKmzYUhUyTMBEANHmtbwjLApkvnYeNbxGNC6PVcoqi65m1XJnSrvgt8WiD89BapFAWRUwAGx6SWD7KZPsk3RQyysU7W7FjD3Q99NusxFGhsEfD6HXc7i8xH9KHDRGjLwh6x9VTtSp4FS8HEvpLSiiJoX7LCTi8pB7dXvrQ8G5w3jPsFz4qXYFdsVaCNL1BpFFZuiqQNkfbnM84gEq7UmiV1VzM4oS3AgQHxADG3kpBVp6eKTey9F1Swd4FcUkFA9QEPjgQgqwRGjkquZ2bdDDVLBnCh7JPvboP2kifCiZZ5MDdV9MMx6PKHp4DusWyWLXiHQYPkpGPWBiuccMUXDsuJaCWJbuABdY7CyiJMv1jdHYkjabygSxehPVyEDefWAtjBfv2vaeM1xv63jadbmpKYFxft7qmuT9HvVxiGvRgs4RQFxy8K4rtFBca3HNs1mDaaY81gy9MGXyw7BS5Fniu92jaJpsWDdg6Y3AQBLZtrpJy2obEZ4yzJaCVT7JUNPAyyCUNLck393VFLoEkaD9CU5npK5R7tj1c1G3gkMNQXnSXy5NpSj8deMmXV5qz3JKu1nq2caGQKcqjzy2gLkExdm674AMFjSg9yFjK6VqASXQ17NKtWRUvaYoxGbHDAFQaMKWKh8QLm22QA9mKT8NksLptWozbgDvafnQLNMvezLU5bvKV5o75PAWYiRB56RcYfEhzaB6YWdgL7TJicyY5rFi6Az8UZ7wqB3N5iMuZdpxhKn5KbZDxyuUMuvVt24i5LVPPmmwQtqxMoJ4aLo48a2YvDW6TAkdQjNjvn6KcEEz6GTixujb1YHhMUD8v4AepWKEwKz1ddEca1P2wLQjbpihCuaqbxeohnuZZLogJdUBojBEDgrnrrVpPBaLLEkGSpkJbtrsKUuEeBo1AF3yNgHftLbynGpobVF5DhmsmddmiA6c8vSTokJxHhjpnW8mAcNHBRtmVJCT7VkdHSAhNypM4Hivwfx5jCccG9LauKmCeRMDzHiA57TX9W6ttcPHSvUyQorARQAd2oeNY4H83hZjHh9Bt8iwKZRt4xK6hrTR8tif7hq8eURXrGH9Ys7TzykXK8FHHWvLNzNnYf3E4a9NkD43MjfKvMM1hj4Q2K8MHbmRCqrmFrHP5kim9shq6mhLPTgwha32nvnrBkfPQVPwpGTzKuwE&select=CdsQ7jVNkogQhRzQR3e28Ek39AZ4Ma2y37k5zJaf9EZmQhMjy8GtGm4LGU6dRFuAVG7mYww5xDrQAE74KHQ3Kk1e6661RmcmNALAUjtHyCmrTVBMCnBGNiuq1y7EzmxoodYHU1BV1rnoefQAw2kTBtbWi11hV1P4LcwFCcXfUWF6rpRC7ehEnUCTqUV4bkGVJPLcmk9mdmiGwa2YgmnSShNGPVGZiEi1rMVECyngSRVdqdZwAeXBGWFLfqF1KbZeCo4MTF4SSmFupJ9zLhYbuojEbopyFWHQ6xs3sq9epPeaQziLM4Js7oFYRmuFWUYdFqnZngmewXWmi7tQAgVqhiT6dMjG2eTdfgX6WuRSuoHALkh2XJhHA6GfZLUcxC5Ni9YyKuBTamtaYarbNNJJ8z15WWvuUkLpjgHdEpE2h924xFdu8aoZNuiQxYGvcndaW1BTGMXS5fTKPqYfe2n8Ky2HWPkcX3hEXtyawu1F9BndKNaXLPgsdAoFBArBZnSe28YtSmTa5LRucKVBAxakvv5MWMXchAmpaGFQbZyYUoMgQLcJd7Y96x6zSR7nhwr5Ar81BrmqYz2WFLuk7osUbwsc9HbSG6CQt8p6Vg2u7DjKaZXW8pjkPHAKrHWtHEDiJPJ5rj6VsdFm3)
 | [lightweight-GAN experiments](http://play.aimstack.io:10002/
 images?grouping=E1zQzcmtDR3wibEa1MVysTvCyZEv1T8ixkCxTWExCyMnHtX2HyiF9eszvPgfd2xdJ5TUTKGpSs1bsLVq5tHAV3uWtsZmmckn6HjNtVCMyQDJpwhiEy5tAyw&select=2NEXuD7fFoaLcwRjymjA1wLmUrGs9s3AiXcCW82C367SwJt18CAB6xzkMGowrUDuDwggE1huaPVcQJpQUsmAQx1CnGiqCUBp2jPMd5mMNPX2QKQMcmvu9ZykBNkeBvCQFPd9ERuQD2g1EjWuvyJ3H53mAZTfp94LCXvR9CUsG5ei2CjQUzfZLM6DCyUr1GPaEVnY5f1EwzicNxXuoutkBgqCqaobJ7Do4q4eHAA6ooiWU6ekS3D2sLj6qYwhVTjfGCPfbWwBiH83nFkY3fLExzdeTY2zeUHeeYikQR9S7xHbVD8WvjekdQVp8X4dNLJZxiVmEqHpPRnU3ZrYsMhE7yFAAgjJwPNUzLTt6YFrtZBcmc4rwAC2oyrqysUSEr6gzL6LcJ6yuqDGf9D5tzftHbTLDkhc8B2sCgTS&images=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)|
 |:---:|:---:| | [https://user-images.githubusercontent.com/97726819/225964524-
 0051c2c7-8554-43ae-82b8-adcb77bcf1ba.png] | [https://user-
 images.githubusercontent.com/97726819/225948275-a41946ea-89f4-45f1-bce1-
 251c84dcddca.png] | | Training logs of a neural translation model(from WMT'19
```

### Comparing `aim-4.0.0.dev2/aim/__about__.py` & `aim-4.0.0.dev3/aim/__about__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/cli.py` & `aim-4.0.0.dev3/aim/cli/cli.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/convert/commands.py` & `aim-4.0.0.dev3/aim/cli/convert/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/convert/processors/mlflow.py` & `aim-4.0.0.dev3/aim/cli/convert/processors/mlflow.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/convert/processors/tensorboard.py` & `aim-4.0.0.dev3/aim/cli/convert/processors/tensorboard.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/convert/processors/wandb.py` & `aim-4.0.0.dev3/aim/cli/convert/processors/wandb.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/init/commands.py` & `aim-4.0.0.dev3/aim/cli/init/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/manager/manager.py` & `aim-4.0.0.dev3/aim/cli/manager/manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/reindex/commands.py` & `aim-4.0.0.dev3/aim/cli/reindex/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/runs/commands.py` & `aim-4.0.0.dev3/aim/cli/runs/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/runs/utils.py` & `aim-4.0.0.dev3/aim/cli/runs/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/server/commands.py` & `aim-4.0.0.dev3/aim/cli/server/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/storage/commands.py` & `aim-4.0.0.dev3/aim/cli/storage/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/up/commands.py` & `aim-4.0.0.dev3/aim/cli/up/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/up/utils.py` & `aim-4.0.0.dev3/aim/cli/up/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/configs.py` & `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/configs.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/v3/base_pb2.py` & `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v3/base_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/v3/metric_pb2.py` & `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v3/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/v4/base_pb2.py` & `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v4/base_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/proto/v4/metric_pb2.py` & `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v4/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/repo/metric.py` & `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/metric.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/repo/repo.py` & `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/repo.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/repo/run.py` & `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/repo/trace.py` & `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/trace.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/upgrade/_legacy_repo/repo/utils.py` & `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/upgrade/utils.py` & `aim-4.0.0.dev3/aim/cli/upgrade/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/cli/watcher_cli.py` & `aim-4.0.0.dev3/aim/cli/watcher_cli.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/cleanup/__init__.py` & `aim-4.0.0.dev3/aim/ext/cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/exception_resistant.py` & `aim-4.0.0.dev3/aim/ext/exception_resistant.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/notebook/notebook.py` & `aim-4.0.0.dev3/aim/ext/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/notifier/__init__.py` & `aim-4.0.0.dev3/aim/ext/notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/notifier/config.py` & `aim-4.0.0.dev3/aim/ext/notifier/config.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/notifier/logging_notifier.py` & `aim-4.0.0.dev3/aim/ext/notifier/logging_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/notifier/notifier.py` & `aim-4.0.0.dev3/aim/ext/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/notifier/notifier_builder.py` & `aim-4.0.0.dev3/aim/ext/notifier/notifier_builder.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/notifier/slack_notifier.py` & `aim-4.0.0.dev3/aim/ext/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/notifier/utils.py` & `aim-4.0.0.dev3/aim/ext/notifier/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/notifier/workplace_notifier.py` & `aim-4.0.0.dev3/aim/ext/notifier/workplace_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/resource/log.py` & `aim-4.0.0.dev3/aim/ext/resource/log.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/resource/stat.py` & `aim-4.0.0.dev3/aim/ext/resource/stat.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/resource/tracker.py` & `aim-4.0.0.dev3/aim/ext/resource/tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/sshfs/utils.py` & `aim-4.0.0.dev3/aim/ext/sshfs/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/task_queue/queue.py` & `aim-4.0.0.dev3/aim/ext/task_queue/queue.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/tensorboard_tracker/run.py` & `aim-4.0.0.dev3/aim/ext/tensorboard_tracker/run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/tensorboard_tracker/tracker.py` & `aim-4.0.0.dev3/aim/ext/tensorboard_tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/client.py` & `aim-4.0.0.dev3/aim/ext/transport/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from aim.ext.transport.rpc_queue import RpcQueueWithRetry
 from aim.ext.transport.heartbeat import RPCHeartbeatSender
 from aim.ext.transport.config import (
     AIM_CLIENT_SSL_CERTIFICATES_FILE,
     AIM_RT_MAX_MESSAGE_SIZE,
     AIM_RT_DEFAULT_MAX_MESSAGE_SIZE,
     AIM_CLIENT_QUEUE_MAX_MEMORY,
+    AIM_RT_BEARER_TOKEN,
 )
 from aim.storage.treeutils import encode_tree, decode_tree
 
 
 DEFAULT_RETRY_INTERVAL = 0.1  # 100 ms
 DEFAULT_RETRY_COUNT = 2
 
@@ -72,23 +73,29 @@
         self._sub_path = sub_path
 
     def _create_remote_channels(self):
         import grpc
 
         ssl_certfile = os.getenv(AIM_CLIENT_SSL_CERTIFICATES_FILE)
         msg_max_size = int(os.getenv(AIM_RT_MAX_MESSAGE_SIZE, AIM_RT_DEFAULT_MAX_MESSAGE_SIZE))
+        bearer_token = os.getenv(AIM_RT_BEARER_TOKEN)
         options = [
             ('grpc.max_send_message_length', msg_max_size),
             ('grpc.max_receive_message_length', msg_max_size)
         ]
 
         # open a channel with router
         if ssl_certfile:
             with open(ssl_certfile, 'rb') as f:
                 root_certificates = grpc.ssl_channel_credentials(f.read())
+            if bearer_token:
+                self._call_credentials = grpc.access_token_call_credentials(bearer_token)
+                root_certificates = grpc.composite_channel_credentials(
+                    root_certificates, self._call_credentials
+                )
             self._remote_router_channel = grpc.secure_channel(self.remote_path, root_certificates, options=options)
         else:
             self._remote_router_channel = grpc.insecure_channel(self.remote_path, options=options)
         self._remote_router_stub = remote_router_pb2_grpc.RemoteRouterServiceStub(self._remote_router_channel)
 
         # check client/server version compatibility
         self._check_remote_version_compatibility()
```

### Comparing `aim-4.0.0.dev2/aim/ext/transport/config.py` & `aim-4.0.0.dev3/aim/ext/transport/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 # The path of the PEM-encoded root certificates. Used for secure channel establishment
 AIM_CLIENT_SSL_CERTIFICATES_FILE = '__AIM_CLIENT_SSL_CERTIFICATES_FILE__'
 AIM_CLIENT_QUEUE_MAX_MEMORY = '__AIM_CLIENT_QUEUE_MAX_MEMORY__'
 
 # GRPC OPTIONS
 AIM_RT_MAX_MESSAGE_SIZE = '__AIM_RT_MAX_MESSAGE_SIZE__'
 AIM_RT_DEFAULT_MAX_MESSAGE_SIZE = 16 * 1024 * 1024  # 16MB
+AIM_RT_BEARER_TOKEN = '__AIM_RT_BEARER_TOKEN__'
```

### Comparing `aim-4.0.0.dev2/aim/ext/transport/handlers.py` & `aim-4.0.0.dev3/aim/ext/transport/handlers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/health.py` & `aim-4.0.0.dev3/aim/ext/transport/health.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/heartbeat.py` & `aim-4.0.0.dev3/aim/ext/transport/heartbeat.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/message_utils.py` & `aim-4.0.0.dev3/aim/ext/transport/message_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/proto/health_pb2_grpc.py` & `aim-4.0.0.dev3/aim/ext/transport/proto/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/proto/remote_router_pb2_grpc.py` & `aim-4.0.0.dev3/aim/ext/transport/proto/remote_router_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/proto/remote_tracking_pb2_grpc.py` & `aim-4.0.0.dev3/aim/ext/transport/proto/remote_tracking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/proto/v3/health_pb2.py` & `aim-4.0.0.dev3/aim/ext/transport/proto/v3/health_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/proto/v3/remote_router_pb2.py` & `aim-4.0.0.dev3/aim/ext/transport/proto/v3/remote_router_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/proto/v3/remote_tracking_pb2.py` & `aim-4.0.0.dev3/aim/ext/transport/proto/v3/remote_tracking_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/proto/v4/health_pb2.py` & `aim-4.0.0.dev3/aim/ext/transport/proto/v4/health_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/proto/v4/remote_router_pb2.py` & `aim-4.0.0.dev3/aim/ext/transport/proto/v4/remote_router_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/proto/v4/remote_tracking_pb2.py` & `aim-4.0.0.dev3/aim/ext/transport/proto/v4/remote_tracking_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/remote_tracking.py` & `aim-4.0.0.dev3/aim/ext/transport/remote_tracking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/router.py` & `aim-4.0.0.dev3/aim/ext/transport/router.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/rpc_queue.py` & `aim-4.0.0.dev3/aim/ext/transport/rpc_queue.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/server.py` & `aim-4.0.0.dev3/aim/ext/transport/server.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/transport/worker.py` & `aim-4.0.0.dev3/aim/ext/transport/worker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/ext/utils.py` & `aim-4.0.0.dev3/aim/ext/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/__init__.py` & `aim-4.0.0.dev3/aim/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/acme.py` & `aim-4.0.0.dev3/aim/sdk/adapters/acme.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/catboost.py` & `aim-4.0.0.dev3/aim/sdk/adapters/catboost.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/fastai.py` & `aim-4.0.0.dev3/aim/sdk/adapters/fastai.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/hugging_face.py` & `aim-4.0.0.dev3/aim/sdk/adapters/hugging_face.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/keras.py` & `aim-4.0.0.dev3/aim/sdk/adapters/keras.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/keras_mixins.py` & `aim-4.0.0.dev3/aim/sdk/adapters/keras_mixins.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/keras_tuner.py` & `aim-4.0.0.dev3/aim/sdk/adapters/keras_tuner.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/lightgbm.py` & `aim-4.0.0.dev3/aim/sdk/adapters/lightgbm.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/mxnet.py` & `aim-4.0.0.dev3/aim/sdk/adapters/mxnet.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/optuna.py` & `aim-4.0.0.dev3/aim/sdk/adapters/optuna.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/paddle.py` & `aim-4.0.0.dev3/aim/sdk/adapters/paddle.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/prophet.py` & `aim-4.0.0.dev3/aim/sdk/adapters/prophet.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/pytorch.py` & `aim-4.0.0.dev3/aim/sdk/adapters/pytorch.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/pytorch_ignite.py` & `aim-4.0.0.dev3/aim/sdk/adapters/pytorch_ignite.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/pytorch_lightning.py` & `aim-4.0.0.dev3/aim/sdk/adapters/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/sb3.py` & `aim-4.0.0.dev3/aim/sdk/adapters/sb3.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/tensorflow.py` & `aim-4.0.0.dev3/aim/sdk/adapters/tensorflow.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/adapters/xgboost.py` & `aim-4.0.0.dev3/aim/sdk/adapters/xgboost.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/base_run.py` & `aim-4.0.0.dev3/aim/sdk/base_run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/callbacks/caller.py` & `aim-4.0.0.dev3/aim/sdk/callbacks/caller.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/callbacks/helpers.py` & `aim-4.0.0.dev3/aim/sdk/callbacks/helpers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/index_manager.py` & `aim-4.0.0.dev3/aim/sdk/index_manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/legacy/select.py` & `aim-4.0.0.dev3/aim/sdk/legacy/select.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/legacy/session/session.py` & `aim-4.0.0.dev3/aim/sdk/legacy/session/session.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/lock_manager.py` & `aim-4.0.0.dev3/aim/sdk/lock_manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/logging/log_record.py` & `aim-4.0.0.dev3/aim/sdk/logging/log_record.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/maintenance_run.py` & `aim-4.0.0.dev3/aim/sdk/maintenance_run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/num_utils.py` & `aim-4.0.0.dev3/aim/sdk/num_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/objects/audio.py` & `aim-4.0.0.dev3/aim/sdk/objects/audio.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/objects/distribution.py` & `aim-4.0.0.dev3/aim/sdk/objects/distribution.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/objects/figure.py` & `aim-4.0.0.dev3/aim/sdk/objects/figure.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/objects/image.py` & `aim-4.0.0.dev3/aim/sdk/objects/image.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/objects/io/wavfile.py` & `aim-4.0.0.dev3/aim/sdk/objects/io/wavfile.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/objects/plugins/dvc_metadata.py` & `aim-4.0.0.dev3/aim/sdk/objects/plugins/dvc_metadata.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/objects/plugins/hf_datasets_metadata.py` & `aim-4.0.0.dev3/aim/sdk/objects/plugins/hf_datasets_metadata.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/objects/plugins/hub_dataset.py` & `aim-4.0.0.dev3/aim/sdk/objects/plugins/hub_dataset.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/objects/text.py` & `aim-4.0.0.dev3/aim/sdk/objects/text.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/query_utils.py` & `aim-4.0.0.dev3/aim/sdk/query_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/remote_repo_proxy.py` & `aim-4.0.0.dev3/aim/sdk/remote_repo_proxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/remote_run_reporter.py` & `aim-4.0.0.dev3/aim/sdk/remote_run_reporter.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/repo.py` & `aim-4.0.0.dev3/aim/sdk/repo.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/repo_utils.py` & `aim-4.0.0.dev3/aim/sdk/repo_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/reporter/__init__.py` & `aim-4.0.0.dev3/aim/sdk/reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/reporter/file_manager.py` & `aim-4.0.0.dev3/aim/sdk/reporter/file_manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/run.py` & `aim-4.0.0.dev3/aim/sdk/run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/run_status_watcher.py` & `aim-4.0.0.dev3/aim/sdk/run_status_watcher.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/sequence.py` & `aim-4.0.0.dev3/aim/sdk/sequence.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/sequence_collection.py` & `aim-4.0.0.dev3/aim/sdk/sequence_collection.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/sequences/metric.py` & `aim-4.0.0.dev3/aim/sdk/sequences/metric.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/tracker.py` & `aim-4.0.0.dev3/aim/sdk/tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/training_flow.py` & `aim-4.0.0.dev3/aim/sdk/training_flow.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/uri_service.py` & `aim-4.0.0.dev3/aim/sdk/uri_service.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/sdk/utils.py` & `aim-4.0.0.dev3/aim/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/arrayview.cpp` & `aim-4.0.0.dev3/aim/storage/arrayview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.arrayview",
         "sources": [
             "aim/storage/arrayview.py"
         ]
     },
     "module_name": "aim.storage.arrayview"
```

### Comparing `aim-4.0.0.dev2/aim/storage/arrayview.py` & `aim-4.0.0.dev3/aim/storage/arrayview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/container.cpp` & `aim-4.0.0.dev3/aim/storage/container.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.container",
         "sources": [
             "aim/storage/container.py"
         ]
     },
     "module_name": "aim.storage.container"
```

### Comparing `aim-4.0.0.dev2/aim/storage/container.pxd` & `aim-4.0.0.dev3/aim/storage/container.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/container.py` & `aim-4.0.0.dev3/aim/storage/container.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/containertreeview.cpp` & `aim-4.0.0.dev3/aim/storage/containertreeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.containertreeview",
         "sources": [
             "aim/storage/containertreeview.py"
         ]
     },
     "module_name": "aim.storage.containertreeview"
```

### Comparing `aim-4.0.0.dev2/aim/storage/containertreeview.py` & `aim-4.0.0.dev3/aim/storage/containertreeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/context.py` & `aim-4.0.0.dev3/aim/storage/context.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/encoding/__init__.cpp` & `aim-4.0.0.dev3/aim/storage/encoding/__init__.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.encoding",
         "sources": [
             "aim/storage/encoding/__init__.py"
         ]
     },
     "module_name": "aim.storage.encoding"
```

### Comparing `aim-4.0.0.dev2/aim/storage/encoding/encoding.cpp` & `aim-4.0.0.dev3/aim/storage/encoding/encoding.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.encoding.encoding",
         "sources": [
             "aim/storage/encoding/encoding.pyx"
         ]
     },
     "module_name": "aim.storage.encoding.encoding"
```

### Comparing `aim-4.0.0.dev2/aim/storage/encoding/encoding.pyx` & `aim-4.0.0.dev3/aim/storage/encoding/encoding.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/encoding/encoding_native.cpp` & `aim-4.0.0.dev3/aim/storage/encoding/encoding_native.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.encoding.encoding_native",
         "sources": [
             "aim/storage/encoding/encoding_native.pyx"
         ]
     },
     "module_name": "aim.storage.encoding.encoding_native"
```

### Comparing `aim-4.0.0.dev2/aim/storage/encoding/encoding_native.pxd` & `aim-4.0.0.dev3/aim/storage/encoding/encoding_native.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/encoding/encoding_native.pyx` & `aim-4.0.0.dev3/aim/storage/encoding/encoding_native.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/hashing/__init__.cpp` & `aim-4.0.0.dev3/aim/storage/hashing/__init__.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "aim/storage/hashing",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.hashing",
         "sources": [
             "aim/storage/hashing/__init__.py"
         ]
     },
     "module_name": "aim.storage.hashing"
```

### Comparing `aim-4.0.0.dev2/aim/storage/hashing/c_hash.cpp` & `aim-4.0.0.dev3/aim/storage/hashing/c_hash.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,23 +14,23 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "aim/storage/hashing",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "language_level": "3",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.hashing.c_hash",
         "sources": [
             "aim/storage/hashing/c_hash.pyx"
         ]
     },
     "module_name": "aim.storage.hashing.c_hash"
```

### Comparing `aim-4.0.0.dev2/aim/storage/hashing/c_hash.pyx` & `aim-4.0.0.dev3/aim/storage/hashing/c_hash.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/hashing/hash/hash.h` & `aim-4.0.0.dev3/aim/storage/hashing/hash/hash.h`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/hashing/hashing.cpp` & `aim-4.0.0.dev3/aim/storage/hashing/hashing.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "aim/storage/hashing",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.hashing.hashing",
         "sources": [
             "aim/storage/hashing/hashing.py"
         ]
     },
     "module_name": "aim.storage.hashing.hashing"
```

### Comparing `aim-4.0.0.dev2/aim/storage/hashing/hashing.pxd` & `aim-4.0.0.dev3/aim/storage/hashing/hashing.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/hashing/hashing.py` & `aim-4.0.0.dev3/aim/storage/hashing/hashing.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/inmemorytreeview.cpp` & `aim-4.0.0.dev3/aim/storage/inmemorytreeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.inmemorytreeview",
         "sources": [
             "aim/storage/inmemorytreeview.py"
         ]
     },
     "module_name": "aim.storage.inmemorytreeview"
```

### Comparing `aim-4.0.0.dev2/aim/storage/inmemorytreeview.py` & `aim-4.0.0.dev3/aim/storage/inmemorytreeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/lock_proxy.py` & `aim-4.0.0.dev3/aim/storage/lock_proxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/locking.py` & `aim-4.0.0.dev3/aim/storage/locking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/migrations/alembic.ini` & `aim-4.0.0.dev3/aim/storage/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/migrations/alembic_dev.ini` & `aim-4.0.0.dev3/aim/storage/migrations/alembic_dev.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/migrations/env.py` & `aim-4.0.0.dev3/aim/storage/migrations/env.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/migrations/utils.py` & `aim-4.0.0.dev3/aim/storage/migrations/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/migrations/versions/1ecf8222220d_initial_schema.py` & `aim-4.0.0.dev3/aim/storage/migrations/versions/1ecf8222220d_initial_schema.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/migrations/versions/3c4f22db7a46_run_end_time.py` & `aim-4.0.0.dev3/aim/storage/migrations/versions/3c4f22db7a46_run_end_time.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/migrations/versions/46b89d830ad8_.py` & `aim-4.0.0.dev3/aim/storage/migrations/versions/46b89d830ad8_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/migrations/versions/9ba30ab3b2b4_.py` & `aim-4.0.0.dev3/aim/storage/migrations/versions/9ba30ab3b2b4_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/migrations/versions/b07e7b07c8ce_.py` & `aim-4.0.0.dev3/aim/storage/migrations/versions/b07e7b07c8ce_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/migrations/versions/fbfe5c4702fb_soft_delete.py` & `aim-4.0.0.dev3/aim/storage/migrations/versions/fbfe5c4702fb_soft_delete.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/object.py` & `aim-4.0.0.dev3/aim/storage/object.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/prefixview.cpp` & `aim-4.0.0.dev3/aim/storage/prefixview.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.prefixview",
         "sources": [
             "aim/storage/prefixview.py"
         ]
     },
     "module_name": "aim.storage.prefixview"
```

### Comparing `aim-4.0.0.dev2/aim/storage/prefixview.pxd` & `aim-4.0.0.dev3/aim/storage/prefixview.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/prefixview.py` & `aim-4.0.0.dev3/aim/storage/prefixview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/proxy.py` & `aim-4.0.0.dev3/aim/storage/proxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/query.py` & `aim-4.0.0.dev3/aim/storage/query.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/rockscontainer.cpp` & `aim-4.0.0.dev3/aim/storage/rockscontainer.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.rockscontainer",
         "sources": [
             "aim/storage/rockscontainer.pyx"
         ]
     },
     "module_name": "aim.storage.rockscontainer"
```

### Comparing `aim-4.0.0.dev2/aim/storage/rockscontainer.pyx` & `aim-4.0.0.dev3/aim/storage/rockscontainer.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/structured/db.py` & `aim-4.0.0.dev3/aim/storage/structured/db.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/structured/entities.py` & `aim-4.0.0.dev3/aim/storage/structured/entities.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/structured/proxy.py` & `aim-4.0.0.dev3/aim/storage/structured/proxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/structured/sql_engine/entities.py` & `aim-4.0.0.dev3/aim/storage/structured/sql_engine/entities.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/structured/sql_engine/factory.py` & `aim-4.0.0.dev3/aim/storage/structured/sql_engine/factory.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/structured/sql_engine/models.py` & `aim-4.0.0.dev3/aim/storage/structured/sql_engine/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/structured/sql_engine/utils.py` & `aim-4.0.0.dev3/aim/storage/structured/sql_engine/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/treearrayview.cpp` & `aim-4.0.0.dev3/aim/storage/treearrayview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.treearrayview",
         "sources": [
             "aim/storage/treearrayview.py"
         ]
     },
     "module_name": "aim.storage.treearrayview"
```

### Comparing `aim-4.0.0.dev2/aim/storage/treearrayview.py` & `aim-4.0.0.dev3/aim/storage/treearrayview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/treeutils.cpp` & `aim-4.0.0.dev3/aim/storage/treeutils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.treeutils",
         "sources": [
             "aim/storage/treeutils.pyx"
         ]
     },
     "module_name": "aim.storage.treeutils"
```

### Comparing `aim-4.0.0.dev2/aim/storage/treeutils.pyx` & `aim-4.0.0.dev3/aim/storage/treeutils.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/treeutils_non_native.py` & `aim-4.0.0.dev3/aim/storage/treeutils_non_native.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/treeview.cpp` & `aim-4.0.0.dev3/aim/storage/treeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.treeview",
         "sources": [
             "aim/storage/treeview.py"
         ]
     },
     "module_name": "aim.storage.treeview"
```

### Comparing `aim-4.0.0.dev2/aim/storage/treeview.py` & `aim-4.0.0.dev3/aim/storage/treeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/treeviewproxy.py` & `aim-4.0.0.dev3/aim/storage/treeviewproxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/types.py` & `aim-4.0.0.dev3/aim/storage/types.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/union.cpp` & `aim-4.0.0.dev3/aim/storage/union.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.union",
         "sources": [
             "aim/storage/union.pyx"
         ]
     },
     "module_name": "aim.storage.union"
```

### Comparing `aim-4.0.0.dev2/aim/storage/union.pyx` & `aim-4.0.0.dev3/aim/storage/union.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/storage/utils.cpp` & `aim-4.0.0.dev3/aim/storage/utils.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-pa2lz81q/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.utils",
         "sources": [
             "aim/storage/utils.py"
         ]
     },
     "module_name": "aim.storage.utils"
```

### Comparing `aim-4.0.0.dev2/aim/storage/utils.py` & `aim-4.0.0.dev3/aim/storage/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/utils/deprecation.py` & `aim-4.0.0.dev3/aim/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/utils/tracking.py` & `aim-4.0.0.dev3/aim/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/__init__.py` & `aim-4.0.0.dev3/aim/web/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/dashboard_apps/models.py` & `aim-4.0.0.dev3/aim/web/api/dashboard_apps/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/dashboard_apps/pydantic_models.py` & `aim-4.0.0.dev3/aim/web/api/dashboard_apps/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/dashboard_apps/views.py` & `aim-4.0.0.dev3/aim/web/api/dashboard_apps/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/dashboards/models.py` & `aim-4.0.0.dev3/aim/web/api/dashboards/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/dashboards/pydantic_models.py` & `aim-4.0.0.dev3/aim/web/api/dashboards/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/dashboards/serializers.py` & `aim-4.0.0.dev3/aim/web/api/dashboards/serializers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/dashboards/views.py` & `aim-4.0.0.dev3/aim/web/api/dashboards/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/db.py` & `aim-4.0.0.dev3/aim/web/api/db.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/experiments/pydantic_models.py` & `aim-4.0.0.dev3/aim/web/api/experiments/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/experiments/views.py` & `aim-4.0.0.dev3/aim/web/api/experiments/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/projects/project.py` & `aim-4.0.0.dev3/aim/web/api/projects/project.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/projects/pydantic_models.py` & `aim-4.0.0.dev3/aim/web/api/projects/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/projects/views.py` & `aim-4.0.0.dev3/aim/web/api/projects/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/runs/object_api_utils.py` & `aim-4.0.0.dev3/aim/web/api/runs/object_api_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/runs/object_views.py` & `aim-4.0.0.dev3/aim/web/api/runs/object_views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/runs/pydantic_models.py` & `aim-4.0.0.dev3/aim/web/api/runs/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/runs/utils.py` & `aim-4.0.0.dev3/aim/web/api/runs/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,33 @@
     defaults = [None, None]
     slice_values = chain(range_str.strip().split(':'), defaults)
 
     start, stop, step, *_ = map(lambda x: int(x) if x else None, slice_values)
     return IndexRange(start, stop)
 
 
+def convert_nan_and_inf_to_str(tree):
+    if tree == float('inf'):
+        return 'inf'
+    if tree == float('-inf'):
+        return '-inf'
+    if tree != tree:  # x == x is False for NaN, strings break math.isnan
+        return 'NaN'
+    if isinstance(tree, dict):
+        return {
+            key: convert_nan_and_inf_to_str(value)
+            for key, value in tree.items()
+        }
+    if isinstance(tree, tuple):
+        return tuple(convert_nan_and_inf_to_str(value) for value in tree)
+    if isinstance(tree, list):
+        return [convert_nan_and_inf_to_str(value) for value in tree]
+    return tree
+
+
 def get_run_params(run: Run, *, skip_system: bool):
     params = run.get(..., {}, resolve_objects=True)
     if skip_system and '__system_params' in params:
         del params['__system_params']
     return params
```

### Comparing `aim-4.0.0.dev2/aim/web/api/runs/views.py` & `aim-4.0.0.dev3/aim/web/api/runs/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from aim.web.api.utils import APIRouter  # wrapper for fastapi.APIRouter
 from typing import Optional, Tuple
 
 from aim.sdk.types import QueryReportMode
 from aim.web.api.runs.utils import (
     checked_query,
     collect_requested_metric_traces,
+    convert_nan_and_inf_to_str,
     custom_aligned_metrics_streamer,
     get_project_repo,
     get_run_or_404,
     get_run_params,
     get_run_props,
     metric_search_result_streamer,
     run_active_result_streamer,
@@ -148,14 +149,16 @@
         sequence = repo.available_sequence_types()
 
     response = {
         'params': get_run_params(run, skip_system=skip_system),
         'traces': run.collect_sequence_info(sequence, skip_last_value=True),
         'props': get_run_props(run)
     }
+    # Convert NaN and Inf to strings
+    response = convert_nan_and_inf_to_str(response)
 
     response['props'].update({
         'notes': len(run.props.notes_obj)
     })
     return response
```

### Comparing `aim-4.0.0.dev2/aim/web/api/tags/pydantic_models.py` & `aim-4.0.0.dev3/aim/web/api/tags/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/tags/views.py` & `aim-4.0.0.dev3/aim/web/api/tags/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/utils.py` & `aim-4.0.0.dev3/aim/web/api/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/api/views.py` & `aim-4.0.0.dev3/aim/web/api/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/middlewares/profiler/profiler.py` & `aim-4.0.0.dev3/aim/web/middlewares/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/migrations/alembic.ini` & `aim-4.0.0.dev3/aim/web/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/migrations/alembic_dev.ini` & `aim-4.0.0.dev3/aim/web/migrations/alembic_dev.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/migrations/env.py` & `aim-4.0.0.dev3/aim/web/migrations/env.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/migrations/versions/11672b13f92c_.py` & `aim-4.0.0.dev3/aim/web/migrations/versions/11672b13f92c_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/migrations/versions/517a45b2e62c_.py` & `aim-4.0.0.dev3/aim/web/migrations/versions/517a45b2e62c_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/migrations/versions/5ae8371b7481_.py` & `aim-4.0.0.dev3/aim/web/migrations/versions/5ae8371b7481_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/migrations/versions/73a3d004c227_.py` & `aim-4.0.0.dev3/aim/web/migrations/versions/73a3d004c227_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim/web/utils.py` & `aim-4.0.0.dev3/aim/web/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/aim.egg-info/PKG-INFO` & `aim-4.0.0.dev3/aim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aim
-Version: 4.0.0.dev2
+Version: 4.0.0.dev3
 Summary: A super-easy way to record, search and compare AI experiments.
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,25 +20,27 @@
     <tbody>
       <tr>
         <td>Drop a star to support Aim ⭐</td>
         <td>
           <a href="https://community.aimstack.io/">Join Aim discord community</a>
           <img width="20px" src="https://user-images.githubusercontent.com/13848158/226759622-063b725d-8b3e-4c75-80c7-11fb04b7adf5.png">
         </td>
+        <td><a href="#-aim-40">🔮 Aim 4.0 - COMING SOON!!</a></td>
       </tr>
     </tbody>
   </table>
 </div>
 
 <div align="center">
   <img src="https://user-images.githubusercontent.com/13848158/225620298-9f9293e9-a138-41fd-bd77-21d53d0490b7.png">
   <h3>
-    An easy-to-use & supercharged open-source experiment tracker
+    An easy-to-use & supercharged open-source AI metadata tracker. 
   </h3>
-  Aim logs your training runs and any AI Metadata, enables a beautiful UI to compare, observe them and an API to query them programmatically.
+  
+  Aim logs all your AI metadata(**experiments**, **prompts**, etc), enables a UI to compare & observe them and SDK to query them programmatically.
 </div>
 
 <br/>
 
 <div align="center">
   
   [![Discord Server](https://dcbadge.vercel.app/api/server/zXq2NfVdtF?compact=true&style=flat)](https://community.aimstack.io/)
@@ -114,24 +116,26 @@
   <a href="#-about"><b>About</b></a> &bull;
   <a href="#-demos"><b>Demos</b></a> &bull;
   <a href="#-ecosystem"><b>Ecosystem</b></a> &bull;
   <a href="#-quick-start"><b>Quick Start</b></a> &bull;
   <a href="https://github.com/aimhubio/aim/tree/main/examples"><b>Examples</b></a> &bull;
   <a href="https://aimstack.readthedocs.io/en/latest/"><b>Documentation</b></a> &bull;
   <a href="#-community"><b>Community</b></a> &bull;
-  <a href="https://aimstack.io/blog"><b>Blog</b></a>
+  <a href="https://aimstack.io/blog"><b>Blog</b></a> &bull;
+  <a href="#-aim-40"><b>COMING SOON!!</b></a>
 </h3>  
 
 ---
 
 # ℹ️ About
 
-Aim is an open-source, self-hosted ML experiment tracking tool designed to handle 10,000s of training runs.
+Aim is an open-source, self-hosted AI Metadata tracking tool designed to handle 100,000s of tracked metadata sequences.
+Two most famous AI metadata applications are: experiment tracking and prompt engineering.
 
-Aim provides a performant and beautiful UI for exploring and comparing training runs.
+Aim provides a performant and beautiful UI for exploring and comparing training runs, prompt sessions.
 Additionally, its SDK enables programmatic access to tracked metadata — perfect for automations and Jupyter Notebook analysis.
 
 <p align="center">
   <strong>Aim's mission is to democratize AI dev tools 🎯 </strong>
 </p>
 
 <div align="center">
@@ -184,14 +188,28 @@
             <li>Runs grouping with tags and experiments</li></ul>
         </td>
       </tr>
     </tbody>
   </table>
 </div>
 
+# 🔮 Aim 4.0
+**Aim 4.0 is coming soon!!**
+
+A major iteration of Aim as the ultimate metadata library to track all your interactions with your models - including experiments, prompts etc.
+
+- Remote first
+- Scalable 
+- Capable of storing and querying 100,000s of metadata sequences
+- Custom UI dashboards and reports
+
+The Aim experiment tracker is not just one-off experiment tracker.
+It's built on top of the metadata library that Aim is. Now you can also do prompt engineering on Aim.
+Stay tuned for more...
+
 # 🎬 Demos
 
 Check out live Aim demos NOW to see it in action.
 
 | [Machine translation experiments](http://play.aimstack.io:10001/metrics?grouping=HQGdK9Xxy35e6sY1CYkCmk1WbWMN2AsCNfJJ3d1RJYLtrVPMoF5UpGiA6CF8bEJnfzRsKpqespf3AEuKSVrhUYvYk9MxzNGA9XZWYUf6phEg8AMbZGLRVDXnAPDuo8tueqsST1ZLizWzQwDYJWHUza6pyB2Eojt9uWqNHUdb858TqDRnCJzqiVJXKXEzFWUyvU8MckJo1qpqWWCTb4GpYN6DUJZx2GXDGR21e2xxd4m7PmNUnbA9B3apLttZoipJF6c3v7tNUKmb6irpqnNB3yc57tqYDa1XZuKfDxkMtyFdQ1x95K4jjsTVwhftEWLze35QNcxNXRCGGS9o9yEfTLG26GUX2zjPZFCjjMGU6vV7z1xRccK8MyoGrLSgAQCbvk68dTGBHpXUBvCRq8N&chart=FviZzVrt4fVQPjpCLr9sVGGrcR5etSroyqambiKpm3nTgpyv4eQxKuwNX9uN8UtKmzYUhUyTMBEANHmtbwjLApkvnYeNbxGNC6PVcoqi65m1XJnSrvgt8WiD89BapFAWRUwAGx6SWD7KZPsk3RQyysU7W7FjD3Q99NusxFGhsEfD6HXc7i8xH9KHDRGjLwh6x9VTtSp4FS8HEvpLSiiJoX7LCTi8pB7dXvrQ8G5w3jPsFz4qXYFdsVaCNL1BpFFZuiqQNkfbnM84gEq7UmiV1VzM4oS3AgQHxADG3kpBVp6eKTey9F1Swd4FcUkFA9QEPjgQgqwRGjkquZ2bdDDVLBnCh7JPvboP2kifCiZZ5MDdV9MMx6PKHp4DusWyWLXiHQYPkpGPWBiuccMUXDsuJaCWJbuABdY7CyiJMv1jdHYkjabygSxehPVyEDefWAtjBfv2vaeM1xv63jadbmpKYFxft7qmuT9HvVxiGvRgs4RQFxy8K4rtFBca3HNs1mDaaY81gy9MGXyw7BS5Fniu92jaJpsWDdg6Y3AQBLZtrpJy2obEZ4yzJaCVT7JUNPAyyCUNLck393VFLoEkaD9CU5npK5R7tj1c1G3gkMNQXnSXy5NpSj8deMmXV5qz3JKu1nq2caGQKcqjzy2gLkExdm674AMFjSg9yFjK6VqASXQ17NKtWRUvaYoxGbHDAFQaMKWKh8QLm22QA9mKT8NksLptWozbgDvafnQLNMvezLU5bvKV5o75PAWYiRB56RcYfEhzaB6YWdgL7TJicyY5rFi6Az8UZ7wqB3N5iMuZdpxhKn5KbZDxyuUMuvVt24i5LVPPmmwQtqxMoJ4aLo48a2YvDW6TAkdQjNjvn6KcEEz6GTixujb1YHhMUD8v4AepWKEwKz1ddEca1P2wLQjbpihCuaqbxeohnuZZLogJdUBojBEDgrnrrVpPBaLLEkGSpkJbtrsKUuEeBo1AF3yNgHftLbynGpobVF5DhmsmddmiA6c8vSTokJxHhjpnW8mAcNHBRtmVJCT7VkdHSAhNypM4Hivwfx5jCccG9LauKmCeRMDzHiA57TX9W6ttcPHSvUyQorARQAd2oeNY4H83hZjHh9Bt8iwKZRt4xK6hrTR8tif7hq8eURXrGH9Ys7TzykXK8FHHWvLNzNnYf3E4a9NkD43MjfKvMM1hj4Q2K8MHbmRCqrmFrHP5kim9shq6mhLPTgwha32nvnrBkfPQVPwpGTzKuwE&select=CdsQ7jVNkogQhRzQR3e28Ek39AZ4Ma2y37k5zJaf9EZmQhMjy8GtGm4LGU6dRFuAVG7mYww5xDrQAE74KHQ3Kk1e6661RmcmNALAUjtHyCmrTVBMCnBGNiuq1y7EzmxoodYHU1BV1rnoefQAw2kTBtbWi11hV1P4LcwFCcXfUWF6rpRC7ehEnUCTqUV4bkGVJPLcmk9mdmiGwa2YgmnSShNGPVGZiEi1rMVECyngSRVdqdZwAeXBGWFLfqF1KbZeCo4MTF4SSmFupJ9zLhYbuojEbopyFWHQ6xs3sq9epPeaQziLM4Js7oFYRmuFWUYdFqnZngmewXWmi7tQAgVqhiT6dMjG2eTdfgX6WuRSuoHALkh2XJhHA6GfZLUcxC5Ni9YyKuBTamtaYarbNNJJ8z15WWvuUkLpjgHdEpE2h924xFdu8aoZNuiQxYGvcndaW1BTGMXS5fTKPqYfe2n8Ky2HWPkcX3hEXtyawu1F9BndKNaXLPgsdAoFBArBZnSe28YtSmTa5LRucKVBAxakvv5MWMXchAmpaGFQbZyYUoMgQLcJd7Y96x6zSR7nhwr5Ar81BrmqYz2WFLuk7osUbwsc9HbSG6CQt8p6Vg2u7DjKaZXW8pjkPHAKrHWtHEDiJPJ5rj6VsdFm3) | [lightweight-GAN experiments](http://play.aimstack.io:10002/images?grouping=E1zQzcmtDR3wibEa1MVysTvCyZEv1T8ixkCxTWExCyMnHtX2HyiF9eszvPgfd2xdJ5TUTKGpSs1bsLVq5tHAV3uWtsZmmckn6HjNtVCMyQDJpwhiEy5tAyw&select=2NEXuD7fFoaLcwRjymjA1wLmUrGs9s3AiXcCW82C367SwJt18CAB6xzkMGowrUDuDwggE1huaPVcQJpQUsmAQx1CnGiqCUBp2jPMd5mMNPX2QKQMcmvu9ZykBNkeBvCQFPd9ERuQD2g1EjWuvyJ3H53mAZTfp94LCXvR9CUsG5ei2CjQUzfZLM6DCyUr1GPaEVnY5f1EwzicNxXuoutkBgqCqaobJ7Do4q4eHAA6ooiWU6ekS3D2sLj6qYwhVTjfGCPfbWwBiH83nFkY3fLExzdeTY2zeUHeeYikQR9S7xHbVD8WvjekdQVp8X4dNLJZxiVmEqHpPRnU3ZrYsMhE7yFAAgjJwPNUzLTt6YFrtZBcmc4rwAC2oyrqysUSEr6gzL6LcJ6yuqDGf9D5tzftHbTLDkhc8B2sCgTS&images=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)|
 |:---:|:---:|
 | <a href="http://play.aimstack.io:10001/metrics?grouping=HQGdK9Xxy35e6sY1CYkCmk1WbWMN2AsCNfJJ3d1RJYLtrVPMoF5UpGiA6CF8bEJnfzRsKpqespf3AEuKSVrhUYvYk9MxzNGA9XZWYUf6phEg8AMbZGLRVDXnAPDuo8tueqsST1ZLizWzQwDYJWHUza6pyB2Eojt9uWqNHUdb858TqDRnCJzqiVJXKXEzFWUyvU8MckJo1qpqWWCTb4GpYN6DUJZx2GXDGR21e2xxd4m7PmNUnbA9B3apLttZoipJF6c3v7tNUKmb6irpqnNB3yc57tqYDa1XZuKfDxkMtyFdQ1x95K4jjsTVwhftEWLze35QNcxNXRCGGS9o9yEfTLG26GUX2zjPZFCjjMGU6vV7z1xRccK8MyoGrLSgAQCbvk68dTGBHpXUBvCRq8N&chart=FviZzVrt4fVQPjpCLr9sVGGrcR5etSroyqambiKpm3nTgpyv4eQxKuwNX9uN8UtKmzYUhUyTMBEANHmtbwjLApkvnYeNbxGNC6PVcoqi65m1XJnSrvgt8WiD89BapFAWRUwAGx6SWD7KZPsk3RQyysU7W7FjD3Q99NusxFGhsEfD6HXc7i8xH9KHDRGjLwh6x9VTtSp4FS8HEvpLSiiJoX7LCTi8pB7dXvrQ8G5w3jPsFz4qXYFdsVaCNL1BpFFZuiqQNkfbnM84gEq7UmiV1VzM4oS3AgQHxADG3kpBVp6eKTey9F1Swd4FcUkFA9QEPjgQgqwRGjkquZ2bdDDVLBnCh7JPvboP2kifCiZZ5MDdV9MMx6PKHp4DusWyWLXiHQYPkpGPWBiuccMUXDsuJaCWJbuABdY7CyiJMv1jdHYkjabygSxehPVyEDefWAtjBfv2vaeM1xv63jadbmpKYFxft7qmuT9HvVxiGvRgs4RQFxy8K4rtFBca3HNs1mDaaY81gy9MGXyw7BS5Fniu92jaJpsWDdg6Y3AQBLZtrpJy2obEZ4yzJaCVT7JUNPAyyCUNLck393VFLoEkaD9CU5npK5R7tj1c1G3gkMNQXnSXy5NpSj8deMmXV5qz3JKu1nq2caGQKcqjzy2gLkExdm674AMFjSg9yFjK6VqASXQ17NKtWRUvaYoxGbHDAFQaMKWKh8QLm22QA9mKT8NksLptWozbgDvafnQLNMvezLU5bvKV5o75PAWYiRB56RcYfEhzaB6YWdgL7TJicyY5rFi6Az8UZ7wqB3N5iMuZdpxhKn5KbZDxyuUMuvVt24i5LVPPmmwQtqxMoJ4aLo48a2YvDW6TAkdQjNjvn6KcEEz6GTixujb1YHhMUD8v4AepWKEwKz1ddEca1P2wLQjbpihCuaqbxeohnuZZLogJdUBojBEDgrnrrVpPBaLLEkGSpkJbtrsKUuEeBo1AF3yNgHftLbynGpobVF5DhmsmddmiA6c8vSTokJxHhjpnW8mAcNHBRtmVJCT7VkdHSAhNypM4Hivwfx5jCccG9LauKmCeRMDzHiA57TX9W6ttcPHSvUyQorARQAd2oeNY4H83hZjHh9Bt8iwKZRt4xK6hrTR8tif7hq8eURXrGH9Ys7TzykXK8FHHWvLNzNnYf3E4a9NkD43MjfKvMM1hj4Q2K8MHbmRCqrmFrHP5kim9shq6mhLPTgwha32nvnrBkfPQVPwpGTzKuwE&select=CdsQ7jVNkogQhRzQR3e28Ek39AZ4Ma2y37k5zJaf9EZmQhMjy8GtGm4LGU6dRFuAVG7mYww5xDrQAE74KHQ3Kk1e6661RmcmNALAUjtHyCmrTVBMCnBGNiuq1y7EzmxoodYHU1BV1rnoefQAw2kTBtbWi11hV1P4LcwFCcXfUWF6rpRC7ehEnUCTqUV4bkGVJPLcmk9mdmiGwa2YgmnSShNGPVGZiEi1rMVECyngSRVdqdZwAeXBGWFLfqF1KbZeCo4MTF4SSmFupJ9zLhYbuojEbopyFWHQ6xs3sq9epPeaQziLM4Js7oFYRmuFWUYdFqnZngmewXWmi7tQAgVqhiT6dMjG2eTdfgX6WuRSuoHALkh2XJhHA6GfZLUcxC5Ni9YyKuBTamtaYarbNNJJ8z15WWvuUkLpjgHdEpE2h924xFdu8aoZNuiQxYGvcndaW1BTGMXS5fTKPqYfe2n8Ky2HWPkcX3hEXtyawu1F9BndKNaXLPgsdAoFBArBZnSe28YtSmTa5LRucKVBAxakvv5MWMXchAmpaGFQbZyYUoMgQLcJd7Y96x6zSR7nhwr5Ar81BrmqYz2WFLuk7osUbwsc9HbSG6CQt8p6Vg2u7DjKaZXW8pjkPHAKrHWtHEDiJPJ5rj6VsdFm3"> <img src="https://user-images.githubusercontent.com/97726819/225964524-0051c2c7-8554-43ae-82b8-adcb77bcf1ba.png"> </a> | <a href="http://play.aimstack.io:10002/images?grouping=E1zQzcmtDR3wibEa1MVysTvCyZEv1T8ixkCxTWExCyMnHtX2HyiF9eszvPgfd2xdJ5TUTKGpSs1bsLVq5tHAV3uWtsZmmckn6HjNtVCMyQDJpwhiEy5tAyw&select=2NEXuD7fFoaLcwRjymjA1wLmUrGs9s3AiXcCW82C367SwJt18CAB6xzkMGowrUDuDwggE1huaPVcQJpQUsmAQx1CnGiqCUBp2jPMd5mMNPX2QKQMcmvu9ZykBNkeBvCQFPd9ERuQD2g1EjWuvyJ3H53mAZTfp94LCXvR9CUsG5ei2CjQUzfZLM6DCyUr1GPaEVnY5f1EwzicNxXuoutkBgqCqaobJ7Do4q4eHAA6ooiWU6ekS3D2sLj6qYwhVTjfGCPfbWwBiH83nFkY3fLExzdeTY2zeUHeeYikQR9S7xHbVD8WvjekdQVp8X4dNLJZxiVmEqHpPRnU3ZrYsMhE7yFAAgjJwPNUzLTt6YFrtZBcmc4rwAC2oyrqysUSEr6gzL6LcJ6yuqDGf9D5tzftHbTLDkhc8B2sCgTS&images=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"> <img src="https://user-images.githubusercontent.com/97726819/225948275-a41946ea-89f4-45f1-bce1-251c84dcddca.png"> </a> |
```

#### html2text {}

```diff
@@ -1,24 +1,27 @@
-Metadata-Version: 2.1 Name: aim Version: 4.0.0.dev2 Summary: A super-easy way
+Metadata-Version: 2.1 Name: aim Version: 4.0.0.dev3 Summary: A super-easy way
 to record, search and compare AI experiments. Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
 Python: >=3.7.0 Description-Content-Type: text/markdown License-File: LICENSE
-                               Join_Aim_discord_community [https://user-
-Drop a star to support Aim â­images.githubusercontent.com/13848158/226759622-
-                               063b725d-8b3e-4c75-80c7-11fb04b7adf5.png]
+                       Join_Aim_discord_community
+                       [https://user-
+Drop a star to support images.githubusercontent.com/ ð®_Aim_4.0_-_COMING
+Aim â­             13848158/226759622-063b725d-  SOON!!
+                       8b3e-4c75-80c7-
+                       11fb04b7adf5.png]
  [https://user-images.githubusercontent.com/13848158/225620298-9f9293e9-a138-
                           41fd-bd77-21d53d0490b7.png]
-    **** An easy-to-use & supercharged open-source experiment tracker ****
-  Aim logs your training runs and any AI Metadata, enables a beautiful UI to
-       compare, observe them and an API to query them programmatically.
+   **** An easy-to-use & supercharged open-source AI metadata tracker. ****
+Aim logs all your AI metadata(**experiments**, **prompts**, etc), enables a UI
+       to compare & observe them and SDK to query them programmatically.
 
            [![Discord Server](https://dcbadge.vercel.app/api/server/
 zXq2NfVdtF?compact=true&style=flat)](https://community.aimstack.io/) [![Twitter
 Follow](https://img.shields.io/twitter/follow/aimstackio?style=social)](https:/
    /twitter.com/aimstackio) [![Medium](https://img.shields.io/badge/Medium-
 12100E?style=flat&logo=medium&logoColor=white)](https://medium.com/aimstack) [!
  [Platform Support](https://img.shields.io/badge/platform-Linux%20%7C%20macOS-
@@ -77,20 +80,21 @@
     bf1bc685477b.png] [https://user-images.githubusercontent.com/97726819/
               225953432-4b27653a-aa12-4fbf-897c-01349afa2ad0.png]
 
     AimStack offers enterprise support that's beyond core Aim. Contact via
                            hello@aimstack.io e-mail.
 ---
    **** About • Demos • Ecosystem • Quick_Start • Examples • Documentation •
-                             Community • Blog ****
---- # â¹ï¸ About Aim is an open-source, self-hosted ML experiment tracking
-tool designed to handle 10,000s of training runs. Aim provides a performant and
-beautiful UI for exploring and comparing training runs. Additionally, its SDK
-enables programmatic access to tracked metadata â perfect for automations and
-Jupyter Notebook analysis.
+                     Community • Blog • COMING_SOON!! ****
+--- # â¹ï¸ About Aim is an open-source, self-hosted AI Metadata tracking tool
+designed to handle 100,000s of tracked metadata sequences. Two most famous AI
+metadata applications are: experiment tracking and prompt engineering. Aim
+provides a performant and beautiful UI for exploring and comparing training
+runs, prompt sessions. Additionally, its SDK enables programmatic access to
+tracked metadata â perfect for automations and Jupyter Notebook analysis.
                Aim's mission is to democratize AI dev tools ð¯
  [https://user-images.githubusercontent.com/13848158/226426018-f7c11c9b-78d9-
     4ee4-b292-df28b3e8eaa6.jpg] [https://user-images.githubusercontent.com/
   13848158/226426005-f7e83923-0f92-44a4-88e4-1735a3d3e119.jpg] [https://user-
    images.githubusercontent.com/13848158/226426015-4f1122d8-c96a-443f-8698-
                                3db942b1972a.jpg]
 Log Metadata Across Your ML Pipeline  Visualize & Compare Metadata via UI ð
@@ -104,16 +108,23 @@
 Run ML Trainings Effectively â¡   Organize Your Experiments ðï¸
     * System info and resource usage      * Detailed run information for easy
       tracking                              debugging
     * Real-time alerting on training      * Centralized dashboard for holistic
       progress                              view
     * Logging and configurable            * Runs grouping with tags and
       notifications                         experiments
-# ð¬ Demos Check out live Aim demos NOW to see it in action. | [Machine
-translation experiments](http://play.aimstack.io:10001/
+# ð® Aim 4.0 **Aim 4.0 is coming soon!!** A major iteration of Aim as the
+ultimate metadata library to track all your interactions with your models -
+including experiments, prompts etc. - Remote first - Scalable - Capable of
+storing and querying 100,000s of metadata sequences - Custom UI dashboards and
+reports The Aim experiment tracker is not just one-off experiment tracker. It's
+built on top of the metadata library that Aim is. Now you can also do prompt
+engineering on Aim. Stay tuned for more... # ð¬ Demos Check out live Aim
+demos NOW to see it in action. | [Machine translation experiments](http://
+play.aimstack.io:10001/
 metrics?grouping=HQGdK9Xxy35e6sY1CYkCmk1WbWMN2AsCNfJJ3d1RJYLtrVPMoF5UpGiA6CF8bEJnfzRsKpqespf3AEuKSVrhUYvYk9MxzNGA9XZWYUf6phEg8AMbZGLRVDXnAPDuo8tueqsST1ZLizWzQwDYJWHUza6pyB2Eojt9uWqNHUdb858TqDRnCJzqiVJXKXEzFWUyvU8MckJo1qpqWWCTb4GpYN6DUJZx2GXDGR21e2xxd4m7PmNUnbA9B3apLttZoipJF6c3v7tNUKmb6irpqnNB3yc57tqYDa1XZuKfDxkMtyFdQ1x95K4jjsTVwhftEWLze35QNcxNXRCGGS9o9yEfTLG26GUX2zjPZFCjjMGU6vV7z1xRccK8MyoGrLSgAQCbvk68dTGBHpXUBvCRq8N&chart=FviZzVrt4fVQPjpCLr9sVGGrcR5etSroyqambiKpm3nTgpyv4eQxKuwNX9uN8UtKmzYUhUyTMBEANHmtbwjLApkvnYeNbxGNC6PVcoqi65m1XJnSrvgt8WiD89BapFAWRUwAGx6SWD7KZPsk3RQyysU7W7FjD3Q99NusxFGhsEfD6HXc7i8xH9KHDRGjLwh6x9VTtSp4FS8HEvpLSiiJoX7LCTi8pB7dXvrQ8G5w3jPsFz4qXYFdsVaCNL1BpFFZuiqQNkfbnM84gEq7UmiV1VzM4oS3AgQHxADG3kpBVp6eKTey9F1Swd4FcUkFA9QEPjgQgqwRGjkquZ2bdDDVLBnCh7JPvboP2kifCiZZ5MDdV9MMx6PKHp4DusWyWLXiHQYPkpGPWBiuccMUXDsuJaCWJbuABdY7CyiJMv1jdHYkjabygSxehPVyEDefWAtjBfv2vaeM1xv63jadbmpKYFxft7qmuT9HvVxiGvRgs4RQFxy8K4rtFBca3HNs1mDaaY81gy9MGXyw7BS5Fniu92jaJpsWDdg6Y3AQBLZtrpJy2obEZ4yzJaCVT7JUNPAyyCUNLck393VFLoEkaD9CU5npK5R7tj1c1G3gkMNQXnSXy5NpSj8deMmXV5qz3JKu1nq2caGQKcqjzy2gLkExdm674AMFjSg9yFjK6VqASXQ17NKtWRUvaYoxGbHDAFQaMKWKh8QLm22QA9mKT8NksLptWozbgDvafnQLNMvezLU5bvKV5o75PAWYiRB56RcYfEhzaB6YWdgL7TJicyY5rFi6Az8UZ7wqB3N5iMuZdpxhKn5KbZDxyuUMuvVt24i5LVPPmmwQtqxMoJ4aLo48a2YvDW6TAkdQjNjvn6KcEEz6GTixujb1YHhMUD8v4AepWKEwKz1ddEca1P2wLQjbpihCuaqbxeohnuZZLogJdUBojBEDgrnrrVpPBaLLEkGSpkJbtrsKUuEeBo1AF3yNgHftLbynGpobVF5DhmsmddmiA6c8vSTokJxHhjpnW8mAcNHBRtmVJCT7VkdHSAhNypM4Hivwfx5jCccG9LauKmCeRMDzHiA57TX9W6ttcPHSvUyQorARQAd2oeNY4H83hZjHh9Bt8iwKZRt4xK6hrTR8tif7hq8eURXrGH9Ys7TzykXK8FHHWvLNzNnYf3E4a9NkD43MjfKvMM1hj4Q2K8MHbmRCqrmFrHP5kim9shq6mhLPTgwha32nvnrBkfPQVPwpGTzKuwE&select=CdsQ7jVNkogQhRzQR3e28Ek39AZ4Ma2y37k5zJaf9EZmQhMjy8GtGm4LGU6dRFuAVG7mYww5xDrQAE74KHQ3Kk1e6661RmcmNALAUjtHyCmrTVBMCnBGNiuq1y7EzmxoodYHU1BV1rnoefQAw2kTBtbWi11hV1P4LcwFCcXfUWF6rpRC7ehEnUCTqUV4bkGVJPLcmk9mdmiGwa2YgmnSShNGPVGZiEi1rMVECyngSRVdqdZwAeXBGWFLfqF1KbZeCo4MTF4SSmFupJ9zLhYbuojEbopyFWHQ6xs3sq9epPeaQziLM4Js7oFYRmuFWUYdFqnZngmewXWmi7tQAgVqhiT6dMjG2eTdfgX6WuRSuoHALkh2XJhHA6GfZLUcxC5Ni9YyKuBTamtaYarbNNJJ8z15WWvuUkLpjgHdEpE2h924xFdu8aoZNuiQxYGvcndaW1BTGMXS5fTKPqYfe2n8Ky2HWPkcX3hEXtyawu1F9BndKNaXLPgsdAoFBArBZnSe28YtSmTa5LRucKVBAxakvv5MWMXchAmpaGFQbZyYUoMgQLcJd7Y96x6zSR7nhwr5Ar81BrmqYz2WFLuk7osUbwsc9HbSG6CQt8p6Vg2u7DjKaZXW8pjkPHAKrHWtHEDiJPJ5rj6VsdFm3)
 | [lightweight-GAN experiments](http://play.aimstack.io:10002/
 images?grouping=E1zQzcmtDR3wibEa1MVysTvCyZEv1T8ixkCxTWExCyMnHtX2HyiF9eszvPgfd2xdJ5TUTKGpSs1bsLVq5tHAV3uWtsZmmckn6HjNtVCMyQDJpwhiEy5tAyw&select=2NEXuD7fFoaLcwRjymjA1wLmUrGs9s3AiXcCW82C367SwJt18CAB6xzkMGowrUDuDwggE1huaPVcQJpQUsmAQx1CnGiqCUBp2jPMd5mMNPX2QKQMcmvu9ZykBNkeBvCQFPd9ERuQD2g1EjWuvyJ3H53mAZTfp94LCXvR9CUsG5ei2CjQUzfZLM6DCyUr1GPaEVnY5f1EwzicNxXuoutkBgqCqaobJ7Do4q4eHAA6ooiWU6ekS3D2sLj6qYwhVTjfGCPfbWwBiH83nFkY3fLExzdeTY2zeUHeeYikQR9S7xHbVD8WvjekdQVp8X4dNLJZxiVmEqHpPRnU3ZrYsMhE7yFAAgjJwPNUzLTt6YFrtZBcmc4rwAC2oyrqysUSEr6gzL6LcJ6yuqDGf9D5tzftHbTLDkhc8B2sCgTS&images=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)|
 |:---:|:---:| | [https://user-images.githubusercontent.com/97726819/225964524-
 0051c2c7-8554-43ae-82b8-adcb77bcf1ba.png] | [https://user-
 images.githubusercontent.com/97726819/225948275-a41946ea-89f4-45f1-bce1-
 251c84dcddca.png] | | Training logs of a neural translation model(from WMT'19
```

### Comparing `aim-4.0.0.dev2/aim.egg-info/SOURCES.txt` & `aim-4.0.0.dev3/aim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/performance_tests/sdk/test_data_collection.py` & `aim-4.0.0.dev3/performance_tests/sdk/test_data_collection.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/performance_tests/sdk/test_query.py` & `aim-4.0.0.dev3/performance_tests/sdk/test_query.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/performance_tests/sdk/utils.py` & `aim-4.0.0.dev3/performance_tests/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/performance_tests/storage/test_container_open.py` & `aim-4.0.0.dev3/performance_tests/storage/test_container_open.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/performance_tests/storage/test_iterative_access.py` & `aim-4.0.0.dev3/performance_tests/storage/test_iterative_access.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/performance_tests/storage/test_random_access.py` & `aim-4.0.0.dev3/performance_tests/storage/test_random_access.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/performance_tests/storage/utils.py` & `aim-4.0.0.dev3/performance_tests/storage/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/setup.py` & `aim-4.0.0.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/api/test_dashboards_api.py` & `aim-4.0.0.dev3/tests/api/test_dashboards_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/api/test_project_api.py` & `aim-4.0.0.dev3/tests/api/test_project_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/api/test_run_api.py` & `aim-4.0.0.dev3/tests/api/test_run_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/api/test_run_images_api.py` & `aim-4.0.0.dev3/tests/api/test_run_images_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/api/test_structured_data_api.py` & `aim-4.0.0.dev3/tests/api/test_structured_data_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/integrations/test_dvc_metadata.py` & `aim-4.0.0.dev3/tests/integrations/test_dvc_metadata.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/integrations/test_hf_datasets.py` & `aim-4.0.0.dev3/tests/integrations/test_hf_datasets.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/integrations/test_hub_dataset.py` & `aim-4.0.0.dev3/tests/integrations/test_hub_dataset.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/sdk/test_image_construction.py` & `aim-4.0.0.dev3/tests/sdk/test_image_construction.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/sdk/test_resource_tracker.py` & `aim-4.0.0.dev3/tests/sdk/test_resource_tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/sdk/test_run_apis.py` & `aim-4.0.0.dev3/tests/sdk/test_run_apis.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/sdk/test_run_creation_checks.py` & `aim-4.0.0.dev3/tests/sdk/test_run_creation_checks.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/sdk/test_run_finalization_time.py` & `aim-4.0.0.dev3/tests/sdk/test_run_finalization_time.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/sdk/test_run_metric_types.py` & `aim-4.0.0.dev3/tests/sdk/test_run_metric_types.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/sdk/test_run_track_type_checking.py` & `aim-4.0.0.dev3/tests/sdk/test_run_track_type_checking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/sdk/test_run_write_container_data.py` & `aim-4.0.0.dev3/tests/sdk/test_run_write_container_data.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/sdk/test_utils.py` & `aim-4.0.0.dev3/tests/sdk/test_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/storage/test_query.py` & `aim-4.0.0.dev3/tests/storage/test_query.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/storage/test_query_with_epoch_none.py` & `aim-4.0.0.dev3/tests/storage/test_query_with_epoch_none.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev2/tests/storage/test_structured_db.py` & `aim-4.0.0.dev3/tests/storage/test_structured_db.py`

 * *Files identical despite different names*

