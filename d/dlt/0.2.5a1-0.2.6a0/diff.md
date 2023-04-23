# Comparing `tmp/dlt-0.2.5a1.tar.gz` & `tmp/dlt-0.2.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.2.5a1.tar", max compression
+gzip compressed data, was "dlt-0.2.6a0.tar", max compression
```

## Comparing `dlt-0.2.5a1.tar` & `dlt-0.2.6a0.tar`

### file list

```diff
@@ -1,202 +1,204 @@
--rw-r--r--   0        0        0    11343 2023-04-06 15:20:13.865351 dlt-0.2.5a1/LICENSE.txt
--rw-r--r--   0        0        0     5277 2023-04-13 12:36:14.969762 dlt-0.2.5a1/README.md
--rw-r--r--   0        0        0     1661 2023-04-12 17:10:39.598778 dlt-0.2.5a1/dlt/__init__.py
--rw-r--r--   0        0        0       31 2023-04-06 15:20:13.866512 dlt-0.2.5a1/dlt/cli/__init__.py
--rw-r--r--   0        0        0    13282 2023-04-06 15:20:13.866661 dlt-0.2.5a1/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3653 2023-04-06 15:20:13.866767 dlt-0.2.5a1/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    16662 2023-04-06 15:20:13.866947 dlt-0.2.5a1/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0     1683 2023-04-06 15:20:13.867073 dlt-0.2.5a1/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-04-06 15:20:13.867191 dlt-0.2.5a1/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    18888 2023-04-13 13:06:57.962424 dlt-0.2.5a1/dlt/cli/init_command.py
--rw-r--r--   0        0        0     6255 2023-04-06 15:20:13.867536 dlt-0.2.5a1/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9419 2023-04-06 15:20:13.867687 dlt-0.2.5a1/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     4404 2023-04-06 15:20:13.867805 dlt-0.2.5a1/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1776 2023-04-06 15:20:13.867916 dlt-0.2.5a1/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0      106 2023-04-06 15:20:13.868003 dlt-0.2.5a1/dlt/cli/typing.py
--rw-r--r--   0        0        0     3662 2023-04-06 15:20:13.868104 dlt-0.2.5a1/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-04-06 15:20:13.868241 dlt-0.2.5a1/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2023-04-06 15:20:13.868339 dlt-0.2.5a1/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      428 2023-04-06 15:20:13.868485 dlt-0.2.5a1/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     4898 2023-04-06 15:20:13.868600 dlt-0.2.5a1/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3448 2023-04-06 15:20:13.868721 dlt-0.2.5a1/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     5884 2023-04-06 15:20:13.868843 dlt-0.2.5a1/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7773 2023-04-11 19:17:13.136572 dlt-0.2.5a1/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1198 2023-04-06 15:20:13.869116 dlt-0.2.5a1/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      252 2023-04-06 15:20:13.869256 dlt-0.2.5a1/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0     1089 2023-04-06 15:20:13.869358 dlt-0.2.5a1/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1193 2023-04-06 15:20:13.869462 dlt-0.2.5a1/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     2050 2023-04-06 15:20:13.869570 dlt-0.2.5a1/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0      758 2023-04-06 15:20:13.869667 dlt-0.2.5a1/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0     4922 2023-04-11 20:01:32.767153 dlt-0.2.5a1/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    18084 2023-04-12 15:12:05.711413 dlt-0.2.5a1/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0      815 2023-04-06 15:20:13.870177 dlt-0.2.5a1/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0    10914 2023-04-11 19:17:13.137158 dlt-0.2.5a1/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     1854 2023-04-06 15:20:13.870453 dlt-0.2.5a1/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     2792 2023-04-06 15:20:13.870561 dlt-0.2.5a1/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     1124 2023-04-06 15:20:13.870700 dlt-0.2.5a1/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0     3047 2023-04-06 15:20:13.870845 dlt-0.2.5a1/dlt/common/configuration/specs/gcp_client_credentials.py
--rw-r--r--   0        0        0      665 2023-04-06 15:20:13.870968 dlt-0.2.5a1/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0      556 2023-04-06 15:20:13.871124 dlt-0.2.5a1/dlt/common/configuration/specs/load_volume_configuration.py
--rw-r--r--   0        0        0      417 2023-04-06 15:20:13.871244 dlt-0.2.5a1/dlt/common/configuration/specs/normalize_volume_configuration.py
--rw-r--r--   0        0        0     2769 2023-04-06 15:20:13.871358 dlt-0.2.5a1/dlt/common/configuration/specs/postgres_credentials.py
--rw-r--r--   0        0        0     2532 2023-04-06 15:20:13.871468 dlt-0.2.5a1/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0      944 2023-04-06 15:20:13.871570 dlt-0.2.5a1/dlt/common/configuration/specs/schema_volume_configuration.py
--rw-r--r--   0        0        0     5339 2023-04-06 15:20:13.871785 dlt-0.2.5a1/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-04-06 15:20:13.871968 dlt-0.2.5a1/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-04-06 15:20:13.872137 dlt-0.2.5a1/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-04-06 15:20:13.872251 dlt-0.2.5a1/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-04-06 15:20:13.872403 dlt-0.2.5a1/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     5893 2023-04-06 15:20:13.872525 dlt-0.2.5a1/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2395 2023-04-06 15:20:13.872641 dlt-0.2.5a1/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-04-06 15:20:13.872732 dlt-0.2.5a1/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     5159 2023-04-06 15:20:13.872876 dlt-0.2.5a1/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0       97 2023-04-06 15:20:13.873047 dlt-0.2.5a1/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     2206 2023-04-06 15:20:13.873165 dlt-0.2.5a1/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    10682 2023-04-11 19:17:13.137365 dlt-0.2.5a1/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6439 2023-04-11 19:17:13.137531 dlt-0.2.5a1/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-04-06 15:20:13.873598 dlt-0.2.5a1/dlt/common/git.py
--rw-r--r--   0        0        0     5248 2023-04-11 19:17:13.137693 dlt-0.2.5a1/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-04-11 19:17:13.137836 dlt-0.2.5a1/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-04-11 19:17:13.138015 dlt-0.2.5a1/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0      232 2023-04-06 15:20:13.874188 dlt-0.2.5a1/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1210 2023-04-06 15:20:13.874288 dlt-0.2.5a1/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-04-06 15:20:13.874377 dlt-0.2.5a1/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-04-11 19:17:13.138171 dlt-0.2.5a1/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13396 2023-04-11 19:17:13.138353 dlt-0.2.5a1/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-04-06 15:20:13.874875 dlt-0.2.5a1/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-04-06 15:20:13.875007 dlt-0.2.5a1/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-04-06 15:20:13.875132 dlt-0.2.5a1/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-04-06 15:20:13.875231 dlt-0.2.5a1/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-04-06 15:20:13.875343 dlt-0.2.5a1/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-04-06 15:20:13.875460 dlt-0.2.5a1/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-04-06 15:20:13.875554 dlt-0.2.5a1/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-04-11 19:17:13.138502 dlt-0.2.5a1/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-04-06 15:20:13.875758 dlt-0.2.5a1/dlt/common/pendulum.py
--rw-r--r--   0        0        0    14410 2023-04-12 15:12:05.711649 dlt-0.2.5a1/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-04-06 15:20:13.876032 dlt-0.2.5a1/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-04-06 15:20:13.876156 dlt-0.2.5a1/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-04-11 19:17:13.138862 dlt-0.2.5a1/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5117 2023-04-06 15:20:13.876379 dlt-0.2.5a1/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      210 2023-04-06 15:20:13.876517 dlt-0.2.5a1/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0     1079 2023-04-06 15:20:13.876626 dlt-0.2.5a1/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0      939 2023-04-06 15:20:13.876720 dlt-0.2.5a1/dlt/common/runners/init.py
--rw-r--r--   0        0        0     7832 2023-04-06 15:20:13.876921 dlt-0.2.5a1/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-04-06 15:20:13.877077 dlt-0.2.5a1/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-04-06 15:20:13.877194 dlt-0.2.5a1/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-04-06 15:20:13.877453 dlt-0.2.5a1/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      583 2023-04-06 15:20:13.877558 dlt-0.2.5a1/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5250 2023-04-06 15:20:13.877675 dlt-0.2.5a1/dlt/common/runners/venv.py
--rw-r--r--   0        0        0        0 2023-04-06 15:20:13.877784 dlt-0.2.5a1/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0     3828 2023-04-06 15:20:13.877913 dlt-0.2.5a1/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0     6320 2023-04-06 15:20:13.878085 dlt-0.2.5a1/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2026 2023-04-06 15:20:13.878281 dlt-0.2.5a1/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     6554 2023-04-06 15:20:13.878421 dlt-0.2.5a1/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2479 2023-04-06 15:20:13.878523 dlt-0.2.5a1/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     1943 2023-04-06 15:20:13.878627 dlt-0.2.5a1/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-04-06 15:20:13.878735 dlt-0.2.5a1/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0      989 2023-04-06 15:20:13.878839 dlt-0.2.5a1/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-04-06 15:20:13.878980 dlt-0.2.5a1/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-04-06 15:20:13.879100 dlt-0.2.5a1/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-04-06 15:20:13.879229 dlt-0.2.5a1/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25175 2023-04-11 19:17:13.139202 dlt-0.2.5a1/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     2976 2023-04-06 15:20:13.879636 dlt-0.2.5a1/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    21530 2023-04-12 15:12:05.712017 dlt-0.2.5a1/dlt/common/schema/utils.py
--rw-r--r--   0        0        0      410 2023-04-06 15:20:13.880044 dlt-0.2.5a1/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1906 2023-04-06 15:20:13.880173 dlt-0.2.5a1/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     2804 2023-04-06 15:20:13.880285 dlt-0.2.5a1/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0     9059 2023-04-06 15:20:13.880432 dlt-0.2.5a1/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2685 2023-04-12 15:12:05.712222 dlt-0.2.5a1/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21684 2023-04-06 15:20:13.880777 dlt-0.2.5a1/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2414 2023-04-06 15:20:13.880947 dlt-0.2.5a1/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8508 2023-04-06 15:20:13.881095 dlt-0.2.5a1/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     2465 2023-04-06 15:20:13.881225 dlt-0.2.5a1/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2677 2023-04-06 15:20:13.881365 dlt-0.2.5a1/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-04-06 15:20:13.881494 dlt-0.2.5a1/dlt/common/typing.py
--rw-r--r--   0        0        0    10588 2023-04-11 19:17:13.139619 dlt-0.2.5a1/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-04-06 15:20:13.881847 dlt-0.2.5a1/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-04-06 15:20:13.882015 dlt-0.2.5a1/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-04-06 15:20:13.882122 dlt-0.2.5a1/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-04-06 15:20:13.882326 dlt-0.2.5a1/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     1813 2023-04-06 15:20:13.882430 dlt-0.2.5a1/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    12301 2023-04-11 19:17:13.139861 dlt-0.2.5a1/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0      392 2023-04-06 15:20:13.882780 dlt-0.2.5a1/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10169 2023-04-06 15:20:13.882921 dlt-0.2.5a1/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     1935 2023-04-06 15:20:13.883076 dlt-0.2.5a1/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     5503 2023-04-06 15:20:13.883187 dlt-0.2.5a1/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     2754 2023-04-06 15:20:13.883437 dlt-0.2.5a1/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6936 2023-04-06 15:20:13.883566 dlt-0.2.5a1/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1671 2023-04-06 15:20:13.883757 dlt-0.2.5a1/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-04-06 15:20:13.883867 dlt-0.2.5a1/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4975 2023-04-06 15:20:13.883996 dlt-0.2.5a1/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4159 2023-04-06 15:20:13.884122 dlt-0.2.5a1/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     4983 2023-04-06 15:20:13.884272 dlt-0.2.5a1/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    14398 2023-04-11 19:17:13.140063 dlt-0.2.5a1/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     1303 2023-04-06 15:20:13.884546 dlt-0.2.5a1/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0      251 2023-04-06 15:20:13.884710 dlt-0.2.5a1/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     1934 2023-04-06 15:20:13.884806 dlt-0.2.5a1/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0      443 2023-04-06 15:20:13.884893 dlt-0.2.5a1/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     3025 2023-04-06 15:20:13.884988 dlt-0.2.5a1/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     6066 2023-04-12 15:12:05.712412 dlt-0.2.5a1/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-04-06 15:20:13.885239 dlt-0.2.5a1/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     1905 2023-04-06 15:20:13.885340 dlt-0.2.5a1/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      405 2023-04-06 15:20:13.885474 dlt-0.2.5a1/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     3761 2023-04-06 15:20:13.885590 dlt-0.2.5a1/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     6850 2023-04-06 15:20:13.885722 dlt-0.2.5a1/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    10101 2023-04-11 19:17:13.140321 dlt-0.2.5a1/dlt/destinations/sql_merge_job.py
--rw-r--r--   0        0        0     1933 2023-04-06 15:20:13.885947 dlt-0.2.5a1/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2023-04-06 15:20:13.886049 dlt-0.2.5a1/dlt/extract/__init__.py
--rw-r--r--   0        0        0    22227 2023-04-11 19:17:13.140593 dlt-0.2.5a1/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12183 2023-04-11 19:17:13.140877 dlt-0.2.5a1/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     7654 2023-04-12 15:12:05.712637 dlt-0.2.5a1/dlt/extract/extract.py
--rw-r--r--   0        0        0    13689 2023-04-12 15:12:05.712864 dlt-0.2.5a1/dlt/extract/incremental.py
--rw-r--r--   0        0        0    31421 2023-04-12 15:12:05.713134 dlt-0.2.5a1/dlt/extract/pipe.py
--rw-r--r--   0        0        0     8210 2023-04-12 15:12:05.713430 dlt-0.2.5a1/dlt/extract/schema.py
--rw-r--r--   0        0        0    30388 2023-04-12 15:12:05.713696 dlt-0.2.5a1/dlt/extract/source.py
--rw-r--r--   0        0        0     4781 2023-04-12 15:12:05.713893 dlt-0.2.5a1/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-04-06 15:20:13.887409 dlt-0.2.5a1/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2023-04-06 15:20:13.887511 dlt-0.2.5a1/dlt/helpers/__init__.py
--rw-r--r--   0        0        0      842 2023-04-06 15:20:13.887654 dlt-0.2.5a1/dlt/helpers/dbt/README.md
--rw-r--r--   0        0        0     2907 2023-04-06 15:20:13.887756 dlt-0.2.5a1/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-04-06 15:20:13.887882 dlt-0.2.5a1/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6137 2023-04-06 15:20:13.888012 dlt-0.2.5a1/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-04-06 15:20:13.888126 dlt-0.2.5a1/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     3583 2023-04-06 15:20:13.888232 dlt-0.2.5a1/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    14293 2023-04-06 15:20:13.888399 dlt-0.2.5a1/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2373 2023-04-06 15:20:13.888508 dlt-0.2.5a1/dlt/helpers/pandas.py
--rw-r--r--   0        0        0     1035 2023-04-06 15:20:13.888600 dlt-0.2.5a1/dlt/helpers/parquet.py
--rw-r--r--   0        0        0    12920 2023-04-13 13:08:09.451202 dlt-0.2.5a1/dlt/helpers/streamlit.py
--rw-r--r--   0        0        0       31 2023-04-06 15:20:13.888885 dlt-0.2.5a1/dlt/load/__init__.py
--rw-r--r--   0        0        0     1103 2023-04-06 15:20:13.889003 dlt-0.2.5a1/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-04-06 15:20:13.889110 dlt-0.2.5a1/dlt/load/exceptions.py
--rw-r--r--   0        0        0    20447 2023-04-06 15:20:13.889323 dlt-0.2.5a1/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-04-06 15:20:13.889485 dlt-0.2.5a1/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1182 2023-04-06 15:20:13.889573 dlt-0.2.5a1/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2023-04-06 15:20:13.889615 dlt-0.2.5a1/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    17989 2023-04-11 19:17:13.142942 dlt-0.2.5a1/dlt/normalize/normalize.py
--rw-r--r--   0        0        0     1880 2023-04-06 15:20:13.889985 dlt-0.2.5a1/dlt/pipeline/README.md
--rw-r--r--   0        0        0    12224 2023-04-12 15:12:05.714087 dlt-0.2.5a1/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     1823 2023-04-06 15:20:13.890499 dlt-0.2.5a1/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      342 2023-04-06 15:20:13.890615 dlt-0.2.5a1/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-04-06 15:20:13.890730 dlt-0.2.5a1/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     2537 2023-04-06 15:20:13.890828 dlt-0.2.5a1/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     1497 2023-04-06 15:20:13.890922 dlt-0.2.5a1/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-04-11 19:17:13.143161 dlt-0.2.5a1/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    58159 2023-04-13 12:59:16.401972 dlt-0.2.5a1/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0     4200 2023-04-11 19:17:13.143762 dlt-0.2.5a1/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     7990 2023-04-06 15:20:13.891660 dlt-0.2.5a1/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     4563 2023-04-06 15:20:13.891788 dlt-0.2.5a1/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-04-06 15:20:13.891882 dlt-0.2.5a1/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2023-04-06 15:20:13.891929 dlt-0.2.5a1/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-04-06 15:20:13.892040 dlt-0.2.5a1/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-04-06 15:20:13.892137 dlt-0.2.5a1/dlt/reflection/names.py
--rw-r--r--   0        0        0     4805 2023-04-06 15:20:13.892251 dlt-0.2.5a1/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-04-06 15:20:13.892405 dlt-0.2.5a1/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      118 2023-04-11 19:17:13.143908 dlt-0.2.5a1/dlt/sources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 15:20:13.892603 dlt-0.2.5a1/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      574 2023-04-06 15:20:13.892755 dlt-0.2.5a1/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0     9089 2023-04-06 15:20:13.892883 dlt-0.2.5a1/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1336 2023-04-06 15:20:13.892983 dlt-0.2.5a1/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      679 2023-04-11 19:17:13.144029 dlt-0.2.5a1/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-04-13 13:00:28.813120 dlt-0.2.5a1/dlt/version.py
--rw-r--r--   0        0        0     3716 2023-04-13 13:03:11.818599 dlt-0.2.5a1/pyproject.toml
--rw-r--r--   0        0        0     8423 1970-01-01 00:00:00.000000 dlt-0.2.5a1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.2.6a0/LICENSE.txt
+-rw-r--r--   0        0        0     5264 2023-04-22 20:26:30.632198 dlt-0.2.6a0/README.md
+-rw-r--r--   0        0        0     1677 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/__init__.py
+-rw-r--r--   0        0        0       31 2023-03-03 14:20:21.286564 dlt-0.2.6a0/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    13282 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3653 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    16663 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0     1683 2023-03-26 19:01:53.563115 dlt-0.2.6a0/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18888 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/cli/init_command.py
+-rw-r--r--   0        0        0     6255 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9419 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4404 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0      106 2023-03-03 14:20:18.076564 dlt-0.2.6a0/dlt/cli/typing.py
+-rw-r--r--   0        0        0     3662 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.2.6a0/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      428 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     4898 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3448 2023-04-05 15:15:49.779453 dlt-0.2.6a0/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     5884 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1198 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      252 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0     1108 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1089 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1193 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     2050 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0      758 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0     5320 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    18084 2023-04-22 20:22:19.252199 dlt-0.2.6a0/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0      868 2023-04-23 12:08:49.194852 dlt-0.2.6a0/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1679 2023-04-23 12:08:49.194852 dlt-0.2.6a0/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0    10914 2023-04-09 16:39:04.593180 dlt-0.2.6a0/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     3190 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     2792 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     2125 2023-04-23 12:08:49.194852 dlt-0.2.6a0/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12020 2023-04-23 12:08:49.194852 dlt-0.2.6a0/dlt/common/configuration/specs/gcp_client_credentials.py
+-rw-r--r--   0        0        0      665 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0      556 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/specs/load_volume_configuration.py
+-rw-r--r--   0        0        0      417 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/specs/normalize_volume_configuration.py
+-rw-r--r--   0        0        0     2769 2023-04-06 08:59:11.959561 dlt-0.2.6a0/dlt/common/configuration/specs/postgres_credentials.py
+-rw-r--r--   0        0        0     2532 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0      944 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/specs/schema_volume_configuration.py
+-rw-r--r--   0        0        0     5339 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.2.6a0/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     5893 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2395 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0       97 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    10682 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6439 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/git.py
+-rw-r--r--   0        0        0     5248 2023-04-10 08:12:53.759595 dlt-0.2.6a0/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.2.6a0/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.2.6a0/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1210 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.2.6a0/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13396 2023-04-06 15:27:24.759561 dlt-0.2.6a0/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.2.6a0/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.2.6a0/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    14901 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.2.6a0/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-04-23 12:08:49.194852 dlt-0.2.6a0/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      210 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0     1079 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0      939 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/init.py
+-rw-r--r--   0        0        0     7832 2023-04-03 13:25:54.449156 dlt-0.2.6a0/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      583 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5250 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0     3828 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0     6320 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2026 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7170 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2479 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     1943 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0      989 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25175 2023-04-09 16:39:04.593180 dlt-0.2.6a0/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    21954 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0      410 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     2804 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0     9059 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2685 2023-04-13 08:33:43.967587 dlt-0.2.6a0/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21684 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2414 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8508 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     2525 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2677 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/common/typing.py
+-rw-r--r--   0        0        0    11275 2023-04-23 12:08:49.204852 dlt-0.2.6a0/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    12301 2023-04-06 15:27:24.759561 dlt-0.2.6a0/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0      392 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10123 2023-04-23 12:08:49.204852 dlt-0.2.6a0/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     6964 2023-04-23 18:00:31.976853 dlt-0.2.6a0/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.2.6a0/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4975 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     4983 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    14398 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0      443 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     6066 2023-04-13 08:33:43.967587 dlt-0.2.6a0/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      405 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     6850 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    10101 2023-04-09 16:39:04.593180 dlt-0.2.6a0/dlt/destinations/sql_merge_job.py
+-rw-r--r--   0        0        0     1931 2023-04-23 12:08:49.204852 dlt-0.2.6a0/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.6a0/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    22569 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12184 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     7654 2023-04-16 18:26:08.732459 dlt-0.2.6a0/dlt/extract/extract.py
+-rw-r--r--   0        0        0    14541 2023-04-23 12:24:07.664852 dlt-0.2.6a0/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    31380 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9683 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/extract/schema.py
+-rw-r--r--   0        0        0    31994 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/extract/source.py
+-rw-r--r--   0        0        0     4350 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.2.6a0/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.2.6a0/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    14293 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2373 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/helpers/pandas.py
+-rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/helpers/parquet.py
+-rw-r--r--   0        0        0    13039 2023-04-23 12:23:38.014852 dlt-0.2.6a0/dlt/helpers/streamlit.py
+-rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1103 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    20447 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1182 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.6a0/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    17989 2023-04-13 12:56:33.587587 dlt-0.2.6a0/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0     1880 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/pipeline/README.md
+-rw-r--r--   0        0        0    12224 2023-04-13 08:33:43.967587 dlt-0.2.6a0/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     1823 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      363 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     2537 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     1497 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.2.6a0/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    58298 2023-04-23 13:33:49.844852 dlt-0.2.6a0/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0     4200 2023-04-10 08:12:53.769595 dlt-0.2.6a0/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.2.6a0/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     4563 2023-04-03 18:50:36.903525 dlt-0.2.6a0/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.2.6a0/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/reflection/names.py
+-rw-r--r--   0        0        0     4986 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      118 2023-04-06 15:27:24.759561 dlt-0.2.6a0/dlt/sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.2.6a0/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0     9092 2023-04-23 12:08:49.204852 dlt-0.2.6a0/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.2.6a0/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/version.py
+-rw-r--r--   0        0        0     3893 2023-04-23 18:00:31.976853 dlt-0.2.6a0/pyproject.toml
+-rw-r--r--   0        0        0     8483 1970-01-01 00:00:00.000000 dlt-0.2.6a0/setup.py
+-rw-r--r--   0        0        0     8409 1970-01-01 00:00:00.000000 dlt-0.2.6a0/PKG-INFO
```

### Comparing `dlt-0.2.5a1/LICENSE.txt` & `dlt-0.2.6a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/README.md` & `dlt-0.2.6a0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,104 @@
 ![](https://github.com/dlt-hub/dlt/raw/devel/docs/DLT-Pacman-Big.gif)
 
 <p align="center">
 
-[![PyPI version](https://badge.fury.io/py/python-dlt.svg)](https://pypi.org/project/python-dlt/)
+[![PyPI version](https://badge.fury.io/py/dlt.svg)](https://pypi.org/project/dlt/)
 [![LINT Badge](https://github.com/dlt-hub/dlt/actions/workflows/lint.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/lint.yml)
 [![TEST COMMON Badge](https://github.com/dlt-hub/dlt/actions/workflows/test_common.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/test_common.yml)
 [![TEST DESTINATIONS Badge](https://github.com/dlt-hub/dlt/actions/workflows/test_destinations.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/test_destinations.yml)
 [![TEST BIGQUERY Badge](https://github.com/dlt-hub/dlt/actions/workflows/test_destination_bigquery.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/test_destination_bigquery.yml)
 [![TEST DBT Badge](https://github.com/dlt-hub/dlt/actions/workflows/test_dbt_runner.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/test_dbt_runner.yml)
 
-
 </p>
 
 # data load tool (dlt)
 
-**[Colab Demo](https://colab.research.google.com/drive/1BXvma_9R9MX8p_iSvHE4ebg90sUroty2)**
+**[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**
 
 ```python
 import dlt
 from chess import chess # a utility function that grabs data from the chess.com API
 
 # create a dlt pipeline that will load chess game data to the DuckDB destination
-pipeline = dlt.pipeline(pipeline_name="chess_pipeline", destination='duckdb', dataset_name="games_data")
+pipeline = dlt.pipeline(
+    pipeline_name='chess_pipeline',
+    destination='duckdb',
+    dataset_name='games_data'
+)
 
 # use chess.com API to grab data about a few players
-data = chess(['magnuscarlsen', 'rpragchess'], start_month="2022/11", end_month="2022/12")
+data = chess(['magnuscarlsen', 'rpragchess'], start_month='2022/11', end_month='2022/12')
 
 # extract, normalize, and load the data
 pipeline.run(data)
 ```
 
-**data load tool (dlt)** is a simple, open source Python library that makes data loading easy
+**data load tool (dlt)** is an open source Python library that makes data loading easy
+
 - Automatically turn the JSON returned by any API into a live dataset stored wherever you want it
-- `pip install python-dlt` and then include `import dlt` to use it in your Python loading script
+- `pip install dlt` and then include `import dlt` to use it in your Python loading script
 - The **dlt** library is licensed under the Apache License 2.0, so you can use it for free forever
 
 Read more about it on the [dlt Docs](https://dlthub.com/docs)
 
 # semantic versioning
-`python-dlt` will follow the semantic versioning with [`MAJOR.MINOR.PATCH`](https://peps.python.org/pep-0440/#semantic-versioning) pattern. Currently we do **pre-release versioning** with major version being 0.
+
+`dlt` will follow the semantic versioning with [`MAJOR.MINOR.PATCH`](https://peps.python.org/pep-0440/#semantic-versioning) pattern. Currently we do **pre-release versioning** with major version being 0.
+
 - `minor` version change means breaking changes
 - `patch` version change means new features that should be backward compatible
 - any suffix change ie. `a10` -> `a11` is a patch
 
 # development
-`python-dlt` uses `poetry` to manage, build and version the package. It also uses `make` to automate tasks. To start
+
+`dlt` uses `poetry` to manage, build and version the package. It also uses `make` to automate tasks. To start
+
 ```sh
 make install-poetry  # will install poetry, to be run outside virtualenv
 ```
+
 then
+
 ```sh
 make dev  # will install all deps including dev
 ```
+
 Executing `poetry shell` and working in it is very convenient at this moment.
 
 ## python version
-Use python 3.8 for development which is the lowest supported version for `python-dlt`. You'll need `distutils` and `venv`:
+
+Use python 3.8 for development which is the lowest supported version for `dlt`. You'll need `distutils` and `venv`:
 
 ```shell
 sudo apt-get install python3.8
 sudo apt-get install python3.8-distutils
 sudo apt install python3.8-venv
 ```
+
 You may also use `pyenv` as [poetry](https://python-poetry.org/docs/managing-environments/) suggests.
 
 ## bumping version
+
 Please use `poetry version prerelease` to bump patch and then `make build-library` to apply changes. The source of the version is `pyproject.toml` and we use poetry to manage it.
 
 ## testing and linting
-`python-dlt` uses `mypy` and `flake8` with several plugins for linting. We do not reorder imports or reformat code.
+
+`dlt` uses `mypy` and `flake8` with several plugins for linting. We do not reorder imports or reformat code.
 
 `pytest` is used as test harness. `make test-common` will run tests of common components and does not require any external resources.
 
 ### testing destinations
+
 To test destinations use `make test`. You will need following external resources
+
 1. `BigQuery` project
 2. `Redshift` cluster
 3. `Postgres` instance. You can find a docker compose for postgres instance [here](tests/load/postgres/docker-compose.yml). When run the instance is configured to work with the tests.
+
 ```shell
 cd tests/load/postgres/
 docker-compose up --build -d
 ```
 
 See `tests/.example.env` for the expected environment variables and command line example to run the tests. Then create `tests/.env` from it. You configure the tests as you would configure the dlt pipeline.
 We'll provide you with access to the resources above if you wish to test locally.
@@ -88,20 +106,23 @@
 To test local destinations (`duckdb` and `postgres`) run `make test-local`. You can run this tests without additional credentials (just copy `.example.env` into `.env`)
 
 ## publishing
 
 1. Make sure that you are on `devel` branch and you have the newest code that passed all tests on CI.
 2. Verify the current version with `poetry version`
 3. You'll need `pypi` access token and use `poetry config pypi-token.pypi your-api-token` then
+
 ```
 make publish-library
 ```
+
 4. Make a release on github, use version and git tag as release name
 
 ## contributing
 
 To contribute via pull request:
+
 1. Create an issue with your idea for a feature etc.
 2. Write your code and tests
 3. Lint your code with `make lint`. Test the common modules with `make test-common`
 4. If you work on a destination code then contact us to get access to test destinations
 5. Create a pull request
```

### Comparing `dlt-0.2.5a1/dlt/__init__.py` & `dlt-0.2.6a0/dlt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 For more detailed info, see https://dlthub.com/docs/getting-started
 """
 
 from dlt.version import __version__
 from dlt.common.configuration.accessors import config, secrets
 from dlt.common.typing import TSecretValue as _TSecretValue
 from dlt.common.configuration.specs import CredentialsConfiguration as _CredentialsConfiguration
-from dlt.common.pipeline import state
+from dlt.common.pipeline import source_state as state
 from dlt.common.schema import Schema
 
 from dlt import sources
 from dlt.extract.decorators import source, resource, transformer, defer
 from dlt.pipeline import pipeline as _pipeline, run, attach, Pipeline, dbt, current as _current, mark as _mark
 
 pipeline = _pipeline
```

### Comparing `dlt-0.2.5a1/dlt/cli/_dlt.py` & `dlt-0.2.6a0/dlt/cli/_dlt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/cli/config_toml_writer.py` & `dlt-0.2.6a0/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/cli/deploy_command.py` & `dlt-0.2.6a0/dlt/cli/deploy_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,15 @@
     cycles = pipdeptree.cyclic_deps(tree)
     if conflicts:
         fmt.warning(f"Unable to create dependencies for the github action. Please edit {REQUIREMENTS_GITHUB_ACTION} yourself")
         pipdeptree.render_conflicts_text(conflicts)
         pipdeptree.render_cycles_text(cycles)
         fmt.echo()
         # do not create package because it will most probably fail
-        return "# please provide valid dependencies including python-dlt"
+        return "# please provide valid dependencies including dlt package"
 
     lines = [node.render(None, False) for node in nodes]
     return "\n".join(lines)
 
 
 def github_origin_to_url(origin: str, path: str) -> str:
     # repository origin must end with .git
```

### Comparing `dlt-0.2.5a1/dlt/cli/echo.py` & `dlt-0.2.6a0/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/cli/init_command.py` & `dlt-0.2.6a0/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/cli/pipeline_command.py` & `dlt-0.2.6a0/dlt/cli/pipeline_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/cli/pipeline_files.py` & `dlt-0.2.6a0/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/cli/source_detection.py` & `dlt-0.2.6a0/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/cli/telemetry_command.py` & `dlt-0.2.6a0/dlt/cli/telemetry_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 from dlt.common.configuration.providers.toml import ConfigTomlProvider
 from dlt.common.configuration.specs import RunConfiguration
 
 from dlt.cli import echo as fmt
 from dlt.cli.utils import get_telemetry_status
 from dlt.cli.config_toml_writer import WritableConfigValue, write_values
 from dlt.common.configuration.specs.config_providers_context import ConfigProvidersContext
+from dlt.common.runtime.segment import get_anonymous_id
 
 DLT_TELEMETRY_DOCS_URL = "https://dlthub.com/docs/reference/telemetry"
 
 
 def telemetry_status_command() -> None:
     if get_telemetry_status():
         fmt.echo("Telemetry is %s" % fmt.bold("ENABLED"))
+        fmt.echo("Anonymous id %s" % fmt.bold(get_anonymous_id()))
     else:
         fmt.echo("Telemetry is %s" % fmt.bold("DISABLED"))
 
 
 def change_telemetry_status_command(enabled: bool) -> None:
     # value to write
     telemetry_value = [WritableConfigValue("dlthub_telemetry", bool, enabled, (RunConfiguration.__section__, ))]
```

### Comparing `dlt-0.2.5a1/dlt/cli/utils.py` & `dlt-0.2.6a0/dlt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/arithmetics.py` & `dlt-0.2.6a0/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/accessors.py` & `dlt-0.2.6a0/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/container.py` & `dlt-0.2.6a0/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/exceptions.py` & `dlt-0.2.6a0/dlt/common/configuration/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     def __str__(self) -> str:
         msg = f"Following fields are missing: {str(self.fields)} in configuration with spec {self.spec_name}\n"
         for f, field_traces in self.traces.items():
             msg += f'\tfor field "{f}" config providers and keys were tried in following order:\n'
             for tr in field_traces:
                 msg += f'\t\tIn {tr.provider} key {tr.key} was not found.\n'
-        msg += "Please refer to https://dlthub.com/docs/customization/credentials for more information\n"
+        msg += "Please refer to https://dlthub.com/docs/general-usage/credentials for more information\n"
         return msg
 
 
 class FinalConfigFieldException(ConfigurationException):
     """rises when field was annotated as final ie Final[str] and the value is modified by config provider"""
     def __init__(self, spec_name: str, field: str) -> None:
         super().__init__(f"Field {field} in spec {spec_name} is final but is being changed by a config provider")
```

### Comparing `dlt-0.2.5a1/dlt/common/configuration/inject.py` & `dlt-0.2.6a0/dlt/common/configuration/inject.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,23 +130,25 @@
                 # resolve SPEC, also provide section_context with pipeline_name
                 if pipeline_name_arg:
                     section_context.pipeline_name = bound_args.arguments.get(pipeline_name_arg.name, pipeline_name_arg_default)
                 with inject_section(section_context):
                     # print(f"RESOLVE CONF in inject: {f.__name__}: {section_context.sections} vs {sections}")
                     config = resolve_configuration(config or SPEC(), explicit_value=bound_args.arguments)
             resolved_params = dict(config)
-            bound_args.apply_defaults()
             # overwrite or add resolved params
             for p in sig.parameters.values():
                 if p.name in resolved_params:
                     bound_args.arguments[p.name] = resolved_params.pop(p.name)
                 if p.annotation is SPEC:
                     bound_args.arguments[p.name] = config
             # pass all other config parameters into kwargs if present
             if kwargs_arg is not None:
+                if kwargs_arg.name not in bound_args.arguments:
+                    # add variadic keyword argument
+                    bound_args.arguments[kwargs_arg.name] = {}
                 bound_args.arguments[kwargs_arg.name].update(resolved_params)
                 bound_args.arguments[kwargs_arg.name][_LAST_DLT_CONFIG] = config
                 bound_args.arguments[kwargs_arg.name][_ORIGINAL_ARGS] = (args, kwargs)
             # call the function with resolved config
             return f(*bound_args.args, **bound_args.kwargs)
 
         # register the spec for a wrapped function
```

### Comparing `dlt-0.2.5a1/dlt/common/configuration/paths.py` & `dlt-0.2.6a0/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/providers/context.py` & `dlt-0.2.6a0/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/providers/dictionary.py` & `dlt-0.2.6a0/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/providers/environ.py` & `dlt-0.2.6a0/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/providers/provider.py` & `dlt-0.2.6a0/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/providers/toml.py` & `dlt-0.2.6a0/dlt/common/configuration/providers/toml.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,44 +8,17 @@
 from dlt.common.utils import update_dict_nested
 
 from .provider import ConfigProvider, ConfigProviderException
 
 CONFIG_TOML = "config.toml"
 SECRETS_TOML = "secrets.toml"
 
-
-class TomlProvider(ConfigProvider):
-
-    def __init__(self, file_name: str, project_dir: str = None, add_global_config: bool = False) -> None:
-        """Creates config provider from a `toml` file
-
-        The provider loads the `toml` file with specified name and from specified folder. If `add_global_config` flags is specified,
-        it will look for `file_name` in `dlt` home dir. The "project" (`project_dir`) values overwrite the "global" values.
-
-        If none of the files exist, an empty provider is created.
-
-        Args:
-            file_name (str): The name of `toml` file to load
-            project_dir (str, optional): The location of `file_name`. If not specified, defaults to $cwd/.dlt
-            add_global_config (bool, optional): Looks for `file_name` in `dlt` home directory which in most cases is $HOME/.dlt
-
-        Raises:
-            TomlProviderReadException: File could not be read, most probably `toml` parsing error
-        """
-        self._file_name = file_name
-        self._toml_path = os.path.join(project_dir or get_dlt_project_dir(), file_name)
-        self._add_global_config = add_global_config
-        try:
-            project_toml = self._read_toml(self._toml_path)
-            if add_global_config:
-                global_toml = self._read_toml(os.path.join(self.global_config_path(), file_name))
-                project_toml = update_dict_nested(global_toml, project_toml)
-            self._toml = project_toml
-        except Exception as ex:
-            raise TomlProviderReadException(self.name, file_name, self._toml_path, str(ex))
+class BaseTomlProvider(ConfigProvider):
+    def __init__(self, toml_document: tomlkit.TOMLDocument) -> None:
+        self._toml = toml_document
 
     @staticmethod
     def get_key_name(key: str, *sections: str) -> str:
         # env key is always upper case
         if sections:
             sections = filter(lambda x: bool(x), sections)  # type: ignore
             env_key = ".".join((*sections, key))
@@ -72,14 +45,48 @@
         return True
 
     @property
     def is_empty(self) -> bool:
         # no keys
         return self._toml.as_string() == ""
 
+
+class TomlProvider(BaseTomlProvider):
+    def __init__(self, file_name: str, project_dir: str = None, add_global_config: bool = False) -> None:
+        """Creates config provider from a `toml` file
+
+        The provider loads the `toml` file with specified name and from specified folder. If `add_global_config` flags is specified,
+        it will look for `file_name` in `dlt` home dir. The "project" (`project_dir`) values overwrite the "global" values.
+
+        If none of the files exist, an empty provider is created.
+
+        Args:
+            file_name (str): The name of `toml` file to load
+            project_dir (str, optional): The location of `file_name`. If not specified, defaults to $cwd/.dlt
+            add_global_config (bool, optional): Looks for `file_name` in `dlt` home directory which in most cases is $HOME/.dlt
+
+        Raises:
+            TomlProviderReadException: File could not be read, most probably `toml` parsing error
+        """
+        toml_document = self._read_toml_file(file_name, project_dir, add_global_config)
+        super().__init__(toml_document)
+
+    def _read_toml_file(self, file_name: str, project_dir: str = None, add_global_config: bool = False) -> tomlkit.TOMLDocument:
+        self._file_name = file_name
+        self._toml_path = os.path.join(project_dir or get_dlt_project_dir(), file_name)
+        self._add_global_config = add_global_config
+        try:
+            project_toml = self._read_toml(self._toml_path)
+            if add_global_config:
+                global_toml = self._read_toml(os.path.join(self.global_config_path(), file_name))
+                project_toml = update_dict_nested(global_toml, project_toml)
+            return project_toml
+        except Exception as ex:
+            raise TomlProviderReadException(self.name, file_name, self._toml_path, str(ex))
+
     @staticmethod
     def global_config_path() -> str:
         return get_dlt_home_dir()
 
     def write_toml(self) -> None:
         assert not self._add_global_config, "Will not write configs when `add_global_config` flag was set"
         with open(self._toml_path, "w", encoding="utf-8") as f:
```

### Comparing `dlt-0.2.5a1/dlt/common/configuration/resolve.py` & `dlt-0.2.6a0/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/specs/__init__.py` & `dlt-0.2.6a0/dlt/common/configuration/specs/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 from .run_configuration import RunConfiguration  # noqa: F401
 from .base_configuration import BaseConfiguration, CredentialsConfiguration, CredentialsWithDefault, ContainerInjectableContext, extract_inner_hint, is_base_configuration_inner_hint  # noqa: F401
 from .normalize_volume_configuration import NormalizeVolumeConfiguration  # noqa: F401
 from .load_volume_configuration import LoadVolumeConfiguration  # noqa: F401
 from .schema_volume_configuration import SchemaVolumeConfiguration, TSchemaFileFormat  # noqa: F401
-from .gcp_client_credentials import GcpClientCredentials, GcpClientCredentialsWithDefault  # noqa: F401
+from .gcp_client_credentials import GcpClientCredentials, GcpClientCredentialsWithDefault, GcpOAuthCredentials, GcpOAuthCredentialsWithDefault  # noqa: F401
 from .postgres_credentials import PostgresCredentials, RedshiftCredentials, ConnectionStringCredentials  # noqa: F401
 from .config_section_context import ConfigSectionContext  # noqa: F401
```

### Comparing `dlt-0.2.5a1/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.2.6a0/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.2.6a0/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/specs/known_sections.py` & `dlt-0.2.6a0/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/specs/load_volume_configuration.py` & `dlt-0.2.6a0/dlt/common/configuration/specs/load_volume_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/specs/postgres_credentials.py` & `dlt-0.2.6a0/dlt/common/configuration/specs/postgres_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.2.6a0/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/specs/schema_volume_configuration.py` & `dlt-0.2.6a0/dlt/common/configuration/specs/schema_volume_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/configuration/utils.py` & `dlt-0.2.6a0/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/data_types/type_helpers.py` & `dlt-0.2.6a0/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/data_writers/buffered.py` & `dlt-0.2.6a0/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/data_writers/escape.py` & `dlt-0.2.6a0/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/data_writers/exceptions.py` & `dlt-0.2.6a0/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/data_writers/writers.py` & `dlt-0.2.6a0/dlt/common/data_writers/writers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/destination/capabilities.py` & `dlt-0.2.6a0/dlt/common/destination/capabilities.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/destination/reference.py` & `dlt-0.2.6a0/dlt/common/destination/reference.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/exceptions.py` & `dlt-0.2.6a0/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/git.py` & `dlt-0.2.6a0/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/json/__init__.py` & `dlt-0.2.6a0/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/json/_orjson.py` & `dlt-0.2.6a0/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/json/_simplejson.py` & `dlt-0.2.6a0/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/normalizers/configuration.py` & `dlt-0.2.6a0/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/normalizers/json/__init__.py` & `dlt-0.2.6a0/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/normalizers/json/relational.py` & `dlt-0.2.6a0/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/normalizers/naming/direct.py` & `dlt-0.2.6a0/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.2.6a0/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.2.6a0/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/normalizers/naming/naming.py` & `dlt-0.2.6a0/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.2.6a0/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/normalizers/utils.py` & `dlt-0.2.6a0/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/pipeline.py` & `dlt-0.2.6a0/dlt/common/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,14 +144,16 @@
     """The destination reference which is ModuleType. `destination.__name__` returns the name string"""
     dataset_name: str = None
     """Name of the dataset to which pipeline will be loaded to"""
     runtime_config: RunConfiguration
     """A configuration of runtime options like logging level and format and various tracing options"""
     working_dir: str
     """A working directory of the pipeline"""
+    pipeline_salt: str
+    """A configurable pipeline secret to be used as a salt or a seed for encryption key"""
 
     @property
     def state(self) -> TPipelineState:
         """Returns dictionary with pipeline state"""
 
     def set_local_state_val(self, key: str, value: Any) -> None:
         """Sets value in local state. Local state is not synchronized with destination."""
@@ -233,15 +235,15 @@
     can_create_default: ClassVar[bool] = False
 
     if TYPE_CHECKING:
         def __init__(self, state: TPipelineState = None) -> None:
             ...
 
 
-def state_value(container: Container, initial_default: TPipelineState = None) -> Tuple[TPipelineState, bool]:
+def pipeline_state(container: Container, initial_default: TPipelineState = None) -> Tuple[TPipelineState, bool]:
     """Gets value of the state from context or active pipeline, if none found returns `initial_default`
 
         Injected state is called "writable": it is injected by the `Pipeline` class and all the changes will be persisted.
         The state coming from pipeline context or `initial_default` is called "read only" and all the changes to it will be discarded
 
         Returns tuple (state, writable)
     """
@@ -255,24 +257,26 @@
             return initial_default, False
         else:
             # get unmanaged state that is read only
             # TODO: make sure that state if up to date by syncing the pipeline earlier
             return proxy.pipeline().state, False
 
 
-def state() -> DictStrAny:
-    """Returns a dictionary with the source/resource state. Such state is preserved across pipeline runs and may be used to implement incremental loads.
+def source_state() -> DictStrAny:
+    """Returns a dictionary with the source state. Such state is preserved across pipeline runs and may be used to implement incremental loads.
 
     ### Summary
     The state is a python dictionary-like object that is available within the `@dlt.source` and `@dlt.resource` decorated functions and may be read and written to.
     The data within the state is loaded into destination together with any other extracted data and made automatically available to the source/resource extractor functions when they are run next time.
     When using the state:
-    * Any JSON-serializable values can be written and the read from the state.
-    * The state available in the `dlt source` is read only and any changes will be discarded. Still it may be used to initialize the resources.
-    * The state available in the `dlt resource` is writable and written values will be available only once
+    * The source state is scoped to a section of the source. The source section is set by default to the module name in which source function is defined.
+    * If the `section` argument when decorating source function is not specified, all sources in the module will share the state
+    * Any JSON-serializable values can be written and the read from the state. `dlt` dumps and restores instances of Python bytes, DateTime, Date and Decimal types.
+    * The state available in the source decorated function is read only and any changes will be discarded.
+    * The state available in the resource decorated function is writable and written values will be available on the next pipeline run
 
     ### Example
     The most typical use case for the state is to implement incremental load.
     >>> @dlt.resource(write_disposition="append")
     >>> def players_games(chess_url, players, start_month=None, end_month=None):
     >>>     checked_archives = dlt.current.state().setdefault("archives", [])
     >>>     archives = players_archives(chess_url, players)
@@ -301,15 +305,15 @@
         sections_context = container[ConfigSectionContext]
         with contextlib.suppress(ValueError):
             source_section = sections_context.source_section()
 
     if not source_section:
         raise SourceSectionNotAvailable()
 
-    state, _ = state_value(container)
+    state, _ = pipeline_state(container)
     if state is None:
         raise PipelineStateNotAvailable(source_section)
 
     source_state: DictStrAny = state.setdefault(known_sections.SOURCES, {})  # type: ignore
     if source_section:
         source_state = source_state.setdefault(source_section, {})
 
@@ -320,20 +324,20 @@
 _last_full_state: TPipelineState = None
 
 
 def _resource_state(resource_name: str) -> DictStrAny:
     """Alpha version of the resource state, the signature will change.
     Returns resource-scoped state.
     """
-    return state().setdefault('resources', {}).setdefault(resource_name, {})  # type: ignore
+    return source_state().setdefault('resources', {}).setdefault(resource_name, {})  # type: ignore
 
 
 def _reset_resource_state(resource_name: str) -> None:
-    """Alpha version of the resource state. Resets the resource states"""
-    state_ = state()
+    """Alpha version of the resource state. Resets the resource state"""
+    state_ = source_state()
     if "resources" in state_ and resource_name in state_["resources"]:
         state_["resources"].pop(resource_name)
 
 
 def get_dlt_pipelines_dir() -> str:
     """ Gets default directory where pipelines' data will be stored
         1. in user home directory ~/.dlt/pipelines/
```

### Comparing `dlt-0.2.5a1/dlt/common/reflection/spec.py` & `dlt-0.2.6a0/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/reflection/utils.py` & `dlt-0.2.6a0/dlt/common/reflection/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,18 +46,18 @@
     return None
 
 
 def find_outer_func_def(node: ast.AST) -> Optional[ast.FunctionDef]:
     """Finds the outer function definition node in which the 'node' is contained. Returns None if 'node' is toplevel."""
     if not hasattr(node, "parent"):
         raise ValueError("No parent information in node, not enabled in visitor", node)
-    while not isinstance(node.parent, ast.FunctionDef):  # type: ignore
-        if node.parent is None:  # type: ignore
+    while not isinstance(node.parent, ast.FunctionDef):
+        if node.parent is None:
             return None
-        node = node.parent  # type: ignore
+        node = node.parent
     return node  # type: ignore
 
 
 def set_ast_parents(tree: ast.AST) -> None:
     """Walks AST tree and sets the `parent` attr in each node to the node's parent. Toplevel nodes (parent is a `tree`) have the `parent` attr set to None."""
     for node in ast.walk(tree):
         for child in ast.iter_child_nodes(node):
```

### Comparing `dlt-0.2.5a1/dlt/common/runners/configuration.py` & `dlt-0.2.6a0/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/runners/init.py` & `dlt-0.2.6a0/dlt/common/runners/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/runners/pool_runner.py` & `dlt-0.2.6a0/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/runners/runnable.py` & `dlt-0.2.6a0/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/runners/stdout.py` & `dlt-0.2.6a0/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/runners/synth_pickle.py` & `dlt-0.2.6a0/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/runners/typing.py` & `dlt-0.2.6a0/dlt/common/runners/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/runners/venv.py` & `dlt-0.2.6a0/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/runtime/exec_info.py` & `dlt-0.2.6a0/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/runtime/logger.py` & `dlt-0.2.6a0/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/runtime/prometheus.py` & `dlt-0.2.6a0/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/runtime/segment.py` & `dlt-0.2.6a0/dlt/common/runtime/segment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """dltHub telemetry using Segment"""
 
 # several code fragments come from https://github.com/RasaHQ/rasa/blob/main/rasa/telemetry.py
+import os
 import sys
 import multiprocessing
 import atexit
 import base64
 import requests
 import platform
-import time
 from concurrent.futures import ThreadPoolExecutor
 from typing import Literal, Optional
+from dlt.common.configuration.paths import get_dlt_home_dir
 
 from dlt.common.runtime import logger
 from dlt.common.configuration.specs import RunConfiguration
 from dlt.common.runtime.exec_info import exec_info_names, in_continuous_integration
 from dlt.common.typing import DictStrAny, StrAny
+from dlt.common.utils import uniq_id
 from dlt.version import __version__, DLT_PKG_NAME
 
 TEventCategory = Literal["pipeline", "command"]
 
 _THREAD_POOL: ThreadPoolExecutor = None
 _SESSION: requests.Session = None
 _WRITE_KEY: str = None
@@ -104,14 +106,30 @@
     """
     return {
         "Authorization": "Basic {}".format(write_key),
         "Content-Type": "application/json",
     }
 
 
+def get_anonymous_id() -> str:
+    """Creates or reads a anonymous user id"""
+    home_dir = get_dlt_home_dir()
+    if not os.path.isdir(home_dir):
+        os.makedirs(home_dir, exist_ok=True)
+    anonymous_id_file = os.path.join(home_dir, ".anonymous_id")
+    if not os.path.isfile(anonymous_id_file):
+        anonymous_id = uniq_id()
+        with open(anonymous_id_file, "w", encoding="utf-8") as f:
+            f.write(anonymous_id)
+    else:
+        with open(anonymous_id_file, "r", encoding="utf-8") as f:
+            anonymous_id = f.read()
+    return anonymous_id
+
+
 def _segment_request_payload(
     event_name: str,
     properties: StrAny,
     context: StrAny
 ) -> DictStrAny:
     """Compose a valid payload for the segment API.
 
@@ -120,15 +138,15 @@
         properties: Values to report along the event.
         context: Context information about the event.
 
     Returns:
         Valid segment payload.
     """
     return {
-        "anonymousId": "8c45f93d27f72347a3604521e2d4c33b",
+        "anonymousId": get_anonymous_id(),
         "event": event_name,
         "properties": properties,
         "context": context,
     }
 
 
 def _default_context_fields() -> DictStrAny:
@@ -158,15 +176,15 @@
 
 
 def _send_event(
     event_name: str,
     properties: StrAny,
     context: StrAny
 ) -> None:
-    """Report the contents segmentof an event to the /track Segment endpoint.
+    """Report the contents segment of an event to the /track Segment endpoint.
 
     Args:
         event_name: Name of the event.
         properties: Values to report along the event.
         context: Context information about the event.
     """
     # formulate payload and process in before send
@@ -181,15 +199,14 @@
         logger.debug("Skipping request to external service: telemetry key not set.")
         return
 
     headers = _segment_request_header(_WRITE_KEY)
 
     def _future_send() -> None:
         # start_ts = time.time()
-        # print("sending to Segment")
         resp = _SESSION.post(_SEGMENT_ENDPOINT, headers=headers, json=payload, timeout=_SEGMENT_REQUEST_TIMEOUT)
         # print(f"sending to Segment done {resp.status_code} {time.time() - start_ts}")
         # handle different failure cases
         if resp.status_code != 200:
             logger.debug(
                 f"Segment telemetry request returned a {resp.status_code} response. "
                 f"Body: {resp.text}"
```

### Comparing `dlt-0.2.5a1/dlt/common/runtime/sentry.py` & `dlt-0.2.6a0/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/runtime/signals.py` & `dlt-0.2.6a0/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/runtime/slack.py` & `dlt-0.2.6a0/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/runtime/telemetry.py` & `dlt-0.2.6a0/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/schema/detections.py` & `dlt-0.2.6a0/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/schema/exceptions.py` & `dlt-0.2.6a0/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/schema/schema.py` & `dlt-0.2.6a0/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/schema/typing.py` & `dlt-0.2.6a0/dlt/common/schema/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     name: Optional[str]
     description: Optional[str]
     write_disposition: Optional[TWriteDisposition]
     table_sealed: Optional[bool]
     parent: Optional[str]
     filters: Optional[TRowFilters]
     columns: TTableSchemaColumns
+    resource: Optional[str]
 
 
 class TPartialTableSchema(TTableSchema):
     pass
 
 
 TSchemaTables = Dict[str, TTableSchema]
```

### Comparing `dlt-0.2.5a1/dlt/common/schema/utils.py` & `dlt-0.2.6a0/dlt/common/schema/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,30 +25,35 @@
 
 
 def apply_defaults(stored_schema: TStoredSchema) -> None:
     for table_name, table in stored_schema["tables"].items():
         # overwrite name
         table["name"] = table_name
         # add default write disposition to root tables
-        if table.get("parent") is None and table.get("write_disposition") is None:
-            table["write_disposition"] = DEFAULT_WRITE_DISPOSITION
+        if table.get("parent") is None:
+            if table.get("write_disposition") is None:
+                table["write_disposition"] = DEFAULT_WRITE_DISPOSITION
+            if table.get('resource') is None:
+                table['resource'] = table_name
         # add missing hints to columns
         for column_name in table["columns"]:
             # add default hints to tables
             column = add_missing_hints(table["columns"][column_name])
             # overwrite column name
             column["name"] = column_name
             # set column with default
             table["columns"][column_name] = column
 
 
 def remove_defaults(stored_schema: TStoredSchema) -> TStoredSchema:
     clean_tables = deepcopy(stored_schema["tables"])
-    for t in clean_tables.values():
+    for table_name, t in clean_tables.items():
         del t["name"]
+        if t.get('resource') == table_name:
+            del t['resource']
         for c in t["columns"].values():
             # do not save names
             del c["name"]
             # remove hints with default values
             for h in list(c.keys()):
                 if isinstance(c[h], bool) and c[h] is False and h != "nullable":  # type: ignore
                     del c[h]  # type: ignore
@@ -354,14 +359,16 @@
     diff_table = diff_tables(table, partial_table, ignore_table_name=True)
     # add new columns when all checks passed
     table["columns"].update(diff_table["columns"])
 
     partial_w_d = partial_table.get("write_disposition")
     if partial_w_d:
         table["write_disposition"] = partial_w_d
+    if table.get('parent') is None and (resource := partial_table.get('resource')):
+        table['resource'] = resource
 
     return diff_table
 
 
 def hint_to_column_prop(h: TColumnHint) -> TColumnProp:
     if h == "not_null":
         return "nullable"
@@ -492,27 +499,30 @@
 
 
 def new_table(
     table_name: str,
     parent_table_name: str = None,
     write_disposition: TWriteDisposition = None,
     columns: Sequence[TColumnSchema] = None,
-    validate_schema: bool = False
+    validate_schema: bool = False,
+    resource: str = None
 ) -> TTableSchema:
 
     table: TTableSchema = {
         "name": table_name,
         "columns": {} if columns is None else {c["name"]: add_missing_hints(c) for c in columns}
     }
     if parent_table_name:
         table["parent"] = parent_table_name
         assert write_disposition is None
+        assert resource is None
     else:
         # set write disposition only for root tables
         table["write_disposition"] = write_disposition or DEFAULT_WRITE_DISPOSITION
+        table["resource"] = resource or table_name
     if validate_schema:
         validate_dict(TTableSchema, table, f"new_table/{table_name}")
     return table
 
 
 def new_column(column_name: str, data_type: TDataType = None, nullable: bool = True, validate_schema: bool = False) -> TColumnSchema:
     column = add_missing_hints({
```

### Comparing `dlt-0.2.5a1/dlt/common/storages/data_item_storage.py` & `dlt-0.2.6a0/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/storages/exceptions.py` & `dlt-0.2.6a0/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/storages/file_storage.py` & `dlt-0.2.6a0/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/storages/live_schema_storage.py` & `dlt-0.2.6a0/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/storages/load_storage.py` & `dlt-0.2.6a0/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/storages/normalize_storage.py` & `dlt-0.2.6a0/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/storages/schema_storage.py` & `dlt-0.2.6a0/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/storages/versioned_storage.py` & `dlt-0.2.6a0/dlt/common/storages/versioned_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,11 +44,12 @@
         pass
 
     @property
     def version(self) -> semver.VersionInfo:
         return self._load_version()
 
     def _load_version(self) -> semver.VersionInfo:
-        return self.storage.load(VersionedStorage.VERSION_FILE)
+        version_str = self.storage.load(VersionedStorage.VERSION_FILE)
+        return semver.VersionInfo.parse(version_str)
 
     def _save_version(self, version: semver.VersionInfo) -> None:
         self.storage.save(VersionedStorage.VERSION_FILE, str(version))
```

### Comparing `dlt-0.2.5a1/dlt/common/time.py` & `dlt-0.2.6a0/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/typing.py` & `dlt-0.2.6a0/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/utils.py` & `dlt-0.2.6a0/dlt/common/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import sys
 import base64
 import hashlib
 import secrets
 from contextlib import contextmanager
 from functools import wraps
 from os import environ
+from types import ModuleType
 import zlib
 
 from typing import Any, ContextManager, Dict, Iterator, Optional, Sequence, TypeVar, Mapping, List, Union, Counter
 from collections.abc import Mapping as C_Mapping
 
 from dlt.common.typing import AnyFun, StrAny, DictStrAny, StrStr, TAny, TFun
 
@@ -174,15 +175,15 @@
     return dst
 
 
 def map_nested_in_place(func: AnyFun, _complex: TAny) -> TAny:
     """Applies `func` to all elements in `_dict` recursively, replacing elements in nested dictionaries and lists in place."""
     if isinstance(_complex, tuple):
         if hasattr(_complex, "_asdict"):
-            _complex = _complex._asdict()  # type: ignore
+            _complex = _complex._asdict()
         else:
             _complex = list(_complex)  # type: ignore
 
     if isinstance(_complex, dict):
         for k, v in _complex.items():
             if isinstance(v, (dict, list, tuple)):
                 _complex[k] = map_nested_in_place(func, v)
@@ -196,15 +197,23 @@
                 _complex[idx] = func(_l)
     else:
         raise ValueError(_complex, "Not a complex type")
     return _complex
 
 
 def is_interactive() -> bool:
+    """
+    Determine if the current environment is interactive.
+
+    Returns:
+        bool: True if interactive (e.g., REPL, IPython, Jupyter Notebook), False if running as a script.
+    """
     import __main__ as main
+    # When running as a script, the __main__ module has a __file__ attribute.
+    # In an interactive environment, the __file__ attribute is absent.
     return not hasattr(main, '__file__')
 
 
 def dict_remove_nones_in_place(d: Dict[Any, Any]) -> Dict[Any, Any]:
     for k in list(d.keys()):
         if d[k] is None:
             del d[k]
@@ -305,14 +314,23 @@
     return base64.b64encode(bytes([_a ^ _b for _a, _b in zip(pseudo_secret.encode("utf-8"), pseudo_key*250)])).decode()
 
 
 def reveal_pseudo_secret(obfuscated_secret: str, pseudo_key: bytes) -> str:
     return bytes([_a ^ _b for _a, _b in zip(base64.b64decode(obfuscated_secret.encode("ascii"), validate=True), pseudo_key*250)]).decode("utf-8")
 
 
+def get_module_name(m: ModuleType) -> str:
+    """Gets module name from module with a fallback for executing module __main__"""
+    if m.__name__ == "__main__":
+        module_file = os.path.basename(m.__file__)
+        module_name, _ = os.path.splitext(module_file)
+        return module_name
+    return m.__name__.split(".")[-1]
+
+
 def derives_from_class_of_name(o: object, name: str) -> bool:
     """Checks if object o has class of name in its derivation tree"""
     mro = type.mro(type(o))
     return any(t.__name__ == name for t in mro)
 
 
 def compressed_b64encode(value: bytes) -> str:
```

### Comparing `dlt-0.2.5a1/dlt/common/validation.py` & `dlt-0.2.6a0/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/common/wei.py` & `dlt-0.2.6a0/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/bigquery/__init__.py` & `dlt-0.2.6a0/dlt/destinations/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/bigquery/bigquery.py` & `dlt-0.2.6a0/dlt/destinations/bigquery/bigquery.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/bigquery/sql_client.py` & `dlt-0.2.6a0/dlt/destinations/bigquery/sql_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 
 from contextlib import contextmanager
-from typing import Any, AnyStr, ClassVar, Iterator, List, Optional, Sequence, Tuple
+from typing import Any, AnyStr, ClassVar, Iterator, List, Optional, Sequence
 
 import google.cloud.bigquery as bigquery  # noqa: I250
 from google.cloud.bigquery import dbapi as bq_dbapi
 from google.cloud.bigquery.dbapi import Connection as DbApiConnection, Cursor as BQDbApiCursor
 from google.cloud import exceptions as gcp_exceptions
 from google.cloud.bigquery.dbapi import exceptions as dbapi_exceptions
 from google.api_core import exceptions as api_core_exceptions
 
-from dlt.common import logger
 from dlt.common.configuration.specs import GcpClientCredentials
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.typing import StrAny
 
 from dlt.destinations.typing import DBApi, DBApiCursor, DBTransaction, DataFrame
 from dlt.destinations.exceptions import DatabaseTerminalException, DatabaseTransientException, DatabaseUndefinedRelation
 from dlt.destinations.sql_client import DBApiCursorImpl, SqlClientBase, raise_database_error, raise_open_connection_error
@@ -57,15 +56,15 @@
         self._default_query = bigquery.QueryJobConfig(default_dataset=self.fully_qualified_dataset_name(escape=False))
         self._session_query: bigquery.QueryJobConfig = None
 
     @raise_open_connection_error
     def open_connection(self) -> bigquery.Client:
         self._client = bigquery.Client(
             self.credentials.project_id,
-            credentials=self.credentials.to_service_account_credentials(),
+            credentials=self.credentials.to_google_credentials(),
             location=self.credentials.location
         )
 
         # patch the client query so our defaults are used
         query_orig = self._client.query
 
         def query_patch(
```

### Comparing `dlt-0.2.5a1/dlt/destinations/duckdb/__init__.py` & `dlt-0.2.6a0/dlt/destinations/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/duckdb/configuration.py` & `dlt-0.2.6a0/dlt/destinations/duckdb/configuration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import threading
 from pathvalidate import is_valid_filepath
-from typing import Any, Final, Optional
+from typing import Any, Final, Optional, Tuple
 
+from dlt.common import logger
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import ConnectionStringCredentials
 from dlt.common.configuration.specs.exceptions import InvalidConnectionString
 from dlt.common.destination.reference import DestinationClientDwhConfiguration
 from dlt.common.typing import TSecretValue
 
 DUCK_DB_NAME = "%s.duckdb"
@@ -78,23 +79,26 @@
                 raise
 
     def on_resolved(self) -> None:
         # do not set any paths for external database
         if self.database == ":external:":
             return
         # try the pipeline context
+        is_default_path = False
         if self.database == ":pipeline:":
             self.database = self._path_in_pipeline(DEFAULT_DUCK_DB_NAME)
         # if pipeline context was not present or database was not set
         if not self.database:
             # create database locally
-            self.database = self._path_from_pipeline(DEFAULT_DUCK_DB_NAME)
+            self.database, is_default_path = self._path_from_pipeline(DEFAULT_DUCK_DB_NAME)
         # always make database an abs path
         self.database = os.path.abspath(self.database)
-        self._path_to_pipeline(self.database)
+        # do not save the default path into pipeline's local state
+        if not is_default_path:
+            self._path_to_pipeline(self.database)
 
     def _path_in_pipeline(self, rel_path: str) -> str:
         from dlt.common.configuration.container import Container
         from dlt.common.pipeline import PipelineContext
 
         context = Container()[PipelineContext]
         if context.is_active():
@@ -107,27 +111,50 @@
         from dlt.common.configuration.container import Container
         from dlt.common.pipeline import PipelineContext
 
         context = Container()[PipelineContext]
         if context.is_active():
             context.pipeline().set_local_state_val(LOCAL_STATE_KEY, abspath)
 
-    def _path_from_pipeline(self, default_path: str) -> str:
+    def _path_from_pipeline(self, default_path: str) -> Tuple[str, bool]:
+        """
+        Returns path to DuckDB as stored in the active pipeline's local state and a boolean flag.
+
+        If the pipeline state is not available, returns the default DuckDB path that includes the pipeline name and sets the flag to True.
+        If the pipeline context is not available, returns the provided default_path and sets the flag to True.
+
+        Args:
+            default_path (str): The default DuckDB path to return if the pipeline context or state is not available.
+
+        Returns:
+            Tuple[str, bool]: The path to the DuckDB as stored in the active pipeline's local state or the default path if not available,
+            and a boolean flag set to True when the default path is returned.
+        """
         from dlt.common.configuration.container import Container
         from dlt.common.pipeline import PipelineContext
 
         context = Container()[PipelineContext]
         if context.is_active():
             try:
                 # use pipeline name as default
-                default_path = DUCK_DB_NAME % context.pipeline().pipeline_name
-                return context.pipeline().get_local_state_val(LOCAL_STATE_KEY)  # type: ignore
+                pipeline = context.pipeline()
+                default_path = DUCK_DB_NAME % pipeline.pipeline_name
+                # get pipeline path from local state
+                pipeline_path = pipeline.get_local_state_val(LOCAL_STATE_KEY)
+                # make sure that path exists
+                if not os.path.exists(pipeline_path):
+                    logger.warning(f"Duckdb attached to pipeline {pipeline.pipeline_name} in path {os.path.relpath(pipeline_path)} was deleted. Attaching to duckdb database '{default_path}' in current folder.")
+                else:
+                    return pipeline_path, False
             except KeyError:
+                # no local state: default_path will be used
                 pass
-        return default_path
+
+        return default_path, True
+
 
     def _delete_conn(self) -> None:
         # print("Closing conn because is owner")
         self._conn.close()
         delattr(self, "_conn")
 
     def __del__(self) -> None:
```

### Comparing `dlt-0.2.5a1/dlt/destinations/duckdb/duck.py` & `dlt-0.2.6a0/dlt/destinations/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/duckdb/sql_client.py` & `dlt-0.2.6a0/dlt/destinations/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/dummy/__init__.py` & `dlt-0.2.6a0/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/dummy/configuration.py` & `dlt-0.2.6a0/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/dummy/dummy.py` & `dlt-0.2.6a0/dlt/destinations/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/exceptions.py` & `dlt-0.2.6a0/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/insert_job_client.py` & `dlt-0.2.6a0/dlt/destinations/insert_job_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/job_client_impl.py` & `dlt-0.2.6a0/dlt/destinations/job_client_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/job_impl.py` & `dlt-0.2.6a0/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/postgres/__init__.py` & `dlt-0.2.6a0/dlt/destinations/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/postgres/postgres.py` & `dlt-0.2.6a0/dlt/destinations/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/postgres/sql_client.py` & `dlt-0.2.6a0/dlt/destinations/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/redshift/README.md` & `dlt-0.2.6a0/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/redshift/__init__.py` & `dlt-0.2.6a0/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/redshift/redshift.py` & `dlt-0.2.6a0/dlt/destinations/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/sql_client.py` & `dlt-0.2.6a0/dlt/destinations/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/sql_merge_job.py` & `dlt-0.2.6a0/dlt/destinations/sql_merge_job.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/destinations/typing.py` & `dlt-0.2.6a0/dlt/destinations/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,16 @@
         ...
 
     def rollback_transaction(self) -> None:
         ...
 
 
 class DBApi(Protocol):
-    threadsafety: bool
-    apilevel: bool
+    threadsafety: int
+    apilevel: str
     paramstyle: str
 
 
 class DBApiCursor(Protocol):
     """Protocol for DBAPI cursor"""
     description: Tuple[Any, ...]
```

### Comparing `dlt-0.2.5a1/dlt/extract/decorators.py` & `dlt-0.2.6a0/dlt/extract/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.exceptions import ArgumentsOverloadException
 from dlt.common.schema.schema import Schema
 from dlt.common.schema.typing import TColumnKey, TColumnName, TTableSchemaColumns, TWriteDisposition
 from dlt.common.storages.exceptions import SchemaNotFoundError
 from dlt.common.storages.schema_storage import SchemaStorage
 from dlt.common.typing import AnyFun, ParamSpec, Concatenate, TDataItem, TDataItems
-from dlt.common.utils import get_callable_name, is_inner_callable
+from dlt.common.utils import get_callable_name, get_module_name, is_inner_callable
 from dlt.extract.exceptions import InvalidTransformerDataTypeGeneratorFunctionRequired, ResourceFunctionExpected, ResourceInnerCallableConfigWrapDisallowed, SourceDataIsNone, SourceIsAClassTypeError, SourceNotAFunction, SourceSchemaNotAvailable
 from dlt.extract.incremental import IncrementalResourceWrapper
 
 from dlt.extract.typing import TTableHintTemplate
 from dlt.extract.source import DltResource, DltSource, TUnboundDltResource
 
 
@@ -87,26 +87,28 @@
     schema: Schema = None,
     spec: Type[BaseConfiguration] = None
 ) -> Any:
     """A decorator that transforms a function returning one or more `dlt resources` into a `dlt source` in order to load it with `dlt`.
 
     ### Summary
     A `dlt source` is a logical grouping of resources that are often extracted and loaded together. A source is associated with a schema, which describes the structure of the loaded data and provides instructions how to load it.
-    Such schema contains table schemas that describe the structure of the data coming from the resources. See https://dlthub.com/docs/glossary for more basic term definitions.
+    Such schema contains table schemas that describe the structure of the data coming from the resources.
+
+    Please refer to https://dlthub.com/docs/general-usage/source for a complete documentation.
 
     ### Passing credentials
     Another important function of the source decorator is to provide credentials and other configuration to the code that extracts data. The decorator may automatically bind the source function arguments to the secret and config values.
     >>> @dlt.source
-    >>> def chess(username, chess_url: str = dlt.config.value, api_secret = dlt.secret.value, title: str = "GM"):
+    >>> def chess(username, chess_url: str = dlt.config.value, api_secret = dlt.secrets.value, title: str = "GM"):
     >>>     return user_profile(username, chess_url, api_secret), user_games(username, chess_url, api_secret, with_titles=title)
     >>>
     >>> list(chess("magnuscarlsen"))
 
     Here `username` is a required, explicit python argument, `chess_url` is a required argument, that if not explicitly passed will be taken from configuration ie. `config.toml`, `api_secret` is a required argument, that if not explicitly passed will be taken from dlt secrets ie. `secrets.toml`.
-    See https://dlthub.com/docs/customization/credentials for details.
+    See https://dlthub.com/docs/general-usage/credentials for details.
 
     ### Args:
         func: A function that returns a dlt resource or a list of those or a list of any data items that can be loaded by `dlt`.
 
         name (str, optional): A name of the source which is also the name of the associated schema. If not present, the function name will be used.
 
         section (str, optional): A name of configuration and state sections. If not present, the current python module name will be used.
@@ -251,26 +253,28 @@
     depends_on: TUnboundDltResource = None,
 ) -> Any:
     """When used as a decorator, transforms any generator (yielding) function into a `dlt resource`. When used as a function, it transforms data in `data` argument into a `dlt resource`.
 
     ### Summary
     A `resource`is a location within a `source` that holds the data with specific structure (schema) or coming from specific origin. A resource may be a rest API endpoint, table in the database or a tab in Google Sheets.
     A `dlt resource` is python representation of a `resource` that combines both data and metadata (table schema) that describes the structure and instructs the loading of the data.
-    A `dlt resource` is also an `Iterable` and can used like any other similar object ie. list or tuple. See https://dlthub.com/docs/glossary for more on basic term definitions.
+    A `dlt resource` is also an `Iterable` and can used like any other iterable object ie. list or tuple.
+
+    Please refer to https://dlthub.com/docs/general-usage/resource for a complete documentation.
 
     ### Passing credentials
     If used as a decorator (`data` argument is a `Generator`), it may automatically bind the source function arguments to the secret and config values.
     >>> @dlt.resource
-    >>> def user_games(username, chess_url: str = dlt.config.value, api_secret = dlt.secret.value):
+    >>> def user_games(username, chess_url: str = dlt.config.value, api_secret = dlt.secrets.value):
     >>>     return requests.get("%s/games/%s" % (chess_url, username), headers={"Authorization": f"Bearer {api_secret}"})
     >>>
     >>> list(user_games("magnuscarlsen"))
 
     Here `username` is a required, explicit python argument, `chess_url` is a required argument, that if not explicitly passed will be taken from configuration ie. `config.toml`, `api_secret` is a required argument, that if not explicitly passed will be taken from dlt secrets ie. `secrets.toml`.
-    See https://dlthub.com/docs/customization/credentials for details.
+    See https://dlthub.com/docs/general-usage/credentials for details.
     Note that if decorated function is an inner function, passing of the credentials will be disabled.
 
     ### Args:
         data (Callable | Any, optional): a function to be decorated or a data compatible with `dlt` `run`.
 
         name (str, optional): A name of the resource that by default also becomes the name of the table to which the data is loaded.
         If not present, the name of the decorated function will be used.
@@ -281,16 +285,18 @@
         write_disposition (Literal["skip", "append", "replace", "merge"], optional): Controls how to write data to a table. `append` will always add new data at the end of the table. `replace` will replace existing data with new data. `skip` will prevent data from loading. "merge" will deduplicate and merge data based on "primary_key" and "merge_key" hints. Defaults to "append".
         This argument also accepts a callable that is used to dynamically create tables for stream-like resources yielding many datatypes.
 
         columns (Sequence[TColumnSchema], optional): A list of column schemas. Typed dictionary describing column names, data types, write disposition and performance hints that gives you full control over the created table schema.
         This argument also accepts a callable that is used to dynamically create tables for stream-like resources yielding many datatypes.
 
         primary_key (str | Sequence[str]): A column name or a list of column names that comprise a private key. Typically used with "merge" write disposition to deduplicate loaded data.
+        This argument also accepts a callable that is used to dynamically create tables for stream-like resources yielding many datatypes.
 
         merge_key (str | Sequence[str]): A column name or a list of column names that define a merge key. Typically used with "merge" write disposition to remove overlapping data ranges ie. to keep a single record for a given day.
+        This argument also accepts a callable that is used to dynamically create tables for stream-like resources yielding many datatypes.
 
         selected (bool, optional): When `True` `dlt pipeline` will extract and load this resource, if `False`, the resource will be ignored.
 
         spec (Type[BaseConfiguration], optional): A specification of configuration and secret values required by the source.
 
         depends_on (TUnboundDltResource, optional): Allows to pipe data from one resource to another to build multi-step pipelines.
 
@@ -431,15 +437,15 @@
     parent_fun = ".".join(parts[:-2])
     return _SOURCES.get(parent_fun)
 
 
 def _get_source_section_name(m: ModuleType) -> str:
     if hasattr(m, "__source_name__"):
         return cast(str, m.__source_name__)
-    return m.__name__.split(".")[-1]
+    return get_module_name(m)
 
 
 def get_source_schema() -> Schema:
     """When executed from the function decorated with @dlt.source, returns a writable source Schema"""
     try:
         return Container()[SourceSchemaInjectableContext].schema
     except ContextDefaultCannotBeCreated:
```

### Comparing `dlt-0.2.5a1/dlt/extract/exceptions.py` & `dlt-0.2.6a0/dlt/extract/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
         super().__init__(resource_name, msg)
 
 
 class ResourceInnerCallableConfigWrapDisallowed(DltResourceException):
     def __init__(self, resource_name: str, section: str) -> None:
         self.section = section
-        msg = f"Resource {resource_name} in section {section} is defined over an inner function and requests config/secrets in its arguments. Requesting secret and config values via 'dlt.secret.values' or 'dlt.config.value' is disallowed for resources that are inner functions. Use the dlt.source to get the required configuration and pass them explicitly to your source."
+        msg = f"Resource {resource_name} in section {section} is defined over an inner function and requests config/secrets in its arguments. Requesting secret and config values via 'dlt.secrets.values' or 'dlt.config.value' is disallowed for resources that are inner functions. Use the dlt.source to get the required configuration and pass them explicitly to your source."
         super().__init__(resource_name, msg)
 
 
 class InvalidResourceDataTypeIsNone(InvalidResourceDataType):
     def __init__(self, resource_name: str, item: Any, _typ: Type[Any]) -> None:
         super().__init__(resource_name, item, _typ, "Resource data missing. Did you forget the return statement in @dlt.resource decorated function?")
```

### Comparing `dlt-0.2.5a1/dlt/extract/extract.py` & `dlt-0.2.6a0/dlt/extract/extract.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/extract/incremental.py` & `dlt-0.2.6a0/dlt/extract/incremental.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from dlt.common.typing import DictStrAny, TDataItem, TDataItems, TFun, extract_inner_type, is_optional_type
 from dlt.common.schema.typing import TColumnKey
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import BaseConfiguration
 from dlt.common.pipeline import _resource_state
 from dlt.common.utils import digest128
 from dlt.extract.exceptions import PipeException
+from dlt.extract.pipe import Pipe
 from dlt.extract.utils import resolve_column_value
 from dlt.extract.typing import FilterItem, SupportsPipe, TTableHintTemplate
 
 
 TCursorValue = TypeVar("TCursorValue", bound=Any)
 LastValueFunc = Callable[[Sequence[TCursorValue]], Any]
 
@@ -68,15 +69,15 @@
     >>> r = some_data().add_step(dlt.sources.incremental("item.ts", initial_value=now, primary_key="delta"))
     >>> info = p.run(r, destination="duckdb")
 
     Args:
         cursor_path: The name or a JSON path to an cursor field. Uses the same names of fields as in your JSON document, before they are normalized to store in the database.
         initial_value: Optional value used for `last_value` when no state is available, e.g. on the first run of the pipeline. If not provided `last_value` will be `None` on the first run.
         last_value_func: Callable used to determine which cursor value to save in state. It is called with a list of the stored state value and all cursor vals from currently processing items. Default is `max`
-        primary_key: Optional primary key used to deduplicate data. If not provided, a primary key defined by the resource will be used. Pass a tuple to define a compound key
+        primary_key: Optional primary key used to deduplicate data. If not provided, a primary key defined by the resource will be used. Pass a tuple to define a compound key. Pass empty tuple to disable unique checks
     """
     cursor_path: str = None
     initial_value: Optional[Any] = None
 
     def __init__(
             self,
             cursor_path: str = dlt.config.value,
@@ -85,30 +86,33 @@
             primary_key: Optional[TTableHintTemplate[TColumnKey]] = None
     ) -> None:
         self.cursor_path = cursor_path
         if self.cursor_path:
             self.cursor_path_p: JSONPath = jsonpath_parse(cursor_path)
         self.last_value_func = last_value_func
         self.initial_value = initial_value
+        """Initial value of last_value"""
+        self.start_value: Any = initial_value
+        """Value of last_value at the beginning of current pipeline run"""
         self.resource_name: Optional[str] = None
         self.primary_key: Optional[TTableHintTemplate[TColumnKey]] = primary_key
         self._cached_state: IncrementalColumnState = None
         """State dictionary cached on first access"""
         super().__init__(self.transform)
 
     @classmethod
     def from_existing_state(cls, resource_name: str, cursor_path: str) -> "Incremental[TCursorValue]":
         """Create Incremental instance from existing state."""
-        state = Incremental.get_state(resource_name, cursor_path)
+        state = Incremental._get_state(resource_name, cursor_path)
         i = cls(cursor_path, state["initial_value"])
         i.resource_name = resource_name
         return i
 
     def copy(self) -> "Incremental[TCursorValue]":
-        return self.__class__(self.cursor_path, initial_value=self.initial_value, last_value_func=self.last_value_func)
+        return self.__class__(self.cursor_path, initial_value=self.initial_value, last_value_func=self.last_value_func, primary_key=self.primary_key)
 
     def on_resolved(self) -> None:
         self.cursor_path_p = jsonpath_parse(self.cursor_path)
 
     def parse_native_representation(self, native_value: Any) -> None:
         if isinstance(native_value, Incremental):
             self.cursor_path = native_value.cursor_path
@@ -117,94 +121,98 @@
             self.cursor_path_p = self.cursor_path_p
             self.resource_name = self.resource_name
         else:  # TODO: Maybe check if callable(getattr(native_value, '__lt__', None))
             # Passing bare value `incremental=44` gets parsed as initial_value
             self.initial_value = native_value
         self.__is_resolved__ = not self.is_partial()
 
-
-    def get_cached_state(self) -> IncrementalColumnState:
-        """Given resource state, returns a Incremental state for particular cursor column"""
-        if self._cached_state:
-            return self._cached_state
-        self._cached_state = Incremental.get_state(self.resource_name, self.cursor_path)
+    def get_state(self) -> IncrementalColumnState:
+        """Returns an Incremental state for a particular cursor column"""
+        self._cached_state = Incremental._get_state(self.resource_name, self.cursor_path)
         if len(self._cached_state) == 0:
             # set the default like this, setdefault evaluates the default no matter if it is needed or not. and our default is heavy
             self._cached_state.update(
                 {
                     "initial_value": self.initial_value,
                     "last_value": self.initial_value,
                     'unique_hashes': []
                 }
             )
         return self._cached_state
 
     @staticmethod
-    def get_state(resource_name: str, cursor_path: str) -> IncrementalColumnState:
+    def _get_state(resource_name: str, cursor_path: str) -> IncrementalColumnState:
         state: IncrementalColumnState = _resource_state(resource_name).setdefault('incremental', {}).setdefault(cursor_path, {})
         # if state params is empty
         return state
 
     @property
     def last_value(self) -> Optional[TCursorValue]:
-        s = self.get_cached_state()
+        s = self.get_state()
         return s['last_value']  # type: ignore
 
     def unique_value(self, row: TDataItem) -> str:
         try:
             if self.primary_key:
                 return digest128(json.dumps(resolve_column_value(self.primary_key, row), sort_keys=True))
-            else:
+            elif self.primary_key is None:
                 return digest128(json.dumps(row, sort_keys=True))
+            else:
+                return None
         except KeyError as k_err:
             raise IncrementalPrimaryKeyMissing(self.resource_name, k_err.args[0], row)
 
     def transform(self, row: TDataItem) -> bool:
         if row is None:
             return True
 
         row_values = self.cursor_path_p.find(row)
         if len(row_values) == 0:
             raise IncrementalCursorPathMissing(self.resource_name, self.cursor_path, row)
 
         incremental_state = self._cached_state
         last_value = incremental_state['last_value']
         row_value = row_values[0].value  # For now the value needs to match deserialized presentation from state
-        check_values = [row_value] + ([last_value] if last_value is not None else [])
+        check_values = (row_value,) + ((last_value, ) if last_value is not None else ())
         new_value = self.last_value_func(check_values)
         if last_value == new_value:
             # we store row id for all records with the current "last_value" in state and use it to deduplicate
-            if self.last_value_func([row_value]) == last_value:
+            if self.last_value_func((row_value, )) == last_value:
                 unique_value = self.unique_value(row)
-                if unique_value in incremental_state['unique_hashes']:
-                    return False
-                # add new hash only if the record row id is same as current last value
-                incremental_state['unique_hashes'].append(unique_value)
+                # if unique value exists then use it to deduplicate
+                if unique_value:
+                    if unique_value in incremental_state['unique_hashes']:
+                        return False
+                    # add new hash only if the record row id is same as current last value
+                    incremental_state['unique_hashes'].append(unique_value)
                 return True
             # skip the record that is not a last_value or new_value: that record was already processed
-            check_values = ([self.initial_value] if self.initial_value is not None else []) + [row_value]
+            check_values = (row_value,) + ((self.start_value,) if self.start_value is not None else ())
             new_value = self.last_value_func(check_values)
-            if new_value == self.initial_value:
+            if new_value == self.start_value:
                 return False
             else:
                 return True
         if new_value != last_value:
+            incremental_state["last_value"] = new_value
             unique_value = self.unique_value(row)
-            incremental_state.update({'last_value': new_value, 'unique_hashes': [unique_value]})
+            if unique_value:
+                incremental_state["unique_hashes"] = [unique_value]
         return True
 
     def bind(self, pipe: SupportsPipe) -> "Incremental[TCursorValue]":
         "Called by pipe just before evaluation"
         # bind the resource/pipe name
-        if self.resource_name is None:
-            self.resource_name = pipe.name
         if self.is_partial():
             raise IncrementalCursorPathMissing(pipe.name, None, None)
-        # fill cache
-        self.get_cached_state()
+        self.resource_name = pipe.name
+        # set initial value from last value, in case of a new state those are equal
+        self.start_value = self.last_value
+        # cache state
+        self._cached_state = self.get_state()
         return self
 
     def __str__(self) -> str:
         return f"Incremental at {id(self)} for resource {self.resource_name} with cursor path: {self.cursor_path} initial {self.initial_value} lv_func {self.last_value_func}"
 
 
 class IncrementalResourceWrapper(FilterItem):
@@ -238,18 +246,15 @@
         assert incremental_param, "Please use `should_wrap` to decide if to call this function"
 
         @wraps(func)
         def _wrap(*args: Any, **kwargs: Any) -> Any:
             p = incremental_param
             assert p is not None
             new_incremental: Incremental[Any] = None
-
             bound_args = sig.bind(*args, **kwargs)
-            if isinstance(p.default, Incremental):
-                new_incremental = p.default.copy()
 
             if p.name in bound_args.arguments:
                 explicit_value = bound_args.arguments[p.name]
                 if isinstance(explicit_value, Incremental):
                     # Explicit Incremental instance is untouched
                     new_incremental = explicit_value.copy()
                 elif isinstance(p.default, Incremental):
@@ -260,22 +265,29 @@
                 new_incremental = p.default.copy()
 
             if not new_incremental or new_incremental.is_partial():
                 if is_optional_type(p.annotation):
                     bound_args.arguments[p.name] = None  # Remove partial spec
                     return func(*bound_args.args, **bound_args.kwargs)
                 raise ValueError(f"{p.name} Incremental has no default")
-            new_incremental.resource_name = self.resource_name
-            # set initial value from last value, in case of a new state those are equal
-            # this will also cache state in incremental
-            new_incremental.initial_value = new_incremental.last_value
-            self._incremental = new_incremental
-            bound_args.arguments[p.name] = new_incremental
+            # set the incremental only if not yet set or if it was passed explicitly
+            # NOTE: the _incremental may be also set by applying hints to the resource see `set_template` in `DltResource`
+            if p.name in bound_args.arguments or not self._incremental:
+                self._incremental = new_incremental
+            # in case of transformers the bind will be called before this wrapper is set: because transformer is called for a first time late in the pipe
+            self._incremental.bind(Pipe(self.resource_name))
+            bound_args.arguments[p.name] = self._incremental
             return func(*bound_args.args, **bound_args.kwargs)
 
         return _wrap  # type: ignore
 
+    def bind(self, pipe: SupportsPipe) -> "IncrementalResourceWrapper":
+        if self._incremental:
+            self._incremental.bind(pipe)
+        return self
+
     def __call__(self, item: TDataItems, meta: Any = None) -> Optional[TDataItems]:
         if not self._incremental:
             return item
-        self._incremental.primary_key = self.primary_key
+        if self._incremental.primary_key is None:
+            self._incremental.primary_key = self.primary_key
         return self._incremental(item, meta)
```

### Comparing `dlt-0.2.5a1/dlt/extract/pipe.py` & `dlt-0.2.6a0/dlt/extract/pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,17 +133,17 @@
     def tail(self) -> TPipeStep:
         return self._steps[-1]
 
     @property
     def steps(self) -> List[TPipeStep]:
         return self._steps
 
-    def find(self, step_type: AnyType) -> int:
+    def find(self, *step_type: AnyType) -> int:
         """Finds a step with object of type `step_type`"""
-        return next((i for i,v in enumerate(self._steps) if type(v) is step_type), -1)
+        return next((i for i,v in enumerate(self._steps) if type(v) in step_type), -1)
 
     def __getitem__(self, i: int) -> TPipeStep:
         return self._steps[i]
 
     def __len__(self) -> int:
         return len(self._steps)
 
@@ -233,19 +233,14 @@
             raise ParametrizedResourceUnbound(self.name, callable_name, sig.replace(parameters=list(sig.parameters.values())[1:]), "resource", str(ex))
 
     def evaluate_gen(self) -> None:
         """Lazily evaluate gen of the pipe when creating PipeIterator. Allows creating multiple use pipes from generator functions and lists"""
         if not self.is_data_bound:
             raise PipeNotBoundToData(self.name, self.has_parent)
 
-        # evaluate transforms
-        for step_no, step in enumerate(self._steps):
-            if isinstance(step, ItemTransform):
-                self._steps[step_no] = step.bind(self)
-
         gen = self.gen
         if not self.has_parent:
             if callable(gen):
                 try:
                     # must be parameter-less callable or parameters must have defaults
                     self.replace_gen(gen())  # type: ignore
                 except TypeError as ex:
@@ -253,14 +248,20 @@
             # otherwise it must be an iterator
             if isinstance(gen, Iterable):
                 self.replace_gen(iter(gen))
         else:
             # verify if transformer can be called
             self._ensure_transform_step(self._gen_idx, gen)
 
+        # evaluate transforms
+        for step_no, step in enumerate(self._steps):
+            # print(f"pipe {self.name} step no {step_no} step({step})")
+            if isinstance(step, ItemTransform):
+                self._steps[step_no] = step.bind(self)
+
     def bind_gen(self, *args: Any, **kwargs: Any) -> Any:
         """Finds and wraps with `args` + `kwargs` the callable generating step in the resource pipe and then replaces the pipe gen with the wrapped one"""
         try:
             gen = self._wrap_gen(*args, **kwargs)
             self.replace_gen(gen)
             return gen
         except InvalidResourceDataTypeFunctionNotAGenerator:
@@ -313,19 +314,17 @@
                 if len(sig.parameters) == 0:
                     return head
 
                 # always wrap generators and generator functions. evaluate only at runtime!
 
                 def _partial() -> Any:
                     # print(f"_PARTIAL: {args} {kwargs} vs {args_}{kwargs_}")
-                    # raise Exception("WTF")
                     return head(*args, **kwargs)  # type: ignore
 
                 # this partial preserves the original signature and just defers the call to pipe
-                # _data = makefun.wraps(head, new_sig=sig)(_partial)
                 _data = makefun.wraps(head, new_sig=inspect.signature(_partial))(_partial)
             else:
                 raise InvalidResourceDataTypeFunctionNotAGenerator(self.name, head, type(head))
         return _data
 
     def _verify_head_step(self, step: TPipeStep) -> None:
         # first element must be Iterable, Iterator or Callable in resource pipe
```

### Comparing `dlt-0.2.5a1/dlt/extract/schema.py` & `dlt-0.2.6a0/dlt/extract/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 from copy import copy, deepcopy
 from collections.abc import Mapping as C_Mapping
-from typing import List, cast, Any
+from typing import List, TypedDict, cast, Any
 
 from dlt.common.schema.utils import DEFAULT_WRITE_DISPOSITION, merge_columns, new_column, new_table
 from dlt.common.schema.typing import TColumnProp, TColumnSchema, TPartialTableSchema, TTableSchemaColumns, TWriteDisposition
 from dlt.common.typing import TDataItem
 from dlt.common.validation import validate_dict
 
-from dlt.extract.typing import TColumnKey, TFunHintTemplate, TTableHintTemplate, TTableSchemaTemplate
+from dlt.extract.incremental import Incremental
+from dlt.extract.typing import TColumnKey, TFunHintTemplate, TTableHintTemplate
 from dlt.extract.exceptions import DataItemRequiredForDynamicTableHints, InconsistentTableTemplate, TableNameMissing
 
 
+class TTableSchemaTemplate(TypedDict, total=False):
+    name: TTableHintTemplate[str]
+    # description: TTableHintTemplate[str]
+    write_disposition: TTableHintTemplate[TWriteDisposition]
+    # table_sealed: Optional[bool]
+    parent: TTableHintTemplate[str]
+    columns: TTableHintTemplate[TTableSchemaColumns]
+    primary_key: TTableHintTemplate[TColumnKey]
+    merge_key: TTableHintTemplate[TColumnKey]
+    incremental: Incremental[Any]
+
+
 class DltResourceSchema:
     def __init__(self, name: str, table_schema_template: TTableSchemaTemplate = None):
         self.__qualname__ = self.__name__ = self._name = name
         self._table_name_hint_fun: TFunHintTemplate[str] = None
         self._table_has_other_dynamic_hints: bool = False
         self._table_schema_template: TTableSchemaTemplate = None
         if table_schema_template:
@@ -36,41 +49,52 @@
             raise DataItemRequiredForDynamicTableHints(self._name)
         else:
             return w_d
 
     def table_schema(self, item: TDataItem =  None) -> TPartialTableSchema:
         """Computes the table schema based on hints and column definitions passed during resource creation. `item` parameter is used to resolve table hints based on data"""
         if not self._table_schema_template:
-            return new_table(self._name)
+            return new_table(self._name, resource=self._name)
 
         # resolve a copy of a held template
         table_template = copy(self._table_schema_template)
         table_template["columns"] = copy(self._table_schema_template["columns"])
 
         # if table template present and has dynamic hints, the data item must be provided
         if self._table_name_hint_fun and item is None:
             raise DataItemRequiredForDynamicTableHints(self._name)
         # resolve
         resolved_template: TTableSchemaTemplate = {k: self._resolve_hint(item, v) for k, v in table_template.items()}  # type: ignore
+        resolved_template.pop("incremental", None)
         table_schema = self._merge_keys(resolved_template)
+        table_schema["resource"] = self._name
         validate_dict(TPartialTableSchema, table_schema, f"new_table/{self._name}")
         return table_schema
 
     def apply_hints(
         self,
         table_name: TTableHintTemplate[str] = None,
         parent_table_name: TTableHintTemplate[str] = None,
         write_disposition: TTableHintTemplate[TWriteDisposition] = None,
         columns: TTableHintTemplate[TTableSchemaColumns] = None,
         primary_key: TTableHintTemplate[TColumnKey] = None,
-        merge_key: TTableHintTemplate[TColumnKey] = None
+        merge_key: TTableHintTemplate[TColumnKey] = None,
+        incremental: Incremental[Any] = None
     ) -> None:
-        """Allows to create or modify existing table schema by setting provided hints. Accepts dynamic hints based on data.
-           Pass None to keep old value
-           Pass empty value (for particular type) to remove hint
+        """Creates or modifies existing table schema by setting provided hints. Accepts both static and dynamic hints based on data.
+
+           This method accepts the same table hints arguments as `dlt.resource` decorator with the following additions.
+           Skip the argument or pass None to leave the existing hint.
+           Pass empty value (for particular type ie "" for a string) to remove hint
+
+           parent_table_name (str, optional): A name of parent table if foreign relation is defined. Please note that if you use merge you must define `root_key` columns explicitly
+           incremental (Incremental, optional): Enables the incremental loading for a resource.
+
+           Please note that for efficient incremental loading, the resource must be aware of the Incremental by accepting it as one if its arguments and then using is to skip already loaded data.
+           In non-aware resources, `dlt` will filter out the loaded values, however the resource will yield all the values again.
         """
         t = None
         if not self._table_schema_template:
             # if there's no template yet, create and set new one
             t = self.new_table_template(table_name, parent_table_name, write_disposition, columns, primary_key, merge_key)
         else:
             # set single hints
@@ -89,14 +113,15 @@
                 t["write_disposition"] = write_disposition
             if columns is not None:
                 t["columns"] = columns
             if primary_key is not None:
                 t["primary_key"] = primary_key
             if merge_key is not None:
                 t["merge_key"] = merge_key
+            t["incremental"] = incremental
         self.set_template(t)
 
     def set_template(self, table_schema_template: TTableSchemaTemplate) -> None:
         # if "name" is callable in the template then the table schema requires actual data item to be inferred
         name_hint = table_schema_template["name"]
         if callable(name_hint):
             self._table_name_hint_fun = name_hint
```

### Comparing `dlt-0.2.5a1/dlt/extract/source.py` & `dlt-0.2.6a0/dlt/extract/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 from dlt.common.configuration.resolve import inject_section
 from dlt.common.configuration.specs import known_sections
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.normalizers.json.relational import DataItemNormalizer as RelationalNormalizer, RelationalNormalizerConfigPropagation
 from dlt.common.schema import Schema
 from dlt.common.schema.typing import TColumnName
-from dlt.common.typing import AnyFun, TDataItem, TDataItems, NoneType
+from dlt.common.typing import AnyFun, StrAny, TDataItem, TDataItems, NoneType
 from dlt.common.configuration.container import Container
-from dlt.common.pipeline import PipelineContext, StateInjectableContext, SupportsPipelineRun, state_value
+from dlt.common.pipeline import PipelineContext, StateInjectableContext, SupportsPipelineRun, _resource_state, source_state, pipeline_state
 from dlt.common.utils import flatten_list_or_items, get_callable_name, multi_context_manager, uniq_id
 
-from dlt.extract.typing import DataItemWithMeta, ItemTransformFunc, ItemTransformFunctionWithMeta, TableNameMeta, TTableSchemaTemplate, FilterItem, MapItem, YieldMapItem
+from dlt.extract.typing import DataItemWithMeta, ItemTransformFunc, ItemTransformFunctionWithMeta, TableNameMeta, FilterItem, MapItem, YieldMapItem
 from dlt.extract.pipe import Pipe, ManagedPipeIterator
-from dlt.extract.schema import DltResourceSchema
-from dlt.extract.incremental import IncrementalResourceWrapper
+from dlt.extract.schema import DltResourceSchema, TTableSchemaTemplate
+from dlt.extract.incremental import Incremental, IncrementalResourceWrapper
 from dlt.extract.exceptions import (
     InvalidTransformerDataTypeGeneratorFunctionRequired, InvalidParentResourceDataType, InvalidParentResourceIsAFunction, InvalidResourceDataType, InvalidResourceDataTypeFunctionNotAGenerator, InvalidResourceDataTypeIsNone, InvalidTransformerGeneratorFunction,
     DataItemRequiredForDynamicTableHints, InvalidResourceDataTypeAsync, InvalidResourceDataTypeBasic,
     InvalidResourceDataTypeMultiplePipes, ParametrizedResourceUnbound, ResourceNameMissing, ResourceNotATransformer, ResourcesNotFoundError, SourceExhausted, DeletingResourcesNotSupported)
 
 
 def with_table_name(item: TDataItems, table_name: str) -> DataItemWithMeta:
@@ -121,15 +121,15 @@
         except (TypeError, ParametrizedResourceUnbound):
             return True
 
     @property
     def incremental(self) -> IncrementalResourceWrapper:
         """Gets incremental transform if it is in the pipe"""
         incremental: IncrementalResourceWrapper = None
-        step_no = self._pipe.find(IncrementalResourceWrapper)
+        step_no = self._pipe.find(IncrementalResourceWrapper, Incremental)
         if step_no >= 0:
             incremental = self._pipe.steps[step_no]  # type: ignore
         return incremental
 
     def pipe_data_from(self, data_from: Union["DltResource", Pipe]) -> None:
         """Replaces the parent in the transformer resource pipe from which the data is piped."""
         if self.is_transformer:
@@ -218,17 +218,26 @@
         else:
             self._pipe.insert_step(item_transform, insert_at)
         return self
 
     def set_template(self, table_schema_template: TTableSchemaTemplate) -> None:
         super().set_template(table_schema_template)
         incremental = self.incremental
+        # try to late assign incremental
+        if table_schema_template.get("incremental") is not None:
+            if incremental:
+                incremental._incremental = table_schema_template["incremental"]
+            else:
+                # if there's no wrapper add incremental as a transform
+                incremental = table_schema_template["incremental"]  # type: ignore
+                self.add_step(incremental)
+
         if incremental:
             primary_key = table_schema_template.get("primary_key", incremental.primary_key)
-            if primary_key:
+            if primary_key is not None:
                 incremental.primary_key = primary_key
 
     def bind(self, *args: Any, **kwargs: Any) -> "DltResource":
         """Binds the parametrized resource to passed arguments. Modifies resource pipe in place. Does not evaluate generators or iterators."""
         if self._bound:
             raise TypeError("Bound DltResource object is not callable")
         gen = self._pipe.bind_gen(*args, **kwargs)
@@ -247,14 +256,20 @@
             self._pipe.__dict__.clear()
             # write props from new pipe instance
             self._pipe.__dict__.update(gen.__dict__)
         else:
             self._bound = True
         return self
 
+    @property
+    def state(self) -> StrAny:
+        """Gets resource-scoped state from the existing pipeline context. If pipeline context is not available, PipelineStateNotAvailable is raised"""
+        with self._get_config_section_context():
+            return _resource_state(self.name)
+
     def __call__(self, *args: Any, **kwargs: Any) -> "DltResource":
         """Binds the parametrized resources to passed arguments. Creates and returns a bound resource. Generators and iterators are not evaluated."""
         if self._bound:
             raise TypeError("Bound DltResource object is not callable")
         r = DltResource.from_data(self._pipe._clone(keep_pipe_id=False), self._name, self.section, self._table_schema_template, self.selected, self._pipe.parent)
         return r.bind(*args, **kwargs)
 
@@ -275,33 +290,36 @@
     def __iter__(self) -> Iterator[TDataItem]:
         """Opens iterator that yields the data items from the resources in the same order as in Pipeline class.
 
             A read-only state is provided, initialized from active pipeline state. The state is discarded after the iterator is closed.
         """
         # use the same state dict when opening iterator and when iterator is iterated
         container = Container()
-        state, _ = state_value(container, {})
-        # get section should be active pipeline name
-        proxy = container[PipelineContext]
-        pipeline_name = uniq_id() if not proxy.is_active() else proxy.pipeline().pipeline_name
+        state, _ = pipeline_state(container, {})
 
         def _get_context() -> List[ContextManager[Any]]:
             return [
-                inject_section(ConfigSectionContext(sections=(known_sections.SOURCES, self.section or pipeline_name, self._name))),
+                self._get_config_section_context(),
                 Container().injectable_context(StateInjectableContext(state=state))
             ]
 
         # managed pipe iterator will remove injected contexts when closing
         with multi_context_manager(_get_context()):
             pipe_iterator: ManagedPipeIterator = ManagedPipeIterator.from_pipe(self._pipe)  # type: ignore
 
         pipe_iterator.set_context_manager(multi_context_manager(_get_context()))
         _iter = map(lambda item: item.item, pipe_iterator)
         return flatten_list_or_items(_iter)
 
+    def _get_config_section_context(self) -> ContextManager[ConfigSectionContext]:
+        container = Container()
+        proxy = container[PipelineContext]
+        pipeline_name = uniq_id() if not proxy.is_active() else proxy.pipeline().pipeline_name
+        return inject_section(ConfigSectionContext(sections=(known_sections.SOURCES, self.section or pipeline_name, self._name)))
+
     def __str__(self) -> str:
         info = f"DltResource {self._name}"
         if self.section:
             info += f" in section {self.section}:"
         else:
             info += ":"
         if self.is_transformer:
@@ -363,17 +381,18 @@
 
 # produce Empty resource singleton
 DltResource.Empty = DltResource(Pipe(None), None, False)
 TUnboundDltResource = Callable[[], DltResource]
 
 
 class DltResourceDict(Dict[str, DltResource]):
-    def __init__(self, source_name: str) -> None:
+    def __init__(self, source_name: str, source_section: str) -> None:
         super().__init__()
         self.source_name = source_name
+        self.source_section = source_section
         self._recently_added: List[DltResource] = []
         self._known_pipes: Dict[str, DltResource] = {}
 
     @property
     def selected(self) -> Dict[str, DltResource]:
         """Returns a subset of all resources that will be extracted and loaded to the destination."""
         return {k:v for k,v in self.items() if v.selected}
@@ -388,15 +407,16 @@
         for resource in self.selected.values():
             while (pipe := resource._pipe.parent) is not None:
                 if not pipe.is_empty:
                     try:
                         resource = self.find_by_pipe(pipe)
                     except KeyError:
                         # resource for pipe not found: return mock resource
-                        resource = DltResource(pipe, resource._table_schema_template, False, section=resource.section)
+                        mock_template = DltResourceSchema.new_table_template(pipe.name, write_disposition=resource._table_schema_template.get("write_disposition"))
+                        resource = DltResource(pipe, mock_template, False, section=resource.section)
                     extracted[resource._name] = resource
                 else:
                     break
         return extracted
 
     @property
     def pipes(self) -> List[Pipe]:
@@ -435,14 +455,15 @@
         for cloned in cloned_pipes:
             self.find_by_pipe(cloned)._pipe = cloned
         self._recently_added.clear()
 
     def __setitem__(self, resource_name: str, resource: DltResource) -> None:
         # make shallow copy of the resource
         resource = copy(resource)
+        resource.section = self.source_section
         # now set it in dict
         self._recently_added.append(resource)
         return super().__setitem__(resource_name, resource)
 
     def __delitem__(self, resource_name: str) -> None:
         raise DeletingResourcesNotSupported(self.source_name, resource_name)
 
@@ -461,15 +482,15 @@
     """
     def __init__(self, name: str, section: str, schema: Schema, resources: Sequence[DltResource] = None) -> None:
         self.name = name
         self.section = section
         self.exhausted = False
         """Tells if iterator associated with a source is exhausted"""
         self._schema = schema
-        self._resources: DltResourceDict = DltResourceDict(self.name)
+        self._resources: DltResourceDict = DltResourceDict(self.name, self.section)
         if resources:
             for resource in resources:
                 self._add_resource(resource._name, resource)
             self._resources.clone_new_pipes()
 
     @classmethod
     def from_data(cls, name: str, section: str, schema: Schema, data: Any) -> "DltSource":
@@ -555,60 +576,69 @@
 
     @property
     def run(self) -> SupportsPipelineRun:
         """A convenience method that will call `run` run on the currently active `dlt` pipeline. If pipeline instance is not found, one with default settings will be created."""
         self_run: SupportsPipelineRun = makefun.partial(Container()[PipelineContext].pipeline().run, *(), data=self)
         return self_run
 
-    def _add_resource(self, name: str, resource: DltResource) -> None:
-        if self.exhausted:
-            raise SourceExhausted(self.name)
-
-        if name in self._resources:
-            # for resources with the same name try to add the resource as an another pipe
-            self._resources[name].add_pipe(resource)
-        else:
-            self._resources[name] = resource
-            # remember that resource got cloned when set into dict
-            super().__setattr__(name, self._resources[name])
-
-    def __getattr__(self, resource_name: str) -> DltResource:
-        return self._resources[resource_name]
-
-    def __setattr__(self, name: str, value: Any) -> None:
-        if isinstance(value, DltResource):
-            # TODO: refactor adding resources. 1. resource dict should be read only 2. we should correct the parent pipes after cloning 3. allow replacing existing resources
-            self._add_resource(name, value)
-        else:
-            super().__setattr__(name, value)
+    @property
+    def state(self) -> StrAny:
+        """Gets source-scoped state from the existing pipeline context. If pipeline context is not available, PipelineStateNotAvailable is raised"""
+        with self._get_config_section_context():
+            return source_state()
 
     def __iter__(self) -> Iterator[TDataItem]:
         """Opens iterator that yields the data items from all the resources within the source in the same order as in Pipeline class.
 
             A read-only state is provided, initialized from active pipeline state. The state is discarded after the iterator is closed.
 
             A source config section is injected to allow secrets/config injection as during regular extraction.
         """
         # use the same state dict when opening iterator and when iterator is iterated
-        mock_state, _ = state_value(Container(), {})
+        mock_state, _ = pipeline_state(Container(), {})
 
         def _get_context() -> List[ContextManager[Any]]:
             return [
-                inject_section(ConfigSectionContext(sections=(known_sections.SOURCES, self.section, self.name))),
+                self._get_config_section_context(),
                 Container().injectable_context(StateInjectableContext(state=mock_state))
             ]
 
         # managed pipe iterator will remove injected contexts when closing
         with multi_context_manager(_get_context()):
             pipe_iterator: ManagedPipeIterator = ManagedPipeIterator.from_pipes(self._resources.selected_pipes)  # type: ignore
         pipe_iterator.set_context_manager(multi_context_manager(_get_context()))
         _iter = map(lambda item: item.item, pipe_iterator)
         self.exhausted = True
         return flatten_list_or_items(_iter)
 
+    def _get_config_section_context(self) -> ContextManager[ConfigSectionContext]:
+        return inject_section(ConfigSectionContext(sections=(known_sections.SOURCES, self.section, self.name)))
+
+    def _add_resource(self, name: str, resource: DltResource) -> None:
+        if self.exhausted:
+            raise SourceExhausted(self.name)
+
+        if name in self._resources:
+            # for resources with the same name try to add the resource as an another pipe
+            self._resources[name].add_pipe(resource)
+        else:
+            self._resources[name] = resource
+            # remember that resource got cloned when set into dict
+            super().__setattr__(name, self._resources[name])
+
+    def __getattr__(self, resource_name: str) -> DltResource:
+        return self._resources[resource_name]
+
+    def __setattr__(self, name: str, value: Any) -> None:
+        if isinstance(value, DltResource):
+            # TODO: refactor adding resources. 1. resource dict should be read only 2. we should correct the parent pipes after cloning 3. allow replacing existing resources
+            self._add_resource(name, value)
+        else:
+            super().__setattr__(name, value)
+
     def __str__(self) -> str:
         info = f"DltSource {self.name} section {self.section} contains {len(self.resources)} resource(s) of which {len(self.selected_resources)} are selected"
         for r in self.resources.values():
             selected_info = "selected" if r.selected else "not selected"
             if r.is_transformer:
                 info += f"\ntransformer {r._name} is {selected_info} and takes data from {r._pipe.parent.name}"
             else:
```

### Comparing `dlt-0.2.5a1/dlt/extract/typing.py` & `dlt-0.2.6a0/dlt/extract/typing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,24 @@
 import inspect
 from abc import ABC, abstractmethod
-from typing import Any, Callable, Generic, Iterator, Optional, Protocol, TypedDict, TypeVar, Union, Awaitable, Sequence
+from typing import Any, Callable, Generic, Iterator, Optional, Protocol, TypedDict, TypeVar, Union, Awaitable
 
-from dlt.common.typing import TAny, TDataItem, TDataItems, TypeAlias
+from dlt.common.typing import TAny, TDataItem, TDataItems
 from dlt.common.schema.typing import TTableSchemaColumns, TWriteDisposition, TColumnKey
 
 
 TDeferredDataItems = Callable[[], TDataItems]
 TAwaitableDataItems = Awaitable[TDataItems]
 TPipedDataItems = Union[TDataItems, TDeferredDataItems, TAwaitableDataItems]
 
 TDynHintType = TypeVar("TDynHintType")
 TFunHintTemplate = Callable[[TDataItem], TDynHintType]
 TTableHintTemplate = Union[TDynHintType, TFunHintTemplate[TDynHintType]]
 
 
-class TTableSchemaTemplate(TypedDict, total=False):
-    name: TTableHintTemplate[str]
-    # description: TTableHintTemplate[str]
-    write_disposition: TTableHintTemplate[TWriteDisposition]
-    # table_sealed: Optional[bool]
-    parent: TTableHintTemplate[str]
-    columns: TTableHintTemplate[TTableSchemaColumns]
-    primary_key: TTableHintTemplate[TColumnKey]
-    merge_key: TTableHintTemplate[TColumnKey]
-
-
 class DataItemWithMeta:
     __slots__ = "meta", "data"
 
     meta: Any
     data: TDataItems
 
     def __init__(self, meta: Any, data: TDataItems) -> None:
```

### Comparing `dlt-0.2.5a1/dlt/extract/utils.py` & `dlt-0.2.6a0/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/helpers/dbt/__init__.py` & `dlt-0.2.6a0/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/helpers/dbt/configuration.py` & `dlt-0.2.6a0/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.2.6a0/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/helpers/dbt/exceptions.py` & `dlt-0.2.6a0/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/helpers/dbt/profiles.yml` & `dlt-0.2.6a0/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/helpers/dbt/runner.py` & `dlt-0.2.6a0/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/helpers/pandas.py` & `dlt-0.2.6a0/dlt/helpers/pandas.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/helpers/parquet.py` & `dlt-0.2.6a0/dlt/helpers/parquet.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/helpers/streamlit.py` & `dlt-0.2.6a0/dlt/helpers/streamlit.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,35 +90,41 @@
 
 #     with open(SECRETS_FILE_LOC, "w", encoding="utf-8") as f:
 #         # use whitespace preserving parser
 #         tomlkit.dump(secrets_, f)
 
 
 def write_load_status_page(pipeline: Pipeline) -> None:
-    """Display pipeline loading information. Will be moved to python-dlt once tested"""
+    """Display pipeline loading information. Will be moved to dlt package once tested"""
 
     @cache_data(ttl=600)
     def _query_data(query: str, schema_name: str = None) -> pd.DataFrame:
         with pipeline.sql_client(schema_name) as client:
             with client.execute_query(query) as curr:
                 return curr.df()
 
+    @cache_data(ttl=5)
+    def _query_data_live(query: str, schema_name: str = None) -> pd.DataFrame:
+        with pipeline.sql_client(schema_name) as client:
+            with client.execute_query(query) as curr:
+                return curr.df()
+
     try:
         st.header("Pipeline info")
         credentials = pipeline.sql_client().credentials
         st.markdown(f"""
         * pipeline name: **{pipeline.pipeline_name}**
         * destination: **{str(credentials)}** in **{pipeline.destination.__name__}**
         * dataset name: **{pipeline.dataset_name}**
         * default schema name: **{pipeline.default_schema_name}**
         """)
 
         st.header("Last load info")
         col1, col2, col3 = st.columns(3)
-        loads_df = _query_data(
+        loads_df = _query_data_live(
             f"SELECT load_id, inserted_at FROM {LOADS_TABLE_NAME} WHERE status = 0 ORDER BY inserted_at DESC LIMIT 101 "
         )
         loads_no = loads_df.shape[0]
         if loads_df.shape[0] > 0:
             rel_time = humanize.naturaldelta(pendulum.now() - pendulum.from_timestamp(loads_df.iloc[0, 1].timestamp())) + " ago"
             last_load_id = loads_df.iloc[0, 0]
             if loads_no > 100:
@@ -135,31 +141,28 @@
         schema = pipeline.default_schema
 
         # construct a union query
         query_parts = []
         for table in schema.data_tables():
             if "parent" in table:
                 continue
-            if "columns" not in table or len(table["columns"]) == 0:
-                continue
-
             table_name = table["name"]
             query_parts.append(f"SELECT '{table_name}' as table_name, COUNT(1) As rows_count FROM {table_name} WHERE _dlt_load_id = '{selected_load_id}'")
             query_parts.append("UNION ALL")
         query_parts.pop()
         rows_counts_df = _query_data("\n".join(query_parts))
 
         st.markdown(f"Rows loaded in **{selected_load_id}**")
         st.dataframe(rows_counts_df)
 
         st.markdown("**Last 100 loads**")
         st.dataframe(loads_df)
 
         st.header("Schema updates")
-        schemas_df = _query_data(
+        schemas_df = _query_data_live(
             f"SELECT schema_name, inserted_at, version, version_hash FROM {VERSION_TABLE_NAME} ORDER BY inserted_at DESC LIMIT 101 "
             )
         st.markdown("**100 recent schema updates**")
         st.dataframe(schemas_df)
 
         st.header("Pipeline state info")
         with pipeline.sql_client() as client:
@@ -202,26 +205,25 @@
         example_query (str, optional): Example query to be displayed in the SQL Query box.
         show_charts (bool, optional): Should automatically show charts for the queries from SQL Query box. Defaults to True.
 
     Raises:
         MissingDependencyException: Raised when a particular python dependency is not installed
     """
 
-    @cache_data(ttl=600)
+    @cache_data(ttl=60)
     def _query_data(query: str, chunk_size: int = None) -> pd.DataFrame:
         with pipeline.sql_client(schema_name) as client:
             with client.execute_query(query) as curr:
                 return curr.df(chunk_size=chunk_size)
 
     if schema_name:
         schema = pipeline.schemas[schema_name]
     else:
         schema = pipeline.default_schema
     st.title(f"Available tables in {schema.name} schema")
-    # st.text(schema.to_pretty_yaml())
 
     for table in schema.data_tables():
         table_name = table["name"]
         st.header(table_name)
         if "description" in table:
             st.text(table["description"])
         if "parent" in table:
@@ -290,15 +292,15 @@
 def display(pipeline_name: str) -> None:
     import dlt
 
     pipeline = dlt.attach(pipeline_name)
 
     pages: Dict[str, AnyFun] = {
         "Explore data": write_data_explorer_page,
-        "Pipeline info": write_load_status_page,
+        "Load info": write_load_status_page,
     }
 
     st.title(f"Show {pipeline_name} pipeline")
 
     st.sidebar.title("Navigation")
     selection = st.sidebar.radio("Go to", list(pages.keys()))
     page = pages[selection]
```

### Comparing `dlt-0.2.5a1/dlt/load/configuration.py` & `dlt-0.2.6a0/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/load/exceptions.py` & `dlt-0.2.6a0/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/load/load.py` & `dlt-0.2.6a0/dlt/load/load.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/normalize/configuration.py` & `dlt-0.2.6a0/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/normalize/normalize.py` & `dlt-0.2.6a0/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/pipeline/README.md` & `dlt-0.2.6a0/dlt/pipeline/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/pipeline/__init__.py` & `dlt-0.2.6a0/dlt/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/pipeline/configuration.py` & `dlt-0.2.6a0/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/pipeline/dbt.py` & `dlt-0.2.6a0/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/pipeline/exceptions.py` & `dlt-0.2.6a0/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/pipeline/helpers.py` & `dlt-0.2.6a0/dlt/pipeline/helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/pipeline/pipeline.py` & `dlt-0.2.6a0/dlt/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,17 @@
 from dlt.common.destination.reference import DestinationReference, JobClientBase, DestinationClientConfiguration, DestinationClientDwhConfiguration, TDestinationReferenceArg
 from dlt.common.pipeline import ExtractInfo, LoadInfo, NormalizeInfo, SupportsPipeline, TPipelineLocalState, TPipelineState, StateInjectableContext
 from dlt.common.schema import Schema
 from dlt.common.storages.file_storage import FileStorage
 from dlt.common.utils import is_interactive
 
 from dlt.destinations.exceptions import DatabaseUndefinedRelation
-from dlt.extract.decorators import SourceSchemaInjectableContext
 
 from dlt.extract.exceptions import DataItemRequiredForDynamicTableHints, SourceExhausted
-from dlt.extract.extract import ExtractorStorage, extract, extract_with_schema
+from dlt.extract.extract import ExtractorStorage, extract_with_schema
 from dlt.extract.source import DltResource, DltSource
 from dlt.extract.typing import TColumnKey
 from dlt.normalize import Normalize
 from dlt.normalize.configuration import NormalizeConfiguration
 from dlt.destinations.sql_client import SqlClientBase
 from dlt.destinations.job_client_impl import SqlJobClientBase
 from dlt.load.configuration import LoaderConfiguration
@@ -191,15 +190,15 @@
 
         self.pipeline_salt = pipeline_salt
         self.config = config
         self.runtime_config = runtime
         self.full_refresh = full_refresh
 
         self._container = Container()
-        self._pipeline_instance_id = pendulum.now().format("_YYYYMMDDhhmmss")
+        self._pipeline_instance_id = self._create_pipeline_instance_id()
         self._pipeline_storage: FileStorage = None
         self._schema_storage: LiveSchemaStorage = None
         self._schema_storage_config: SchemaVolumeConfiguration = None
         self._normalize_storage_config: NormalizeVolumeConfiguration = None
         self._load_storage_config: LoadVolumeConfiguration = None
         self._trace: PipelineTrace = None
         self._last_trace: PipelineTrace = None
@@ -434,18 +433,20 @@
             self._state_restored = True
 
         # normalize and load pending data
         if self.list_extracted_resources():
             self.normalize()
         if self.list_normalized_load_packages():
             # if there were any pending loads, load them and **exit**
+            if data is not None:
+                logger.warn("The pipeline `run` method will now load the pending load packages. The data you passed to the run function will not be loaded. In order to do that you must run the pipeline again")
             return self.load(destination, dataset_name, credentials=credentials)
 
         # extract from the source
-        if data:
+        if data is not None:
             self.extract(data, table_name=table_name, write_disposition=write_disposition, columns=columns, primary_key=primary_key, schema=schema)
             self.normalize()
             return self.load(destination, dataset_name, credentials=credentials)
         else:
             return None
 
     @with_schemas_sync
@@ -713,18 +714,19 @@
             if table_name or parent_table_name or write_disposition or columns or primary_key:
                 resource_table_name: str = None
                 with contextlib.suppress(DataItemRequiredForDynamicTableHints):
                     resource_table_name = resource.table_name
                 resource.apply_hints(table_name or resource_table_name or resource.name, parent_table_name, write_disposition, columns_dict, primary_key)
 
         def choose_schema() -> Schema:
+            """Except of explicitly passed schema, use a clone that will get discarded if extraction fails"""
             if schema:
                 return schema
             if self.default_schema_name:
-                return self.default_schema
+                return self.default_schema.clone()
             return self._make_schema_with_default_name()
 
         effective_schema = choose_schema()
 
         # a list of sources or a list of resources may be passed as data
         sources: List[DltSource] = []
         resources: List[DltResource] = []
@@ -765,39 +767,37 @@
             # add all the appended resources in one source
             sources.append(DltSource(effective_schema.name, self.pipeline_name, effective_schema, resources))
 
         return sources
 
     def _extract_source(self, storage: ExtractorStorage, source: DltSource, max_parallel_items: int, workers: int) -> str:
         # discover the schema from source
-        # TODO: do not save any schemas here and do not set default schema, just generate all the schemas and save them one all data is extracted
         source_schema = source.schema
-        pipeline_schema: Schema = None
-        with contextlib.suppress(FileNotFoundError):
-            pipeline_schema = self._schema_storage.load_schema(source_schema.name)
+
+        # make CTRL-C working while running user code
+        with signals.raise_immediately():
+            extract_id = extract_with_schema(storage, source, source_schema, max_parallel_items, workers)
 
         # if source schema does not exist in the pipeline
         if source_schema.name not in self._schema_storage:
             # save schema into the pipeline
             self._schema_storage.save_schema(source_schema)
-        pipeline_schema = self._schema_storage[source_schema.name]
 
         # and set as default if this is first schema in pipeline
         if not self.default_schema_name:
             # this performs additional validations as schema contains the naming module
             self._set_default_schema_name(source_schema)
 
-        # make CTRL-C working while running user code
-        with signals.raise_immediately():
-            extract_id = extract_with_schema(storage, source, source_schema, max_parallel_items, workers)
+        pipeline_schema = self._schema_storage[source_schema.name]
 
         # initialize import with fully discovered schema
         self._schema_storage.save_import_schema_if_not_exists(source_schema)
 
-        # get the current schema and merge tables from source_schema, we'll not merge the high level props
+        # get the current schema and merge tables from source_schema
+        # note we are not merging props like max nesting or column propagation
         for table in source_schema.data_tables():
             pipeline_schema.update_schema(pipeline_schema.normalize_table_identifiers(table))
 
         return extract_id
 
     def _run_step_in_pool(self, step: TPipelineStep, runnable: Runnable[Any], config: PoolRunnerConfiguration) -> int:
         # TODO: remove runner altogether. it does not fit into current architecture
@@ -945,14 +945,17 @@
         self._validate_dataset_name(dataset_name)
         self.dataset_name = dataset_name
 
     def _set_default_schema_name(self, schema: Schema) -> None:
         assert self.default_schema_name is None
         self.default_schema_name = schema.name
 
+    def _create_pipeline_instance_id(self) -> str:
+        return pendulum.now().format("_YYYYMMDDhhmmss")  # type: ignore
+
     @with_schemas_sync
     @with_state_sync()
     def _inject_schema(self, schema: Schema) -> None:
         """Injects a schema into the pipeline. Existing schema will be overwritten"""
         self._schema_storage.save_schema(schema)
         if not self.default_schema_name:
             self._set_default_schema_name(schema)
```

### Comparing `dlt-0.2.5a1/dlt/pipeline/state_sync.py` & `dlt-0.2.6a0/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/pipeline/trace.py` & `dlt-0.2.6a0/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/pipeline/track.py` & `dlt-0.2.6a0/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/reflection/names.py` & `dlt-0.2.6a0/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/reflection/script_inspector.py` & `dlt-0.2.6a0/dlt/reflection/script_inspector.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,20 @@
 def patch__init__(self: Any, *args: Any, **kwargs: Any) -> None:
     raise PipelineIsRunning(self, args, kwargs)
 
 
 class DummyModule(ModuleType):
     """A dummy module from which you can import anything"""
     def __getattr__(self, key: str) -> Any:
-        return SimpleNamespace()
+        if key[0].isupper():
+            # if imported name is capitalized, import type
+            return SimpleNamespace
+        else:
+            # otherwise import instance
+            return SimpleNamespace()
     __all__: List[Any] = []   # support wildcard imports
 
 
 def _import_module(name: str, missing_modules: Tuple[str, ...] = ()) -> ModuleType:
     """Module importer that ignores missing modules by importing a dummy module"""
 
     def _try_import(name: str, _globals: Mapping[str, Any] = None, _locals: Mapping[str, Any] = None, fromlist: Sequence[str] = (), level:int = 0) -> ModuleType:
```

### Comparing `dlt-0.2.5a1/dlt/reflection/script_visitor.py` & `dlt-0.2.6a0/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/sources/helpers/requests/__init__.py` & `dlt-0.2.6a0/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/sources/helpers/requests/retry.py` & `dlt-0.2.6a0/dlt/sources/helpers/requests/retry.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     def _make_session(self) -> Session:
         session = Session(**self._session_kwargs)  # type: ignore[arg-type]
         for key, value in self._session_attrs.items():
             setattr(session, key, value)
         session.mount('http://', self._adapter)
         session.mount('https://', self._adapter)
         retry = _make_retry(**self._retry_kwargs)  # type: ignore[arg-type]
-        session.request = retry.wraps(session.request)  # type: ignore[assignment]
+        session.request = retry.wraps(session.request)  # type: ignore[method-assign]
         return session
 
     @property
     def session(self) -> Session:
         session: Optional[Session] = getattr(self._local, 'session', None)
         if session is None:
             session = self._local.session = self._make_session()
```

### Comparing `dlt-0.2.5a1/dlt/sources/helpers/requests/session.py` & `dlt-0.2.6a0/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/sources/helpers/transform.py` & `dlt-0.2.6a0/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/dlt/version.py` & `dlt-0.2.6a0/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.5a1/pyproject.toml` & `dlt-0.2.6a0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.2.5a1"
+version = "0.2.6a0"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
@@ -47,15 +47,14 @@
 astunparse = ">=1.6.3"
 cron-descriptor = ">=1.2.32"
 pipdeptree = ">=2.3.3"
 gitpython = ">=3.1.29"
 pytz = ">=2022.6"
 tqdm = ">=4.64.1"
 giturlparse = ">=0.10.0"
-reretry = ">=0.11.8"
 orjson = {version = "^3.8.6", markers="platform_python_implementation != 'PyPy'"}
 
 psycopg2-binary = {version = ">=2.9.1", optional = true}
 # use this dependency as the current version of psycopg2cffi does not have sql module
 # psycopg2cffi = {git = "https://github.com/chtd/psycopg2cffi.git", optional = true, markers="platform_python_implementation == 'PyPy'"}
 psycopg2cffi = {version = ">=2.9.0", optional = true, markers="platform_python_implementation == 'PyPy'"}
 
@@ -67,19 +66,20 @@
 
 dbt-core = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-redshift = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-bigquery = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-duckdb = {version = ">=1.3.0,<1.5.0", optional = true}
 tenacity = "^8.2.2"
 jsonpath-ng = "^1.5.3"
+deprecated = "^1.2.13"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
-mypy = "0.982"
+mypy = "1.2.0"
 flake8 = "^5.0.0"
 bandit = "^1.7.0"
 flake8-bugbear = "^22.0.0"
 pytest-pythonpath = "^0.7.3"
 pytest-order = "^1.0.0"
 pytest-cases = "^3.6.9"
 pytest-forked = "^1.3.0"
@@ -107,11 +107,19 @@
 dlt = "dlt.cli._dlt:_main"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.10.0"
 types-click = "^7.1.8"
 pandas = "^1.5.3"
 sqlfluff = "^1.4.5"
+google-auth-oauthlib = "^1.0.0"
+types-deprecated = "^1.2.9.2"
+
+[tool.poetry.group.airflow]
+optional = true
+
+[tool.poetry.group.airflow.dependencies]
+apache-airflow = "^2.5.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.8"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dlt-0.2.5a1/PKG-INFO` & `dlt-0.2.6a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.2.5a1
+Version: 0.2.6a0
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
@@ -30,40 +30,40 @@
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: SQLAlchemy (>=1.4.0)
 Requires-Dist: astunparse (>=1.6.3)
 Requires-Dist: asyncstdlib (>=3.10.5)
 Requires-Dist: cachetools (>=5.2.0)
 Requires-Dist: click (>=7.1)
 Requires-Dist: cron-descriptor (>=1.2.32)
-Requires-Dist: dbt-bigquery (>=1.3.0,<1.5.0) ; extra == "dbt"
-Requires-Dist: dbt-core (>=1.3.0,<1.5.0) ; extra == "dbt"
-Requires-Dist: dbt-duckdb (>=1.3.0,<1.5.0) ; extra == "dbt"
-Requires-Dist: dbt-redshift (>=1.3.0,<1.5.0) ; extra == "dbt"
-Requires-Dist: duckdb (>=0.6.1,<0.8.0) ; extra == "duckdb"
+Requires-Dist: dbt-bigquery (>=1.3.0,<1.5.0); extra == "dbt"
+Requires-Dist: dbt-core (>=1.3.0,<1.5.0); extra == "dbt"
+Requires-Dist: dbt-duckdb (>=1.3.0,<1.5.0); extra == "dbt"
+Requires-Dist: dbt-redshift (>=1.3.0,<1.5.0); extra == "dbt"
+Requires-Dist: deprecated (>=1.2.13,<2.0.0)
+Requires-Dist: duckdb (>=0.6.1,<0.8.0); extra == "duckdb"
 Requires-Dist: gitpython (>=3.1.29)
 Requires-Dist: giturlparse (>=0.10.0)
-Requires-Dist: google-cloud-bigquery (>=2.26.0) ; extra == "gcp" or extra == "bigquery"
-Requires-Dist: grpcio (>=1.50.0) ; extra == "gcp" or extra == "bigquery"
+Requires-Dist: google-cloud-bigquery (>=2.26.0); extra == "gcp" or extra == "bigquery"
+Requires-Dist: grpcio (>=1.50.0); extra == "gcp" or extra == "bigquery"
 Requires-Dist: hexbytes (>=0.2.2)
 Requires-Dist: humanize (>=4.4.0)
 Requires-Dist: json-logging (==1.4.1rc0)
 Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0)
 Requires-Dist: makefun (>=1.15.0)
-Requires-Dist: orjson (>=3.8.6,<4.0.0) ; platform_python_implementation != "PyPy"
+Requires-Dist: orjson (>=3.8.6,<4.0.0); platform_python_implementation != "PyPy"
 Requires-Dist: pathvalidate (>=2.5.2)
 Requires-Dist: pendulum (>=2.1.2)
 Requires-Dist: pipdeptree (>=2.3.3)
 Requires-Dist: prometheus-client (>=0.11.0)
-Requires-Dist: psycopg2-binary (>=2.9.1) ; extra == "postgres" or extra == "redshift"
-Requires-Dist: psycopg2cffi (>=2.9.0) ; (platform_python_implementation == "PyPy") and (extra == "postgres" or extra == "redshift")
-Requires-Dist: pyarrow (>=8.0.0) ; extra == "gcp" or extra == "bigquery"
+Requires-Dist: psycopg2-binary (>=2.9.1); extra == "postgres" or extra == "redshift"
+Requires-Dist: psycopg2cffi (>=2.9.0); (platform_python_implementation == "PyPy") and (extra == "postgres" or extra == "redshift")
+Requires-Dist: pyarrow (>=8.0.0); extra == "gcp" or extra == "bigquery"
 Requires-Dist: pytz (>=2022.6)
 Requires-Dist: requests (>=2.26.0)
 Requires-Dist: requirements-parser (>=0.5.0)
-Requires-Dist: reretry (>=0.11.8)
 Requires-Dist: semver (>=2.13.0)
 Requires-Dist: sentry-sdk (>=1.4.3)
 Requires-Dist: setuptools (>=65.6.0)
 Requires-Dist: simplejson (>=3.17.5)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tomlkit (>=0.11.3)
 Requires-Dist: tqdm (>=4.64.1)
@@ -72,89 +72,107 @@
 Project-URL: Repository, https://github.com/dlt-hub/dlt
 Description-Content-Type: text/markdown
 
 ![](https://github.com/dlt-hub/dlt/raw/devel/docs/DLT-Pacman-Big.gif)
 
 <p align="center">
 
-[![PyPI version](https://badge.fury.io/py/python-dlt.svg)](https://pypi.org/project/python-dlt/)
+[![PyPI version](https://badge.fury.io/py/dlt.svg)](https://pypi.org/project/dlt/)
 [![LINT Badge](https://github.com/dlt-hub/dlt/actions/workflows/lint.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/lint.yml)
 [![TEST COMMON Badge](https://github.com/dlt-hub/dlt/actions/workflows/test_common.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/test_common.yml)
 [![TEST DESTINATIONS Badge](https://github.com/dlt-hub/dlt/actions/workflows/test_destinations.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/test_destinations.yml)
 [![TEST BIGQUERY Badge](https://github.com/dlt-hub/dlt/actions/workflows/test_destination_bigquery.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/test_destination_bigquery.yml)
 [![TEST DBT Badge](https://github.com/dlt-hub/dlt/actions/workflows/test_dbt_runner.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/test_dbt_runner.yml)
 
-
 </p>
 
 # data load tool (dlt)
 
-**[Colab Demo](https://colab.research.google.com/drive/1BXvma_9R9MX8p_iSvHE4ebg90sUroty2)**
+**[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**
 
 ```python
 import dlt
 from chess import chess # a utility function that grabs data from the chess.com API
 
 # create a dlt pipeline that will load chess game data to the DuckDB destination
-pipeline = dlt.pipeline(pipeline_name="chess_pipeline", destination='duckdb', dataset_name="games_data")
+pipeline = dlt.pipeline(
+    pipeline_name='chess_pipeline',
+    destination='duckdb',
+    dataset_name='games_data'
+)
 
 # use chess.com API to grab data about a few players
-data = chess(['magnuscarlsen', 'rpragchess'], start_month="2022/11", end_month="2022/12")
+data = chess(['magnuscarlsen', 'rpragchess'], start_month='2022/11', end_month='2022/12')
 
 # extract, normalize, and load the data
 pipeline.run(data)
 ```
 
-**data load tool (dlt)** is a simple, open source Python library that makes data loading easy
+**data load tool (dlt)** is an open source Python library that makes data loading easy
+
 - Automatically turn the JSON returned by any API into a live dataset stored wherever you want it
-- `pip install python-dlt` and then include `import dlt` to use it in your Python loading script
+- `pip install dlt` and then include `import dlt` to use it in your Python loading script
 - The **dlt** library is licensed under the Apache License 2.0, so you can use it for free forever
 
 Read more about it on the [dlt Docs](https://dlthub.com/docs)
 
 # semantic versioning
-`python-dlt` will follow the semantic versioning with [`MAJOR.MINOR.PATCH`](https://peps.python.org/pep-0440/#semantic-versioning) pattern. Currently we do **pre-release versioning** with major version being 0.
+
+`dlt` will follow the semantic versioning with [`MAJOR.MINOR.PATCH`](https://peps.python.org/pep-0440/#semantic-versioning) pattern. Currently we do **pre-release versioning** with major version being 0.
+
 - `minor` version change means breaking changes
 - `patch` version change means new features that should be backward compatible
 - any suffix change ie. `a10` -> `a11` is a patch
 
 # development
-`python-dlt` uses `poetry` to manage, build and version the package. It also uses `make` to automate tasks. To start
+
+`dlt` uses `poetry` to manage, build and version the package. It also uses `make` to automate tasks. To start
+
 ```sh
 make install-poetry  # will install poetry, to be run outside virtualenv
 ```
+
 then
+
 ```sh
 make dev  # will install all deps including dev
 ```
+
 Executing `poetry shell` and working in it is very convenient at this moment.
 
 ## python version
-Use python 3.8 for development which is the lowest supported version for `python-dlt`. You'll need `distutils` and `venv`:
+
+Use python 3.8 for development which is the lowest supported version for `dlt`. You'll need `distutils` and `venv`:
 
 ```shell
 sudo apt-get install python3.8
 sudo apt-get install python3.8-distutils
 sudo apt install python3.8-venv
 ```
+
 You may also use `pyenv` as [poetry](https://python-poetry.org/docs/managing-environments/) suggests.
 
 ## bumping version
+
 Please use `poetry version prerelease` to bump patch and then `make build-library` to apply changes. The source of the version is `pyproject.toml` and we use poetry to manage it.
 
 ## testing and linting
-`python-dlt` uses `mypy` and `flake8` with several plugins for linting. We do not reorder imports or reformat code.
+
+`dlt` uses `mypy` and `flake8` with several plugins for linting. We do not reorder imports or reformat code.
 
 `pytest` is used as test harness. `make test-common` will run tests of common components and does not require any external resources.
 
 ### testing destinations
+
 To test destinations use `make test`. You will need following external resources
+
 1. `BigQuery` project
 2. `Redshift` cluster
 3. `Postgres` instance. You can find a docker compose for postgres instance [here](tests/load/postgres/docker-compose.yml). When run the instance is configured to work with the tests.
+
 ```shell
 cd tests/load/postgres/
 docker-compose up --build -d
 ```
 
 See `tests/.example.env` for the expected environment variables and command line example to run the tests. Then create `tests/.env` from it. You configure the tests as you would configure the dlt pipeline.
 We'll provide you with access to the resources above if you wish to test locally.
@@ -162,21 +180,24 @@
 To test local destinations (`duckdb` and `postgres`) run `make test-local`. You can run this tests without additional credentials (just copy `.example.env` into `.env`)
 
 ## publishing
 
 1. Make sure that you are on `devel` branch and you have the newest code that passed all tests on CI.
 2. Verify the current version with `poetry version`
 3. You'll need `pypi` access token and use `poetry config pypi-token.pypi your-api-token` then
+
 ```
 make publish-library
 ```
+
 4. Make a release on github, use version and git tag as release name
 
 ## contributing
 
 To contribute via pull request:
+
 1. Create an issue with your idea for a feature etc.
 2. Write your code and tests
 3. Lint your code with `make lint`. Test the common modules with `make test-common`
 4. If you work on a destination code then contact us to get access to test destinations
 5. Create a pull request
```

