# Comparing `tmp/windmill_api-1.88.1.tar.gz` & `tmp/windmill_api-1.89.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windmill_api-1.88.1.tar", max compression
+gzip compressed data, was "windmill_api-1.89.0.tar", max compression
```

## Comparing `windmill_api-1.88.1.tar` & `windmill_api-1.89.0.tar`

### file list

```diff
@@ -1,1267 +1,1268 @@
--rw-r--r--   0        0        0    11348 2023-04-18 06:32:05.645729 windmill_api-1.88.1/LICENSE
--rw-r--r--   0        0        0     2952 2023-04-18 06:32:05.649729 windmill_api-1.88.1/README.md
--rw-r--r--   0        0        0      717 2023-04-18 06:32:05.649729 windmill_api-1.88.1/pyproject.toml
--rw-r--r--   0        0        0      100 2023-04-18 06:31:33.841384 windmill_api-1.88.1/windmill_api/__init__.py
--rw-r--r--   0        0        0       47 2023-04-18 06:31:34.325389 windmill_api-1.88.1/windmill_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.429390 windmill_api-1.88.1/windmill_api/api/app/__init__.py
--rw-r--r--   0        0        0     1999 2023-04-18 06:31:44.665500 windmill_api-1.88.1/windmill_api/api/app/create_app.py
--rw-r--r--   0        0        0     1769 2023-04-18 06:31:44.681500 windmill_api-1.88.1/windmill_api/api/app/delete_app.py
--rw-r--r--   0        0        0     2214 2023-04-18 06:31:44.701501 windmill_api-1.88.1/windmill_api/api/app/execute_component.py
--rw-r--r--   0        0        0     2782 2023-04-18 06:31:44.745501 windmill_api-1.88.1/windmill_api/api/app/exists_app.py
--rw-r--r--   0        0        0     3020 2023-04-18 06:31:44.741501 windmill_api-1.88.1/windmill_api/api/app/get_app_by_path.py
--rw-r--r--   0        0        0     3031 2023-04-18 06:31:44.781501 windmill_api-1.88.1/windmill_api/api/app/get_app_by_version.py
--rw-r--r--   0        0        0     2649 2023-04-18 06:31:44.785501 windmill_api-1.88.1/windmill_api/api/app/get_hub_app_by_id.py
--rw-r--r--   0        0        0     3168 2023-04-18 06:31:44.837502 windmill_api-1.88.1/windmill_api/api/app/get_public_app_by_secret.py
--rw-r--r--   0        0        0     1797 2023-04-18 06:31:44.813502 windmill_api-1.88.1/windmill_api/api/app/get_public_secret_of_app.py
--rw-r--r--   0        0        0     7289 2023-04-18 06:31:44.917503 windmill_api-1.88.1/windmill_api/api/app/list_apps.py
--rw-r--r--   0        0        0     2405 2023-04-18 06:31:44.869502 windmill_api-1.88.1/windmill_api/api/app/list_hub_apps.py
--rw-r--r--   0        0        0     2140 2023-04-18 06:31:44.897503 windmill_api-1.88.1/windmill_api/api/app/update_app.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.365389 windmill_api-1.88.1/windmill_api/api/audit/__init__.py
--rw-r--r--   0        0        0     3065 2023-04-18 06:31:44.941503 windmill_api-1.88.1/windmill_api/api/audit/get_audit_log.py
--rw-r--r--   0        0        0     8723 2023-04-18 06:31:45.021504 windmill_api-1.88.1/windmill_api/api/audit/list_audit_logs.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.481391 windmill_api-1.88.1/windmill_api/api/capture/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-18 06:31:44.969503 windmill_api-1.88.1/windmill_api/api/capture/create_capture.py
--rw-r--r--   0        0        0     1790 2023-04-18 06:31:44.997504 windmill_api-1.88.1/windmill_api/api/capture/get_capture.py
--rw-r--r--   0        0        0     1799 2023-04-18 06:31:45.021504 windmill_api-1.88.1/windmill_api/api/capture/update_capture.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.481391 windmill_api-1.88.1/windmill_api/api/favorite/__init__.py
--rw-r--r--   0        0        0     1964 2023-04-18 06:31:45.057504 windmill_api-1.88.1/windmill_api/api/favorite/star.py
--rw-r--r--   0        0        0     1984 2023-04-18 06:31:45.053504 windmill_api-1.88.1/windmill_api/api/favorite/unstar.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.421390 windmill_api-1.88.1/windmill_api/api/flow/__init__.py
--rw-r--r--   0        0        0     2220 2023-04-18 06:31:45.085505 windmill_api-1.88.1/windmill_api/api/flow/archive_flow_by_path.py
--rw-r--r--   0        0        0     2009 2023-04-18 06:31:45.085505 windmill_api-1.88.1/windmill_api/api/flow/create_flow.py
--rw-r--r--   0        0        0     1788 2023-04-18 06:31:45.109505 windmill_api-1.88.1/windmill_api/api/flow/delete_flow_by_path.py
--rw-r--r--   0        0        0     2755 2023-04-18 06:31:45.125505 windmill_api-1.88.1/windmill_api/api/flow/exists_flow_by_path.py
--rw-r--r--   0        0        0     3036 2023-04-18 06:31:45.149505 windmill_api-1.88.1/windmill_api/api/flow/get_flow_by_path.py
--rw-r--r--   0        0        0     4827 2023-04-18 06:31:45.205506 windmill_api-1.88.1/windmill_api/api/flow/get_flow_input_history_by_path.py
--rw-r--r--   0        0        0     2667 2023-04-18 06:31:45.213506 windmill_api-1.88.1/windmill_api/api/flow/get_hub_flow_by_id.py
--rw-r--r--   0        0        0     1668 2023-04-18 06:31:45.233506 windmill_api-1.88.1/windmill_api/api/flow/list_flow_paths.py
--rw-r--r--   0        0        0     7969 2023-04-18 06:31:45.305507 windmill_api-1.88.1/windmill_api/api/flow/list_flows.py
--rw-r--r--   0        0        0     2423 2023-04-18 06:31:45.269507 windmill_api-1.88.1/windmill_api/api/flow/list_hub_flows.py
--rw-r--r--   0        0        0     2150 2023-04-18 06:31:45.297507 windmill_api-1.88.1/windmill_api/api/flow/update_flow.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.473390 windmill_api-1.88.1/windmill_api/api/folder/__init__.py
--rw-r--r--   0        0        0     2214 2023-04-18 06:31:45.329507 windmill_api-1.88.1/windmill_api/api/folder/add_owner_to_folder.py
--rw-r--r--   0        0        0     2029 2023-04-18 06:31:45.333507 windmill_api-1.88.1/windmill_api/api/folder/create_folder.py
--rw-r--r--   0        0        0     1778 2023-04-18 06:31:45.357508 windmill_api-1.88.1/windmill_api/api/folder/delete_folder.py
--rw-r--r--   0        0        0     2960 2023-04-18 06:31:45.373508 windmill_api-1.88.1/windmill_api/api/folder/get_folder.py
--rw-r--r--   0        0        0     3055 2023-04-18 06:31:45.393508 windmill_api-1.88.1/windmill_api/api/folder/get_folder_usage.py
--rw-r--r--   0        0        0     3405 2023-04-18 06:31:45.421508 windmill_api-1.88.1/windmill_api/api/folder/list_folder_names.py
--rw-r--r--   0        0        0     4251 2023-04-18 06:31:45.449509 windmill_api-1.88.1/windmill_api/api/folder/list_folders.py
--rw-r--r--   0        0        0     2244 2023-04-18 06:31:45.453509 windmill_api-1.88.1/windmill_api/api/folder/remove_owner_to_folder.py
--rw-r--r--   0        0        0     2170 2023-04-18 06:31:45.501509 windmill_api-1.88.1/windmill_api/api/folder/update_folder.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.477391 windmill_api-1.88.1/windmill_api/api/granular_acl/__init__.py
--rw-r--r--   0        0        0     2480 2023-04-18 06:31:45.485509 windmill_api-1.88.1/windmill_api/api/granular_acl/add_granular_acls.py
--rw-r--r--   0        0        0     3526 2023-04-18 06:31:45.549510 windmill_api-1.88.1/windmill_api/api/granular_acl/get_granular_acls.py
--rw-r--r--   0        0        0     2545 2023-04-18 06:31:45.533510 windmill_api-1.88.1/windmill_api/api/granular_acl/remove_granular_acls.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.465390 windmill_api-1.88.1/windmill_api/api/group/__init__.py
--rw-r--r--   0        0        0     2194 2023-04-18 06:31:45.577510 windmill_api-1.88.1/windmill_api/api/group/add_user_to_group.py
--rw-r--r--   0        0        0     2019 2023-04-18 06:31:45.577510 windmill_api-1.88.1/windmill_api/api/group/create_group.py
--rw-r--r--   0        0        0     1775 2023-04-18 06:31:45.601510 windmill_api-1.88.1/windmill_api/api/group/delete_group.py
--rw-r--r--   0        0        0     2942 2023-04-18 06:31:45.617510 windmill_api-1.88.1/windmill_api/api/group/get_group.py
--rw-r--r--   0        0        0     3400 2023-04-18 06:31:45.645511 windmill_api-1.88.1/windmill_api/api/group/list_group_names.py
--rw-r--r--   0        0        0     4233 2023-04-18 06:31:45.673511 windmill_api-1.88.1/windmill_api/api/group/list_groups.py
--rw-r--r--   0        0        0     2224 2023-04-18 06:31:45.677511 windmill_api-1.88.1/windmill_api/api/group/remove_user_to_group.py
--rw-r--r--   0        0        0     2160 2023-04-18 06:31:45.705511 windmill_api-1.88.1/windmill_api/api/group/update_group.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.485391 windmill_api-1.88.1/windmill_api/api/input_/__init__.py
--rw-r--r--   0        0        0     3338 2023-04-18 06:31:45.717512 windmill_api-1.88.1/windmill_api/api/input_/create_input.py
--rw-r--r--   0        0        0     1811 2023-04-18 06:31:45.733512 windmill_api-1.88.1/windmill_api/api/input_/delete_input.py
--rw-r--r--   0        0        0     6187 2023-04-18 06:31:45.785512 windmill_api-1.88.1/windmill_api/api/input_/get_input_history.py
--rw-r--r--   0        0        0     6010 2023-04-18 06:31:45.809512 windmill_api-1.88.1/windmill_api/api/input_/list_inputs.py
--rw-r--r--   0        0        0     2025 2023-04-18 06:31:45.813513 windmill_api-1.88.1/windmill_api/api/input_/update_input.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.437390 windmill_api-1.88.1/windmill_api/api/job/__init__.py
--rw-r--r--   0        0        0     2181 2023-04-18 06:31:45.861513 windmill_api-1.88.1/windmill_api/api/job/cancel_queued_job.py
--rw-r--r--   0        0        0     2687 2023-04-18 06:31:45.849513 windmill_api-1.88.1/windmill_api/api/job/cancel_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-04-18 06:31:45.909514 windmill_api-1.88.1/windmill_api/api/job/cancel_suspended_job_post.py
--rw-r--r--   0        0        0     2535 2023-04-18 06:31:45.897513 windmill_api-1.88.1/windmill_api/api/job/create_job_signature.py
--rw-r--r--   0        0        0     3217 2023-04-18 06:31:45.937514 windmill_api-1.88.1/windmill_api/api/job/delete_completed_job.py
--rw-r--r--   0        0        0     2235 2023-04-18 06:31:45.941514 windmill_api-1.88.1/windmill_api/api/job/force_cancel_queued_job.py
--rw-r--r--   0        0        0     3034 2023-04-18 06:31:45.977514 windmill_api-1.88.1/windmill_api/api/job/get_completed_job.py
--rw-r--r--   0        0        0     1784 2023-04-18 06:31:45.969514 windmill_api-1.88.1/windmill_api/api/job/get_completed_job_result.py
--rw-r--r--   0        0        0     2868 2023-04-18 06:31:46.009515 windmill_api-1.88.1/windmill_api/api/job/get_job.py
--rw-r--r--   0        0        0     4305 2023-04-18 06:31:46.033515 windmill_api-1.88.1/windmill_api/api/job/get_job_updates.py
--rw-r--r--   0        0        0     4306 2023-04-18 06:31:46.061515 windmill_api-1.88.1/windmill_api/api/job/get_resume_urls.py
--rw-r--r--   0        0        0     4601 2023-04-18 06:31:46.089516 windmill_api-1.88.1/windmill_api/api/job/get_suspended_job_flow.py
--rw-r--r--   0        0        0    12602 2023-04-18 06:31:46.201517 windmill_api-1.88.1/windmill_api/api/job/list_completed_jobs.py
--rw-r--r--   0        0        0    11829 2023-04-18 06:31:46.245517 windmill_api-1.88.1/windmill_api/api/job/list_jobs.py
--rw-r--r--   0        0        0    12367 2023-04-18 06:31:46.365519 windmill_api-1.88.1/windmill_api/api/job/list_queue.py
--rw-r--r--   0        0        0     2067 2023-04-18 06:31:46.277518 windmill_api-1.88.1/windmill_api/api/job/result_by_id.py
--rw-r--r--   0        0        0     2313 2023-04-18 06:31:46.309518 windmill_api-1.88.1/windmill_api/api/job/resume_suspended_flow_as_owner.py
--rw-r--r--   0        0        0     2994 2023-04-18 06:31:46.349518 windmill_api-1.88.1/windmill_api/api/job/resume_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-04-18 06:31:46.393519 windmill_api-1.88.1/windmill_api/api/job/resume_suspended_job_post.py
--rw-r--r--   0        0        0     4566 2023-04-18 06:31:46.417519 windmill_api-1.88.1/windmill_api/api/job/run_flow_by_path.py
--rw-r--r--   0        0        0     3037 2023-04-18 06:31:46.433519 windmill_api-1.88.1/windmill_api/api/job/run_flow_preview.py
--rw-r--r--   0        0        0     4594 2023-04-18 06:31:46.473520 windmill_api-1.88.1/windmill_api/api/job/run_script_by_hash.py
--rw-r--r--   0        0        0     4200 2023-04-18 06:31:46.489520 windmill_api-1.88.1/windmill_api/api/job/run_script_by_path.py
--rw-r--r--   0        0        0     3050 2023-04-18 06:31:46.513520 windmill_api-1.88.1/windmill_api/api/job/run_script_preview.py
--rw-r--r--   0        0        0     3215 2023-04-18 06:31:46.533520 windmill_api-1.88.1/windmill_api/api/job/run_wait_result_flow_by_path.py
--rw-r--r--   0        0        0     3521 2023-04-18 06:31:46.557521 windmill_api-1.88.1/windmill_api/api/job/run_wait_result_script_by_path.py
--rw-r--r--   0        0        0     3356 2023-04-18 06:31:46.601521 windmill_api-1.88.1/windmill_api/api/job/run_wait_result_script_by_path_get.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.393390 windmill_api-1.88.1/windmill_api/api/oauth/__init__.py
--rw-r--r--   0        0        0     3506 2023-04-18 06:31:46.625521 windmill_api-1.88.1/windmill_api/api/oauth/connect_callback.py
--rw-r--r--   0        0        0     2118 2023-04-18 06:31:46.629521 windmill_api-1.88.1/windmill_api/api/oauth/connect_slack_callback.py
--rw-r--r--   0        0        0     2056 2023-04-18 06:31:46.653522 windmill_api-1.88.1/windmill_api/api/oauth/create_account.py
--rw-r--r--   0        0        0     1764 2023-04-18 06:31:46.661522 windmill_api-1.88.1/windmill_api/api/oauth/disconnect_account.py
--rw-r--r--   0        0        0     1649 2023-04-18 06:31:46.677522 windmill_api-1.88.1/windmill_api/api/oauth/disconnect_slack.py
--rw-r--r--   0        0        0     1426 2023-04-18 06:31:46.685522 windmill_api-1.88.1/windmill_api/api/oauth/list_o_auth_connects.py
--rw-r--r--   0        0        0     2162 2023-04-18 06:31:46.713522 windmill_api-1.88.1/windmill_api/api/oauth/list_o_auth_logins.py
--rw-r--r--   0        0        0     2151 2023-04-18 06:31:46.717522 windmill_api-1.88.1/windmill_api/api/oauth/refresh_token.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.401390 windmill_api-1.88.1/windmill_api/api/resource/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-18 06:31:46.741523 windmill_api-1.88.1/windmill_api/api/resource/create_resource.py
--rw-r--r--   0        0        0     2093 2023-04-18 06:31:46.745523 windmill_api-1.88.1/windmill_api/api/resource/create_resource_type.py
--rw-r--r--   0        0        0     1784 2023-04-18 06:31:46.765523 windmill_api-1.88.1/windmill_api/api/resource/delete_resource.py
--rw-r--r--   0        0        0     1799 2023-04-18 06:31:46.773523 windmill_api-1.88.1/windmill_api/api/resource/delete_resource_type.py
--rw-r--r--   0        0        0     2763 2023-04-18 06:31:46.805523 windmill_api-1.88.1/windmill_api/api/resource/exists_resource.py
--rw-r--r--   0        0        0     2788 2023-04-18 06:31:46.813523 windmill_api-1.88.1/windmill_api/api/resource/exists_resource_type.py
--rw-r--r--   0        0        0     2996 2023-04-18 06:31:46.841524 windmill_api-1.88.1/windmill_api/api/resource/get_resource.py
--rw-r--r--   0        0        0     3074 2023-04-18 06:31:46.853524 windmill_api-1.88.1/windmill_api/api/resource/get_resource_type.py
--rw-r--r--   0        0        0     1790 2023-04-18 06:31:46.865524 windmill_api-1.88.1/windmill_api/api/resource/get_resource_value.py
--rw-r--r--   0        0        0     5732 2023-04-18 06:31:46.941525 windmill_api-1.88.1/windmill_api/api/resource/list_resource.py
--rw-r--r--   0        0        0     3149 2023-04-18 06:31:46.921525 windmill_api-1.88.1/windmill_api/api/resource/list_resource_type.py
--rw-r--r--   0        0        0     2600 2023-04-18 06:31:46.957525 windmill_api-1.88.1/windmill_api/api/resource/list_resource_type_names.py
--rw-r--r--   0        0        0     2190 2023-04-18 06:31:46.973525 windmill_api-1.88.1/windmill_api/api/resource/update_resource.py
--rw-r--r--   0        0        0     2234 2023-04-18 06:31:46.989525 windmill_api-1.88.1/windmill_api/api/resource/update_resource_type.py
--rw-r--r--   0        0        0     2244 2023-04-18 06:31:47.013526 windmill_api-1.88.1/windmill_api/api/resource/update_resource_value.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.461390 windmill_api-1.88.1/windmill_api/api/schedule/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-18 06:31:47.021526 windmill_api-1.88.1/windmill_api/api/schedule/create_schedule.py
--rw-r--r--   0        0        0     1784 2023-04-18 06:31:47.041526 windmill_api-1.88.1/windmill_api/api/schedule/delete_schedule.py
--rw-r--r--   0        0        0     2763 2023-04-18 06:31:47.061526 windmill_api-1.88.1/windmill_api/api/schedule/exists_schedule.py
--rw-r--r--   0        0        0     2996 2023-04-18 06:31:47.081526 windmill_api-1.88.1/windmill_api/api/schedule/get_schedule.py
--rw-r--r--   0        0        0     4287 2023-04-18 06:31:47.117527 windmill_api-1.88.1/windmill_api/api/schedule/list_schedules.py
--rw-r--r--   0        0        0     3217 2023-04-18 06:31:47.121527 windmill_api-1.88.1/windmill_api/api/schedule/preview_schedule.py
--rw-r--r--   0        0        0     2233 2023-04-18 06:31:47.149527 windmill_api-1.88.1/windmill_api/api/schedule/set_schedule_enabled.py
--rw-r--r--   0        0        0     2190 2023-04-18 06:31:47.149527 windmill_api-1.88.1/windmill_api/api/schedule/update_schedule.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.409390 windmill_api-1.88.1/windmill_api/api/script/__init__.py
--rw-r--r--   0        0        0     3165 2023-04-18 06:31:47.189527 windmill_api-1.88.1/windmill_api/api/script/archive_script_by_hash.py
--rw-r--r--   0        0        0     1797 2023-04-18 06:31:47.177527 windmill_api-1.88.1/windmill_api/api/script/archive_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-04-18 06:31:47.213528 windmill_api-1.88.1/windmill_api/api/script/bash_to_jsonschema.py
--rw-r--r--   0        0        0     2029 2023-04-18 06:31:47.213528 windmill_api-1.88.1/windmill_api/api/script/create_script.py
--rw-r--r--   0        0        0     3327 2023-04-18 06:31:47.273528 windmill_api-1.88.1/windmill_api/api/script/delete_script_by_hash.py
--rw-r--r--   0        0        0     2873 2023-04-18 06:31:47.253528 windmill_api-1.88.1/windmill_api/api/script/delete_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-04-18 06:31:47.309529 windmill_api-1.88.1/windmill_api/api/script/deno_to_jsonschema.py
--rw-r--r--   0        0        0     2767 2023-04-18 06:31:47.309529 windmill_api-1.88.1/windmill_api/api/script/exists_script_by_path.py
--rw-r--r--   0        0        0     2802 2023-04-18 06:31:47.345529 windmill_api-1.88.1/windmill_api/api/script/get_hub_script_by_path.py
--rw-r--r--   0        0        0     1607 2023-04-18 06:31:47.333529 windmill_api-1.88.1/windmill_api/api/script/get_hub_script_content_by_path.py
--rw-r--r--   0        0        0     3092 2023-04-18 06:31:47.377529 windmill_api-1.88.1/windmill_api/api/script/get_script_by_hash.py
--rw-r--r--   0        0        0     3074 2023-04-18 06:31:47.381530 windmill_api-1.88.1/windmill_api/api/script/get_script_by_path.py
--rw-r--r--   0        0        0     3276 2023-04-18 06:31:47.417530 windmill_api-1.88.1/windmill_api/api/script/get_script_deployment_status.py
--rw-r--r--   0        0        0     2967 2023-04-18 06:31:47.421530 windmill_api-1.88.1/windmill_api/api/script/go_to_jsonschema.py
--rw-r--r--   0        0        0     2459 2023-04-18 06:31:47.453530 windmill_api-1.88.1/windmill_api/api/script/list_hub_scripts.py
--rw-r--r--   0        0        0     1676 2023-04-18 06:31:47.441530 windmill_api-1.88.1/windmill_api/api/script/list_script_paths.py
--rw-r--r--   0        0        0    11165 2023-04-18 06:31:47.565532 windmill_api-1.88.1/windmill_api/api/script/list_scripts.py
--rw-r--r--   0        0        0     3039 2023-04-18 06:31:47.493531 windmill_api-1.88.1/windmill_api/api/script/python_to_jsonschema.py
--rw-r--r--   0        0        0     1784 2023-04-18 06:31:47.521531 windmill_api-1.88.1/windmill_api/api/script/raw_script_by_hash.py
--rw-r--r--   0        0        0     1784 2023-04-18 06:31:47.549531 windmill_api-1.88.1/windmill_api/api/script/raw_script_by_path.py
--rw-r--r--   0        0        0     2119 2023-04-18 06:31:47.585532 windmill_api-1.88.1/windmill_api/api/script/raw_script_by_path_tokened.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.337389 windmill_api-1.88.1/windmill_api/api/settings/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-18 06:31:47.613532 windmill_api-1.88.1/windmill_api/api/settings/backend_version.py
--rw-r--r--   0        0        0     1423 2023-04-18 06:31:47.609532 windmill_api-1.88.1/windmill_api/api/settings/get_open_api_yaml.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.365389 windmill_api-1.88.1/windmill_api/api/user/__init__.py
--rw-r--r--   0        0        0     1857 2023-04-18 06:31:47.661532 windmill_api-1.88.1/windmill_api/api/user/accept_invite.py
--rw-r--r--   0        0        0     1822 2023-04-18 06:31:47.641532 windmill_api-1.88.1/windmill_api/api/user/create_token.py
--rw-r--r--   0        0        0     1991 2023-04-18 06:31:47.665533 windmill_api-1.88.1/windmill_api/api/user/create_token_impersonate.py
--rw-r--r--   0        0        0     2058 2023-04-18 06:31:47.693533 windmill_api-1.88.1/windmill_api/api/user/create_user.py
--rw-r--r--   0        0        0     1863 2023-04-18 06:31:47.693533 windmill_api-1.88.1/windmill_api/api/user/create_user_globally.py
--rw-r--r--   0        0        0     1867 2023-04-18 06:31:47.725533 windmill_api-1.88.1/windmill_api/api/user/decline_invite.py
--rw-r--r--   0        0        0     1674 2023-04-18 06:31:47.721533 windmill_api-1.88.1/windmill_api/api/user/delete_token.py
--rw-r--r--   0        0        0     1872 2023-04-18 06:31:47.745534 windmill_api-1.88.1/windmill_api/api/user/delete_user.py
--rw-r--r--   0        0        0     1454 2023-04-18 06:31:47.749534 windmill_api-1.88.1/windmill_api/api/user/get_current_email.py
--rw-r--r--   0        0        0     1474 2023-04-18 06:31:47.769534 windmill_api-1.88.1/windmill_api/api/user/get_usage.py
--rw-r--r--   0        0        0     1639 2023-04-18 06:31:47.777534 windmill_api-1.88.1/windmill_api/api/user/global_user_delete.py
--rw-r--r--   0        0        0     2060 2023-04-18 06:31:47.797534 windmill_api-1.88.1/windmill_api/api/user/global_user_update.py
--rw-r--r--   0        0        0     2468 2023-04-18 06:31:47.813534 windmill_api-1.88.1/windmill_api/api/user/global_whoami.py
--rw-r--r--   0        0        0     2745 2023-04-18 06:31:47.833535 windmill_api-1.88.1/windmill_api/api/user/is_owner_of_path.py
--rw-r--r--   0        0        0     1646 2023-04-18 06:31:47.837535 windmill_api-1.88.1/windmill_api/api/user/leave_workspace.py
--rw-r--r--   0        0        0     2633 2023-04-18 06:31:47.869535 windmill_api-1.88.1/windmill_api/api/user/list_tokens.py
--rw-r--r--   0        0        0     2552 2023-04-18 06:31:47.877535 windmill_api-1.88.1/windmill_api/api/user/list_usernames.py
--rw-r--r--   0        0        0     3012 2023-04-18 06:31:47.925536 windmill_api-1.88.1/windmill_api/api/user/list_users.py
--rw-r--r--   0        0        0     4222 2023-04-18 06:31:47.933535 windmill_api-1.88.1/windmill_api/api/user/list_users_as_super_admin.py
--rw-r--r--   0        0        0     2829 2023-04-18 06:31:47.961536 windmill_api-1.88.1/windmill_api/api/user/list_workspace_invites.py
--rw-r--r--   0        0        0     1784 2023-04-18 06:31:47.961536 windmill_api-1.88.1/windmill_api/api/user/login.py
--rw-r--r--   0        0        0     2116 2023-04-18 06:31:47.985536 windmill_api-1.88.1/windmill_api/api/user/login_with_oauth.py
--rw-r--r--   0        0        0     1393 2023-04-18 06:31:48.005536 windmill_api-1.88.1/windmill_api/api/user/logout.py
--rw-r--r--   0        0        0     1820 2023-04-18 06:31:48.013536 windmill_api-1.88.1/windmill_api/api/user/set_password.py
--rw-r--r--   0        0        0     2250 2023-04-18 06:31:48.041537 windmill_api-1.88.1/windmill_api/api/user/update_user.py
--rw-r--r--   0        0        0     2652 2023-04-18 06:31:48.049537 windmill_api-1.88.1/windmill_api/api/user/whoami.py
--rw-r--r--   0        0        0     2967 2023-04-18 06:31:48.081537 windmill_api-1.88.1/windmill_api/api/user/whois.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.389390 windmill_api-1.88.1/windmill_api/api/variable/__init__.py
--rw-r--r--   0        0        0     2634 2023-04-18 06:31:48.085537 windmill_api-1.88.1/windmill_api/api/variable/create_variable.py
--rw-r--r--   0        0        0     1784 2023-04-18 06:31:48.109537 windmill_api-1.88.1/windmill_api/api/variable/delete_variable.py
--rw-r--r--   0        0        0     2795 2023-04-18 06:31:48.137538 windmill_api-1.88.1/windmill_api/api/variable/exists_variable.py
--rw-r--r--   0        0        0     3840 2023-04-18 06:31:48.161538 windmill_api-1.88.1/windmill_api/api/variable/get_variable.py
--rw-r--r--   0        0        0     3270 2023-04-18 06:31:48.181538 windmill_api-1.88.1/windmill_api/api/variable/list_contextual_variables.py
--rw-r--r--   0        0        0     3071 2023-04-18 06:31:48.197538 windmill_api-1.88.1/windmill_api/api/variable/list_variable.py
--rw-r--r--   0        0        0     2775 2023-04-18 06:31:48.221539 windmill_api-1.88.1/windmill_api/api/variable/update_variable.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.477391 windmill_api-1.88.1/windmill_api/api/worker/__init__.py
--rw-r--r--   0        0        0     3896 2023-04-18 06:31:48.253539 windmill_api-1.88.1/windmill_api/api/worker/list_workers.py
--rw-r--r--   0        0        0        0 2023-04-18 06:31:34.381389 windmill_api-1.88.1/windmill_api/api/workspace/__init__.py
--rw-r--r--   0        0        0     2015 2023-04-18 06:31:48.249539 windmill_api-1.88.1/windmill_api/api/workspace/add_user.py
--rw-r--r--   0        0        0     1647 2023-04-18 06:31:48.293539 windmill_api-1.88.1/windmill_api/api/workspace/archive_workspace.py
--rw-r--r--   0        0        0     1856 2023-04-18 06:31:48.277539 windmill_api-1.88.1/windmill_api/api/workspace/create_workspace.py
--rw-r--r--   0        0        0     2049 2023-04-18 06:31:48.305539 windmill_api-1.88.1/windmill_api/api/workspace/delete_invite.py
--rw-r--r--   0        0        0     1688 2023-04-18 06:31:48.321540 windmill_api-1.88.1/windmill_api/api/workspace/delete_workspace.py
--rw-r--r--   0        0        0     2063 2023-04-18 06:31:48.353540 windmill_api-1.88.1/windmill_api/api/workspace/edit_auto_invite.py
--rw-r--r--   0        0        0     2083 2023-04-18 06:31:48.349540 windmill_api-1.88.1/windmill_api/api/workspace/edit_slack_command.py
--rw-r--r--   0        0        0     2029 2023-04-18 06:31:48.377540 windmill_api-1.88.1/windmill_api/api/workspace/edit_webhook.py
--rw-r--r--   0        0        0     1856 2023-04-18 06:31:48.381540 windmill_api-1.88.1/windmill_api/api/workspace/exists_username.py
--rw-r--r--   0        0        0     1856 2023-04-18 06:31:48.405541 windmill_api-1.88.1/windmill_api/api/workspace/exists_workspace.py
--rw-r--r--   0        0        0     2809 2023-04-18 06:31:48.417541 windmill_api-1.88.1/windmill_api/api/workspace/get_premium_info.py
--rw-r--r--   0        0        0     2753 2023-04-18 06:31:48.445541 windmill_api-1.88.1/windmill_api/api/workspace/get_settings.py
--rw-r--r--   0        0        0     2045 2023-04-18 06:31:48.445541 windmill_api-1.88.1/windmill_api/api/workspace/invite_user.py
--rw-r--r--   0        0        0     2176 2023-04-18 06:31:48.477542 windmill_api-1.88.1/windmill_api/api/workspace/is_domain_allowed.py
--rw-r--r--   0        0        0     3255 2023-04-18 06:31:48.485541 windmill_api-1.88.1/windmill_api/api/workspace/list_pending_invites.py
--rw-r--r--   0        0        0     2583 2023-04-18 06:31:48.509542 windmill_api-1.88.1/windmill_api/api/workspace/list_user_workspaces.py
--rw-r--r--   0        0        0     2775 2023-04-18 06:31:48.521542 windmill_api-1.88.1/windmill_api/api/workspace/list_workspaces.py
--rw-r--r--   0        0        0     4311 2023-04-18 06:31:48.565542 windmill_api-1.88.1/windmill_api/api/workspace/list_workspaces_as_super_admin.py
--rw-r--r--   0        0        0     1651 2023-04-18 06:31:48.545542 windmill_api-1.88.1/windmill_api/api/workspace/unarchive_workspace.py
--rw-r--r--   0        0        0     1821 2023-04-18 06:31:48.573542 windmill_api-1.88.1/windmill_api/client.py
--rw-r--r--   0        0        0        1 2023-04-18 06:32:05.641729 windmill_api-1.88.1/windmill_api/models/__init__.py
--rw-r--r--   0        0        0     1667 2023-04-18 06:31:48.597543 windmill_api-1.88.1/windmill_api/models/accept_invite_json_body.py
--rw-r--r--   0        0        0     1710 2023-04-18 06:31:48.629543 windmill_api-1.88.1/windmill_api/models/add_granular_acls_json_body.py
--rw-r--r--   0        0        0      301 2023-04-18 06:31:43.781491 windmill_api-1.88.1/windmill_api/models/add_granular_acls_kind.py
--rw-r--r--   0        0        0     1529 2023-04-18 06:31:48.657543 windmill_api-1.88.1/windmill_api/models/add_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1940 2023-04-18 06:31:48.701544 windmill_api-1.88.1/windmill_api/models/add_user_json_body.py
--rw-r--r--   0        0        0     1552 2023-04-18 06:31:48.725544 windmill_api-1.88.1/windmill_api/models/add_user_to_group_json_body.py
--rw-r--r--   0        0        0     3940 2023-04-18 06:31:48.753544 windmill_api-1.88.1/windmill_api/models/app_with_last_version.py
--rw-r--r--   0        0        0      214 2023-04-18 06:31:43.701490 windmill_api-1.88.1/windmill_api/models/app_with_last_version_execution_mode.py
--rw-r--r--   0        0        0     1248 2023-04-18 06:31:48.745544 windmill_api-1.88.1/windmill_api/models/app_with_last_version_extra_perms.py
--rw-r--r--   0        0        0     3716 2023-04-18 06:31:48.797545 windmill_api-1.88.1/windmill_api/models/app_with_last_version_policy.py
--rw-r--r--   0        0        0      220 2023-04-18 06:31:43.153484 windmill_api-1.88.1/windmill_api/models/app_with_last_version_policy_execution_mode.py
--rw-r--r--   0        0        0     1946 2023-04-18 06:31:48.777545 windmill_api-1.88.1/windmill_api/models/app_with_last_version_policy_triggerables.py
--rw-r--r--   0        0        0     1381 2023-04-18 06:31:48.797545 windmill_api-1.88.1/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     1569 2023-04-18 06:31:48.821545 windmill_api-1.88.1/windmill_api/models/archive_flow_by_path_json_body.py
--rw-r--r--   0        0        0     6879 2023-04-18 06:31:48.881546 windmill_api-1.88.1/windmill_api/models/archive_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1314 2023-04-18 06:31:48.837545 windmill_api-1.88.1/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      259 2023-04-18 06:31:43.353486 windmill_api-1.88.1/windmill_api/models/archive_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      217 2023-04-18 06:31:43.821491 windmill_api-1.88.1/windmill_api/models/archive_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1288 2023-04-18 06:31:48.861546 windmill_api-1.88.1/windmill_api/models/archive_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     3452 2023-04-18 06:31:48.909546 windmill_api-1.88.1/windmill_api/models/audit_log.py
--rw-r--r--   0        0        0      217 2023-04-18 06:31:43.277485 windmill_api-1.88.1/windmill_api/models/audit_log_action_kind.py
--rw-r--r--   0        0        0      620 2023-04-18 06:31:43.181484 windmill_api-1.88.1/windmill_api/models/audit_log_operation.py
--rw-r--r--   0        0        0     1186 2023-04-18 06:31:48.905546 windmill_api-1.88.1/windmill_api/models/audit_log_parameters.py
--rw-r--r--   0        0        0     2933 2023-04-18 06:31:48.945546 windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-04-18 06:31:48.993547 windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-04-18 06:31:43.245485 windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-04-18 06:31:48.973547 windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-04-18 06:31:49.001547 windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-04-18 06:31:49.017547 windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-04-18 06:31:49.041548 windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-04-18 06:31:43.041483 windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-04-18 06:31:49.041548 windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-04-18 06:31:49.101548 windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-04-18 06:31:43.737490 windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-04-18 06:31:49.073548 windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-04-18 06:31:43.009482 windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2377 2023-04-18 06:31:49.113548 windmill_api-1.88.1/windmill_api/models/branch_all.py
--rw-r--r--   0        0        0     2543 2023-04-18 06:31:49.133549 windmill_api-1.88.1/windmill_api/models/branch_all_branches_item.py
--rw-r--r--   0        0        0     6620 2023-04-18 06:31:49.205549 windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-04-18 06:31:49.173549 windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-04-18 06:31:49.201549 windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-18 06:31:49.233550 windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-18 06:31:49.237550 windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-18 06:31:43.365486 windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-18 06:31:49.261550 windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-18 06:31:43.469487 windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-18 06:31:49.269550 windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-18 06:31:49.289550 windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      146 2023-04-18 06:31:44.041493 windmill_api-1.88.1/windmill_api/models/branch_all_type.py
--rw-r--r--   0        0        0     2670 2023-04-18 06:31:49.313551 windmill_api-1.88.1/windmill_api/models/branch_one.py
--rw-r--r--   0        0        0     2372 2023-04-18 06:31:49.325551 windmill_api-1.88.1/windmill_api/models/branch_one_branches_item.py
--rw-r--r--   0        0        0     6620 2023-04-18 06:31:49.417552 windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-04-18 06:31:49.365551 windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-04-18 06:31:49.393551 windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-18 06:31:49.429552 windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-18 06:31:49.445552 windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-18 06:31:43.277485 windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-18 06:31:49.481552 windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-18 06:31:43.913492 windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-18 06:31:49.473552 windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-18 06:31:49.505553 windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6125 2023-04-18 06:31:49.561553 windmill_api-1.88.1/windmill_api/models/branch_one_default_item.py
--rw-r--r--   0        0        0     2906 2023-04-18 06:31:49.541553 windmill_api-1.88.1/windmill_api/models/branch_one_default_item_retry.py
--rw-r--r--   0        0        0     1863 2023-04-18 06:31:49.573553 windmill_api-1.88.1/windmill_api/models/branch_one_default_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-04-18 06:31:49.589553 windmill_api-1.88.1/windmill_api/models/branch_one_default_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-04-18 06:31:49.605554 windmill_api-1.88.1/windmill_api/models/branch_one_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-04-18 06:31:43.625489 windmill_api-1.88.1/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-04-18 06:31:49.617554 windmill_api-1.88.1/windmill_api/models/branch_one_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-04-18 06:31:43.141484 windmill_api-1.88.1/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-04-18 06:31:49.637554 windmill_api-1.88.1/windmill_api/models/branch_one_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-04-18 06:31:49.645554 windmill_api-1.88.1/windmill_api/models/branch_one_default_item_suspend.py
--rw-r--r--   0        0        0      146 2023-04-18 06:31:43.553488 windmill_api-1.88.1/windmill_api/models/branch_one_type.py
--rw-r--r--   0        0        0     1532 2023-04-18 06:31:49.665554 windmill_api-1.88.1/windmill_api/models/cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     1255 2023-04-18 06:31:49.665554 windmill_api-1.88.1/windmill_api/models/cancel_suspended_job_post_json_body.py
--rw-r--r--   0        0        0    10376 2023-04-18 06:31:49.837556 windmill_api-1.88.1/windmill_api/models/completed_job.py
--rw-r--r--   0        0        0     1176 2023-04-18 06:31:49.685555 windmill_api-1.88.1/windmill_api/models/completed_job_args.py
--rw-r--r--   0        0        0     3265 2023-04-18 06:31:49.725555 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status.py
--rw-r--r--   0        0        0     6800 2023-04-18 06:31:49.833556 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1789 2023-04-18 06:31:49.861556 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2136 2023-04-18 06:31:49.869557 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      202 2023-04-18 06:31:43.753490 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1694 2023-04-18 06:31:49.889557 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2230 2023-04-18 06:31:49.901557 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      360 2023-04-18 06:31:43.345486 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6402 2023-04-18 06:31:49.969558 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1779 2023-04-18 06:31:49.925557 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2116 2023-04-18 06:31:49.953557 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      200 2023-04-18 06:31:43.801491 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1684 2023-04-18 06:31:49.981558 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2220 2023-04-18 06:31:50.001558 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      358 2023-04-18 06:31:43.357486 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2040 2023-04-18 06:31:50.013558 windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_retry.py
--rw-r--r--   0        0        0      310 2023-04-18 06:31:43.301485 windmill_api-1.88.1/windmill_api/models/completed_job_job_kind.py
--rw-r--r--   0        0        0      199 2023-04-18 06:31:43.393486 windmill_api-1.88.1/windmill_api/models/completed_job_language.py
--rw-r--r--   0        0        0     3127 2023-04-18 06:31:50.049558 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow.py
--rw-r--r--   0        0        0     6620 2023-04-18 06:31:50.125559 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3129 2023-04-18 06:31:50.089559 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1929 2023-04-18 06:31:50.117559 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-18 06:31:50.149560 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-18 06:31:50.153560 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-18 06:31:43.549488 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-18 06:31:50.201560 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-18 06:31:44.041493 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-18 06:31:50.185560 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-18 06:31:50.225560 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6544 2023-04-18 06:31:50.281561 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3095 2023-04-18 06:31:50.265561 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1919 2023-04-18 06:31:50.289561 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2223 2023-04-18 06:31:50.313561 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2050 2023-04-18 06:31:50.317561 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      179 2023-04-18 06:31:44.017493 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1917 2023-04-18 06:31:50.345562 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      179 2023-04-18 06:31:43.177484 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1912 2023-04-18 06:31:50.345562 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1963 2023-04-18 06:31:50.377562 windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1572 2023-04-18 06:31:50.377562 windmill_api-1.88.1/windmill_api/models/connect_callback_json_body.py
--rw-r--r--   0        0        0     2533 2023-04-18 06:31:50.417563 windmill_api-1.88.1/windmill_api/models/connect_callback_response_200.py
--rw-r--r--   0        0        0     1600 2023-04-18 06:31:50.401562 windmill_api-1.88.1/windmill_api/models/connect_slack_callback_json_body.py
--rw-r--r--   0        0        0     1753 2023-04-18 06:31:50.429563 windmill_api-1.88.1/windmill_api/models/contextual_variable.py
--rw-r--r--   0        0        0     2147 2023-04-18 06:31:50.449563 windmill_api-1.88.1/windmill_api/models/create_account_json_body.py
--rw-r--r--   0        0        0     2035 2023-04-18 06:31:50.461563 windmill_api-1.88.1/windmill_api/models/create_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-04-18 06:31:50.525564 windmill_api-1.88.1/windmill_api/models/create_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-04-18 06:31:43.445487 windmill_api-1.88.1/windmill_api/models/create_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-04-18 06:31:50.485563 windmill_api-1.88.1/windmill_api/models/create_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-04-18 06:31:50.505564 windmill_api-1.88.1/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-04-18 06:31:50.561564 windmill_api-1.88.1/windmill_api/models/create_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-04-18 06:31:50.545564 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-04-18 06:31:50.589564 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-04-18 06:31:50.641565 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-04-18 06:31:50.629565 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-04-18 06:31:50.657565 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-04-18 06:31:50.673565 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-04-18 06:31:50.689566 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-04-18 06:31:43.481487 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-04-18 06:31:50.701566 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-04-18 06:31:44.009493 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-04-18 06:31:50.721566 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-04-18 06:31:50.729566 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-04-18 06:31:50.805567 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-04-18 06:31:50.765566 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-04-18 06:31:50.793567 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-04-18 06:31:50.825567 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-04-18 06:31:50.833567 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-04-18 06:31:43.569488 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-04-18 06:31:50.853567 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-04-18 06:31:43.681490 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-04-18 06:31:50.897568 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-04-18 06:31:50.881568 windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2126 2023-04-18 06:31:50.937568 windmill_api-1.88.1/windmill_api/models/create_folder_json_body.py
--rw-r--r--   0        0        0     1697 2023-04-18 06:31:50.925568 windmill_api-1.88.1/windmill_api/models/create_group_json_body.py
--rw-r--r--   0        0        0     1613 2023-04-18 06:31:50.953568 windmill_api-1.88.1/windmill_api/models/create_input.py
--rw-r--r--   0        0        0     1171 2023-04-18 06:31:50.957569 windmill_api-1.88.1/windmill_api/models/create_input_args.py
--rw-r--r--   0        0        0     1701 2023-04-18 06:31:50.985569 windmill_api-1.88.1/windmill_api/models/create_input_json_body.py
--rw-r--r--   0        0        0     1217 2023-04-18 06:31:50.977569 windmill_api-1.88.1/windmill_api/models/create_input_json_body_args.py
--rw-r--r--   0        0        0      214 2023-04-18 06:31:43.481487 windmill_api-1.88.1/windmill_api/models/create_input_runnable_type.py
--rw-r--r--   0        0        0     2094 2023-04-18 06:31:51.009569 windmill_api-1.88.1/windmill_api/models/create_resource.py
--rw-r--r--   0        0        0     2140 2023-04-18 06:31:51.017569 windmill_api-1.88.1/windmill_api/models/create_resource_json_body.py
--rw-r--r--   0        0        0     2335 2023-04-18 06:31:51.045570 windmill_api-1.88.1/windmill_api/models/create_resource_type_json_body.py
--rw-r--r--   0        0        0     2780 2023-04-18 06:31:51.057570 windmill_api-1.88.1/windmill_api/models/create_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-04-18 06:31:51.061570 windmill_api-1.88.1/windmill_api/models/create_schedule_json_body_args.py
--rw-r--r--   0        0        0     4616 2023-04-18 06:31:51.125570 windmill_api-1.88.1/windmill_api/models/create_script_json_body.py
--rw-r--r--   0        0        0      249 2023-04-18 06:31:43.545488 windmill_api-1.88.1/windmill_api/models/create_script_json_body_kind.py
--rw-r--r--   0        0        0      207 2023-04-18 06:31:43.293485 windmill_api-1.88.1/windmill_api/models/create_script_json_body_language.py
--rw-r--r--   0        0        0     1232 2023-04-18 06:31:51.085570 windmill_api-1.88.1/windmill_api/models/create_script_json_body_schema.py
--rw-r--r--   0        0        0     2534 2023-04-18 06:31:51.121570 windmill_api-1.88.1/windmill_api/models/create_token_impersonate_json_body.py
--rw-r--r--   0        0        0     2169 2023-04-18 06:31:51.153571 windmill_api-1.88.1/windmill_api/models/create_token_json_body.py
--rw-r--r--   0        0        0     2364 2023-04-18 06:31:51.161571 windmill_api-1.88.1/windmill_api/models/create_user_globally_json_body.py
--rw-r--r--   0        0        0     1771 2023-04-18 06:31:51.181571 windmill_api-1.88.1/windmill_api/models/create_user_json_body.py
--rw-r--r--   0        0        0     2493 2023-04-18 06:31:51.201571 windmill_api-1.88.1/windmill_api/models/create_variable.py
--rw-r--r--   0        0        0     2539 2023-04-18 06:31:51.221571 windmill_api-1.88.1/windmill_api/models/create_variable_json_body.py
--rw-r--r--   0        0        0     1678 2023-04-18 06:31:51.245572 windmill_api-1.88.1/windmill_api/models/create_workspace.py
--rw-r--r--   0        0        0     1724 2023-04-18 06:31:51.277572 windmill_api-1.88.1/windmill_api/models/create_workspace_json_body.py
--rw-r--r--   0        0        0     1490 2023-04-18 06:31:51.269572 windmill_api-1.88.1/windmill_api/models/decline_invite_json_body.py
--rw-r--r--   0        0        0    10978 2023-04-18 06:31:51.433574 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200.py
--rw-r--r--   0        0        0     1270 2023-04-18 06:31:51.293572 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3658 2023-04-18 06:31:51.361573 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7442 2023-04-18 06:31:51.441574 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1883 2023-04-18 06:31:51.461574 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2318 2023-04-18 06:31:51.469574 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      219 2023-04-18 06:31:43.153484 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1788 2023-04-18 06:31:51.489574 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2324 2023-04-18 06:31:51.505575 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      377 2023-04-18 06:31:43.901492 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7053 2023-04-18 06:31:51.573575 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1873 2023-04-18 06:31:51.529575 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2298 2023-04-18 06:31:51.553575 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      217 2023-04-18 06:31:43.853491 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1778 2023-04-18 06:31:51.581575 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2314 2023-04-18 06:31:51.613576 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      375 2023-04-18 06:31:44.065494 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2134 2023-04-18 06:31:51.613576 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      327 2023-04-18 06:31:44.021493 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      216 2023-04-18 06:31:44.049493 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3432 2023-04-18 06:31:51.657576 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7425 2023-04-18 06:31:51.745577 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3442 2023-04-18 06:31:51.725577 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2023 2023-04-18 06:31:51.753577 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2327 2023-04-18 06:31:51.777577 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2261 2023-04-18 06:31:51.777577 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      198 2023-04-18 06:31:43.101483 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-18 06:31:51.805578 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      198 2023-04-18 06:31:43.749490 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2016 2023-04-18 06:31:51.813578 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2067 2023-04-18 06:31:51.833578 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7349 2023-04-18 06:31:51.897579 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3408 2023-04-18 06:31:51.873579 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2013 2023-04-18 06:31:51.905579 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2317 2023-04-18 06:31:51.933579 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2241 2023-04-18 06:31:51.929579 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-04-18 06:31:43.185484 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2108 2023-04-18 06:31:51.957579 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-04-18 06:31:43.653489 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2006 2023-04-18 06:31:51.965580 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2057 2023-04-18 06:31:51.985580 windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1783 2023-04-18 06:31:51.993580 windmill_api-1.88.1/windmill_api/models/delete_invite_json_body.py
--rw-r--r--   0        0        0     6853 2023-04-18 06:31:52.097581 windmill_api-1.88.1/windmill_api/models/delete_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1309 2023-04-18 06:31:52.013580 windmill_api-1.88.1/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      258 2023-04-18 06:31:43.705490 windmill_api-1.88.1/windmill_api/models/delete_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      216 2023-04-18 06:31:43.973493 windmill_api-1.88.1/windmill_api/models/delete_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1283 2023-04-18 06:31:52.037580 windmill_api-1.88.1/windmill_api/models/delete_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     2933 2023-04-18 06:31:52.081581 windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-04-18 06:31:52.189582 windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-04-18 06:31:43.429487 windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-04-18 06:31:52.121581 windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-04-18 06:31:52.145582 windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-04-18 06:31:52.173582 windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-04-18 06:31:52.209582 windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-04-18 06:31:43.137484 windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-04-18 06:31:52.213582 windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-04-18 06:31:52.245583 windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-04-18 06:31:43.489488 windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-04-18 06:31:52.241583 windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-04-18 06:31:43.597488 windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     1551 2023-04-18 06:31:52.269583 windmill_api-1.88.1/windmill_api/models/edit_auto_invite_json_body.py
--rw-r--r--   0        0        0     1980 2023-04-18 06:31:52.277583 windmill_api-1.88.1/windmill_api/models/edit_resource.py
--rw-r--r--   0        0        0     1791 2023-04-18 06:31:52.301583 windmill_api-1.88.1/windmill_api/models/edit_resource_type.py
--rw-r--r--   0        0        0     1845 2023-04-18 06:31:52.305583 windmill_api-1.88.1/windmill_api/models/edit_schedule.py
--rw-r--r--   0        0        0     1176 2023-04-18 06:31:52.321584 windmill_api-1.88.1/windmill_api/models/edit_schedule_args.py
--rw-r--r--   0        0        0     1691 2023-04-18 06:31:52.329584 windmill_api-1.88.1/windmill_api/models/edit_slack_command_json_body.py
--rw-r--r--   0        0        0     2260 2023-04-18 06:31:52.357584 windmill_api-1.88.1/windmill_api/models/edit_variable.py
--rw-r--r--   0        0        0     1520 2023-04-18 06:31:52.353584 windmill_api-1.88.1/windmill_api/models/edit_webhook_json_body.py
--rw-r--r--   0        0        0     2058 2023-04-18 06:31:52.385584 windmill_api-1.88.1/windmill_api/models/edit_workspace_user.py
--rw-r--r--   0        0        0     3663 2023-04-18 06:31:52.405584 windmill_api-1.88.1/windmill_api/models/execute_component_json_body.py
--rw-r--r--   0        0        0     1346 2023-04-18 06:31:52.401584 windmill_api-1.88.1/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
--rw-r--r--   0        0        0     1942 2023-04-18 06:31:52.461585 windmill_api-1.88.1/windmill_api/models/execute_component_json_body_raw_code.py
--rw-r--r--   0        0        0     1577 2023-04-18 06:31:52.433585 windmill_api-1.88.1/windmill_api/models/exists_username_json_body.py
--rw-r--r--   0        0        0     1400 2023-04-18 06:31:52.453585 windmill_api-1.88.1/windmill_api/models/exists_workspace_json_body.py
--rw-r--r--   0        0        0     4633 2023-04-18 06:31:52.561586 windmill_api-1.88.1/windmill_api/models/flow.py
--rw-r--r--   0        0        0     1166 2023-04-18 06:31:52.481585 windmill_api-1.88.1/windmill_api/models/flow_extra_perms.py
--rw-r--r--   0        0        0     3416 2023-04-18 06:31:52.525586 windmill_api-1.88.1/windmill_api/models/flow_metadata.py
--rw-r--r--   0        0        0     1209 2023-04-18 06:31:52.545586 windmill_api-1.88.1/windmill_api/models/flow_metadata_extra_perms.py
--rw-r--r--   0        0        0     5729 2023-04-18 06:31:52.629587 windmill_api-1.88.1/windmill_api/models/flow_module.py
--rw-r--r--   0        0        0     2726 2023-04-18 06:31:52.601587 windmill_api-1.88.1/windmill_api/models/flow_module_retry.py
--rw-r--r--   0        0        0     1807 2023-04-18 06:31:52.629587 windmill_api-1.88.1/windmill_api/models/flow_module_retry_constant.py
--rw-r--r--   0        0        0     2111 2023-04-18 06:31:52.665587 windmill_api-1.88.1/windmill_api/models/flow_module_retry_exponential.py
--rw-r--r--   0        0        0     1834 2023-04-18 06:31:52.657587 windmill_api-1.88.1/windmill_api/models/flow_module_sleep_type_0.py
--rw-r--r--   0        0        0      159 2023-04-18 06:31:43.193484 windmill_api-1.88.1/windmill_api/models/flow_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1701 2023-04-18 06:31:52.685588 windmill_api-1.88.1/windmill_api/models/flow_module_sleep_type_1.py
--rw-r--r--   0        0        0      159 2023-04-18 06:31:43.197484 windmill_api-1.88.1/windmill_api/models/flow_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1800 2023-04-18 06:31:52.693588 windmill_api-1.88.1/windmill_api/models/flow_module_stop_after_if.py
--rw-r--r--   0        0        0     1851 2023-04-18 06:31:52.713588 windmill_api-1.88.1/windmill_api/models/flow_module_suspend.py
--rw-r--r--   0        0        0     3080 2023-04-18 06:31:52.733588 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_0.py
--rw-r--r--   0        0        0     3564 2023-04-18 06:31:52.749588 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-18 06:31:52.765588 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-18 06:31:43.133484 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-18 06:31:52.777588 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-18 06:31:43.145484 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      208 2023-04-18 06:31:43.757490 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_0_language.py
--rw-r--r--   0        0        0      158 2023-04-18 06:31:43.449487 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_0_type.py
--rw-r--r--   0        0        0     2477 2023-04-18 06:31:52.825589 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_1.py
--rw-r--r--   0        0        0     3564 2023-04-18 06:31:52.813589 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-18 06:31:52.841589 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-18 06:31:43.141484 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-18 06:31:52.857589 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-18 06:31:43.445487 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      152 2023-04-18 06:31:43.373486 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_1_type.py
--rw-r--r--   0        0        0     2204 2023-04-18 06:31:52.873590 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_2.py
--rw-r--r--   0        0        0     3564 2023-04-18 06:31:52.893590 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-18 06:31:52.933590 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-18 06:31:43.953492 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-18 06:31:52.921590 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-18 06:31:44.081494 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      148 2023-04-18 06:31:43.697490 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_2_type.py
--rw-r--r--   0        0        0     4138 2023-04-18 06:31:52.973591 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3.py
--rw-r--r--   0        0        0     1990 2023-04-18 06:31:52.957590 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
--rw-r--r--   0        0        0      173 2023-04-18 06:31:43.205484 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
--rw-r--r--   0        0        0     1857 2023-04-18 06:31:53.001591 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
--rw-r--r--   0        0        0      173 2023-04-18 06:31:44.045493 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
--rw-r--r--   0        0        0     6636 2023-04-18 06:31:53.057592 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item.py
--rw-r--r--   0        0        0     3148 2023-04-18 06:31:53.041592 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
--rw-r--r--   0        0        0     1935 2023-04-18 06:31:53.073592 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-04-18 06:31:53.089592 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-04-18 06:31:53.101592 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-18 06:31:43.353486 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-04-18 06:31:53.117592 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-18 06:31:43.877492 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-04-18 06:31:53.133592 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-04-18 06:31:53.141593 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
--rw-r--r--   0        0        0      162 2023-04-18 06:31:43.153484 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_type.py
--rw-r--r--   0        0        0     2934 2023-04-18 06:31:53.173593 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4.py
--rw-r--r--   0        0        0     2508 2023-04-18 06:31:53.209593 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item.py
--rw-r--r--   0        0        0     7243 2023-04-18 06:31:53.257594 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-04-18 06:31:53.249594 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-04-18 06:31:53.277594 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-04-18 06:31:53.337595 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-04-18 06:31:53.305594 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-18 06:31:43.485487 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-04-18 06:31:53.333595 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-18 06:31:43.737490 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-04-18 06:31:53.361595 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-04-18 06:31:53.365595 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6636 2023-04-18 06:31:53.437596 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item.py
--rw-r--r--   0        0        0     3148 2023-04-18 06:31:53.405595 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
--rw-r--r--   0        0        0     1935 2023-04-18 06:31:53.433596 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-04-18 06:31:53.469596 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-04-18 06:31:53.465596 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-18 06:31:43.129484 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-04-18 06:31:53.497596 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-18 06:31:43.621489 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-04-18 06:31:53.497596 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-04-18 06:31:53.525597 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
--rw-r--r--   0        0        0      158 2023-04-18 06:31:43.881492 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_type.py
--rw-r--r--   0        0        0     2577 2023-04-18 06:31:53.537597 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5.py
--rw-r--r--   0        0        0     2679 2023-04-18 06:31:53.597597 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item.py
--rw-r--r--   0        0        0     7243 2023-04-18 06:31:53.621598 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-04-18 06:31:53.633598 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-04-18 06:31:53.649598 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-04-18 06:31:53.665598 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-04-18 06:31:53.725599 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-18 06:31:44.053494 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-04-18 06:31:53.693599 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-18 06:31:43.397486 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-04-18 06:31:53.721599 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-04-18 06:31:53.753599 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      158 2023-04-18 06:31:43.781491 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_type.py
--rw-r--r--   0        0        0     1839 2023-04-18 06:31:53.757599 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_6.py
--rw-r--r--   0        0        0      156 2023-04-18 06:31:43.625489 windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_6_type.py
--rw-r--r--   0        0        0     2009 2023-04-18 06:31:53.785600 windmill_api-1.88.1/windmill_api/models/flow_preview.py
--rw-r--r--   0        0        0     1171 2023-04-18 06:31:53.777600 windmill_api-1.88.1/windmill_api/models/flow_preview_args.py
--rw-r--r--   0        0        0     3074 2023-04-18 06:31:53.817600 windmill_api-1.88.1/windmill_api/models/flow_preview_value.py
--rw-r--r--   0        0        0     6498 2023-04-18 06:31:53.869601 windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module.py
--rw-r--r--   0        0        0     3064 2023-04-18 06:31:53.857601 windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_retry.py
--rw-r--r--   0        0        0     1911 2023-04-18 06:31:53.885601 windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2215 2023-04-18 06:31:53.901601 windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2036 2023-04-18 06:31:53.913601 windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-18 06:31:43.445487 windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1903 2023-04-18 06:31:53.929601 windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-18 06:31:43.405486 windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1904 2023-04-18 06:31:53.945601 windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1955 2023-04-18 06:31:53.993602 windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6422 2023-04-18 06:31:54.021602 windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item.py
--rw-r--r--   0        0        0     3030 2023-04-18 06:31:54.033602 windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_retry.py
--rw-r--r--   0        0        0     1901 2023-04-18 06:31:54.049603 windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2205 2023-04-18 06:31:54.065603 windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2016 2023-04-18 06:31:54.121603 windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-04-18 06:31:43.881492 windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1883 2023-04-18 06:31:54.093603 windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-04-18 06:31:43.449487 windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1894 2023-04-18 06:31:54.121603 windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1945 2023-04-18 06:31:54.153604 windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1143 2023-04-18 06:31:54.141604 windmill_api-1.88.1/windmill_api/models/flow_schema.py
--rw-r--r--   0        0        0     3001 2023-04-18 06:31:54.185604 windmill_api-1.88.1/windmill_api/models/flow_status.py
--rw-r--r--   0        0        0     6370 2023-04-18 06:31:54.241605 windmill_api-1.88.1/windmill_api/models/flow_status_failure_module.py
--rw-r--r--   0        0        0     1723 2023-04-18 06:31:54.209604 windmill_api-1.88.1/windmill_api/models/flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     1999 2023-04-18 06:31:54.245605 windmill_api-1.88.1/windmill_api/models/flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      190 2023-04-18 06:31:43.361486 windmill_api-1.88.1/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1628 2023-04-18 06:31:54.269605 windmill_api-1.88.1/windmill_api/models/flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2164 2023-04-18 06:31:54.281605 windmill_api-1.88.1/windmill_api/models/flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      348 2023-04-18 06:31:43.133484 windmill_api-1.88.1/windmill_api/models/flow_status_failure_module_type.py
--rw-r--r--   0        0        0     5808 2023-04-18 06:31:54.389606 windmill_api-1.88.1/windmill_api/models/flow_status_module.py
--rw-r--r--   0        0        0     1685 2023-04-18 06:31:54.309605 windmill_api-1.88.1/windmill_api/models/flow_status_module_approvers_item.py
--rw-r--r--   0        0        0     1925 2023-04-18 06:31:54.337606 windmill_api-1.88.1/windmill_api/models/flow_status_module_branch_chosen.py
--rw-r--r--   0        0        0      183 2023-04-18 06:31:43.413487 windmill_api-1.88.1/windmill_api/models/flow_status_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1590 2023-04-18 06:31:54.361606 windmill_api-1.88.1/windmill_api/models/flow_status_module_branchall.py
--rw-r--r--   0        0        0     2126 2023-04-18 06:31:54.397606 windmill_api-1.88.1/windmill_api/models/flow_status_module_iterator.py
--rw-r--r--   0        0        0      341 2023-04-18 06:31:43.885492 windmill_api-1.88.1/windmill_api/models/flow_status_module_type.py
--rw-r--r--   0        0        0     5981 2023-04-18 06:31:54.469607 windmill_api-1.88.1/windmill_api/models/flow_status_modules_item.py
--rw-r--r--   0        0        0     1713 2023-04-18 06:31:54.421607 windmill_api-1.88.1/windmill_api/models/flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     1979 2023-04-18 06:31:54.449607 windmill_api-1.88.1/windmill_api/models/flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      188 2023-04-18 06:31:43.229485 windmill_api-1.88.1/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1618 2023-04-18 06:31:54.477607 windmill_api-1.88.1/windmill_api/models/flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2154 2023-04-18 06:31:54.505607 windmill_api-1.88.1/windmill_api/models/flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      346 2023-04-18 06:31:43.233485 windmill_api-1.88.1/windmill_api/models/flow_status_modules_item_type.py
--rw-r--r--   0        0        0     1974 2023-04-18 06:31:54.553608 windmill_api-1.88.1/windmill_api/models/flow_status_retry.py
--rw-r--r--   0        0        0     2957 2023-04-18 06:31:54.541608 windmill_api-1.88.1/windmill_api/models/flow_value.py
--rw-r--r--   0        0        0     6224 2023-04-18 06:31:54.621609 windmill_api-1.88.1/windmill_api/models/flow_value_failure_module.py
--rw-r--r--   0        0        0     2940 2023-04-18 06:31:54.593608 windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1873 2023-04-18 06:31:54.625609 windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-04-18 06:31:54.653609 windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-04-18 06:31:54.657609 windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-04-18 06:31:43.245485 windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-04-18 06:31:54.681609 windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-04-18 06:31:43.389486 windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-04-18 06:31:54.689610 windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-04-18 06:31:54.757610 windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6125 2023-04-18 06:31:54.781611 windmill_api-1.88.1/windmill_api/models/flow_value_modules_item.py
--rw-r--r--   0        0        0     2906 2023-04-18 06:31:54.797611 windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1863 2023-04-18 06:31:54.809611 windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-04-18 06:31:54.829611 windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-04-18 06:31:54.837611 windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-04-18 06:31:44.085494 windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-04-18 06:31:54.857612 windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-04-18 06:31:43.509488 windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-04-18 06:31:54.865612 windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-04-18 06:31:54.889612 windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1858 2023-04-18 06:31:54.897612 windmill_api-1.88.1/windmill_api/models/folder.py
--rw-r--r--   0        0        0     1179 2023-04-18 06:31:54.909612 windmill_api-1.88.1/windmill_api/models/folder_extra_perms.py
--rw-r--r--   0        0        0     1560 2023-04-18 06:31:54.977613 windmill_api-1.88.1/windmill_api/models/force_cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     3807 2023-04-18 06:31:54.957613 windmill_api-1.88.1/windmill_api/models/forloop_flow.py
--rw-r--r--   0        0        0     1874 2023-04-18 06:31:54.989613 windmill_api-1.88.1/windmill_api/models/forloop_flow_iterator_type_0.py
--rw-r--r--   0        0        0      163 2023-04-18 06:31:43.713490 windmill_api-1.88.1/windmill_api/models/forloop_flow_iterator_type_0_type.py
--rw-r--r--   0        0        0     1741 2023-04-18 06:31:55.005613 windmill_api-1.88.1/windmill_api/models/forloop_flow_iterator_type_1.py
--rw-r--r--   0        0        0      163 2023-04-18 06:31:43.333486 windmill_api-1.88.1/windmill_api/models/forloop_flow_iterator_type_1_type.py
--rw-r--r--   0        0        0     6224 2023-04-18 06:31:55.069614 windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item.py
--rw-r--r--   0        0        0     2940 2023-04-18 06:31:55.045614 windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1873 2023-04-18 06:31:55.073614 windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-04-18 06:31:55.101614 windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-04-18 06:31:55.101614 windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-04-18 06:31:43.777490 windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-04-18 06:31:55.173615 windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-04-18 06:31:43.145484 windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-04-18 06:31:55.149615 windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-04-18 06:31:55.181615 windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_suspend.py
--rw-r--r--   0        0        0      152 2023-04-18 06:31:43.065483 windmill_api-1.88.1/windmill_api/models/forloop_flow_type.py
--rw-r--r--   0        0        0     4052 2023-04-18 06:31:55.221615 windmill_api-1.88.1/windmill_api/models/get_app_by_path_response_200.py
--rw-r--r--   0        0        0      219 2023-04-18 06:31:43.621489 windmill_api-1.88.1/windmill_api/models/get_app_by_path_response_200_execution_mode.py
--rw-r--r--   0        0        0     1279 2023-04-18 06:31:55.205615 windmill_api-1.88.1/windmill_api/models/get_app_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     3811 2023-04-18 06:31:55.257616 windmill_api-1.88.1/windmill_api/models/get_app_by_path_response_200_policy.py
--rw-r--r--   0        0        0      225 2023-04-18 06:31:43.369486 windmill_api-1.88.1/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2009 2023-04-18 06:31:55.249616 windmill_api-1.88.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1412 2023-04-18 06:31:55.265616 windmill_api-1.88.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4112 2023-04-18 06:31:55.309616 windmill_api-1.88.1/windmill_api/models/get_app_by_version_response_200.py
--rw-r--r--   0        0        0      222 2023-04-18 06:31:43.929492 windmill_api-1.88.1/windmill_api/models/get_app_by_version_response_200_execution_mode.py
--rw-r--r--   0        0        0     1294 2023-04-18 06:31:55.285616 windmill_api-1.88.1/windmill_api/models/get_app_by_version_response_200_extra_perms.py
--rw-r--r--   0        0        0     3862 2023-04-18 06:31:55.333617 windmill_api-1.88.1/windmill_api/models/get_app_by_version_response_200_policy.py
--rw-r--r--   0        0        0      228 2023-04-18 06:31:43.829491 windmill_api-1.88.1/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2042 2023-04-18 06:31:55.389617 windmill_api-1.88.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1427 2023-04-18 06:31:55.349617 windmill_api-1.88.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3764 2023-04-18 06:31:55.397617 windmill_api-1.88.1/windmill_api/models/get_audit_log_response_200.py
--rw-r--r--   0        0        0      231 2023-04-18 06:31:43.393486 windmill_api-1.88.1/windmill_api/models/get_audit_log_response_200_action_kind.py
--rw-r--r--   0        0        0      634 2023-04-18 06:31:43.289485 windmill_api-1.88.1/windmill_api/models/get_audit_log_response_200_operation.py
--rw-r--r--   0        0        0     1265 2023-04-18 06:31:55.413617 windmill_api-1.88.1/windmill_api/models/get_audit_log_response_200_parameters.py
--rw-r--r--   0        0        0    10876 2023-04-18 06:31:55.569619 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200.py
--rw-r--r--   0        0        0     1255 2023-04-18 06:31:55.433618 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3595 2023-04-18 06:31:55.477618 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7343 2023-04-18 06:31:55.561619 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1868 2023-04-18 06:31:55.589619 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2288 2023-04-18 06:31:55.597620 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      216 2023-04-18 06:31:43.665489 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1773 2023-04-18 06:31:55.617620 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2309 2023-04-18 06:31:55.629620 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      374 2023-04-18 06:31:43.433487 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6924 2023-04-18 06:31:55.705621 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1858 2023-04-18 06:31:55.653620 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-04-18 06:31:55.681620 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-04-18 06:31:43.629489 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-04-18 06:31:55.705621 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2299 2023-04-18 06:31:55.793622 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      372 2023-04-18 06:31:43.001482 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2119 2023-04-18 06:31:55.737621 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      324 2023-04-18 06:31:44.057494 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      213 2023-04-18 06:31:43.917492 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3375 2023-04-18 06:31:55.781622 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7311 2023-04-18 06:31:55.901623 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3391 2023-04-18 06:31:55.833622 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2008 2023-04-18 06:31:55.861622 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2312 2023-04-18 06:31:55.893623 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2231 2023-04-18 06:31:55.925623 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      195 2023-04-18 06:31:43.361486 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2098 2023-04-18 06:31:55.937623 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      195 2023-04-18 06:31:43.933492 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2001 2023-04-18 06:31:55.953624 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2052 2023-04-18 06:31:55.965624 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7235 2023-04-18 06:31:56.037624 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3357 2023-04-18 06:31:56.001624 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1998 2023-04-18 06:31:56.029624 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-04-18 06:31:56.065625 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-04-18 06:31:56.065625 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-18 06:31:43.033482 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-04-18 06:31:56.093625 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-18 06:31:43.653489 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-04-18 06:31:56.101625 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-04-18 06:31:56.121625 windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     5083 2023-04-18 06:31:56.165626 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200.py
--rw-r--r--   0        0        0     1281 2023-04-18 06:31:56.141626 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     1258 2023-04-18 06:31:56.213626 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_schema.py
--rw-r--r--   0        0        0     3302 2023-04-18 06:31:56.209626 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value.py
--rw-r--r--   0        0        0     7159 2023-04-18 06:31:56.353628 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
--rw-r--r--   0        0        0     3323 2023-04-18 06:31:56.249627 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
--rw-r--r--   0        0        0     1988 2023-04-18 06:31:56.281627 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-04-18 06:31:56.313628 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-04-18 06:31:56.341628 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-18 06:31:43.393486 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-04-18 06:31:56.373628 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-18 06:31:43.237485 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-04-18 06:31:56.381628 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-04-18 06:31:56.401629 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7066 2023-04-18 06:31:56.465629 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
--rw-r--r--   0        0        0     3289 2023-04-18 06:31:56.441629 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
--rw-r--r--   0        0        0     1978 2023-04-18 06:31:56.469629 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2282 2023-04-18 06:31:56.501630 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2171 2023-04-18 06:31:56.497630 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-18 06:31:43.441487 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2038 2023-04-18 06:31:56.529630 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-18 06:31:43.797491 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1971 2023-04-18 06:31:56.529630 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2022 2023-04-18 06:31:56.557630 windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2756 2023-04-18 06:31:56.569630 windmill_api-1.88.1/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
--rw-r--r--   0        0        0     1337 2023-04-18 06:31:56.577630 windmill_api-1.88.1/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
--rw-r--r--   0        0        0     2010 2023-04-18 06:31:56.601631 windmill_api-1.88.1/windmill_api/models/get_folder_response_200.py
--rw-r--r--   0        0        0     1258 2023-04-18 06:31:56.597631 windmill_api-1.88.1/windmill_api/models/get_folder_response_200_extra_perms.py
--rw-r--r--   0        0        0     2357 2023-04-18 06:31:56.681632 windmill_api-1.88.1/windmill_api/models/get_folder_usage_response_200.py
--rw-r--r--   0        0        0      301 2023-04-18 06:31:43.257485 windmill_api-1.88.1/windmill_api/models/get_granular_acls_kind.py
--rw-r--r--   0        0        0     1235 2023-04-18 06:31:56.625631 windmill_api-1.88.1/windmill_api/models/get_granular_acls_response_200.py
--rw-r--r--   0        0        0     2888 2023-04-18 06:31:56.665631 windmill_api-1.88.1/windmill_api/models/get_group_response_200.py
--rw-r--r--   0        0        0     1253 2023-04-18 06:31:56.753632 windmill_api-1.88.1/windmill_api/models/get_group_response_200_extra_perms.py
--rw-r--r--   0        0        0     1606 2023-04-18 06:31:56.705632 windmill_api-1.88.1/windmill_api/models/get_hub_app_by_id_response_200.py
--rw-r--r--   0        0        0     1634 2023-04-18 06:31:56.733632 windmill_api-1.88.1/windmill_api/models/get_hub_app_by_id_response_200_app.py
--rw-r--r--   0        0        0     1977 2023-04-18 06:31:56.761633 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200.py
--rw-r--r--   0        0        0     2950 2023-04-18 06:31:56.797633 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
--rw-r--r--   0        0        0     1289 2023-04-18 06:31:56.781633 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
--rw-r--r--   0        0        0     3410 2023-04-18 06:31:56.825633 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
--rw-r--r--   0        0        0     7365 2023-04-18 06:31:56.881634 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
--rw-r--r--   0        0        0     3418 2023-04-18 06:31:56.861634 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     2019 2023-04-18 06:31:56.889634 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2323 2023-04-18 06:31:56.913634 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2249 2023-04-18 06:31:56.917634 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-04-18 06:31:43.453487 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2116 2023-04-18 06:31:56.941635 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-04-18 06:31:43.273485 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2012 2023-04-18 06:31:56.949634 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2063 2023-04-18 06:31:56.969635 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7289 2023-04-18 06:31:57.085636 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
--rw-r--r--   0        0        0     3384 2023-04-18 06:31:57.009635 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     2009 2023-04-18 06:31:57.037635 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2313 2023-04-18 06:31:57.069636 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2229 2023-04-18 06:31:57.145637 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      194 2023-04-18 06:31:43.457487 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2096 2023-04-18 06:31:57.113636 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      194 2023-04-18 06:31:43.593489 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2002 2023-04-18 06:31:57.141637 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2053 2023-04-18 06:31:57.169637 windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2698 2023-04-18 06:31:57.181637 windmill_api-1.88.1/windmill_api/models/get_hub_script_by_path_response_200.py
--rw-r--r--   0        0        0      216 2023-04-18 06:31:43.109483 windmill_api-1.88.1/windmill_api/models/get_hub_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     2644 2023-04-18 06:31:57.209637 windmill_api-1.88.1/windmill_api/models/get_input_history_response_200_item.py
--rw-r--r--   0        0        0     1278 2023-04-18 06:31:57.201637 windmill_api-1.88.1/windmill_api/models/get_input_history_response_200_item_args.py
--rw-r--r--   0        0        0      218 2023-04-18 06:31:43.793491 windmill_api-1.88.1/windmill_api/models/get_input_history_runnable_type.py
--rw-r--r--   0        0        0     1852 2023-04-18 06:31:57.233638 windmill_api-1.88.1/windmill_api/models/get_job_response_200.py
--rw-r--r--   0        0        0      188 2023-04-18 06:31:43.869491 windmill_api-1.88.1/windmill_api/models/get_job_response_200_type.py
--rw-r--r--   0        0        0     2364 2023-04-18 06:31:57.249638 windmill_api-1.88.1/windmill_api/models/get_job_updates_response_200.py
--rw-r--r--   0        0        0     1744 2023-04-18 06:31:57.257638 windmill_api-1.88.1/windmill_api/models/get_premium_info_response_200.py
--rw-r--r--   0        0        0     4218 2023-04-18 06:31:57.297638 windmill_api-1.88.1/windmill_api/models/get_public_app_by_secret_response_200.py
--rw-r--r--   0        0        0      227 2023-04-18 06:31:43.629489 windmill_api-1.88.1/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
--rw-r--r--   0        0        0     1322 2023-04-18 06:31:57.281638 windmill_api-1.88.1/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
--rw-r--r--   0        0        0     3970 2023-04-18 06:31:57.329639 windmill_api-1.88.1/windmill_api/models/get_public_app_by_secret_response_200_policy.py
--rw-r--r--   0        0        0      233 2023-04-18 06:31:43.149484 windmill_api-1.88.1/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2131 2023-04-18 06:31:57.321639 windmill_api-1.88.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1455 2023-04-18 06:31:57.341639 windmill_api-1.88.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3533 2023-04-18 06:31:57.377639 windmill_api-1.88.1/windmill_api/models/get_resource_response_200.py
--rw-r--r--   0        0        0     1268 2023-04-18 06:31:57.361639 windmill_api-1.88.1/windmill_api/models/get_resource_response_200_extra_perms.py
--rw-r--r--   0        0        0     2335 2023-04-18 06:31:57.393639 windmill_api-1.88.1/windmill_api/models/get_resource_type_response_200.py
--rw-r--r--   0        0        0     1840 2023-04-18 06:31:57.405640 windmill_api-1.88.1/windmill_api/models/get_resume_urls_response_200.py
--rw-r--r--   0        0        0     4325 2023-04-18 06:31:57.493641 windmill_api-1.88.1/windmill_api/models/get_schedule_response_200.py
--rw-r--r--   0        0        0     1232 2023-04-18 06:31:57.425640 windmill_api-1.88.1/windmill_api/models/get_schedule_response_200_args.py
--rw-r--r--   0        0        0     1268 2023-04-18 06:31:57.445640 windmill_api-1.88.1/windmill_api/models/get_schedule_response_200_extra_perms.py
--rw-r--r--   0        0        0     6775 2023-04-18 06:31:57.585641 windmill_api-1.88.1/windmill_api/models/get_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1294 2023-04-18 06:31:57.517641 windmill_api-1.88.1/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-18 06:31:43.633489 windmill_api-1.88.1/windmill_api/models/get_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-04-18 06:31:43.137484 windmill_api-1.88.1/windmill_api/models/get_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-04-18 06:31:57.537641 windmill_api-1.88.1/windmill_api/models/get_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     6775 2023-04-18 06:31:57.621642 windmill_api-1.88.1/windmill_api/models/get_script_by_path_response_200.py
--rw-r--r--   0        0        0     1294 2023-04-18 06:31:57.609642 windmill_api-1.88.1/windmill_api/models/get_script_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-18 06:31:43.445487 windmill_api-1.88.1/windmill_api/models/get_script_by_path_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-04-18 06:31:43.933492 windmill_api-1.88.1/windmill_api/models/get_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-04-18 06:31:57.633642 windmill_api-1.88.1/windmill_api/models/get_script_by_path_response_200_schema.py
--rw-r--r--   0        0        0     1922 2023-04-18 06:31:57.649642 windmill_api-1.88.1/windmill_api/models/get_script_deployment_status_response_200.py
--rw-r--r--   0        0        0     4157 2023-04-18 06:31:57.689643 windmill_api-1.88.1/windmill_api/models/get_settings_response_200.py
--rw-r--r--   0        0        0     2428 2023-04-18 06:31:57.681643 windmill_api-1.88.1/windmill_api/models/get_suspended_job_flow_response_200.py
--rw-r--r--   0        0        0     1764 2023-04-18 06:31:57.705643 windmill_api-1.88.1/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
--rw-r--r--   0        0        0     2040 2023-04-18 06:31:57.717643 windmill_api-1.88.1/windmill_api/models/get_suspended_job_flow_response_200_job.py
--rw-r--r--   0        0        0      204 2023-04-18 06:31:43.137484 windmill_api-1.88.1/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
--rw-r--r--   0        0        0     4554 2023-04-18 06:31:57.769644 windmill_api-1.88.1/windmill_api/models/get_variable_response_200.py
--rw-r--r--   0        0        0     1268 2023-04-18 06:31:57.737643 windmill_api-1.88.1/windmill_api/models/get_variable_response_200_extra_perms.py
--rw-r--r--   0        0        0     2647 2023-04-18 06:31:57.777644 windmill_api-1.88.1/windmill_api/models/global_user_info.py
--rw-r--r--   0        0        0      176 2023-04-18 06:31:43.169484 windmill_api-1.88.1/windmill_api/models/global_user_info_login_type.py
--rw-r--r--   0        0        0     1627 2023-04-18 06:31:57.793644 windmill_api-1.88.1/windmill_api/models/global_user_update_json_body.py
--rw-r--r--   0        0        0     2741 2023-04-18 06:31:57.813644 windmill_api-1.88.1/windmill_api/models/global_whoami_response_200.py
--rw-r--r--   0        0        0      185 2023-04-18 06:31:43.093483 windmill_api-1.88.1/windmill_api/models/global_whoami_response_200_login_type.py
--rw-r--r--   0        0        0     2903 2023-04-18 06:31:57.893645 windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5478 2023-04-18 06:31:57.873645 windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      324 2023-04-18 06:31:43.369486 windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1598 2023-04-18 06:31:57.897645 windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1663 2023-04-18 06:31:57.917645 windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2151 2023-04-18 06:31:57.929645 windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3257 2023-04-18 06:31:57.953646 windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      342 2023-04-18 06:31:43.745490 windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1631 2023-04-18 06:31:58.009646 windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3100 2023-04-18 06:31:57.989646 windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      333 2023-04-18 06:31:43.753490 windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1580 2023-04-18 06:31:58.017646 windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      178 2023-04-18 06:31:43.077483 windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2722 2023-04-18 06:31:58.053647 windmill_api-1.88.1/windmill_api/models/group.py
--rw-r--r--   0        0        0     1174 2023-04-18 06:31:58.033646 windmill_api-1.88.1/windmill_api/models/group_extra_perms.py
--rw-r--r--   0        0        0     1689 2023-04-18 06:31:58.065647 windmill_api-1.88.1/windmill_api/models/identity.py
--rw-r--r--   0        0        0      143 2023-04-18 06:31:43.721490 windmill_api-1.88.1/windmill_api/models/identity_type.py
--rw-r--r--   0        0        0     2377 2023-04-18 06:31:58.093647 windmill_api-1.88.1/windmill_api/models/input_.py
--rw-r--r--   0        0        0     1138 2023-04-18 06:31:58.085647 windmill_api-1.88.1/windmill_api/models/input_args.py
--rw-r--r--   0        0        0     1820 2023-04-18 06:31:58.113647 windmill_api-1.88.1/windmill_api/models/input_transform_type_0.py
--rw-r--r--   0        0        0      158 2023-04-18 06:31:43.605489 windmill_api-1.88.1/windmill_api/models/input_transform_type_0_type.py
--rw-r--r--   0        0        0     1687 2023-04-18 06:31:58.125647 windmill_api-1.88.1/windmill_api/models/input_transform_type_1.py
--rw-r--r--   0        0        0      158 2023-04-18 06:31:43.509488 windmill_api-1.88.1/windmill_api/models/input_transform_type_1_type.py
--rw-r--r--   0        0        0     1773 2023-04-18 06:31:58.141648 windmill_api-1.88.1/windmill_api/models/invite_user_json_body.py
--rw-r--r--   0        0        0     1679 2023-04-18 06:31:58.153648 windmill_api-1.88.1/windmill_api/models/javascript_transform.py
--rw-r--r--   0        0        0      158 2023-04-18 06:31:44.077494 windmill_api-1.88.1/windmill_api/models/javascript_transform_type.py
--rw-r--r--   0        0        0     1686 2023-04-18 06:31:58.173648 windmill_api-1.88.1/windmill_api/models/job.py
--rw-r--r--   0        0        0      174 2023-04-18 06:31:43.425487 windmill_api-1.88.1/windmill_api/models/job_type.py
--rw-r--r--   0        0        0     3583 2023-04-18 06:31:58.197648 windmill_api-1.88.1/windmill_api/models/list_apps_response_200_item.py
--rw-r--r--   0        0        0      219 2023-04-18 06:31:43.209484 windmill_api-1.88.1/windmill_api/models/list_apps_response_200_item_execution_mode.py
--rw-r--r--   0        0        0     1276 2023-04-18 06:31:58.193648 windmill_api-1.88.1/windmill_api/models/list_apps_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      218 2023-04-18 06:31:43.333486 windmill_api-1.88.1/windmill_api/models/list_audit_logs_action_kind.py
--rw-r--r--   0        0        0     3896 2023-04-18 06:31:58.293649 windmill_api-1.88.1/windmill_api/models/list_audit_logs_response_200_item.py
--rw-r--r--   0        0        0      237 2023-04-18 06:31:43.781491 windmill_api-1.88.1/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
--rw-r--r--   0        0        0      640 2023-04-18 06:31:43.773491 windmill_api-1.88.1/windmill_api/models/list_audit_logs_response_200_item_operation.py
--rw-r--r--   0        0        0     1298 2023-04-18 06:31:58.221649 windmill_api-1.88.1/windmill_api/models/list_audit_logs_response_200_item_parameters.py
--rw-r--r--   0        0        0    11088 2023-04-18 06:31:58.353650 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item.py
--rw-r--r--   0        0        0     1288 2023-04-18 06:31:58.313650 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_args.py
--rw-r--r--   0        0        0     3736 2023-04-18 06:31:58.357650 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7579 2023-04-18 06:31:58.489651 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1901 2023-04-18 06:31:58.385650 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2352 2023-04-18 06:31:58.409651 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      222 2023-04-18 06:31:43.245485 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1806 2023-04-18 06:31:58.437651 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2342 2023-04-18 06:31:58.473651 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      380 2023-04-18 06:31:43.373486 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7160 2023-04-18 06:31:58.553652 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1891 2023-04-18 06:31:58.517652 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2332 2023-04-18 06:31:58.545652 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      220 2023-04-18 06:31:43.645489 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1796 2023-04-18 06:31:58.569652 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2332 2023-04-18 06:31:58.589652 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      378 2023-04-18 06:31:44.057494 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2152 2023-04-18 06:31:58.605653 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      330 2023-04-18 06:31:43.089483 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
--rw-r--r--   0        0        0      219 2023-04-18 06:31:43.377486 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_language.py
--rw-r--r--   0        0        0     3485 2023-04-18 06:31:58.633653 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7593 2023-04-18 06:31:58.685654 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3498 2023-04-18 06:31:58.729654 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2041 2023-04-18 06:31:58.713654 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2345 2023-04-18 06:31:58.745654 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2295 2023-04-18 06:31:58.757654 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      201 2023-04-18 06:31:43.945492 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2162 2023-04-18 06:31:58.829655 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      201 2023-04-18 06:31:43.457487 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2034 2023-04-18 06:31:58.785655 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2085 2023-04-18 06:31:58.813655 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7471 2023-04-18 06:31:58.893656 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3464 2023-04-18 06:31:58.869655 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2031 2023-04-18 06:31:58.897656 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2335 2023-04-18 06:31:58.921656 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2275 2023-04-18 06:31:58.925656 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      199 2023-04-18 06:31:43.677489 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2142 2023-04-18 06:31:58.949656 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      199 2023-04-18 06:31:43.765490 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2024 2023-04-18 06:31:58.957656 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2075 2023-04-18 06:31:58.977657 windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1865 2023-04-18 06:31:58.985657 windmill_api-1.88.1/windmill_api/models/list_contextual_variables_response_200_item.py
--rw-r--r--   0        0        0     5077 2023-04-18 06:31:59.101658 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item.py
--rw-r--r--   0        0        0     1278 2023-04-18 06:31:59.005657 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     1255 2023-04-18 06:31:59.025657 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_schema.py
--rw-r--r--   0        0        0     3297 2023-04-18 06:31:59.065658 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value.py
--rw-r--r--   0        0        0     7151 2023-04-18 06:31:59.149659 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module.py
--rw-r--r--   0        0        0     3318 2023-04-18 06:31:59.141658 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py
--rw-r--r--   0        0        0     1985 2023-04-18 06:31:59.169659 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2289 2023-04-18 06:31:59.241659 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2187 2023-04-18 06:31:59.197659 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-18 06:31:43.013482 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2054 2023-04-18 06:31:59.225659 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-18 06:31:43.297485 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1978 2023-04-18 06:31:59.253660 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2029 2023-04-18 06:31:59.269660 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7049 2023-04-18 06:31:59.337661 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item.py
--rw-r--r--   0        0        0     3284 2023-04-18 06:31:59.309660 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py
--rw-r--r--   0        0        0     1975 2023-04-18 06:31:59.337661 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-04-18 06:31:59.369661 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-04-18 06:31:59.365661 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-18 06:31:43.845491 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-04-18 06:31:59.397661 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-18 06:31:43.961493 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-04-18 06:31:59.397661 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-04-18 06:31:59.421661 windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2074 2023-04-18 06:31:59.429662 windmill_api-1.88.1/windmill_api/models/list_folders_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-04-18 06:31:59.501662 windmill_api-1.88.1/windmill_api/models/list_folders_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2958 2023-04-18 06:31:59.473662 windmill_api-1.88.1/windmill_api/models/list_groups_response_200_item.py
--rw-r--r--   0        0        0     1286 2023-04-18 06:31:59.493662 windmill_api-1.88.1/windmill_api/models/list_groups_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2076 2023-04-18 06:31:59.525663 windmill_api-1.88.1/windmill_api/models/list_hub_apps_response_200.py
--rw-r--r--   0        0        0     2304 2023-04-18 06:31:59.537663 windmill_api-1.88.1/windmill_api/models/list_hub_apps_response_200_apps_item.py
--rw-r--r--   0        0        0     2116 2023-04-18 06:31:59.557663 windmill_api-1.88.1/windmill_api/models/list_hub_flows_response_200.py
--rw-r--r--   0        0        0     2324 2023-04-18 06:31:59.573663 windmill_api-1.88.1/windmill_api/models/list_hub_flows_response_200_flows_item.py
--rw-r--r--   0        0        0     2106 2023-04-18 06:31:59.589663 windmill_api-1.88.1/windmill_api/models/list_hub_scripts_response_200.py
--rw-r--r--   0        0        0     2790 2023-04-18 06:31:59.609664 windmill_api-1.88.1/windmill_api/models/list_hub_scripts_response_200_asks_item.py
--rw-r--r--   0        0        0      262 2023-04-18 06:31:43.589489 windmill_api-1.88.1/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
--rw-r--r--   0        0        0     2590 2023-04-18 06:31:59.629664 windmill_api-1.88.1/windmill_api/models/list_inputs_response_200_item.py
--rw-r--r--   0        0        0     1250 2023-04-18 06:31:59.629664 windmill_api-1.88.1/windmill_api/models/list_inputs_response_200_item_args.py
--rw-r--r--   0        0        0      213 2023-04-18 06:31:43.153484 windmill_api-1.88.1/windmill_api/models/list_inputs_runnable_type.py
--rw-r--r--   0        0        0     1922 2023-04-18 06:31:59.657664 windmill_api-1.88.1/windmill_api/models/list_jobs_response_200_item.py
--rw-r--r--   0        0        0      194 2023-04-18 06:31:43.217485 windmill_api-1.88.1/windmill_api/models/list_jobs_response_200_item_type.py
--rw-r--r--   0        0        0     2076 2023-04-18 06:31:59.665664 windmill_api-1.88.1/windmill_api/models/list_pending_invites_response_200_item.py
--rw-r--r--   0        0        0    11982 2023-04-18 06:31:59.801666 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item.py
--rw-r--r--   0        0        0     1245 2023-04-18 06:31:59.745665 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_args.py
--rw-r--r--   0        0        0     3544 2023-04-18 06:31:59.789666 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7247 2023-04-18 06:31:59.873666 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1858 2023-04-18 06:31:59.829666 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-04-18 06:31:59.917667 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-04-18 06:31:43.873492 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-04-18 06:31:59.901667 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2299 2023-04-18 06:31:59.933667 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      372 2023-04-18 06:31:43.213484 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6858 2023-04-18 06:32:00.001668 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1848 2023-04-18 06:31:59.961667 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2248 2023-04-18 06:31:59.989668 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      212 2023-04-18 06:31:43.221485 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1753 2023-04-18 06:32:00.013668 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2289 2023-04-18 06:32:00.037668 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      370 2023-04-18 06:31:43.881492 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2109 2023-04-18 06:32:00.049668 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      322 2023-04-18 06:31:43.005482 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_job_kind.py
--rw-r--r--   0        0        0      211 2023-04-18 06:31:43.625489 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_language.py
--rw-r--r--   0        0        0     3334 2023-04-18 06:32:00.081669 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7235 2023-04-18 06:32:00.189670 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3357 2023-04-18 06:32:00.121669 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1998 2023-04-18 06:32:00.149670 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-04-18 06:32:00.181670 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-04-18 06:32:00.213670 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-18 06:31:43.589489 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-04-18 06:32:00.221670 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-18 06:31:43.821491 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-04-18 06:32:00.241670 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-04-18 06:32:00.249671 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7159 2023-04-18 06:32:00.393672 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3323 2023-04-18 06:32:00.289671 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1988 2023-04-18 06:32:00.317671 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-04-18 06:32:00.349672 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-04-18 06:32:00.377672 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-18 06:31:43.001482 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-04-18 06:32:00.409672 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-18 06:31:43.421487 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-04-18 06:32:00.421672 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-04-18 06:32:00.437672 windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     4884 2023-04-18 06:32:00.485673 windmill_api-1.88.1/windmill_api/models/list_resource_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-04-18 06:32:00.453673 windmill_api-1.88.1/windmill_api/models/list_resource_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2363 2023-04-18 06:32:00.489673 windmill_api-1.88.1/windmill_api/models/list_resource_type_response_200_item.py
--rw-r--r--   0        0        0     4426 2023-04-18 06:32:00.541674 windmill_api-1.88.1/windmill_api/models/list_schedules_response_200_item.py
--rw-r--r--   0        0        0     1265 2023-04-18 06:32:00.509673 windmill_api-1.88.1/windmill_api/models/list_schedules_response_200_item_args.py
--rw-r--r--   0        0        0     1301 2023-04-18 06:32:00.529673 windmill_api-1.88.1/windmill_api/models/list_schedules_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     6768 2023-04-18 06:32:00.689675 windmill_api-1.88.1/windmill_api/models/list_scripts_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-04-18 06:32:00.561674 windmill_api-1.88.1/windmill_api/models/list_scripts_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-18 06:31:43.753490 windmill_api-1.88.1/windmill_api/models/list_scripts_response_200_item_kind.py
--rw-r--r--   0        0        0      213 2023-04-18 06:31:43.169484 windmill_api-1.88.1/windmill_api/models/list_scripts_response_200_item_language.py
--rw-r--r--   0        0        0     1265 2023-04-18 06:32:00.585674 windmill_api-1.88.1/windmill_api/models/list_scripts_response_200_item_schema.py
--rw-r--r--   0        0        0     2985 2023-04-18 06:32:00.625675 windmill_api-1.88.1/windmill_api/models/list_tokens_response_200_item.py
--rw-r--r--   0        0        0     2250 2023-04-18 06:32:00.653675 windmill_api-1.88.1/windmill_api/models/list_user_workspaces_response_200.py
--rw-r--r--   0        0        0     1833 2023-04-18 06:32:00.757676 windmill_api-1.88.1/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
--rw-r--r--   0        0        0     2896 2023-04-18 06:32:00.729676 windmill_api-1.88.1/windmill_api/models/list_users_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0      198 2023-04-18 06:31:43.477487 windmill_api-1.88.1/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
--rw-r--r--   0        0        0     4307 2023-04-18 06:32:00.789676 windmill_api-1.88.1/windmill_api/models/list_users_response_200_item.py
--rw-r--r--   0        0        0     1613 2023-04-18 06:32:00.785676 windmill_api-1.88.1/windmill_api/models/list_users_response_200_item_usage.py
--rw-r--r--   0        0        0     4608 2023-04-18 06:32:00.845677 windmill_api-1.88.1/windmill_api/models/list_variable_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-04-18 06:32:00.809677 windmill_api-1.88.1/windmill_api/models/list_variable_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2693 2023-04-18 06:32:00.845677 windmill_api-1.88.1/windmill_api/models/list_workers_response_200_item.py
--rw-r--r--   0        0        0     2086 2023-04-18 06:32:00.877677 windmill_api-1.88.1/windmill_api/models/list_workspace_invites_response_200_item.py
--rw-r--r--   0        0        0     2082 2023-04-18 06:32:00.877677 windmill_api-1.88.1/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0     2013 2023-04-18 06:32:00.905678 windmill_api-1.88.1/windmill_api/models/list_workspaces_response_200_item.py
--rw-r--r--   0        0        0     3388 2023-04-18 06:32:00.925678 windmill_api-1.88.1/windmill_api/models/listable_app.py
--rw-r--r--   0        0        0      207 2023-04-18 06:31:43.005482 windmill_api-1.88.1/windmill_api/models/listable_app_execution_mode.py
--rw-r--r--   0        0        0     1207 2023-04-18 06:32:00.929678 windmill_api-1.88.1/windmill_api/models/listable_app_extra_perms.py
--rw-r--r--   0        0        0     4751 2023-04-18 06:32:00.989678 windmill_api-1.88.1/windmill_api/models/listable_resource.py
--rw-r--r--   0        0        0     1232 2023-04-18 06:32:00.945678 windmill_api-1.88.1/windmill_api/models/listable_resource_extra_perms.py
--rw-r--r--   0        0        0     4486 2023-04-18 06:32:01.005679 windmill_api-1.88.1/windmill_api/models/listable_variable.py
--rw-r--r--   0        0        0     1232 2023-04-18 06:32:01.009679 windmill_api-1.88.1/windmill_api/models/listable_variable_extra_perms.py
--rw-r--r--   0        0        0     1513 2023-04-18 06:32:01.033679 windmill_api-1.88.1/windmill_api/models/login.py
--rw-r--r--   0        0        0     1559 2023-04-18 06:32:01.117680 windmill_api-1.88.1/windmill_api/models/login_json_body.py
--rw-r--r--   0        0        0     1739 2023-04-18 06:32:01.061679 windmill_api-1.88.1/windmill_api/models/login_with_oauth_json_body.py
--rw-r--r--   0        0        0     2758 2023-04-18 06:32:01.101680 windmill_api-1.88.1/windmill_api/models/main_arg_signature.py
--rw-r--r--   0        0        0     5099 2023-04-18 06:32:01.221681 windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item.py
--rw-r--r--   0        0        0      315 2023-04-18 06:31:43.981493 windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1547 2023-04-18 06:32:01.141680 windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1612 2023-04-18 06:32:01.169680 windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2044 2023-04-18 06:32:01.193681 windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3049 2023-04-18 06:32:01.233681 windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      333 2023-04-18 06:31:43.069483 windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1580 2023-04-18 06:32:01.245681 windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     2862 2023-04-18 06:32:01.269682 windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
--rw-r--r--   0        0        0      324 2023-04-18 06:31:43.889492 windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1529 2023-04-18 06:32:01.269682 windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      169 2023-04-18 06:31:44.017493 windmill_api-1.88.1/windmill_api/models/main_arg_signature_type.py
--rw-r--r--   0        0        0     2662 2023-04-18 06:32:01.309682 windmill_api-1.88.1/windmill_api/models/new_schedule.py
--rw-r--r--   0        0        0     1171 2023-04-18 06:32:01.289682 windmill_api-1.88.1/windmill_api/models/new_schedule_args.py
--rw-r--r--   0        0        0     2108 2023-04-18 06:32:01.325682 windmill_api-1.88.1/windmill_api/models/new_token.py
--rw-r--r--   0        0        0     2473 2023-04-18 06:32:01.345682 windmill_api-1.88.1/windmill_api/models/new_token_impersonate.py
--rw-r--r--   0        0        0     1710 2023-04-18 06:32:01.349682 windmill_api-1.88.1/windmill_api/models/new_user.py
--rw-r--r--   0        0        0     2584 2023-04-18 06:32:01.385683 windmill_api-1.88.1/windmill_api/models/open_flow.py
--rw-r--r--   0        0        0     1166 2023-04-18 06:32:01.369683 windmill_api-1.88.1/windmill_api/models/open_flow_schema.py
--rw-r--r--   0        0        0     3026 2023-04-18 06:32:01.413683 windmill_api-1.88.1/windmill_api/models/open_flow_value.py
--rw-r--r--   0        0        0     6384 2023-04-18 06:32:01.525684 windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module.py
--rw-r--r--   0        0        0     3013 2023-04-18 06:32:01.449684 windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1896 2023-04-18 06:32:01.477684 windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2200 2023-04-18 06:32:01.509684 windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2006 2023-04-18 06:32:01.541684 windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      175 2023-04-18 06:31:43.601489 windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1873 2023-04-18 06:32:01.553685 windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      175 2023-04-18 06:31:43.913492 windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1889 2023-04-18 06:32:01.565685 windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1940 2023-04-18 06:32:01.585685 windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6308 2023-04-18 06:32:01.645686 windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item.py
--rw-r--r--   0        0        0     2979 2023-04-18 06:32:01.621685 windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1886 2023-04-18 06:32:01.653686 windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2190 2023-04-18 06:32:01.673686 windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1986 2023-04-18 06:32:01.681686 windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      173 2023-04-18 06:31:43.357486 windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1853 2023-04-18 06:32:01.701686 windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      173 2023-04-18 06:31:44.049493 windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1879 2023-04-18 06:32:01.709686 windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1930 2023-04-18 06:32:01.729687 windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-04-18 06:32:01.753687 windmill_api-1.88.1/windmill_api/models/open_flow_w_path.py
--rw-r--r--   0        0        0     1197 2023-04-18 06:32:01.817688 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_schema.py
--rw-r--r--   0        0        0     3116 2023-04-18 06:32:01.793687 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value.py
--rw-r--r--   0        0        0     6590 2023-04-18 06:32:01.877688 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module.py
--rw-r--r--   0        0        0     3117 2023-04-18 06:32:01.857688 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
--rw-r--r--   0        0        0     1927 2023-04-18 06:32:01.885688 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2231 2023-04-18 06:32:01.997690 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2073 2023-04-18 06:32:01.913689 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      180 2023-04-18 06:31:43.645489 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1940 2023-04-18 06:32:01.941689 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      180 2023-04-18 06:31:43.249485 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1920 2023-04-18 06:32:01.973689 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1971 2023-04-18 06:32:01.997690 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6514 2023-04-18 06:32:02.081690 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item.py
--rw-r--r--   0        0        0     3074 2023-04-18 06:32:02.041690 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
--rw-r--r--   0        0        0     1917 2023-04-18 06:32:02.069690 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2221 2023-04-18 06:32:02.101691 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2044 2023-04-18 06:32:02.109691 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-18 06:31:43.917492 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1911 2023-04-18 06:32:02.129691 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-18 06:31:43.049483 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1910 2023-04-18 06:32:02.137691 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1961 2023-04-18 06:32:02.161691 windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1989 2023-04-18 06:32:02.165691 windmill_api-1.88.1/windmill_api/models/path_flow.py
--rw-r--r--   0        0        0     3089 2023-04-18 06:32:02.197692 windmill_api-1.88.1/windmill_api/models/path_flow_input_transforms.py
--rw-r--r--   0        0        0     2115 2023-04-18 06:32:02.193692 windmill_api-1.88.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      185 2023-04-18 06:31:43.697490 windmill_api-1.88.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1982 2023-04-18 06:32:02.225692 windmill_api-1.88.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      185 2023-04-18 06:31:43.633489 windmill_api-1.88.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      135 2023-04-18 06:31:43.325486 windmill_api-1.88.1/windmill_api/models/path_flow_type.py
--rw-r--r--   0        0        0     2292 2023-04-18 06:32:02.233692 windmill_api-1.88.1/windmill_api/models/path_script.py
--rw-r--r--   0        0        0     3181 2023-04-18 06:32:02.261692 windmill_api-1.88.1/windmill_api/models/path_script_input_transforms.py
--rw-r--r--   0        0        0     2135 2023-04-18 06:32:02.265692 windmill_api-1.88.1/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      187 2023-04-18 06:31:43.297485 windmill_api-1.88.1/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2002 2023-04-18 06:32:02.289693 windmill_api-1.88.1/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      187 2023-04-18 06:31:43.141484 windmill_api-1.88.1/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      141 2023-04-18 06:31:43.369486 windmill_api-1.88.1/windmill_api/models/path_script_type.py
--rw-r--r--   0        0        0     3390 2023-04-18 06:32:02.401694 windmill_api-1.88.1/windmill_api/models/policy.py
--rw-r--r--   0        0        0      202 2023-04-18 06:31:43.421487 windmill_api-1.88.1/windmill_api/models/policy_execution_mode.py
--rw-r--r--   0        0        0     1709 2023-04-18 06:32:02.313693 windmill_api-1.88.1/windmill_api/models/policy_triggerables.py
--rw-r--r--   0        0        0     1279 2023-04-18 06:32:02.337693 windmill_api-1.88.1/windmill_api/models/policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2147 2023-04-18 06:32:02.465695 windmill_api-1.88.1/windmill_api/models/preview.py
--rw-r--r--   0        0        0     1148 2023-04-18 06:32:02.425694 windmill_api-1.88.1/windmill_api/models/preview_args.py
--rw-r--r--   0        0        0      194 2023-04-18 06:31:43.233485 windmill_api-1.88.1/windmill_api/models/preview_language.py
--rw-r--r--   0        0        0     1642 2023-04-18 06:32:02.453694 windmill_api-1.88.1/windmill_api/models/preview_schedule_json_body.py
--rw-r--r--   0        0        0     2963 2023-04-18 06:32:02.489695 windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5679 2023-04-18 06:32:02.529695 windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      328 2023-04-18 06:31:43.925492 windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1618 2023-04-18 06:32:02.517695 windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1683 2023-04-18 06:32:02.541695 windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2191 2023-04-18 06:32:02.553696 windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3329 2023-04-18 06:32:02.585696 windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      346 2023-04-18 06:31:43.285485 windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1651 2023-04-18 06:32:02.577696 windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3214 2023-04-18 06:32:02.613696 windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      337 2023-04-18 06:31:43.001482 windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1600 2023-04-18 06:32:02.609696 windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      182 2023-04-18 06:31:43.853491 windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0    11448 2023-04-18 06:32:02.829698 windmill_api-1.88.1/windmill_api/models/queued_job.py
--rw-r--r--   0        0        0     1161 2023-04-18 06:32:02.633696 windmill_api-1.88.1/windmill_api/models/queued_job_args.py
--rw-r--r--   0        0        0     3202 2023-04-18 06:32:02.677697 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status.py
--rw-r--r--   0        0        0     6683 2023-04-18 06:32:02.757698 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1774 2023-04-18 06:32:02.865699 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2106 2023-04-18 06:32:02.857699 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      199 2023-04-18 06:31:43.417487 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1679 2023-04-18 06:32:02.885699 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2215 2023-04-18 06:32:02.901699 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      357 2023-04-18 06:31:43.393486 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6294 2023-04-18 06:32:02.969700 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1764 2023-04-18 06:32:02.925700 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2086 2023-04-18 06:32:02.953700 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      197 2023-04-18 06:31:43.493487 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1669 2023-04-18 06:32:02.981700 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2205 2023-04-18 06:32:03.001700 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      355 2023-04-18 06:31:43.429487 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2025 2023-04-18 06:32:03.013701 windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_retry.py
--rw-r--r--   0        0        0      307 2023-04-18 06:31:42.997482 windmill_api-1.88.1/windmill_api/models/queued_job_job_kind.py
--rw-r--r--   0        0        0      196 2023-04-18 06:31:43.909492 windmill_api-1.88.1/windmill_api/models/queued_job_language.py
--rw-r--r--   0        0        0     3079 2023-04-18 06:32:03.045701 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow.py
--rw-r--r--   0        0        0     6506 2023-04-18 06:32:03.097701 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3069 2023-04-18 06:32:03.081701 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1914 2023-04-18 06:32:03.113702 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2218 2023-04-18 06:32:03.129702 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2040 2023-04-18 06:32:03.141702 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-18 06:31:43.549488 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1907 2023-04-18 06:32:03.157702 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-18 06:31:43.569488 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1907 2023-04-18 06:32:03.245703 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1958 2023-04-18 06:32:03.185702 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6430 2023-04-18 06:32:03.349704 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3035 2023-04-18 06:32:03.285704 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1904 2023-04-18 06:32:03.313704 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2208 2023-04-18 06:32:03.345704 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2020 2023-04-18 06:32:03.373704 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-04-18 06:31:43.501488 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1887 2023-04-18 06:32:03.377704 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-04-18 06:31:43.109483 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1897 2023-04-18 06:32:03.401705 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1948 2023-04-18 06:32:03.405705 windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-04-18 06:32:03.441705 windmill_api-1.88.1/windmill_api/models/raw_script.py
--rw-r--r--   0        0        0     3139 2023-04-18 06:32:03.441705 windmill_api-1.88.1/windmill_api/models/raw_script_input_transforms.py
--rw-r--r--   0        0        0     2125 2023-04-18 06:32:03.469705 windmill_api-1.88.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      186 2023-04-18 06:31:43.077483 windmill_api-1.88.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1992 2023-04-18 06:32:03.473705 windmill_api-1.88.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      186 2023-04-18 06:31:44.053494 windmill_api-1.88.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      196 2023-04-18 06:31:43.201484 windmill_api-1.88.1/windmill_api/models/raw_script_language.py
--rw-r--r--   0        0        0      146 2023-04-18 06:31:43.837491 windmill_api-1.88.1/windmill_api/models/raw_script_type.py
--rw-r--r--   0        0        0     1405 2023-04-18 06:32:03.497706 windmill_api-1.88.1/windmill_api/models/refresh_token_json_body.py
--rw-r--r--   0        0        0     1448 2023-04-18 06:32:03.497706 windmill_api-1.88.1/windmill_api/models/remove_granular_acls_json_body.py
--rw-r--r--   0        0        0      304 2023-04-18 06:31:44.009493 windmill_api-1.88.1/windmill_api/models/remove_granular_acls_kind.py
--rw-r--r--   0        0        0     1544 2023-04-18 06:32:03.521706 windmill_api-1.88.1/windmill_api/models/remove_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1567 2023-04-18 06:32:03.525706 windmill_api-1.88.1/windmill_api/models/remove_user_to_group_json_body.py
--rw-r--r--   0        0        0     3367 2023-04-18 06:32:03.569707 windmill_api-1.88.1/windmill_api/models/resource.py
--rw-r--r--   0        0        0     1189 2023-04-18 06:32:03.541706 windmill_api-1.88.1/windmill_api/models/resource_extra_perms.py
--rw-r--r--   0        0        0     2256 2023-04-18 06:32:03.577707 windmill_api-1.88.1/windmill_api/models/resource_type.py
--rw-r--r--   0        0        0     1278 2023-04-18 06:32:03.589707 windmill_api-1.88.1/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
--rw-r--r--   0        0        0     1255 2023-04-18 06:32:03.597707 windmill_api-1.88.1/windmill_api/models/resume_suspended_job_post_json_body.py
--rw-r--r--   0        0        0     2546 2023-04-18 06:32:03.629707 windmill_api-1.88.1/windmill_api/models/retry.py
--rw-r--r--   0        0        0     1751 2023-04-18 06:32:03.625707 windmill_api-1.88.1/windmill_api/models/retry_constant.py
--rw-r--r--   0        0        0     2055 2023-04-18 06:32:03.657708 windmill_api-1.88.1/windmill_api/models/retry_exponential.py
--rw-r--r--   0        0        0     1210 2023-04-18 06:32:03.649707 windmill_api-1.88.1/windmill_api/models/run_flow_by_path_json_body.py
--rw-r--r--   0        0        0     2189 2023-04-18 06:32:03.677708 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body.py
--rw-r--r--   0        0        0     1235 2023-04-18 06:32:03.677708 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_args.py
--rw-r--r--   0        0        0     3265 2023-04-18 06:32:03.721708 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value.py
--rw-r--r--   0        0        0     7049 2023-04-18 06:32:03.865710 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3284 2023-04-18 06:32:03.757709 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1975 2023-04-18 06:32:03.785709 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-04-18 06:32:03.901710 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-04-18 06:32:03.893710 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-18 06:31:43.793491 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-04-18 06:32:03.921710 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-18 06:31:43.505488 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-04-18 06:32:03.929710 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-04-18 06:32:03.953711 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6939 2023-04-18 06:32:04.009711 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3250 2023-04-18 06:32:03.993711 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1965 2023-04-18 06:32:04.021711 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2269 2023-04-18 06:32:04.041712 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2147 2023-04-18 06:32:04.053712 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      187 2023-04-18 06:31:43.149484 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2014 2023-04-18 06:32:04.069712 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      187 2023-04-18 06:31:43.909492 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1958 2023-04-18 06:32:04.081712 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2009 2023-04-18 06:32:04.097712 windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1220 2023-04-18 06:32:04.101712 windmill_api-1.88.1/windmill_api/models/run_script_by_hash_json_body.py
--rw-r--r--   0        0        0     1220 2023-04-18 06:32:04.117712 windmill_api-1.88.1/windmill_api/models/run_script_by_path_json_body.py
--rw-r--r--   0        0        0     2422 2023-04-18 06:32:04.137713 windmill_api-1.88.1/windmill_api/models/run_script_preview_json_body.py
--rw-r--r--   0        0        0     1245 2023-04-18 06:32:04.137713 windmill_api-1.88.1/windmill_api/models/run_script_preview_json_body_args.py
--rw-r--r--   0        0        0      211 2023-04-18 06:31:43.373486 windmill_api-1.88.1/windmill_api/models/run_script_preview_json_body_language.py
--rw-r--r--   0        0        0     1266 2023-04-18 06:32:04.157713 windmill_api-1.88.1/windmill_api/models/run_wait_result_flow_by_path_json_body.py
--rw-r--r--   0        0        0     1276 2023-04-18 06:32:04.153713 windmill_api-1.88.1/windmill_api/models/run_wait_result_script_by_path_json_body.py
--rw-r--r--   0        0        0      203 2023-04-18 06:31:43.197484 windmill_api-1.88.1/windmill_api/models/runnable_type.py
--rw-r--r--   0        0        0     4086 2023-04-18 06:32:04.213714 windmill_api-1.88.1/windmill_api/models/schedule.py
--rw-r--r--   0        0        0     1153 2023-04-18 06:32:04.177713 windmill_api-1.88.1/windmill_api/models/schedule_args.py
--rw-r--r--   0        0        0     1189 2023-04-18 06:32:04.197713 windmill_api-1.88.1/windmill_api/models/schedule_extra_perms.py
--rw-r--r--   0        0        0     6220 2023-04-18 06:32:04.277714 windmill_api-1.88.1/windmill_api/models/script.py
--rw-r--r--   0        0        0     1143 2023-04-18 06:32:04.233714 windmill_api-1.88.1/windmill_api/models/script_args.py
--rw-r--r--   0        0        0     1179 2023-04-18 06:32:04.249714 windmill_api-1.88.1/windmill_api/models/script_extra_perms.py
--rw-r--r--   0        0        0      235 2023-04-18 06:31:43.145484 windmill_api-1.88.1/windmill_api/models/script_kind.py
--rw-r--r--   0        0        0      193 2023-04-18 06:31:43.465487 windmill_api-1.88.1/windmill_api/models/script_language.py
--rw-r--r--   0        0        0     1153 2023-04-18 06:32:04.273714 windmill_api-1.88.1/windmill_api/models/script_schema.py
--rw-r--r--   0        0        0     1440 2023-04-18 06:32:04.293714 windmill_api-1.88.1/windmill_api/models/set_password_json_body.py
--rw-r--r--   0        0        0     1470 2023-04-18 06:32:04.301715 windmill_api-1.88.1/windmill_api/models/set_schedule_enabled_json_body.py
--rw-r--r--   0        0        0     2032 2023-04-18 06:32:04.325715 windmill_api-1.88.1/windmill_api/models/slack_token.py
--rw-r--r--   0        0        0     1586 2023-04-18 06:32:04.325715 windmill_api-1.88.1/windmill_api/models/slack_token_bot.py
--rw-r--r--   0        0        0     2227 2023-04-18 06:32:04.357715 windmill_api-1.88.1/windmill_api/models/star_json_body.py
--rw-r--r--   0        0        0      185 2023-04-18 06:31:43.633489 windmill_api-1.88.1/windmill_api/models/star_json_body_favorite_kind.py
--rw-r--r--   0        0        0     1772 2023-04-18 06:32:04.357715 windmill_api-1.88.1/windmill_api/models/static_transform.py
--rw-r--r--   0        0        0      154 2023-04-18 06:31:43.017482 windmill_api-1.88.1/windmill_api/models/static_transform_type.py
--rw-r--r--   0        0        0     2462 2023-04-18 06:32:04.393715 windmill_api-1.88.1/windmill_api/models/token_response.py
--rw-r--r--   0        0        0     2921 2023-04-18 06:32:04.481716 windmill_api-1.88.1/windmill_api/models/truncated_token.py
--rw-r--r--   0        0        0     2249 2023-04-18 06:32:04.425716 windmill_api-1.88.1/windmill_api/models/unstar_json_body.py
--rw-r--r--   0        0        0      187 2023-04-18 06:31:43.333486 windmill_api-1.88.1/windmill_api/models/unstar_json_body_favorite_kind.py
--rw-r--r--   0        0        0     2638 2023-04-18 06:32:04.469716 windmill_api-1.88.1/windmill_api/models/update_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-04-18 06:32:04.517717 windmill_api-1.88.1/windmill_api/models/update_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-04-18 06:31:43.401486 windmill_api-1.88.1/windmill_api/models/update_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-04-18 06:32:04.509717 windmill_api-1.88.1/windmill_api/models/update_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-04-18 06:32:04.529717 windmill_api-1.88.1/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-04-18 06:32:04.665718 windmill_api-1.88.1/windmill_api/models/update_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-04-18 06:32:04.549717 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-04-18 06:32:04.589717 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-04-18 06:32:04.669718 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-04-18 06:32:04.705719 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-04-18 06:32:04.697719 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-04-18 06:32:04.729719 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-04-18 06:32:04.733719 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-04-18 06:31:44.057494 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-04-18 06:32:04.757719 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-04-18 06:31:43.665489 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-04-18 06:32:04.761720 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-04-18 06:32:04.785720 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-04-18 06:32:04.841720 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-04-18 06:32:04.905721 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-04-18 06:32:04.869721 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-04-18 06:32:04.901721 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-04-18 06:32:04.929721 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-04-18 06:31:43.477487 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-04-18 06:32:04.933721 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-04-18 06:31:43.053483 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-04-18 06:32:04.957722 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-04-18 06:32:04.961722 windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1949 2023-04-18 06:32:04.989722 windmill_api-1.88.1/windmill_api/models/update_folder_json_body.py
--rw-r--r--   0        0        0     1520 2023-04-18 06:32:04.985722 windmill_api-1.88.1/windmill_api/models/update_group_json_body.py
--rw-r--r--   0        0        0     1670 2023-04-18 06:32:05.013722 windmill_api-1.88.1/windmill_api/models/update_input.py
--rw-r--r--   0        0        0     1716 2023-04-18 06:32:05.017722 windmill_api-1.88.1/windmill_api/models/update_input_json_body.py
--rw-r--r--   0        0        0     2036 2023-04-18 06:32:05.045723 windmill_api-1.88.1/windmill_api/models/update_resource_json_body.py
--rw-r--r--   0        0        0     1847 2023-04-18 06:32:05.045723 windmill_api-1.88.1/windmill_api/models/update_resource_type_json_body.py
--rw-r--r--   0        0        0     1541 2023-04-18 06:32:05.069723 windmill_api-1.88.1/windmill_api/models/update_resource_value_json_body.py
--rw-r--r--   0        0        0     1953 2023-04-18 06:32:05.077723 windmill_api-1.88.1/windmill_api/models/update_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-04-18 06:32:05.089723 windmill_api-1.88.1/windmill_api/models/update_schedule_json_body_args.py
--rw-r--r--   0        0        0     2066 2023-04-18 06:32:05.109723 windmill_api-1.88.1/windmill_api/models/update_user_json_body.py
--rw-r--r--   0        0        0     2316 2023-04-18 06:32:05.125723 windmill_api-1.88.1/windmill_api/models/update_variable_json_body.py
--rw-r--r--   0        0        0     1478 2023-04-18 06:32:05.133724 windmill_api-1.88.1/windmill_api/models/usage.py
--rw-r--r--   0        0        0     4071 2023-04-18 06:32:05.185724 windmill_api-1.88.1/windmill_api/models/user.py
--rw-r--r--   0        0        0     1501 2023-04-18 06:32:05.157724 windmill_api-1.88.1/windmill_api/models/user_usage.py
--rw-r--r--   0        0        0     2122 2023-04-18 06:32:05.189724 windmill_api-1.88.1/windmill_api/models/user_workspace_list.py
--rw-r--r--   0        0        0     1767 2023-04-18 06:32:05.329726 windmill_api-1.88.1/windmill_api/models/user_workspace_list_workspaces_item.py
--rw-r--r--   0        0        0     4222 2023-04-18 06:32:05.249725 windmill_api-1.88.1/windmill_api/models/whoami_response_200.py
--rw-r--r--   0        0        0     1572 2023-04-18 06:32:05.273725 windmill_api-1.88.1/windmill_api/models/whoami_response_200_usage.py
--rw-r--r--   0        0        0     4211 2023-04-18 06:32:05.333726 windmill_api-1.88.1/windmill_api/models/whois_response_200.py
--rw-r--r--   0        0        0     1567 2023-04-18 06:32:05.353726 windmill_api-1.88.1/windmill_api/models/whois_response_200_usage.py
--rw-r--r--   0        0        0     2604 2023-04-18 06:32:05.369726 windmill_api-1.88.1/windmill_api/models/worker_ping.py
--rw-r--r--   0        0        0     1901 2023-04-18 06:32:05.385726 windmill_api-1.88.1/windmill_api/models/workspace.py
--rw-r--r--   0        0        0     1974 2023-04-18 06:32:05.485727 windmill_api-1.88.1/windmill_api/models/workspace_invite.py
--rw-r--r--   0        0        0       25 2023-04-18 06:31:33.841384 windmill_api-1.88.1/windmill_api/py.typed
--rw-r--r--   0        0        0      939 2023-04-18 06:32:05.401726 windmill_api-1.88.1/windmill_api/types.py
--rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 windmill_api-1.88.1/setup.py
--rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.88.1/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-04-23 15:07:47.008977 windmill_api-1.89.0/LICENSE
+-rw-r--r--   0        0        0     2952 2023-04-23 15:07:47.016977 windmill_api-1.89.0/README.md
+-rw-r--r--   0        0        0      717 2023-04-23 15:07:47.012977 windmill_api-1.89.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-04-23 15:07:04.900570 windmill_api-1.89.0/windmill_api/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-23 15:07:05.624578 windmill_api-1.89.0/windmill_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.772579 windmill_api-1.89.0/windmill_api/api/app/__init__.py
+-rw-r--r--   0        0        0     1999 2023-04-23 15:07:18.920700 windmill_api-1.89.0/windmill_api/api/app/create_app.py
+-rw-r--r--   0        0        0     1769 2023-04-23 15:07:18.944700 windmill_api-1.89.0/windmill_api/api/app/delete_app.py
+-rw-r--r--   0        0        0     2214 2023-04-23 15:07:18.960700 windmill_api-1.89.0/windmill_api/api/app/execute_component.py
+-rw-r--r--   0        0        0     2782 2023-04-23 15:07:19.024701 windmill_api-1.89.0/windmill_api/api/app/exists_app.py
+-rw-r--r--   0        0        0     3020 2023-04-23 15:07:19.012701 windmill_api-1.89.0/windmill_api/api/app/get_app_by_path.py
+-rw-r--r--   0        0        0     3031 2023-04-23 15:07:19.064701 windmill_api-1.89.0/windmill_api/api/app/get_app_by_version.py
+-rw-r--r--   0        0        0     2649 2023-04-23 15:07:19.088701 windmill_api-1.89.0/windmill_api/api/app/get_hub_app_by_id.py
+-rw-r--r--   0        0        0     3168 2023-04-23 15:07:19.132702 windmill_api-1.89.0/windmill_api/api/app/get_public_app_by_secret.py
+-rw-r--r--   0        0        0     1797 2023-04-23 15:07:19.128702 windmill_api-1.89.0/windmill_api/api/app/get_public_secret_of_app.py
+-rw-r--r--   0        0        0     7289 2023-04-23 15:07:19.276703 windmill_api-1.89.0/windmill_api/api/app/list_apps.py
+-rw-r--r--   0        0        0     2405 2023-04-23 15:07:19.180702 windmill_api-1.89.0/windmill_api/api/app/list_hub_apps.py
+-rw-r--r--   0        0        0     2140 2023-04-23 15:07:19.220703 windmill_api-1.89.0/windmill_api/api/app/update_app.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.672578 windmill_api-1.89.0/windmill_api/api/audit/__init__.py
+-rw-r--r--   0        0        0     3065 2023-04-23 15:07:19.272703 windmill_api-1.89.0/windmill_api/api/audit/get_audit_log.py
+-rw-r--r--   0        0        0     8723 2023-04-23 15:07:19.416705 windmill_api-1.89.0/windmill_api/api/audit/list_audit_logs.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.848580 windmill_api-1.89.0/windmill_api/api/capture/__init__.py
+-rw-r--r--   0        0        0     1796 2023-04-23 15:07:19.324704 windmill_api-1.89.0/windmill_api/api/capture/create_capture.py
+-rw-r--r--   0        0        0     1790 2023-04-23 15:07:19.364704 windmill_api-1.89.0/windmill_api/api/capture/get_capture.py
+-rw-r--r--   0        0        0     1799 2023-04-23 15:07:19.404705 windmill_api-1.89.0/windmill_api/api/capture/update_capture.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.848580 windmill_api-1.89.0/windmill_api/api/favorite/__init__.py
+-rw-r--r--   0        0        0     1964 2023-04-23 15:07:19.452705 windmill_api-1.89.0/windmill_api/api/favorite/star.py
+-rw-r--r--   0        0        0     1984 2023-04-23 15:07:19.452705 windmill_api-1.89.0/windmill_api/api/favorite/unstar.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.760579 windmill_api-1.89.0/windmill_api/api/flow/__init__.py
+-rw-r--r--   0        0        0     2220 2023-04-23 15:07:19.500706 windmill_api-1.89.0/windmill_api/api/flow/archive_flow_by_path.py
+-rw-r--r--   0        0        0     2009 2023-04-23 15:07:19.492706 windmill_api-1.89.0/windmill_api/api/flow/create_flow.py
+-rw-r--r--   0        0        0     1788 2023-04-23 15:07:19.524706 windmill_api-1.89.0/windmill_api/api/flow/delete_flow_by_path.py
+-rw-r--r--   0        0        0     2755 2023-04-23 15:07:19.560706 windmill_api-1.89.0/windmill_api/api/flow/exists_flow_by_path.py
+-rw-r--r--   0        0        0     3036 2023-04-23 15:07:19.596707 windmill_api-1.89.0/windmill_api/api/flow/get_flow_by_path.py
+-rw-r--r--   0        0        0     4827 2023-04-23 15:07:19.652707 windmill_api-1.89.0/windmill_api/api/flow/get_flow_input_history_by_path.py
+-rw-r--r--   0        0        0     2667 2023-04-23 15:07:19.644707 windmill_api-1.89.0/windmill_api/api/flow/get_hub_flow_by_id.py
+-rw-r--r--   0        0        0     1668 2023-04-23 15:07:19.680708 windmill_api-1.89.0/windmill_api/api/flow/list_flow_paths.py
+-rw-r--r--   0        0        0     7969 2023-04-23 15:07:19.800709 windmill_api-1.89.0/windmill_api/api/flow/list_flows.py
+-rw-r--r--   0        0        0     2423 2023-04-23 15:07:19.728708 windmill_api-1.89.0/windmill_api/api/flow/list_hub_flows.py
+-rw-r--r--   0        0        0     2150 2023-04-23 15:07:19.768709 windmill_api-1.89.0/windmill_api/api/flow/update_flow.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.832580 windmill_api-1.89.0/windmill_api/api/folder/__init__.py
+-rw-r--r--   0        0        0     2214 2023-04-23 15:07:19.808709 windmill_api-1.89.0/windmill_api/api/folder/add_owner_to_folder.py
+-rw-r--r--   0        0        0     2029 2023-04-23 15:07:19.840709 windmill_api-1.89.0/windmill_api/api/folder/create_folder.py
+-rw-r--r--   0        0        0     1778 2023-04-23 15:07:19.844709 windmill_api-1.89.0/windmill_api/api/folder/delete_folder.py
+-rw-r--r--   0        0        0     2960 2023-04-23 15:07:19.896710 windmill_api-1.89.0/windmill_api/api/folder/get_folder.py
+-rw-r--r--   0        0        0     3055 2023-04-23 15:07:19.900710 windmill_api-1.89.0/windmill_api/api/folder/get_folder_usage.py
+-rw-r--r--   0        0        0     3405 2023-04-23 15:07:19.972711 windmill_api-1.89.0/windmill_api/api/folder/list_folder_names.py
+-rw-r--r--   0        0        0     4251 2023-04-23 15:07:19.972711 windmill_api-1.89.0/windmill_api/api/folder/list_folders.py
+-rw-r--r--   0        0        0     2244 2023-04-23 15:07:20.016711 windmill_api-1.89.0/windmill_api/api/folder/remove_owner_to_folder.py
+-rw-r--r--   0        0        0     2170 2023-04-23 15:07:20.032711 windmill_api-1.89.0/windmill_api/api/folder/update_folder.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.844580 windmill_api-1.89.0/windmill_api/api/granular_acl/__init__.py
+-rw-r--r--   0        0        0     2480 2023-04-23 15:07:20.064712 windmill_api-1.89.0/windmill_api/api/granular_acl/add_granular_acls.py
+-rw-r--r--   0        0        0     3526 2023-04-23 15:07:20.092712 windmill_api-1.89.0/windmill_api/api/granular_acl/get_granular_acls.py
+-rw-r--r--   0        0        0     2545 2023-04-23 15:07:20.104712 windmill_api-1.89.0/windmill_api/api/granular_acl/remove_granular_acls.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.828580 windmill_api-1.89.0/windmill_api/api/group/__init__.py
+-rw-r--r--   0        0        0     2194 2023-04-23 15:07:20.152713 windmill_api-1.89.0/windmill_api/api/group/add_user_to_group.py
+-rw-r--r--   0        0        0     2019 2023-04-23 15:07:20.140712 windmill_api-1.89.0/windmill_api/api/group/create_group.py
+-rw-r--r--   0        0        0     1775 2023-04-23 15:07:20.196713 windmill_api-1.89.0/windmill_api/api/group/delete_group.py
+-rw-r--r--   0        0        0     2942 2023-04-23 15:07:20.208713 windmill_api-1.89.0/windmill_api/api/group/get_group.py
+-rw-r--r--   0        0        0     3400 2023-04-23 15:07:20.264714 windmill_api-1.89.0/windmill_api/api/group/list_group_names.py
+-rw-r--r--   0        0        0     4233 2023-04-23 15:07:20.324714 windmill_api-1.89.0/windmill_api/api/group/list_groups.py
+-rw-r--r--   0        0        0     2224 2023-04-23 15:07:20.300714 windmill_api-1.89.0/windmill_api/api/group/remove_user_to_group.py
+-rw-r--r--   0        0        0     2160 2023-04-23 15:07:20.344714 windmill_api-1.89.0/windmill_api/api/group/update_group.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.848580 windmill_api-1.89.0/windmill_api/api/input_/__init__.py
+-rw-r--r--   0        0        0     3338 2023-04-23 15:07:20.384715 windmill_api-1.89.0/windmill_api/api/input_/create_input.py
+-rw-r--r--   0        0        0     1811 2023-04-23 15:07:20.380715 windmill_api-1.89.0/windmill_api/api/input_/delete_input.py
+-rw-r--r--   0        0        0     6187 2023-04-23 15:07:20.488716 windmill_api-1.89.0/windmill_api/api/input_/get_input_history.py
+-rw-r--r--   0        0        0     6010 2023-04-23 15:07:20.480716 windmill_api-1.89.0/windmill_api/api/input_/list_inputs.py
+-rw-r--r--   0        0        0     2025 2023-04-23 15:07:20.536717 windmill_api-1.89.0/windmill_api/api/input_/update_input.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.784579 windmill_api-1.89.0/windmill_api/api/job/__init__.py
+-rw-r--r--   0        0        0     2181 2023-04-23 15:07:20.528716 windmill_api-1.89.0/windmill_api/api/job/cancel_queued_job.py
+-rw-r--r--   0        0        0     2687 2023-04-23 15:07:20.592717 windmill_api-1.89.0/windmill_api/api/job/cancel_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-04-23 15:07:20.600717 windmill_api-1.89.0/windmill_api/api/job/cancel_suspended_job_post.py
+-rw-r--r--   0        0        0     2535 2023-04-23 15:07:20.664718 windmill_api-1.89.0/windmill_api/api/job/create_job_signature.py
+-rw-r--r--   0        0        0     3217 2023-04-23 15:07:20.652718 windmill_api-1.89.0/windmill_api/api/job/delete_completed_job.py
+-rw-r--r--   0        0        0     2235 2023-04-23 15:07:20.692718 windmill_api-1.89.0/windmill_api/api/job/force_cancel_queued_job.py
+-rw-r--r--   0        0        0     3034 2023-04-23 15:07:20.716719 windmill_api-1.89.0/windmill_api/api/job/get_completed_job.py
+-rw-r--r--   0        0        0     1784 2023-04-23 15:07:20.728719 windmill_api-1.89.0/windmill_api/api/job/get_completed_job_result.py
+-rw-r--r--   0        0        0     2868 2023-04-23 15:07:20.772719 windmill_api-1.89.0/windmill_api/api/job/get_job.py
+-rw-r--r--   0        0        0     4305 2023-04-23 15:07:20.804719 windmill_api-1.89.0/windmill_api/api/job/get_job_updates.py
+-rw-r--r--   0        0        0     4306 2023-04-23 15:07:20.844720 windmill_api-1.89.0/windmill_api/api/job/get_resume_urls.py
+-rw-r--r--   0        0        0     4601 2023-04-23 15:07:20.876720 windmill_api-1.89.0/windmill_api/api/job/get_suspended_job_flow.py
+-rw-r--r--   0        0        0    12602 2023-04-23 15:07:21.028722 windmill_api-1.89.0/windmill_api/api/job/list_completed_jobs.py
+-rw-r--r--   0        0        0    11829 2023-04-23 15:07:21.076722 windmill_api-1.89.0/windmill_api/api/job/list_jobs.py
+-rw-r--r--   0        0        0    12367 2023-04-23 15:07:21.244724 windmill_api-1.89.0/windmill_api/api/job/list_queue.py
+-rw-r--r--   0        0        0     2067 2023-04-23 15:07:21.116723 windmill_api-1.89.0/windmill_api/api/job/result_by_id.py
+-rw-r--r--   0        0        0     2313 2023-04-23 15:07:21.160723 windmill_api-1.89.0/windmill_api/api/job/resume_suspended_flow_as_owner.py
+-rw-r--r--   0        0        0     2994 2023-04-23 15:07:21.220724 windmill_api-1.89.0/windmill_api/api/job/resume_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-04-23 15:07:21.280724 windmill_api-1.89.0/windmill_api/api/job/resume_suspended_job_post.py
+-rw-r--r--   0        0        0     4566 2023-04-23 15:07:21.320725 windmill_api-1.89.0/windmill_api/api/job/run_flow_by_path.py
+-rw-r--r--   0        0        0     3037 2023-04-23 15:07:21.336725 windmill_api-1.89.0/windmill_api/api/job/run_flow_preview.py
+-rw-r--r--   0        0        0     4594 2023-04-23 15:07:21.400726 windmill_api-1.89.0/windmill_api/api/job/run_script_by_hash.py
+-rw-r--r--   0        0        0     4200 2023-04-23 15:07:21.412726 windmill_api-1.89.0/windmill_api/api/job/run_script_by_path.py
+-rw-r--r--   0        0        0     3050 2023-04-23 15:07:21.456726 windmill_api-1.89.0/windmill_api/api/job/run_script_preview.py
+-rw-r--r--   0        0        0     3215 2023-04-23 15:07:21.488726 windmill_api-1.89.0/windmill_api/api/job/run_wait_result_flow_by_path.py
+-rw-r--r--   0        0        0     3521 2023-04-23 15:07:21.516727 windmill_api-1.89.0/windmill_api/api/job/run_wait_result_script_by_path.py
+-rw-r--r--   0        0        0     3356 2023-04-23 15:07:21.552727 windmill_api-1.89.0/windmill_api/api/job/run_wait_result_script_by_path_get.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.716579 windmill_api-1.89.0/windmill_api/api/oauth/__init__.py
+-rw-r--r--   0        0        0     3506 2023-04-23 15:07:21.576727 windmill_api-1.89.0/windmill_api/api/oauth/connect_callback.py
+-rw-r--r--   0        0        0     2118 2023-04-23 15:07:21.592728 windmill_api-1.89.0/windmill_api/api/oauth/connect_slack_callback.py
+-rw-r--r--   0        0        0     2056 2023-04-23 15:07:21.636728 windmill_api-1.89.0/windmill_api/api/oauth/create_account.py
+-rw-r--r--   0        0        0     1764 2023-04-23 15:07:21.628728 windmill_api-1.89.0/windmill_api/api/oauth/disconnect_account.py
+-rw-r--r--   0        0        0     1649 2023-04-23 15:07:21.664728 windmill_api-1.89.0/windmill_api/api/oauth/disconnect_slack.py
+-rw-r--r--   0        0        0     1426 2023-04-23 15:07:21.668728 windmill_api-1.89.0/windmill_api/api/oauth/list_o_auth_connects.py
+-rw-r--r--   0        0        0     2162 2023-04-23 15:07:21.716729 windmill_api-1.89.0/windmill_api/api/oauth/list_o_auth_logins.py
+-rw-r--r--   0        0        0     2151 2023-04-23 15:07:21.712729 windmill_api-1.89.0/windmill_api/api/oauth/refresh_token.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.724579 windmill_api-1.89.0/windmill_api/api/resource/__init__.py
+-rw-r--r--   0        0        0     2049 2023-04-23 15:07:21.752729 windmill_api-1.89.0/windmill_api/api/resource/create_resource.py
+-rw-r--r--   0        0        0     2093 2023-04-23 15:07:21.760729 windmill_api-1.89.0/windmill_api/api/resource/create_resource_type.py
+-rw-r--r--   0        0        0     1784 2023-04-23 15:07:21.788730 windmill_api-1.89.0/windmill_api/api/resource/delete_resource.py
+-rw-r--r--   0        0        0     1799 2023-04-23 15:07:21.800730 windmill_api-1.89.0/windmill_api/api/resource/delete_resource_type.py
+-rw-r--r--   0        0        0     2763 2023-04-23 15:07:21.840730 windmill_api-1.89.0/windmill_api/api/resource/exists_resource.py
+-rw-r--r--   0        0        0     2788 2023-04-23 15:07:21.860731 windmill_api-1.89.0/windmill_api/api/resource/exists_resource_type.py
+-rw-r--r--   0        0        0     2996 2023-04-23 15:07:21.896731 windmill_api-1.89.0/windmill_api/api/resource/get_resource.py
+-rw-r--r--   0        0        0     3074 2023-04-23 15:07:21.920731 windmill_api-1.89.0/windmill_api/api/resource/get_resource_type.py
+-rw-r--r--   0        0        0     1790 2023-04-23 15:07:21.932731 windmill_api-1.89.0/windmill_api/api/resource/get_resource_value.py
+-rw-r--r--   0        0        0     5732 2023-04-23 15:07:22.036732 windmill_api-1.89.0/windmill_api/api/resource/list_resource.py
+-rw-r--r--   0        0        0     3149 2023-04-23 15:07:21.984732 windmill_api-1.89.0/windmill_api/api/resource/list_resource_type.py
+-rw-r--r--   0        0        0     2600 2023-04-23 15:07:22.036732 windmill_api-1.89.0/windmill_api/api/resource/list_resource_type_names.py
+-rw-r--r--   0        0        0     2190 2023-04-23 15:07:22.088733 windmill_api-1.89.0/windmill_api/api/resource/update_resource.py
+-rw-r--r--   0        0        0     2234 2023-04-23 15:07:22.092733 windmill_api-1.89.0/windmill_api/api/resource/update_resource_type.py
+-rw-r--r--   0        0        0     2244 2023-04-23 15:07:22.132733 windmill_api-1.89.0/windmill_api/api/resource/update_resource_value.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.820580 windmill_api-1.89.0/windmill_api/api/schedule/__init__.py
+-rw-r--r--   0        0        0     2049 2023-04-23 15:07:22.128733 windmill_api-1.89.0/windmill_api/api/schedule/create_schedule.py
+-rw-r--r--   0        0        0     1784 2023-04-23 15:07:22.172734 windmill_api-1.89.0/windmill_api/api/schedule/delete_schedule.py
+-rw-r--r--   0        0        0     2763 2023-04-23 15:07:22.196734 windmill_api-1.89.0/windmill_api/api/schedule/exists_schedule.py
+-rw-r--r--   0        0        0     2996 2023-04-23 15:07:22.228734 windmill_api-1.89.0/windmill_api/api/schedule/get_schedule.py
+-rw-r--r--   0        0        0     4287 2023-04-23 15:07:22.276735 windmill_api-1.89.0/windmill_api/api/schedule/list_schedules.py
+-rw-r--r--   0        0        0     3217 2023-04-23 15:07:22.284735 windmill_api-1.89.0/windmill_api/api/schedule/preview_schedule.py
+-rw-r--r--   0        0        0     2233 2023-04-23 15:07:22.316735 windmill_api-1.89.0/windmill_api/api/schedule/set_schedule_enabled.py
+-rw-r--r--   0        0        0     2190 2023-04-23 15:07:22.324735 windmill_api-1.89.0/windmill_api/api/schedule/update_schedule.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.736579 windmill_api-1.89.0/windmill_api/api/script/__init__.py
+-rw-r--r--   0        0        0     3165 2023-04-23 15:07:22.376736 windmill_api-1.89.0/windmill_api/api/script/archive_script_by_hash.py
+-rw-r--r--   0        0        0     1797 2023-04-23 15:07:22.364736 windmill_api-1.89.0/windmill_api/api/script/archive_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-04-23 15:07:22.412736 windmill_api-1.89.0/windmill_api/api/script/bash_to_jsonschema.py
+-rw-r--r--   0        0        0     2029 2023-04-23 15:07:22.416736 windmill_api-1.89.0/windmill_api/api/script/create_script.py
+-rw-r--r--   0        0        0     3327 2023-04-23 15:07:22.468737 windmill_api-1.89.0/windmill_api/api/script/delete_script_by_hash.py
+-rw-r--r--   0        0        0     2873 2023-04-23 15:07:22.488737 windmill_api-1.89.0/windmill_api/api/script/delete_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-04-23 15:07:22.532738 windmill_api-1.89.0/windmill_api/api/script/deno_to_jsonschema.py
+-rw-r--r--   0        0        0     2767 2023-04-23 15:07:22.548738 windmill_api-1.89.0/windmill_api/api/script/exists_script_by_path.py
+-rw-r--r--   0        0        0     2802 2023-04-23 15:07:22.580738 windmill_api-1.89.0/windmill_api/api/script/get_hub_script_by_path.py
+-rw-r--r--   0        0        0     1607 2023-04-23 15:07:22.588738 windmill_api-1.89.0/windmill_api/api/script/get_hub_script_content_by_path.py
+-rw-r--r--   0        0        0     3092 2023-04-23 15:07:22.636739 windmill_api-1.89.0/windmill_api/api/script/get_script_by_hash.py
+-rw-r--r--   0        0        0     3074 2023-04-23 15:07:22.648739 windmill_api-1.89.0/windmill_api/api/script/get_script_by_path.py
+-rw-r--r--   0        0        0     3276 2023-04-23 15:07:22.688739 windmill_api-1.89.0/windmill_api/api/script/get_script_deployment_status.py
+-rw-r--r--   0        0        0     2967 2023-04-23 15:07:22.704739 windmill_api-1.89.0/windmill_api/api/script/go_to_jsonschema.py
+-rw-r--r--   0        0        0     2459 2023-04-23 15:07:22.732740 windmill_api-1.89.0/windmill_api/api/script/list_hub_scripts.py
+-rw-r--r--   0        0        0     1676 2023-04-23 15:07:22.744740 windmill_api-1.89.0/windmill_api/api/script/list_script_paths.py
+-rw-r--r--   0        0        0    11165 2023-04-23 15:07:22.900741 windmill_api-1.89.0/windmill_api/api/script/list_scripts.py
+-rw-r--r--   0        0        0     3039 2023-04-23 15:07:22.800740 windmill_api-1.89.0/windmill_api/api/script/python_to_jsonschema.py
+-rw-r--r--   0        0        0     1784 2023-04-23 15:07:22.840741 windmill_api-1.89.0/windmill_api/api/script/raw_script_by_hash.py
+-rw-r--r--   0        0        0     1784 2023-04-23 15:07:22.880741 windmill_api-1.89.0/windmill_api/api/script/raw_script_by_path.py
+-rw-r--r--   0        0        0     2119 2023-04-23 15:07:22.924741 windmill_api-1.89.0/windmill_api/api/script/raw_script_by_path_tokened.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.640578 windmill_api-1.89.0/windmill_api/api/settings/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-23 15:07:22.932741 windmill_api-1.89.0/windmill_api/api/settings/backend_version.py
+-rw-r--r--   0        0        0     1423 2023-04-23 15:07:22.972742 windmill_api-1.89.0/windmill_api/api/settings/get_open_api_yaml.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.676578 windmill_api-1.89.0/windmill_api/api/user/__init__.py
+-rw-r--r--   0        0        0     1857 2023-04-23 15:07:22.992742 windmill_api-1.89.0/windmill_api/api/user/accept_invite.py
+-rw-r--r--   0        0        0     1822 2023-04-23 15:07:23.012742 windmill_api-1.89.0/windmill_api/api/user/create_token.py
+-rw-r--r--   0        0        0     1991 2023-04-23 15:07:23.028742 windmill_api-1.89.0/windmill_api/api/user/create_token_impersonate.py
+-rw-r--r--   0        0        0     2058 2023-04-23 15:07:23.052743 windmill_api-1.89.0/windmill_api/api/user/create_user.py
+-rw-r--r--   0        0        0     1863 2023-04-23 15:07:23.068743 windmill_api-1.89.0/windmill_api/api/user/create_user_globally.py
+-rw-r--r--   0        0        0     1867 2023-04-23 15:07:23.088743 windmill_api-1.89.0/windmill_api/api/user/decline_invite.py
+-rw-r--r--   0        0        0     1674 2023-04-23 15:07:23.104743 windmill_api-1.89.0/windmill_api/api/user/delete_token.py
+-rw-r--r--   0        0        0     1872 2023-04-23 15:07:23.124743 windmill_api-1.89.0/windmill_api/api/user/delete_user.py
+-rw-r--r--   0        0        0     1454 2023-04-23 15:07:23.140744 windmill_api-1.89.0/windmill_api/api/user/get_current_email.py
+-rw-r--r--   0        0        0     1474 2023-04-23 15:07:23.156744 windmill_api-1.89.0/windmill_api/api/user/get_usage.py
+-rw-r--r--   0        0        0     1639 2023-04-23 15:07:23.176744 windmill_api-1.89.0/windmill_api/api/user/global_user_delete.py
+-rw-r--r--   0        0        0     2060 2023-04-23 15:07:23.192744 windmill_api-1.89.0/windmill_api/api/user/global_user_update.py
+-rw-r--r--   0        0        0     2468 2023-04-23 15:07:23.220744 windmill_api-1.89.0/windmill_api/api/user/global_whoami.py
+-rw-r--r--   0        0        0     2745 2023-04-23 15:07:23.244744 windmill_api-1.89.0/windmill_api/api/user/is_owner_of_path.py
+-rw-r--r--   0        0        0     1646 2023-04-23 15:07:23.256745 windmill_api-1.89.0/windmill_api/api/user/leave_workspace.py
+-rw-r--r--   0        0        0     2633 2023-04-23 15:07:23.296745 windmill_api-1.89.0/windmill_api/api/user/list_tokens.py
+-rw-r--r--   0        0        0     2552 2023-04-23 15:07:23.308745 windmill_api-1.89.0/windmill_api/api/user/list_usernames.py
+-rw-r--r--   0        0        0     3012 2023-04-23 15:07:23.348745 windmill_api-1.89.0/windmill_api/api/user/list_users.py
+-rw-r--r--   0        0        0     4222 2023-04-23 15:07:23.380746 windmill_api-1.89.0/windmill_api/api/user/list_users_as_super_admin.py
+-rw-r--r--   0        0        0     2829 2023-04-23 15:07:23.412746 windmill_api-1.89.0/windmill_api/api/user/list_workspace_invites.py
+-rw-r--r--   0        0        0     1784 2023-04-23 15:07:23.420746 windmill_api-1.89.0/windmill_api/api/user/login.py
+-rw-r--r--   0        0        0     2116 2023-04-23 15:07:23.452746 windmill_api-1.89.0/windmill_api/api/user/login_with_oauth.py
+-rw-r--r--   0        0        0     1393 2023-04-23 15:07:23.468747 windmill_api-1.89.0/windmill_api/api/user/logout.py
+-rw-r--r--   0        0        0     1820 2023-04-23 15:07:23.488747 windmill_api-1.89.0/windmill_api/api/user/set_password.py
+-rw-r--r--   0        0        0     2250 2023-04-23 15:07:23.508747 windmill_api-1.89.0/windmill_api/api/user/update_user.py
+-rw-r--r--   0        0        0     2652 2023-04-23 15:07:23.536747 windmill_api-1.89.0/windmill_api/api/user/whoami.py
+-rw-r--r--   0        0        0     2967 2023-04-23 15:07:23.564748 windmill_api-1.89.0/windmill_api/api/user/whois.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.712579 windmill_api-1.89.0/windmill_api/api/variable/__init__.py
+-rw-r--r--   0        0        0     2634 2023-04-23 15:07:23.584748 windmill_api-1.89.0/windmill_api/api/variable/create_variable.py
+-rw-r--r--   0        0        0     1784 2023-04-23 15:07:23.608748 windmill_api-1.89.0/windmill_api/api/variable/delete_variable.py
+-rw-r--r--   0        0        0     2795 2023-04-23 15:07:23.640748 windmill_api-1.89.0/windmill_api/api/variable/exists_variable.py
+-rw-r--r--   0        0        0     3840 2023-04-23 15:07:23.676749 windmill_api-1.89.0/windmill_api/api/variable/get_variable.py
+-rw-r--r--   0        0        0     3270 2023-04-23 15:07:23.692749 windmill_api-1.89.0/windmill_api/api/variable/list_contextual_variables.py
+-rw-r--r--   0        0        0     3071 2023-04-23 15:07:23.736749 windmill_api-1.89.0/windmill_api/api/variable/list_variable.py
+-rw-r--r--   0        0        0     2775 2023-04-23 15:07:23.740749 windmill_api-1.89.0/windmill_api/api/variable/update_variable.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.780579 windmill_api-1.89.0/windmill_api/api/worker/__init__.py
+-rw-r--r--   0        0        0     2448 2023-04-23 15:07:23.784750 windmill_api-1.89.0/windmill_api/api/worker/get_custom_tags.py
+-rw-r--r--   0        0        0     3896 2023-04-23 15:07:23.812750 windmill_api-1.89.0/windmill_api/api/worker/list_workers.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:07:05.696578 windmill_api-1.89.0/windmill_api/api/workspace/__init__.py
+-rw-r--r--   0        0        0     2015 2023-04-23 15:07:23.828750 windmill_api-1.89.0/windmill_api/api/workspace/add_user.py
+-rw-r--r--   0        0        0     1647 2023-04-23 15:07:23.864750 windmill_api-1.89.0/windmill_api/api/workspace/archive_workspace.py
+-rw-r--r--   0        0        0     1856 2023-04-23 15:07:23.868751 windmill_api-1.89.0/windmill_api/api/workspace/create_workspace.py
+-rw-r--r--   0        0        0     2049 2023-04-23 15:07:23.900751 windmill_api-1.89.0/windmill_api/api/workspace/delete_invite.py
+-rw-r--r--   0        0        0     1688 2023-04-23 15:07:23.924751 windmill_api-1.89.0/windmill_api/api/workspace/delete_workspace.py
+-rw-r--r--   0        0        0     2063 2023-04-23 15:07:23.940751 windmill_api-1.89.0/windmill_api/api/workspace/edit_auto_invite.py
+-rw-r--r--   0        0        0     2083 2023-04-23 15:07:23.968752 windmill_api-1.89.0/windmill_api/api/workspace/edit_slack_command.py
+-rw-r--r--   0        0        0     2029 2023-04-23 15:07:23.976752 windmill_api-1.89.0/windmill_api/api/workspace/edit_webhook.py
+-rw-r--r--   0        0        0     1856 2023-04-23 15:07:24.008752 windmill_api-1.89.0/windmill_api/api/workspace/exists_username.py
+-rw-r--r--   0        0        0     1856 2023-04-23 15:07:24.012752 windmill_api-1.89.0/windmill_api/api/workspace/exists_workspace.py
+-rw-r--r--   0        0        0     2809 2023-04-23 15:07:24.068753 windmill_api-1.89.0/windmill_api/api/workspace/get_premium_info.py
+-rw-r--r--   0        0        0     2753 2023-04-23 15:07:24.060752 windmill_api-1.89.0/windmill_api/api/workspace/get_settings.py
+-rw-r--r--   0        0        0     2045 2023-04-23 15:07:24.100753 windmill_api-1.89.0/windmill_api/api/workspace/invite_user.py
+-rw-r--r--   0        0        0     2176 2023-04-23 15:07:24.116753 windmill_api-1.89.0/windmill_api/api/workspace/is_domain_allowed.py
+-rw-r--r--   0        0        0     3255 2023-04-23 15:07:24.156753 windmill_api-1.89.0/windmill_api/api/workspace/list_pending_invites.py
+-rw-r--r--   0        0        0     2583 2023-04-23 15:07:24.172754 windmill_api-1.89.0/windmill_api/api/workspace/list_user_workspaces.py
+-rw-r--r--   0        0        0     2775 2023-04-23 15:07:24.204754 windmill_api-1.89.0/windmill_api/api/workspace/list_workspaces.py
+-rw-r--r--   0        0        0     4311 2023-04-23 15:07:24.252754 windmill_api-1.89.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py
+-rw-r--r--   0        0        0     1651 2023-04-23 15:07:24.240754 windmill_api-1.89.0/windmill_api/api/workspace/unarchive_workspace.py
+-rw-r--r--   0        0        0     1821 2023-04-23 15:07:24.308755 windmill_api-1.89.0/windmill_api/client.py
+-rw-r--r--   0        0        0        1 2023-04-23 15:07:47.004977 windmill_api-1.89.0/windmill_api/models/__init__.py
+-rw-r--r--   0        0        0     1667 2023-04-23 15:07:24.344755 windmill_api-1.89.0/windmill_api/models/accept_invite_json_body.py
+-rw-r--r--   0        0        0     1710 2023-04-23 15:07:24.380756 windmill_api-1.89.0/windmill_api/models/add_granular_acls_json_body.py
+-rw-r--r--   0        0        0      301 2023-04-23 15:07:17.572686 windmill_api-1.89.0/windmill_api/models/add_granular_acls_kind.py
+-rw-r--r--   0        0        0     1529 2023-04-23 15:07:24.420756 windmill_api-1.89.0/windmill_api/models/add_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1940 2023-04-23 15:07:24.472756 windmill_api-1.89.0/windmill_api/models/add_user_json_body.py
+-rw-r--r--   0        0        0     1552 2023-04-23 15:07:24.492757 windmill_api-1.89.0/windmill_api/models/add_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3940 2023-04-23 15:07:24.544757 windmill_api-1.89.0/windmill_api/models/app_with_last_version.py
+-rw-r--r--   0        0        0      214 2023-04-23 15:07:17.452684 windmill_api-1.89.0/windmill_api/models/app_with_last_version_execution_mode.py
+-rw-r--r--   0        0        0     1248 2023-04-23 15:07:24.524757 windmill_api-1.89.0/windmill_api/models/app_with_last_version_extra_perms.py
+-rw-r--r--   0        0        0     3716 2023-04-23 15:07:24.592758 windmill_api-1.89.0/windmill_api/models/app_with_last_version_policy.py
+-rw-r--r--   0        0        0      220 2023-04-23 15:07:16.632676 windmill_api-1.89.0/windmill_api/models/app_with_last_version_policy_execution_mode.py
+-rw-r--r--   0        0        0     1946 2023-04-23 15:07:24.576758 windmill_api-1.89.0/windmill_api/models/app_with_last_version_policy_triggerables.py
+-rw-r--r--   0        0        0     1381 2023-04-23 15:07:24.608758 windmill_api-1.89.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1569 2023-04-23 15:07:24.628758 windmill_api-1.89.0/windmill_api/models/archive_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     7091 2023-04-23 15:07:24.760759 windmill_api-1.89.0/windmill_api/models/archive_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1314 2023-04-23 15:07:24.660758 windmill_api-1.89.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      259 2023-04-23 15:07:16.936679 windmill_api-1.89.0/windmill_api/models/archive_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      217 2023-04-23 15:07:17.632686 windmill_api-1.89.0/windmill_api/models/archive_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1288 2023-04-23 15:07:24.692759 windmill_api-1.89.0/windmill_api/models/archive_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     3452 2023-04-23 15:07:24.780760 windmill_api-1.89.0/windmill_api/models/audit_log.py
+-rw-r--r--   0        0        0      217 2023-04-23 15:07:16.820678 windmill_api-1.89.0/windmill_api/models/audit_log_action_kind.py
+-rw-r--r--   0        0        0      620 2023-04-23 15:07:16.676676 windmill_api-1.89.0/windmill_api/models/audit_log_operation.py
+-rw-r--r--   0        0        0     1186 2023-04-23 15:07:24.808760 windmill_api-1.89.0/windmill_api/models/audit_log_parameters.py
+-rw-r--r--   0        0        0     2933 2023-04-23 15:07:24.844760 windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-04-23 15:07:24.912761 windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-04-23 15:07:16.772677 windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-04-23 15:07:24.884760 windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-04-23 15:07:24.952761 windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-04-23 15:07:24.948761 windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-04-23 15:07:24.996762 windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-04-23 15:07:16.456674 windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-04-23 15:07:24.992762 windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-04-23 15:07:25.052762 windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-04-23 15:07:17.504685 windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-04-23 15:07:25.032762 windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-04-23 15:07:16.408673 windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2377 2023-04-23 15:07:25.088763 windmill_api-1.89.0/windmill_api/models/branch_all.py
+-rw-r--r--   0        0        0     2543 2023-04-23 15:07:25.120763 windmill_api-1.89.0/windmill_api/models/branch_all_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-04-23 15:07:25.192764 windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-04-23 15:07:25.180764 windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-04-23 15:07:25.224764 windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-04-23 15:07:25.236764 windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-04-23 15:07:25.272764 windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-23 15:07:16.952679 windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-04-23 15:07:25.276764 windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-23 15:07:17.100680 windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-04-23 15:07:25.308765 windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-04-23 15:07:25.320765 windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-04-23 15:07:17.960690 windmill_api-1.89.0/windmill_api/models/branch_all_type.py
+-rw-r--r--   0        0        0     2670 2023-04-23 15:07:25.364765 windmill_api-1.89.0/windmill_api/models/branch_one.py
+-rw-r--r--   0        0        0     2372 2023-04-23 15:07:25.388765 windmill_api-1.89.0/windmill_api/models/branch_one_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-04-23 15:07:25.496767 windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-04-23 15:07:25.444766 windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-04-23 15:07:25.488767 windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-04-23 15:07:25.532767 windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-04-23 15:07:25.532767 windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-23 15:07:16.816678 windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-04-23 15:07:25.568767 windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-23 15:07:17.772688 windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-04-23 15:07:25.588767 windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-04-23 15:07:25.608768 windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6125 2023-04-23 15:07:25.708769 windmill_api-1.89.0/windmill_api/models/branch_one_default_item.py
+-rw-r--r--   0        0        0     2906 2023-04-23 15:07:25.660768 windmill_api-1.89.0/windmill_api/models/branch_one_default_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-04-23 15:07:25.700769 windmill_api-1.89.0/windmill_api/models/branch_one_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-04-23 15:07:25.744769 windmill_api-1.89.0/windmill_api/models/branch_one_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-04-23 15:07:25.752769 windmill_api-1.89.0/windmill_api/models/branch_one_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-04-23 15:07:17.340683 windmill_api-1.89.0/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-04-23 15:07:25.780769 windmill_api-1.89.0/windmill_api/models/branch_one_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-04-23 15:07:16.616675 windmill_api-1.89.0/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-04-23 15:07:25.800770 windmill_api-1.89.0/windmill_api/models/branch_one_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-04-23 15:07:25.824770 windmill_api-1.89.0/windmill_api/models/branch_one_default_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-04-23 15:07:17.228682 windmill_api-1.89.0/windmill_api/models/branch_one_type.py
+-rw-r--r--   0        0        0     1532 2023-04-23 15:07:25.840770 windmill_api-1.89.0/windmill_api/models/cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     1255 2023-04-23 15:07:25.848770 windmill_api-1.89.0/windmill_api/models/cancel_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0    10508 2023-04-23 15:07:26.072772 windmill_api-1.89.0/windmill_api/models/completed_job.py
+-rw-r--r--   0        0        0     1176 2023-04-23 15:07:25.892770 windmill_api-1.89.0/windmill_api/models/completed_job_args.py
+-rw-r--r--   0        0        0     3265 2023-04-23 15:07:25.948771 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status.py
+-rw-r--r--   0        0        0     6800 2023-04-23 15:07:26.056772 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1789 2023-04-23 15:07:26.096773 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2136 2023-04-23 15:07:26.120773 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      202 2023-04-23 15:07:17.532685 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1694 2023-04-23 15:07:26.132773 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2230 2023-04-23 15:07:26.176773 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      360 2023-04-23 15:07:16.924679 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6402 2023-04-23 15:07:26.240774 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1779 2023-04-23 15:07:26.212774 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2116 2023-04-23 15:07:26.252774 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      200 2023-04-23 15:07:17.604686 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1684 2023-04-23 15:07:26.276774 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2220 2023-04-23 15:07:26.304775 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      358 2023-04-23 15:07:16.940679 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2040 2023-04-23 15:07:26.320775 windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_retry.py
+-rw-r--r--   0        0        0      310 2023-04-23 15:07:16.860678 windmill_api-1.89.0/windmill_api/models/completed_job_job_kind.py
+-rw-r--r--   0        0        0      199 2023-04-23 15:07:16.988679 windmill_api-1.89.0/windmill_api/models/completed_job_language.py
+-rw-r--r--   0        0        0     3127 2023-04-23 15:07:26.368775 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow.py
+-rw-r--r--   0        0        0     6620 2023-04-23 15:07:26.448776 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3129 2023-04-23 15:07:26.424776 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1929 2023-04-23 15:07:26.464776 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-04-23 15:07:26.496776 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-04-23 15:07:26.504777 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-23 15:07:17.220682 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-04-23 15:07:26.532777 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-23 15:07:17.960690 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-04-23 15:07:26.556777 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-04-23 15:07:26.572777 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6544 2023-04-23 15:07:26.684778 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3095 2023-04-23 15:07:26.624778 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1919 2023-04-23 15:07:26.660778 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2223 2023-04-23 15:07:26.704779 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2050 2023-04-23 15:07:26.728779 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      179 2023-04-23 15:07:17.924689 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1917 2023-04-23 15:07:26.744779 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      179 2023-04-23 15:07:16.672676 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1912 2023-04-23 15:07:26.768779 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1963 2023-04-23 15:07:26.780779 windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1572 2023-04-23 15:07:26.804779 windmill_api-1.89.0/windmill_api/models/connect_callback_json_body.py
+-rw-r--r--   0        0        0     2533 2023-04-23 15:07:26.852780 windmill_api-1.89.0/windmill_api/models/connect_callback_response_200.py
+-rw-r--r--   0        0        0     1600 2023-04-23 15:07:26.840780 windmill_api-1.89.0/windmill_api/models/connect_slack_callback_json_body.py
+-rw-r--r--   0        0        0     1753 2023-04-23 15:07:26.880780 windmill_api-1.89.0/windmill_api/models/contextual_variable.py
+-rw-r--r--   0        0        0     2147 2023-04-23 15:07:26.908780 windmill_api-1.89.0/windmill_api/models/create_account_json_body.py
+-rw-r--r--   0        0        0     2035 2023-04-23 15:07:26.924780 windmill_api-1.89.0/windmill_api/models/create_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-04-23 15:07:26.984781 windmill_api-1.89.0/windmill_api/models/create_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-04-23 15:07:17.068680 windmill_api-1.89.0/windmill_api/models/create_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-04-23 15:07:26.960781 windmill_api-1.89.0/windmill_api/models/create_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-04-23 15:07:26.988781 windmill_api-1.89.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-04-23 15:07:27.044782 windmill_api-1.89.0/windmill_api/models/create_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-04-23 15:07:27.016781 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-04-23 15:07:27.072782 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-04-23 15:07:27.164783 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-04-23 15:07:27.148783 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-04-23 15:07:27.188783 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-04-23 15:07:27.212783 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-04-23 15:07:27.232784 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-04-23 15:07:17.116681 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-04-23 15:07:27.252784 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-04-23 15:07:17.916689 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-04-23 15:07:27.272784 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-04-23 15:07:27.292784 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-04-23 15:07:27.388785 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-04-23 15:07:27.352785 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-04-23 15:07:27.420786 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-04-23 15:07:27.432786 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-04-23 15:07:27.464786 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-04-23 15:07:17.252682 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-04-23 15:07:27.476786 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-04-23 15:07:17.420684 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-04-23 15:07:27.500786 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-04-23 15:07:27.516786 windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2126 2023-04-23 15:07:27.548787 windmill_api-1.89.0/windmill_api/models/create_folder_json_body.py
+-rw-r--r--   0        0        0     1697 2023-04-23 15:07:27.556787 windmill_api-1.89.0/windmill_api/models/create_group_json_body.py
+-rw-r--r--   0        0        0     1613 2023-04-23 15:07:27.584787 windmill_api-1.89.0/windmill_api/models/create_input.py
+-rw-r--r--   0        0        0     1171 2023-04-23 15:07:27.584787 windmill_api-1.89.0/windmill_api/models/create_input_args.py
+-rw-r--r--   0        0        0     1701 2023-04-23 15:07:27.616787 windmill_api-1.89.0/windmill_api/models/create_input_json_body.py
+-rw-r--r--   0        0        0     1217 2023-04-23 15:07:27.636788 windmill_api-1.89.0/windmill_api/models/create_input_json_body_args.py
+-rw-r--r--   0        0        0      214 2023-04-23 15:07:17.116681 windmill_api-1.89.0/windmill_api/models/create_input_runnable_type.py
+-rw-r--r--   0        0        0     2094 2023-04-23 15:07:27.664788 windmill_api-1.89.0/windmill_api/models/create_resource.py
+-rw-r--r--   0        0        0     2140 2023-04-23 15:07:27.688788 windmill_api-1.89.0/windmill_api/models/create_resource_json_body.py
+-rw-r--r--   0        0        0     2335 2023-04-23 15:07:27.712788 windmill_api-1.89.0/windmill_api/models/create_resource_type_json_body.py
+-rw-r--r--   0        0        0     2780 2023-04-23 15:07:27.748789 windmill_api-1.89.0/windmill_api/models/create_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-04-23 15:07:27.736789 windmill_api-1.89.0/windmill_api/models/create_schedule_json_body_args.py
+-rw-r--r--   0        0        0     4829 2023-04-23 15:07:27.828789 windmill_api-1.89.0/windmill_api/models/create_script_json_body.py
+-rw-r--r--   0        0        0      249 2023-04-23 15:07:17.220682 windmill_api-1.89.0/windmill_api/models/create_script_json_body_kind.py
+-rw-r--r--   0        0        0      207 2023-04-23 15:07:16.840678 windmill_api-1.89.0/windmill_api/models/create_script_json_body_language.py
+-rw-r--r--   0        0        0     1232 2023-04-23 15:07:27.788789 windmill_api-1.89.0/windmill_api/models/create_script_json_body_schema.py
+-rw-r--r--   0        0        0     2534 2023-04-23 15:07:27.840790 windmill_api-1.89.0/windmill_api/models/create_token_impersonate_json_body.py
+-rw-r--r--   0        0        0     2169 2023-04-23 15:07:27.892790 windmill_api-1.89.0/windmill_api/models/create_token_json_body.py
+-rw-r--r--   0        0        0     2364 2023-04-23 15:07:27.900790 windmill_api-1.89.0/windmill_api/models/create_user_globally_json_body.py
+-rw-r--r--   0        0        0     1771 2023-04-23 15:07:27.928790 windmill_api-1.89.0/windmill_api/models/create_user_json_body.py
+-rw-r--r--   0        0        0     2493 2023-04-23 15:07:27.964791 windmill_api-1.89.0/windmill_api/models/create_variable.py
+-rw-r--r--   0        0        0     2539 2023-04-23 15:07:27.980791 windmill_api-1.89.0/windmill_api/models/create_variable_json_body.py
+-rw-r--r--   0        0        0     1678 2023-04-23 15:07:28.004791 windmill_api-1.89.0/windmill_api/models/create_workspace.py
+-rw-r--r--   0        0        0     1724 2023-04-23 15:07:28.016791 windmill_api-1.89.0/windmill_api/models/create_workspace_json_body.py
+-rw-r--r--   0        0        0     1490 2023-04-23 15:07:28.036791 windmill_api-1.89.0/windmill_api/models/decline_invite_json_body.py
+-rw-r--r--   0        0        0    11110 2023-04-23 15:07:28.204793 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200.py
+-rw-r--r--   0        0        0     1270 2023-04-23 15:07:28.068792 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3658 2023-04-23 15:07:28.128792 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7442 2023-04-23 15:07:28.268794 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1883 2023-04-23 15:07:28.240794 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2318 2023-04-23 15:07:28.280794 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      219 2023-04-23 15:07:16.632676 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1788 2023-04-23 15:07:28.308794 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2324 2023-04-23 15:07:28.328794 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      377 2023-04-23 15:07:17.752687 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7053 2023-04-23 15:07:28.424795 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1873 2023-04-23 15:07:28.388795 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2298 2023-04-23 15:07:28.428795 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      217 2023-04-23 15:07:17.680687 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1778 2023-04-23 15:07:28.464796 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2314 2023-04-23 15:07:28.480796 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      375 2023-04-23 15:07:17.996690 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2134 2023-04-23 15:07:28.508796 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      327 2023-04-23 15:07:17.932689 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      216 2023-04-23 15:07:17.976690 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3432 2023-04-23 15:07:28.548797 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7425 2023-04-23 15:07:28.620797 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3442 2023-04-23 15:07:28.604797 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2023 2023-04-23 15:07:28.648797 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2327 2023-04-23 15:07:28.664798 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2261 2023-04-23 15:07:28.716798 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-23 15:07:16.548675 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-23 15:07:28.700798 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-23 15:07:17.524685 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2016 2023-04-23 15:07:28.740798 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2067 2023-04-23 15:07:28.756799 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7349 2023-04-23 15:07:28.876800 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3408 2023-04-23 15:07:28.812799 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2013 2023-04-23 15:07:28.852800 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2317 2023-04-23 15:07:28.900800 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2241 2023-04-23 15:07:28.920800 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-04-23 15:07:16.680676 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2108 2023-04-23 15:07:28.940800 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-04-23 15:07:17.380684 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2006 2023-04-23 15:07:28.964801 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2057 2023-04-23 15:07:28.980801 windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1783 2023-04-23 15:07:29.004801 windmill_api-1.89.0/windmill_api/models/delete_invite_json_body.py
+-rw-r--r--   0        0        0     7065 2023-04-23 15:07:29.108802 windmill_api-1.89.0/windmill_api/models/delete_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1309 2023-04-23 15:07:29.040801 windmill_api-1.89.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      258 2023-04-23 15:07:17.460684 windmill_api-1.89.0/windmill_api/models/delete_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      216 2023-04-23 15:07:17.864688 windmill_api-1.89.0/windmill_api/models/delete_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1283 2023-04-23 15:07:29.076802 windmill_api-1.89.0/windmill_api/models/delete_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     2933 2023-04-23 15:07:29.128802 windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-04-23 15:07:29.192803 windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-04-23 15:07:17.040680 windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-04-23 15:07:29.164803 windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-04-23 15:07:29.196803 windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-04-23 15:07:29.264804 windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-04-23 15:07:29.248803 windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-04-23 15:07:16.608675 windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-04-23 15:07:29.280804 windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-04-23 15:07:29.320804 windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-04-23 15:07:17.132681 windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-04-23 15:07:29.316804 windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-04-23 15:07:17.292683 windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     1551 2023-04-23 15:07:29.352804 windmill_api-1.89.0/windmill_api/models/edit_auto_invite_json_body.py
+-rw-r--r--   0        0        0     1980 2023-04-23 15:07:29.372804 windmill_api-1.89.0/windmill_api/models/edit_resource.py
+-rw-r--r--   0        0        0     1791 2023-04-23 15:07:29.412805 windmill_api-1.89.0/windmill_api/models/edit_resource_type.py
+-rw-r--r--   0        0        0     1845 2023-04-23 15:07:29.412805 windmill_api-1.89.0/windmill_api/models/edit_schedule.py
+-rw-r--r--   0        0        0     1176 2023-04-23 15:07:29.440805 windmill_api-1.89.0/windmill_api/models/edit_schedule_args.py
+-rw-r--r--   0        0        0     1691 2023-04-23 15:07:29.448805 windmill_api-1.89.0/windmill_api/models/edit_slack_command_json_body.py
+-rw-r--r--   0        0        0     2260 2023-04-23 15:07:29.488806 windmill_api-1.89.0/windmill_api/models/edit_variable.py
+-rw-r--r--   0        0        0     1520 2023-04-23 15:07:29.480806 windmill_api-1.89.0/windmill_api/models/edit_webhook_json_body.py
+-rw-r--r--   0        0        0     2058 2023-04-23 15:07:29.524806 windmill_api-1.89.0/windmill_api/models/edit_workspace_user.py
+-rw-r--r--   0        0        0     3663 2023-04-23 15:07:29.552806 windmill_api-1.89.0/windmill_api/models/execute_component_json_body.py
+-rw-r--r--   0        0        0     1346 2023-04-23 15:07:29.560806 windmill_api-1.89.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
+-rw-r--r--   0        0        0     1942 2023-04-23 15:07:29.592807 windmill_api-1.89.0/windmill_api/models/execute_component_json_body_raw_code.py
+-rw-r--r--   0        0        0     1577 2023-04-23 15:07:29.604807 windmill_api-1.89.0/windmill_api/models/exists_username_json_body.py
+-rw-r--r--   0        0        0     1400 2023-04-23 15:07:29.620807 windmill_api-1.89.0/windmill_api/models/exists_workspace_json_body.py
+-rw-r--r--   0        0        0     4633 2023-04-23 15:07:29.696808 windmill_api-1.89.0/windmill_api/models/flow.py
+-rw-r--r--   0        0        0     1166 2023-04-23 15:07:29.648807 windmill_api-1.89.0/windmill_api/models/flow_extra_perms.py
+-rw-r--r--   0        0        0     3416 2023-04-23 15:07:29.712808 windmill_api-1.89.0/windmill_api/models/flow_metadata.py
+-rw-r--r--   0        0        0     1209 2023-04-23 15:07:29.728808 windmill_api-1.89.0/windmill_api/models/flow_metadata_extra_perms.py
+-rw-r--r--   0        0        0     5729 2023-04-23 15:07:29.848809 windmill_api-1.89.0/windmill_api/models/flow_module.py
+-rw-r--r--   0        0        0     2726 2023-04-23 15:07:29.788809 windmill_api-1.89.0/windmill_api/models/flow_module_retry.py
+-rw-r--r--   0        0        0     1807 2023-04-23 15:07:29.832809 windmill_api-1.89.0/windmill_api/models/flow_module_retry_constant.py
+-rw-r--r--   0        0        0     2111 2023-04-23 15:07:29.876810 windmill_api-1.89.0/windmill_api/models/flow_module_retry_exponential.py
+-rw-r--r--   0        0        0     1834 2023-04-23 15:07:29.884810 windmill_api-1.89.0/windmill_api/models/flow_module_sleep_type_0.py
+-rw-r--r--   0        0        0      159 2023-04-23 15:07:16.696676 windmill_api-1.89.0/windmill_api/models/flow_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1701 2023-04-23 15:07:29.916810 windmill_api-1.89.0/windmill_api/models/flow_module_sleep_type_1.py
+-rw-r--r--   0        0        0      159 2023-04-23 15:07:16.700676 windmill_api-1.89.0/windmill_api/models/flow_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1800 2023-04-23 15:07:29.924810 windmill_api-1.89.0/windmill_api/models/flow_module_stop_after_if.py
+-rw-r--r--   0        0        0     1851 2023-04-23 15:07:29.984811 windmill_api-1.89.0/windmill_api/models/flow_module_suspend.py
+-rw-r--r--   0        0        0     3292 2023-04-23 15:07:29.984811 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_0.py
+-rw-r--r--   0        0        0     3564 2023-04-23 15:07:30.036811 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-04-23 15:07:30.024811 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-23 15:07:16.604675 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-23 15:07:30.064812 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-23 15:07:16.620675 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      208 2023-04-23 15:07:17.536685 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_0_language.py
+-rw-r--r--   0        0        0      158 2023-04-23 15:07:17.072680 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_0_type.py
+-rw-r--r--   0        0        0     2477 2023-04-23 15:07:30.100812 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_1.py
+-rw-r--r--   0        0        0     3564 2023-04-23 15:07:30.116812 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-04-23 15:07:30.144812 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-23 15:07:16.616675 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-23 15:07:30.156813 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-23 15:07:17.068680 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      152 2023-04-23 15:07:16.960679 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_1_type.py
+-rw-r--r--   0        0        0     2204 2023-04-23 15:07:30.196813 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_2.py
+-rw-r--r--   0        0        0     3564 2023-04-23 15:07:30.208813 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-04-23 15:07:30.240813 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-23 15:07:17.828688 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-23 15:07:30.284814 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-23 15:07:18.020690 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      148 2023-04-23 15:07:17.444684 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_2_type.py
+-rw-r--r--   0        0        0     4138 2023-04-23 15:07:30.332814 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3.py
+-rw-r--r--   0        0        0     1990 2023-04-23 15:07:30.320814 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
+-rw-r--r--   0        0        0      173 2023-04-23 15:07:16.712676 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1857 2023-04-23 15:07:30.360815 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
+-rw-r--r--   0        0        0      173 2023-04-23 15:07:17.968690 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6636 2023-04-23 15:07:30.456816 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py
+-rw-r--r--   0        0        0     3148 2023-04-23 15:07:30.412815 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-04-23 15:07:30.456816 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-04-23 15:07:30.528816 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-04-23 15:07:30.500816 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-23 15:07:16.936679 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-04-23 15:07:30.540816 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-23 15:07:17.716687 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-04-23 15:07:30.568817 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-04-23 15:07:30.584817 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
+-rw-r--r--   0        0        0      162 2023-04-23 15:07:16.632676 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_type.py
+-rw-r--r--   0        0        0     2934 2023-04-23 15:07:30.620817 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4.py
+-rw-r--r--   0        0        0     2508 2023-04-23 15:07:30.632817 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-04-23 15:07:30.732818 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-04-23 15:07:30.688818 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-04-23 15:07:30.728818 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-04-23 15:07:30.796819 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-04-23 15:07:30.768819 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-23 15:07:17.124681 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-04-23 15:07:30.808819 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-23 15:07:17.504685 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-04-23 15:07:30.836819 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-04-23 15:07:30.844819 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6636 2023-04-23 15:07:30.956821 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item.py
+-rw-r--r--   0        0        0     3148 2023-04-23 15:07:30.900820 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-04-23 15:07:30.936820 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-04-23 15:07:30.984821 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-04-23 15:07:31.000821 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-23 15:07:16.592675 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-04-23 15:07:31.060822 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-23 15:07:17.332683 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-04-23 15:07:31.044821 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-04-23 15:07:31.104822 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-04-23 15:07:17.720687 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_type.py
+-rw-r--r--   0        0        0     2577 2023-04-23 15:07:31.112822 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5.py
+-rw-r--r--   0        0        0     2679 2023-04-23 15:07:31.156823 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-04-23 15:07:31.228823 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-04-23 15:07:31.208823 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-04-23 15:07:31.248823 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-04-23 15:07:31.276824 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-04-23 15:07:31.292824 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-23 15:07:17.976690 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-04-23 15:07:31.316824 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-23 15:07:17.000680 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-04-23 15:07:31.364824 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-04-23 15:07:31.352824 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-04-23 15:07:17.576686 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_type.py
+-rw-r--r--   0        0        0     1839 2023-04-23 15:07:31.396825 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_6.py
+-rw-r--r--   0        0        0      156 2023-04-23 15:07:17.332683 windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_6_type.py
+-rw-r--r--   0        0        0     2009 2023-04-23 15:07:31.412825 windmill_api-1.89.0/windmill_api/models/flow_preview.py
+-rw-r--r--   0        0        0     1171 2023-04-23 15:07:31.420825 windmill_api-1.89.0/windmill_api/models/flow_preview_args.py
+-rw-r--r--   0        0        0     3074 2023-04-23 15:07:31.468825 windmill_api-1.89.0/windmill_api/models/flow_preview_value.py
+-rw-r--r--   0        0        0     6498 2023-04-23 15:07:31.568827 windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module.py
+-rw-r--r--   0        0        0     3064 2023-04-23 15:07:31.520826 windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1911 2023-04-23 15:07:31.564826 windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2215 2023-04-23 15:07:31.612827 windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2036 2023-04-23 15:07:31.604827 windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-04-23 15:07:17.064680 windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1903 2023-04-23 15:07:31.644827 windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-23 15:07:17.008679 windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1904 2023-04-23 15:07:31.652827 windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1955 2023-04-23 15:07:31.684828 windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6422 2023-04-23 15:07:31.760828 windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item.py
+-rw-r--r--   0        0        0     3030 2023-04-23 15:07:31.736828 windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1901 2023-04-23 15:07:31.776829 windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2205 2023-04-23 15:07:31.808829 windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2016 2023-04-23 15:07:31.816829 windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-04-23 15:07:17.724687 windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1883 2023-04-23 15:07:31.880830 windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-04-23 15:07:17.072680 windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1894 2023-04-23 15:07:31.860829 windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1945 2023-04-23 15:07:31.904830 windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1143 2023-04-23 15:07:31.912830 windmill_api-1.89.0/windmill_api/models/flow_schema.py
+-rw-r--r--   0        0        0     3001 2023-04-23 15:07:31.968830 windmill_api-1.89.0/windmill_api/models/flow_status.py
+-rw-r--r--   0        0        0     6370 2023-04-23 15:07:32.024831 windmill_api-1.89.0/windmill_api/models/flow_status_failure_module.py
+-rw-r--r--   0        0        0     1723 2023-04-23 15:07:32.008831 windmill_api-1.89.0/windmill_api/models/flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     1999 2023-04-23 15:07:32.044831 windmill_api-1.89.0/windmill_api/models/flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      190 2023-04-23 15:07:16.944679 windmill_api-1.89.0/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1628 2023-04-23 15:07:32.068831 windmill_api-1.89.0/windmill_api/models/flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2164 2023-04-23 15:07:32.092832 windmill_api-1.89.0/windmill_api/models/flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      348 2023-04-23 15:07:16.604675 windmill_api-1.89.0/windmill_api/models/flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     5808 2023-04-23 15:07:32.192833 windmill_api-1.89.0/windmill_api/models/flow_status_module.py
+-rw-r--r--   0        0        0     1685 2023-04-23 15:07:32.164832 windmill_api-1.89.0/windmill_api/models/flow_status_module_approvers_item.py
+-rw-r--r--   0        0        0     1925 2023-04-23 15:07:32.204833 windmill_api-1.89.0/windmill_api/models/flow_status_module_branch_chosen.py
+-rw-r--r--   0        0        0      183 2023-04-23 15:07:17.020680 windmill_api-1.89.0/windmill_api/models/flow_status_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1590 2023-04-23 15:07:32.236833 windmill_api-1.89.0/windmill_api/models/flow_status_module_branchall.py
+-rw-r--r--   0        0        0     2126 2023-04-23 15:07:32.252833 windmill_api-1.89.0/windmill_api/models/flow_status_module_iterator.py
+-rw-r--r--   0        0        0      341 2023-04-23 15:07:17.732687 windmill_api-1.89.0/windmill_api/models/flow_status_module_type.py
+-rw-r--r--   0        0        0     5981 2023-04-23 15:07:32.356834 windmill_api-1.89.0/windmill_api/models/flow_status_modules_item.py
+-rw-r--r--   0        0        0     1713 2023-04-23 15:07:32.284834 windmill_api-1.89.0/windmill_api/models/flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     1979 2023-04-23 15:07:32.320834 windmill_api-1.89.0/windmill_api/models/flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      188 2023-04-23 15:07:16.748677 windmill_api-1.89.0/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1618 2023-04-23 15:07:32.356834 windmill_api-1.89.0/windmill_api/models/flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2154 2023-04-23 15:07:32.404835 windmill_api-1.89.0/windmill_api/models/flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      346 2023-04-23 15:07:16.756677 windmill_api-1.89.0/windmill_api/models/flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     1974 2023-04-23 15:07:32.440835 windmill_api-1.89.0/windmill_api/models/flow_status_retry.py
+-rw-r--r--   0        0        0     2957 2023-04-23 15:07:32.460835 windmill_api-1.89.0/windmill_api/models/flow_value.py
+-rw-r--r--   0        0        0     6224 2023-04-23 15:07:32.560836 windmill_api-1.89.0/windmill_api/models/flow_value_failure_module.py
+-rw-r--r--   0        0        0     2940 2023-04-23 15:07:32.516836 windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1873 2023-04-23 15:07:32.552836 windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-04-23 15:07:32.596837 windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-04-23 15:07:32.604837 windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-04-23 15:07:16.768677 windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-04-23 15:07:32.636837 windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-04-23 15:07:16.988679 windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-04-23 15:07:32.648837 windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-04-23 15:07:32.708838 windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6125 2023-04-23 15:07:32.768838 windmill_api-1.89.0/windmill_api/models/flow_value_modules_item.py
+-rw-r--r--   0        0        0     2906 2023-04-23 15:07:32.764838 windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-04-23 15:07:32.812839 windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-04-23 15:07:32.816839 windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-04-23 15:07:32.856839 windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-04-23 15:07:18.028690 windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-04-23 15:07:32.856839 windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-04-23 15:07:17.164681 windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-04-23 15:07:32.896839 windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-04-23 15:07:32.896839 windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1858 2023-04-23 15:07:32.968840 windmill_api-1.89.0/windmill_api/models/folder.py
+-rw-r--r--   0        0        0     1179 2023-04-23 15:07:32.928840 windmill_api-1.89.0/windmill_api/models/folder_extra_perms.py
+-rw-r--r--   0        0        0     1560 2023-04-23 15:07:32.964840 windmill_api-1.89.0/windmill_api/models/force_cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     3807 2023-04-23 15:07:33.032841 windmill_api-1.89.0/windmill_api/models/forloop_flow.py
+-rw-r--r--   0        0        0     1874 2023-04-23 15:07:33.012841 windmill_api-1.89.0/windmill_api/models/forloop_flow_iterator_type_0.py
+-rw-r--r--   0        0        0      163 2023-04-23 15:07:17.468684 windmill_api-1.89.0/windmill_api/models/forloop_flow_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1741 2023-04-23 15:07:33.052841 windmill_api-1.89.0/windmill_api/models/forloop_flow_iterator_type_1.py
+-rw-r--r--   0        0        0      163 2023-04-23 15:07:16.904678 windmill_api-1.89.0/windmill_api/models/forloop_flow_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6224 2023-04-23 15:07:33.156842 windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item.py
+-rw-r--r--   0        0        0     2940 2023-04-23 15:07:33.108842 windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1873 2023-04-23 15:07:33.156842 windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-04-23 15:07:33.200842 windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-04-23 15:07:33.236843 windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-04-23 15:07:17.568685 windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-04-23 15:07:33.240843 windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-04-23 15:07:16.620675 windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-04-23 15:07:33.276843 windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-04-23 15:07:33.284843 windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0      152 2023-04-23 15:07:16.496674 windmill_api-1.89.0/windmill_api/models/forloop_flow_type.py
+-rw-r--r--   0        0        0     4052 2023-04-23 15:07:33.344844 windmill_api-1.89.0/windmill_api/models/get_app_by_path_response_200.py
+-rw-r--r--   0        0        0      219 2023-04-23 15:07:17.328683 windmill_api-1.89.0/windmill_api/models/get_app_by_path_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1279 2023-04-23 15:07:33.312844 windmill_api-1.89.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3811 2023-04-23 15:07:33.376844 windmill_api-1.89.0/windmill_api/models/get_app_by_path_response_200_policy.py
+-rw-r--r--   0        0        0      225 2023-04-23 15:07:16.956679 windmill_api-1.89.0/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2009 2023-04-23 15:07:33.380844 windmill_api-1.89.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1412 2023-04-23 15:07:33.408845 windmill_api-1.89.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4112 2023-04-23 15:07:33.452845 windmill_api-1.89.0/windmill_api/models/get_app_by_version_response_200.py
+-rw-r--r--   0        0        0      222 2023-04-23 15:07:17.796688 windmill_api-1.89.0/windmill_api/models/get_app_by_version_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1294 2023-04-23 15:07:33.436845 windmill_api-1.89.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3862 2023-04-23 15:07:33.528846 windmill_api-1.89.0/windmill_api/models/get_app_by_version_response_200_policy.py
+-rw-r--r--   0        0        0      228 2023-04-23 15:07:17.644686 windmill_api-1.89.0/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2042 2023-04-23 15:07:33.488845 windmill_api-1.89.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1427 2023-04-23 15:07:33.516846 windmill_api-1.89.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3764 2023-04-23 15:07:33.588846 windmill_api-1.89.0/windmill_api/models/get_audit_log_response_200.py
+-rw-r--r--   0        0        0      231 2023-04-23 15:07:16.992679 windmill_api-1.89.0/windmill_api/models/get_audit_log_response_200_action_kind.py
+-rw-r--r--   0        0        0      634 2023-04-23 15:07:16.840678 windmill_api-1.89.0/windmill_api/models/get_audit_log_response_200_operation.py
+-rw-r--r--   0        0        0     1265 2023-04-23 15:07:33.560846 windmill_api-1.89.0/windmill_api/models/get_audit_log_response_200_parameters.py
+-rw-r--r--   0        0        0    11008 2023-04-23 15:07:33.744848 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200.py
+-rw-r--r--   0        0        0     1255 2023-04-23 15:07:33.616847 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3595 2023-04-23 15:07:33.680847 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7343 2023-04-23 15:07:33.840849 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1868 2023-04-23 15:07:33.784848 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2288 2023-04-23 15:07:33.820849 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      216 2023-04-23 15:07:17.400684 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1773 2023-04-23 15:07:33.856849 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2309 2023-04-23 15:07:33.896849 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      374 2023-04-23 15:07:17.048680 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6924 2023-04-23 15:07:34.008850 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1858 2023-04-23 15:07:33.928850 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-04-23 15:07:33.968850 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-04-23 15:07:17.340683 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-04-23 15:07:34.008850 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2299 2023-04-23 15:07:34.064851 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      372 2023-04-23 15:07:16.392673 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2119 2023-04-23 15:07:34.052851 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      324 2023-04-23 15:07:17.988690 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      213 2023-04-23 15:07:17.780688 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3375 2023-04-23 15:07:34.112851 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7311 2023-04-23 15:07:34.176852 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3391 2023-04-23 15:07:34.168852 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2008 2023-04-23 15:07:34.208852 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2312 2023-04-23 15:07:34.220852 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2231 2023-04-23 15:07:34.244853 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      195 2023-04-23 15:07:16.948679 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2098 2023-04-23 15:07:34.308853 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      195 2023-04-23 15:07:17.800688 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2001 2023-04-23 15:07:34.284853 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2052 2023-04-23 15:07:34.324854 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7235 2023-04-23 15:07:34.428855 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3357 2023-04-23 15:07:34.376854 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1998 2023-04-23 15:07:34.412854 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-04-23 15:07:34.456855 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-04-23 15:07:34.468855 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-23 15:07:16.444674 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-04-23 15:07:34.524855 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-23 15:07:17.380684 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-04-23 15:07:34.508855 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-04-23 15:07:34.552856 windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     5083 2023-04-23 15:07:34.616856 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200.py
+-rw-r--r--   0        0        0     1281 2023-04-23 15:07:34.580856 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1258 2023-04-23 15:07:34.604856 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     3302 2023-04-23 15:07:34.680857 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value.py
+-rw-r--r--   0        0        0     7159 2023-04-23 15:07:34.728857 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
+-rw-r--r--   0        0        0     3323 2023-04-23 15:07:34.736858 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1988 2023-04-23 15:07:34.768858 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-04-23 15:07:34.780858 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-04-23 15:07:34.812858 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-04-23 15:07:16.992679 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-04-23 15:07:34.872859 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-04-23 15:07:16.760677 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-04-23 15:07:34.856859 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-04-23 15:07:34.896859 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7066 2023-04-23 15:07:34.984860 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
+-rw-r--r--   0        0        0     3289 2023-04-23 15:07:34.948860 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1978 2023-04-23 15:07:35.024860 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2282 2023-04-23 15:07:35.028860 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2171 2023-04-23 15:07:35.064861 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-04-23 15:07:17.064680 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2038 2023-04-23 15:07:35.076861 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-04-23 15:07:17.596686 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1971 2023-04-23 15:07:35.104861 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2022 2023-04-23 15:07:35.120861 windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2756 2023-04-23 15:07:35.156862 windmill_api-1.89.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
+-rw-r--r--   0        0        0     1337 2023-04-23 15:07:35.148862 windmill_api-1.89.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
+-rw-r--r--   0        0        0     2010 2023-04-23 15:07:35.196862 windmill_api-1.89.0/windmill_api/models/get_folder_response_200.py
+-rw-r--r--   0        0        0     1258 2023-04-23 15:07:35.188862 windmill_api-1.89.0/windmill_api/models/get_folder_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2357 2023-04-23 15:07:35.248863 windmill_api-1.89.0/windmill_api/models/get_folder_usage_response_200.py
+-rw-r--r--   0        0        0      301 2023-04-23 15:07:16.788677 windmill_api-1.89.0/windmill_api/models/get_granular_acls_kind.py
+-rw-r--r--   0        0        0     1235 2023-04-23 15:07:35.224862 windmill_api-1.89.0/windmill_api/models/get_granular_acls_response_200.py
+-rw-r--r--   0        0        0     2888 2023-04-23 15:07:35.292863 windmill_api-1.89.0/windmill_api/models/get_group_response_200.py
+-rw-r--r--   0        0        0     1253 2023-04-23 15:07:35.280863 windmill_api-1.89.0/windmill_api/models/get_group_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1606 2023-04-23 15:07:35.320863 windmill_api-1.89.0/windmill_api/models/get_hub_app_by_id_response_200.py
+-rw-r--r--   0        0        0     1634 2023-04-23 15:07:35.328863 windmill_api-1.89.0/windmill_api/models/get_hub_app_by_id_response_200_app.py
+-rw-r--r--   0        0        0     1977 2023-04-23 15:07:35.360864 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200.py
+-rw-r--r--   0        0        0     2950 2023-04-23 15:07:35.380864 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
+-rw-r--r--   0        0        0     1289 2023-04-23 15:07:35.388864 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
+-rw-r--r--   0        0        0     3410 2023-04-23 15:07:35.436864 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
+-rw-r--r--   0        0        0     7365 2023-04-23 15:07:35.504865 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3418 2023-04-23 15:07:35.532865 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2019 2023-04-23 15:07:35.576866 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2323 2023-04-23 15:07:35.576866 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2249 2023-04-23 15:07:35.616866 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-04-23 15:07:17.076680 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2116 2023-04-23 15:07:35.616866 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-04-23 15:07:16.812677 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2012 2023-04-23 15:07:35.656867 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2063 2023-04-23 15:07:35.660867 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7289 2023-04-23 15:07:35.768868 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
+-rw-r--r--   0        0        0     3384 2023-04-23 15:07:35.712867 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2009 2023-04-23 15:07:35.752868 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2313 2023-04-23 15:07:35.796868 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2229 2023-04-23 15:07:35.804868 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      194 2023-04-23 15:07:17.084680 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2096 2023-04-23 15:07:35.836868 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      194 2023-04-23 15:07:17.284682 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2002 2023-04-23 15:07:35.844868 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2053 2023-04-23 15:07:35.880869 windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2698 2023-04-23 15:07:35.900869 windmill_api-1.89.0/windmill_api/models/get_hub_script_by_path_response_200.py
+-rw-r--r--   0        0        0      216 2023-04-23 15:07:16.560675 windmill_api-1.89.0/windmill_api/models/get_hub_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     2644 2023-04-23 15:07:35.936869 windmill_api-1.89.0/windmill_api/models/get_input_history_response_200_item.py
+-rw-r--r--   0        0        0     1278 2023-04-23 15:07:35.924869 windmill_api-1.89.0/windmill_api/models/get_input_history_response_200_item_args.py
+-rw-r--r--   0        0        0      218 2023-04-23 15:07:17.592686 windmill_api-1.89.0/windmill_api/models/get_input_history_runnable_type.py
+-rw-r--r--   0        0        0     1852 2023-04-23 15:07:35.976870 windmill_api-1.89.0/windmill_api/models/get_job_response_200.py
+-rw-r--r--   0        0        0      188 2023-04-23 15:07:17.704687 windmill_api-1.89.0/windmill_api/models/get_job_response_200_type.py
+-rw-r--r--   0        0        0     2364 2023-04-23 15:07:35.992870 windmill_api-1.89.0/windmill_api/models/get_job_updates_response_200.py
+-rw-r--r--   0        0        0     1744 2023-04-23 15:07:36.064870 windmill_api-1.89.0/windmill_api/models/get_premium_info_response_200.py
+-rw-r--r--   0        0        0     4218 2023-04-23 15:07:36.072871 windmill_api-1.89.0/windmill_api/models/get_public_app_by_secret_response_200.py
+-rw-r--r--   0        0        0      227 2023-04-23 15:07:17.344683 windmill_api-1.89.0/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1322 2023-04-23 15:07:36.100871 windmill_api-1.89.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3970 2023-04-23 15:07:36.176872 windmill_api-1.89.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py
+-rw-r--r--   0        0        0      233 2023-04-23 15:07:16.624676 windmill_api-1.89.0/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2131 2023-04-23 15:07:36.136871 windmill_api-1.89.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1455 2023-04-23 15:07:36.164872 windmill_api-1.89.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3533 2023-04-23 15:07:36.236872 windmill_api-1.89.0/windmill_api/models/get_resource_response_200.py
+-rw-r--r--   0        0        0     1268 2023-04-23 15:07:36.204872 windmill_api-1.89.0/windmill_api/models/get_resource_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2335 2023-04-23 15:07:36.256873 windmill_api-1.89.0/windmill_api/models/get_resource_type_response_200.py
+-rw-r--r--   0        0        0     1840 2023-04-23 15:07:36.276873 windmill_api-1.89.0/windmill_api/models/get_resume_urls_response_200.py
+-rw-r--r--   0        0        0     4325 2023-04-23 15:07:36.336873 windmill_api-1.89.0/windmill_api/models/get_schedule_response_200.py
+-rw-r--r--   0        0        0     1232 2023-04-23 15:07:36.300873 windmill_api-1.89.0/windmill_api/models/get_schedule_response_200_args.py
+-rw-r--r--   0        0        0     1268 2023-04-23 15:07:36.332873 windmill_api-1.89.0/windmill_api/models/get_schedule_response_200_extra_perms.py
+-rw-r--r--   0        0        0     6987 2023-04-23 15:07:36.448874 windmill_api-1.89.0/windmill_api/models/get_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1294 2023-04-23 15:07:36.360873 windmill_api-1.89.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-04-23 15:07:17.348683 windmill_api-1.89.0/windmill_api/models/get_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-04-23 15:07:16.612676 windmill_api-1.89.0/windmill_api/models/get_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-04-23 15:07:36.392874 windmill_api-1.89.0/windmill_api/models/get_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     6987 2023-04-23 15:07:36.520875 windmill_api-1.89.0/windmill_api/models/get_script_by_path_response_200.py
+-rw-r--r--   0        0        0     1294 2023-04-23 15:07:36.476875 windmill_api-1.89.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-04-23 15:07:17.064680 windmill_api-1.89.0/windmill_api/models/get_script_by_path_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-04-23 15:07:17.800688 windmill_api-1.89.0/windmill_api/models/get_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-04-23 15:07:36.512875 windmill_api-1.89.0/windmill_api/models/get_script_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     1922 2023-04-23 15:07:36.552875 windmill_api-1.89.0/windmill_api/models/get_script_deployment_status_response_200.py
+-rw-r--r--   0        0        0     4157 2023-04-23 15:07:36.600876 windmill_api-1.89.0/windmill_api/models/get_settings_response_200.py
+-rw-r--r--   0        0        0     2428 2023-04-23 15:07:36.596876 windmill_api-1.89.0/windmill_api/models/get_suspended_job_flow_response_200.py
+-rw-r--r--   0        0        0     1764 2023-04-23 15:07:36.692877 windmill_api-1.89.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
+-rw-r--r--   0        0        0     2040 2023-04-23 15:07:36.644876 windmill_api-1.89.0/windmill_api/models/get_suspended_job_flow_response_200_job.py
+-rw-r--r--   0        0        0      204 2023-04-23 15:07:16.612676 windmill_api-1.89.0/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
+-rw-r--r--   0        0        0     4554 2023-04-23 15:07:36.772878 windmill_api-1.89.0/windmill_api/models/get_variable_response_200.py
+-rw-r--r--   0        0        0     1268 2023-04-23 15:07:36.720877 windmill_api-1.89.0/windmill_api/models/get_variable_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2647 2023-04-23 15:07:36.772878 windmill_api-1.89.0/windmill_api/models/global_user_info.py
+-rw-r--r--   0        0        0      176 2023-04-23 15:07:16.656676 windmill_api-1.89.0/windmill_api/models/global_user_info_login_type.py
+-rw-r--r--   0        0        0     1627 2023-04-23 15:07:36.808878 windmill_api-1.89.0/windmill_api/models/global_user_update_json_body.py
+-rw-r--r--   0        0        0     2741 2023-04-23 15:07:36.824878 windmill_api-1.89.0/windmill_api/models/global_whoami_response_200.py
+-rw-r--r--   0        0        0      185 2023-04-23 15:07:16.540675 windmill_api-1.89.0/windmill_api/models/global_whoami_response_200_login_type.py
+-rw-r--r--   0        0        0     2903 2023-04-23 15:07:36.864878 windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5478 2023-04-23 15:07:36.916879 windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      324 2023-04-23 15:07:16.960679 windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1598 2023-04-23 15:07:36.896879 windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1663 2023-04-23 15:07:36.932879 windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2151 2023-04-23 15:07:36.956879 windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3257 2023-04-23 15:07:36.984880 windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      342 2023-04-23 15:07:17.520685 windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1631 2023-04-23 15:07:36.992880 windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3100 2023-04-23 15:07:37.032880 windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      333 2023-04-23 15:07:17.532685 windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1580 2023-04-23 15:07:37.032880 windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-23 15:07:16.512674 windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2722 2023-04-23 15:07:37.096881 windmill_api-1.89.0/windmill_api/models/group.py
+-rw-r--r--   0        0        0     1174 2023-04-23 15:07:37.060880 windmill_api-1.89.0/windmill_api/models/group_extra_perms.py
+-rw-r--r--   0        0        0     1689 2023-04-23 15:07:37.100881 windmill_api-1.89.0/windmill_api/models/identity.py
+-rw-r--r--   0        0        0      143 2023-04-23 15:07:17.484685 windmill_api-1.89.0/windmill_api/models/identity_type.py
+-rw-r--r--   0        0        0     2377 2023-04-23 15:07:37.152881 windmill_api-1.89.0/windmill_api/models/input_.py
+-rw-r--r--   0        0        0     1138 2023-04-23 15:07:37.128881 windmill_api-1.89.0/windmill_api/models/input_args.py
+-rw-r--r--   0        0        0     1820 2023-04-23 15:07:37.164881 windmill_api-1.89.0/windmill_api/models/input_transform_type_0.py
+-rw-r--r--   0        0        0      158 2023-04-23 15:07:17.308683 windmill_api-1.89.0/windmill_api/models/input_transform_type_0_type.py
+-rw-r--r--   0        0        0     1687 2023-04-23 15:07:37.196882 windmill_api-1.89.0/windmill_api/models/input_transform_type_1.py
+-rw-r--r--   0        0        0      158 2023-04-23 15:07:17.160681 windmill_api-1.89.0/windmill_api/models/input_transform_type_1_type.py
+-rw-r--r--   0        0        0     1773 2023-04-23 15:07:37.208882 windmill_api-1.89.0/windmill_api/models/invite_user_json_body.py
+-rw-r--r--   0        0        0     1679 2023-04-23 15:07:37.268882 windmill_api-1.89.0/windmill_api/models/javascript_transform.py
+-rw-r--r--   0        0        0      158 2023-04-23 15:07:18.016690 windmill_api-1.89.0/windmill_api/models/javascript_transform_type.py
+-rw-r--r--   0        0        0     1686 2023-04-23 15:07:37.248882 windmill_api-1.89.0/windmill_api/models/job.py
+-rw-r--r--   0        0        0      174 2023-04-23 15:07:17.040680 windmill_api-1.89.0/windmill_api/models/job_type.py
+-rw-r--r--   0        0        0     3583 2023-04-23 15:07:37.384883 windmill_api-1.89.0/windmill_api/models/list_apps_response_200_item.py
+-rw-r--r--   0        0        0      219 2023-04-23 15:07:16.716677 windmill_api-1.89.0/windmill_api/models/list_apps_response_200_item_execution_mode.py
+-rw-r--r--   0        0        0     1276 2023-04-23 15:07:37.296882 windmill_api-1.89.0/windmill_api/models/list_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      218 2023-04-23 15:07:16.904678 windmill_api-1.89.0/windmill_api/models/list_audit_logs_action_kind.py
+-rw-r--r--   0        0        0     3896 2023-04-23 15:07:37.368883 windmill_api-1.89.0/windmill_api/models/list_audit_logs_response_200_item.py
+-rw-r--r--   0        0        0      237 2023-04-23 15:07:17.572686 windmill_api-1.89.0/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
+-rw-r--r--   0        0        0      640 2023-04-23 15:07:17.560685 windmill_api-1.89.0/windmill_api/models/list_audit_logs_response_200_item_operation.py
+-rw-r--r--   0        0        0     1298 2023-04-23 15:07:37.404884 windmill_api-1.89.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py
+-rw-r--r--   0        0        0    11220 2023-04-23 15:07:37.572885 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item.py
+-rw-r--r--   0        0        0     1288 2023-04-23 15:07:37.432884 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_args.py
+-rw-r--r--   0        0        0     3736 2023-04-23 15:07:37.488885 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7579 2023-04-23 15:07:37.608886 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1901 2023-04-23 15:07:37.608886 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2352 2023-04-23 15:07:37.648886 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      222 2023-04-23 15:07:16.772677 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1806 2023-04-23 15:07:37.648886 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2342 2023-04-23 15:07:37.696887 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      380 2023-04-23 15:07:16.964679 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7160 2023-04-23 15:07:37.808888 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1891 2023-04-23 15:07:37.728887 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2332 2023-04-23 15:07:37.764887 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      220 2023-04-23 15:07:17.368683 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1796 2023-04-23 15:07:37.800887 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2332 2023-04-23 15:07:37.912889 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      378 2023-04-23 15:07:17.984690 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2152 2023-04-23 15:07:37.856888 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      330 2023-04-23 15:07:16.532675 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      219 2023-04-23 15:07:16.972679 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_language.py
+-rw-r--r--   0        0        0     3485 2023-04-23 15:07:37.920889 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7593 2023-04-23 15:07:38.024890 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3498 2023-04-23 15:07:37.972889 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2041 2023-04-23 15:07:38.012890 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2345 2023-04-23 15:07:38.060890 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2295 2023-04-23 15:07:38.064890 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      201 2023-04-23 15:07:17.816688 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2162 2023-04-23 15:07:38.100890 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      201 2023-04-23 15:07:17.084680 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2034 2023-04-23 15:07:38.108891 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2085 2023-04-23 15:07:38.144891 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7471 2023-04-23 15:07:38.220892 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3464 2023-04-23 15:07:38.208892 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2031 2023-04-23 15:07:38.252892 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2335 2023-04-23 15:07:38.264892 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2275 2023-04-23 15:07:38.328893 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      199 2023-04-23 15:07:17.412684 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2142 2023-04-23 15:07:38.304893 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      199 2023-04-23 15:07:17.552685 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2024 2023-04-23 15:07:38.344893 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2075 2023-04-23 15:07:38.368893 windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1865 2023-04-23 15:07:38.436894 windmill_api-1.89.0/windmill_api/models/list_contextual_variables_response_200_item.py
+-rw-r--r--   0        0        0     5077 2023-04-23 15:07:38.452894 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item.py
+-rw-r--r--   0        0        0     1278 2023-04-23 15:07:38.464894 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     1255 2023-04-23 15:07:38.480894 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_schema.py
+-rw-r--r--   0        0        0     3297 2023-04-23 15:07:38.516895 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value.py
+-rw-r--r--   0        0        0     7151 2023-04-23 15:07:38.592896 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py
+-rw-r--r--   0        0        0     3318 2023-04-23 15:07:38.572895 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1985 2023-04-23 15:07:38.612896 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2289 2023-04-23 15:07:38.636896 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2187 2023-04-23 15:07:38.652896 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-04-23 15:07:16.416673 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2054 2023-04-23 15:07:38.676896 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-04-23 15:07:16.848678 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1978 2023-04-23 15:07:38.688897 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2029 2023-04-23 15:07:38.712897 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7049 2023-04-23 15:07:38.800898 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py
+-rw-r--r--   0        0        0     3284 2023-04-23 15:07:38.768897 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1975 2023-04-23 15:07:38.848898 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-04-23 15:07:38.848898 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-04-23 15:07:38.888898 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-04-23 15:07:17.668686 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-04-23 15:07:38.892899 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-04-23 15:07:17.840688 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-04-23 15:07:38.928899 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-04-23 15:07:38.996900 windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2074 2023-04-23 15:07:38.968899 windmill_api-1.89.0/windmill_api/models/list_folders_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-04-23 15:07:38.996900 windmill_api-1.89.0/windmill_api/models/list_folders_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2958 2023-04-23 15:07:39.064900 windmill_api-1.89.0/windmill_api/models/list_groups_response_200_item.py
+-rw-r--r--   0        0        0     1286 2023-04-23 15:07:39.024900 windmill_api-1.89.0/windmill_api/models/list_groups_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2076 2023-04-23 15:07:39.072900 windmill_api-1.89.0/windmill_api/models/list_hub_apps_response_200.py
+-rw-r--r--   0        0        0     2304 2023-04-23 15:07:39.120901 windmill_api-1.89.0/windmill_api/models/list_hub_apps_response_200_apps_item.py
+-rw-r--r--   0        0        0     2116 2023-04-23 15:07:39.112901 windmill_api-1.89.0/windmill_api/models/list_hub_flows_response_200.py
+-rw-r--r--   0        0        0     2324 2023-04-23 15:07:39.164901 windmill_api-1.89.0/windmill_api/models/list_hub_flows_response_200_flows_item.py
+-rw-r--r--   0        0        0     2106 2023-04-23 15:07:39.160901 windmill_api-1.89.0/windmill_api/models/list_hub_scripts_response_200.py
+-rw-r--r--   0        0        0     2790 2023-04-23 15:07:39.220902 windmill_api-1.89.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py
+-rw-r--r--   0        0        0      262 2023-04-23 15:07:17.284682 windmill_api-1.89.0/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
+-rw-r--r--   0        0        0     2590 2023-04-23 15:07:39.220902 windmill_api-1.89.0/windmill_api/models/list_inputs_response_200_item.py
+-rw-r--r--   0        0        0     1250 2023-04-23 15:07:39.244902 windmill_api-1.89.0/windmill_api/models/list_inputs_response_200_item_args.py
+-rw-r--r--   0        0        0      213 2023-04-23 15:07:16.628676 windmill_api-1.89.0/windmill_api/models/list_inputs_runnable_type.py
+-rw-r--r--   0        0        0     1922 2023-04-23 15:07:39.268902 windmill_api-1.89.0/windmill_api/models/list_jobs_response_200_item.py
+-rw-r--r--   0        0        0      194 2023-04-23 15:07:16.732677 windmill_api-1.89.0/windmill_api/models/list_jobs_response_200_item_type.py
+-rw-r--r--   0        0        0     2076 2023-04-23 15:07:39.288903 windmill_api-1.89.0/windmill_api/models/list_pending_invites_response_200_item.py
+-rw-r--r--   0        0        0    12114 2023-04-23 15:07:39.488905 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item.py
+-rw-r--r--   0        0        0     1245 2023-04-23 15:07:39.316903 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_args.py
+-rw-r--r--   0        0        0     3544 2023-04-23 15:07:39.372903 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7247 2023-04-23 15:07:39.524905 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1858 2023-04-23 15:07:39.612906 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-04-23 15:07:39.564905 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-04-23 15:07:17.708687 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-04-23 15:07:39.604906 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2299 2023-04-23 15:07:39.652906 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      372 2023-04-23 15:07:16.724677 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6858 2023-04-23 15:07:39.736907 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1848 2023-04-23 15:07:39.692906 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2248 2023-04-23 15:07:39.728907 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      212 2023-04-23 15:07:16.732677 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1753 2023-04-23 15:07:39.768907 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2289 2023-04-23 15:07:39.812908 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      370 2023-04-23 15:07:17.724687 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2109 2023-04-23 15:07:39.812908 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      322 2023-04-23 15:07:16.400673 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      211 2023-04-23 15:07:17.336683 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_language.py
+-rw-r--r--   0        0        0     3334 2023-04-23 15:07:39.872908 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7235 2023-04-23 15:07:39.948909 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3357 2023-04-23 15:07:39.928909 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1998 2023-04-23 15:07:40.008910 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-04-23 15:07:39.996909 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-04-23 15:07:40.040910 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-23 15:07:17.284682 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-04-23 15:07:40.048910 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-23 15:07:17.628686 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-04-23 15:07:40.084910 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-04-23 15:07:40.088910 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7159 2023-04-23 15:07:40.268912 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3323 2023-04-23 15:07:40.140911 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1988 2023-04-23 15:07:40.188912 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-04-23 15:07:40.232912 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-04-23 15:07:40.272912 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-04-23 15:07:16.396673 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-04-23 15:07:40.308913 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-04-23 15:07:17.032680 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-04-23 15:07:40.312913 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-04-23 15:07:40.352913 windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     4884 2023-04-23 15:07:40.400914 windmill_api-1.89.0/windmill_api/models/list_resource_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-04-23 15:07:40.380913 windmill_api-1.89.0/windmill_api/models/list_resource_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2363 2023-04-23 15:07:40.428914 windmill_api-1.89.0/windmill_api/models/list_resource_type_response_200_item.py
+-rw-r--r--   0        0        0     4426 2023-04-23 15:07:40.512915 windmill_api-1.89.0/windmill_api/models/list_schedules_response_200_item.py
+-rw-r--r--   0        0        0     1265 2023-04-23 15:07:40.452914 windmill_api-1.89.0/windmill_api/models/list_schedules_response_200_item_args.py
+-rw-r--r--   0        0        0     1301 2023-04-23 15:07:40.480914 windmill_api-1.89.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     6980 2023-04-23 15:07:40.600916 windmill_api-1.89.0/windmill_api/models/list_scripts_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-04-23 15:07:40.540915 windmill_api-1.89.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-04-23 15:07:17.532685 windmill_api-1.89.0/windmill_api/models/list_scripts_response_200_item_kind.py
+-rw-r--r--   0        0        0      213 2023-04-23 15:07:16.656676 windmill_api-1.89.0/windmill_api/models/list_scripts_response_200_item_language.py
+-rw-r--r--   0        0        0     1265 2023-04-23 15:07:40.572915 windmill_api-1.89.0/windmill_api/models/list_scripts_response_200_item_schema.py
+-rw-r--r--   0        0        0     2985 2023-04-23 15:07:40.628916 windmill_api-1.89.0/windmill_api/models/list_tokens_response_200_item.py
+-rw-r--r--   0        0        0     2250 2023-04-23 15:07:40.640916 windmill_api-1.89.0/windmill_api/models/list_user_workspaces_response_200.py
+-rw-r--r--   0        0        0     1833 2023-04-23 15:07:40.668916 windmill_api-1.89.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
+-rw-r--r--   0        0        0     2896 2023-04-23 15:07:40.696916 windmill_api-1.89.0/windmill_api/models/list_users_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0      198 2023-04-23 15:07:17.112681 windmill_api-1.89.0/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
+-rw-r--r--   0        0        0     4307 2023-04-23 15:07:40.752917 windmill_api-1.89.0/windmill_api/models/list_users_response_200_item.py
+-rw-r--r--   0        0        0     1613 2023-04-23 15:07:40.728917 windmill_api-1.89.0/windmill_api/models/list_users_response_200_item_usage.py
+-rw-r--r--   0        0        0     4608 2023-04-23 15:07:40.888918 windmill_api-1.89.0/windmill_api/models/list_variable_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-04-23 15:07:40.780917 windmill_api-1.89.0/windmill_api/models/list_variable_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2693 2023-04-23 15:07:40.828918 windmill_api-1.89.0/windmill_api/models/list_workers_response_200_item.py
+-rw-r--r--   0        0        0     2086 2023-04-23 15:07:40.872918 windmill_api-1.89.0/windmill_api/models/list_workspace_invites_response_200_item.py
+-rw-r--r--   0        0        0     2082 2023-04-23 15:07:40.916919 windmill_api-1.89.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0     2013 2023-04-23 15:07:40.928919 windmill_api-1.89.0/windmill_api/models/list_workspaces_response_200_item.py
+-rw-r--r--   0        0        0     3388 2023-04-23 15:07:40.976919 windmill_api-1.89.0/windmill_api/models/listable_app.py
+-rw-r--r--   0        0        0      207 2023-04-23 15:07:16.400673 windmill_api-1.89.0/windmill_api/models/listable_app_execution_mode.py
+-rw-r--r--   0        0        0     1207 2023-04-23 15:07:40.956919 windmill_api-1.89.0/windmill_api/models/listable_app_extra_perms.py
+-rw-r--r--   0        0        0     4751 2023-04-23 15:07:41.044920 windmill_api-1.89.0/windmill_api/models/listable_resource.py
+-rw-r--r--   0        0        0     1232 2023-04-23 15:07:41.008920 windmill_api-1.89.0/windmill_api/models/listable_resource_extra_perms.py
+-rw-r--r--   0        0        0     4486 2023-04-23 15:07:41.132921 windmill_api-1.89.0/windmill_api/models/listable_variable.py
+-rw-r--r--   0        0        0     1232 2023-04-23 15:07:41.076920 windmill_api-1.89.0/windmill_api/models/listable_variable_extra_perms.py
+-rw-r--r--   0        0        0     1513 2023-04-23 15:07:41.112921 windmill_api-1.89.0/windmill_api/models/login.py
+-rw-r--r--   0        0        0     1559 2023-04-23 15:07:41.148921 windmill_api-1.89.0/windmill_api/models/login_json_body.py
+-rw-r--r--   0        0        0     1739 2023-04-23 15:07:41.168921 windmill_api-1.89.0/windmill_api/models/login_with_oauth_json_body.py
+-rw-r--r--   0        0        0     2758 2023-04-23 15:07:41.204922 windmill_api-1.89.0/windmill_api/models/main_arg_signature.py
+-rw-r--r--   0        0        0     5099 2023-04-23 15:07:41.252922 windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item.py
+-rw-r--r--   0        0        0      315 2023-04-23 15:07:17.872689 windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1547 2023-04-23 15:07:41.240922 windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1612 2023-04-23 15:07:41.276922 windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2044 2023-04-23 15:07:41.296923 windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3049 2023-04-23 15:07:41.328923 windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      333 2023-04-23 15:07:16.496674 windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1580 2023-04-23 15:07:41.332923 windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     2862 2023-04-23 15:07:41.376923 windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      324 2023-04-23 15:07:17.736687 windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1529 2023-04-23 15:07:41.364923 windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      169 2023-04-23 15:07:17.924689 windmill_api-1.89.0/windmill_api/models/main_arg_signature_type.py
+-rw-r--r--   0        0        0     2662 2023-04-23 15:07:41.420924 windmill_api-1.89.0/windmill_api/models/new_schedule.py
+-rw-r--r--   0        0        0     1171 2023-04-23 15:07:41.404924 windmill_api-1.89.0/windmill_api/models/new_schedule_args.py
+-rw-r--r--   0        0        0     2108 2023-04-23 15:07:41.448924 windmill_api-1.89.0/windmill_api/models/new_token.py
+-rw-r--r--   0        0        0     2473 2023-04-23 15:07:41.468924 windmill_api-1.89.0/windmill_api/models/new_token_impersonate.py
+-rw-r--r--   0        0        0     1710 2023-04-23 15:07:41.488924 windmill_api-1.89.0/windmill_api/models/new_user.py
+-rw-r--r--   0        0        0     2584 2023-04-23 15:07:41.536925 windmill_api-1.89.0/windmill_api/models/open_flow.py
+-rw-r--r--   0        0        0     1166 2023-04-23 15:07:41.516925 windmill_api-1.89.0/windmill_api/models/open_flow_schema.py
+-rw-r--r--   0        0        0     3026 2023-04-23 15:07:41.576925 windmill_api-1.89.0/windmill_api/models/open_flow_value.py
+-rw-r--r--   0        0        0     6384 2023-04-23 15:07:41.700927 windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3013 2023-04-23 15:07:41.716927 windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1896 2023-04-23 15:07:41.740927 windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2200 2023-04-23 15:07:41.764927 windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2006 2023-04-23 15:07:41.780927 windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      175 2023-04-23 15:07:17.304683 windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1873 2023-04-23 15:07:41.804927 windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      175 2023-04-23 15:07:17.768688 windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1889 2023-04-23 15:07:41.816928 windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1940 2023-04-23 15:07:41.848928 windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6308 2023-04-23 15:07:41.924929 windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item.py
+-rw-r--r--   0        0        0     2979 2023-04-23 15:07:41.904929 windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1886 2023-04-23 15:07:41.948929 windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2190 2023-04-23 15:07:41.968929 windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1986 2023-04-23 15:07:41.992929 windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      173 2023-04-23 15:07:16.944679 windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1853 2023-04-23 15:07:42.004930 windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      173 2023-04-23 15:07:17.976690 windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1879 2023-04-23 15:07:42.040930 windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1930 2023-04-23 15:07:42.044930 windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2816 2023-04-23 15:07:42.096930 windmill_api-1.89.0/windmill_api/models/open_flow_w_path.py
+-rw-r--r--   0        0        0     1197 2023-04-23 15:07:42.072930 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_schema.py
+-rw-r--r--   0        0        0     3116 2023-04-23 15:07:42.128931 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value.py
+-rw-r--r--   0        0        0     6590 2023-04-23 15:07:42.212932 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module.py
+-rw-r--r--   0        0        0     3117 2023-04-23 15:07:42.232932 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1927 2023-04-23 15:07:42.252932 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2231 2023-04-23 15:07:42.276932 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2073 2023-04-23 15:07:42.376933 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      180 2023-04-23 15:07:17.368683 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1940 2023-04-23 15:07:42.316933 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      180 2023-04-23 15:07:16.780677 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1920 2023-04-23 15:07:42.356933 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1971 2023-04-23 15:07:42.400934 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6514 2023-04-23 15:07:42.496935 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item.py
+-rw-r--r--   0        0        0     3074 2023-04-23 15:07:42.452934 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1917 2023-04-23 15:07:42.492934 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2221 2023-04-23 15:07:42.536935 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2044 2023-04-23 15:07:42.544935 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-04-23 15:07:17.776688 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1911 2023-04-23 15:07:42.576935 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-23 15:07:16.468674 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1910 2023-04-23 15:07:42.584935 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1961 2023-04-23 15:07:42.616936 windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1989 2023-04-23 15:07:42.628936 windmill_api-1.89.0/windmill_api/models/path_flow.py
+-rw-r--r--   0        0        0     3089 2023-04-23 15:07:42.664936 windmill_api-1.89.0/windmill_api/models/path_flow_input_transforms.py
+-rw-r--r--   0        0        0     2115 2023-04-23 15:07:42.672936 windmill_api-1.89.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      185 2023-04-23 15:07:17.448684 windmill_api-1.89.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1982 2023-04-23 15:07:42.756937 windmill_api-1.89.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      185 2023-04-23 15:07:17.348683 windmill_api-1.89.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      135 2023-04-23 15:07:16.888678 windmill_api-1.89.0/windmill_api/models/path_flow_type.py
+-rw-r--r--   0        0        0     2292 2023-04-23 15:07:42.724937 windmill_api-1.89.0/windmill_api/models/path_script.py
+-rw-r--r--   0        0        0     3181 2023-04-23 15:07:42.780937 windmill_api-1.89.0/windmill_api/models/path_script_input_transforms.py
+-rw-r--r--   0        0        0     2135 2023-04-23 15:07:42.796938 windmill_api-1.89.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      187 2023-04-23 15:07:16.848678 windmill_api-1.89.0/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2002 2023-04-23 15:07:42.820938 windmill_api-1.89.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      187 2023-04-23 15:07:16.612676 windmill_api-1.89.0/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      141 2023-04-23 15:07:16.956679 windmill_api-1.89.0/windmill_api/models/path_script_type.py
+-rw-r--r--   0        0        0     3390 2023-04-23 15:07:42.864938 windmill_api-1.89.0/windmill_api/models/policy.py
+-rw-r--r--   0        0        0      202 2023-04-23 15:07:17.036680 windmill_api-1.89.0/windmill_api/models/policy_execution_mode.py
+-rw-r--r--   0        0        0     1709 2023-04-23 15:07:42.856938 windmill_api-1.89.0/windmill_api/models/policy_triggerables.py
+-rw-r--r--   0        0        0     1279 2023-04-23 15:07:42.888938 windmill_api-1.89.0/windmill_api/models/policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2359 2023-04-23 15:07:42.916939 windmill_api-1.89.0/windmill_api/models/preview.py
+-rw-r--r--   0        0        0     1148 2023-04-23 15:07:42.912939 windmill_api-1.89.0/windmill_api/models/preview_args.py
+-rw-r--r--   0        0        0      194 2023-04-23 15:07:16.752677 windmill_api-1.89.0/windmill_api/models/preview_language.py
+-rw-r--r--   0        0        0     1642 2023-04-23 15:07:42.948939 windmill_api-1.89.0/windmill_api/models/preview_schedule_json_body.py
+-rw-r--r--   0        0        0     2963 2023-04-23 15:07:42.968939 windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5679 2023-04-23 15:07:43.032940 windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      328 2023-04-23 15:07:17.788688 windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1618 2023-04-23 15:07:43.004939 windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1683 2023-04-23 15:07:43.036940 windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2191 2023-04-23 15:07:43.072940 windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3329 2023-04-23 15:07:43.088940 windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      346 2023-04-23 15:07:16.832678 windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1651 2023-04-23 15:07:43.104941 windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3214 2023-04-23 15:07:43.140941 windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      337 2023-04-23 15:07:16.396673 windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1600 2023-04-23 15:07:43.212942 windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      182 2023-04-23 15:07:17.676687 windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0    11580 2023-04-23 15:07:43.396943 windmill_api-1.89.0/windmill_api/models/queued_job.py
+-rw-r--r--   0        0        0     1161 2023-04-23 15:07:43.240942 windmill_api-1.89.0/windmill_api/models/queued_job_args.py
+-rw-r--r--   0        0        0     3202 2023-04-23 15:07:43.304942 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status.py
+-rw-r--r--   0        0        0     6683 2023-04-23 15:07:43.424944 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1774 2023-04-23 15:07:43.432944 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2106 2023-04-23 15:07:43.468944 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      199 2023-04-23 15:07:17.028680 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1679 2023-04-23 15:07:43.468944 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2215 2023-04-23 15:07:43.516945 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      357 2023-04-23 15:07:16.992679 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6294 2023-04-23 15:07:43.580945 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1764 2023-04-23 15:07:43.548945 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2086 2023-04-23 15:07:43.588945 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      197 2023-04-23 15:07:17.136681 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1669 2023-04-23 15:07:43.620946 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2205 2023-04-23 15:07:43.640946 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      355 2023-04-23 15:07:17.044680 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2025 2023-04-23 15:07:43.664946 windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_retry.py
+-rw-r--r--   0        0        0      307 2023-04-23 15:07:16.388673 windmill_api-1.89.0/windmill_api/models/queued_job_job_kind.py
+-rw-r--r--   0        0        0      196 2023-04-23 15:07:17.764687 windmill_api-1.89.0/windmill_api/models/queued_job_language.py
+-rw-r--r--   0        0        0     3079 2023-04-23 15:07:43.700946 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow.py
+-rw-r--r--   0        0        0     6506 2023-04-23 15:07:43.884948 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3069 2023-04-23 15:07:43.824948 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1914 2023-04-23 15:07:43.864948 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2218 2023-04-23 15:07:43.908949 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2040 2023-04-23 15:07:43.924949 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-04-23 15:07:17.224682 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1907 2023-04-23 15:07:43.944949 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-23 15:07:17.252682 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1907 2023-04-23 15:07:43.964949 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1958 2023-04-23 15:07:43.984949 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6430 2023-04-23 15:07:44.072950 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3035 2023-04-23 15:07:44.044950 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1904 2023-04-23 15:07:44.080950 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2208 2023-04-23 15:07:44.112951 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2020 2023-04-23 15:07:44.120951 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-04-23 15:07:17.144681 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1887 2023-04-23 15:07:44.152951 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-04-23 15:07:16.564675 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1897 2023-04-23 15:07:44.160951 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1948 2023-04-23 15:07:44.192951 windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     3028 2023-04-23 15:07:44.224952 windmill_api-1.89.0/windmill_api/models/raw_script.py
+-rw-r--r--   0        0        0     3139 2023-04-23 15:07:44.244952 windmill_api-1.89.0/windmill_api/models/raw_script_input_transforms.py
+-rw-r--r--   0        0        0     2125 2023-04-23 15:07:44.264952 windmill_api-1.89.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      186 2023-04-23 15:07:16.508674 windmill_api-1.89.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1992 2023-04-23 15:07:44.288952 windmill_api-1.89.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      186 2023-04-23 15:07:17.984690 windmill_api-1.89.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      196 2023-04-23 15:07:16.708676 windmill_api-1.89.0/windmill_api/models/raw_script_language.py
+-rw-r--r--   0        0        0      146 2023-04-23 15:07:17.652686 windmill_api-1.89.0/windmill_api/models/raw_script_type.py
+-rw-r--r--   0        0        0     1405 2023-04-23 15:07:44.304952 windmill_api-1.89.0/windmill_api/models/refresh_token_json_body.py
+-rw-r--r--   0        0        0     1448 2023-04-23 15:07:44.316953 windmill_api-1.89.0/windmill_api/models/remove_granular_acls_json_body.py
+-rw-r--r--   0        0        0      304 2023-04-23 15:07:17.916689 windmill_api-1.89.0/windmill_api/models/remove_granular_acls_kind.py
+-rw-r--r--   0        0        0     1544 2023-04-23 15:07:44.340953 windmill_api-1.89.0/windmill_api/models/remove_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1567 2023-04-23 15:07:44.352953 windmill_api-1.89.0/windmill_api/models/remove_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3367 2023-04-23 15:07:44.460954 windmill_api-1.89.0/windmill_api/models/resource.py
+-rw-r--r--   0        0        0     1189 2023-04-23 15:07:44.380953 windmill_api-1.89.0/windmill_api/models/resource_extra_perms.py
+-rw-r--r--   0        0        0     2256 2023-04-23 15:07:44.428954 windmill_api-1.89.0/windmill_api/models/resource_type.py
+-rw-r--r--   0        0        0     1278 2023-04-23 15:07:44.456954 windmill_api-1.89.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
+-rw-r--r--   0        0        0     1255 2023-04-23 15:07:44.484954 windmill_api-1.89.0/windmill_api/models/resume_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0     2546 2023-04-23 15:07:44.512955 windmill_api-1.89.0/windmill_api/models/retry.py
+-rw-r--r--   0        0        0     1751 2023-04-23 15:07:44.524955 windmill_api-1.89.0/windmill_api/models/retry_constant.py
+-rw-r--r--   0        0        0     2055 2023-04-23 15:07:44.556955 windmill_api-1.89.0/windmill_api/models/retry_exponential.py
+-rw-r--r--   0        0        0     1210 2023-04-23 15:07:44.548955 windmill_api-1.89.0/windmill_api/models/run_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     2189 2023-04-23 15:07:44.592955 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body.py
+-rw-r--r--   0        0        0     1235 2023-04-23 15:07:44.584955 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_args.py
+-rw-r--r--   0        0        0     3265 2023-04-23 15:07:44.640956 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value.py
+-rw-r--r--   0        0        0     7049 2023-04-23 15:07:44.828958 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3284 2023-04-23 15:07:44.696956 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1975 2023-04-23 15:07:44.736957 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-04-23 15:07:44.780957 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-04-23 15:07:44.824958 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-04-23 15:07:17.588686 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-04-23 15:07:44.864958 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-04-23 15:07:17.156681 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-04-23 15:07:44.872958 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-04-23 15:07:44.904958 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6939 2023-04-23 15:07:44.984959 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3250 2023-04-23 15:07:44.960959 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1965 2023-04-23 15:07:45.000959 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2269 2023-04-23 15:07:45.028960 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2147 2023-04-23 15:07:45.040960 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      187 2023-04-23 15:07:16.628676 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2014 2023-04-23 15:07:45.068960 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      187 2023-04-23 15:07:17.764687 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1958 2023-04-23 15:07:45.076960 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2009 2023-04-23 15:07:45.112960 windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1220 2023-04-23 15:07:45.104961 windmill_api-1.89.0/windmill_api/models/run_script_by_hash_json_body.py
+-rw-r--r--   0        0        0     1220 2023-04-23 15:07:45.128961 windmill_api-1.89.0/windmill_api/models/run_script_by_path_json_body.py
+-rw-r--r--   0        0        0     2634 2023-04-23 15:07:45.168961 windmill_api-1.89.0/windmill_api/models/run_script_preview_json_body.py
+-rw-r--r--   0        0        0     1245 2023-04-23 15:07:45.156961 windmill_api-1.89.0/windmill_api/models/run_script_preview_json_body_args.py
+-rw-r--r--   0        0        0      211 2023-04-23 15:07:16.960679 windmill_api-1.89.0/windmill_api/models/run_script_preview_json_body_language.py
+-rw-r--r--   0        0        0     1266 2023-04-23 15:07:45.184961 windmill_api-1.89.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     1276 2023-04-23 15:07:45.196961 windmill_api-1.89.0/windmill_api/models/run_wait_result_script_by_path_json_body.py
+-rw-r--r--   0        0        0      203 2023-04-23 15:07:16.700676 windmill_api-1.89.0/windmill_api/models/runnable_type.py
+-rw-r--r--   0        0        0     4086 2023-04-23 15:07:45.312962 windmill_api-1.89.0/windmill_api/models/schedule.py
+-rw-r--r--   0        0        0     1153 2023-04-23 15:07:45.228962 windmill_api-1.89.0/windmill_api/models/schedule_args.py
+-rw-r--r--   0        0        0     1189 2023-04-23 15:07:45.256962 windmill_api-1.89.0/windmill_api/models/schedule_extra_perms.py
+-rw-r--r--   0        0        0     6432 2023-04-23 15:07:45.496964 windmill_api-1.89.0/windmill_api/models/script.py
+-rw-r--r--   0        0        0     1143 2023-04-23 15:07:45.340963 windmill_api-1.89.0/windmill_api/models/script_args.py
+-rw-r--r--   0        0        0     1179 2023-04-23 15:07:45.372963 windmill_api-1.89.0/windmill_api/models/script_extra_perms.py
+-rw-r--r--   0        0        0      235 2023-04-23 15:07:16.624676 windmill_api-1.89.0/windmill_api/models/script_kind.py
+-rw-r--r--   0        0        0      193 2023-04-23 15:07:17.096680 windmill_api-1.89.0/windmill_api/models/script_language.py
+-rw-r--r--   0        0        0     1153 2023-04-23 15:07:45.408964 windmill_api-1.89.0/windmill_api/models/script_schema.py
+-rw-r--r--   0        0        0     1440 2023-04-23 15:07:45.436964 windmill_api-1.89.0/windmill_api/models/set_password_json_body.py
+-rw-r--r--   0        0        0     1470 2023-04-23 15:07:45.468964 windmill_api-1.89.0/windmill_api/models/set_schedule_enabled_json_body.py
+-rw-r--r--   0        0        0     2032 2023-04-23 15:07:45.512965 windmill_api-1.89.0/windmill_api/models/slack_token.py
+-rw-r--r--   0        0        0     1586 2023-04-23 15:07:45.528965 windmill_api-1.89.0/windmill_api/models/slack_token_bot.py
+-rw-r--r--   0        0        0     2227 2023-04-23 15:07:45.556965 windmill_api-1.89.0/windmill_api/models/star_json_body.py
+-rw-r--r--   0        0        0      185 2023-04-23 15:07:17.348683 windmill_api-1.89.0/windmill_api/models/star_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     1772 2023-04-23 15:07:45.568965 windmill_api-1.89.0/windmill_api/models/static_transform.py
+-rw-r--r--   0        0        0      154 2023-04-23 15:07:16.420673 windmill_api-1.89.0/windmill_api/models/static_transform_type.py
+-rw-r--r--   0        0        0     2462 2023-04-23 15:07:45.612965 windmill_api-1.89.0/windmill_api/models/token_response.py
+-rw-r--r--   0        0        0     2921 2023-04-23 15:07:45.624966 windmill_api-1.89.0/windmill_api/models/truncated_token.py
+-rw-r--r--   0        0        0     2249 2023-04-23 15:07:45.656966 windmill_api-1.89.0/windmill_api/models/unstar_json_body.py
+-rw-r--r--   0        0        0      187 2023-04-23 15:07:16.904678 windmill_api-1.89.0/windmill_api/models/unstar_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     2638 2023-04-23 15:07:45.684966 windmill_api-1.89.0/windmill_api/models/update_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-04-23 15:07:45.732967 windmill_api-1.89.0/windmill_api/models/update_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-04-23 15:07:17.004680 windmill_api-1.89.0/windmill_api/models/update_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-04-23 15:07:45.720967 windmill_api-1.89.0/windmill_api/models/update_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-04-23 15:07:45.748967 windmill_api-1.89.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-04-23 15:07:45.796967 windmill_api-1.89.0/windmill_api/models/update_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-04-23 15:07:45.772967 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-04-23 15:07:45.828968 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-04-23 15:07:45.952969 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-04-23 15:07:45.884968 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-04-23 15:07:45.924969 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-04-23 15:07:45.968969 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-04-23 15:07:45.992969 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-04-23 15:07:17.984690 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-04-23 15:07:46.004969 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-04-23 15:07:17.396684 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-04-23 15:07:46.028970 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-04-23 15:07:46.044970 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-04-23 15:07:46.140971 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-04-23 15:07:46.096970 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-04-23 15:07:46.136971 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-04-23 15:07:46.180971 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-04-23 15:07:46.176971 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-04-23 15:07:17.112681 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-04-23 15:07:46.212972 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-04-23 15:07:16.476674 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-04-23 15:07:46.220971 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-04-23 15:07:46.260972 windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1949 2023-04-23 15:07:46.264972 windmill_api-1.89.0/windmill_api/models/update_folder_json_body.py
+-rw-r--r--   0        0        0     1520 2023-04-23 15:07:46.292972 windmill_api-1.89.0/windmill_api/models/update_group_json_body.py
+-rw-r--r--   0        0        0     1670 2023-04-23 15:07:46.300972 windmill_api-1.89.0/windmill_api/models/update_input.py
+-rw-r--r--   0        0        0     1716 2023-04-23 15:07:46.328973 windmill_api-1.89.0/windmill_api/models/update_input_json_body.py
+-rw-r--r--   0        0        0     2036 2023-04-23 15:07:46.348973 windmill_api-1.89.0/windmill_api/models/update_resource_json_body.py
+-rw-r--r--   0        0        0     1847 2023-04-23 15:07:46.420974 windmill_api-1.89.0/windmill_api/models/update_resource_type_json_body.py
+-rw-r--r--   0        0        0     1541 2023-04-23 15:07:46.384973 windmill_api-1.89.0/windmill_api/models/update_resource_value_json_body.py
+-rw-r--r--   0        0        0     1953 2023-04-23 15:07:46.424974 windmill_api-1.89.0/windmill_api/models/update_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-04-23 15:07:46.448974 windmill_api-1.89.0/windmill_api/models/update_schedule_json_body_args.py
+-rw-r--r--   0        0        0     2066 2023-04-23 15:07:46.472974 windmill_api-1.89.0/windmill_api/models/update_user_json_body.py
+-rw-r--r--   0        0        0     2316 2023-04-23 15:07:46.500974 windmill_api-1.89.0/windmill_api/models/update_variable_json_body.py
+-rw-r--r--   0        0        0     1478 2023-04-23 15:07:46.508974 windmill_api-1.89.0/windmill_api/models/usage.py
+-rw-r--r--   0        0        0     4071 2023-04-23 15:07:46.580975 windmill_api-1.89.0/windmill_api/models/user.py
+-rw-r--r--   0        0        0     1501 2023-04-23 15:07:46.540975 windmill_api-1.89.0/windmill_api/models/user_usage.py
+-rw-r--r--   0        0        0     2122 2023-04-23 15:07:46.580975 windmill_api-1.89.0/windmill_api/models/user_workspace_list.py
+-rw-r--r--   0        0        0     1767 2023-04-23 15:07:46.620975 windmill_api-1.89.0/windmill_api/models/user_workspace_list_workspaces_item.py
+-rw-r--r--   0        0        0     4222 2023-04-23 15:07:46.772976 windmill_api-1.89.0/windmill_api/models/whoami_response_200.py
+-rw-r--r--   0        0        0     1572 2023-04-23 15:07:46.652975 windmill_api-1.89.0/windmill_api/models/whoami_response_200_usage.py
+-rw-r--r--   0        0        0     4211 2023-04-23 15:07:46.732976 windmill_api-1.89.0/windmill_api/models/whois_response_200.py
+-rw-r--r--   0        0        0     1567 2023-04-23 15:07:46.764976 windmill_api-1.89.0/windmill_api/models/whois_response_200_usage.py
+-rw-r--r--   0        0        0     2604 2023-04-23 15:07:46.816976 windmill_api-1.89.0/windmill_api/models/worker_ping.py
+-rw-r--r--   0        0        0     1901 2023-04-23 15:07:46.820976 windmill_api-1.89.0/windmill_api/models/workspace.py
+-rw-r--r--   0        0        0     1974 2023-04-23 15:07:46.856976 windmill_api-1.89.0/windmill_api/models/workspace_invite.py
+-rw-r--r--   0        0        0       25 2023-04-23 15:07:04.900570 windmill_api-1.89.0/windmill_api/py.typed
+-rw-r--r--   0        0        0      939 2023-04-23 15:07:46.836976 windmill_api-1.89.0/windmill_api/types.py
+-rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 windmill_api-1.89.0/setup.py
+-rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.89.0/PKG-INFO
```

### Comparing `windmill_api-1.88.1/LICENSE` & `windmill_api-1.89.0/LICENSE`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/README.md` & `windmill_api-1.89.0/README.md`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/pyproject.toml` & `windmill_api-1.89.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "windmill-api"
-version = "1.88.1"
+version = "1.89.0"
 description = "A client library for accessing Windmill API"
 license = "Apache-2.0"
 
 authors = ["Ruben Fiszel <ruben@windmill.dev>"]
 
 readme = "README.md"
 packages = [
```

### Comparing `windmill_api-1.88.1/windmill_api/api/app/create_app.py` & `windmill_api-1.89.0/windmill_api/api/app/create_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/app/delete_app.py` & `windmill_api-1.89.0/windmill_api/api/app/delete_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/app/execute_component.py` & `windmill_api-1.89.0/windmill_api/api/app/execute_component.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/app/exists_app.py` & `windmill_api-1.89.0/windmill_api/api/app/exists_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/app/get_app_by_path.py` & `windmill_api-1.89.0/windmill_api/api/app/get_app_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/app/get_app_by_version.py` & `windmill_api-1.89.0/windmill_api/api/app/get_app_by_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/app/get_hub_app_by_id.py` & `windmill_api-1.89.0/windmill_api/api/app/get_hub_app_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/app/get_public_app_by_secret.py` & `windmill_api-1.89.0/windmill_api/api/app/get_public_app_by_secret.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/app/get_public_secret_of_app.py` & `windmill_api-1.89.0/windmill_api/api/app/get_public_secret_of_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/app/list_apps.py` & `windmill_api-1.89.0/windmill_api/api/app/list_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/app/list_hub_apps.py` & `windmill_api-1.89.0/windmill_api/api/app/list_hub_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/app/update_app.py` & `windmill_api-1.89.0/windmill_api/api/app/update_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/audit/get_audit_log.py` & `windmill_api-1.89.0/windmill_api/api/audit/get_audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/audit/list_audit_logs.py` & `windmill_api-1.89.0/windmill_api/api/audit/list_audit_logs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/capture/create_capture.py` & `windmill_api-1.89.0/windmill_api/api/capture/create_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/capture/get_capture.py` & `windmill_api-1.89.0/windmill_api/api/capture/get_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/capture/update_capture.py` & `windmill_api-1.89.0/windmill_api/api/capture/update_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/favorite/star.py` & `windmill_api-1.89.0/windmill_api/api/favorite/star.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/favorite/unstar.py` & `windmill_api-1.89.0/windmill_api/api/favorite/unstar.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/flow/archive_flow_by_path.py` & `windmill_api-1.89.0/windmill_api/api/flow/archive_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/flow/create_flow.py` & `windmill_api-1.89.0/windmill_api/api/flow/create_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/flow/delete_flow_by_path.py` & `windmill_api-1.89.0/windmill_api/api/flow/delete_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/flow/exists_flow_by_path.py` & `windmill_api-1.89.0/windmill_api/api/flow/exists_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/flow/get_flow_by_path.py` & `windmill_api-1.89.0/windmill_api/api/flow/get_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/flow/get_flow_input_history_by_path.py` & `windmill_api-1.89.0/windmill_api/api/flow/get_flow_input_history_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/flow/get_hub_flow_by_id.py` & `windmill_api-1.89.0/windmill_api/api/flow/get_hub_flow_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/flow/list_flow_paths.py` & `windmill_api-1.89.0/windmill_api/api/flow/list_flow_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/flow/list_flows.py` & `windmill_api-1.89.0/windmill_api/api/flow/list_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/flow/list_hub_flows.py` & `windmill_api-1.89.0/windmill_api/api/flow/list_hub_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/flow/update_flow.py` & `windmill_api-1.89.0/windmill_api/api/flow/update_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/folder/add_owner_to_folder.py` & `windmill_api-1.89.0/windmill_api/api/folder/add_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/folder/create_folder.py` & `windmill_api-1.89.0/windmill_api/api/folder/create_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/folder/delete_folder.py` & `windmill_api-1.89.0/windmill_api/api/folder/delete_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/folder/get_folder.py` & `windmill_api-1.89.0/windmill_api/api/folder/get_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/folder/get_folder_usage.py` & `windmill_api-1.89.0/windmill_api/api/folder/get_folder_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/folder/list_folder_names.py` & `windmill_api-1.89.0/windmill_api/api/folder/list_folder_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/folder/list_folders.py` & `windmill_api-1.89.0/windmill_api/api/folder/list_folders.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/folder/remove_owner_to_folder.py` & `windmill_api-1.89.0/windmill_api/api/folder/remove_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/folder/update_folder.py` & `windmill_api-1.89.0/windmill_api/api/folder/update_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/granular_acl/add_granular_acls.py` & `windmill_api-1.89.0/windmill_api/api/granular_acl/add_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/granular_acl/get_granular_acls.py` & `windmill_api-1.89.0/windmill_api/api/granular_acl/get_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/granular_acl/remove_granular_acls.py` & `windmill_api-1.89.0/windmill_api/api/granular_acl/remove_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/group/add_user_to_group.py` & `windmill_api-1.89.0/windmill_api/api/group/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/group/create_group.py` & `windmill_api-1.89.0/windmill_api/api/group/create_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/group/delete_group.py` & `windmill_api-1.89.0/windmill_api/api/group/delete_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/group/get_group.py` & `windmill_api-1.89.0/windmill_api/api/group/get_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/group/list_group_names.py` & `windmill_api-1.89.0/windmill_api/api/group/list_group_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/group/list_groups.py` & `windmill_api-1.89.0/windmill_api/api/group/list_groups.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/group/remove_user_to_group.py` & `windmill_api-1.89.0/windmill_api/api/group/remove_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/group/update_group.py` & `windmill_api-1.89.0/windmill_api/api/group/update_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/input_/create_input.py` & `windmill_api-1.89.0/windmill_api/api/input_/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/input_/delete_input.py` & `windmill_api-1.89.0/windmill_api/api/input_/delete_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/input_/get_input_history.py` & `windmill_api-1.89.0/windmill_api/api/input_/get_input_history.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/input_/list_inputs.py` & `windmill_api-1.89.0/windmill_api/api/input_/list_inputs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/input_/update_input.py` & `windmill_api-1.89.0/windmill_api/api/input_/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/cancel_queued_job.py` & `windmill_api-1.89.0/windmill_api/api/job/cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/cancel_suspended_job_get.py` & `windmill_api-1.89.0/windmill_api/api/job/cancel_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/cancel_suspended_job_post.py` & `windmill_api-1.89.0/windmill_api/api/job/cancel_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/create_job_signature.py` & `windmill_api-1.89.0/windmill_api/api/job/create_job_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/delete_completed_job.py` & `windmill_api-1.89.0/windmill_api/api/job/delete_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/force_cancel_queued_job.py` & `windmill_api-1.89.0/windmill_api/api/job/force_cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/get_completed_job.py` & `windmill_api-1.89.0/windmill_api/api/job/get_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/get_completed_job_result.py` & `windmill_api-1.89.0/windmill_api/api/job/get_completed_job_result.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/get_job.py` & `windmill_api-1.89.0/windmill_api/api/job/get_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/get_job_updates.py` & `windmill_api-1.89.0/windmill_api/api/job/get_job_updates.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/get_resume_urls.py` & `windmill_api-1.89.0/windmill_api/api/job/get_resume_urls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/get_suspended_job_flow.py` & `windmill_api-1.89.0/windmill_api/api/job/get_suspended_job_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/list_completed_jobs.py` & `windmill_api-1.89.0/windmill_api/api/job/list_completed_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/list_jobs.py` & `windmill_api-1.89.0/windmill_api/api/job/list_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/list_queue.py` & `windmill_api-1.89.0/windmill_api/api/job/list_queue.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/result_by_id.py` & `windmill_api-1.89.0/windmill_api/api/job/result_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/resume_suspended_flow_as_owner.py` & `windmill_api-1.89.0/windmill_api/api/job/resume_suspended_flow_as_owner.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/resume_suspended_job_get.py` & `windmill_api-1.89.0/windmill_api/api/job/resume_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/resume_suspended_job_post.py` & `windmill_api-1.89.0/windmill_api/api/job/resume_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/run_flow_by_path.py` & `windmill_api-1.89.0/windmill_api/api/job/run_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/run_flow_preview.py` & `windmill_api-1.89.0/windmill_api/api/job/run_flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/run_script_by_hash.py` & `windmill_api-1.89.0/windmill_api/api/job/run_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/run_script_by_path.py` & `windmill_api-1.89.0/windmill_api/api/job/run_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/run_script_preview.py` & `windmill_api-1.89.0/windmill_api/api/job/run_script_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/run_wait_result_flow_by_path.py` & `windmill_api-1.89.0/windmill_api/api/job/run_wait_result_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/run_wait_result_script_by_path.py` & `windmill_api-1.89.0/windmill_api/api/job/run_wait_result_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/job/run_wait_result_script_by_path_get.py` & `windmill_api-1.89.0/windmill_api/api/job/run_wait_result_script_by_path_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/oauth/connect_callback.py` & `windmill_api-1.89.0/windmill_api/api/oauth/connect_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/oauth/connect_slack_callback.py` & `windmill_api-1.89.0/windmill_api/api/oauth/connect_slack_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/oauth/create_account.py` & `windmill_api-1.89.0/windmill_api/api/oauth/create_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/oauth/disconnect_account.py` & `windmill_api-1.89.0/windmill_api/api/oauth/disconnect_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/oauth/disconnect_slack.py` & `windmill_api-1.89.0/windmill_api/api/oauth/disconnect_slack.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/oauth/list_o_auth_connects.py` & `windmill_api-1.89.0/windmill_api/api/oauth/list_o_auth_connects.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/oauth/list_o_auth_logins.py` & `windmill_api-1.89.0/windmill_api/api/oauth/list_o_auth_logins.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/oauth/refresh_token.py` & `windmill_api-1.89.0/windmill_api/api/oauth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/create_resource.py` & `windmill_api-1.89.0/windmill_api/api/resource/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/create_resource_type.py` & `windmill_api-1.89.0/windmill_api/api/resource/create_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/delete_resource.py` & `windmill_api-1.89.0/windmill_api/api/resource/delete_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/delete_resource_type.py` & `windmill_api-1.89.0/windmill_api/api/resource/delete_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/exists_resource.py` & `windmill_api-1.89.0/windmill_api/api/resource/exists_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/exists_resource_type.py` & `windmill_api-1.89.0/windmill_api/api/resource/exists_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/get_resource.py` & `windmill_api-1.89.0/windmill_api/api/resource/get_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/get_resource_type.py` & `windmill_api-1.89.0/windmill_api/api/resource/get_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/get_resource_value.py` & `windmill_api-1.89.0/windmill_api/api/resource/get_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/list_resource.py` & `windmill_api-1.89.0/windmill_api/api/resource/list_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/list_resource_type.py` & `windmill_api-1.89.0/windmill_api/api/resource/list_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/list_resource_type_names.py` & `windmill_api-1.89.0/windmill_api/api/resource/list_resource_type_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/update_resource.py` & `windmill_api-1.89.0/windmill_api/api/resource/update_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/update_resource_type.py` & `windmill_api-1.89.0/windmill_api/api/resource/update_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/resource/update_resource_value.py` & `windmill_api-1.89.0/windmill_api/api/resource/update_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/schedule/create_schedule.py` & `windmill_api-1.89.0/windmill_api/api/schedule/create_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/schedule/delete_schedule.py` & `windmill_api-1.89.0/windmill_api/api/schedule/delete_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/schedule/exists_schedule.py` & `windmill_api-1.89.0/windmill_api/api/schedule/exists_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/schedule/get_schedule.py` & `windmill_api-1.89.0/windmill_api/api/schedule/get_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/schedule/list_schedules.py` & `windmill_api-1.89.0/windmill_api/api/schedule/list_schedules.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/schedule/preview_schedule.py` & `windmill_api-1.89.0/windmill_api/api/schedule/preview_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/schedule/set_schedule_enabled.py` & `windmill_api-1.89.0/windmill_api/api/schedule/set_schedule_enabled.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/schedule/update_schedule.py` & `windmill_api-1.89.0/windmill_api/api/schedule/update_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/archive_script_by_hash.py` & `windmill_api-1.89.0/windmill_api/api/script/archive_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/archive_script_by_path.py` & `windmill_api-1.89.0/windmill_api/api/script/archive_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/bash_to_jsonschema.py` & `windmill_api-1.89.0/windmill_api/api/script/bash_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/create_script.py` & `windmill_api-1.89.0/windmill_api/api/script/create_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/delete_script_by_hash.py` & `windmill_api-1.89.0/windmill_api/api/script/delete_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/delete_script_by_path.py` & `windmill_api-1.89.0/windmill_api/api/script/delete_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/deno_to_jsonschema.py` & `windmill_api-1.89.0/windmill_api/api/script/deno_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/exists_script_by_path.py` & `windmill_api-1.89.0/windmill_api/api/script/exists_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/get_hub_script_by_path.py` & `windmill_api-1.89.0/windmill_api/api/script/get_hub_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/get_hub_script_content_by_path.py` & `windmill_api-1.89.0/windmill_api/api/script/get_hub_script_content_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/get_script_by_hash.py` & `windmill_api-1.89.0/windmill_api/api/script/get_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/get_script_by_path.py` & `windmill_api-1.89.0/windmill_api/api/script/get_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/get_script_deployment_status.py` & `windmill_api-1.89.0/windmill_api/api/script/get_script_deployment_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/go_to_jsonschema.py` & `windmill_api-1.89.0/windmill_api/api/script/go_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/list_hub_scripts.py` & `windmill_api-1.89.0/windmill_api/api/script/list_hub_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/list_script_paths.py` & `windmill_api-1.89.0/windmill_api/api/script/list_script_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/list_scripts.py` & `windmill_api-1.89.0/windmill_api/api/script/list_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/python_to_jsonschema.py` & `windmill_api-1.89.0/windmill_api/api/script/python_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/raw_script_by_hash.py` & `windmill_api-1.89.0/windmill_api/api/script/raw_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/raw_script_by_path.py` & `windmill_api-1.89.0/windmill_api/api/script/raw_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/script/raw_script_by_path_tokened.py` & `windmill_api-1.89.0/windmill_api/api/script/raw_script_by_path_tokened.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/settings/backend_version.py` & `windmill_api-1.89.0/windmill_api/api/settings/backend_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/settings/get_open_api_yaml.py` & `windmill_api-1.89.0/windmill_api/api/settings/get_open_api_yaml.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/accept_invite.py` & `windmill_api-1.89.0/windmill_api/api/user/accept_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/create_token.py` & `windmill_api-1.89.0/windmill_api/api/user/create_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/create_token_impersonate.py` & `windmill_api-1.89.0/windmill_api/api/user/create_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/create_user.py` & `windmill_api-1.89.0/windmill_api/api/user/create_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/create_user_globally.py` & `windmill_api-1.89.0/windmill_api/api/user/create_user_globally.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/decline_invite.py` & `windmill_api-1.89.0/windmill_api/api/user/decline_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/delete_token.py` & `windmill_api-1.89.0/windmill_api/api/user/delete_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/delete_user.py` & `windmill_api-1.89.0/windmill_api/api/user/delete_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/get_current_email.py` & `windmill_api-1.89.0/windmill_api/api/user/get_current_email.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/get_usage.py` & `windmill_api-1.89.0/windmill_api/api/user/get_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/global_user_delete.py` & `windmill_api-1.89.0/windmill_api/api/user/global_user_delete.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/global_user_update.py` & `windmill_api-1.89.0/windmill_api/api/user/global_user_update.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/global_whoami.py` & `windmill_api-1.89.0/windmill_api/api/user/global_whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/is_owner_of_path.py` & `windmill_api-1.89.0/windmill_api/api/user/is_owner_of_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/leave_workspace.py` & `windmill_api-1.89.0/windmill_api/api/user/leave_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/list_tokens.py` & `windmill_api-1.89.0/windmill_api/api/user/list_tokens.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/list_usernames.py` & `windmill_api-1.89.0/windmill_api/api/user/list_usernames.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/list_users.py` & `windmill_api-1.89.0/windmill_api/api/user/list_users.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/list_users_as_super_admin.py` & `windmill_api-1.89.0/windmill_api/api/user/list_users_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/list_workspace_invites.py` & `windmill_api-1.89.0/windmill_api/api/user/list_workspace_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/login.py` & `windmill_api-1.89.0/windmill_api/api/user/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/login_with_oauth.py` & `windmill_api-1.89.0/windmill_api/api/user/login_with_oauth.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/logout.py` & `windmill_api-1.89.0/windmill_api/api/user/logout.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/set_password.py` & `windmill_api-1.89.0/windmill_api/api/user/set_password.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/update_user.py` & `windmill_api-1.89.0/windmill_api/api/user/update_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/whoami.py` & `windmill_api-1.89.0/windmill_api/api/user/whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/user/whois.py` & `windmill_api-1.89.0/windmill_api/api/user/whois.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/variable/create_variable.py` & `windmill_api-1.89.0/windmill_api/api/variable/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/variable/delete_variable.py` & `windmill_api-1.89.0/windmill_api/api/variable/delete_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/variable/exists_variable.py` & `windmill_api-1.89.0/windmill_api/api/variable/exists_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/variable/get_variable.py` & `windmill_api-1.89.0/windmill_api/api/variable/get_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/variable/list_contextual_variables.py` & `windmill_api-1.89.0/windmill_api/api/variable/list_contextual_variables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/variable/list_variable.py` & `windmill_api-1.89.0/windmill_api/api/variable/list_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/variable/update_variable.py` & `windmill_api-1.89.0/windmill_api/api/variable/update_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/worker/list_workers.py` & `windmill_api-1.89.0/windmill_api/api/worker/list_workers.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/add_user.py` & `windmill_api-1.89.0/windmill_api/api/workspace/add_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/archive_workspace.py` & `windmill_api-1.89.0/windmill_api/api/workspace/archive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/create_workspace.py` & `windmill_api-1.89.0/windmill_api/api/workspace/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/delete_invite.py` & `windmill_api-1.89.0/windmill_api/api/workspace/delete_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/delete_workspace.py` & `windmill_api-1.89.0/windmill_api/api/workspace/delete_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/edit_auto_invite.py` & `windmill_api-1.89.0/windmill_api/api/workspace/edit_auto_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/edit_slack_command.py` & `windmill_api-1.89.0/windmill_api/api/workspace/edit_slack_command.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/edit_webhook.py` & `windmill_api-1.89.0/windmill_api/api/workspace/edit_webhook.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/exists_username.py` & `windmill_api-1.89.0/windmill_api/api/workspace/exists_username.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/exists_workspace.py` & `windmill_api-1.89.0/windmill_api/api/workspace/exists_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/get_premium_info.py` & `windmill_api-1.89.0/windmill_api/api/workspace/get_premium_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/get_settings.py` & `windmill_api-1.89.0/windmill_api/api/workspace/get_settings.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/invite_user.py` & `windmill_api-1.89.0/windmill_api/api/workspace/invite_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/is_domain_allowed.py` & `windmill_api-1.89.0/windmill_api/api/workspace/is_domain_allowed.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/list_pending_invites.py` & `windmill_api-1.89.0/windmill_api/api/workspace/list_pending_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/list_user_workspaces.py` & `windmill_api-1.89.0/windmill_api/api/workspace/list_user_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/list_workspaces.py` & `windmill_api-1.89.0/windmill_api/api/workspace/list_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/list_workspaces_as_super_admin.py` & `windmill_api-1.89.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/api/workspace/unarchive_workspace.py` & `windmill_api-1.89.0/windmill_api/api/workspace/unarchive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/client.py` & `windmill_api-1.89.0/windmill_api/client.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/accept_invite_json_body.py` & `windmill_api-1.89.0/windmill_api/models/accept_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/add_granular_acls_json_body.py` & `windmill_api-1.89.0/windmill_api/models/add_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/add_owner_to_folder_json_body.py` & `windmill_api-1.89.0/windmill_api/models/add_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/add_user_json_body.py` & `windmill_api-1.89.0/windmill_api/models/add_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/add_user_to_group_json_body.py` & `windmill_api-1.89.0/windmill_api/models/add_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/app_with_last_version.py` & `windmill_api-1.89.0/windmill_api/models/app_with_last_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/app_with_last_version_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/app_with_last_version_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/app_with_last_version_policy.py` & `windmill_api-1.89.0/windmill_api/models/app_with_last_version_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/app_with_last_version_policy_triggerables.py` & `windmill_api-1.89.0/windmill_api/models/app_with_last_version_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py` & `windmill_api-1.89.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/archive_flow_by_path_json_body.py` & `windmill_api-1.89.0/windmill_api/models/archive_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/archive_script_by_hash_response_200.py` & `windmill_api-1.89.0/windmill_api/models/archive_script_by_hash_response_200.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         starred (bool):
         workspace_id (Union[Unset, str]):
         parent_hashes (Union[Unset, List[str]]): The first element is the direct parent of the script, the second is the
             parent of the first, etc
         schema (Union[Unset, ArchiveScriptByHashResponse200Schema]):
         lock (Union[Unset, str]):
         lock_error_logs (Union[Unset, str]):
+        tag (Union[Unset, str]):
     """
 
     hash_: str
     path: str
     summary: str
     description: str
     content: str
@@ -54,14 +55,15 @@
     kind: ArchiveScriptByHashResponse200Kind
     starred: bool
     workspace_id: Union[Unset, str] = UNSET
     parent_hashes: Union[Unset, List[str]] = UNSET
     schema: Union[Unset, ArchiveScriptByHashResponse200Schema] = UNSET
     lock: Union[Unset, str] = UNSET
     lock_error_logs: Union[Unset, str] = UNSET
+    tag: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         hash_ = self.hash_
         path = self.path
         summary = self.summary
         description = self.description
@@ -86,14 +88,15 @@
 
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         lock = self.lock
         lock_error_logs = self.lock_error_logs
+        tag = self.tag
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "hash": hash_,
                 "path": path,
@@ -117,14 +120,16 @@
             field_dict["parent_hashes"] = parent_hashes
         if schema is not UNSET:
             field_dict["schema"] = schema
         if lock is not UNSET:
             field_dict["lock"] = lock
         if lock_error_logs is not UNSET:
             field_dict["lock_error_logs"] = lock_error_logs
+        if tag is not UNSET:
+            field_dict["tag"] = tag
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         hash_ = d.pop("hash")
@@ -166,14 +171,16 @@
         else:
             schema = ArchiveScriptByHashResponse200Schema.from_dict(_schema)
 
         lock = d.pop("lock", UNSET)
 
         lock_error_logs = d.pop("lock_error_logs", UNSET)
 
+        tag = d.pop("tag", UNSET)
+
         archive_script_by_hash_response_200 = cls(
             hash_=hash_,
             path=path,
             summary=summary,
             description=description,
             content=content,
             created_by=created_by,
@@ -186,14 +193,15 @@
             kind=kind,
             starred=starred,
             workspace_id=workspace_id,
             parent_hashes=parent_hashes,
             schema=schema,
             lock=lock,
             lock_error_logs=lock_error_logs,
+            tag=tag,
         )
 
         archive_script_by_hash_response_200.additional_properties = d
         return archive_script_by_hash_response_200
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.88.1/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/archive_script_by_hash_response_200_schema.py` & `windmill_api-1.89.0/windmill_api/models/archive_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/audit_log.py` & `windmill_api-1.89.0/windmill_api/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/audit_log_operation.py` & `windmill_api-1.89.0/windmill_api/models/audit_log_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/audit_log_parameters.py` & `windmill_api-1.89.0/windmill_api/models/audit_log_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200.py` & `windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item.py` & `windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.89.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_all.py` & `windmill_api-1.89.0/windmill_api/models/branch_all.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_all_branches_item.py` & `windmill_api-1.89.0/windmill_api/models/branch_all_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_all_branches_item_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one.py` & `windmill_api-1.89.0/windmill_api/models/branch_one.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_branches_item.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_branches_item_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_default_item.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_default_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_default_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_default_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_default_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_default_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_default_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/branch_one_default_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/branch_one_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/cancel_queued_job_json_body.py` & `windmill_api-1.89.0/windmill_api/models/cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/cancel_suspended_job_post_json_body.py` & `windmill_api-1.89.0/windmill_api/models/cancel_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job.py` & `windmill_api-1.89.0/windmill_api/models/completed_job.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         job_kind (CompletedJobJobKind):
         permissioned_as (str): The user (u/userfoo) or group (g/groupfoo) whom
             the execution of this script will be permissioned_as and by extension its DT_TOKEN.
         is_flow_step (bool):
         is_skipped (bool):
         email (str):
         visible_to_owner (bool):
+        tag (str):
         workspace_id (Union[Unset, str]):
         parent_job (Union[Unset, str]):
         script_path (Union[Unset, str]):
         script_hash (Union[Unset, str]):
         args (Union[Unset, CompletedJobArgs]):
         result (Union[Unset, Any]):
         logs (Union[Unset, str]):
@@ -59,14 +60,15 @@
     canceled: bool
     job_kind: CompletedJobJobKind
     permissioned_as: str
     is_flow_step: bool
     is_skipped: bool
     email: str
     visible_to_owner: bool
+    tag: str
     workspace_id: Union[Unset, str] = UNSET
     parent_job: Union[Unset, str] = UNSET
     script_path: Union[Unset, str] = UNSET
     script_hash: Union[Unset, str] = UNSET
     args: Union[Unset, CompletedJobArgs] = UNSET
     result: Union[Unset, Any] = UNSET
     logs: Union[Unset, str] = UNSET
@@ -94,14 +96,15 @@
         job_kind = self.job_kind.value
 
         permissioned_as = self.permissioned_as
         is_flow_step = self.is_flow_step
         is_skipped = self.is_skipped
         email = self.email
         visible_to_owner = self.visible_to_owner
+        tag = self.tag
         workspace_id = self.workspace_id
         parent_job = self.parent_job
         script_path = self.script_path
         script_hash = self.script_hash
         args: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.args, Unset):
             args = self.args.to_dict()
@@ -140,14 +143,15 @@
                 "canceled": canceled,
                 "job_kind": job_kind,
                 "permissioned_as": permissioned_as,
                 "is_flow_step": is_flow_step,
                 "is_skipped": is_skipped,
                 "email": email,
                 "visible_to_owner": visible_to_owner,
+                "tag": tag,
             }
         )
         if workspace_id is not UNSET:
             field_dict["workspace_id"] = workspace_id
         if parent_job is not UNSET:
             field_dict["parent_job"] = parent_job
         if script_path is not UNSET:
@@ -206,14 +210,16 @@
 
         is_skipped = d.pop("is_skipped")
 
         email = d.pop("email")
 
         visible_to_owner = d.pop("visible_to_owner")
 
+        tag = d.pop("tag")
+
         workspace_id = d.pop("workspace_id", UNSET)
 
         parent_job = d.pop("parent_job", UNSET)
 
         script_path = d.pop("script_path", UNSET)
 
         script_hash = d.pop("script_hash", UNSET)
@@ -272,14 +278,15 @@
             canceled=canceled,
             job_kind=job_kind,
             permissioned_as=permissioned_as,
             is_flow_step=is_flow_step,
             is_skipped=is_skipped,
             email=email,
             visible_to_owner=visible_to_owner,
+            tag=tag,
             workspace_id=workspace_id,
             parent_job=parent_job,
             script_path=script_path,
             script_hash=script_hash,
             args=args,
             result=result,
             logs=logs,
```

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_args.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_flow_status.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_failure_module_branchall.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_failure_module_iterator.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_modules_item_branchall.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_modules_item_iterator.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_flow_status_retry.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/connect_callback_json_body.py` & `windmill_api-1.89.0/windmill_api/models/connect_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/connect_callback_response_200.py` & `windmill_api-1.89.0/windmill_api/models/connect_callback_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/connect_slack_callback_json_body.py` & `windmill_api-1.89.0/windmill_api/models/connect_slack_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/contextual_variable.py` & `windmill_api-1.89.0/windmill_api/models/contextual_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_account_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_account_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_app_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_app_json_body_policy.py` & `windmill_api-1.89.0/windmill_api/models/create_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_app_json_body_policy_triggerables.py` & `windmill_api-1.89.0/windmill_api/models/create_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.89.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_schema.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_folder_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_group_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_input.py` & `windmill_api-1.89.0/windmill_api/models/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_input_args.py` & `windmill_api-1.89.0/windmill_api/models/create_input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_input_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_input_json_body_args.py` & `windmill_api-1.89.0/windmill_api/models/create_input_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_resource.py` & `windmill_api-1.89.0/windmill_api/models/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_resource_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_resource_type_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_schedule_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_schedule_json_body_args.py` & `windmill_api-1.89.0/windmill_api/models/create_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_script_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_script_json_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,26 +20,28 @@
         content (str):
         language (CreateScriptJsonBodyLanguage):
         parent_hash (Union[Unset, str]):
         schema (Union[Unset, CreateScriptJsonBodySchema]):
         is_template (Union[Unset, bool]):
         lock (Union[Unset, List[str]]):
         kind (Union[Unset, CreateScriptJsonBodyKind]):
+        tag (Union[Unset, str]):
     """
 
     path: str
     summary: str
     description: str
     content: str
     language: CreateScriptJsonBodyLanguage
     parent_hash: Union[Unset, str] = UNSET
     schema: Union[Unset, CreateScriptJsonBodySchema] = UNSET
     is_template: Union[Unset, bool] = UNSET
     lock: Union[Unset, List[str]] = UNSET
     kind: Union[Unset, CreateScriptJsonBodyKind] = UNSET
+    tag: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         path = self.path
         summary = self.summary
         description = self.description
         content = self.content
@@ -55,14 +57,16 @@
         if not isinstance(self.lock, Unset):
             lock = self.lock
 
         kind: Union[Unset, str] = UNSET
         if not isinstance(self.kind, Unset):
             kind = self.kind.value
 
+        tag = self.tag
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "path": path,
                 "summary": summary,
                 "description": description,
@@ -76,14 +80,16 @@
             field_dict["schema"] = schema
         if is_template is not UNSET:
             field_dict["is_template"] = is_template
         if lock is not UNSET:
             field_dict["lock"] = lock
         if kind is not UNSET:
             field_dict["kind"] = kind
+        if tag is not UNSET:
+            field_dict["tag"] = tag
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         path = d.pop("path")
@@ -112,25 +118,28 @@
         _kind = d.pop("kind", UNSET)
         kind: Union[Unset, CreateScriptJsonBodyKind]
         if isinstance(_kind, Unset):
             kind = UNSET
         else:
             kind = CreateScriptJsonBodyKind(_kind)
 
+        tag = d.pop("tag", UNSET)
+
         create_script_json_body = cls(
             path=path,
             summary=summary,
             description=description,
             content=content,
             language=language,
             parent_hash=parent_hash,
             schema=schema,
             is_template=is_template,
             lock=lock,
             kind=kind,
+            tag=tag,
         )
 
         create_script_json_body.additional_properties = d
         return create_script_json_body
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.88.1/windmill_api/models/create_script_json_body_schema.py` & `windmill_api-1.89.0/windmill_api/models/create_script_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_token_impersonate_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_token_impersonate_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_token_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_user_globally_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_user_globally_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_user_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_variable.py` & `windmill_api-1.89.0/windmill_api/models/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_variable_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_workspace.py` & `windmill_api-1.89.0/windmill_api/models/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/create_workspace_json_body.py` & `windmill_api-1.89.0/windmill_api/models/create_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/decline_invite_json_body.py` & `windmill_api-1.89.0/windmill_api/models/decline_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         job_kind (DeleteCompletedJobResponse200JobKind):
         permissioned_as (str): The user (u/userfoo) or group (g/groupfoo) whom
             the execution of this script will be permissioned_as and by extension its DT_TOKEN.
         is_flow_step (bool):
         is_skipped (bool):
         email (str):
         visible_to_owner (bool):
+        tag (str):
         workspace_id (Union[Unset, str]):
         parent_job (Union[Unset, str]):
         script_path (Union[Unset, str]):
         script_hash (Union[Unset, str]):
         args (Union[Unset, DeleteCompletedJobResponse200Args]):
         result (Union[Unset, Any]):
         logs (Union[Unset, str]):
@@ -59,14 +60,15 @@
     canceled: bool
     job_kind: DeleteCompletedJobResponse200JobKind
     permissioned_as: str
     is_flow_step: bool
     is_skipped: bool
     email: str
     visible_to_owner: bool
+    tag: str
     workspace_id: Union[Unset, str] = UNSET
     parent_job: Union[Unset, str] = UNSET
     script_path: Union[Unset, str] = UNSET
     script_hash: Union[Unset, str] = UNSET
     args: Union[Unset, DeleteCompletedJobResponse200Args] = UNSET
     result: Union[Unset, Any] = UNSET
     logs: Union[Unset, str] = UNSET
@@ -94,14 +96,15 @@
         job_kind = self.job_kind.value
 
         permissioned_as = self.permissioned_as
         is_flow_step = self.is_flow_step
         is_skipped = self.is_skipped
         email = self.email
         visible_to_owner = self.visible_to_owner
+        tag = self.tag
         workspace_id = self.workspace_id
         parent_job = self.parent_job
         script_path = self.script_path
         script_hash = self.script_hash
         args: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.args, Unset):
             args = self.args.to_dict()
@@ -140,14 +143,15 @@
                 "canceled": canceled,
                 "job_kind": job_kind,
                 "permissioned_as": permissioned_as,
                 "is_flow_step": is_flow_step,
                 "is_skipped": is_skipped,
                 "email": email,
                 "visible_to_owner": visible_to_owner,
+                "tag": tag,
             }
         )
         if workspace_id is not UNSET:
             field_dict["workspace_id"] = workspace_id
         if parent_job is not UNSET:
             field_dict["parent_job"] = parent_job
         if script_path is not UNSET:
@@ -206,14 +210,16 @@
 
         is_skipped = d.pop("is_skipped")
 
         email = d.pop("email")
 
         visible_to_owner = d.pop("visible_to_owner")
 
+        tag = d.pop("tag")
+
         workspace_id = d.pop("workspace_id", UNSET)
 
         parent_job = d.pop("parent_job", UNSET)
 
         script_path = d.pop("script_path", UNSET)
 
         script_hash = d.pop("script_hash", UNSET)
@@ -272,14 +278,15 @@
             canceled=canceled,
             job_kind=job_kind,
             permissioned_as=permissioned_as,
             is_flow_step=is_flow_step,
             is_skipped=is_skipped,
             email=email,
             visible_to_owner=visible_to_owner,
+            tag=tag,
             workspace_id=workspace_id,
             parent_job=parent_job,
             script_path=script_path,
             script_hash=script_hash,
             args=args,
             result=result,
             logs=logs,
```

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_args.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_invite_json_body.py` & `windmill_api-1.89.0/windmill_api/models/delete_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_script_by_hash_response_200.py` & `windmill_api-1.89.0/windmill_api/models/delete_script_by_hash_response_200.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         starred (bool):
         workspace_id (Union[Unset, str]):
         parent_hashes (Union[Unset, List[str]]): The first element is the direct parent of the script, the second is the
             parent of the first, etc
         schema (Union[Unset, DeleteScriptByHashResponse200Schema]):
         lock (Union[Unset, str]):
         lock_error_logs (Union[Unset, str]):
+        tag (Union[Unset, str]):
     """
 
     hash_: str
     path: str
     summary: str
     description: str
     content: str
@@ -54,14 +55,15 @@
     kind: DeleteScriptByHashResponse200Kind
     starred: bool
     workspace_id: Union[Unset, str] = UNSET
     parent_hashes: Union[Unset, List[str]] = UNSET
     schema: Union[Unset, DeleteScriptByHashResponse200Schema] = UNSET
     lock: Union[Unset, str] = UNSET
     lock_error_logs: Union[Unset, str] = UNSET
+    tag: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         hash_ = self.hash_
         path = self.path
         summary = self.summary
         description = self.description
@@ -86,14 +88,15 @@
 
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         lock = self.lock
         lock_error_logs = self.lock_error_logs
+        tag = self.tag
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "hash": hash_,
                 "path": path,
@@ -117,14 +120,16 @@
             field_dict["parent_hashes"] = parent_hashes
         if schema is not UNSET:
             field_dict["schema"] = schema
         if lock is not UNSET:
             field_dict["lock"] = lock
         if lock_error_logs is not UNSET:
             field_dict["lock_error_logs"] = lock_error_logs
+        if tag is not UNSET:
+            field_dict["tag"] = tag
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         hash_ = d.pop("hash")
@@ -166,14 +171,16 @@
         else:
             schema = DeleteScriptByHashResponse200Schema.from_dict(_schema)
 
         lock = d.pop("lock", UNSET)
 
         lock_error_logs = d.pop("lock_error_logs", UNSET)
 
+        tag = d.pop("tag", UNSET)
+
         delete_script_by_hash_response_200 = cls(
             hash_=hash_,
             path=path,
             summary=summary,
             description=description,
             content=content,
             created_by=created_by,
@@ -186,14 +193,15 @@
             kind=kind,
             starred=starred,
             workspace_id=workspace_id,
             parent_hashes=parent_hashes,
             schema=schema,
             lock=lock,
             lock_error_logs=lock_error_logs,
+            tag=tag,
         )
 
         delete_script_by_hash_response_200.additional_properties = d
         return delete_script_by_hash_response_200
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/delete_script_by_hash_response_200_schema.py` & `windmill_api-1.89.0/windmill_api/models/delete_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200.py` & `windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item.py` & `windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.89.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/edit_auto_invite_json_body.py` & `windmill_api-1.89.0/windmill_api/models/edit_auto_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/edit_resource.py` & `windmill_api-1.89.0/windmill_api/models/edit_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/edit_resource_type.py` & `windmill_api-1.89.0/windmill_api/models/edit_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/edit_schedule.py` & `windmill_api-1.89.0/windmill_api/models/edit_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/edit_schedule_args.py` & `windmill_api-1.89.0/windmill_api/models/edit_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/edit_slack_command_json_body.py` & `windmill_api-1.89.0/windmill_api/models/edit_slack_command_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/edit_variable.py` & `windmill_api-1.89.0/windmill_api/models/edit_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/edit_webhook_json_body.py` & `windmill_api-1.89.0/windmill_api/models/edit_webhook_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/edit_workspace_user.py` & `windmill_api-1.89.0/windmill_api/models/edit_workspace_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/execute_component_json_body.py` & `windmill_api-1.89.0/windmill_api/models/execute_component_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py` & `windmill_api-1.89.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/execute_component_json_body_raw_code.py` & `windmill_api-1.89.0/windmill_api/models/execute_component_json_body_raw_code.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/exists_username_json_body.py` & `windmill_api-1.89.0/windmill_api/models/exists_username_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/exists_workspace_json_body.py` & `windmill_api-1.89.0/windmill_api/models/exists_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow.py` & `windmill_api-1.89.0/windmill_api/models/flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/flow_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_metadata.py` & `windmill_api-1.89.0/windmill_api/models/flow_metadata.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_metadata_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/flow_metadata_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module.py` & `windmill_api-1.89.0/windmill_api/models/flow_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_0.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_0.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,34 +16,37 @@
     Attributes:
         input_transforms (FlowModuleValue2Type0InputTransforms):
         content (str):
         language (FlowModuleValue2Type0Language):
         type (FlowModuleValue2Type0Type):
         path (Union[Unset, str]):
         lock (Union[Unset, str]):
+        tag (Union[Unset, str]):
     """
 
     input_transforms: FlowModuleValue2Type0InputTransforms
     content: str
     language: FlowModuleValue2Type0Language
     type: FlowModuleValue2Type0Type
     path: Union[Unset, str] = UNSET
     lock: Union[Unset, str] = UNSET
+    tag: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         input_transforms = self.input_transforms.to_dict()
 
         content = self.content
         language = self.language.value
 
         type = self.type.value
 
         path = self.path
         lock = self.lock
+        tag = self.tag
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "input_transforms": input_transforms,
                 "content": content,
@@ -51,14 +54,16 @@
                 "type": type,
             }
         )
         if path is not UNSET:
             field_dict["path"] = path
         if lock is not UNSET:
             field_dict["lock"] = lock
+        if tag is not UNSET:
+            field_dict["tag"] = tag
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         input_transforms = FlowModuleValue2Type0InputTransforms.from_dict(d.pop("input_transforms"))
@@ -69,21 +74,24 @@
 
         type = FlowModuleValue2Type0Type(d.pop("type"))
 
         path = d.pop("path", UNSET)
 
         lock = d.pop("lock", UNSET)
 
+        tag = d.pop("tag", UNSET)
+
         flow_module_value_2_type_0 = cls(
             input_transforms=input_transforms,
             content=content,
             language=language,
             type=type,
             path=path,
             lock=lock,
+            tag=tag,
         )
 
         flow_module_value_2_type_0.additional_properties = d
         return flow_module_value_2_type_0
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_0_input_transforms.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_1.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_1_input_transforms.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_2.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_2_input_transforms.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_module_value_2_type_6.py` & `windmill_api-1.89.0/windmill_api/models/flow_module_value_2_type_6.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_args.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_preview_value_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/flow_preview_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_schema.py` & `windmill_api-1.89.0/windmill_api/models/flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status.py` & `windmill_api-1.89.0/windmill_api/models/flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_failure_module_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_failure_module_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_failure_module_branchall.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_failure_module_iterator.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_module.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_module_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_module_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_module_branchall.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_module_iterator.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_modules_item_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_modules_item_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_modules_item_branchall.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_modules_item_iterator.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_status_retry.py` & `windmill_api-1.89.0/windmill_api/models/flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value.py` & `windmill_api-1.89.0/windmill_api/models/flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/flow_value_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/folder.py` & `windmill_api-1.89.0/windmill_api/models/folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/folder_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/folder_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/force_cancel_queued_job_json_body.py` & `windmill_api-1.89.0/windmill_api/models/force_cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/forloop_flow.py` & `windmill_api-1.89.0/windmill_api/models/forloop_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/forloop_flow_iterator_type_0.py` & `windmill_api-1.89.0/windmill_api/models/forloop_flow_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/forloop_flow_iterator_type_1.py` & `windmill_api-1.89.0/windmill_api/models/forloop_flow_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/forloop_flow_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/forloop_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_app_by_path_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_app_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_app_by_path_response_200_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_app_by_path_response_200_policy.py` & `windmill_api-1.89.0/windmill_api/models/get_app_by_path_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py` & `windmill_api-1.89.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.89.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_app_by_version_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_app_by_version_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_app_by_version_response_200_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_app_by_version_response_200_policy.py` & `windmill_api-1.89.0/windmill_api/models/get_app_by_version_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py` & `windmill_api-1.89.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.89.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_audit_log_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_audit_log_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_audit_log_response_200_operation.py` & `windmill_api-1.89.0/windmill_api/models/get_audit_log_response_200_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_audit_log_response_200_parameters.py` & `windmill_api-1.89.0/windmill_api/models/get_audit_log_response_200_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         job_kind (GetCompletedJobResponse200JobKind):
         permissioned_as (str): The user (u/userfoo) or group (g/groupfoo) whom
             the execution of this script will be permissioned_as and by extension its DT_TOKEN.
         is_flow_step (bool):
         is_skipped (bool):
         email (str):
         visible_to_owner (bool):
+        tag (str):
         workspace_id (Union[Unset, str]):
         parent_job (Union[Unset, str]):
         script_path (Union[Unset, str]):
         script_hash (Union[Unset, str]):
         args (Union[Unset, GetCompletedJobResponse200Args]):
         result (Union[Unset, Any]):
         logs (Union[Unset, str]):
@@ -59,14 +60,15 @@
     canceled: bool
     job_kind: GetCompletedJobResponse200JobKind
     permissioned_as: str
     is_flow_step: bool
     is_skipped: bool
     email: str
     visible_to_owner: bool
+    tag: str
     workspace_id: Union[Unset, str] = UNSET
     parent_job: Union[Unset, str] = UNSET
     script_path: Union[Unset, str] = UNSET
     script_hash: Union[Unset, str] = UNSET
     args: Union[Unset, GetCompletedJobResponse200Args] = UNSET
     result: Union[Unset, Any] = UNSET
     logs: Union[Unset, str] = UNSET
@@ -94,14 +96,15 @@
         job_kind = self.job_kind.value
 
         permissioned_as = self.permissioned_as
         is_flow_step = self.is_flow_step
         is_skipped = self.is_skipped
         email = self.email
         visible_to_owner = self.visible_to_owner
+        tag = self.tag
         workspace_id = self.workspace_id
         parent_job = self.parent_job
         script_path = self.script_path
         script_hash = self.script_hash
         args: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.args, Unset):
             args = self.args.to_dict()
@@ -140,14 +143,15 @@
                 "canceled": canceled,
                 "job_kind": job_kind,
                 "permissioned_as": permissioned_as,
                 "is_flow_step": is_flow_step,
                 "is_skipped": is_skipped,
                 "email": email,
                 "visible_to_owner": visible_to_owner,
+                "tag": tag,
             }
         )
         if workspace_id is not UNSET:
             field_dict["workspace_id"] = workspace_id
         if parent_job is not UNSET:
             field_dict["parent_job"] = parent_job
         if script_path is not UNSET:
@@ -206,14 +210,16 @@
 
         is_skipped = d.pop("is_skipped")
 
         email = d.pop("email")
 
         visible_to_owner = d.pop("visible_to_owner")
 
+        tag = d.pop("tag")
+
         workspace_id = d.pop("workspace_id", UNSET)
 
         parent_job = d.pop("parent_job", UNSET)
 
         script_path = d.pop("script_path", UNSET)
 
         script_hash = d.pop("script_hash", UNSET)
@@ -272,14 +278,15 @@
             canceled=canceled,
             job_kind=job_kind,
             permissioned_as=permissioned_as,
             is_flow_step=is_flow_step,
             is_skipped=is_skipped,
             email=email,
             visible_to_owner=visible_to_owner,
+            tag=tag,
             workspace_id=workspace_id,
             parent_job=parent_job,
             script_path=script_path,
             script_hash=script_hash,
             args=args,
             result=result,
             logs=logs,
```

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_args.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_schema.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_input_history_by_path_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py` & `windmill_api-1.89.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_folder_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_folder_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_folder_response_200_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/get_folder_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_folder_usage_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_folder_usage_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_granular_acls_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_granular_acls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_group_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_group_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_group_response_200_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/get_group_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_app_by_id_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_app_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_app_by_id_response_200_app.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_app_by_id_response_200_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_hub_script_by_path_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_hub_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_input_history_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/get_input_history_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_input_history_response_200_item_args.py` & `windmill_api-1.89.0/windmill_api/models/get_input_history_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_job_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_job_updates_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_job_updates_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_premium_info_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_premium_info_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_public_app_by_secret_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_public_app_by_secret_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_public_app_by_secret_response_200_policy.py` & `windmill_api-1.89.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py` & `windmill_api-1.89.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.89.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_resource_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_resource_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_resource_response_200_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/get_resource_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_resource_type_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_resource_type_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_resume_urls_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_resume_urls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_schedule_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_schedule_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_schedule_response_200_args.py` & `windmill_api-1.89.0/windmill_api/models/get_schedule_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_schedule_response_200_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/get_schedule_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_script_by_hash_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_script_by_hash_response_200.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         starred (bool):
         workspace_id (Union[Unset, str]):
         parent_hashes (Union[Unset, List[str]]): The first element is the direct parent of the script, the second is the
             parent of the first, etc
         schema (Union[Unset, GetScriptByHashResponse200Schema]):
         lock (Union[Unset, str]):
         lock_error_logs (Union[Unset, str]):
+        tag (Union[Unset, str]):
     """
 
     hash_: str
     path: str
     summary: str
     description: str
     content: str
@@ -54,14 +55,15 @@
     kind: GetScriptByHashResponse200Kind
     starred: bool
     workspace_id: Union[Unset, str] = UNSET
     parent_hashes: Union[Unset, List[str]] = UNSET
     schema: Union[Unset, GetScriptByHashResponse200Schema] = UNSET
     lock: Union[Unset, str] = UNSET
     lock_error_logs: Union[Unset, str] = UNSET
+    tag: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         hash_ = self.hash_
         path = self.path
         summary = self.summary
         description = self.description
@@ -86,14 +88,15 @@
 
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         lock = self.lock
         lock_error_logs = self.lock_error_logs
+        tag = self.tag
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "hash": hash_,
                 "path": path,
@@ -117,14 +120,16 @@
             field_dict["parent_hashes"] = parent_hashes
         if schema is not UNSET:
             field_dict["schema"] = schema
         if lock is not UNSET:
             field_dict["lock"] = lock
         if lock_error_logs is not UNSET:
             field_dict["lock_error_logs"] = lock_error_logs
+        if tag is not UNSET:
+            field_dict["tag"] = tag
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         hash_ = d.pop("hash")
@@ -166,14 +171,16 @@
         else:
             schema = GetScriptByHashResponse200Schema.from_dict(_schema)
 
         lock = d.pop("lock", UNSET)
 
         lock_error_logs = d.pop("lock_error_logs", UNSET)
 
+        tag = d.pop("tag", UNSET)
+
         get_script_by_hash_response_200 = cls(
             hash_=hash_,
             path=path,
             summary=summary,
             description=description,
             content=content,
             created_by=created_by,
@@ -186,14 +193,15 @@
             kind=kind,
             starred=starred,
             workspace_id=workspace_id,
             parent_hashes=parent_hashes,
             schema=schema,
             lock=lock,
             lock_error_logs=lock_error_logs,
+            tag=tag,
         )
 
         get_script_by_hash_response_200.additional_properties = d
         return get_script_by_hash_response_200
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.88.1/windmill_api/models/get_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_script_by_hash_response_200_schema.py` & `windmill_api-1.89.0/windmill_api/models/get_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_script_by_path_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_script_by_path_response_200.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         starred (bool):
         workspace_id (Union[Unset, str]):
         parent_hashes (Union[Unset, List[str]]): The first element is the direct parent of the script, the second is the
             parent of the first, etc
         schema (Union[Unset, GetScriptByPathResponse200Schema]):
         lock (Union[Unset, str]):
         lock_error_logs (Union[Unset, str]):
+        tag (Union[Unset, str]):
     """
 
     hash_: str
     path: str
     summary: str
     description: str
     content: str
@@ -54,14 +55,15 @@
     kind: GetScriptByPathResponse200Kind
     starred: bool
     workspace_id: Union[Unset, str] = UNSET
     parent_hashes: Union[Unset, List[str]] = UNSET
     schema: Union[Unset, GetScriptByPathResponse200Schema] = UNSET
     lock: Union[Unset, str] = UNSET
     lock_error_logs: Union[Unset, str] = UNSET
+    tag: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         hash_ = self.hash_
         path = self.path
         summary = self.summary
         description = self.description
@@ -86,14 +88,15 @@
 
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         lock = self.lock
         lock_error_logs = self.lock_error_logs
+        tag = self.tag
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "hash": hash_,
                 "path": path,
@@ -117,14 +120,16 @@
             field_dict["parent_hashes"] = parent_hashes
         if schema is not UNSET:
             field_dict["schema"] = schema
         if lock is not UNSET:
             field_dict["lock"] = lock
         if lock_error_logs is not UNSET:
             field_dict["lock_error_logs"] = lock_error_logs
+        if tag is not UNSET:
+            field_dict["tag"] = tag
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         hash_ = d.pop("hash")
@@ -166,14 +171,16 @@
         else:
             schema = GetScriptByPathResponse200Schema.from_dict(_schema)
 
         lock = d.pop("lock", UNSET)
 
         lock_error_logs = d.pop("lock_error_logs", UNSET)
 
+        tag = d.pop("tag", UNSET)
+
         get_script_by_path_response_200 = cls(
             hash_=hash_,
             path=path,
             summary=summary,
             description=description,
             content=content,
             created_by=created_by,
@@ -186,14 +193,15 @@
             kind=kind,
             starred=starred,
             workspace_id=workspace_id,
             parent_hashes=parent_hashes,
             schema=schema,
             lock=lock,
             lock_error_logs=lock_error_logs,
+            tag=tag,
         )
 
         get_script_by_path_response_200.additional_properties = d
         return get_script_by_path_response_200
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.88.1/windmill_api/models/get_script_by_path_response_200_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_script_by_path_response_200_schema.py` & `windmill_api-1.89.0/windmill_api/models/get_script_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_script_deployment_status_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_script_deployment_status_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_settings_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_suspended_job_flow_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_suspended_job_flow_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_suspended_job_flow_response_200_job.py` & `windmill_api-1.89.0/windmill_api/models/get_suspended_job_flow_response_200_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_variable_response_200.py` & `windmill_api-1.89.0/windmill_api/models/get_variable_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/get_variable_response_200_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/get_variable_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/global_user_info.py` & `windmill_api-1.89.0/windmill_api/models/global_user_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/global_user_update_json_body.py` & `windmill_api-1.89.0/windmill_api/models/global_user_update_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/global_whoami_response_200.py` & `windmill_api-1.89.0/windmill_api/models/global_whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200.py` & `windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item.py` & `windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.89.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/group.py` & `windmill_api-1.89.0/windmill_api/models/group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/group_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/group_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/identity.py` & `windmill_api-1.89.0/windmill_api/models/identity.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/input_.py` & `windmill_api-1.89.0/windmill_api/models/input_.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/input_args.py` & `windmill_api-1.89.0/windmill_api/models/input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/input_transform_type_0.py` & `windmill_api-1.89.0/windmill_api/models/input_transform_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/input_transform_type_1.py` & `windmill_api-1.89.0/windmill_api/models/input_transform_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/invite_user_json_body.py` & `windmill_api-1.89.0/windmill_api/models/invite_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/javascript_transform.py` & `windmill_api-1.89.0/windmill_api/models/javascript_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/job.py` & `windmill_api-1.89.0/windmill_api/models/job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_apps_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_apps_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_apps_response_200_item_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/list_apps_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_audit_logs_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_audit_logs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_audit_logs_response_200_item_operation.py` & `windmill_api-1.89.0/windmill_api/models/list_audit_logs_response_200_item_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_audit_logs_response_200_item_parameters.py` & `windmill_api-1.89.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         job_kind (ListCompletedJobsResponse200ItemJobKind):
         permissioned_as (str): The user (u/userfoo) or group (g/groupfoo) whom
             the execution of this script will be permissioned_as and by extension its DT_TOKEN.
         is_flow_step (bool):
         is_skipped (bool):
         email (str):
         visible_to_owner (bool):
+        tag (str):
         workspace_id (Union[Unset, str]):
         parent_job (Union[Unset, str]):
         script_path (Union[Unset, str]):
         script_hash (Union[Unset, str]):
         args (Union[Unset, ListCompletedJobsResponse200ItemArgs]):
         result (Union[Unset, Any]):
         logs (Union[Unset, str]):
@@ -59,14 +60,15 @@
     canceled: bool
     job_kind: ListCompletedJobsResponse200ItemJobKind
     permissioned_as: str
     is_flow_step: bool
     is_skipped: bool
     email: str
     visible_to_owner: bool
+    tag: str
     workspace_id: Union[Unset, str] = UNSET
     parent_job: Union[Unset, str] = UNSET
     script_path: Union[Unset, str] = UNSET
     script_hash: Union[Unset, str] = UNSET
     args: Union[Unset, ListCompletedJobsResponse200ItemArgs] = UNSET
     result: Union[Unset, Any] = UNSET
     logs: Union[Unset, str] = UNSET
@@ -94,14 +96,15 @@
         job_kind = self.job_kind.value
 
         permissioned_as = self.permissioned_as
         is_flow_step = self.is_flow_step
         is_skipped = self.is_skipped
         email = self.email
         visible_to_owner = self.visible_to_owner
+        tag = self.tag
         workspace_id = self.workspace_id
         parent_job = self.parent_job
         script_path = self.script_path
         script_hash = self.script_hash
         args: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.args, Unset):
             args = self.args.to_dict()
@@ -140,14 +143,15 @@
                 "canceled": canceled,
                 "job_kind": job_kind,
                 "permissioned_as": permissioned_as,
                 "is_flow_step": is_flow_step,
                 "is_skipped": is_skipped,
                 "email": email,
                 "visible_to_owner": visible_to_owner,
+                "tag": tag,
             }
         )
         if workspace_id is not UNSET:
             field_dict["workspace_id"] = workspace_id
         if parent_job is not UNSET:
             field_dict["parent_job"] = parent_job
         if script_path is not UNSET:
@@ -206,14 +210,16 @@
 
         is_skipped = d.pop("is_skipped")
 
         email = d.pop("email")
 
         visible_to_owner = d.pop("visible_to_owner")
 
+        tag = d.pop("tag")
+
         workspace_id = d.pop("workspace_id", UNSET)
 
         parent_job = d.pop("parent_job", UNSET)
 
         script_path = d.pop("script_path", UNSET)
 
         script_hash = d.pop("script_hash", UNSET)
@@ -272,14 +278,15 @@
             canceled=canceled,
             job_kind=job_kind,
             permissioned_as=permissioned_as,
             is_flow_step=is_flow_step,
             is_skipped=is_skipped,
             email=email,
             visible_to_owner=visible_to_owner,
+            tag=tag,
             workspace_id=workspace_id,
             parent_job=parent_job,
             script_path=script_path,
             script_hash=script_hash,
             args=args,
             result=result,
             logs=logs,
```

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_args.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_contextual_variables_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_contextual_variables_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_schema.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_folders_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_folders_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_folders_response_200_item_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/list_folders_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_groups_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_groups_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_groups_response_200_item_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/list_groups_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_hub_apps_response_200.py` & `windmill_api-1.89.0/windmill_api/models/list_hub_apps_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_hub_apps_response_200_apps_item.py` & `windmill_api-1.89.0/windmill_api/models/list_hub_apps_response_200_apps_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_hub_flows_response_200.py` & `windmill_api-1.89.0/windmill_api/models/list_hub_flows_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_hub_flows_response_200_flows_item.py` & `windmill_api-1.89.0/windmill_api/models/list_hub_flows_response_200_flows_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_hub_scripts_response_200.py` & `windmill_api-1.89.0/windmill_api/models/list_hub_scripts_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_hub_scripts_response_200_asks_item.py` & `windmill_api-1.89.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_inputs_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_inputs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_inputs_response_200_item_args.py` & `windmill_api-1.89.0/windmill_api/models/list_inputs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_jobs_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_pending_invites_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_pending_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         canceled (bool):
         job_kind (ListQueueResponse200ItemJobKind):
         permissioned_as (str): The user (u/userfoo) or group (g/groupfoo) whom
             the execution of this script will be permissioned_as and by extension its DT_TOKEN.
         is_flow_step (bool):
         email (str):
         visible_to_owner (bool):
+        tag (str):
         workspace_id (Union[Unset, str]):
         parent_job (Union[Unset, str]):
         created_by (Union[Unset, str]):
         created_at (Union[Unset, datetime.datetime]):
         started_at (Union[Unset, datetime.datetime]):
         scheduled_for (Union[Unset, datetime.datetime]):
         script_path (Union[Unset, str]):
@@ -52,14 +53,15 @@
     running: bool
     canceled: bool
     job_kind: ListQueueResponse200ItemJobKind
     permissioned_as: str
     is_flow_step: bool
     email: str
     visible_to_owner: bool
+    tag: str
     workspace_id: Union[Unset, str] = UNSET
     parent_job: Union[Unset, str] = UNSET
     created_by: Union[Unset, str] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     scheduled_for: Union[Unset, datetime.datetime] = UNSET
     script_path: Union[Unset, str] = UNSET
@@ -83,14 +85,15 @@
         canceled = self.canceled
         job_kind = self.job_kind.value
 
         permissioned_as = self.permissioned_as
         is_flow_step = self.is_flow_step
         email = self.email
         visible_to_owner = self.visible_to_owner
+        tag = self.tag
         workspace_id = self.workspace_id
         parent_job = self.parent_job
         created_by = self.created_by
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
 
@@ -139,14 +142,15 @@
                 "running": running,
                 "canceled": canceled,
                 "job_kind": job_kind,
                 "permissioned_as": permissioned_as,
                 "is_flow_step": is_flow_step,
                 "email": email,
                 "visible_to_owner": visible_to_owner,
+                "tag": tag,
             }
         )
         if workspace_id is not UNSET:
             field_dict["workspace_id"] = workspace_id
         if parent_job is not UNSET:
             field_dict["parent_job"] = parent_job
         if created_by is not UNSET:
@@ -201,14 +205,16 @@
 
         is_flow_step = d.pop("is_flow_step")
 
         email = d.pop("email")
 
         visible_to_owner = d.pop("visible_to_owner")
 
+        tag = d.pop("tag")
+
         workspace_id = d.pop("workspace_id", UNSET)
 
         parent_job = d.pop("parent_job", UNSET)
 
         created_by = d.pop("created_by", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
@@ -288,14 +294,15 @@
             running=running,
             canceled=canceled,
             job_kind=job_kind,
             permissioned_as=permissioned_as,
             is_flow_step=is_flow_step,
             email=email,
             visible_to_owner=visible_to_owner,
+            tag=tag,
             workspace_id=workspace_id,
             parent_job=parent_job,
             created_by=created_by,
             created_at=created_at,
             started_at=started_at,
             scheduled_for=scheduled_for,
             script_path=script_path,
```

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_args.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_flow_status_retry.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_resource_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_resource_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_resource_response_200_item_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/list_resource_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_resource_type_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_resource_type_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_schedules_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_schedules_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_schedules_response_200_item_args.py` & `windmill_api-1.89.0/windmill_api/models/list_schedules_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_schedules_response_200_item_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_scripts_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_scripts_response_200_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         starred (bool):
         workspace_id (Union[Unset, str]):
         parent_hashes (Union[Unset, List[str]]): The first element is the direct parent of the script, the second is the
             parent of the first, etc
         schema (Union[Unset, ListScriptsResponse200ItemSchema]):
         lock (Union[Unset, str]):
         lock_error_logs (Union[Unset, str]):
+        tag (Union[Unset, str]):
     """
 
     hash_: str
     path: str
     summary: str
     description: str
     content: str
@@ -54,14 +55,15 @@
     kind: ListScriptsResponse200ItemKind
     starred: bool
     workspace_id: Union[Unset, str] = UNSET
     parent_hashes: Union[Unset, List[str]] = UNSET
     schema: Union[Unset, ListScriptsResponse200ItemSchema] = UNSET
     lock: Union[Unset, str] = UNSET
     lock_error_logs: Union[Unset, str] = UNSET
+    tag: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         hash_ = self.hash_
         path = self.path
         summary = self.summary
         description = self.description
@@ -86,14 +88,15 @@
 
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         lock = self.lock
         lock_error_logs = self.lock_error_logs
+        tag = self.tag
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "hash": hash_,
                 "path": path,
@@ -117,14 +120,16 @@
             field_dict["parent_hashes"] = parent_hashes
         if schema is not UNSET:
             field_dict["schema"] = schema
         if lock is not UNSET:
             field_dict["lock"] = lock
         if lock_error_logs is not UNSET:
             field_dict["lock_error_logs"] = lock_error_logs
+        if tag is not UNSET:
+            field_dict["tag"] = tag
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         hash_ = d.pop("hash")
@@ -166,14 +171,16 @@
         else:
             schema = ListScriptsResponse200ItemSchema.from_dict(_schema)
 
         lock = d.pop("lock", UNSET)
 
         lock_error_logs = d.pop("lock_error_logs", UNSET)
 
+        tag = d.pop("tag", UNSET)
+
         list_scripts_response_200_item = cls(
             hash_=hash_,
             path=path,
             summary=summary,
             description=description,
             content=content,
             created_by=created_by,
@@ -186,14 +193,15 @@
             kind=kind,
             starred=starred,
             workspace_id=workspace_id,
             parent_hashes=parent_hashes,
             schema=schema,
             lock=lock,
             lock_error_logs=lock_error_logs,
+            tag=tag,
         )
 
         list_scripts_response_200_item.additional_properties = d
         return list_scripts_response_200_item
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.88.1/windmill_api/models/list_scripts_response_200_item_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_scripts_response_200_item_schema.py` & `windmill_api-1.89.0/windmill_api/models/list_scripts_response_200_item_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_tokens_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_tokens_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_user_workspaces_response_200.py` & `windmill_api-1.89.0/windmill_api/models/list_user_workspaces_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py` & `windmill_api-1.89.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_users_as_super_admin_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_users_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_users_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_users_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_users_response_200_item_usage.py` & `windmill_api-1.89.0/windmill_api/models/list_users_response_200_item_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_variable_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_variable_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_variable_response_200_item_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/list_variable_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_workers_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_workers_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_workspace_invites_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_workspace_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/list_workspaces_response_200_item.py` & `windmill_api-1.89.0/windmill_api/models/list_workspaces_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/listable_app.py` & `windmill_api-1.89.0/windmill_api/models/listable_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/listable_app_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/listable_app_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/listable_resource.py` & `windmill_api-1.89.0/windmill_api/models/listable_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/listable_resource_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/listable_resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/listable_variable.py` & `windmill_api-1.89.0/windmill_api/models/listable_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/listable_variable_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/listable_variable_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/login.py` & `windmill_api-1.89.0/windmill_api/models/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/login_json_body.py` & `windmill_api-1.89.0/windmill_api/models/login_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/login_with_oauth_json_body.py` & `windmill_api-1.89.0/windmill_api/models/login_with_oauth_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/main_arg_signature.py` & `windmill_api-1.89.0/windmill_api/models/main_arg_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item.py` & `windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_1.py` & `windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_2.py` & `windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_3.py` & `windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py` & `windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_4.py` & `windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.89.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/new_schedule.py` & `windmill_api-1.89.0/windmill_api/models/new_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/new_schedule_args.py` & `windmill_api-1.89.0/windmill_api/models/new_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/new_token.py` & `windmill_api-1.89.0/windmill_api/models/new_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/new_token_impersonate.py` & `windmill_api-1.89.0/windmill_api/models/new_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/new_user.py` & `windmill_api-1.89.0/windmill_api/models/new_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow.py` & `windmill_api-1.89.0/windmill_api/models/open_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_schema.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_value_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_schema.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/path_flow.py` & `windmill_api-1.89.0/windmill_api/models/path_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/path_flow_input_transforms.py` & `windmill_api-1.89.0/windmill_api/models/path_flow_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py` & `windmill_api-1.89.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py` & `windmill_api-1.89.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/path_script.py` & `windmill_api-1.89.0/windmill_api/models/path_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/path_script_input_transforms.py` & `windmill_api-1.89.0/windmill_api/models/path_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/path_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.89.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/path_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.89.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/policy.py` & `windmill_api-1.89.0/windmill_api/models/policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/policy_triggerables.py` & `windmill_api-1.89.0/windmill_api/models/policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/policy_triggerables_additional_property.py` & `windmill_api-1.89.0/windmill_api/models/policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/preview.py` & `windmill_api-1.89.0/windmill_api/models/preview.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,60 +13,68 @@
 class Preview:
     """
     Attributes:
         content (str):
         args (PreviewArgs):
         language (PreviewLanguage):
         path (Union[Unset, str]):
+        tag (Union[Unset, str]):
     """
 
     content: str
     args: PreviewArgs
     language: PreviewLanguage
     path: Union[Unset, str] = UNSET
+    tag: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         content = self.content
         args = self.args.to_dict()
 
         language = self.language.value
 
         path = self.path
+        tag = self.tag
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "content": content,
                 "args": args,
                 "language": language,
             }
         )
         if path is not UNSET:
             field_dict["path"] = path
+        if tag is not UNSET:
+            field_dict["tag"] = tag
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         content = d.pop("content")
 
         args = PreviewArgs.from_dict(d.pop("args"))
 
         language = PreviewLanguage(d.pop("language"))
 
         path = d.pop("path", UNSET)
 
+        tag = d.pop("tag", UNSET)
+
         preview = cls(
             content=content,
             args=args,
             language=language,
             path=path,
+            tag=tag,
         )
 
         preview.additional_properties = d
         return preview
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.88.1/windmill_api/models/preview_args.py` & `windmill_api-1.89.0/windmill_api/models/preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/preview_schedule_json_body.py` & `windmill_api-1.89.0/windmill_api/models/preview_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200.py` & `windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item.py` & `windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.89.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job.py` & `windmill_api-1.89.0/windmill_api/models/queued_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         canceled (bool):
         job_kind (QueuedJobJobKind):
         permissioned_as (str): The user (u/userfoo) or group (g/groupfoo) whom
             the execution of this script will be permissioned_as and by extension its DT_TOKEN.
         is_flow_step (bool):
         email (str):
         visible_to_owner (bool):
+        tag (str):
         workspace_id (Union[Unset, str]):
         parent_job (Union[Unset, str]):
         created_by (Union[Unset, str]):
         created_at (Union[Unset, datetime.datetime]):
         started_at (Union[Unset, datetime.datetime]):
         scheduled_for (Union[Unset, datetime.datetime]):
         script_path (Union[Unset, str]):
@@ -52,14 +53,15 @@
     running: bool
     canceled: bool
     job_kind: QueuedJobJobKind
     permissioned_as: str
     is_flow_step: bool
     email: str
     visible_to_owner: bool
+    tag: str
     workspace_id: Union[Unset, str] = UNSET
     parent_job: Union[Unset, str] = UNSET
     created_by: Union[Unset, str] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     scheduled_for: Union[Unset, datetime.datetime] = UNSET
     script_path: Union[Unset, str] = UNSET
@@ -83,14 +85,15 @@
         canceled = self.canceled
         job_kind = self.job_kind.value
 
         permissioned_as = self.permissioned_as
         is_flow_step = self.is_flow_step
         email = self.email
         visible_to_owner = self.visible_to_owner
+        tag = self.tag
         workspace_id = self.workspace_id
         parent_job = self.parent_job
         created_by = self.created_by
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
 
@@ -139,14 +142,15 @@
                 "running": running,
                 "canceled": canceled,
                 "job_kind": job_kind,
                 "permissioned_as": permissioned_as,
                 "is_flow_step": is_flow_step,
                 "email": email,
                 "visible_to_owner": visible_to_owner,
+                "tag": tag,
             }
         )
         if workspace_id is not UNSET:
             field_dict["workspace_id"] = workspace_id
         if parent_job is not UNSET:
             field_dict["parent_job"] = parent_job
         if created_by is not UNSET:
@@ -201,14 +205,16 @@
 
         is_flow_step = d.pop("is_flow_step")
 
         email = d.pop("email")
 
         visible_to_owner = d.pop("visible_to_owner")
 
+        tag = d.pop("tag")
+
         workspace_id = d.pop("workspace_id", UNSET)
 
         parent_job = d.pop("parent_job", UNSET)
 
         created_by = d.pop("created_by", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
@@ -288,14 +294,15 @@
             running=running,
             canceled=canceled,
             job_kind=job_kind,
             permissioned_as=permissioned_as,
             is_flow_step=is_flow_step,
             email=email,
             visible_to_owner=visible_to_owner,
+            tag=tag,
             workspace_id=workspace_id,
             parent_job=parent_job,
             created_by=created_by,
             created_at=created_at,
             started_at=started_at,
             scheduled_for=scheduled_for,
             script_path=script_path,
```

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_args.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_flow_status.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_failure_module_branchall.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_failure_module_iterator.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_modules_item_branchall.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_modules_item_iterator.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_flow_status_retry.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/raw_script.py` & `windmill_api-1.89.0/windmill_api/models/raw_script.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,34 +16,37 @@
     Attributes:
         input_transforms (RawScriptInputTransforms):
         content (str):
         language (RawScriptLanguage):
         type (RawScriptType):
         path (Union[Unset, str]):
         lock (Union[Unset, str]):
+        tag (Union[Unset, str]):
     """
 
     input_transforms: RawScriptInputTransforms
     content: str
     language: RawScriptLanguage
     type: RawScriptType
     path: Union[Unset, str] = UNSET
     lock: Union[Unset, str] = UNSET
+    tag: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         input_transforms = self.input_transforms.to_dict()
 
         content = self.content
         language = self.language.value
 
         type = self.type.value
 
         path = self.path
         lock = self.lock
+        tag = self.tag
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "input_transforms": input_transforms,
                 "content": content,
@@ -51,14 +54,16 @@
                 "type": type,
             }
         )
         if path is not UNSET:
             field_dict["path"] = path
         if lock is not UNSET:
             field_dict["lock"] = lock
+        if tag is not UNSET:
+            field_dict["tag"] = tag
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         input_transforms = RawScriptInputTransforms.from_dict(d.pop("input_transforms"))
@@ -69,21 +74,24 @@
 
         type = RawScriptType(d.pop("type"))
 
         path = d.pop("path", UNSET)
 
         lock = d.pop("lock", UNSET)
 
+        tag = d.pop("tag", UNSET)
+
         raw_script = cls(
             input_transforms=input_transforms,
             content=content,
             language=language,
             type=type,
             path=path,
             lock=lock,
+            tag=tag,
         )
 
         raw_script.additional_properties = d
         return raw_script
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.88.1/windmill_api/models/raw_script_input_transforms.py` & `windmill_api-1.89.0/windmill_api/models/raw_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.89.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.89.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/refresh_token_json_body.py` & `windmill_api-1.89.0/windmill_api/models/refresh_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/remove_granular_acls_json_body.py` & `windmill_api-1.89.0/windmill_api/models/remove_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/remove_owner_to_folder_json_body.py` & `windmill_api-1.89.0/windmill_api/models/remove_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/remove_user_to_group_json_body.py` & `windmill_api-1.89.0/windmill_api/models/remove_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/resource.py` & `windmill_api-1.89.0/windmill_api/models/resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/resource_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/resource_type.py` & `windmill_api-1.89.0/windmill_api/models/resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/resume_suspended_flow_as_owner_json_body.py` & `windmill_api-1.89.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/resume_suspended_job_post_json_body.py` & `windmill_api-1.89.0/windmill_api/models/resume_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/retry.py` & `windmill_api-1.89.0/windmill_api/models/retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_by_path_json_body.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_args.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_script_by_hash_json_body.py` & `windmill_api-1.89.0/windmill_api/models/run_script_by_hash_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_script_by_path_json_body.py` & `windmill_api-1.89.0/windmill_api/models/run_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_script_preview_json_body.py` & `windmill_api-1.89.0/windmill_api/models/run_script_preview_json_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,60 +13,68 @@
 class RunScriptPreviewJsonBody:
     """
     Attributes:
         content (str):
         args (RunScriptPreviewJsonBodyArgs):
         language (RunScriptPreviewJsonBodyLanguage):
         path (Union[Unset, str]):
+        tag (Union[Unset, str]):
     """
 
     content: str
     args: RunScriptPreviewJsonBodyArgs
     language: RunScriptPreviewJsonBodyLanguage
     path: Union[Unset, str] = UNSET
+    tag: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         content = self.content
         args = self.args.to_dict()
 
         language = self.language.value
 
         path = self.path
+        tag = self.tag
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "content": content,
                 "args": args,
                 "language": language,
             }
         )
         if path is not UNSET:
             field_dict["path"] = path
+        if tag is not UNSET:
+            field_dict["tag"] = tag
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         content = d.pop("content")
 
         args = RunScriptPreviewJsonBodyArgs.from_dict(d.pop("args"))
 
         language = RunScriptPreviewJsonBodyLanguage(d.pop("language"))
 
         path = d.pop("path", UNSET)
 
+        tag = d.pop("tag", UNSET)
+
         run_script_preview_json_body = cls(
             content=content,
             args=args,
             language=language,
             path=path,
+            tag=tag,
         )
 
         run_script_preview_json_body.additional_properties = d
         return run_script_preview_json_body
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.88.1/windmill_api/models/run_script_preview_json_body_args.py` & `windmill_api-1.89.0/windmill_api/models/run_script_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_wait_result_flow_by_path_json_body.py` & `windmill_api-1.89.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/run_wait_result_script_by_path_json_body.py` & `windmill_api-1.89.0/windmill_api/models/run_wait_result_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/schedule.py` & `windmill_api-1.89.0/windmill_api/models/schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/schedule_args.py` & `windmill_api-1.89.0/windmill_api/models/schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/schedule_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/schedule_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/script.py` & `windmill_api-1.89.0/windmill_api/models/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         starred (bool):
         workspace_id (Union[Unset, str]):
         parent_hashes (Union[Unset, List[str]]): The first element is the direct parent of the script, the second is the
             parent of the first, etc
         schema (Union[Unset, ScriptSchema]):
         lock (Union[Unset, str]):
         lock_error_logs (Union[Unset, str]):
+        tag (Union[Unset, str]):
     """
 
     hash_: str
     path: str
     summary: str
     description: str
     content: str
@@ -54,14 +55,15 @@
     kind: ScriptKind
     starred: bool
     workspace_id: Union[Unset, str] = UNSET
     parent_hashes: Union[Unset, List[str]] = UNSET
     schema: Union[Unset, ScriptSchema] = UNSET
     lock: Union[Unset, str] = UNSET
     lock_error_logs: Union[Unset, str] = UNSET
+    tag: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         hash_ = self.hash_
         path = self.path
         summary = self.summary
         description = self.description
@@ -86,14 +88,15 @@
 
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         lock = self.lock
         lock_error_logs = self.lock_error_logs
+        tag = self.tag
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "hash": hash_,
                 "path": path,
@@ -117,14 +120,16 @@
             field_dict["parent_hashes"] = parent_hashes
         if schema is not UNSET:
             field_dict["schema"] = schema
         if lock is not UNSET:
             field_dict["lock"] = lock
         if lock_error_logs is not UNSET:
             field_dict["lock_error_logs"] = lock_error_logs
+        if tag is not UNSET:
+            field_dict["tag"] = tag
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         hash_ = d.pop("hash")
@@ -166,14 +171,16 @@
         else:
             schema = ScriptSchema.from_dict(_schema)
 
         lock = d.pop("lock", UNSET)
 
         lock_error_logs = d.pop("lock_error_logs", UNSET)
 
+        tag = d.pop("tag", UNSET)
+
         script = cls(
             hash_=hash_,
             path=path,
             summary=summary,
             description=description,
             content=content,
             created_by=created_by,
@@ -186,14 +193,15 @@
             kind=kind,
             starred=starred,
             workspace_id=workspace_id,
             parent_hashes=parent_hashes,
             schema=schema,
             lock=lock,
             lock_error_logs=lock_error_logs,
+            tag=tag,
         )
 
         script.additional_properties = d
         return script
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.88.1/windmill_api/models/script_args.py` & `windmill_api-1.89.0/windmill_api/models/script_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/script_extra_perms.py` & `windmill_api-1.89.0/windmill_api/models/script_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/script_schema.py` & `windmill_api-1.89.0/windmill_api/models/script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/set_password_json_body.py` & `windmill_api-1.89.0/windmill_api/models/set_password_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/set_schedule_enabled_json_body.py` & `windmill_api-1.89.0/windmill_api/models/set_schedule_enabled_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/slack_token.py` & `windmill_api-1.89.0/windmill_api/models/slack_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/slack_token_bot.py` & `windmill_api-1.89.0/windmill_api/models/slack_token_bot.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/star_json_body.py` & `windmill_api-1.89.0/windmill_api/models/star_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/static_transform.py` & `windmill_api-1.89.0/windmill_api/models/static_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/token_response.py` & `windmill_api-1.89.0/windmill_api/models/token_response.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/truncated_token.py` & `windmill_api-1.89.0/windmill_api/models/truncated_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/unstar_json_body.py` & `windmill_api-1.89.0/windmill_api/models/unstar_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_app_json_body.py` & `windmill_api-1.89.0/windmill_api/models/update_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_app_json_body_policy.py` & `windmill_api-1.89.0/windmill_api/models/update_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_app_json_body_policy_triggerables.py` & `windmill_api-1.89.0/windmill_api/models/update_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.89.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_schema.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.89.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_folder_json_body.py` & `windmill_api-1.89.0/windmill_api/models/update_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_group_json_body.py` & `windmill_api-1.89.0/windmill_api/models/update_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_input.py` & `windmill_api-1.89.0/windmill_api/models/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_input_json_body.py` & `windmill_api-1.89.0/windmill_api/models/update_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_resource_json_body.py` & `windmill_api-1.89.0/windmill_api/models/update_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_resource_type_json_body.py` & `windmill_api-1.89.0/windmill_api/models/update_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_resource_value_json_body.py` & `windmill_api-1.89.0/windmill_api/models/update_resource_value_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_schedule_json_body.py` & `windmill_api-1.89.0/windmill_api/models/update_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_schedule_json_body_args.py` & `windmill_api-1.89.0/windmill_api/models/update_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_user_json_body.py` & `windmill_api-1.89.0/windmill_api/models/update_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/update_variable_json_body.py` & `windmill_api-1.89.0/windmill_api/models/update_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/usage.py` & `windmill_api-1.89.0/windmill_api/models/usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/user.py` & `windmill_api-1.89.0/windmill_api/models/user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/user_usage.py` & `windmill_api-1.89.0/windmill_api/models/user_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/user_workspace_list.py` & `windmill_api-1.89.0/windmill_api/models/user_workspace_list.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/user_workspace_list_workspaces_item.py` & `windmill_api-1.89.0/windmill_api/models/user_workspace_list_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/whoami_response_200.py` & `windmill_api-1.89.0/windmill_api/models/whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/whoami_response_200_usage.py` & `windmill_api-1.89.0/windmill_api/models/whoami_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/whois_response_200.py` & `windmill_api-1.89.0/windmill_api/models/whois_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/whois_response_200_usage.py` & `windmill_api-1.89.0/windmill_api/models/whois_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/worker_ping.py` & `windmill_api-1.89.0/windmill_api/models/worker_ping.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/workspace.py` & `windmill_api-1.89.0/windmill_api/models/workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/models/workspace_invite.py` & `windmill_api-1.89.0/windmill_api/models/workspace_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/windmill_api/types.py` & `windmill_api-1.89.0/windmill_api/types.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.88.1/setup.py` & `windmill_api-1.89.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=21.3.0', 'httpx>=0.15.4,<0.24.0', 'python-dateutil>=2.8.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'windmill-api',
-    'version': '1.88.1',
+    'version': '1.89.0',
     'description': 'A client library for accessing Windmill API',
     'long_description': '# Autogenerated Windmill OpenApi Client\nThis is the raw autogenerated api client. You are most likely more interested in [wmill](https://pypi.org/project/wmill/) which leverages this client to offer an user friendly experience. We use [this openapi python client generator](https://github.com/openapi-generators/openapi-python-client/)\n\n# windmill-api\nA client library for accessing Windmill API\n\n## Usage\nFirst, create a client:\n\n```python\nfrom windmill_api import Client\n\nclient = Client(base_url="https://api.example.com")\n```\n\nIf the endpoints you\'re going to hit require authentication, use `AuthenticatedClient` instead:\n\n```python\nfrom windmill_api import AuthenticatedClient\n\nclient = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken",\n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken", \n    verify_ssl=False\n)\n```\n\nThings to know:\n1. Every path/method combo becomes a Python module with four functions:\n    1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n    1. `asyncio`: Like `sync` but async instead of blocking\n    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `windmill_api.api.default`\n\n',
     'author': 'Ruben Fiszel',
     'author_email': 'ruben@windmill.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `windmill_api-1.88.1/PKG-INFO` & `windmill_api-1.89.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-api
-Version: 1.88.1
+Version: 1.89.0
 Summary: A client library for accessing Windmill API
 License: Apache-2.0
 Author: Ruben Fiszel
 Author-email: ruben@windmill.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

