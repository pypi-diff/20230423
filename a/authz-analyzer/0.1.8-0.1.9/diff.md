# Comparing `tmp/authz_analyzer-0.1.8.tar.gz` & `tmp/authz_analyzer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authz_analyzer-0.1.8.tar", max compression
+gzip compressed data, was "authz_analyzer-0.1.9.tar", max compression
```

## Comparing `authz_analyzer-0.1.8.tar` & `authz_analyzer-0.1.9.tar`

### file list

```diff
@@ -1,225 +1,238 @@
--rw-r--r--   0        0        0    11357 2023-03-13 10:06:06.900091 authz_analyzer-0.1.8/LICENSE
--rw-r--r--   0        0        0     2347 2023-03-13 10:06:06.900091 authz_analyzer-0.1.8/README.md
--rw-r--r--   0        0        0      827 2023-03-13 10:06:06.900091 authz_analyzer-0.1.8/authz_analyzer/__init__.py
--rw-r--r--   0        0        0     9100 2023-03-13 10:06:06.900091 authz_analyzer-0.1.8/authz_analyzer/cli.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.900091 authz_analyzer-0.1.8/authz_analyzer/datastores/__init__.py
--rw-r--r--   0        0        0      626 2023-03-13 10:06:06.900091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/__init__.py
--rw-r--r--   0        0        0      113 2023-03-13 10:06:06.900091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/__init__.py
--rw-r--r--   0        0        0     3172 2023-03-13 10:06:06.900091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/analyzer.py
--rw-r--r--   0        0        0     7099 2023-03-13 10:06:06.900091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/exporter.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.900091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/__init__.py
--rw-r--r--   0        0        0    12696 2023-03-13 10:06:06.900091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/analyzer.py
--rw-r--r--   0        0        0       90 2023-03-13 10:06:06.900091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/commands/all_databases.sql
--rw-r--r--   0        0        0      141 2023-03-13 10:06:06.900091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/commands/all_tables.sql
--rw-r--r--   0        0        0      111 2023-03-13 10:06:06.900091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/commands/datashare_consumers.sql
--rw-r--r--   0        0        0       14 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/commands/datashare_desc.sql
--rw-r--r--   0        0        0      125 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/commands/datashares.sql
--rw-r--r--   0        0        0      893 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/commands/identities.sql
--rw-r--r--   0        0        0      262 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/commands/identities_privileges.sql
--rw-r--r--   0        0        0     5422 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/exporter.py
--rw-r--r--   0        0        0     3504 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/model.py
--rw-r--r--   0        0        0      660 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/service.py
--rw-r--r--   0        0        0       81 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/actions/__init__.py
--rw-r--r--   0        0        0     3041 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py
--rw-r--r--   0        0        0     2045 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/__init__.py
--rw-r--r--   0        0        0     5028 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py
--rw-r--r--   0        0        0     3505 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py
--rw-r--r--   0        0        0     2481 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py
--rw-r--r--   0        0        0     6201 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py
--rw-r--r--   0        0        0     3963 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py
--rw-r--r--   0        0        0      254 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/__init__.py
--rw-r--r--   0        0        0       87 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/effect.py
--rw-r--r--   0        0        0      263 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/group_policy.py
--rw-r--r--   0        0        0      415 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy.py
--rw-r--r--   0        0        0     5854 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py
--rw-r--r--   0        0        0    10500 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py
--rw-r--r--   0        0        0      373 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_utils.py
--rw-r--r--   0        0        0      261 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/user_policy.py
--rw-r--r--   0        0        0      263 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/public_block_access_config.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/__init__.py
--rw-r--r--   0        0        0      261 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/role_policy.py
--rw-r--r--   0        0        0      263 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/__init__.py
--rw-r--r--   0        0        0    18760 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py
--rw-r--r--   0        0        0      172 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/__init__.py
--rw-r--r--   0        0        0    12130 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py
--rw-r--r--   0        0        0     1267 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py
--rw-r--r--   0        0        0    12301 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py
--rw-r--r--   0        0        0     3704 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py
--rw-r--r--   0        0        0     9066 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/__init__.py
--rw-r--r--   0        0        0    11330 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py
--rw-r--r--   0        0        0     7437 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py
--rw-r--r--   0        0        0    13540 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py
--rw-r--r--   0        0        0    21197 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py
--rw-r--r--   0        0        0     5660 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py
--rw-r--r--   0        0        0      513 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py
--rw-r--r--   0        0        0     8356 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/resources/__init__.py
--rw-r--r--   0        0        0     5233 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py
--rw-r--r--   0        0        0     4475 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py
--rw-r--r--   0        0        0     1644 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/__init__.py
--rw-r--r--   0        0        0     2905 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py
--rw-r--r--   0        0        0     6158 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py
--rw-r--r--   0        0        0     2185 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/__init__.py
--rw-r--r--   0        0        0     2147 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py
--rw-r--r--   0        0        0     7453 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py
--rw-r--r--   0        0        0     2289 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py
--rw-r--r--   0        0        0     2594 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/__init__.py
--rw-r--r--   0        0        0     3377 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py
--rw-r--r--   0        0        0      936 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py
--rw-r--r--   0        0        0    17633 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py
--rw-r--r--   0        0        0     7562 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py
--rw-r--r--   0        0        0     1894 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py
--rw-r--r--   0        0        0      398 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_base.py
--rw-r--r--   0        0        0     1973 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py
--rw-r--r--   0        0        0     3041 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py
--rw-r--r--   0        0        0      397 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_base.py
--rw-r--r--   0        0        0      561 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py
--rw-r--r--   0        0        0     2501 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py
--rw-r--r--   0        0        0     9989 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/__init__.py
--rw-r--r--   0        0        0      879 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py
--rw-r--r--   0        0        0     1000 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py
--rw-r--r--   0        0        0     2747 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py
--rw-r--r--   0        0        0      173 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/serde.py
--rw-r--r--   0        0        0      131 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/bigquery/__init__.py
--rw-r--r--   0        0        0    11607 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/bigquery/analyzer.py
--rw-r--r--   0        0        0    12669 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/bigquery/policy_tree.py
--rw-r--r--   0        0        0     7504 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/bigquery/service.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/__init__.py
--rw-r--r--   0        0        0    15935 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/analyzer.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/atlas/__init__.py
--rw-r--r--   0        0        0    17290 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/atlas/analyzer.py
--rw-r--r--   0        0        0     6132 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/atlas/model.py
--rw-r--r--   0        0        0     2487 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/atlas/permission_resolvers.py
--rw-r--r--   0        0        0     5832 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/atlas/service.py
--rw-r--r--   0        0        0     2394 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/atlas/service_model.py
--rw-r--r--   0        0        0     2157 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/model.py
--rw-r--r--   0        0        0     1533 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/resolvers.py
--rw-r--r--   0        0        0     1408 2023-03-13 10:06:06.904091 authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/service.py
--rw-r--r--   0        0        0     1196 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/service_model.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/__init__.py
--rw-r--r--   0        0        0    10121 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/analyzer.py
--rw-r--r--   0        0        0       71 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/commands/all_databases.sql
--rw-r--r--   0        0        0      369 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/commands/all_tables.sql
--rw-r--r--   0        0        0      272 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/commands/roles.sql
--rw-r--r--   0        0        0      313 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/commands/roles_grants.sql
--rw-r--r--   0        0        0     2403 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/database_query_results.py
--rw-r--r--   0        0        0      822 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/deployment.py
--rw-r--r--   0        0        0     2627 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/exporter.py
--rw-r--r--   0        0        0     1852 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/model.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/snowflake/__init__.py
--rw-r--r--   0        0        0    11171 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/snowflake/analyzer.py
--rw-r--r--   0        0        0      389 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/snowflake/commands/grants_roles.sql
--rw-r--r--   0        0        0       20 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/snowflake/commands/grants_to_share.sql
--rw-r--r--   0        0        0       11 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/snowflake/commands/shares.sql
--rw-r--r--   0        0        0      535 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/snowflake/commands/user_grants.sql
--rw-r--r--   0        0        0     5747 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/snowflake/exporter.py
--rw-r--r--   0        0        0     4665 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/snowflake/model.py
--rw-r--r--   0        0        0     1048 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/datastores/snowflake/service.py
--rw-r--r--   0        0        0     6059 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/main.py
--rw-r--r--   0        0        0      175 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/models/__init__.py
--rw-r--r--   0        0        0     7019 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/models/model.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/utils/__init__.py
--rw-r--r--   0        0        0      651 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/utils/logger.py
--rw-r--r--   0        0        0      372 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/writers/__init__.py
--rw-r--r--   0        0        0     1000 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/writers/base_writers.py
--rw-r--r--   0        0        0      688 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/writers/csv_writer.py
--rw-r--r--   0        0        0     1078 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/writers/get_writers.py
--rw-r--r--   0        0        0     2050 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/authz_analyzer/writers/multi_json_exporter.py
--rw-r--r--   0        0        0     3003 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       44 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/mocks/__init__.py
--rw-r--r--   0        0        0      701 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/mocks/mock_writers.py
--rw-r--r--   0        0        0     1028 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/test_authz_analyzer.py
--rw-r--r--   0        0        0     4708 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/test_cli.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/test_writers/__init__.py
--rw-r--r--   0        0        0     1315 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/test_writers/test_csv_writer.py
--rw-r--r--   0        0        0      913 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/test_writers/test_multijson_writer.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/tests_datastores/__init__.py
--rw-r--r--   0        0        0        1 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/tests_datastores/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/__init__.py
--rw-r--r--   0        0        0    14110 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json
--rw-r--r--   0        0        0    11644 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json
--rw-r--r--   0        0        0    14917 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json
--rw-r--r--   0        0        0     9884 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json
--rw-r--r--   0        0        0    20662 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json
--rw-r--r--   0        0        0    31812 2023-03-13 10:06:06.908091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json
--rw-r--r--   0        0        0    18235 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json
--rw-r--r--   0        0        0    17618 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json
--rw-r--r--   0        0        0     7529 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json
--rw-r--r--   0        0        0     7744 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json
--rw-r--r--   0        0        0     4073 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json
--rw-r--r--   0        0        0    20163 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json
--rw-r--r--   0        0        0    13494 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json
--rw-r--r--   0        0        0     8446 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json
--rw-r--r--   0        0        0    16466 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json
--rw-r--r--   0        0        0    16126 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json
--rw-r--r--   0        0        0    14831 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json
--rw-r--r--   0        0        0     3066 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json
--rw-r--r--   0        0        0     5550 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json
--rw-r--r--   0        0        0     5906 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json
--rw-r--r--   0        0        0     4446 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json
--rw-r--r--   0        0        0     8937 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json
--rw-r--r--   0        0        0    20162 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json
--rw-r--r--   0        0        0    10324 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json
--rw-r--r--   0        0        0     6886 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json
--rw-r--r--   0        0        0    23422 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json
--rw-r--r--   0        0        0     2358 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json
--rw-r--r--   0        0        0     7124 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json
--rw-r--r--   0        0        0     4549 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json
--rw-r--r--   0        0        0     5215 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json
--rw-r--r--   0        0        0     5987 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json
--rw-r--r--   0        0        0     5862 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json
--rw-r--r--   0        0        0     3396 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json
--rw-r--r--   0        0        0     2298 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json
--rw-r--r--   0        0        0     5264 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json
--rw-r--r--   0        0        0     4596 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json
--rw-r--r--   0        0        0     3653 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json
--rw-r--r--   0        0        0     4392 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json
--rw-r--r--   0        0        0    26158 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json
--rw-r--r--   0        0        0    10097 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json
--rw-r--r--   0        0        0     8580 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json
--rw-r--r--   0        0        0    33775 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json
--rw-r--r--   0        0        0    16439 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json
--rw-r--r--   0        0        0    13955 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json
--rw-r--r--   0        0        0    18162 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json
--rw-r--r--   0        0        0     3040 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json
--rw-r--r--   0        0        0     5254 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json
--rw-r--r--   0        0        0     3569 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json
--rw-r--r--   0        0        0     4436 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json
--rw-r--r--   0        0        0    14441 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json
--rw-r--r--   0        0        0     3582 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py
--rw-r--r--   0        0        0     4794 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py
--rw-r--r--   0        0        0     4744 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/utils/__init__.py
--rw-r--r--   0        0        0     2311 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py
--rw-r--r--   0        0        0     1595 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json
--rw-r--r--   0        0        0     2597 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json
--rw-r--r--   0        0        0     2321 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json
--rw-r--r--   0        0        0     4018 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json
--rw-r--r--   0        0        0     5298 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json
--rw-r--r--   0        0        0     1539 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/test_exporter.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/utils/__init__.py
--rw-r--r--   0        0        0     1731 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/bigquery/__init__.py
--rw-r--r--   0        0        0     5576 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/bigquery/generate_authz_entry.py
--rw-r--r--   0        0        0     6916 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/bigquery/mocks.py
--rw-r--r--   0        0        0    15479 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/bigquery/test_bigquery.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/mongodb/__init__.py
--rw-r--r--   0        0        0    14412 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/mongodb/test_atlas_organization_users.py
--rw-r--r--   0        0        0     7291 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/mongodb/test_mongodb.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/postgres/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/postgres/mocks/__init__.py
--rw-r--r--   0        0        0     1195 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py
--rw-r--r--   0        0        0    12831 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/postgres/test_postgress_analyzer.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/redshift/__init__.py
--rw-r--r--   0        0        0    12099 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/redshift/test_redshift.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/snowflake/__init__.py
--rw-r--r--   0        0        0    14290 2023-03-13 10:06:06.912091 authz_analyzer-0.1.8/tests/tests_datastores/snowflake/test_snowflake_analyzer.py
--rw-r--r--   0        0        0     4997 1970-01-01 00:00:00.000000 authz_analyzer-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2347 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/README.md
+-rw-r--r--   0        0        0      925 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/__init__.py
+-rw-r--r--   0        0        0     9100 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/cli.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/__init__.py
+-rw-r--r--   0        0        0      626 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/__init__.py
+-rw-r--r--   0        0        0      113 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/__init__.py
+-rw-r--r--   0        0        0     3172 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/analyzer.py
+-rw-r--r--   0        0        0     7099 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/exporter.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/__init__.py
+-rw-r--r--   0        0        0    12696 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/analyzer.py
+-rw-r--r--   0        0        0       90 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/commands/all_databases.sql
+-rw-r--r--   0        0        0      141 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/commands/all_tables.sql
+-rw-r--r--   0        0        0      111 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/commands/datashare_consumers.sql
+-rw-r--r--   0        0        0       14 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/commands/datashare_desc.sql
+-rw-r--r--   0        0        0      125 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/commands/datashares.sql
+-rw-r--r--   0        0        0      893 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/commands/identities.sql
+-rw-r--r--   0        0        0      262 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/commands/identities_privileges.sql
+-rw-r--r--   0        0        0     5422 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/exporter.py
+-rw-r--r--   0        0        0     3504 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/model.py
+-rw-r--r--   0        0        0      660 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/service.py
+-rw-r--r--   0        0        0       81 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/actions/__init__.py
+-rw-r--r--   0        0        0     3041 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py
+-rw-r--r--   0        0        0     2045 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/__init__.py
+-rw-r--r--   0        0        0     5028 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py
+-rw-r--r--   0        0        0     3505 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py
+-rw-r--r--   0        0        0     2481 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py
+-rw-r--r--   0        0        0     6201 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py
+-rw-r--r--   0        0        0     3963 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py
+-rw-r--r--   0        0        0      254 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/__init__.py
+-rw-r--r--   0        0        0       87 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/effect.py
+-rw-r--r--   0        0        0      263 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/group_policy.py
+-rw-r--r--   0        0        0      415 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy.py
+-rw-r--r--   0        0        0     5854 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py
+-rw-r--r--   0        0        0    10500 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py
+-rw-r--r--   0        0        0      373 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_utils.py
+-rw-r--r--   0        0        0      261 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/user_policy.py
+-rw-r--r--   0        0        0      263 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/public_block_access_config.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/__init__.py
+-rw-r--r--   0        0        0      261 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/role_policy.py
+-rw-r--r--   0        0        0      263 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/__init__.py
+-rw-r--r--   0        0        0    18760 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py
+-rw-r--r--   0        0        0      172 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/__init__.py
+-rw-r--r--   0        0        0    12130 2023-03-21 18:31:07.576223 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py
+-rw-r--r--   0        0        0     1267 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py
+-rw-r--r--   0        0        0    12301 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py
+-rw-r--r--   0        0        0     3704 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py
+-rw-r--r--   0        0        0     9066 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/__init__.py
+-rw-r--r--   0        0        0    11330 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py
+-rw-r--r--   0        0        0     7437 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py
+-rw-r--r--   0        0        0    13540 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py
+-rw-r--r--   0        0        0    21197 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py
+-rw-r--r--   0        0        0     5660 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py
+-rw-r--r--   0        0        0      513 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py
+-rw-r--r--   0        0        0     8356 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/resources/__init__.py
+-rw-r--r--   0        0        0     5233 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py
+-rw-r--r--   0        0        0     4475 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py
+-rw-r--r--   0        0        0     1644 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/__init__.py
+-rw-r--r--   0        0        0     2905 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py
+-rw-r--r--   0        0        0     6158 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py
+-rw-r--r--   0        0        0     2185 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/__init__.py
+-rw-r--r--   0        0        0     2147 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py
+-rw-r--r--   0        0        0     7453 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py
+-rw-r--r--   0        0        0     2289 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py
+-rw-r--r--   0        0        0     2594 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/__init__.py
+-rw-r--r--   0        0        0     3377 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py
+-rw-r--r--   0        0        0      936 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py
+-rw-r--r--   0        0        0    17633 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py
+-rw-r--r--   0        0        0     7562 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py
+-rw-r--r--   0        0        0     1894 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py
+-rw-r--r--   0        0        0      398 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_base.py
+-rw-r--r--   0        0        0     1973 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py
+-rw-r--r--   0        0        0     3041 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py
+-rw-r--r--   0        0        0      397 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_base.py
+-rw-r--r--   0        0        0      561 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py
+-rw-r--r--   0        0        0     2501 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py
+-rw-r--r--   0        0        0     9989 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/__init__.py
+-rw-r--r--   0        0        0      879 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py
+-rw-r--r--   0        0        0     1000 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py
+-rw-r--r--   0        0        0     2747 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py
+-rw-r--r--   0        0        0      173 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/serde.py
+-rw-r--r--   0        0        0      131 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/bigquery/__init__.py
+-rw-r--r--   0        0        0    11607 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/bigquery/analyzer.py
+-rw-r--r--   0        0        0    12669 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/bigquery/policy_tree.py
+-rw-r--r--   0        0        0     7504 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/bigquery/service.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/databricks/__init__.py
+-rw-r--r--   0        0        0     5021 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/databricks/analyzer.py
+-rw-r--r--   0        0        0       53 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/databricks/exceptions.py
+-rw-r--r--   0        0        0     8186 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/databricks/identities.py
+-rw-r--r--   0        0        0     1331 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/databricks/model.py
+-rw-r--r--   0        0        0    10088 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/databricks/policy_tree.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/databricks/service/__init__.py
+-rw-r--r--   0        0        0     2412 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/databricks/service/model.py
+-rw-r--r--   0        0        0     1388 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/databricks/service/scim.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/__init__.py
+-rw-r--r--   0        0        0    15935 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/analyzer.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.580222 authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/atlas/__init__.py
+-rw-r--r--   0        0        0    17262 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/atlas/analyzer.py
+-rw-r--r--   0        0        0     6132 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/atlas/model.py
+-rw-r--r--   0        0        0     2487 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/atlas/permission_resolvers.py
+-rw-r--r--   0        0        0     5832 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/atlas/service.py
+-rw-r--r--   0        0        0     2394 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/atlas/service_model.py
+-rw-r--r--   0        0        0     2157 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/model.py
+-rw-r--r--   0        0        0     1533 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/resolvers.py
+-rw-r--r--   0        0        0     1408 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/service.py
+-rw-r--r--   0        0        0     1196 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/service_model.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/__init__.py
+-rw-r--r--   0        0        0    10188 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/analyzer.py
+-rw-r--r--   0        0        0       71 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/commands/all_databases.sql
+-rw-r--r--   0        0        0      369 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/commands/all_tables.sql
+-rw-r--r--   0        0        0      272 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/commands/roles.sql
+-rw-r--r--   0        0        0      313 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/commands/roles_grants.sql
+-rw-r--r--   0        0        0     2404 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/database_query_results.py
+-rw-r--r--   0        0        0      822 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/deployment.py
+-rw-r--r--   0        0        0     2627 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/exporter.py
+-rw-r--r--   0        0        0     1851 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/model.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/snowflake/__init__.py
+-rw-r--r--   0        0        0    11171 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/snowflake/analyzer.py
+-rw-r--r--   0        0        0      389 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/snowflake/commands/grants_roles.sql
+-rw-r--r--   0        0        0       20 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/snowflake/commands/grants_to_share.sql
+-rw-r--r--   0        0        0       11 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/snowflake/commands/shares.sql
+-rw-r--r--   0        0        0      535 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/snowflake/commands/user_grants.sql
+-rw-r--r--   0        0        0     5747 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/snowflake/exporter.py
+-rw-r--r--   0        0        0     4665 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/snowflake/model.py
+-rw-r--r--   0        0        0     1048 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/datastores/snowflake/service.py
+-rw-r--r--   0        0        0     6059 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/main.py
+-rw-r--r--   0        0        0      175 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/models/__init__.py
+-rw-r--r--   0        0        0     7362 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/models/model.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/utils/__init__.py
+-rw-r--r--   0        0        0      651 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/utils/logger.py
+-rw-r--r--   0        0        0      372 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/writers/__init__.py
+-rw-r--r--   0        0        0     1000 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/writers/base_writers.py
+-rw-r--r--   0        0        0      688 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/writers/csv_writer.py
+-rw-r--r--   0        0        0     1078 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/writers/get_writers.py
+-rw-r--r--   0        0        0     2050 2023-03-21 18:31:07.584222 authz_analyzer-0.1.9/authz_analyzer/writers/multi_json_exporter.py
+-rw-r--r--   0        0        0     3030 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/mocks/__init__.py
+-rw-r--r--   0        0        0      701 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/mocks/mock_writers.py
+-rw-r--r--   0        0        0     1028 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/test_authz_analyzer.py
+-rw-r--r--   0        0        0     4708 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/test_cli.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/test_writers/__init__.py
+-rw-r--r--   0        0        0     1315 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/test_writers/test_csv_writer.py
+-rw-r--r--   0        0        0      913 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/test_writers/test_multijson_writer.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/__init__.py
+-rw-r--r--   0        0        0        1 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/__init__.py
+-rw-r--r--   0        0        0    14110 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json
+-rw-r--r--   0        0        0    11644 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json
+-rw-r--r--   0        0        0    14917 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json
+-rw-r--r--   0        0        0     9884 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json
+-rw-r--r--   0        0        0    20662 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json
+-rw-r--r--   0        0        0    31812 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json
+-rw-r--r--   0        0        0    18235 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json
+-rw-r--r--   0        0        0    17618 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json
+-rw-r--r--   0        0        0     7529 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json
+-rw-r--r--   0        0        0     7744 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json
+-rw-r--r--   0        0        0     4073 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json
+-rw-r--r--   0        0        0    20163 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json
+-rw-r--r--   0        0        0    13494 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json
+-rw-r--r--   0        0        0     8446 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json
+-rw-r--r--   0        0        0    16466 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json
+-rw-r--r--   0        0        0    16126 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json
+-rw-r--r--   0        0        0    14831 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json
+-rw-r--r--   0        0        0     3066 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json
+-rw-r--r--   0        0        0     5550 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json
+-rw-r--r--   0        0        0     5906 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json
+-rw-r--r--   0        0        0     4446 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json
+-rw-r--r--   0        0        0     8937 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json
+-rw-r--r--   0        0        0    20162 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json
+-rw-r--r--   0        0        0    10324 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json
+-rw-r--r--   0        0        0     6886 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json
+-rw-r--r--   0        0        0    23422 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json
+-rw-r--r--   0        0        0     2358 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json
+-rw-r--r--   0        0        0     7124 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json
+-rw-r--r--   0        0        0     4549 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json
+-rw-r--r--   0        0        0     5215 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json
+-rw-r--r--   0        0        0     5987 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json
+-rw-r--r--   0        0        0     5862 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json
+-rw-r--r--   0        0        0     3396 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json
+-rw-r--r--   0        0        0     2298 2023-03-21 18:31:07.588222 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json
+-rw-r--r--   0        0        0     5264 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json
+-rw-r--r--   0        0        0     4596 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json
+-rw-r--r--   0        0        0     3653 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json
+-rw-r--r--   0        0        0     4392 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json
+-rw-r--r--   0        0        0    26158 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json
+-rw-r--r--   0        0        0    10097 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json
+-rw-r--r--   0        0        0     8580 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json
+-rw-r--r--   0        0        0    33775 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json
+-rw-r--r--   0        0        0    16439 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json
+-rw-r--r--   0        0        0    13955 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json
+-rw-r--r--   0        0        0    18162 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json
+-rw-r--r--   0        0        0     3040 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json
+-rw-r--r--   0        0        0     5254 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json
+-rw-r--r--   0        0        0     3569 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json
+-rw-r--r--   0        0        0     4436 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json
+-rw-r--r--   0        0        0    14441 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json
+-rw-r--r--   0        0        0     3582 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py
+-rw-r--r--   0        0        0     4794 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py
+-rw-r--r--   0        0        0     4744 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/utils/__init__.py
+-rw-r--r--   0        0        0     2311 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py
+-rw-r--r--   0        0        0     1595 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json
+-rw-r--r--   0        0        0     2597 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json
+-rw-r--r--   0        0        0     2321 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json
+-rw-r--r--   0        0        0     4018 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json
+-rw-r--r--   0        0        0     5298 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json
+-rw-r--r--   0        0        0     1539 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/test_exporter.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/utils/__init__.py
+-rw-r--r--   0        0        0     1731 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/bigquery/__init__.py
+-rw-r--r--   0        0        0     5576 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/bigquery/generate_authz_entry.py
+-rw-r--r--   0        0        0     6916 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/bigquery/mocks.py
+-rw-r--r--   0        0        0    15479 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/bigquery/test_bigquery.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/databricks/__init__.py
+-rw-r--r--   0        0        0    17883 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/databricks/generate_authz_entry.py
+-rw-r--r--   0        0        0     8709 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/databricks/mocks.py
+-rw-r--r--   0        0        0     7642 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/databricks/test_analyzer.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/mongodb/__init__.py
+-rw-r--r--   0        0        0    14412 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/mongodb/test_atlas_organization_users.py
+-rw-r--r--   0        0        0     7291 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/mongodb/test_mongodb.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/postgres/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/postgres/mocks/__init__.py
+-rw-r--r--   0        0        0     1195 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py
+-rw-r--r--   0        0        0    12830 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/postgres/test_postgress_analyzer.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/redshift/__init__.py
+-rw-r--r--   0        0        0    12099 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/redshift/test_redshift.py
+-rw-r--r--   0        0        0        0 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/snowflake/__init__.py
+-rw-r--r--   0        0        0    14290 2023-03-21 18:31:07.592223 authz_analyzer-0.1.9/tests/tests_datastores/snowflake/test_snowflake_analyzer.py
+-rw-r--r--   0        0        0     5046 1970-01-01 00:00:00.000000 authz_analyzer-0.1.9/PKG-INFO
```

### Comparing `authz_analyzer-0.1.8/LICENSE` & `authz_analyzer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/README.md` & `authz_analyzer-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/__init__.py` & `authz_analyzer-0.1.9/authz_analyzer/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Top-level package for authz-analyzer."""
 
 __author__ = """SatoriCyber"""
 __email__ = 'contact@satoricyber.com'
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 from authz_analyzer.datastores.aws.analyzer import AwsAssumeRoleInput, AWSAuthzAnalyzer  # type: ignore
 from authz_analyzer.datastores.aws.analyzer.redshift.analyzer import RedshiftAuthzAnalyzer  # type: ignore
 from authz_analyzer.datastores.bigquery.analyzer import BigQueryAuthzAnalyzer  # type: ignore
+from authz_analyzer.datastores.databricks.analyzer import DatabricksAuthzAnalyzer  # type: ignore
 from authz_analyzer.datastores.mongodb.analyzer import MongoDBAuthzAnalyzer  # type: ignore
 from authz_analyzer.datastores.mongodb.atlas.analyzer import MongoDBAtlasAuthzAnalyzer  # type: ignore
 from authz_analyzer.datastores.postgres.analyzer import PostgresAuthzAnalyzer  # type: ignore
 from authz_analyzer.datastores.snowflake.analyzer import SnowflakeAuthzAnalyzer  # type: ignore
```

### Comparing `authz_analyzer-0.1.8/authz_analyzer/cli.py` & `authz_analyzer-0.1.9/authz_analyzer/cli.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/__init__.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/analyzer.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/exporter.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/exporter.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/analyzer.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/analyzer.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/commands/identities.sql` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/commands/identities.sql`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/exporter.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/exporter.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/model.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/model.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/analyzer/redshift/service.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/analyzer/redshift/service.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/bigquery/analyzer.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/bigquery/analyzer.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/bigquery/policy_tree.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/bigquery/policy_tree.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/bigquery/service.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/bigquery/service.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/analyzer.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/analyzer.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/atlas/analyzer.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/atlas/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,17 +110,17 @@
         """Connect to the MongoDB atlas.
         Tries to authenticate with the provided credentials to the base API.
         Because Atlas is REST API, there is no notion of a connection.
         """
         if logger is None:
             logger = get_logger(False)
         logger.info("Starting to scan project %s, cluster %s", project_name, cluster_name)
-        
-        writer = get_writer(filename=output_path, output_format=output_format)            
-        
+
+        writer = get_writer(filename=output_path, output_format=output_format)
+
         service = AtlasService.connect(public_key, private_key)
         return cls(
             atlas_service=service,
             writer=writer,
             logger=logger,
             db_user=db_user,
             db_password=db_password,
```

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/atlas/model.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/atlas/model.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/atlas/permission_resolvers.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/atlas/permission_resolvers.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/atlas/service.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/atlas/service.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/atlas/service_model.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/atlas/service_model.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/model.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/model.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/resolvers.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/resolvers.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/service.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/service.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/mongodb/service_model.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/mongodb/service_model.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/analyzer.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,34 +13,33 @@
 
 from dataclasses import dataclass
 from logging import Logger
 from pathlib import Path
 from typing import Any, Dict, Generator, List, Optional, Set, Tuple, Union
 
 import psycopg2
-from psycopg2.extensions import ISOLATION_LEVEL_AUTOCOMMIT, cursor, connection
+from psycopg2.extensions import ISOLATION_LEVEL_AUTOCOMMIT, connection, cursor
 
 from authz_analyzer.datastores.postgres import exporter
+from authz_analyzer.datastores.postgres.database_query_results import DataBaseAcl
+from authz_analyzer.datastores.postgres.database_query_results import RoleGrant as DataBaseRoleGrant
+from authz_analyzer.datastores.postgres.deployment import Deployment
 from authz_analyzer.datastores.postgres.model import (
     PERMISSION_LEVEL_MAP,
     RESOURCE_TYPE_MAP,
     AuthorizationModel,
     DBRole,
     ResourceGrant,
     RoleName,
 )
 from authz_analyzer.models.model import AssetType, PermissionLevel
 from authz_analyzer.utils.logger import get_logger
 from authz_analyzer.writers import BaseWriter, OutputFormat, get_writer
 from authz_analyzer.writers.base_writers import DEFAULT_OUTPUT_FILE
 
-from authz_analyzer.datastores.postgres.database_query_results import DataBaseAcl, RoleGrant as DataBaseRoleGrant
-
-from authz_analyzer.datastores.postgres.deployment import Deployment
-
 COMMANDS_DIR = Path(__file__).parent / "commands"
 
 DbName = str
 
 
 @dataclass
 class PostgresAuthzAnalyzer:
```

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/database_query_results.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/database_query_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from enum import Enum
 from logging import Logger
 from typing import List, NamedTuple, Optional
 
 
 class RoleGrant(NamedTuple):
     resource_name: str
```

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/deployment.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/deployment.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/exporter.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/exporter.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/postgres/model.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/postgres/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Dict, List, Set
 
 from authz_analyzer.models import PermissionLevel
-
 from authz_analyzer.models.model import AssetType
 
 RoleName = str
 
 RESOURCE_TYPE_MAP = {
     "r": AssetType.TABLE,
     "t": AssetType.TOAST_TABLE,
```

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/snowflake/analyzer.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/snowflake/analyzer.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/snowflake/commands/user_grants.sql` & `authz_analyzer-0.1.9/authz_analyzer/datastores/snowflake/commands/user_grants.sql`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/snowflake/exporter.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/snowflake/exporter.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/snowflake/model.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/snowflake/model.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/datastores/snowflake/service.py` & `authz_analyzer-0.1.9/authz_analyzer/datastores/snowflake/service.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/main.py` & `authz_analyzer-0.1.9/authz_analyzer/main.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/models/model.py` & `authz_analyzer-0.1.9/authz_analyzer/models/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,22 +15,25 @@
 from serde import field as serde_field  # pylint: disable=import-error #type: ignore
 from serde import serde  # pylint: disable=import-error #type: ignore
 
 
 class AssetType(Enum):
     """Types of assets that are stored at the datastores."""
 
-    TABLE = auto()
-    VIEW = auto()
-    MATERIALIZED_VIEW = auto()
-    S3_BUCKET = auto()  # AWS S3
-    COLLECTION = auto()  # MongoDB collection
-    TOAST_TABLE = auto()  # Postgres
-    FOREIGN_TABLE = auto()  # Postgres
-    PARTITION_TABLE = auto()  # Postgres
+    TABLE = "TABLE"
+    VIEW = "VIEW"
+    MATERIALIZED_VIEW = "MATERIALIZED_VIEW"
+    S3_BUCKET = "S3_BUCKET"  # AWS S3
+    COLLECTION = "COLLECTION"  # MongoDB collection
+    TOAST_TABLE = "TOAST_TABLE"  # Postgres
+    FOREIGN_TABLE = "FOREIGN_TABLE"  # Postgres
+    PARTITION_TABLE = "PARTITION_TABLE"  # Postgres
+    EXTERNAL = "EXTERNAL"  # Databricks
+    MANAGED = "MANAGED"  # Databricks
+    STREAMING_TABLE = "STREAMING_TABLE"  # Databricks
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return self.name
 
@@ -57,14 +60,15 @@
     SAML_SESSION = auto()  # AWS
     FEDERATED_USER = auto()  # AWS
     ANONYMOUS_USER = auto()  # AWS
     ACCOUNT = auto()  # Snowflake
     DB_USER = auto()  # MongoDB Atlas
     ORG_USER = auto()  # MongoDB Atlas
     CLUSTER = auto()  # AWS Redshift Cluster
+    SERVICE_PRINCIPAL = auto()  # Databricks
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return self.name
 
@@ -95,14 +99,17 @@
     WEB_IDENTITY_SESSION = auto()  # AWS
     SAML_SESSION = auto()  # AWS
     FEDERATED_USER = auto()  # AWS
     ANONYMOUS_USER = auto()  # AWS
     CLUSTER = auto()  # Mongo Atlas
     RESOURCE_POLICY = auto()  # AWS
     SHARE = auto()  # Snowflake
+    CATALOG = auto()  # Databricks
+    SCHEMA = auto()  # Databricks
+    SERVICE_PRINCIPAL = auto()  # Databricks
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return self.name
```

### Comparing `authz_analyzer-0.1.8/authz_analyzer/utils/logger.py` & `authz_analyzer-0.1.9/authz_analyzer/utils/logger.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/writers/base_writers.py` & `authz_analyzer-0.1.9/authz_analyzer/writers/base_writers.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/writers/csv_writer.py` & `authz_analyzer-0.1.9/authz_analyzer/writers/csv_writer.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/writers/get_writers.py` & `authz_analyzer-0.1.9/authz_analyzer/writers/get_writers.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/authz_analyzer/writers/multi_json_exporter.py` & `authz_analyzer-0.1.9/authz_analyzer/writers/multi_json_exporter.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/pyproject.toml` & `authz_analyzer-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "authz-analyzer"
-version = "0.1.8"
+version = "0.1.9"
 homepage = "https://github.com/satoricyber/authz-analyzer"
 description = "Analyze authorization."
 authors = ["SatoriCyber"]
 readme = "README.md"
 classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
@@ -53,14 +53,15 @@
 bump2version = {version="^1.0.1", optional=true}
 mkdocs = {version="^1.4.2", optional=true}
 pylint = {version="^2.16.2", optional=true}
 pyright = {version="^1.1.293", optional=true}
 mkdocs-material = {version="^9.0.12", optional=true}
 mkdocs-include-markdown-plugin = {version = "^4.0.3", optional=true}
 markdown-it-py = {version = "^2.2.0", optional=true}
+databricks-cli = "^0.17.4"
 
 [tool.poetry.extras]
 test = ["pytest", "pytest-cov", "black", "isort", "twine", "mypy", "types-psycopg2", 
         "google-api-python-client-stubs", "types-requests", "pylint", "pyright", "bump2version"]
 release = ["twine", "mkdocs", "mkdocs-material", "mkdocs-include-markdown-plugin"]
 
 [tool.poetry.scripts]
```

### Comparing `authz_analyzer-0.1.8/tests/mocks/mock_writers.py` & `authz_analyzer-0.1.9/tests/mocks/mock_writers.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/test_authz_analyzer.py` & `authz_analyzer-0.1.9/tests/test_authz_analyzer.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/test_cli.py` & `authz_analyzer-0.1.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/test_writers/test_csv_writer.py` & `authz_analyzer-0.1.9/tests/test_writers/test_csv_writer.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/test_writers/test_multijson_writer.py` & `authz_analyzer-0.1.9/tests/test_writers/test_multijson_writer.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/test_exporter.py` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/test_exporter.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py` & `authz_analyzer-0.1.9/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/bigquery/generate_authz_entry.py` & `authz_analyzer-0.1.9/tests/tests_datastores/bigquery/generate_authz_entry.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/bigquery/mocks.py` & `authz_analyzer-0.1.9/tests/tests_datastores/bigquery/mocks.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/bigquery/test_bigquery.py` & `authz_analyzer-0.1.9/tests/tests_datastores/bigquery/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/mongodb/test_atlas_organization_users.py` & `authz_analyzer-0.1.9/tests/tests_datastores/mongodb/test_atlas_organization_users.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/mongodb/test_mongodb.py` & `authz_analyzer-0.1.9/tests/tests_datastores/mongodb/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py` & `authz_analyzer-0.1.9/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/postgres/test_postgress_analyzer.py` & `authz_analyzer-0.1.9/tests/tests_datastores/postgres/test_postgress_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from typing import List, Optional
 from unittest.mock import MagicMock
 
+import pytest
+
 from authz_analyzer import PostgresAuthzAnalyzer
+from authz_analyzer.datastores.postgres.deployment import Deployment
+from authz_analyzer.datastores.postgres.model import RESOURCE_TYPE_MAP
 from authz_analyzer.models.model import (
     Asset,
     AssetType,
     AuthzEntry,
     AuthzPathElement,
     AuthzPathElementType,
     Identity,
     IdentityType,
     PermissionLevel,
 )
-import pytest
 from tests.mocks.mock_writers import MockWriter
 from tests.tests_datastores.postgres.mocks.postgres_mock_connector import PostgresMockCursor, Role, RoleGrant, Table
 
-from authz_analyzer.datastores.postgres.model import RESOURCE_TYPE_MAP
-
-from authz_analyzer.datastores.postgres.deployment import Deployment
-
 ALL_TABLES = [
     Table(
         "db1",
         "schema1",
         "table3",
     )
 ]
```

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/redshift/test_redshift.py` & `authz_analyzer-0.1.9/tests/tests_datastores/redshift/test_redshift.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/tests/tests_datastores/snowflake/test_snowflake_analyzer.py` & `authz_analyzer-0.1.9/tests/tests_datastores/snowflake/test_snowflake_analyzer.py`

 * *Files identical despite different names*

### Comparing `authz_analyzer-0.1.8/PKG-INFO` & `authz_analyzer-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authz-analyzer
-Version: 0.1.8
+Version: 0.1.9
 Summary: Analyze authorization.
 Home-page: https://github.com/satoricyber/authz-analyzer
 Author: SatoriCyber
 Requires-Python: >=3.8.1,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: release
 Provides-Extra: test
 Requires-Dist: black (>=22.12.0,<23.0.0) ; extra == "test"
 Requires-Dist: boto3 (>=1.26.27,<2.0.0)
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "test"
 Requires-Dist: click (==8.1.3)
+Requires-Dist: databricks-cli (>=0.17.4,<0.18.0)
 Requires-Dist: google-api-python-client (>=2.66.0,<2.67.0)
 Requires-Dist: google-api-python-client-stubs (>=1.13.0,<2.0.0) ; extra == "test"
 Requires-Dist: google-cloud-bigquery (>=2.1.0,<3.0)
 Requires-Dist: google-cloud-iam (>=2.10.0,<3.0.0)
 Requires-Dist: google-cloud-resource-manager (>=1.6.3,<2.0)
 Requires-Dist: isort (>=5.11.3,<6.0.0) ; extra == "test"
 Requires-Dist: markdown-it-py (>=2.2.0,<3.0.0)
```

