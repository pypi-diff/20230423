# Comparing `tmp/django-common-task-system-1.2.2.tar.gz` & `tmp/django-common-task-system-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-task-system-1.2.2.tar", last modified: Fri Apr 21 09:44:39 2023, max compression
+gzip compressed data, was "django-common-task-system-1.2.3.tar", last modified: Sun Apr 23 03:20:20 2023, max compression
```

## Comparing `django-common-task-system-1.2.2.tar` & `django-common-task-system-1.2.3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.822747 django-common-task-system-1.2.2/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.2.2/LICENSE
--rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      303 2023-04-21 09:44:39.821268 django-common-task-system-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.759484 django-common-task-system-1.2.2/django_common_task_system/
--rw-rw-rw-   0        0        0     3014 2023-04-17 02:45:20.000000 django-common-task-system-1.2.2/django_common_task_system/__init__.py
--rw-rw-rw-   0        0        0    11370 2023-04-21 09:44:38.000000 django-common-task-system-1.2.2/django_common_task_system/admin.py
--rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.2.2/django_common_task_system/apps.py
--rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.2.2/django_common_task_system/choices.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.2.2/django_common_task_system/fields.py
--rw-rw-rw-   0        0        0    15985 2023-04-21 09:40:54.000000 django-common-task-system-1.2.2/django_common_task_system/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.775060 django-common-task-system-1.2.2/django_common_task_system/migrations/
--rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.2.2/django_common_task_system/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.2.2/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
--rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.2.2/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
--rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.2.2/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.2.2/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.2.2/django_common_task_system/migrations/0006_consumerpermission.py
--rw-rw-rw-   0        0        0     1275 2023-04-21 07:23:00.000000 django-common-task-system-1.2.2/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.2.2/django_common_task_system/migrations/__init__.py
--rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.2.2/django_common_task_system/mixin.py
--rw-rw-rw-   0        0        0    36588 2023-04-21 07:09:25.000000 django-common-task-system-1.2.2/django_common_task_system/models.py
--rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.2.2/django_common_task_system/permissions.py
--rw-rw-rw-   0        0        0     2272 2023-04-21 08:20:32.000000 django-common-task-system-1.2.2/django_common_task_system/serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.738982 django-common-task-system-1.2.2/django_common_task_system/static/
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.738982 django-common-task-system-1.2.2/django_common_task_system/static/common_task_system/
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.777491 django-common-task-system-1.2.2/django_common_task_system/static/common_task_system/css/
--rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.2.2/django_common_task_system/static/common_task_system/css/calendar.css
--rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.2.2/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.778491 django-common-task-system-1.2.2/django_common_task_system/static/common_task_system/js/
--rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.2.2/django_common_task_system/static/common_task_system/js/calendar.js
--rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.2.2/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.790686 django-common-task-system-1.2.2/django_common_task_system/system_task/
--rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/__init__.py
--rw-rw-rw-   0        0        0     5166 2023-04-21 07:14:23.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/admin.py
--rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/apps.py
--rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/choices.py
--rw-rw-rw-   0        0        0     4130 2023-04-19 09:42:02.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.798927 django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/
--rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
--rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
--rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
--rw-rw-rw-   0        0        0     1062 2023-04-21 07:23:00.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/__init__.py
--rw-rw-rw-   0        0        0    14945 2023-04-21 07:09:25.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/models.py
--rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/process.py
--rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/queue.py
--rw-rw-rw-   0        0        0     1679 2023-04-21 07:11:39.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/serializers.py
--rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/tests.py
--rw-rw-rw-   0        0        0      846 2023-04-21 07:22:44.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/urls.py
--rw-rw-rw-   0        0        0     5505 2023-04-21 07:22:44.000000 django-common-task-system-1.2.2/django_common_task_system/system_task/views.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.800131 django-common-task-system-1.2.2/django_common_task_system/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.2.2/django_common_task_system/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     1674 2023-04-19 09:54:46.000000 django-common-task-system-1.2.2/django_common_task_system/system_task_execution/main.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.803364 django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     3100 2023-04-21 07:40:43.000000 django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/executor.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.808092 django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/executors/
--rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
--rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
--rw-rw-rw-   0        0        0     3500 2023-04-17 05:43:02.000000 django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
--rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
--rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
--rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.742347 django-common-task-system-1.2.2/django_common_task_system/templates/
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.742347 django-common-task-system-1.2.2/django_common_task_system/templates/admin/
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.809101 django-common-task-system-1.2.2/django_common_task_system/templates/admin/system_schedule/
--rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.2.2/django_common_task_system/templates/admin/system_schedule/change_list.html
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.815799 django-common-task-system-1.2.2/django_common_task_system/templates/task_schedule/
--rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.2.2/django_common_task_system/templates/task_schedule/datetime_range.html
--rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.2.2/django_common_task_system/templates/task_schedule/multi_day_select.html
--rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.2.2/django_common_task_system/templates/task_schedule/multi_month_day_select.html
--rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.2.2/django_common_task_system/templates/task_schedule/nlp_input.html
--rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.2.2/django_common_task_system/templates/task_schedule/period.html
--rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.2.2/django_common_task_system/templates/task_schedule/period_schedule.html
--rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.2.2/django_common_task_system/tests.py
--rw-rw-rw-   0        0        0     1060 2023-04-21 07:22:44.000000 django-common-task-system-1.2.2/django_common_task_system/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.818866 django-common-task-system-1.2.2/django_common_task_system/utils/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.2.2/django_common_task_system/utils/__init__.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.2.2/django_common_task_system/utils/algorithm.py
--rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.2.2/django_common_task_system/utils/cron_utils.py
--rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.2.2/django_common_task_system/utils/foreign_key.py
--rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.2.2/django_common_task_system/utils/schedule_time.py
--rw-rw-rw-   0        0        0    11510 2023-04-21 08:19:22.000000 django-common-task-system-1.2.2/django_common_task_system/views.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.767132 django-common-task-system-1.2.2/django_common_task_system.egg-info/
--rw-rw-rw-   0        0        0      303 2023-04-21 09:44:39.000000 django-common-task-system-1.2.2/django_common_task_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4423 2023-04-21 09:44:39.000000 django-common-task-system-1.2.2/django_common_task_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 09:44:39.000000 django-common-task-system-1.2.2/django_common_task_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-04-21 09:44:39.000000 django-common-task-system-1.2.2/django_common_task_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-04-21 09:44:39.000000 django-common-task-system-1.2.2/django_common_task_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 09:44:39.822747 django-common-task-system-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-04-21 09:42:25.000000 django-common-task-system-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:44:39.820236 django-common-task-system-1.2.2/tests/
--rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.2.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.083304 django-common-task-system-1.2.3/
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      303 2023-04-23 03:20:20.083304 django-common-task-system-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.037069 django-common-task-system-1.2.3/django_common_task_system/
+-rw-rw-rw-   0        0        0     3014 2023-04-17 02:45:20.000000 django-common-task-system-1.2.3/django_common_task_system/__init__.py
+-rw-rw-rw-   0        0        0    11370 2023-04-21 09:44:38.000000 django-common-task-system-1.2.3/django_common_task_system/admin.py
+-rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.2.3/django_common_task_system/apps.py
+-rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.2.3/django_common_task_system/choices.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.2.3/django_common_task_system/fields.py
+-rw-rw-rw-   0        0        0    15985 2023-04-21 09:40:54.000000 django-common-task-system-1.2.3/django_common_task_system/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.050304 django-common-task-system-1.2.3/django_common_task_system/migrations/
+-rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+-rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+-rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/0006_consumerpermission.py
+-rw-rw-rw-   0        0        0     1275 2023-04-21 07:23:00.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.2.3/django_common_task_system/mixin.py
+-rw-rw-rw-   0        0        0    36762 2023-04-23 03:16:06.000000 django-common-task-system-1.2.3/django_common_task_system/models.py
+-rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.2.3/django_common_task_system/permissions.py
+-rw-rw-rw-   0        0        0     2272 2023-04-21 08:20:32.000000 django-common-task-system-1.2.3/django_common_task_system/serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.023551 django-common-task-system-1.2.3/django_common_task_system/static/
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.024551 django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.051308 django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/css/
+-rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/css/calendar.css
+-rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.053307 django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/js/
+-rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/js/calendar.js
+-rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.061304 django-common-task-system-1.2.3/django_common_task_system/system_task/
+-rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/__init__.py
+-rw-rw-rw-   0        0        0     5166 2023-04-21 07:14:23.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/admin.py
+-rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/apps.py
+-rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/choices.py
+-rw-rw-rw-   0        0        0     4130 2023-04-19 09:42:02.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.066307 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/
+-rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+-rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
+-rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
+-rw-rw-rw-   0        0        0     1062 2023-04-21 07:23:00.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/__init__.py
+-rw-rw-rw-   0        0        0    14945 2023-04-21 07:09:25.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/models.py
+-rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/process.py
+-rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/queue.py
+-rw-rw-rw-   0        0        0     1679 2023-04-21 07:11:39.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/tests.py
+-rw-rw-rw-   0        0        0      846 2023-04-21 07:22:44.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/urls.py
+-rw-rw-rw-   0        0        0     5505 2023-04-21 07:22:44.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/views.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.067306 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     1674 2023-04-19 09:54:46.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/main.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.069307 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     3100 2023-04-21 07:40:43.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executor.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.073310 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/
+-rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+-rw-rw-rw-   0        0        0     3500 2023-04-17 05:43:02.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+-rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+-rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+-rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.026547 django-common-task-system-1.2.3/django_common_task_system/templates/
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.025546 django-common-task-system-1.2.3/django_common_task_system/templates/admin/
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.074309 django-common-task-system-1.2.3/django_common_task_system/templates/admin/system_schedule/
+-rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.2.3/django_common_task_system/templates/admin/system_schedule/change_list.html
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.078307 django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/
+-rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/datetime_range.html
+-rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/multi_day_select.html
+-rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/multi_month_day_select.html
+-rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/nlp_input.html
+-rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/period.html
+-rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/period_schedule.html
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.2.3/django_common_task_system/tests.py
+-rw-rw-rw-   0        0        0     1060 2023-04-21 07:22:44.000000 django-common-task-system-1.2.3/django_common_task_system/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.082304 django-common-task-system-1.2.3/django_common_task_system/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.2.3/django_common_task_system/utils/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.2.3/django_common_task_system/utils/algorithm.py
+-rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.2.3/django_common_task_system/utils/cron_utils.py
+-rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.2.3/django_common_task_system/utils/foreign_key.py
+-rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.2.3/django_common_task_system/utils/schedule_time.py
+-rw-rw-rw-   0        0        0    11880 2023-04-23 03:18:23.000000 django-common-task-system-1.2.3/django_common_task_system/views.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.043308 django-common-task-system-1.2.3/django_common_task_system.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-04-23 03:20:20.000000 django-common-task-system-1.2.3/django_common_task_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4423 2023-04-23 03:20:20.000000 django-common-task-system-1.2.3/django_common_task_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 03:20:20.000000 django-common-task-system-1.2.3/django_common_task_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-04-23 03:20:20.000000 django-common-task-system-1.2.3/django_common_task_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-23 03:20:20.000000 django-common-task-system-1.2.3/django_common_task_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 03:20:20.084304 django-common-task-system-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-04-23 03:13:16.000000 django-common-task-system-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.082304 django-common-task-system-1.2.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.2.3/tests/__init__.py
```

### Comparing `django-common-task-system-1.2.2/LICENSE` & `django-common-task-system-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/__init__.py` & `django-common-task-system-1.2.3/django_common_task_system/__init__.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/admin.py` & `django-common-task-system-1.2.3/django_common_task_system/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/choices.py` & `django-common-task-system-1.2.3/django_common_task_system/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/fields.py` & `django-common-task-system-1.2.3/django_common_task_system/fields.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/forms.py` & `django-common-task-system-1.2.3/django_common_task_system/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/migrations/0001_initial.py` & `django-common-task-system-1.2.3/django_common_task_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py` & `django-common-task-system-1.2.3/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py` & `django-common-task-system-1.2.3/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/migrations/0006_consumerpermission.py` & `django-common-task-system-1.2.3/django_common_task_system/migrations/0006_consumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py` & `django-common-task-system-1.2.3/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/mixin.py` & `django-common-task-system-1.2.3/django_common_task_system/mixin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/models.py` & `django-common-task-system-1.2.3/django_common_task_system/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,38 +19,41 @@
 from django.core.validators import ValidationError
 from django.dispatch import Signal, receiver
 from threading import Event
 from collections import OrderedDict
 
 system_initialize_signal = Signal()
 system_schedule_event = Event()
+system_signal_sent = False
 
 mdays = [0, 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
 
 
 UserModel = get_user_model()
 
 is_task_initialized = 'django_common_task_system' in settings.INSTALLED_APPS
 is_system_task_initialized = 'django_common_system_task.system_task' in settings.INSTALLED_APPS
 
 
 @receiver(system_initialize_signal, sender='builtin_initialized')
 def on_builtin_initialized(sender, app=None, **kwargs):
-    global is_task_initialized, is_system_task_initialized
+    global is_task_initialized, is_system_task_initialized, system_signal_sent
     if app == 'django_common_task_system':
         is_task_initialized = True
     elif app == 'django_common_task_system.system_task':
         is_system_task_initialized = True
-    if is_task_initialized and is_system_task_initialized:
+    # 加入system_signal_sent判断, 防止重复发送信号
+    if is_task_initialized and is_system_task_initialized and not system_signal_sent:
         from threading import Timer
 
         def send_signal():
             system_initialize_signal.send(sender='system_initialized')
         # 这里django_common_task_system和django_common_system_task都初始化完成了, 但是其他app还未
         # 完成初始化, 所以这里延迟一段时间再发送信号
+        system_signal_sent = True
         Timer(2, send_signal).start()
 
 
 def code_validator(value):
     if re.match(r'[a-zA-Z_-]+', value) is None:
         raise ValidationError('编码只能包含字母、数字、下划线和中划线')
```

### Comparing `django-common-task-system-1.2.2/django_common_task_system/permissions.py` & `django-common-task-system-1.2.3/django_common_task_system/permissions.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/serializers.py` & `django-common-task-system-1.2.3/django_common_task_system/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/static/common_task_system/css/calendar.css` & `django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/css/calendar.css`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/static/common_task_system/js/calendar.js` & `django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/js/calendar.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/static/common_task_system/js/task_schedule_admin.js` & `django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/js/task_schedule_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/admin.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/choices.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/forms.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/0001_initial.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/models.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/models.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/process.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/process.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/queue.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/queue.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/serializers.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/urls.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task/views.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task_execution/main.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task_execution/main.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/executor.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executor.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/executors/base.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/base.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py` & `django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/templates/admin/system_schedule/change_list.html` & `django-common-task-system-1.2.3/django_common_task_system/templates/admin/system_schedule/change_list.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/templates/task_schedule/multi_day_select.html` & `django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/multi_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/templates/task_schedule/multi_month_day_select.html` & `django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/multi_month_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/templates/task_schedule/nlp_input.html` & `django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/nlp_input.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/templates/task_schedule/period_schedule.html` & `django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/period_schedule.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/urls.py` & `django-common-task-system-1.2.3/django_common_task_system/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/utils/algorithm.py` & `django-common-task-system-1.2.3/django_common_task_system/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/utils/foreign_key.py` & `django-common-task-system-1.2.3/django_common_task_system/utils/foreign_key.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/utils/schedule_time.py` & `django-common-task-system-1.2.3/django_common_task_system/utils/schedule_time.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/django_common_task_system/views.py` & `django-common-task-system-1.2.3/django_common_task_system/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from rest_framework.decorators import api_view
 from rest_framework.generics import CreateAPIView
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.views import APIView
 from rest_framework.viewsets import ModelViewSet
 from django.http.response import JsonResponse
+from django.conf import settings
 from . import serializers, get_task_model, get_schedule_log_model, get_task_schedule_model, get_task_schedule_serializer
 from .choices import TaskScheduleStatus
 from .models import TaskSchedule, TaskScheduleProducer, TaskScheduleQueue, \
     ConsumerPermission, ExceptionReport, builtins, ScheduleConfig
 from django_common_objects.rest_view import UserListAPIView, UserRetrieveAPIView
 from queue import Empty
 from datetime import datetime
@@ -38,45 +39,50 @@
     serializer = ScheduleSerializer
 
     def __init__(self):
         super().__init__(daemon=True)
 
     def produce(self):
         now = datetime.now()
+        qsize = getattr(settings, 'SCHEDULE_QUEUE_MAX_SIZE', 1000)
+        max_queue_size = qsize * 2
         for producer in self.producers.values():
-            queue = self.queues[producer.queue.code]
+            queue_instance = self.queues[producer.queue.code]
+            queue = queue_instance.queue
             # 队列长度大于1000时不再生产, 防止内存溢出
-            if queue.queue.qsize() > 1000:
+            if queue.qsize() >= qsize:
                 continue
             queryset = self.schedule_model.objects.filter(**producer.filters)
             if producer.lte_now:
                 queryset = queryset.filter(next_schedule_time__lte=now)
             for schedule in queryset:
                 try:
-                    while schedule.next_schedule_time <= now:
+                    # 限制队列长度, 防止内存溢出
+                    while queue.qsize() < max_queue_size and schedule.next_schedule_time <= now:
                         data = self.serializer(schedule).data
-                        data['queue'] = queue.code
-                        queue.queue.put(data)
+                        data['queue'] = queue_instance.code
+                        queue.put(data)
                         schedule.next_schedule_time = ScheduleConfig(config=schedule.config
                                                                      ).get_next_time(schedule.next_schedule_time)
                     schedule.save(update_fields=('next_schedule_time', ))
                 except Exception as e:
                     schedule.status = TaskScheduleStatus.ERROR.value
                     schedule.save(update_fields=('status',))
                     traceback.print_exc()
 
     def run(self) -> None:
         # 等待系统初始化完成, 5秒后自动开始
         system_schedule_event.wait(timeout=5)
+        SCHEDULE_INTERVAL = getattr(settings, 'SCHEDULE_INTERVAL', 1)
         while True:
             try:
                 self.produce()
             except Exception as err:
                 traceback.print_exc()
-            time.sleep(0.5)
+            time.sleep(SCHEDULE_INTERVAL)
 
 
 @receiver(system_initialize_signal, sender='system_initialized')
 def on_system_initialized(sender, **kwargs):
     thread = TaskScheduleThread()
     thread.start()
```

### Comparing `django-common-task-system-1.2.2/django_common_task_system.egg-info/SOURCES.txt` & `django-common-task-system-1.2.3/django_common_task_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.2/setup.py` & `django-common-task-system-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-common-task-system',
     packages=find_packages(exclude=['local_tests']),
-    version='1.2.2',
+    version='1.2.3',
     install_requires=[
         "django-common-objects>=1.0.5",
         "django>=3.2.18",
         "croniter>=1.3.8",
         "djangorestframework>=3.14.0",
         "PyMySQL>=1.0.2",
         "jionlp-time>=1.0.0",
```

