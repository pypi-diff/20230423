# Comparing `tmp/pulsar-app-0.9.0.tar.gz` & `tmp/pulsar-app-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulsar-app-0.9.0.tar", last modified: Fri Apr 12 17:05:14 2019, max compression
+gzip compressed data, was "dist/pulsar-app-0.9.1.tar", last modified: Wed May  1 13:01:22 2019, max compression
```

## Comparing `pulsar-app-0.9.0.tar` & `pulsar-app-0.9.1.tar`

### file list

```diff
@@ -1,147 +1,149 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/
--rw-r--r--   0 nate       (501) staff       (20)     5349 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 nate       (501) staff       (20)     4175 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 nate       (501) staff       (20)    11561 2019-04-12 17:05:13.000000 pulsar-app-0.9.0/HISTORY.rst
--rw-r--r--   0 nate       (501) staff       (20)    11358 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)       67 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/MANIFEST.in
--rw-r--r--   0 nate       (501) staff       (20)    19262 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/PKG-INFO
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/
--rw-r--r--   0 nate       (501) staff       (20)      379 2019-04-12 17:05:13.000000 pulsar-app-0.9.0/pulsar/__init__.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/cache/
--rw-r--r--   0 nate       (501) staff       (20)     1736 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/cache/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)      970 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/cache/persistence.py
--rw-r--r--   0 nate       (501) staff       (20)     1085 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/cache/util.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/client/
--rw-r--r--   0 nate       (501) staff       (20)     2010 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)    25586 2019-04-12 14:35:58.000000 pulsar-app-0.9.0/pulsar/client/action_mapper.py
--rw-r--r--   0 nate       (501) staff       (20)    13314 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/amqp_exchange.py
--rw-r--r--   0 nate       (501) staff       (20)     2139 2019-04-12 14:35:58.000000 pulsar-app-0.9.0/pulsar/client/amqp_exchange_factory.py
--rw-r--r--   0 nate       (501) staff       (20)    15976 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/client.py
--rw-r--r--   0 nate       (501) staff       (20)     1688 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/config_util.py
--rw-r--r--   0 nate       (501) staff       (20)      825 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/decorators.py
--rw-r--r--   0 nate       (501) staff       (20)     1855 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/destination.py
--rw-r--r--   0 nate       (501) staff       (20)     1296 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/exceptions.py
--rw-r--r--   0 nate       (501) staff       (20)     6231 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/interface.py
--rw-r--r--   0 nate       (501) staff       (20)     5330 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/job_directory.py
--rw-r--r--   0 nate       (501) staff       (20)    11836 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/manager.py
--rw-r--r--   0 nate       (501) staff       (20)     1712 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/object_client.py
--rw-r--r--   0 nate       (501) staff       (20)     4458 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/path_mapper.py
--rw-r--r--   0 nate       (501) staff       (20)     4066 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/setup_handler.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/client/staging/
--rw-r--r--   0 nate       (501) staff       (20)     7597 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/staging/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)     7287 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/staging/down.py
--rw-r--r--   0 nate       (501) staff       (20)    19921 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/staging/up.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/client/test/
--rw-r--r--   0 nate       (501) staff       (20)        0 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/test/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)    19979 2019-04-12 14:35:58.000000 pulsar-app-0.9.0/pulsar/client/test/check.py
--rw-r--r--   0 nate       (501) staff       (20)      686 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/test/test_common.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/client/transport/
--rw-r--r--   0 nate       (501) staff       (20)     1484 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/transport/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)     4044 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/transport/curl.py
--rw-r--r--   0 nate       (501) staff       (20)     1261 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/transport/poster.py
--rw-r--r--   0 nate       (501) staff       (20)     1338 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/transport/requests.py
--rw-r--r--   0 nate       (501) staff       (20)     1767 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/transport/ssh.py
--rw-r--r--   0 nate       (501) staff       (20)     2088 2019-04-12 14:35:58.000000 pulsar-app-0.9.0/pulsar/client/transport/standard.py
--rw-r--r--   0 nate       (501) staff       (20)     9105 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/client/util.py
--rw-r--r--   0 nate       (501) staff       (20)     5829 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/core.py
--rw-r--r--   0 nate       (501) staff       (20)     1413 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/locks.py
--rw-r--r--   0 nate       (501) staff       (20)    10662 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/main.py
--rw-r--r--   0 nate       (501) staff       (20)     4636 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/manager_endpoint_util.py
--rw-r--r--   0 nate       (501) staff       (20)     6304 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/manager_factory.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/managers/
--rw-r--r--   0 nate       (501) staff       (20)     3746 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/__init__.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/managers/base/
--rw-r--r--   0 nate       (501) staff       (20)    14853 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/base/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)     3495 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/base/base_drmaa.py
--rw-r--r--   0 nate       (501) staff       (20)     5921 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/base/directory.py
--rw-r--r--   0 nate       (501) staff       (20)     2743 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/base/external.py
--rw-r--r--   0 nate       (501) staff       (20)     3433 2019-04-12 14:35:58.000000 pulsar-app-0.9.0/pulsar/managers/queued.py
--rw-r--r--   0 nate       (501) staff       (20)     2970 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/queued_cli.py
--rw-r--r--   0 nate       (501) staff       (20)     3422 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/queued_condor.py
--rw-r--r--   0 nate       (501) staff       (20)     1065 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/queued_drmaa.py
--rw-r--r--   0 nate       (501) staff       (20)     1659 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/queued_drmaa_xsede.py
--rw-r--r--   0 nate       (501) staff       (20)     4574 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/queued_external_drmaa.py
--rw-r--r--   0 nate       (501) staff       (20)      534 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/queued_pbs.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/managers/staging/
--rw-r--r--   0 nate       (501) staff       (20)      321 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/staging/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)     3381 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/staging/post.py
--rw-r--r--   0 nate       (501) staff       (20)      646 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/staging/pre.py
--rw-r--r--   0 nate       (501) staff       (20)    17446 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/stateful.py
--rw-r--r--   0 nate       (501) staff       (20)      859 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/status.py
--rw-r--r--   0 nate       (501) staff       (20)     6437 2019-04-12 14:35:58.000000 pulsar-app-0.9.0/pulsar/managers/unqueued.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/managers/util/
--rw-r--r--   0 nate       (501) staff       (20)      300 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/__init__.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/managers/util/cli/
--rw-r--r--   0 nate       (501) staff       (20)     3140 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/cli/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)      491 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/cli/factory.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/managers/util/cli/job/
--rw-r--r--   0 nate       (501) staff       (20)     1405 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/cli/job/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)     2938 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/cli/job/slurm.py
--rw-r--r--   0 nate       (501) staff       (20)      906 2019-04-12 14:35:58.000000 pulsar-app-0.9.0/pulsar/managers/util/cli/job/slurm_torque.py
--rw-r--r--   0 nate       (501) staff       (20)     3822 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/cli/job/torque.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/managers/util/cli/shell/
--rw-r--r--   0 nate       (501) staff       (20)      447 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/cli/shell/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)     1919 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/cli/shell/local.py
--rw-r--r--   0 nate       (501) staff       (20)     1382 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/cli/shell/rsh.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/managers/util/condor/
--rw-r--r--   0 nate       (501) staff       (20)     3923 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/condor/__init__.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/managers/util/drmaa/
--rw-r--r--   0 nate       (501) staff       (20)     3243 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/drmaa/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)     1279 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/env.py
--rw-r--r--   0 nate       (501) staff       (20)     1103 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/external.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/managers/util/job_script/
--rw-r--r--   0 nate       (501) staff       (20)     5092 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/job_script/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)     1192 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/job_script/CLUSTER_SLOTS_STATEMENT.sh
--rw-r--r--   0 nate       (501) staff       (20)     1011 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/job_script/DEFAULT_JOB_FILE_TEMPLATE.sh
--rw-r--r--   0 nate       (501) staff       (20)     1388 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/kill.py
--rw-r--r--   0 nate       (501) staff       (20)     4271 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/retry.py
--rw-r--r--   0 nate       (501) staff       (20)      780 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/managers/util/sudo.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/mesos/
--rw-r--r--   0 nate       (501) staff       (20)     1034 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/mesos/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)     5977 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/mesos/framework.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/messaging/
--rw-r--r--   0 nate       (501) staff       (20)     1219 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/messaging/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)     4915 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/messaging/bind_amqp.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/scripts/
--rw-r--r--   0 nate       (501) staff       (20)      230 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/scripts/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)        0 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/scripts/bootstrap.py
--rw-r--r--   0 nate       (501) staff       (20)     1381 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/scripts/chown_working_directory.py
--rw-r--r--   0 nate       (501) staff       (20)    13097 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/scripts/config.py
--rw-r--r--   0 nate       (501) staff       (20)      516 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/scripts/drmaa_kill.py
--rw-r--r--   0 nate       (501) staff       (20)      593 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/scripts/drmaa_launch.py
--rw-r--r--   0 nate       (501) staff       (20)     2648 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/scripts/mesos_executor.py
--rw-r--r--   0 nate       (501) staff       (20)      792 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/scripts/mesos_framework.py
--rw-r--r--   0 nate       (501) staff       (20)     4466 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/scripts/run.py
--rw-r--r--   0 nate       (501) staff       (20)      462 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/scripts/submit.py
--rw-r--r--   0 nate       (501) staff       (20)     1907 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/scripts/submit_util.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/tools/
--rw-r--r--   0 nate       (501) staff       (20)       68 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/tools/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)     2660 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/tools/authorization.py
--rw-r--r--   0 nate       (501) staff       (20)     5322 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/tools/toolbox.py
--rw-r--r--   0 nate       (501) staff       (20)     4347 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/tools/validator.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/util/
--rw-r--r--   0 nate       (501) staff       (20)      842 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/util/__init__.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/util/pastescript/
--rw-r--r--   0 nate       (501) staff       (20)       73 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/util/pastescript/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)    28495 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/util/pastescript/loadwsgi.py
--rw-r--r--   0 nate       (501) staff       (20)    36420 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/util/pastescript/serve.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar/web/
--rw-r--r--   0 nate       (501) staff       (20)      109 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/web/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)     5993 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/web/framework.py
--rw-r--r--   0 nate       (501) staff       (20)    10234 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/web/routes.py
--rw-r--r--   0 nate       (501) staff       (20)     1756 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/pulsar/web/wsgi.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar_app.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)        1 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar_app.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)      461 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar_app.egg-info/entry_points.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2019-04-12 15:06:13.000000 pulsar-app-0.9.0/pulsar_app.egg-info/not-zip-safe
--rw-r--r--   0 nate       (501) staff       (20)    19262 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar_app.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)       53 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar_app.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)     3532 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar_app.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        7 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/pulsar_app.egg-info/top_level.txt
--rw-r--r--   0 nate       (501) staff       (20)     3818 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/README.rst
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/scripts/
--rwxr-xr-x   0 nate       (501) staff       (20)     4239 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/scripts/pulsar
--rw-r--r--   0 nate       (501) staff       (20)      286 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)     4080 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/setup.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-04-12 17:05:14.000000 pulsar-app-0.9.0/test/
--rw-r--r--   0 nate       (501) staff       (20)    15707 2019-04-12 14:35:27.000000 pulsar-app-0.9.0/test/test_utils.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/
+-rw-r--r--   0 john       (502) staff       (20)     5349 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 john       (502) staff       (20)     4175 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 john       (502) staff       (20)    12193 2019-05-01 13:01:21.000000 pulsar-app-0.9.1/HISTORY.rst
+-rw-r--r--   0 john       (502) staff       (20)    11358 2018-02-14 01:20:39.000000 pulsar-app-0.9.1/LICENSE
+-rw-r--r--   0 john       (502) staff       (20)       67 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/MANIFEST.in
+-rw-r--r--   0 john       (502) staff       (20)    20006 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/PKG-INFO
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/
+-rw-r--r--   0 john       (502) staff       (20)      379 2019-05-01 13:01:21.000000 pulsar-app-0.9.1/pulsar/__init__.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/cache/
+-rw-r--r--   0 john       (502) staff       (20)     1736 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/cache/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)      970 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/cache/persistence.py
+-rw-r--r--   0 john       (502) staff       (20)     1085 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/cache/util.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/client/
+-rw-r--r--   0 john       (502) staff       (20)     2010 2019-04-15 12:25:16.000000 pulsar-app-0.9.1/pulsar/client/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)    25586 2019-04-15 12:25:16.000000 pulsar-app-0.9.1/pulsar/client/action_mapper.py
+-rw-r--r--   0 john       (502) staff       (20)    13314 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/amqp_exchange.py
+-rw-r--r--   0 john       (502) staff       (20)     2139 2019-04-15 12:25:16.000000 pulsar-app-0.9.1/pulsar/client/amqp_exchange_factory.py
+-rw-r--r--   0 john       (502) staff       (20)    15976 2019-05-01 12:27:50.000000 pulsar-app-0.9.1/pulsar/client/client.py
+-rw-r--r--   0 john       (502) staff       (20)     1688 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/config_util.py
+-rw-r--r--   0 john       (502) staff       (20)      825 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/decorators.py
+-rw-r--r--   0 john       (502) staff       (20)     1855 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/destination.py
+-rw-r--r--   0 john       (502) staff       (20)     1296 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/exceptions.py
+-rw-r--r--   0 john       (502) staff       (20)     6231 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/interface.py
+-rw-r--r--   0 john       (502) staff       (20)     5330 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/job_directory.py
+-rw-r--r--   0 john       (502) staff       (20)    11836 2019-05-01 12:27:50.000000 pulsar-app-0.9.1/pulsar/client/manager.py
+-rw-r--r--   0 john       (502) staff       (20)     1712 2018-02-14 01:20:39.000000 pulsar-app-0.9.1/pulsar/client/object_client.py
+-rw-r--r--   0 john       (502) staff       (20)     4458 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/path_mapper.py
+-rw-r--r--   0 john       (502) staff       (20)     4066 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/setup_handler.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/client/staging/
+-rw-r--r--   0 john       (502) staff       (20)     7597 2019-05-01 12:27:50.000000 pulsar-app-0.9.1/pulsar/client/staging/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)     7287 2019-04-26 13:59:50.000000 pulsar-app-0.9.1/pulsar/client/staging/down.py
+-rw-r--r--   0 john       (502) staff       (20)    20065 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/client/staging/up.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/client/test/
+-rw-r--r--   0 john       (502) staff       (20)        0 2018-02-14 01:20:39.000000 pulsar-app-0.9.1/pulsar/client/test/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)    19996 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/client/test/check.py
+-rw-r--r--   0 john       (502) staff       (20)      686 2018-02-14 01:20:39.000000 pulsar-app-0.9.1/pulsar/client/test/test_common.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/client/transport/
+-rw-r--r--   0 john       (502) staff       (20)     1484 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/transport/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)     4044 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/transport/curl.py
+-rw-r--r--   0 john       (502) staff       (20)     1261 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/transport/poster.py
+-rw-r--r--   0 john       (502) staff       (20)     1338 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/transport/requests.py
+-rw-r--r--   0 john       (502) staff       (20)     1767 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/transport/ssh.py
+-rw-r--r--   0 john       (502) staff       (20)     2088 2019-04-15 12:25:16.000000 pulsar-app-0.9.1/pulsar/client/transport/standard.py
+-rw-r--r--   0 john       (502) staff       (20)     9105 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/client/util.py
+-rw-r--r--   0 john       (502) staff       (20)     5829 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/core.py
+-rw-r--r--   0 john       (502) staff       (20)     1413 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/locks.py
+-rw-r--r--   0 john       (502) staff       (20)    10662 2019-05-01 12:27:50.000000 pulsar-app-0.9.1/pulsar/main.py
+-rw-r--r--   0 john       (502) staff       (20)     4636 2019-05-01 12:27:49.000000 pulsar-app-0.9.1/pulsar/manager_endpoint_util.py
+-rw-r--r--   0 john       (502) staff       (20)     6304 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/manager_factory.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/managers/
+-rw-r--r--   0 john       (502) staff       (20)     3746 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/managers/__init__.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/managers/base/
+-rw-r--r--   0 john       (502) staff       (20)    14853 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/managers/base/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)     3495 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/managers/base/base_drmaa.py
+-rw-r--r--   0 john       (502) staff       (20)     5921 2019-05-01 12:27:50.000000 pulsar-app-0.9.1/pulsar/managers/base/directory.py
+-rw-r--r--   0 john       (502) staff       (20)     2743 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/managers/base/external.py
+-rw-r--r--   0 john       (502) staff       (20)     3433 2019-05-01 12:27:50.000000 pulsar-app-0.9.1/pulsar/managers/queued.py
+-rw-r--r--   0 john       (502) staff       (20)     2970 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/managers/queued_cli.py
+-rw-r--r--   0 john       (502) staff       (20)     3422 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/managers/queued_condor.py
+-rw-r--r--   0 john       (502) staff       (20)     1065 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/managers/queued_drmaa.py
+-rw-r--r--   0 john       (502) staff       (20)     1659 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/managers/queued_drmaa_xsede.py
+-rw-r--r--   0 john       (502) staff       (20)     4574 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/managers/queued_external_drmaa.py
+-rw-r--r--   0 john       (502) staff       (20)      534 2018-02-14 01:20:39.000000 pulsar-app-0.9.1/pulsar/managers/queued_pbs.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/managers/staging/
+-rw-r--r--   0 john       (502) staff       (20)      321 2018-02-14 01:20:39.000000 pulsar-app-0.9.1/pulsar/managers/staging/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)     3381 2019-04-26 13:34:39.000000 pulsar-app-0.9.1/pulsar/managers/staging/post.py
+-rw-r--r--   0 john       (502) staff       (20)      646 2019-04-15 12:25:02.000000 pulsar-app-0.9.1/pulsar/managers/staging/pre.py
+-rw-r--r--   0 john       (502) staff       (20)    17437 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/stateful.py
+-rw-r--r--   0 john       (502) staff       (20)      859 2018-02-14 01:20:39.000000 pulsar-app-0.9.1/pulsar/managers/status.py
+-rw-r--r--   0 john       (502) staff       (20)     6437 2019-05-01 12:27:50.000000 pulsar-app-0.9.1/pulsar/managers/unqueued.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/managers/util/
+-rw-r--r--   0 john       (502) staff       (20)      299 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/__init__.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/managers/util/cli/
+-rw-r--r--   0 john       (502) staff       (20)     3095 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/cli/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)      491 2019-04-26 15:14:26.000000 pulsar-app-0.9.1/pulsar/managers/util/cli/factory.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/managers/util/cli/job/
+-rw-r--r--   0 john       (502) staff       (20)     1727 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/cli/job/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)     4842 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/cli/job/lsf.py
+-rw-r--r--   0 john       (502) staff       (20)     2937 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/cli/job/slurm.py
+-rw-r--r--   0 john       (502) staff       (20)      907 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/cli/job/slurm_torque.py
+-rw-r--r--   0 john       (502) staff       (20)     3821 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/cli/job/torque.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/managers/util/cli/shell/
+-rw-r--r--   0 john       (502) staff       (20)      471 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/cli/shell/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)     2134 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/cli/shell/local.py
+-rw-r--r--   0 john       (502) staff       (20)     3765 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/cli/shell/rsh.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/managers/util/condor/
+-rw-r--r--   0 john       (502) staff       (20)     3948 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/condor/__init__.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/managers/util/drmaa/
+-rw-r--r--   0 john       (502) staff       (20)     3243 2019-04-26 15:19:53.000000 pulsar-app-0.9.1/pulsar/managers/util/drmaa/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)     1279 2019-04-26 15:14:26.000000 pulsar-app-0.9.1/pulsar/managers/util/env.py
+-rw-r--r--   0 john       (502) staff       (20)     1103 2019-04-26 15:14:26.000000 pulsar-app-0.9.1/pulsar/managers/util/external.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/managers/util/job_script/
+-rw-r--r--   0 john       (502) staff       (20)     5633 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/job_script/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)     1319 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/job_script/CLUSTER_SLOTS_STATEMENT.sh
+-rw-r--r--   0 john       (502) staff       (20)     1400 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/job_script/DEFAULT_JOB_FILE_TEMPLATE.sh
+-rw-r--r--   0 john       (502) staff       (20)      871 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/job_script/MEMORY_STATEMENT.sh
+-rw-r--r--   0 john       (502) staff       (20)     1408 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/kill.py
+-rw-r--r--   0 john       (502) staff       (20)     4271 2019-04-26 15:14:56.000000 pulsar-app-0.9.1/pulsar/managers/util/retry.py
+-rw-r--r--   0 john       (502) staff       (20)      733 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/pulsar/managers/util/sudo.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/mesos/
+-rw-r--r--   0 john       (502) staff       (20)     1034 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/mesos/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)     5977 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/mesos/framework.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/messaging/
+-rw-r--r--   0 john       (502) staff       (20)     1219 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/messaging/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)     4915 2018-02-19 20:12:21.000000 pulsar-app-0.9.1/pulsar/messaging/bind_amqp.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/scripts/
+-rw-r--r--   0 john       (502) staff       (20)      230 2018-02-14 01:20:39.000000 pulsar-app-0.9.1/pulsar/scripts/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)        0 2018-02-14 01:20:39.000000 pulsar-app-0.9.1/pulsar/scripts/bootstrap.py
+-rw-r--r--   0 john       (502) staff       (20)     1381 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/scripts/chown_working_directory.py
+-rw-r--r--   0 john       (502) staff       (20)    13097 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/scripts/config.py
+-rw-r--r--   0 john       (502) staff       (20)      516 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/scripts/drmaa_kill.py
+-rw-r--r--   0 john       (502) staff       (20)      593 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/scripts/drmaa_launch.py
+-rw-r--r--   0 john       (502) staff       (20)     2648 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/scripts/mesos_executor.py
+-rw-r--r--   0 john       (502) staff       (20)      792 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/scripts/mesos_framework.py
+-rw-r--r--   0 john       (502) staff       (20)     4466 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/scripts/run.py
+-rw-r--r--   0 john       (502) staff       (20)      462 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/scripts/submit.py
+-rw-r--r--   0 john       (502) staff       (20)     1907 2019-05-01 12:27:49.000000 pulsar-app-0.9.1/pulsar/scripts/submit_util.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/tools/
+-rw-r--r--   0 john       (502) staff       (20)       68 2018-02-14 01:20:39.000000 pulsar-app-0.9.1/pulsar/tools/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)     2660 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/tools/authorization.py
+-rw-r--r--   0 john       (502) staff       (20)     5322 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/tools/toolbox.py
+-rw-r--r--   0 john       (502) staff       (20)     4347 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/tools/validator.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/util/
+-rw-r--r--   0 john       (502) staff       (20)      842 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/util/__init__.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/util/pastescript/
+-rw-r--r--   0 john       (502) staff       (20)       73 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/util/pastescript/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)    28495 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/util/pastescript/loadwsgi.py
+-rw-r--r--   0 john       (502) staff       (20)    36420 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/util/pastescript/serve.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar/web/
+-rw-r--r--   0 john       (502) staff       (20)      109 2018-02-14 01:20:39.000000 pulsar-app-0.9.1/pulsar/web/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)     5993 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/web/framework.py
+-rw-r--r--   0 john       (502) staff       (20)    10234 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/web/routes.py
+-rw-r--r--   0 john       (502) staff       (20)     1756 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/pulsar/web/wsgi.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/pulsar_app.egg-info/
+-rw-r--r--   0 john       (502) staff       (20)        1 2019-05-01 13:01:21.000000 pulsar-app-0.9.1/pulsar_app.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (502) staff       (20)      461 2019-05-01 13:01:21.000000 pulsar-app-0.9.1/pulsar_app.egg-info/entry_points.txt
+-rw-r--r--   0 john       (502) staff       (20)        1 2018-03-06 13:18:19.000000 pulsar-app-0.9.1/pulsar_app.egg-info/not-zip-safe
+-rw-r--r--   0 john       (502) staff       (20)    20006 2019-05-01 13:01:21.000000 pulsar-app-0.9.1/pulsar_app.egg-info/PKG-INFO
+-rw-r--r--   0 john       (502) staff       (20)       53 2019-05-01 13:01:21.000000 pulsar-app-0.9.1/pulsar_app.egg-info/requires.txt
+-rw-r--r--   0 john       (502) staff       (20)     3620 2019-05-01 13:01:21.000000 pulsar-app-0.9.1/pulsar_app.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (502) staff       (20)        7 2019-05-01 13:01:21.000000 pulsar-app-0.9.1/pulsar_app.egg-info/top_level.txt
+-rw-r--r--   0 john       (502) staff       (20)     3818 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/README.rst
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/scripts/
+-rwxr-xr-x   0 john       (502) staff       (20)     4239 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/scripts/pulsar
+-rw-r--r--   0 john       (502) staff       (20)      286 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/setup.cfg
+-rw-r--r--   0 john       (502) staff       (20)     4080 2018-02-19 17:04:35.000000 pulsar-app-0.9.1/setup.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-05-01 13:01:22.000000 pulsar-app-0.9.1/test/
+-rw-r--r--   0 john       (502) staff       (20)    16203 2019-05-01 12:27:56.000000 pulsar-app-0.9.1/test/test_utils.py
```

### Comparing `pulsar-app-0.9.0/CODE_OF_CONDUCT.rst` & `pulsar-app-0.9.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/CONTRIBUTING.rst` & `pulsar-app-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/HISTORY.rst` & `pulsar-app-0.9.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 
 History
 -------
 
 .. to_doc
 
 ---------------------
+0.9.1 (2019-05-01)
+---------------------
+
+* Fix duplicate inputs being a problem when staging Galaxy files.
+  `Pull Request 175`_
+* Fix deprecated ``assertEquals()`` (thanks to @nsoranzo). `Pull Request 173`_
+* Fix a method missing problem. `Pull Request 174`_
+* Sync "recent" galaxy runner util changes. `Pull Request 177`_
+
+---------------------
 0.9.0 (2019-04-12)
 ---------------------
     
 * Add configuration parameter to limit stream size read from disk. `Pull
   Request 157`_
 * Pass full job status for failed and lost jobs. `Pull Request 159`_
 * Improve message handling if problems occur during job setup/staging. `Pull
@@ -193,14 +203,18 @@
 ---------------------
 
 * See the original `announcement <http://dev.list.galaxyproject.org/New-Remote-Job-Runner-td4138951.html>`__
   and `initial commit <https://github.com/galaxyproject/pulsar/commit/163ed48d5a1902ceb84c38f10db8cbe5a0c1039d>`__.
 
 
 .. github_links
+.. _Pull Request 173: https://github.com/galaxyproject/pulsar/pull/173
+.. _Pull Request 174: https://github.com/galaxyproject/pulsar/pull/174
+.. _Pull Request 175: https://github.com/galaxyproject/pulsar/pull/175
+.. _Pull Request 177: https://github.com/galaxyproject/pulsar/pull/177
 .. _Pull Request 172: https://github.com/galaxyproject/pulsar/pull/172
 .. _Pull Request 170: https://github.com/galaxyproject/pulsar/pull/170
 .. _Pull Request 165: https://github.com/galaxyproject/pulsar/pull/165
 .. _Pull Request 164: https://github.com/galaxyproject/pulsar/pull/164
 .. _Pull Request 160: https://github.com/galaxyproject/pulsar/pull/160
 .. _Pull Request 159: https://github.com/galaxyproject/pulsar/pull/159
 .. _Pull Request 157: https://github.com/galaxyproject/pulsar/pull/157
```

### Comparing `pulsar-app-0.9.0/LICENSE` & `pulsar-app-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/PKG-INFO` & `pulsar-app-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pulsar-app
-Version: 0.9.0
+Version: 0.9.1
 Summary: Distributed job execution application built for Galaxy (http://galaxyproject.org/).
 Home-page: https://github.com/galaxyproject/pulsar
 Author: Galaxy Project
 Author-email: jmchilton@gmail.com
 License: Apache License 2.0
 Description: .. figure:: https://galaxyproject.org/images/galaxy-logos/pulsar_transparent.png
            :alt: Pulsar Logo
@@ -109,14 +109,24 @@
         
         History
         -------
         
         .. to_doc
         
         ---------------------
+        0.9.1 (2019-05-01)
+        ---------------------
+        
+        * Fix duplicate inputs being a problem when staging Galaxy files.
+          `Pull Request 175`_
+        * Fix deprecated ``assertEquals()`` (thanks to @nsoranzo). `Pull Request 173`_
+        * Fix a method missing problem. `Pull Request 174`_
+        * Sync "recent" galaxy runner util changes. `Pull Request 177`_
+        
+        ---------------------
         0.9.0 (2019-04-12)
         ---------------------
             
         * Add configuration parameter to limit stream size read from disk. `Pull
           Request 157`_
         * Pass full job status for failed and lost jobs. `Pull Request 159`_
         * Improve message handling if problems occur during job setup/staging. `Pull
@@ -300,14 +310,18 @@
         ---------------------
         
         * See the original `announcement <http://dev.list.galaxyproject.org/New-Remote-Job-Runner-td4138951.html>`__
           and `initial commit <https://github.com/galaxyproject/pulsar/commit/163ed48d5a1902ceb84c38f10db8cbe5a0c1039d>`__.
         
         
         .. github_links
+        .. _Pull Request 173: https://github.com/galaxyproject/pulsar/pull/173
+        .. _Pull Request 174: https://github.com/galaxyproject/pulsar/pull/174
+        .. _Pull Request 175: https://github.com/galaxyproject/pulsar/pull/175
+        .. _Pull Request 177: https://github.com/galaxyproject/pulsar/pull/177
         .. _Pull Request 172: https://github.com/galaxyproject/pulsar/pull/172
         .. _Pull Request 170: https://github.com/galaxyproject/pulsar/pull/170
         .. _Pull Request 165: https://github.com/galaxyproject/pulsar/pull/165
         .. _Pull Request 164: https://github.com/galaxyproject/pulsar/pull/164
         .. _Pull Request 160: https://github.com/galaxyproject/pulsar/pull/160
         .. _Pull Request 159: https://github.com/galaxyproject/pulsar/pull/159
         .. _Pull Request 157: https://github.com/galaxyproject/pulsar/pull/157
```

### Comparing `pulsar-app-0.9.0/pulsar/cache/__init__.py` & `pulsar-app-0.9.1/pulsar/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/cache/persistence.py` & `pulsar-app-0.9.1/pulsar/cache/persistence.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/cache/util.py` & `pulsar-app-0.9.1/pulsar/cache/util.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/__init__.py` & `pulsar-app-0.9.1/pulsar/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/action_mapper.py` & `pulsar-app-0.9.1/pulsar/client/action_mapper.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/amqp_exchange.py` & `pulsar-app-0.9.1/pulsar/client/amqp_exchange.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/amqp_exchange_factory.py` & `pulsar-app-0.9.1/pulsar/client/amqp_exchange_factory.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/client.py` & `pulsar-app-0.9.1/pulsar/client/client.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/config_util.py` & `pulsar-app-0.9.1/pulsar/client/config_util.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/decorators.py` & `pulsar-app-0.9.1/pulsar/client/decorators.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/destination.py` & `pulsar-app-0.9.1/pulsar/client/destination.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/exceptions.py` & `pulsar-app-0.9.1/pulsar/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/interface.py` & `pulsar-app-0.9.1/pulsar/client/interface.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/job_directory.py` & `pulsar-app-0.9.1/pulsar/client/job_directory.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/manager.py` & `pulsar-app-0.9.1/pulsar/client/manager.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/object_client.py` & `pulsar-app-0.9.1/pulsar/client/object_client.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/path_mapper.py` & `pulsar-app-0.9.1/pulsar/client/path_mapper.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/setup_handler.py` & `pulsar-app-0.9.1/pulsar/client/setup_handler.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/staging/__init__.py` & `pulsar-app-0.9.1/pulsar/client/staging/__init__.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/staging/down.py` & `pulsar-app-0.9.1/pulsar/client/staging/down.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/staging/up.py` & `pulsar-app-0.9.1/pulsar/client/staging/up.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,17 +201,21 @@
             self.transfer_tracker.handle_transfer(referenced_tool_file, path_type.TOOL)
 
     def __upload_arbitrary_files(self):
         for path, name in self.arbitrary_files.items():
             self.transfer_tracker.handle_transfer(path, path_type.UNSTRUCTURED, name=name)
 
     def __upload_input_files(self):
+        handled_inputs = set()
         for input_file in self.input_files:
+            if input_file in handled_inputs:
+                continue
             self.__upload_input_file(input_file)
             self.__upload_input_extra_files(input_file)
+            handled_inputs.add(input_file)
 
     def __upload_input_file(self, input_file):
         if self.__stage_input(input_file):
             if exists(input_file):
                 self.transfer_tracker.handle_transfer(input_file, path_type.INPUT)
             else:
                 message = "Pulsar: __upload_input_file called on empty or missing dataset." + \
```

### Comparing `pulsar-app-0.9.0/pulsar/client/test/check.py` & `pulsar-app-0.9.1/pulsar/client/test/check.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             temp_output4_path,
             temp_shared_dir,
             temp_metadata_path,
         )
         assert os.path.exists(temp_index_path)
         command_line = u'python %s "%s" "%s" "%s" "%s" "%s" "%s" "%s" "%s" "%s" "%s" "%s" "%s" "%s"' % command_line_params
         config_files = [temp_config_path]
-        input_files = [temp_input_path, empty_input]
+        input_files = [temp_input_path, temp_input_path, empty_input]
         output_files = [
             temp_output_path,
             temp_output2_path,
             temp_output3_path,
             temp_output4_path,
             temp_output_workdir_destination,
             temp_output_workdir_destination2
```

### Comparing `pulsar-app-0.9.0/pulsar/client/test/test_common.py` & `pulsar-app-0.9.1/pulsar/client/test/test_common.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/transport/__init__.py` & `pulsar-app-0.9.1/pulsar/client/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/transport/curl.py` & `pulsar-app-0.9.1/pulsar/client/transport/curl.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/transport/poster.py` & `pulsar-app-0.9.1/pulsar/client/transport/poster.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/transport/requests.py` & `pulsar-app-0.9.1/pulsar/client/transport/requests.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/transport/ssh.py` & `pulsar-app-0.9.1/pulsar/client/transport/ssh.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/transport/standard.py` & `pulsar-app-0.9.1/pulsar/client/transport/standard.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/client/util.py` & `pulsar-app-0.9.1/pulsar/client/util.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/core.py` & `pulsar-app-0.9.1/pulsar/core.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/locks.py` & `pulsar-app-0.9.1/pulsar/locks.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/main.py` & `pulsar-app-0.9.1/pulsar/main.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/manager_endpoint_util.py` & `pulsar-app-0.9.1/pulsar/manager_endpoint_util.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/manager_factory.py` & `pulsar-app-0.9.1/pulsar/manager_factory.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/__init__.py` & `pulsar-app-0.9.1/pulsar/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/base/__init__.py` & `pulsar-app-0.9.1/pulsar/managers/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/base/base_drmaa.py` & `pulsar-app-0.9.1/pulsar/managers/base/base_drmaa.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/base/directory.py` & `pulsar-app-0.9.1/pulsar/managers/base/directory.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/base/external.py` & `pulsar-app-0.9.1/pulsar/managers/base/external.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/queued.py` & `pulsar-app-0.9.1/pulsar/managers/queued.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/queued_cli.py` & `pulsar-app-0.9.1/pulsar/managers/queued_cli.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/queued_condor.py` & `pulsar-app-0.9.1/pulsar/managers/queued_condor.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/queued_drmaa.py` & `pulsar-app-0.9.1/pulsar/managers/queued_drmaa.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/queued_drmaa_xsede.py` & `pulsar-app-0.9.1/pulsar/managers/queued_drmaa_xsede.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/queued_external_drmaa.py` & `pulsar-app-0.9.1/pulsar/managers/queued_external_drmaa.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/queued_pbs.py` & `pulsar-app-0.9.1/pulsar/managers/queued_pbs.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/staging/post.py` & `pulsar-app-0.9.1/pulsar/managers/staging/post.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/staging/pre.py` & `pulsar-app-0.9.1/pulsar/managers/staging/pre.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/stateful.py` & `pulsar-app-0.9.1/pulsar/managers/stateful.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
                 log.warn("Job scheduled to prepreprocess [%s] previously failed preprocessing, skipping" % job_id)
                 unqueue_preprocessing_ids.append(job_id)
             else:
                 launch_config = job_directory.load_metadata("launch_config")
                 self._launch_prepreprocessing_thread(job_id, launch_config)
 
         for unqueue_preprocessing_id in unqueue_preprocessing_ids:
-            self.active_job_directory.deactivate_job(unqueue_preprocessing_id, active_status=ACTIVE_STATUS_PREPROCESSING)
+            self.active_jobs.deactivate_job(unqueue_preprocessing_id, active_status=ACTIVE_STATUS_PREPROCESSING)
 
         recover_method = getattr(self._proxied_manager, "_recover_active_job", None)
         if recover_method is None:
             return
 
         for job_id in self.active_jobs.active_job_ids(active_status=ACTIVE_STATUS_LAUNCHED):
             try:
```

### Comparing `pulsar-app-0.9.0/pulsar/managers/status.py` & `pulsar-app-0.9.1/pulsar/managers/status.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/unqueued.py` & `pulsar-app-0.9.1/pulsar/managers/unqueued.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/cli/__init__.py` & `pulsar-app-0.9.1/pulsar/managers/util/cli/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 """
+import json
 from glob import glob
-from inspect import getsourcefile
-from os import pardir
-from os.path import abspath
-from os.path import basename
-from os.path import join
+from os import getcwd
+from os.path import (
+    basename,
+    join
+)
 
 DEFAULT_SHELL_PLUGIN = 'LocalShell'
 
 ERROR_MESSAGE_NO_JOB_PLUGIN = "No job plugin parameter found, cannot create CLI job interface"
 ERROR_MESSAGE_NO_SUCH_JOB_PLUGIN = "Failed to find job_plugin of type %s, available types include %s"
 
 
@@ -18,61 +19,60 @@
     High-level interface for loading shell and job plugins and matching
     them to specified parameters.
     """
 
     def __init__(self, code_dir='lib'):
         """
         """
-        def __load(module_prefix, d, code_dir):
-            module_pattern = join(join(code_dir, module_prefix), '*.py')
+        def __load(module_path, d):
+            module_pattern = join(join(getcwd(), code_dir, *module_path.split('.')), '*.py')
             for file in glob(module_pattern):
                 if basename(file).startswith('_'):
                     continue
-                file = file.split(code_dir)[1]
-                module_name = '%s.%s' % (module_prefix.replace("/", "."), basename(file).rsplit('.py', 1)[0])
+                module_name = '%s.%s' % (module_path, basename(file).rsplit('.py', 1)[0])
                 module = __import__(module_name)
                 for comp in module_name.split(".")[1:]:
                     module = getattr(module, comp)
                 for name in module.__all__:
                     try:
                         d[name] = getattr(module, name)
                     except TypeError:
                         raise TypeError("Invalid type for name %s" % name)
 
         self.cli_shells = {}
         self.cli_job_interfaces = {}
+        self.active_cli_shells = {}
 
         module_prefix = self.__module__
-        module_prefix = join(*module_prefix.split("."))
-        module_path = abspath(join(getsourcefile(CliInterface), pardir))
-        code_dir = module_path.split(module_prefix)[0]
-        __load('%s/shell' % module_prefix, self.cli_shells, code_dir)
-        __load('%s/job' % module_prefix, self.cli_job_interfaces, code_dir)
+        __load('%s.shell' % module_prefix, self.cli_shells)
+        __load('%s.job' % module_prefix, self.cli_job_interfaces)
 
     def get_plugins(self, shell_params, job_params):
         """
         Return shell and job interface defined by and configured via
         specified params.
         """
         shell = self.get_shell_plugin(shell_params)
         job_interface = self.get_job_interface(job_params)
         return shell, job_interface
 
     def get_shell_plugin(self, shell_params):
         shell_plugin = shell_params.get('plugin', DEFAULT_SHELL_PLUGIN)
-        shell = self.cli_shells[shell_plugin](**shell_params)
-        return shell
+        requested_shell_settings = json.dumps(shell_params, sort_keys=True)
+        if requested_shell_settings not in self.active_cli_shells:
+            self.active_cli_shells[requested_shell_settings] = self.cli_shells[shell_plugin](**shell_params)
+        return self.active_cli_shells[requested_shell_settings]
 
     def get_job_interface(self, job_params):
         job_plugin = job_params.get('plugin', None)
         if not job_plugin:
             raise ValueError(ERROR_MESSAGE_NO_JOB_PLUGIN)
         job_plugin_class = self.cli_job_interfaces.get(job_plugin, None)
         if not job_plugin_class:
-            raise ValueError(ERROR_MESSAGE_NO_SUCH_JOB_PLUGIN % (job_plugin, self.cli_job_interfaces.keys()))
+            raise ValueError(ERROR_MESSAGE_NO_SUCH_JOB_PLUGIN % (job_plugin, list(self.cli_job_interfaces.keys())))
         job_interface = job_plugin_class(**job_params)
 
         return job_interface
 
 
 def split_params(params):
     shell_params = dict((k.replace('shell_', '', 1), v) for k, v in params.items() if k.startswith('shell_'))
```

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/cli/job/__init__.py` & `pulsar-app-0.9.1/pulsar/managers/util/cli/job/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """
 Abstract base class for cli job plugins.
 """
-from abc import ABCMeta, abstractmethod
+from abc import (
+    ABCMeta,
+    abstractmethod
+)
 
+import six
 
+
+@six.add_metaclass(ABCMeta)
 class BaseJobExec(object):
-    __metaclass__ = ABCMeta
 
     @abstractmethod
     def __init__(self, **params):
         """
         Constructor for CLI job executor.
         """
 
@@ -52,7 +57,19 @@
         """
 
     @abstractmethod
     def parse_single_status(self, status, job_id):
         """
         Parse the status of output from get_single_status command.
         """
+
+    def get_failure_reason(self, job_id):
+        """
+        Return the failure reason for the given job_id.
+        """
+        return None
+
+    def parse_failure_reason(self, reason, job_id):
+        """
+        Parses the failure reason, assigning it against a
+        """
+        return None
```

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/cli/job/slurm.py` & `pulsar-app-0.9.1/pulsar/managers/util/cli/job/slurm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # A simple CLI runner for slurm that can be used when running Galaxy from a
 # non-submit host and using a Slurm cluster.
-
-from ..job import BaseJobExec
-
 from logging import getLogger
 
 try:
     from galaxy.model import Job
     job_states = Job.states
 except ImportError:
     # Not in Galaxy, map Galaxy job states to Pulsar ones.
     from pulsar.util import enum
     job_states = enum(RUNNING='running', OK='complete', QUEUED='queued', ERROR="failed")
 
+from ..job import BaseJobExec
+
 log = getLogger(__name__)
 
 argmap = {
     'time': '-t',
     'ncpus': '-c',
     'partition': '-p'
 }
```

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/cli/job/slurm_torque.py` & `pulsar-app-0.9.1/pulsar/managers/util/cli/job/slurm_torque.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+
 from .torque import Torque
 
 __all__ = ('SlurmTorque',)
 
 
 class SlurmTorque(Torque):
     """ A CLI job executor for Slurm's Torque compatibility mode. This differs
```

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/cli/job/torque.py` & `pulsar-app-0.9.1/pulsar/managers/util/cli/job/torque.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 from ..job import BaseJobExec
 
 log = getLogger(__name__)
 
 ERROR_MESSAGE_UNRECOGNIZED_ARG = 'Unrecognized long argument passed to Torque CLI plugin: %s'
 
-
 argmap = {'destination': '-q',
           'Execution_Time': '-a',
           'Account_Name': '-A',
           'Checkpoint': '-c',
           'Error_Path': '-e',
           'Group_List': '-g',
           'Hold_Types': '-h',
```

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/cli/shell/local.py` & `pulsar-app-0.9.1/pulsar/managers/util/cli/shell/local.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,63 @@
+from logging import getLogger
+from subprocess import (
+    PIPE,
+    Popen
+)
 from tempfile import TemporaryFile
 from time import sleep
-from subprocess import Popen, PIPE
+
+import six
 
 from ..shell import BaseShellExec
-from ....util import Bunch, kill_pid
+from ....util import (
+    Bunch,
+    kill_pid
+)
 
-from logging import getLogger
 log = getLogger(__name__)
 
 TIMEOUT_ERROR_MESSAGE = u'Execution timed out'
 TIMEOUT_RETURN_CODE = -1
 DEFAULT_TIMEOUT = 60
 DEFAULT_TIMEOUT_CHECK_INTERVAL = 3
 
 
 class LocalShell(BaseShellExec):
     """
 
     >>> shell = LocalShell()
-    >>> def exec_python(script, **kwds): return shell.execute('python -c "%s"' % script, **kwds)
+    >>> def exec_python(script, **kwds): return shell.execute(['python', '-c', script], **kwds)
     >>> exec_result = exec_python("from __future__ import print_function; print('Hello World')")
     >>> exec_result.stderr == u''
     True
     >>> exec_result.stdout.strip() == u'Hello World'
     True
-    >>> exec_result = exec_python("import time; time.sleep(90)", timeout=.3, timeout_check_interval=.1)
+    >>> exec_result = exec_python("import time; time.sleep(90)", timeout=1, timeout_check_interval=.1)
     >>> exec_result.stdout == u''
     True
     >>> exec_result.stderr == 'Execution timed out'
     True
     >>> exec_result.returncode == TIMEOUT_RETURN_CODE
     True
+    >>> shell.execute('echo hi').stdout == "hi\\n"
+    True
     """
 
     def __init__(self, **kwds):
         pass
 
     def execute(self, cmd, persist=False, timeout=DEFAULT_TIMEOUT, timeout_check_interval=DEFAULT_TIMEOUT_CHECK_INTERVAL, **kwds):
+        is_cmd_string = isinstance(cmd, six.string_types)
         outf = TemporaryFile()
-        p = Popen(cmd, shell=True, stdin=None, stdout=outf, stderr=PIPE)
+        p = Popen(cmd, stdin=None, stdout=outf, stderr=PIPE, shell=is_cmd_string)
         # poll until timeout
 
         for i in range(int(timeout / timeout_check_interval)):
+            sleep(0.1)  # For fast returning commands
             r = p.poll()
             if r is not None:
                 break
             sleep(timeout_check_interval)
         else:
             kill_pid(p.pid)
             return Bunch(stdout=u'', stderr=TIMEOUT_ERROR_MESSAGE, returncode=TIMEOUT_RETURN_CODE)
```

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/condor/__init__.py` & `pulsar-app-0.9.1/pulsar/managers/util/condor/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 """
 Condor helper utilities.
 """
-from subprocess import Popen, PIPE, STDOUT, check_call, CalledProcessError
+from subprocess import (
+    CalledProcessError,
+    check_call,
+    PIPE,
+    Popen,
+    STDOUT
+)
+
 from ..external import parse_external_id
 
 DEFAULT_QUERY_CLASSAD = dict(
     universe='vanilla',
     getenv='true',
     notification='NEVER',
 )
```

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/drmaa/__init__.py` & `pulsar-app-0.9.1/pulsar/managers/util/drmaa/__init__.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/env.py` & `pulsar-app-0.9.1/pulsar/managers/util/env.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/external.py` & `pulsar-app-0.9.1/pulsar/managers/util/external.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/job_script/__init__.py` & `pulsar-app-0.9.1/pulsar/managers/util/job_script/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+import io
+import logging
 import os
 import subprocess
 import time
 from string import Template
 
 from pkg_resources import resource_string
-from six import text_type
 
 from galaxy.util import unicodify
 
+log = logging.getLogger(__name__)
 DEFAULT_SHELL = '/bin/bash'
 
 DEFAULT_JOB_FILE_TEMPLATE = Template(
-    resource_string(__name__, 'DEFAULT_JOB_FILE_TEMPLATE.sh').decode('UTF-8')
+    unicodify(resource_string(__name__, 'DEFAULT_JOB_FILE_TEMPLATE.sh'))
 )
 
 SLOTS_STATEMENT_CLUSTER_DEFAULT = \
-    resource_string(__name__, 'CLUSTER_SLOTS_STATEMENT.sh').decode('UTF-8')
+    unicodify(resource_string(__name__, 'CLUSTER_SLOTS_STATEMENT.sh'))
+
+MEMORY_STATEMENT_DEFAULT = \
+    unicodify(resource_string(__name__, 'MEMORY_STATEMENT.sh'))
 
 SLOTS_STATEMENT_SINGLE = """
 GALAXY_SLOTS="1"
 """
 
 INTEGRITY_INJECTION = """
 # The following block can be used by the job system
@@ -37,19 +42,21 @@
 REQUIRED_TEMPLATE_PARAMS = ['working_directory', 'command', 'exit_code_path']
 OPTIONAL_TEMPLATE_PARAMS = {
     'galaxy_lib': None,
     'galaxy_virtual_env': None,
     'headers': '',
     'env_setup_commands': [],
     'slots_statement': SLOTS_STATEMENT_CLUSTER_DEFAULT,
+    'memory_statement': MEMORY_STATEMENT_DEFAULT,
     'instrument_pre_commands': '',
     'instrument_post_commands': '',
     'integrity_injection': INTEGRITY_INJECTION,
     'shell': DEFAULT_SHELL,
     'preserve_python_environment': True,
+    'tmp_dir_creation_statement': '""',
 }
 
 
 def job_script(template=DEFAULT_JOB_FILE_TEMPLATE, **kwds):
     """
 
     >>> has_exception = False
@@ -68,14 +75,17 @@
     False
     >>> script = job_script(working_directory='wd', command='uptime', exit_code_path='ec', headers='#PBS -test')
     >>> script.startswith('#!/bin/bash\\n\\n#PBS -test\\n')
     True
     >>> script = job_script(working_directory='wd', command='uptime', exit_code_path='ec', slots_statement='GALAXY_SLOTS="$SLURM_JOB_NUM_NODES"')
     >>> script.find('GALAXY_SLOTS="$SLURM_JOB_NUM_NODES"\\nexport GALAXY_SLOTS\\n') > 0
     True
+    >>> script = job_script(working_directory='wd', command='uptime', exit_code_path='ec', memory_statement='GALAXY_MEMORY_MB="32768"')
+    >>> script.find('GALAXY_MEMORY_MB="32768"\\n') > 0
+    True
     """
     if any([param not in kwds for param in REQUIRED_TEMPLATE_PARAMS]):
         raise Exception("Failed to create job_script, a required parameter is missing.")
     job_instrumenter = kwds.get("job_instrumenter", None)
     if job_instrumenter:
         del kwds["job_instrumenter"]
         working_directory = kwds.get("metadata_directory", kwds["working_directory"])
@@ -98,52 +108,53 @@
 
 
 def write_script(path, contents, config, mode=0o755):
     dir = os.path.dirname(path)
     if not os.path.exists(dir):
         os.makedirs(dir)
 
-    with open(path, 'w') as f:
-        if isinstance(contents, text_type):
-            contents = contents.encode("UTF-8")
-        f.write(contents)
+    with io.open(path, 'w', encoding='utf-8') as f:
+        f.write(unicodify(contents))
     os.chmod(path, mode)
     _handle_script_integrity(path, config)
 
 
 def _handle_script_integrity(path, config):
     if not check_script_integrity(config):
         return
 
     script_integrity_verified = False
     count = getattr(config, "check_job_script_integrity_count", DEFAULT_INTEGRITY_COUNT)
     sleep_amt = getattr(config, "check_job_script_integrity_sleep", DEFAULT_INTEGRITY_SLEEP)
     for i in range(count):
         try:
-            proc = subprocess.Popen([path], shell=True, env={"ABC_TEST_JOB_SCRIPT_INTEGRITY_XYZ": "1"})
-            proc.wait()
-            if proc.returncode == 42:
+            returncode = subprocess.call([path], env={"ABC_TEST_JOB_SCRIPT_INTEGRITY_XYZ": "1"})
+            if returncode == 42:
                 script_integrity_verified = True
                 break
 
+            log.debug("Script integrity error for file '%s': returncode was %d", path, returncode)
+
             # Else we will sync and wait to see if the script becomes
             # executable.
             try:
                 # sync file system to avoid "Text file busy" problems.
                 # These have occurred both in Docker containers and on EC2 clusters
                 # under high load.
                 subprocess.check_call(INTEGRITY_SYNC_COMMAND)
-            except Exception:
-                pass
-            time.sleep(sleep_amt)
-        except Exception:
-            pass
+            except Exception as e:
+                log.debug("Error syncing the filesystem: %s", unicodify(e))
+
+        except Exception as exc:
+            log.debug("Script not available yet: %s", unicodify(exc))
+
+        time.sleep(sleep_amt)
 
     if not script_integrity_verified:
-        raise Exception("Failed to write job script, could not verify job script integrity.")
+        raise Exception("Failed to write job script '%s', could not verify job script integrity." % path)
 
 
 __all__ = (
     'check_script_integrity',
     'job_script',
     'write_script',
     'INTEGRITY_INJECTION',
```

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/job_script/CLUSTER_SLOTS_STATEMENT.sh` & `pulsar-app-0.9.1/pulsar/managers/util/job_script/CLUSTER_SLOTS_STATEMENT.sh`

 * *Files 11% similar despite different names*

```diff
@@ -19,11 +19,14 @@
     GALAXY_SLOTS="$NCPUS"
 elif [ -n "$PBS_NCPUS" ]; then
     GALAXY_SLOTS="$PBS_NCPUS"
 elif [ -f "$PBS_NODEFILE" ]; then
     GALAXY_SLOTS=`wc -l < $PBS_NODEFILE`
 elif [ -n "$LSB_DJOB_NUMPROC" ]; then
     GALAXY_SLOTS="$LSB_DJOB_NUMPROC"
+elif [ -n "$GALAXY_SLOTS" ]; then
+    # kubernetes runner injects GALAXY_SLOTS into environment
+    GALAXY_SLOTS=$GALAXY_SLOTS
 else
     GALAXY_SLOTS="1"
     unset GALAXY_SLOTS_CONFIGURED
 fi
```

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/kill.py` & `pulsar-app-0.9.1/pulsar/managers/util/kill.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
+import subprocess
 from platform import system
 from time import sleep
-from subprocess import Popen
 
 try:
-    from psutil import Process, NoSuchProcess
+    from psutil import NoSuchProcess, Process
 except ImportError:
     """ Don't make psutil a strict requirement, but use if available. """
     Process = None
 
 
 def kill_pid(pid, use_psutil=True):
     if use_psutil and Process:
@@ -37,16 +37,16 @@
         __kill_windows(pid)
     else:
         __kill_posix(pid)
 
 
 def __kill_windows(pid):
     try:
-        Popen("taskkill /F /T /PID %i" % pid, shell=True)
-    except Exception:
+        subprocess.check_call(['taskkill', '/F', '/T', '/PID', pid])
+    except subprocess.CalledProcessError:
         pass
 
 
 def __kill_posix(pid):
     def __check_pid():
         try:
             os.kill(pid, 0)
```

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/retry.py` & `pulsar-app-0.9.1/pulsar/managers/util/retry.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/managers/util/sudo.py` & `pulsar-app-0.9.1/pulsar/managers/util/sudo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import logging
-
-from subprocess import Popen, PIPE
+from subprocess import (
+    PIPE,
+    Popen
+)
 
 SUDO_PATH = '/usr/bin/sudo'
 SUDO_PRESERVE_ENVIRONMENT_ARG = '-E'
-SUDO_NON_INTERACTIVE_ARG = '-n'
 SUDO_USER_ARG = '-u'
 
 log = logging.getLogger(__name__)
 
 
 def sudo_popen(*args, **kwargs):
     """
     Helper method for building and executing Popen command. This is potentially
     sensetive code so should probably be centralized.
     """
     user = kwargs.get("user", None)
-    full_command = [SUDO_PATH, SUDO_PRESERVE_ENVIRONMENT_ARG, SUDO_NON_INTERACTIVE_ARG]
+    full_command = [SUDO_PATH, SUDO_PRESERVE_ENVIRONMENT_ARG]
     if user:
         full_command.extend([SUDO_USER_ARG, user])
     full_command.extend(args)
     log.info("About to execute the following sudo command - [%s]" % ' '.join(full_command))
     p = Popen(full_command, shell=False, stdout=PIPE, stderr=PIPE)
     return p
```

### Comparing `pulsar-app-0.9.0/pulsar/mesos/__init__.py` & `pulsar-app-0.9.1/pulsar/mesos/__init__.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/mesos/framework.py` & `pulsar-app-0.9.1/pulsar/mesos/framework.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/messaging/__init__.py` & `pulsar-app-0.9.1/pulsar/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/messaging/bind_amqp.py` & `pulsar-app-0.9.1/pulsar/messaging/bind_amqp.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/scripts/chown_working_directory.py` & `pulsar-app-0.9.1/pulsar/scripts/chown_working_directory.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/scripts/config.py` & `pulsar-app-0.9.1/pulsar/scripts/config.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/scripts/drmaa_kill.py` & `pulsar-app-0.9.1/pulsar/scripts/drmaa_kill.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/scripts/drmaa_launch.py` & `pulsar-app-0.9.1/pulsar/scripts/drmaa_launch.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/scripts/mesos_executor.py` & `pulsar-app-0.9.1/pulsar/scripts/mesos_executor.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/scripts/mesos_framework.py` & `pulsar-app-0.9.1/pulsar/scripts/mesos_framework.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/scripts/run.py` & `pulsar-app-0.9.1/pulsar/scripts/run.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/scripts/submit_util.py` & `pulsar-app-0.9.1/pulsar/scripts/submit_util.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/tools/authorization.py` & `pulsar-app-0.9.1/pulsar/tools/authorization.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/tools/toolbox.py` & `pulsar-app-0.9.1/pulsar/tools/toolbox.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/tools/validator.py` & `pulsar-app-0.9.1/pulsar/tools/validator.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/util/__init__.py` & `pulsar-app-0.9.1/pulsar/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/util/pastescript/loadwsgi.py` & `pulsar-app-0.9.1/pulsar/util/pastescript/loadwsgi.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/util/pastescript/serve.py` & `pulsar-app-0.9.1/pulsar/util/pastescript/serve.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/web/framework.py` & `pulsar-app-0.9.1/pulsar/web/framework.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/web/routes.py` & `pulsar-app-0.9.1/pulsar/web/routes.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar/web/wsgi.py` & `pulsar-app-0.9.1/pulsar/web/wsgi.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/pulsar_app.egg-info/PKG-INFO` & `pulsar-app-0.9.1/pulsar_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pulsar-app
-Version: 0.9.0
+Version: 0.9.1
 Summary: Distributed job execution application built for Galaxy (http://galaxyproject.org/).
 Home-page: https://github.com/galaxyproject/pulsar
 Author: Galaxy Project
 Author-email: jmchilton@gmail.com
 License: Apache License 2.0
 Description: .. figure:: https://galaxyproject.org/images/galaxy-logos/pulsar_transparent.png
            :alt: Pulsar Logo
@@ -109,14 +109,24 @@
         
         History
         -------
         
         .. to_doc
         
         ---------------------
+        0.9.1 (2019-05-01)
+        ---------------------
+        
+        * Fix duplicate inputs being a problem when staging Galaxy files.
+          `Pull Request 175`_
+        * Fix deprecated ``assertEquals()`` (thanks to @nsoranzo). `Pull Request 173`_
+        * Fix a method missing problem. `Pull Request 174`_
+        * Sync "recent" galaxy runner util changes. `Pull Request 177`_
+        
+        ---------------------
         0.9.0 (2019-04-12)
         ---------------------
             
         * Add configuration parameter to limit stream size read from disk. `Pull
           Request 157`_
         * Pass full job status for failed and lost jobs. `Pull Request 159`_
         * Improve message handling if problems occur during job setup/staging. `Pull
@@ -300,14 +310,18 @@
         ---------------------
         
         * See the original `announcement <http://dev.list.galaxyproject.org/New-Remote-Job-Runner-td4138951.html>`__
           and `initial commit <https://github.com/galaxyproject/pulsar/commit/163ed48d5a1902ceb84c38f10db8cbe5a0c1039d>`__.
         
         
         .. github_links
+        .. _Pull Request 173: https://github.com/galaxyproject/pulsar/pull/173
+        .. _Pull Request 174: https://github.com/galaxyproject/pulsar/pull/174
+        .. _Pull Request 175: https://github.com/galaxyproject/pulsar/pull/175
+        .. _Pull Request 177: https://github.com/galaxyproject/pulsar/pull/177
         .. _Pull Request 172: https://github.com/galaxyproject/pulsar/pull/172
         .. _Pull Request 170: https://github.com/galaxyproject/pulsar/pull/170
         .. _Pull Request 165: https://github.com/galaxyproject/pulsar/pull/165
         .. _Pull Request 164: https://github.com/galaxyproject/pulsar/pull/164
         .. _Pull Request 160: https://github.com/galaxyproject/pulsar/pull/160
         .. _Pull Request 159: https://github.com/galaxyproject/pulsar/pull/159
         .. _Pull Request 157: https://github.com/galaxyproject/pulsar/pull/157
```

### Comparing `pulsar-app-0.9.0/pulsar_app.egg-info/SOURCES.txt` & `pulsar-app-0.9.1/pulsar_app.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -66,24 +66,26 @@
 pulsar/managers/util/external.py
 pulsar/managers/util/kill.py
 pulsar/managers/util/retry.py
 pulsar/managers/util/sudo.py
 pulsar/managers/util/cli/__init__.py
 pulsar/managers/util/cli/factory.py
 pulsar/managers/util/cli/job/__init__.py
+pulsar/managers/util/cli/job/lsf.py
 pulsar/managers/util/cli/job/slurm.py
 pulsar/managers/util/cli/job/slurm_torque.py
 pulsar/managers/util/cli/job/torque.py
 pulsar/managers/util/cli/shell/__init__.py
 pulsar/managers/util/cli/shell/local.py
 pulsar/managers/util/cli/shell/rsh.py
 pulsar/managers/util/condor/__init__.py
 pulsar/managers/util/drmaa/__init__.py
 pulsar/managers/util/job_script/CLUSTER_SLOTS_STATEMENT.sh
 pulsar/managers/util/job_script/DEFAULT_JOB_FILE_TEMPLATE.sh
+pulsar/managers/util/job_script/MEMORY_STATEMENT.sh
 pulsar/managers/util/job_script/__init__.py
 pulsar/mesos/__init__.py
 pulsar/mesos/framework.py
 pulsar/messaging/__init__.py
 pulsar/messaging/bind_amqp.py
 pulsar/scripts/__init__.py
 pulsar/scripts/bootstrap.py
```

### Comparing `pulsar-app-0.9.0/README.rst` & `pulsar-app-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/scripts/pulsar` & `pulsar-app-0.9.1/scripts/pulsar`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/setup.py` & `pulsar-app-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `pulsar-app-0.9.0/test/test_utils.py` & `pulsar-app-0.9.1/test/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -167,19 +167,19 @@
     @nottest
     def _test_simple_execution(self, manager):
         command = """python -c "import sys; sys.stdout.write(\'Hello World!\'); sys.stderr.write(\'moo\')" """
         job_id = manager.setup_job("123", "tool1", "1.0.0")
         manager.launch(job_id, command)
         while manager.get_status(job_id) not in ['complete', 'cancelled']:
             pass
-        self.assertEquals(manager.stderr_contents(job_id), b'moo')
-        self.assertEquals(manager.stdout_contents(job_id), b'Hello World!')
-        self.assertEquals(manager.return_code(job_id), 0)
+        self.assertEqual(manager.stderr_contents(job_id), b'moo')
+        self.assertEqual(manager.stdout_contents(job_id), b'Hello World!')
+        self.assertEqual(manager.return_code(job_id), 0)
         manager.clean(job_id)
-        self.assertEquals(len(listdir(self.staging_directory)), 0)
+        self.assertEqual(len(listdir(self.staging_directory)), 0)
 
     def _test_cancelling(self, manager):
         job_id = manager.setup_job("124", "tool1", "1.0.0")
         command = self._python_to_command("import time; time.sleep(1000)")
         manager.launch(job_id, command)
         time.sleep(0.05)
         manager.kill(job_id)
@@ -425,16 +425,18 @@
 
     def get_authorization(self, tool_id):
         return self.authorization
 
 
 class JobFilesApp(object):
 
-    def __init__(self, root_directory=None):
+    def __init__(self, root_directory=None, allow_multiple_downloads=False):
         self.root_directory = root_directory
+        self.served_files = []
+        self.allow_multiple_downloads = allow_multiple_downloads
 
     def __call__(self, environ, start_response):
         req = webob.Request(environ)
         params = req.params.mixed()
         method = req.method
         if method == "POST":
             resp = self._post(req, params)
@@ -452,28 +454,31 @@
         if not exists(parent_directory):
             makedirs(parent_directory)
         pulsar.util.copy_to_path(params["file"].file, path)
         return webob.Response(body='')
 
     def _get(self, request, params):
         path = params['path']
+        if path in self.served_files and not self.allow_multiple_downloads:  # emulate Galaxy not allowing the same request twice...
+            raise Exception("Same file copied multiple times...")
         if not galaxy.util.in_directory(path, self.root_directory):
             assert False, "%s not in %s" % (path, self.root_directory)
+        self.served_files.append(path)
         return file_response(path)
 
 
 @contextmanager
-def files_server(directory=None):
+def files_server(directory=None, allow_multiple_downloads=False):
     if not directory:
         with temp_directory() as directory:
-            app = TestApp(JobFilesApp(directory))
+            app = TestApp(JobFilesApp(directory, allow_multiple_downloads=allow_multiple_downloads))
             with server_for_test_app(app) as server:
                 yield server, directory
     else:
-        app = TestApp(JobFilesApp(directory))
+        app = TestApp(JobFilesApp(directory, allow_multiple_downloads=allow_multiple_downloads))
         with server_for_test_app(app) as server:
             yield server
 
 
 def dump_other_threads():
     # Utility for debugging threads that aren't dying during
     # tests.
```

