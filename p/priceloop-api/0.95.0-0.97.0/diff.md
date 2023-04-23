# Comparing `tmp/priceloop-api-0.95.0.tar.gz` & `tmp/priceloop-api-0.97.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "priceloop-api-0.95.0.tar", last modified: Wed Apr 19 20:21:03 2023, max compression
+gzip compressed data, was "priceloop-api-0.97.0.tar", last modified: Sun Apr 23 21:11:52 2023, max compression
```

## Comparing `priceloop-api-0.95.0.tar` & `priceloop-api-0.97.0.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.441188 priceloop-api-0.95.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-19 20:21:03.437188 priceloop-api-0.95.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.429188 priceloop-api-0.95.0/priceloop_api/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.429188 priceloop-api-0.95.0/priceloop_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.429188 priceloop-api-0.95.0/priceloop_api/api/column_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/column_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/column_api/add_data_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/column_api/add_formula_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/column_api/delete_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/column_api/get_column_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/column_api/update_column_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/column_api/update_column_is_gui_locked.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/column_api/update_column_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/column_api/update_column_visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.429188 priceloop-api-0.95.0/priceloop_api/api/external_function_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/external_function_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/external_function_api/create_external_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/external_function_api/delete_external_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/external_function_api/get_external_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/external_function_api/update_external_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.429188 priceloop-api-0.95.0/priceloop_api/api/import_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/import_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/import_api/create_csv_import_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/import_api/get_table_upload_csv_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.429188 priceloop-api-0.95.0/priceloop_api/api/other/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/other/hello.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/other/hello_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.433188 priceloop-api-0.95.0/priceloop_api/api/plugin_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/plugin_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/plugin_api/create_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/plugin_api/get_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/plugin_api/get_plugin_live_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/plugin_api/get_plugin_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/plugin_api/list_enabled_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/plugin_api/prepare_ape_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/plugin_api/set_plugin_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/plugin_api/set_plugin_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.433188 priceloop-api-0.95.0/priceloop_api/api/plugin_webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/plugin_webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/plugin_webhooks/add_plugin_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/plugin_webhooks/delete_plugin_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/plugin_webhooks/list_plugin_webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.433188 priceloop-api-0.95.0/priceloop_api/api/table_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/table_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/table_api/create_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/table_api/delete_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/table_api/get_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/table_api/get_table_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/table_api/truncate_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.433188 priceloop-api-0.95.0/priceloop_api/api/workspace_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/workspace_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/workspace_api/create_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/workspace_api/get_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/api/workspace_api/list_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.437188 priceloop-api-0.95.0/priceloop_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/add_data_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/add_plugin_webhook_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/add_plugin_webhook_plugin_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/amazon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/ape_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/ape_data_typeform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/api_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/api_column_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/api_column_attributes_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/api_external_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/api_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/api_table_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/api_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/column_attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/column_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/create_csv_import_job_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/create_external_function_return_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/create_external_function_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/create_plugin_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/csv_separator.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/delete_plugin_webhook_plugin_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/get_plugin_live_status_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/get_plugin_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/get_plugin_tokens_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/get_table_upload_csv_url_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/import_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/import_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/list_enabled_workspaces_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/list_plugin_webhooks_plugin_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/plugin_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/plugin_data_type_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/plugin_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/plugin_live_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/plugin_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/plugin_workspace_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/plugin_workspace_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/prepare_ape_tables_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/presigned_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/s3_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/set_plugin_external_data_json_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/set_plugin_external_data_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/set_plugin_status_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/set_plugin_status_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/table_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/table_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/webhook_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/webhook_event_selector_type_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/models/webhook_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.437188 priceloop-api-0.95.0/priceloop_api/priceloop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/priceloop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.437188 priceloop-api-0.95.0/priceloop_api/priceloop/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/priceloop/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/priceloop/auth/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/priceloop/auth/priceloop_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.437188 priceloop-api-0.95.0/priceloop_api/priceloop/data/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/priceloop/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/priceloop/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/priceloop_api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:21:03.429188 priceloop-api-0.95.0/priceloop_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-19 20:21:03.000000 priceloop-api-0.95.0/priceloop_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-19 20:21:03.000000 priceloop-api-0.95.0/priceloop_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:21:03.000000 priceloop-api-0.95.0/priceloop_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-19 20:21:03.000000 priceloop-api-0.95.0/priceloop_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 20:21:03.000000 priceloop-api-0.95.0/priceloop_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:21:03.441188 priceloop-api-0.95.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-19 20:20:51.000000 priceloop-api-0.95.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.672646 priceloop-api-0.97.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-23 21:11:52.672646 priceloop-api-0.97.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.652645 priceloop-api-0.97.0/priceloop_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.656645 priceloop-api-0.97.0/priceloop_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.656645 priceloop-api-0.97.0/priceloop_api/api/column_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/column_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/column_api/add_data_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/column_api/add_formula_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/column_api/delete_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/column_api/get_column_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/column_api/update_column_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/column_api/update_column_is_gui_locked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/column_api/update_column_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/column_api/update_column_visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.656645 priceloop-api-0.97.0/priceloop_api/api/external_function_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/external_function_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/external_function_api/create_external_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/external_function_api/delete_external_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/external_function_api/get_external_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/external_function_api/update_external_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.656645 priceloop-api-0.97.0/priceloop_api/api/import_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/import_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/import_api/create_csv_import_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/import_api/get_table_upload_csv_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.656645 priceloop-api-0.97.0/priceloop_api/api/other/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/other/hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/other/hello_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.660645 priceloop-api-0.97.0/priceloop_api/api/plugin_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/plugin_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/plugin_api/create_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/plugin_api/get_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/plugin_api/get_plugin_live_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/plugin_api/get_plugin_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/plugin_api/list_enabled_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/plugin_api/prepare_ape_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/plugin_api/set_plugin_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/plugin_api/set_plugin_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.660645 priceloop-api-0.97.0/priceloop_api/api/plugin_webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/plugin_webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/plugin_webhooks/add_plugin_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/plugin_webhooks/delete_plugin_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/plugin_webhooks/list_plugin_webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.660645 priceloop-api-0.97.0/priceloop_api/api/table_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/table_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/table_api/create_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/table_api/delete_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/table_api/get_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/table_api/get_table_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/table_api/truncate_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.660645 priceloop-api-0.97.0/priceloop_api/api/workspace_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/workspace_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/workspace_api/create_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/workspace_api/get_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/api/workspace_api/list_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.672646 priceloop-api-0.97.0/priceloop_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/add_data_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/add_plugin_webhook_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/add_plugin_webhook_plugin_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/amazon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/ape_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/ape_data_typeform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/api_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/api_column_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/api_column_attributes_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/api_external_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/api_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/api_table_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/api_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/column_attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/column_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/create_csv_import_job_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/create_external_function_return_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/create_external_function_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/create_plugin_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/csv_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/delete_plugin_webhook_plugin_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/get_plugin_live_status_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/get_plugin_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/get_plugin_tokens_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/get_table_upload_csv_url_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/import_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/import_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/list_enabled_workspaces_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/list_plugin_webhooks_plugin_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/plugin_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/plugin_data_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/plugin_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/plugin_live_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/plugin_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/plugin_workspace_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/plugin_workspace_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/prepare_ape_tables_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/presigned_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/s3_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/set_plugin_external_data_json_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/set_plugin_external_data_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/set_plugin_status_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/set_plugin_status_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/table_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/table_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/webhook_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/webhook_event_selector_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/models/webhook_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.672646 priceloop-api-0.97.0/priceloop_api/priceloop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/priceloop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.672646 priceloop-api-0.97.0/priceloop_api/priceloop/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/priceloop/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/priceloop/auth/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/priceloop/auth/priceloop_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.672646 priceloop-api-0.97.0/priceloop_api/priceloop/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/priceloop/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/priceloop/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/priceloop_api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:11:52.656645 priceloop-api-0.97.0/priceloop_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-23 21:11:52.000000 priceloop-api-0.97.0/priceloop_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-23 21:11:52.000000 priceloop-api-0.97.0/priceloop_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:11:52.000000 priceloop-api-0.97.0/priceloop_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-23 21:11:52.000000 priceloop-api-0.97.0/priceloop_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 21:11:52.000000 priceloop-api-0.97.0/priceloop_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 21:11:52.672646 priceloop-api-0.97.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-23 21:11:36.000000 priceloop-api-0.97.0/setup.py
```

### Comparing `priceloop-api-0.95.0/LICENSE` & `priceloop-api-0.97.0/LICENSE`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/PKG-INFO` & `priceloop-api-0.97.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: priceloop-api
-Version: 0.95.0
+Version: 0.97.0
 Summary: A client library for accessing Priceloop API
 Home-page: https://github.com/priceloop/priceloop-api-python
 Author: Priceloop
 Author-email: hello@priceloop.ai
 License: UNKNOWN
 Description: # priceloop-api-python
         A client library for accessing Priceloop API
```

### Comparing `priceloop-api-0.95.0/README.md` & `priceloop-api-0.97.0/README.md`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/column_api/add_data_column.py` & `priceloop-api-0.97.0/priceloop_api/api/column_api/add_data_column.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/column_api/add_formula_column.py` & `priceloop-api-0.97.0/priceloop_api/api/column_api/add_formula_column.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/column_api/delete_column.py` & `priceloop-api-0.97.0/priceloop_api/api/column_api/delete_column.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/column_api/get_column_attributes.py` & `priceloop-api-0.97.0/priceloop_api/api/column_api/get_column_attributes.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/column_api/update_column_attributes.py` & `priceloop-api-0.97.0/priceloop_api/api/column_api/update_column_attributes.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/column_api/update_column_is_gui_locked.py` & `priceloop-api-0.97.0/priceloop_api/api/column_api/update_column_is_gui_locked.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/column_api/update_column_position.py` & `priceloop-api-0.97.0/priceloop_api/api/column_api/update_column_position.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/column_api/update_column_visibility.py` & `priceloop-api-0.97.0/priceloop_api/api/column_api/update_column_visibility.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/external_function_api/create_external_function.py` & `priceloop-api-0.97.0/priceloop_api/api/external_function_api/create_external_function.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/external_function_api/delete_external_function.py` & `priceloop-api-0.97.0/priceloop_api/api/external_function_api/delete_external_function.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/external_function_api/get_external_functions.py` & `priceloop-api-0.97.0/priceloop_api/api/external_function_api/get_external_functions.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/external_function_api/update_external_function.py` & `priceloop-api-0.97.0/priceloop_api/api/external_function_api/update_external_function.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/import_api/create_csv_import_job.py` & `priceloop-api-0.97.0/priceloop_api/api/import_api/create_csv_import_job.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/import_api/get_table_upload_csv_url.py` & `priceloop-api-0.97.0/priceloop_api/api/import_api/get_table_upload_csv_url.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/other/hello.py` & `priceloop-api-0.97.0/priceloop_api/api/other/hello.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/other/hello_auth.py` & `priceloop-api-0.97.0/priceloop_api/api/other/hello_auth.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/plugin_api/create_plugin.py` & `priceloop-api-0.97.0/priceloop_api/api/plugin_api/create_plugin.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/plugin_api/get_plugin.py` & `priceloop-api-0.97.0/priceloop_api/api/plugin_api/get_plugin.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/plugin_api/get_plugin_live_status.py` & `priceloop-api-0.97.0/priceloop_api/api/plugin_api/get_plugin_live_status.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/plugin_api/get_plugin_tokens.py` & `priceloop-api-0.97.0/priceloop_api/api/plugin_api/get_plugin_tokens.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/plugin_api/list_enabled_workspaces.py` & `priceloop-api-0.97.0/priceloop_api/api/plugin_api/list_enabled_workspaces.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/plugin_api/prepare_ape_tables.py` & `priceloop-api-0.97.0/priceloop_api/api/plugin_api/prepare_ape_tables.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/plugin_api/set_plugin_external_data.py` & `priceloop-api-0.97.0/priceloop_api/api/plugin_api/set_plugin_external_data.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/plugin_api/set_plugin_status.py` & `priceloop-api-0.97.0/priceloop_api/api/plugin_api/set_plugin_status.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/plugin_webhooks/add_plugin_webhook.py` & `priceloop-api-0.97.0/priceloop_api/api/plugin_webhooks/add_plugin_webhook.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/plugin_webhooks/delete_plugin_webhook.py` & `priceloop-api-0.97.0/priceloop_api/api/plugin_webhooks/delete_plugin_webhook.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/plugin_webhooks/list_plugin_webhooks.py` & `priceloop-api-0.97.0/priceloop_api/api/plugin_webhooks/list_plugin_webhooks.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/table_api/create_table.py` & `priceloop-api-0.97.0/priceloop_api/api/table_api/create_table.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/table_api/delete_table.py` & `priceloop-api-0.97.0/priceloop_api/api/table_api/delete_table.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/table_api/get_table.py` & `priceloop-api-0.97.0/priceloop_api/api/table_api/get_table.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/table_api/get_table_data.py` & `priceloop-api-0.97.0/priceloop_api/api/table_api/get_table_data.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/table_api/truncate_table.py` & `priceloop-api-0.97.0/priceloop_api/api/table_api/truncate_table.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/workspace_api/create_workspace.py` & `priceloop-api-0.97.0/priceloop_api/api/workspace_api/create_workspace.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/workspace_api/get_workspace.py` & `priceloop-api-0.97.0/priceloop_api/api/workspace_api/get_workspace.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/api/workspace_api/list_workspaces.py` & `priceloop-api-0.97.0/priceloop_api/api/workspace_api/list_workspaces.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/client.py` & `priceloop-api-0.97.0/priceloop_api/client.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/__init__.py` & `priceloop-api-0.97.0/priceloop_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/amazon.py` & `priceloop-api-0.97.0/priceloop_api/models/amazon.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/ape_data.py` & `priceloop-api-0.97.0/priceloop_api/models/ape_data.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/ape_data_typeform.py` & `priceloop-api-0.97.0/priceloop_api/models/ape_data_typeform.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/api_column.py` & `priceloop-api-0.97.0/priceloop_api/models/api_column.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/api_column_attributes.py` & `priceloop-api-0.97.0/priceloop_api/models/api_column_attributes.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/api_column_attributes_update.py` & `priceloop-api-0.97.0/priceloop_api/models/api_column_attributes_update.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/api_external_function.py` & `priceloop-api-0.97.0/priceloop_api/models/api_external_function.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/api_table.py` & `priceloop-api-0.97.0/priceloop_api/models/api_table.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/api_table_data.py` & `priceloop-api-0.97.0/priceloop_api/models/api_table_data.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/api_workspace.py` & `priceloop-api-0.97.0/priceloop_api/models/api_workspace.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/column_attribute_schema.py` & `priceloop-api-0.97.0/priceloop_api/models/column_attribute_schema.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/column_schema.py` & `priceloop-api-0.97.0/priceloop_api/models/column_schema.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/csv_separator.py` & `priceloop-api-0.97.0/priceloop_api/models/csv_separator.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/import_job.py` & `priceloop-api-0.97.0/priceloop_api/models/import_job.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/import_job_response.py` & `priceloop-api-0.97.0/priceloop_api/models/import_job_response.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/plugin.py` & `priceloop-api-0.97.0/priceloop_api/models/plugin.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/plugin_1.py` & `priceloop-api-0.97.0/priceloop_api/models/plugin_1.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/plugin_data_type_0.py` & `priceloop-api-0.97.0/priceloop_api/models/plugin_data_type_0.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/plugin_external_data.py` & `priceloop-api-0.97.0/priceloop_api/models/plugin_external_data.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/plugin_live_status.py` & `priceloop-api-0.97.0/priceloop_api/models/plugin_live_status.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/plugin_tokens.py` & `priceloop-api-0.97.0/priceloop_api/models/plugin_tokens.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/plugin_workspace_list.py` & `priceloop-api-0.97.0/priceloop_api/models/plugin_workspace_list.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/plugin_workspace_state.py` & `priceloop-api-0.97.0/priceloop_api/models/plugin_workspace_state.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/presigned_url.py` & `priceloop-api-0.97.0/priceloop_api/models/presigned_url.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/s3_key.py` & `priceloop-api-0.97.0/priceloop_api/models/s3_key.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/set_plugin_external_data_json_body.py` & `priceloop-api-0.97.0/priceloop_api/models/set_plugin_external_data_json_body.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/table_row.py` & `priceloop-api-0.97.0/priceloop_api/models/table_row.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/table_schema.py` & `priceloop-api-0.97.0/priceloop_api/models/table_schema.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/webhook_config.py` & `priceloop-api-0.97.0/priceloop_api/models/webhook_config.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/webhook_event_selector_type_0.py` & `priceloop-api-0.97.0/priceloop_api/models/webhook_event_selector_type_0.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/models/webhook_info.py` & `priceloop-api-0.97.0/priceloop_api/models/webhook_info.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/priceloop/auth/auth.py` & `priceloop-api-0.97.0/priceloop_api/priceloop/auth/auth.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/priceloop/auth/priceloop_client.py` & `priceloop-api-0.97.0/priceloop_api/priceloop/auth/priceloop_client.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/priceloop/data/data.py` & `priceloop-api-0.97.0/priceloop_api/priceloop/data/data.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api/types.py` & `priceloop-api-0.97.0/priceloop_api/types.py`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/priceloop_api.egg-info/PKG-INFO` & `priceloop-api-0.97.0/priceloop_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: priceloop-api
-Version: 0.95.0
+Version: 0.97.0
 Summary: A client library for accessing Priceloop API
 Home-page: https://github.com/priceloop/priceloop-api-python
 Author: Priceloop
 Author-email: hello@priceloop.ai
 License: UNKNOWN
 Description: # priceloop-api-python
         A client library for accessing Priceloop API
```

### Comparing `priceloop-api-0.95.0/priceloop_api.egg-info/SOURCES.txt` & `priceloop-api-0.97.0/priceloop_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `priceloop-api-0.95.0/setup.py` & `priceloop-api-0.97.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "requests==2.25",
     "frozendict==2.3.4",
     "pandas==1.5.2",
 ]
 
 setup(
     name="priceloop-api",
-    version="0.95.0",
+    version="0.97.0",
     description="A client library for accessing Priceloop API",
     author="Priceloop",
     author_email="hello@priceloop.ai",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/priceloop/priceloop-api-python",
     packages=find_packages(),
```

