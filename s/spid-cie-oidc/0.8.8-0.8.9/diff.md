# Comparing `tmp/spid_cie_oidc-0.8.8.tar.gz` & `tmp/spid_cie_oidc-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spid_cie_oidc-0.8.8.tar", last modified: Wed Nov 16 17:53:21 2022, max compression
+gzip compressed data, was "spid_cie_oidc-0.8.9.tar", last modified: Wed Nov 16 18:15:00 2022, max compression
```

## Comparing `spid_cie_oidc-0.8.8.tar` & `spid_cie_oidc-0.8.9.tar`

### file list

```diff
@@ -1,355 +1,355 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.862781 spid_cie_oidc-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10641 2022-11-16 17:53:21.862781 spid_cie_oidc-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9889 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-16 17:53:21.862781 spid_cie_oidc-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.806781 spid_cie_oidc-0.8.8/spid_cie_oidc/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.810781 spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/admin_inlines.py
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.810781 spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     5254 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/migrations/0002_remove_user_taxpayer_id_user_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/migrations/0003_alter_user_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.810781 spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/templatetags/has_group.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.810781 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.814781 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    11942 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0002_alter_federationentityprofile_trust_mark_template.py
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0003_alter_federationdescendantcontact_entity_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0004_federationdescendant_jwks_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0005_alter_federationdescendant_jwks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0006_stafftoken.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0007_stafftoken_expire_at.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0008_alter_stafftoken_token.py
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0009_delete_stafftoken.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9571 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.814781 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/schemas/advanced_entity_list_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/schemas/fetch_endpoint_request.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/schemas/list_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/schemas/trust_mark_status_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.814781 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6202 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/tests/mocked_responses.py
--rw-r--r--   0 runner    (1001) docker     (121)     7023 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    11763 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/tests/test_02_trust_anchor_intermediary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/tests/test_05_validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/tests/test_06_advanced_entity_listing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/tests/test_08_schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     6719 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/authority/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.818781 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/abstract_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     6302 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/http_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2690 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/jwks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3047 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/jwtse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.822781 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     9378 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0002_fetchedentitystatement.py
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0003_federationentityconfiguration_constraints.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0004_alter_federationentityconfiguration_authority_hints_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0005_alter_federationentityconfiguration_constraints.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0006_remove_trustchain_resultant_metadata_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0007_alter_trustchain_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0008_fetchedentitystatement_jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0009_trustchain_trust_marks_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0010_federationentityconfiguration_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0011_alter_trustchain_status.py
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0012_delete_publicjwk.py
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0013_alter_federationentityconfiguration_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0014_alter_trustchain_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0015_alter_trustchain_unique_together_trustchain_type_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0016_alter_trustchain_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0017_remove_federationentityconfiguration_jwks_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0018_trustchain_jwks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0019_stafftoken.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12424 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    12111 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.822781 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/schemas/fa_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/schemas/jwks.py
--rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/schemas/op_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/schemas/resolve_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/schemas/rp_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    15554 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.826781 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/fa_metadata_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/jwks_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     4024 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/op_metadata_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     4539 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/rp_metadata_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2658 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_01_entity_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_01_op_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_02_rp_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_03_jwks.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_04_fa_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3868 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_05_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_06_http_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_07_resolve_entity_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)     2727 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_07_validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_08_statements.py
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_09_trust_chain.py
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_10_schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)    10918 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/trust_chain.py
--rw-r--r--   0 runner    (1001) docker     (121)     6647 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/trust_chain_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     3983 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/entity/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.826781 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.830781 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0002_alter_onboardingregistration_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0003_alter_onboardingregistration_options.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0004_alter_onboardingregistration_public_jwks.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0005_alter_onboardingregistration_status.py
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0006_onboardingregistration_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0007_onboardingregistration_contact.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0008_onboardingregistration_auth_request_url.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.802781 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.830781 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)    12269 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/static/images/SPID-e-CIE-696x383.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/static/images/logo-it.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.834781 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     9399 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_apply_policy.html
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_convert_jwk.html
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_convert_pem.html
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_decode_jwt.html
--rw-r--r--   0 runner    (1001) docker     (121)     3027 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_entities.html
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_jwk.html
--rw-r--r--   0 runner    (1001) docker     (121)     4450 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_landing.html
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_registration.html
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_resolve_statement.html
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_schemas.html
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_validate_ec.html
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_validate_md.html
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_validating_tm.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.834781 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/tests/mocked_responses.py
--rw-r--r--   0 runner    (1001) docker     (121)     4208 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/tests/test_01_onboarding.py
--rw-r--r--   0 runner    (1001) docker     (121)    10228 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/tests/test_02_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/tests/test_11_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/tests/tools_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)    16952 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.834781 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.834781 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.834781 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3287 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/management/commands/fetch_openid_relying_parties.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.838781 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3103 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/migrations/0002_remove_oidcsession_user_claims.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/migrations/0003_remove_oidcsession_sub_issuedtoken_expires_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/migrations/0004_alter_oidcsession_user.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/migrations/0005_oidcsession_sid.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/migrations/0006_oidcsession_acr.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/migrations/0007_alter_issuedtoken_options_alter_oidcsession_options.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3488 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.838781 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7508 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/authn_requests.py
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/authn_response.py
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/introspection_request.py
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/introspection_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/revocation_request.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/revocation_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3658 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/token_requests.py
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/token_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     8278 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.802781 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.838781 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     6337 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/css/provider.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.838781 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)   196297 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/images/logo-cie.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.842781 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/svg/
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/svg/cie-ico-circle-bb.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/svg/logo-cie.svg
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/svg/no_image_available.svg
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/svg/spid-ico-circle-bb.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.842781 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/templates/op_base.html
--rw-r--r--   0 runner    (1001) docker     (121)     4454 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/templates/op_user_consent.html
--rw-r--r--   0 runner    (1001) docker     (121)     5096 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/templates/op_user_history.html
--rw-r--r--   0 runner    (1001) docker     (121)     5978 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/templates/op_user_login.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.842781 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/templatetags/spid_cie_op.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.846781 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/authn_request_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/authn_responses_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/introspection_request_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2493 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/introspection_response_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/revocation_request_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/revocation_response_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     6720 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    15443 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_02_authn_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     6257 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_03_authn_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     4619 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_03_refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     3143 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_04_authn_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3656 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_04_userinfo_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     4327 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_05_introspection_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     5691 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_05_token_request.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_06_processors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3001 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_06_token_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2556 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_07_fetch_relying_parties.py
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_07_introspection_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2888 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_08_introspection_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5232 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_08_token_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     3875 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_09_revocation_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2596 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_09_revocation_request.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_10_no_consent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_10_revocation_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2584 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_11_user_access_history.py
--rw-r--r--   0 runner    (1001) docker     (121)     1904 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_12_init.py
--rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/token_request_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1804 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/token_response_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.850781 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/
--rw-r--r--   0 runner    (1001) docker     (121)    12699 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10943 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/authz_request_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     5107 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/consent_page_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/introspection_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     3143 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/revocation_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     7928 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/token_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/userinfo_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.850781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.850781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.850781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2258 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/management/commands/fetch_openid_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.854781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3568 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/0002_rename_issuer_oidcauthentication_provider_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/0003_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/0004_rename_revoked_oidcauthenticationtoken_logged_out_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/0005_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/0006_alter_oidcauthentication_provider_configuration_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/0007_alter_oidcauthentication_provider_jwks.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/0008_remove_oidcauthentication_provider_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2671 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.854781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/oauth2/
--rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/oauth2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.854781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/oidc/
--rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/processors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.806781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.854781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     7900 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/css/access-button.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.854781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)     5247 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/js/spid-sp-access-button.js
--rw-r--r--   0 runner    (1001) docker     (121)     3335 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/js/spid_button.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.854781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/svg/
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7406 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/svg/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/svg/spid-ico-circle-bb.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.854781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/templates/echo_attributes.html
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/templates/rp_base.html
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/templates/rp_error.html
--rw-r--r--   0 runner    (1001) docker     (121)     5186 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/templates/rp_landing.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.858781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5684 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/mocked_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_01_rp_ops.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_02_rp_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     7872 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_03_rp_begin.py
--rw-r--r--   0 runner    (1001) docker     (121)     9164 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_04_rp_callback.py
--rw-r--r--   0 runner    (1001) docker     (121)     3010 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_05_oidc_rpinitiated_logout.py
--rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_06_fetch_openid_providers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_07_oidc_rp_landing.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_08_callback_echo_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2349 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_09_rp_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.858781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/views/
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7600 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/views/rp_begin.py
--rw-r--r--   0 runner    (1001) docker     (121)    10419 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/views/rp_callback.py
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/views/rp_callback_echo_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/views/rp_initiated_logout.py
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/views/rp_landing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.858781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.862781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/migrations/0002_alter_relyingpartytest_report.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.862781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/snippets/
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/snippets/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3207 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/snippets/crawler.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/snippets/pyppeteer_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.806781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.862781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)    11982 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/static/images/oops.webp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.862781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/templates/
--rw-r--r--   0 runner    (1001) docker     (121)    14291 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/templates/op_user_staff_test.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.862781 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/tests/test_01_user_staff.py
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-11-16 17:53:09.000000 spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 17:53:21.862781 spid_cie_oidc-0.8.8/spid_cie_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10641 2022-11-16 17:53:21.000000 spid_cie_oidc-0.8.8/spid_cie_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16427 2022-11-16 17:53:21.000000 spid_cie_oidc-0.8.8/spid_cie_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 17:53:21.000000 spid_cie_oidc-0.8.8/spid_cie_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 17:53:21.000000 spid_cie_oidc-0.8.8/spid_cie_oidc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-11-16 17:53:21.000000 spid_cie_oidc-0.8.8/spid_cie_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-16 17:53:21.000000 spid_cie_oidc-0.8.8/spid_cie_oidc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.884283 spid_cie_oidc-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    10641 2022-11-16 18:15:00.884283 spid_cie_oidc-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9889 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-16 18:15:00.884283 spid_cie_oidc-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.792282 spid_cie_oidc-0.8.9/spid_cie_oidc/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.792282 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/admin_inlines.py
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.792282 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     5254 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/migrations/0002_remove_user_taxpayer_id_user_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/migrations/0003_alter_user_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.796282 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/templatetags/has_group.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.796282 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.800282 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)    11942 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0002_alter_federationentityprofile_trust_mark_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0003_alter_federationdescendantcontact_entity_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0004_federationdescendant_jwks_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0005_alter_federationdescendant_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0006_stafftoken.py
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0007_stafftoken_expire_at.py
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0008_alter_stafftoken_token.py
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0009_delete_stafftoken.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9571 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.804282 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/advanced_entity_list_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/fetch_endpoint_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/list_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)      815 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/trust_mark_status_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2370 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.804282 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6202 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/mocked_responses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7023 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11765 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_02_trust_anchor_intermediary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_05_validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_06_advanced_entity_listing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_08_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6730 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.808282 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      718 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/abstract_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6302 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2690 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/jwks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3047 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/jwtse.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.816282 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     9378 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0002_fetchedentitystatement.py
+-rw-r--r--   0 runner    (1001) docker     (121)      672 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0003_federationentityconfiguration_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0004_alter_federationentityconfiguration_authority_hints_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0005_alter_federationentityconfiguration_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0006_remove_trustchain_resultant_metadata_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0007_alter_trustchain_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0008_fetchedentitystatement_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (121)      846 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0009_trustchain_trust_marks_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0010_federationentityconfiguration_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0011_alter_trustchain_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0012_delete_publicjwk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      748 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0013_alter_federationentityconfiguration_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      506 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0014_alter_trustchain_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      956 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0015_alter_trustchain_unique_together_trustchain_type_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      519 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0016_alter_trustchain_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0017_remove_federationentityconfiguration_jwks_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0018_trustchain_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0019_stafftoken.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12424 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12111 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.816282 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/fa_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/jwks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/op_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/resolve_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/rp_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15554 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.824282 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/fa_metadata_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/jwks_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4024 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/op_metadata_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4539 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/rp_metadata_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2658 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_01_entity_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_01_op_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_02_rp_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      718 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_03_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_04_fa_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3868 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_05_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_06_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_07_resolve_entity_statement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2727 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_07_validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_08_statements.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_09_trust_chain.py
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_10_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10918 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/trust_chain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6647 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/trust_chain_operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3983 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.824282 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.828282 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0002_alter_onboardingregistration_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0003_alter_onboardingregistration_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0004_alter_onboardingregistration_public_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0005_alter_onboardingregistration_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0006_onboardingregistration_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      573 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0007_onboardingregistration_contact.py
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0008_onboardingregistration_auth_request_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.784282 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.828282 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/static/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    12269 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/static/images/SPID-e-CIE-696x383.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/static/images/logo-it.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.832282 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     9399 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_apply_policy.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_convert_jwk.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_convert_pem.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_decode_jwt.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3027 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_entities.html
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_jwk.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4450 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_landing.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_registration.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_resolve_statement.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_schemas.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_validate_ec.html
+-rw-r--r--   0 runner    (1001) docker     (121)      939 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_validate_md.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_validating_tm.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.836282 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/mocked_responses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4208 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/test_01_onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10247 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/test_02_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/test_11_admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/tools_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16955 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.840282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.840282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/management/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.840282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3287 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/management/commands/fetch_openid_relying_parties.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.840282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     3103 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0002_remove_oidcsession_user_claims.py
+-rw-r--r--   0 runner    (1001) docker     (121)      771 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0003_remove_oidcsession_sub_issuedtoken_expires_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0004_alter_oidcsession_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0005_oidcsession_sid.py
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0006_oidcsession_acr.py
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0007_alter_issuedtoken_options_alter_oidcsession_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3488 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.844282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7508 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/authn_requests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/authn_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/introspection_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)      827 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/introspection_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/revocation_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/revocation_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3658 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/token_requests.py
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8278 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.784282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.844282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)     6337 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/css/provider.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.844282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/images/
+-rw-r--r--   0 runner    (1001) docker     (121)   196297 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/images/logo-cie.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.848282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/
+-rw-r--r--   0 runner    (1001) docker     (121)      706 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/cie-ico-circle-bb.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/logo-cie.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/no_image_available.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/spid-ico-circle-bb.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.848282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_base.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4454 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_user_consent.html
+-rw-r--r--   0 runner    (1001) docker     (121)     5096 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_user_history.html
+-rw-r--r--   0 runner    (1001) docker     (121)     5978 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_user_login.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.848282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templatetags/spid_cie_op.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.856282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/authn_request_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/authn_responses_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/introspection_request_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2493 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/introspection_response_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/revocation_request_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/revocation_response_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6720 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15443 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_02_authn_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6257 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_03_authn_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4619 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_03_refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3143 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_04_authn_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3656 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_04_userinfo_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4327 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_05_introspection_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5691 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_05_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_06_processors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3001 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_06_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2556 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_07_fetch_relying_parties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_07_introspection_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2888 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_08_introspection_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5232 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_08_token_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3875 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_09_revocation_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2596 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_09_revocation_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_10_no_consent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_10_revocation_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2584 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_11_user_access_history.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1904 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_12_init.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/token_request_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1804 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/token_response_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.860283 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/
+-rw-r--r--   0 runner    (1001) docker     (121)    12699 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10943 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/authz_request_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5107 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/consent_page_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/introspection_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3143 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/revocation_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7928 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/token_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/userinfo_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.860283 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.860283 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/management/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.864282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2258 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/management/commands/fetch_openid_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.868282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     3568 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0002_rename_issuer_oidcauthentication_provider_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0003_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      572 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0004_rename_revoked_oidcauthenticationtoken_logged_out_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      825 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0005_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      706 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0006_alter_oidcauthentication_provider_configuration_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)      485 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0007_alter_oidcauthentication_provider_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0008_remove_oidcauthentication_provider_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2671 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.868282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/oauth2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.868282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/oidc/
+-rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/processors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.788282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.868282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)     7900 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/css/access-button.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.868282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/js/
+-rw-r--r--   0 runner    (1001) docker     (121)     5247 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/js/spid-sp-access-button.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3335 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/js/spid_button.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.868282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/svg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     7406 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/svg/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/svg/spid-ico-circle-bb.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.868282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/echo_attributes.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/rp_base.html
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/rp_error.html
+-rw-r--r--   0 runner    (1001) docker     (121)     5186 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/rp_landing.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.872283 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5684 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/mocked_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_01_rp_ops.py
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_02_rp_commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7872 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_03_rp_begin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9164 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_04_rp_callback.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3010 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_05_oidc_rpinitiated_logout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_06_fetch_openid_providers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_07_oidc_rp_landing.py
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_08_callback_echo_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2349 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_09_rp_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.876283 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/
+-rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7600 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_begin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10419 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_callback.py
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_callback_echo_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_initiated_logout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_landing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.876283 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      821 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      862 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.876283 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/migrations/0002_alter_relyingpartytest_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.880282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/snippets/
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/snippets/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3207 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/snippets/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      991 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/snippets/pyppeteer_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.788282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.880282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/static/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    11982 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/static/images/oops.webp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.880282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)    14291 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/templates/op_user_staff_test.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.880282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/tests/test_01_user_staff.py
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.884283 spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10641 2022-11-16 18:15:00.000000 spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    16427 2022-11-16 18:15:00.000000 spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 18:15:00.000000 spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 18:15:00.000000 spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-11-16 18:15:00.000000 spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-16 18:15:00.000000 spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/top_level.txt
```

### Comparing `spid_cie_oidc-0.8.8/LICENSE` & `spid_cie_oidc-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/PKG-INFO` & `spid_cie_oidc-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spid_cie_oidc
-Version: 0.8.8
+Version: 0.8.9
 Summary: SPID/CIE OIDC Federation Entity
 Home-page: https://github.com/peppelinux/spid-cie-oidc
 Author: Giuseppe De Marco
 Author-email: demarcog83@gmail.com
 License: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `spid_cie_oidc-0.8.8/README.md` & `spid_cie_oidc-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/setup.py` & `spid_cie_oidc-0.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/admin.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/migrations/0001_initial.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/migrations/0002_remove_user_taxpayer_id_user_attributes.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/migrations/0002_remove_user_taxpayer_id_user_attributes.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/accounts/models.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/admin.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0001_initial.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0003_alter_federationdescendantcontact_entity_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0003_alter_federationdescendantcontact_entity_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0004_federationdescendant_jwks_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0004_federationdescendant_jwks_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0005_alter_federationdescendant_jwks.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0005_alter_federationdescendant_jwks.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0006_stafftoken.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0006_stafftoken.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/migrations/0008_alter_stafftoken_token.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0008_alter_stafftoken_token.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/models.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/schemas/advanced_entity_list_endpoint.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/advanced_entity_list_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/schemas/fetch_endpoint_request.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/fetch_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/schemas/trust_mark_status_endpoint.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/trust_mark_status_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/tests/mocked_responses.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/mocked_responses.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/tests/settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/tests/test_02_trust_anchor_intermediary.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_02_trust_anchor_intermediary.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,25 +250,25 @@
         self.assertTrue(res.status_code == 200)
         verify_jws(res.content.decode(), self.ta_conf.jwks_fed[0])
 
     def test_trust_mark_status_endpoint(self):
         url = reverse("oidcfed_trust_mark_status")
 
         c = Client()
-        res = c.get(
+        res = c.post(
             url,
             data={
                 "id": self.rp_assigned_profile.profile.profile_id,
                 "sub": self.rp_assigned_profile.descendant.sub,
             },
         )
         self.assertTrue(res.status_code == 200)
         self.assertTrue(res.json() == {"active": True})
 
-        res = c.get(
+        res = c.post(
             url,
             data={
                 "trust_mark": self.rp_assigned_profile.trust_mark["trust_mark"],
             },
         )
         self.assertTrue(res.status_code == 200)
         self.assertTrue(res.json() == {"active": True})
```

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/tests/test_05_validators.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_05_validators.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/tests/test_06_advanced_entity_listing.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_06_advanced_entity_listing.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/tests/test_08_schemas.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_08_schemas.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/urls.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/urls.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/validators.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/validators.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/authority/views.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,22 +183,22 @@
             "404": FedAPIErrorResponse,
             "200": TrustMarkResponse
     },
     tags = ['Federation API']
 )
 def trust_mark_status(request):
     failed_data = {"active": False}
-    if request.GET.get("sub", "") and request.GET.get("id", ""):
-        sub = request.GET["sub"]
-        _id = request.GET["id"]
-
-    elif request.GET.get("trust_mark", ""):
+    if request.POST.get("sub", "") and request.POST.get("id", ""):
+        sub = request.POST["sub"]
+        _id = request.POST["id"]
+    
+    elif request.POST.get("trust_mark", ""):
         try:
-            unpad_jwt_head(request.GET["trust_mark"])
-            payload = unpad_jwt_payload(request.GET["trust_mark"])
+            unpad_jwt_head(request.POST["trust_mark"])
+            payload = unpad_jwt_payload(request.POST["trust_mark"])
             sub = payload.get("sub", "")
             _id = payload.get("id", "")
         except Exception:
             return JsonResponse(failed_data)
     else:
         return JsonResponse(failed_data)
```

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/abstract_models.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/abstract_models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/admin.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/exceptions.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/exceptions.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/http_client.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/http_client.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/jwks.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/jwks.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/jwtse.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/jwtse.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0001_initial.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0002_fetchedentitystatement.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0002_fetchedentitystatement.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0003_federationentityconfiguration_constraints.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0003_federationentityconfiguration_constraints.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0004_alter_federationentityconfiguration_authority_hints_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0004_alter_federationentityconfiguration_authority_hints_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0005_alter_federationentityconfiguration_constraints.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0005_alter_federationentityconfiguration_constraints.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0006_remove_trustchain_resultant_metadata_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0006_remove_trustchain_resultant_metadata_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0007_alter_trustchain_unique_together_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0007_alter_trustchain_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0009_trustchain_trust_marks_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0009_trustchain_trust_marks_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0010_federationentityconfiguration_entity_type.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0010_federationentityconfiguration_entity_type.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0011_alter_trustchain_status.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0011_alter_trustchain_status.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0013_alter_federationentityconfiguration_metadata.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0013_alter_federationentityconfiguration_metadata.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0015_alter_trustchain_unique_together_trustchain_type_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0015_alter_trustchain_unique_together_trustchain_type_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0016_alter_trustchain_unique_together_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0016_alter_trustchain_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0017_remove_federationentityconfiguration_jwks_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0017_remove_federationentityconfiguration_jwks_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/migrations/0019_stafftoken.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0019_stafftoken.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/models.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/policy.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/policy.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/schemas/jwks.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/jwks.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/schemas/op_metadata.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/op_metadata.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/schemas/resolve_endpoint.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/resolve_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/schemas/rp_metadata.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/rp_metadata.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/statements.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/statements.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/jwks_settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/jwks_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/op_metadata_settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/op_metadata_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/rp_metadata_settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/rp_metadata_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_01_entity_configuration.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_01_entity_configuration.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_01_op_metadata.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_01_op_metadata.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_02_rp_metadata.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_02_rp_metadata.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_03_jwks.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_03_jwks.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_05_policy.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_05_policy.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_07_resolve_entity_statement.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_07_resolve_entity_statement.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_07_validators.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_07_validators.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_08_statements.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_08_statements.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/tests/test_09_trust_chain.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_09_trust_chain.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/trust_chain.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/trust_chain.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/trust_chain_operations.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/trust_chain_operations.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/urls.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/urls.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/utils.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/utils.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/validators.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/validators.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/entity/views.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/views.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/admin.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/forms.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/forms.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0001_initial.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0002_alter_onboardingregistration_options_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0002_alter_onboardingregistration_options_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0003_alter_onboardingregistration_options.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0003_alter_onboardingregistration_options.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0004_alter_onboardingregistration_public_jwks.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0004_alter_onboardingregistration_public_jwks.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0005_alter_onboardingregistration_status.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0005_alter_onboardingregistration_status.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0006_onboardingregistration_type.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0006_onboardingregistration_type.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0007_onboardingregistration_contact.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0007_onboardingregistration_contact.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/migrations/0008_onboardingregistration_auth_request_url.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0008_onboardingregistration_auth_request_url.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/models.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/static/images/SPID-e-CIE-696x383.jpg` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/static/images/SPID-e-CIE-696x383.jpg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/static/images/logo-it.svg` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/static/images/logo-it.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/base.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/base.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_apply_policy.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_apply_policy.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_convert_jwk.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_convert_jwk.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_convert_pem.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_convert_pem.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_decode_jwt.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_decode_jwt.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_entities.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_entities.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_jwk.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_jwk.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_landing.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_landing.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_registration.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_registration.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_resolve_statement.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_resolve_statement.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_schemas.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_schemas.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_validate_ec.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_validate_ec.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_validate_md.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_validate_md.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/templates/onboarding_validating_tm.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_validating_tm.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/tests/test_01_onboarding.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/test_01_onboarding.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/tests/test_02_tools.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/test_02_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,35 +202,35 @@
         res = self.client.post(url + '?metadata_type=rp_metadata&provider_profile=cie', 
             {'md': "hello world"})
         self.assertEqual(res.status_code, 200)
         self.assertIn("alert-error", res.content.decode())
     
     def test_validating_trust_mark(self):
         url = reverse("oidc_onboarding_validating_trustmark")
-        res = self.client.get(url)
+        res = self.client.post(url)
         self.assertEqual(res.status_code, 200)
 
-        res = self.client.get(url, {
+        res = self.client.post(url, data={
             "id": "https://www.ciao.gov.it/certification/rp",
             "sub": "http://ciao.it/oidc/rp/",
         })
         self.assertEqual(res.status_code, 200)
         self.assertIn("alert-error", res.content.decode())
 
-        res = self.client.get(url, {
+        res = self.client.post(url, data={
             "id": "https://www.spid.gov.it/certification/rp",
             "sub": "http://rp-test.it/oidc/rp/",
         })
 
         self.assertEqual(res.status_code, 200)
         self.assertIn("alert-success", res.content.decode())
 
         trust_mark = self.rp_assigned_profile.trust_mark_as_jws
         
-        res = self.client.get(url, {
+        res = self.client.post(url, data={
             "trust_mark": trust_mark,
         })
         self.assertEqual(res.status_code, 200)
         self.assertIn("alert-success", res.content.decode())
 
     def test_validate_authn_request(self):
         url = reverse("oidc_onboarding_validate_authn_request_jwt")
```

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/tests/test_11_admin.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/test_11_admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/tests/tools_settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/tools_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/urls.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/urls.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/onboarding/views.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,16 +164,16 @@
             context["resolved_statement"] = json.dumps(resultJson, indent=4)
         except Exception:
             messages.error(request, _('Failed to resolve entity statement, Please check your inserted data'))
     return render(request, 'onboarding_resolve_statement.html', context)
 
 
 def onboarding_validating_trustmark(request):
-    if "id" in request.GET or "trust_mark" in request.GET:
-        form = OnboardingValidatingTrustMarkForm(request.GET)
+    if "id" in request.POST or "trust_mark" in request.POST:
+        form = OnboardingValidatingTrustMarkForm(request.POST)
     else:
         form = OnboardingValidatingTrustMarkForm()
 
     context = {"form": form}
 
     if form.is_valid():
         res = trust_mark_status(request)
```

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/admin.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/forms.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/forms.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/management/commands/fetch_openid_relying_parties.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/management/commands/fetch_openid_relying_parties.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/migrations/0001_initial.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/migrations/0003_remove_oidcsession_sub_issuedtoken_expires_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0003_remove_oidcsession_sub_issuedtoken_expires_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/migrations/0004_alter_oidcsession_user.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0004_alter_oidcsession_user.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/migrations/0007_alter_issuedtoken_options_alter_oidcsession_options.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0007_alter_issuedtoken_options_alter_oidcsession_options.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/models.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/authn_requests.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/authn_requests.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/authn_response.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/authn_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/introspection_response.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/introspection_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/jwt.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/jwt.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/token_requests.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/token_requests.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/schemas/token_response.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/token_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/css/provider.css` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/css/provider.css`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/images/logo-cie.png` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/images/logo-cie.png`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/svg/cie-ico-circle-bb.svg` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/cie-ico-circle-bb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/svg/logo-cie.svg` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/logo-cie.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/svg/spid-ico-circle-bb.svg` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/spid-ico-circle-bb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/templates/op_base.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_base.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/templates/op_user_consent.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_user_consent.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/templates/op_user_history.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_user_history.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/templates/op_user_login.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_user_login.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/templatetags/spid_cie_op.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templatetags/spid_cie_op.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/authn_request_settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/authn_request_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/authn_responses_settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/authn_responses_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/introspection_request_settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/introspection_request_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/introspection_response_settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/introspection_response_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/revocation_request_settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/revocation_request_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/revocation_response_settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/revocation_response_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_02_authn_endpoint.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_02_authn_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_03_authn_request.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_03_authn_request.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_03_refresh_token.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_03_refresh_token.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_04_authn_response.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_04_authn_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_04_userinfo_endpoint.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_04_userinfo_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_05_introspection_endpoint.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_05_introspection_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_05_token_request.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_05_token_request.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_06_token_response.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_06_token_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_07_fetch_relying_parties.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_07_fetch_relying_parties.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_07_introspection_request.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_07_introspection_request.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_08_introspection_response.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_08_introspection_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_08_token_endpoint.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_08_token_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_09_revocation_endpoint.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_09_revocation_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_09_revocation_request.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_09_revocation_request.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_10_no_consent.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_10_no_consent.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_10_revocation_response.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_10_revocation_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_11_user_access_history.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_11_user_access_history.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/test_12_init.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_12_init.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/token_request_settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/token_request_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/tests/token_response_settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/token_response_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/urls.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/urls.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/__init__.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/__init__.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/authz_request_view.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/authz_request_view.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/consent_page_view.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/consent_page_view.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/introspection_endpoint.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/introspection_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/revocation_endpoint.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/revocation_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/token_endpoint.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/token_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/provider/views/userinfo_endpoint.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/userinfo_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/admin.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/management/commands/fetch_openid_providers.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/management/commands/fetch_openid_providers.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/0001_initial.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/0002_rename_issuer_oidcauthentication_provider_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0002_rename_issuer_oidcauthentication_provider_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/0003_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0003_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/0004_rename_revoked_oidcauthenticationtoken_logged_out_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0004_rename_revoked_oidcauthenticationtoken_logged_out_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/0005_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0005_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/migrations/0006_alter_oidcauthentication_provider_configuration_and_more.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0006_alter_oidcauthentication_provider_configuration_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/models.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/oauth2/__init__.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/oauth2/__init__.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/oidc/__init__.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/settings.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/css/access-button.css` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/css/access-button.css`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/js/spid-sp-access-button.js` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/js/spid-sp-access-button.js`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/js/spid_button.js` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/js/spid_button.js`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb.svg` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/svg/favicon.ico` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/svg/favicon.ico`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/static/svg/spid-ico-circle-bb.svg` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/svg/spid-ico-circle-bb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/templates/echo_attributes.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/echo_attributes.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/templates/rp_base.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/rp_base.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/templates/rp_error.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/rp_error.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/templates/rp_landing.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/rp_landing.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/mocked_response.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/mocked_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_01_rp_ops.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_01_rp_ops.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_03_rp_begin.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_03_rp_begin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_04_rp_callback.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_04_rp_callback.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_05_oidc_rpinitiated_logout.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_05_oidc_rpinitiated_logout.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_06_fetch_openid_providers.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_06_fetch_openid_providers.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_07_oidc_rp_landing.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_07_oidc_rp_landing.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_08_callback_echo_attributes.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_08_callback_echo_attributes.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/tests/test_09_rp_model.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_09_rp_model.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/urls.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/urls.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/utils.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/utils.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/views/__init__.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/__init__.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/views/rp_begin.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_begin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/views/rp_callback.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_callback.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/views/rp_initiated_logout.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_initiated_logout.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party/views/rp_landing.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_landing.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/admin.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/forms.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/forms.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/migrations/0001_initial.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/migrations/0002_alter_relyingpartytest_report.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/migrations/0002_alter_relyingpartytest_report.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/models.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/snippets/README.md` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/snippets/README.md`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/snippets/crawler.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/snippets/crawler.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/snippets/pyppeteer_tests.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/snippets/pyppeteer_tests.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/static/images/oops.webp` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/static/images/oops.webp`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/templates/op_user_staff_test.html` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/templates/op_user_staff_test.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/tests/test_01_user_staff.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/tests/test_01_user_staff.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc/relying_party_test/views.py` & `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/views.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc.egg-info/PKG-INFO` & `spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spid-cie-oidc
-Version: 0.8.8
+Version: 0.8.9
 Summary: SPID/CIE OIDC Federation Entity
 Home-page: https://github.com/peppelinux/spid-cie-oidc
 Author: Giuseppe De Marco
 Author-email: demarcog83@gmail.com
 License: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `spid_cie_oidc-0.8.8/spid_cie_oidc.egg-info/SOURCES.txt` & `spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

