# Comparing `tmp/syft-0.8.0b8.tar.gz` & `tmp/syft-0.8.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.0b8.tar", last modified: Sun Apr 16 13:01:58 2023, max compression
+gzip compressed data, was "syft-0.8.0b9.tar", last modified: Sun Apr 23 13:01:36 2023, max compression
```

## Comparing `syft-0.8.0b8.tar` & `syft-0.8.0b9.tar`

### file list

```diff
@@ -1,140 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.464810 syft-0.8.0b8/
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-16 12:59:41.000000 syft-0.8.0b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-16 12:59:41.000000 syft-0.8.0b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-04-16 13:01:58.464810 syft-0.8.0b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-04-16 12:59:41.000000 syft-0.8.0b8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-16 12:59:41.000000 syft-0.8.0b8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-16 13:01:58.464810 syft-0.8.0b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-16 12:59:41.000000 syft-0.8.0b8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.448809 syft-0.8.0b8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.452809 syft-0.8.0b8/src/syft/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-16 12:59:55.000000 syft-0.8.0b8/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-04-16 12:59:55.000000 syft-0.8.0b8/src/syft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.452809 syft-0.8.0b8/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.452809 syft-0.8.0b8/src/syft/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.452809 syft-0.8.0b8/src/syft/core/node/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.464810 syft-0.8.0b8/src/syft/core/node/new/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    26657 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/action_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/action_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/action_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/action_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/capnp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/data_subject_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/dataset_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    22314 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    21597 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/message_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/message_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/metadata_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/network_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/node_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    21086 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/project_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/project_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    12210 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/sqlite_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/third_party.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/unparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_policy_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/worker_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    26120 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/experimental_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.464810 syft-0.8.0b8/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.464810 syft-0.8.0b8/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/gevent_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/user_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.452809 syft-0.8.0b8/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-04-16 13:01:58.000000 syft-0.8.0b8/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-04-16 13:01:58.000000 syft-0.8.0b8/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:01:58.000000 syft-0.8.0b8/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:01:58.000000 syft-0.8.0b8/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-16 13:01:58.000000 syft-0.8.0b8/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-16 13:01:58.000000 syft-0.8.0b8/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.672410 syft-0.8.0b9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-23 12:59:19.000000 syft-0.8.0b9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 12:59:19.000000 syft-0.8.0b9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-04-23 13:01:36.672410 syft-0.8.0b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14766 2023-04-23 12:59:18.000000 syft-0.8.0b9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-23 12:59:19.000000 syft-0.8.0b9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-23 13:01:36.676410 syft-0.8.0b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-23 12:59:19.000000 syft-0.8.0b9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.652410 syft-0.8.0b9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.656410 syft-0.8.0b9/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-23 12:59:33.000000 syft-0.8.0b9/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-23 12:59:33.000000 syft-0.8.0b9/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.660410 syft-0.8.0b9/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.660410 syft-0.8.0b9/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19073 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21112 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.660410 syft-0.8.0b9/src/syft/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.660410 syft-0.8.0b9/src/syft/external/oblv/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.660410 syft-0.8.0b9/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26881 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.664410 syft-0.8.0b9/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/third_party.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.664410 syft-0.8.0b9/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.664410 syft-0.8.0b9/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26733 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.664410 syft-0.8.0b9/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21157 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.664410 syft-0.8.0b9/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/message/message_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/message/message_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/message/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/metadata/metadata_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/network/network_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21237 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/queue/queue_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.672410 syft-0.8.0b9/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.672410 syft-0.8.0b9/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.672410 syft-0.8.0b9/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.656410 syft-0.8.0b9/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-04-23 13:01:36.000000 syft-0.8.0b9/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-23 13:01:36.000000 syft-0.8.0b9/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 13:01:36.000000 syft-0.8.0b9/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-23 13:01:36.000000 syft-0.8.0b9/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 13:01:36.000000 syft-0.8.0b9/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-23 13:01:36.000000 syft-0.8.0b9/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 13:01:36.000000 syft-0.8.0b9/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.0b8/LICENSE` & `syft-0.8.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/PKG-INFO` & `syft-0.8.0b9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.0b8
+Version: 0.8.0b9
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -17,74 +17,116 @@
 Provides-Extra: test_plugins
 Provides-Extra: oblv
 License-File: LICENSE
 
 <div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://pepy.tech/badge/syft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev" /></a> <a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
 <br /><br /></div>
 
-<img src="docs/img/title_syft_light.png#gh-light-mode-only" alt="Syft Logo" width="200px" />
-<img src="docs/img/title_syft_dark.png#gh-dark-mode-only" alt="Syft Logo" width="200px" />
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/title_syft_dark.png">
+  <img alt="Syft Logo" src="docs/img/title_syft_light.png" width="200px" />
+</picture>
 
 Perform `numpy`-like analysis on `data` that remains in `someone else's` server
 
 <div align="left">
-<img src="docs/img/header.png#gh-light-mode-only" alt="Syft Overview" width="100%" />
-<img src="docs/img/header.png#gh-dark-mode-only" alt="Syft Overview" width="100%" />
+<img alt="Syft Logo" src="docs/img/header.png" alt="Syft Overview" width="100%" />
 </div>
 
 # Quickstart
 
 ✅ `Linux` ✅ `macOS`\* ✅ `Windows`†‡
-<img src="docs/img/terminalizer.gif" width="50%" align="right" />
 
-1. Install our handy 🛵 cli tool which makes deploying a Domain or Network server a one-liner:  
+## Install syft on Python 3.8 - 3.10
+
+```bash
+$ pip install --pre syft -f https://whls.blob.core.windows.net/unstable/index.html
+```
+
+## Launch a python dev Domain
+
+```python
+# from Jupyter / Python
+import syft as sy
+sy.requires(">=0.8-beta")
+node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
+```
+
+```bash
+# or from the command line
+$ syft launch --name=my-domain --port=8080 --reset=True
+
+Starting syft-node server on 0.0.0.0:8080
+```
+
+## Connect with our Python Client
+
+```python
+import syft as sy
+sy.requires(">=0.8-beta")
+domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
+```
+
+## Deploy to a Container Engine or Cloud
+
+1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server a one-liner:  
    `pip install -U hagrid`
 
 2. Then run our interactive jupyter Install 🧙🏽‍♂️ Wizard<sup>BETA</sup>:  
    `hagrid quickstart`
 
-- In the tutorial you will learn how to install and deploy:  
-  `PySyft` = our `numpy`-like 🐍 Python library for computing on `private data` in someone else's `Domain`
+3. In the tutorial you will learn how to install and deploy:  
+   `PySyft` = our `numpy`-like 🐍 Python library for computing on `private data` in someone else's `Domain`
 
-  `PyGrid` = our 🐳 `docker` / `k8s` / 🐧 `vm` `Domain` & `Network` Servers where `private data` lives
+   `PyGrid` = our 🐳 `docker` / 🐧 `vm` `Domain` & `Gateway` Servers where `private data` lives
 
-- During quickstart we will deploy `PyGrid` to localhost with 🐳 `docker`, however 🛵 HAGrid can deploy to `k8s` or a 🐧 `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using 🔨 `ansible`†
+4. During quickstart we will deploy `PyGrid` to localhost with 🐳 `docker`, however 🛵 HAGrid can deploy to `podman` or a 🐧 `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using 🔨 `ansible`†
 
-3. Read our 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
-4. Ask Questions ❔ in `#support` on <a href="https://slack.openmined.org/">Slack</a>
+## Docs and Support
+
+- 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
+- `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
-- HAGrid Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
+- HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`  
   †`Windows` does not support `ansible`, preventing some remote deployment targets
-- PySyft Requires: 🐍 `python 3.8+` - Run: `pip install -U syft`  
-  \*`macOS` Apple Silicon users need cmake: `brew install cmake`  
+- PySyft 0.8 Requires: 🐍 `python 3.8 - 3.10` - Run: `pip install -U syft`  
+  \*`macOS` Apple Silicon users might need cmake: `brew install cmake`  
   ‡`Windows` users must run this first: `pip install jaxlib==0.3.14 -f https://whls.blob.core.windows.net/unstable/index.html`
-- PyGrid Requires: 🐳 `docker` / `k8s` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
+- PyGrid Requires: 🐳 `docker` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
 
 # Versions
 
-`0.8.0 beta` - `dev` branch 👈🏽  
-`0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>  
-`0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>  
-`0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix  
-`0.2.0` - `0.5.0` Deprecated
+`0.8.0` (Beta) - `dev` branch 👈🏽  
+`0.7.0` (Stable) - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
+
+Deprecated:
+
+- `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
+- `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
+- `0.2.0` - `0.5.0`
 
 PySyft and PyGrid use the same `version` and its best to match them up where possible. We release weekly betas which can be used in each context:
-PySyft: `pip install -U syft --pre`
-PyGrid: `hagrid launch ... tag=latest`
+
+PySyft (Stable): `pip install -U syft`  
+PyGrid (Stable) `hagrid launch ... tag=latest`
+
+PySyft (Beta): `pip install -U syft --pre`  
+PyGrid (Beta): `hagrid launch ... tag=beta`
 
 HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually the best.
 
 # What is Syft?
 
-<img align="right" src="docs/img/logo_big.png#gh-light-mode-only" alt="Syft" height="250" style="padding-left:30px;">
-
-<img align="right" src="docs/img/logo_big_dark.png#gh-dark-mode-only" alt="Syft" height="250" style="padding-left:30px;">
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_big_dark.png">
+  <img align="right" src="docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
+</picture>
 
 `Syft` is OpenMined's `open source` stack that provides `secure` and `private` Data Science in Python. Syft decouples `private data` from model training, using techniques like [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and integration with `Deep Learning` frameworks, so that you as a `Data Scientist` can maintain your current workflow while using these new `privacy-enhancing techniques`.
 
 ### Why should I use Syft?
 
 `Syft` allows a `Data Scientist` to ask `questions` about a `dataset` and, within `privacy limits` set by the `data owner`, get `answers` to those `questions`, all without obtaining a `copy` of the data itself. We call this process `Remote Data Science`. It means in a wide variety of `domains` across society, the current `risks` of sharing information (`copying` data) with someone such as, privacy invasion, IP theft and blackmail will no longer prevent the vast `benefits` such as innovation, insights and scientific discovery which secure access will provide.
 
@@ -177,52 +219,59 @@
 <tr>
 <th align="center">
 <img width="441" height="1">
 <p>🏰 Domain Server</p>
 </th>
 <th align="center">
 <img width="441" height="1">
-<p>🔗 Network Server</p>
+<p>🔗 Gateway Server</p>
 </th>
 </tr>
 <tr>
 <td valign="top">
 <!-- REMOVE THE BACKSLASHES -->
 
 Manages the `remote study` of the data by a `Data Scientist` and allows the `Data Owner` to manage the `data` and control the `privacy guarantees` of the subjects under study. It also acts as a `gatekeeper` for the `Data Scientist's` access to the data to compute and experiment with the results.
 
 </td>
 <td valign="top">
 <!-- REMOVE THE BACKSLASHES -->
 
-Provides services to a group of `Data Owners` and `Data Scientists`, such as dataset `search` and bulk `project approval` (legal / technical) to participate in a project. A network server acts as a bridge between it's members (`Domains`) and their subscribers (`Data Scientists`) and can provide access to a collection of `domains` at once.</td>
+Provides services to a group of `Data Owners` and `Data Scientists`, such as dataset `search` and bulk `project approval` (legal / technical) to participate in a project. A gateway server acts as a bridge between it's members (`Domains`) and their subscribers (`Data Scientists`) and can provide access to a collection of `domains` at once.</td>
 
 </tr>
 <tr>
 </table>
 
 # Community
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
-<img src="docs/img/panel_slack_title_light.png#gh-light-mode-only" alt="" width="100%" align="center" />
-<img src="docs/img/panel_slack_title_dark.png#gh-dark-mode-only" alt="" width="100%" align="center" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/panel_slack_title_dark.png">
+  <img src="docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
+</picture>
 
 <a href="https://slack.openmined.org/"><img src="docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
 
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
-<img src="docs/img/panel_title_videos_papers_light.png#gh-light-mode-only" alt="" width="100%" align="center" />
-<img src="docs/img/panel_title_videos_papers.png#gh-dark-mode-only" alt="" width="100%" align="center" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/panel_title_videos_papers.png">
+  <img src="docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
+</picture>
+
 <p align="left"><sub><sup>
 🎥 <a href="https://www.youtube.com/watch?v=qVf0tPBzr2k">PETs: Remote Data Science Unleashed - R gov 2021</a><br />
 🎥 <a href="https://youtu.be/sCoDWKTbh3s?list=PL_lsbAsL_o2BQKXG7mkGFA8LSApCnhljL">Introduction to Remote Data Science - PyTorch 2021</a><br />
 🎥 <a href="https://youtu.be/kzLeTz_vIeQ?list=PL_lsbAsL_o2BtOz6KUfUI_Zla6Rg5dmyc">The Future of AI Tools - PyTorch 2020</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=4zrU54VIK6k&t=1s">Privacy Preserving AI - MIT Deep Learning Series</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=Pr4erdusiW0">Privacy-Preserving Data Science - TWiML Talk #241</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=NJBBE_SN90A">Privacy Preserving AI - PyTorch Devcon 2019</a><br />
@@ -231,16 +280,19 @@
 📖 <a href="https://arxiv.org/pdf/1811.04017.pdf">A generic framework for privacy preserving deep ...</a>
 </sup></sup></p>
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
-<img src="docs/img/panel_padawan_title_light.png#gh-light-mode-only" alt="" width="100%" align="center" />
-<img src="docs/img/panel_padawan_title_dark.png#gh-dark-mode-only" alt="" width="100%" align="center" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/panel_padawan_title_dark.png">
+  <img src="docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
+</picture>
 
 <a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
 
 </div>
 </th>
 </tr>
 </table>
@@ -267,17 +319,20 @@
 </div>
 </th>
 </tr>
 </table>
 
 # Contributors
 
-OpenMined and Syft appreciates all contributors, if you would like to fix a bug or suggest a new feature, please see our [guidelines](https://openmined.github.io/PySyft/developer_guide/index.html).<br />  
-<img src="docs/img/contributors_light.jpg#gh-light-mode-only" alt="Contributors" width="100%" />
-<img src="docs/img/contributors_dark.jpg#gh-dark-mode-only" alt="Contributors" width="100%" />
+OpenMined and Syft appreciates all contributors, if you would like to fix a bug or suggest a new feature, please see our [guidelines](https://openmined.github.io/PySyft/developer_guide/index.html).<br />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/contributors_dark.jpg">
+  <img src="docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
+</picture>
 
 # Supporters
 
 <table border="0">
 <tr>
 <th align="center">
 <a href="https://sloan.org/"><img src="docs/img/logo_sloan.png" /></a>
@@ -294,32 +349,41 @@
 <th align="center">
 <a href="https://summerofcode.withgoogle.com/"><img src="docs/img/logo_gsoc.png" /></a>
 </th>
 <th align="center">
 <a href="https://developers.google.com/season-of-docs"><img src="docs/img/logo_gsod.png" /></a>
 </th>
 <th align="center">
-<img src="docs/img/logo_arkhn_light.png#gh-light-mode-only" />
-<img src="docs/img/logo_arkhn.png#gh-dark-mode-only" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_arkhn.png">
+  <img src="docs/img/logo_arkhn_light.png" />
+</picture>
+
 </th>
 <th align="center">
-<img src="docs/img/logo_cape_light.png#gh-light-mode-only" />
-<img src="docs/img/logo_cape.png#gh-dark-mode-only" />
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_cape.png">
+  <img src="docs/img/logo_cape_light.png" />
+</picture>
 </th>
 <th align="center">
 <a href="https://begin.ai/"><img src="docs/img/logo_begin.png" /></a>
 </th>
 </tr>
 </table>
 
 # Open Collective
 
 `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA. We are funded by our generous supporters on <a href="https://opencollective.com/openmined">Open Collective</a>. <br /><br />
-<img src="docs/img/opencollective_light.png#gh-light-mode-only" alt="Contributors" width="100%" />
-<img src="docs/img/opencollective_dark.png#gh-dark-mode-only" alt="Contributors" width="100%" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/opencollective_dark.png">
+  <img src="docs/img/opencollective_light.png" alt="Contributors" width="100%" />
+</picture>
 
 # Disclaimer
 
 Syft is under active development and is not yet ready for pilots on private data without our assistance. As early access participants, please contact us via [Slack](https://slack.openmined.org/) or email if you would like to ask a question or have a use case that you would like to discuss.
 
 # License
```

#### html2text {}

```diff
@@ -1,52 +1,62 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.0b8 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.0b9 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.8 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
 Provides-Extra: oblv License-File: LICENSE
 [https://pepy.tech/badge/syft] [https://badge.fury.io/py/syft.svg] [https://
 img.shields.io/badge/docker-images-blue?logo=docker] [https://github.com/
 OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev] [https:/
 /img.shields.io/badge/chat-on%20slack-purple?logo=slack] [https://
 img.shields.io/badge/read-docs-yellow?logo=mdbook]
 
-[Syft Logo] [Syft Logo] Perform `numpy`-like analysis on `data` that remains in
-`someone else's` server
-[Syft Overview] [Syft Overview]
-# Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ [docs/img/
-terminalizer.gif] 1. Install our handy ðµ cli tool which makes deploying a
-Domain or Network server a one-liner: `pip install -U hagrid` 2. Then run our
-interactive jupyter Install ð§ð½ââï¸ WizardBETA: `hagrid quickstart` -
-In the tutorial you will learn how to install and deploy: `PySyft` = our
-`numpy`-like ð Python library for computing on `private data` in someone
-else's `Domain` `PyGrid` = our ð³ `docker` / `k8s` / ð§ `vm` `Domain` &
-`Network` Servers where `private data` lives - During quickstart we will deploy
-`PyGrid` to localhost with ð³ `docker`, however ðµ HAGrid can deploy to
-`k8s` or a ð§ `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨
-`ansible`â  3. Read our ð Docs 4. Ask Questions â in `#support` on Slack
-# Install Notes - HAGrid Requires: ð `python` ð `git` - Run: `pip install
--U hagrid` - Interactive Install ð§ð½ââï¸ WizardBETA Requires ðµ
-`hagrid`: - Run: `hagrid quickstart` â `Windows` does not support `ansible`,
-preventing some remote deployment targets - PySyft Requires: ð `python 3.8+`
-- Run: `pip install -U syft` \*`macOS` Apple Silicon users need cmake: `brew
-install cmake` â¡`Windows` users must run this first: `pip install
-jaxlib==0.3.14 -f https://whls.blob.core.windows.net/unstable/index.html` -
-PyGrid Requires: ð³ `docker` / `k8s` or ð§ `ubuntu` VM - Run: `hagrid
-launch ...` # Versions `0.8.0 beta` - `dev` branch ðð½ `0.7.0` - Course_3
-Updated `0.6.0` - Course_3 `0.5.1` - Course_2 + M1 Hotfix `0.2.0` - `0.5.0`
-Deprecated PySyft and PyGrid use the same `version` and its best to match them
-up where possible. We release weekly betas which can be used in each context:
-PySyft: `pip install -U syft --pre` PyGrid: `hagrid launch ... tag=latest`
-HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually
-the best. # What is Syft? [Syft] [Syft] `Syft` is OpenMined's `open source`
-stack that provides `secure` and `private` Data Science in Python. Syft
+  [Syft Logo]  Perform `numpy`-like analysis on `data` that remains in `someone
+else's` server
+[Syft Logo]
+# Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ## Install syft on
+Python 3.8 - 3.10 ```bash $ pip install --pre syft -f https://
+whls.blob.core.windows.net/unstable/index.html ``` ## Launch a python dev
+Domain ```python # from Jupyter / Python import syft as sy sy.requires(">=0.8-
+beta") node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True,
+reset=True) ``` ```bash # or from the command line $ syft launch --name=my-
+domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:8080 ```
+## Connect with our Python Client ```python import syft as sy sy.requires
+(">=0.8-beta") domain_client = sy.login(port=8080, email="info@openmined.org",
+password="changethis") ``` ## Deploy to a Container Engine or Cloud 1. Install
+our handy ðµ cli tool which makes deploying a Domain or Gateway server a one-
+liner: `pip install -U hagrid` 2. Then run our interactive jupyter Install
+ð§ð½ââï¸ WizardBETA: `hagrid quickstart` 3. In the tutorial you will
+learn how to install and deploy: `PySyft` = our `numpy`-like ð Python
+library for computing on `private data` in someone else's `Domain` `PyGrid` =
+our ð³ `docker` / ð§ `vm` `Domain` & `Gateway` Servers where `private data`
+lives 4. During quickstart we will deploy `PyGrid` to localhost with ð³
+`docker`, however ðµ HAGrid can deploy to `podman` or a ð§ `ubuntu` VM on
+`azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨ `ansible`â  ## Docs and
+Support - ð Docs - `#support` on Slack # Install Notes - HAGrid 0.3
+Requires: ð `python` ð `git` - Run: `pip install -U hagrid` - Interactive
+Install ð§ð½ââï¸ WizardBETA Requires ðµ `hagrid`: - Run: `hagrid
+quickstart` â `Windows` does not support `ansible`, preventing some remote
+deployment targets - PySyft 0.8 Requires: ð `python 3.8 - 3.10` - Run: `pip
+install -U syft` \*`macOS` Apple Silicon users might need cmake: `brew install
+cmake` â¡`Windows` users must run this first: `pip install jaxlib==0.3.14 -
+f https://whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires:
+ð³ `docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.0`
+(Beta) - `dev` branch ðð½ `0.7.0` (Stable) - Course_3_Updated Deprecated:
+- `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix - `0.2.0` - `0.5.0`
+PySyft and PyGrid use the same `version` and its best to match them up where
+possible. We release weekly betas which can be used in each context: PySyft
+(Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch ... tag=latest`
+PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta): `hagrid launch ...
+tag=beta` HAGrid is a cli / deployment tool so the latest version of `hagrid`
+is usually the best. # What is Syft?   [Syft]  `Syft` is OpenMined's `open
+source` stack that provides `secure` and `private` Data Science in Python. Syft
 decouples `private data` from model training, using techniques like [Federated
 Learning](https://ai.googleblog.com/2017/04/federated-learning-
 collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/
 Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/
 wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and
 integration with `Deep Learning` frameworks, so that you as a `Data Scientist`
 can maintain your current workflow while using these new `privacy-enhancing
@@ -77,20 +87,20 @@
 |                 [Image]                  |                   [Image]                    |
 |_______ð¨ð»âð¼_Data|_______ð©ð½âð¬_Data_Sci|ntists
 | Provide `datasets` which they would like | Are end `users` who desire to perform        |
 |to make available for `study` by an       |`computations` or `answer` a specific         |
 |`outside party` they may or may not `fully|`question` using one or more data owners'     |
 |trust`_has_good_intentions._______________|`datasets`.___________________________________|
 |                     [Image]              |                        [Image]               |
-|________________ð°_Domain_Server____|__________________ð_Network_Server_____|
+|________________ð°_Domain_Server____|__________________ð_Gateway_Server_____|
 | Manages the `remote study` of the data by| Provides services to a group of `Data Owners`|
 |a `Data Scientist` and allows the `Data   |and `Data Scientists`, such as dataset        |
 |Owner` to manage the `data` and control   |`search` and bulk `project approval` (legal / |
 |the `privacy guarantees` of the subjects  |technical) to participate in a project. A     |
-|under study. It also acts as a            |network server acts as a bridge between it's  |
+|under study. It also acts as a            |gateway server acts as a bridge between it's  |
 |`gatekeeper` for the `Data Scientist's`   |members (`Domains`) and their subscribers     |
 |access to the data to compute and         |(`Data Scientists`) and can provide access to |
 |experiment_with_the_results.______________|a_collection_of_`domains`_at_once.____________|
 # Community
  ______________________________________________________________________________
 |[Image]|                           [Image]                            |[Image]|
 |       |                                                              |       |
@@ -105,22 +115,19 @@
 |_______|ð_A_generic_framework_for_privacy_preserving_deep_...__|_______|
 # Courses
  _______________________
 |[Image]|[Image]|[Image]|
 # Contributors OpenMined and Syft appreciates all contributors, if you would
 like to fix a bug or suggest a new feature, please see our [guidelines](https:/
 /openmined.github.io/PySyft/developer_guide/index.html).
-[Contributors] [Contributors] # Supporters
-                                                                                                      [docs/img/              [docs/img/
-  [docs/img/      [docs/img/     [docs/img/       [docs/img/       [docs/img/     [docs/img/   logo_arkhn_light.png#gh- logo_cape_light.png#gh-   [docs/img/
-logo_sloan.png] logo_meta.png] logo_torch.png] logo_udacity.png] logo_gsoc.png] logo_gsod.png] light-mode-only] [docs/  light-mode-only] [docs/ logo_begin.png]
-                                                                                                img/logo_arkhn.png#gh-   img/logo_cape.png#gh-
-                                                                                                   dark-mode-only]          dark-mode-only]
+  [Contributors]  # Supporters
+  [docs/img/      [docs/img/     [docs/img/       [docs/img/       [docs/img/     [docs/img/         [docs/img/            [docs/img/       [docs/img/
+logo_sloan.png] logo_meta.png] logo_torch.png] logo_udacity.png] logo_gsoc.png] logo_gsod.png] logo_arkhn_light.png] logo_cape_light.png] logo_begin.png]
 # Open Collective `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA.
 We are funded by our generous supporters on Open_Collective.
 
-[Contributors] [Contributors] # Disclaimer Syft is under active development and
-is not yet ready for pilots on private data without our assistance. As early
-access participants, please contact us via [Slack](https://slack.openmined.org/
-) or email if you would like to ask a question or have a use case that you
-would like to discuss. # License [Apache License 2.0](LICENSE)
+  [Contributors]  # Disclaimer Syft is under active development and is not yet
+ready for pilots on private data without our assistance. As early access
+participants, please contact us via [Slack](https://slack.openmined.org/) or
+email if you would like to ask a question or have a use case that you would
+like to discuss. # License [Apache License 2.0](LICENSE)
 Person_icons_created_by_Freepik_-_Flaticon
```

### Comparing `syft-0.8.0b8/README.md` & `syft-0.8.0b9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,112 @@
 <div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://pepy.tech/badge/syft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev" /></a> <a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
 <br /><br /></div>
 
-<img src="docs/img/title_syft_light.png#gh-light-mode-only" alt="Syft Logo" width="200px" />
-<img src="docs/img/title_syft_dark.png#gh-dark-mode-only" alt="Syft Logo" width="200px" />
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/title_syft_dark.png">
+  <img alt="Syft Logo" src="docs/img/title_syft_light.png" width="200px" />
+</picture>
 
 Perform `numpy`-like analysis on `data` that remains in `someone else's` server
 
 <div align="left">
-<img src="docs/img/header.png#gh-light-mode-only" alt="Syft Overview" width="100%" />
-<img src="docs/img/header.png#gh-dark-mode-only" alt="Syft Overview" width="100%" />
+<img alt="Syft Logo" src="docs/img/header.png" alt="Syft Overview" width="100%" />
 </div>
 
 # Quickstart
 
 ✅ `Linux` ✅ `macOS`\* ✅ `Windows`†‡
-<img src="docs/img/terminalizer.gif" width="50%" align="right" />
 
-1. Install our handy 🛵 cli tool which makes deploying a Domain or Network server a one-liner:  
+## Install syft on Python 3.8 - 3.10
+
+```bash
+$ pip install --pre syft -f https://whls.blob.core.windows.net/unstable/index.html
+```
+
+## Launch a python dev Domain
+
+```python
+# from Jupyter / Python
+import syft as sy
+sy.requires(">=0.8-beta")
+node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
+```
+
+```bash
+# or from the command line
+$ syft launch --name=my-domain --port=8080 --reset=True
+
+Starting syft-node server on 0.0.0.0:8080
+```
+
+## Connect with our Python Client
+
+```python
+import syft as sy
+sy.requires(">=0.8-beta")
+domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
+```
+
+## Deploy to a Container Engine or Cloud
+
+1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server a one-liner:  
    `pip install -U hagrid`
 
 2. Then run our interactive jupyter Install 🧙🏽‍♂️ Wizard<sup>BETA</sup>:  
    `hagrid quickstart`
 
-- In the tutorial you will learn how to install and deploy:  
-  `PySyft` = our `numpy`-like 🐍 Python library for computing on `private data` in someone else's `Domain`
+3. In the tutorial you will learn how to install and deploy:  
+   `PySyft` = our `numpy`-like 🐍 Python library for computing on `private data` in someone else's `Domain`
 
-  `PyGrid` = our 🐳 `docker` / `k8s` / 🐧 `vm` `Domain` & `Network` Servers where `private data` lives
+   `PyGrid` = our 🐳 `docker` / 🐧 `vm` `Domain` & `Gateway` Servers where `private data` lives
 
-- During quickstart we will deploy `PyGrid` to localhost with 🐳 `docker`, however 🛵 HAGrid can deploy to `k8s` or a 🐧 `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using 🔨 `ansible`†
+4. During quickstart we will deploy `PyGrid` to localhost with 🐳 `docker`, however 🛵 HAGrid can deploy to `podman` or a 🐧 `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using 🔨 `ansible`†
 
-3. Read our 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
-4. Ask Questions ❔ in `#support` on <a href="https://slack.openmined.org/">Slack</a>
+## Docs and Support
+
+- 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
+- `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
-- HAGrid Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
+- HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`  
   †`Windows` does not support `ansible`, preventing some remote deployment targets
-- PySyft Requires: 🐍 `python 3.8+` - Run: `pip install -U syft`  
-  \*`macOS` Apple Silicon users need cmake: `brew install cmake`  
+- PySyft 0.8 Requires: 🐍 `python 3.8 - 3.10` - Run: `pip install -U syft`  
+  \*`macOS` Apple Silicon users might need cmake: `brew install cmake`  
   ‡`Windows` users must run this first: `pip install jaxlib==0.3.14 -f https://whls.blob.core.windows.net/unstable/index.html`
-- PyGrid Requires: 🐳 `docker` / `k8s` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
+- PyGrid Requires: 🐳 `docker` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
 
 # Versions
 
-`0.8.0 beta` - `dev` branch 👈🏽  
-`0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>  
-`0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>  
-`0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix  
-`0.2.0` - `0.5.0` Deprecated
+`0.8.0` (Beta) - `dev` branch 👈🏽  
+`0.7.0` (Stable) - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
+
+Deprecated:
+
+- `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
+- `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
+- `0.2.0` - `0.5.0`
 
 PySyft and PyGrid use the same `version` and its best to match them up where possible. We release weekly betas which can be used in each context:
-PySyft: `pip install -U syft --pre`
-PyGrid: `hagrid launch ... tag=latest`
+
+PySyft (Stable): `pip install -U syft`  
+PyGrid (Stable) `hagrid launch ... tag=latest`
+
+PySyft (Beta): `pip install -U syft --pre`  
+PyGrid (Beta): `hagrid launch ... tag=beta`
 
 HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually the best.
 
 # What is Syft?
 
-<img align="right" src="docs/img/logo_big.png#gh-light-mode-only" alt="Syft" height="250" style="padding-left:30px;">
-
-<img align="right" src="docs/img/logo_big_dark.png#gh-dark-mode-only" alt="Syft" height="250" style="padding-left:30px;">
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_big_dark.png">
+  <img align="right" src="docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
+</picture>
 
 `Syft` is OpenMined's `open source` stack that provides `secure` and `private` Data Science in Python. Syft decouples `private data` from model training, using techniques like [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and integration with `Deep Learning` frameworks, so that you as a `Data Scientist` can maintain your current workflow while using these new `privacy-enhancing techniques`.
 
 ### Why should I use Syft?
 
 `Syft` allows a `Data Scientist` to ask `questions` about a `dataset` and, within `privacy limits` set by the `data owner`, get `answers` to those `questions`, all without obtaining a `copy` of the data itself. We call this process `Remote Data Science`. It means in a wide variety of `domains` across society, the current `risks` of sharing information (`copying` data) with someone such as, privacy invasion, IP theft and blackmail will no longer prevent the vast `benefits` such as innovation, insights and scientific discovery which secure access will provide.
 
@@ -157,52 +199,59 @@
 <tr>
 <th align="center">
 <img width="441" height="1">
 <p>🏰 Domain Server</p>
 </th>
 <th align="center">
 <img width="441" height="1">
-<p>🔗 Network Server</p>
+<p>🔗 Gateway Server</p>
 </th>
 </tr>
 <tr>
 <td valign="top">
 <!-- REMOVE THE BACKSLASHES -->
 
 Manages the `remote study` of the data by a `Data Scientist` and allows the `Data Owner` to manage the `data` and control the `privacy guarantees` of the subjects under study. It also acts as a `gatekeeper` for the `Data Scientist's` access to the data to compute and experiment with the results.
 
 </td>
 <td valign="top">
 <!-- REMOVE THE BACKSLASHES -->
 
-Provides services to a group of `Data Owners` and `Data Scientists`, such as dataset `search` and bulk `project approval` (legal / technical) to participate in a project. A network server acts as a bridge between it's members (`Domains`) and their subscribers (`Data Scientists`) and can provide access to a collection of `domains` at once.</td>
+Provides services to a group of `Data Owners` and `Data Scientists`, such as dataset `search` and bulk `project approval` (legal / technical) to participate in a project. A gateway server acts as a bridge between it's members (`Domains`) and their subscribers (`Data Scientists`) and can provide access to a collection of `domains` at once.</td>
 
 </tr>
 <tr>
 </table>
 
 # Community
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
-<img src="docs/img/panel_slack_title_light.png#gh-light-mode-only" alt="" width="100%" align="center" />
-<img src="docs/img/panel_slack_title_dark.png#gh-dark-mode-only" alt="" width="100%" align="center" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/panel_slack_title_dark.png">
+  <img src="docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
+</picture>
 
 <a href="https://slack.openmined.org/"><img src="docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
 
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
-<img src="docs/img/panel_title_videos_papers_light.png#gh-light-mode-only" alt="" width="100%" align="center" />
-<img src="docs/img/panel_title_videos_papers.png#gh-dark-mode-only" alt="" width="100%" align="center" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/panel_title_videos_papers.png">
+  <img src="docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
+</picture>
+
 <p align="left"><sub><sup>
 🎥 <a href="https://www.youtube.com/watch?v=qVf0tPBzr2k">PETs: Remote Data Science Unleashed - R gov 2021</a><br />
 🎥 <a href="https://youtu.be/sCoDWKTbh3s?list=PL_lsbAsL_o2BQKXG7mkGFA8LSApCnhljL">Introduction to Remote Data Science - PyTorch 2021</a><br />
 🎥 <a href="https://youtu.be/kzLeTz_vIeQ?list=PL_lsbAsL_o2BtOz6KUfUI_Zla6Rg5dmyc">The Future of AI Tools - PyTorch 2020</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=4zrU54VIK6k&t=1s">Privacy Preserving AI - MIT Deep Learning Series</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=Pr4erdusiW0">Privacy-Preserving Data Science - TWiML Talk #241</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=NJBBE_SN90A">Privacy Preserving AI - PyTorch Devcon 2019</a><br />
@@ -211,16 +260,19 @@
 📖 <a href="https://arxiv.org/pdf/1811.04017.pdf">A generic framework for privacy preserving deep ...</a>
 </sup></sup></p>
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
-<img src="docs/img/panel_padawan_title_light.png#gh-light-mode-only" alt="" width="100%" align="center" />
-<img src="docs/img/panel_padawan_title_dark.png#gh-dark-mode-only" alt="" width="100%" align="center" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/panel_padawan_title_dark.png">
+  <img src="docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
+</picture>
 
 <a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
 
 </div>
 </th>
 </tr>
 </table>
@@ -247,17 +299,20 @@
 </div>
 </th>
 </tr>
 </table>
 
 # Contributors
 
-OpenMined and Syft appreciates all contributors, if you would like to fix a bug or suggest a new feature, please see our [guidelines](https://openmined.github.io/PySyft/developer_guide/index.html).<br />  
-<img src="docs/img/contributors_light.jpg#gh-light-mode-only" alt="Contributors" width="100%" />
-<img src="docs/img/contributors_dark.jpg#gh-dark-mode-only" alt="Contributors" width="100%" />
+OpenMined and Syft appreciates all contributors, if you would like to fix a bug or suggest a new feature, please see our [guidelines](https://openmined.github.io/PySyft/developer_guide/index.html).<br />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/contributors_dark.jpg">
+  <img src="docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
+</picture>
 
 # Supporters
 
 <table border="0">
 <tr>
 <th align="center">
 <a href="https://sloan.org/"><img src="docs/img/logo_sloan.png" /></a>
@@ -274,36 +329,45 @@
 <th align="center">
 <a href="https://summerofcode.withgoogle.com/"><img src="docs/img/logo_gsoc.png" /></a>
 </th>
 <th align="center">
 <a href="https://developers.google.com/season-of-docs"><img src="docs/img/logo_gsod.png" /></a>
 </th>
 <th align="center">
-<img src="docs/img/logo_arkhn_light.png#gh-light-mode-only" />
-<img src="docs/img/logo_arkhn.png#gh-dark-mode-only" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_arkhn.png">
+  <img src="docs/img/logo_arkhn_light.png" />
+</picture>
+
 </th>
 <th align="center">
-<img src="docs/img/logo_cape_light.png#gh-light-mode-only" />
-<img src="docs/img/logo_cape.png#gh-dark-mode-only" />
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_cape.png">
+  <img src="docs/img/logo_cape_light.png" />
+</picture>
 </th>
 <th align="center">
 <a href="https://begin.ai/"><img src="docs/img/logo_begin.png" /></a>
 </th>
 </tr>
 </table>
 
 # Open Collective
 
 `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA. We are funded by our generous supporters on <a href="https://opencollective.com/openmined">Open Collective</a>. <br /><br />
-<img src="docs/img/opencollective_light.png#gh-light-mode-only" alt="Contributors" width="100%" />
-<img src="docs/img/opencollective_dark.png#gh-dark-mode-only" alt="Contributors" width="100%" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/opencollective_dark.png">
+  <img src="docs/img/opencollective_light.png" alt="Contributors" width="100%" />
+</picture>
 
 # Disclaimer
 
 Syft is under active development and is not yet ready for pilots on private data without our assistance. As early access participants, please contact us via [Slack](https://slack.openmined.org/) or email if you would like to ask a question or have a use case that you would like to discuss.
 
 # License
 
 [Apache License 2.0](LICENSE)<br />
 <a href="https://www.flaticon.com/free-icons/person" title="person icons">Person icons created by Freepik - Flaticon</a>
 
-<!-- 🥇 -->
+<!-- 🥇 -->
```

#### html2text {}

```diff
@@ -1,43 +1,53 @@
 [https://pepy.tech/badge/syft] [https://badge.fury.io/py/syft.svg] [https://
 img.shields.io/badge/docker-images-blue?logo=docker] [https://github.com/
 OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev] [https:/
 /img.shields.io/badge/chat-on%20slack-purple?logo=slack] [https://
 img.shields.io/badge/read-docs-yellow?logo=mdbook]
 
-[Syft Logo] [Syft Logo] Perform `numpy`-like analysis on `data` that remains in
-`someone else's` server
-[Syft Overview] [Syft Overview]
-# Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ [docs/img/
-terminalizer.gif] 1. Install our handy ðµ cli tool which makes deploying a
-Domain or Network server a one-liner: `pip install -U hagrid` 2. Then run our
-interactive jupyter Install ð§ð½ââï¸ WizardBETA: `hagrid quickstart` -
-In the tutorial you will learn how to install and deploy: `PySyft` = our
-`numpy`-like ð Python library for computing on `private data` in someone
-else's `Domain` `PyGrid` = our ð³ `docker` / `k8s` / ð§ `vm` `Domain` &
-`Network` Servers where `private data` lives - During quickstart we will deploy
-`PyGrid` to localhost with ð³ `docker`, however ðµ HAGrid can deploy to
-`k8s` or a ð§ `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨
-`ansible`â  3. Read our ð Docs 4. Ask Questions â in `#support` on Slack
-# Install Notes - HAGrid Requires: ð `python` ð `git` - Run: `pip install
--U hagrid` - Interactive Install ð§ð½ââï¸ WizardBETA Requires ðµ
-`hagrid`: - Run: `hagrid quickstart` â `Windows` does not support `ansible`,
-preventing some remote deployment targets - PySyft Requires: ð `python 3.8+`
-- Run: `pip install -U syft` \*`macOS` Apple Silicon users need cmake: `brew
-install cmake` â¡`Windows` users must run this first: `pip install
-jaxlib==0.3.14 -f https://whls.blob.core.windows.net/unstable/index.html` -
-PyGrid Requires: ð³ `docker` / `k8s` or ð§ `ubuntu` VM - Run: `hagrid
-launch ...` # Versions `0.8.0 beta` - `dev` branch ðð½ `0.7.0` - Course_3
-Updated `0.6.0` - Course_3 `0.5.1` - Course_2 + M1 Hotfix `0.2.0` - `0.5.0`
-Deprecated PySyft and PyGrid use the same `version` and its best to match them
-up where possible. We release weekly betas which can be used in each context:
-PySyft: `pip install -U syft --pre` PyGrid: `hagrid launch ... tag=latest`
-HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually
-the best. # What is Syft? [Syft] [Syft] `Syft` is OpenMined's `open source`
-stack that provides `secure` and `private` Data Science in Python. Syft
+  [Syft Logo]  Perform `numpy`-like analysis on `data` that remains in `someone
+else's` server
+[Syft Logo]
+# Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ## Install syft on
+Python 3.8 - 3.10 ```bash $ pip install --pre syft -f https://
+whls.blob.core.windows.net/unstable/index.html ``` ## Launch a python dev
+Domain ```python # from Jupyter / Python import syft as sy sy.requires(">=0.8-
+beta") node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True,
+reset=True) ``` ```bash # or from the command line $ syft launch --name=my-
+domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:8080 ```
+## Connect with our Python Client ```python import syft as sy sy.requires
+(">=0.8-beta") domain_client = sy.login(port=8080, email="info@openmined.org",
+password="changethis") ``` ## Deploy to a Container Engine or Cloud 1. Install
+our handy ðµ cli tool which makes deploying a Domain or Gateway server a one-
+liner: `pip install -U hagrid` 2. Then run our interactive jupyter Install
+ð§ð½ââï¸ WizardBETA: `hagrid quickstart` 3. In the tutorial you will
+learn how to install and deploy: `PySyft` = our `numpy`-like ð Python
+library for computing on `private data` in someone else's `Domain` `PyGrid` =
+our ð³ `docker` / ð§ `vm` `Domain` & `Gateway` Servers where `private data`
+lives 4. During quickstart we will deploy `PyGrid` to localhost with ð³
+`docker`, however ðµ HAGrid can deploy to `podman` or a ð§ `ubuntu` VM on
+`azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨ `ansible`â  ## Docs and
+Support - ð Docs - `#support` on Slack # Install Notes - HAGrid 0.3
+Requires: ð `python` ð `git` - Run: `pip install -U hagrid` - Interactive
+Install ð§ð½ââï¸ WizardBETA Requires ðµ `hagrid`: - Run: `hagrid
+quickstart` â `Windows` does not support `ansible`, preventing some remote
+deployment targets - PySyft 0.8 Requires: ð `python 3.8 - 3.10` - Run: `pip
+install -U syft` \*`macOS` Apple Silicon users might need cmake: `brew install
+cmake` â¡`Windows` users must run this first: `pip install jaxlib==0.3.14 -
+f https://whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires:
+ð³ `docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.0`
+(Beta) - `dev` branch ðð½ `0.7.0` (Stable) - Course_3_Updated Deprecated:
+- `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix - `0.2.0` - `0.5.0`
+PySyft and PyGrid use the same `version` and its best to match them up where
+possible. We release weekly betas which can be used in each context: PySyft
+(Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch ... tag=latest`
+PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta): `hagrid launch ...
+tag=beta` HAGrid is a cli / deployment tool so the latest version of `hagrid`
+is usually the best. # What is Syft?   [Syft]  `Syft` is OpenMined's `open
+source` stack that provides `secure` and `private` Data Science in Python. Syft
 decouples `private data` from model training, using techniques like [Federated
 Learning](https://ai.googleblog.com/2017/04/federated-learning-
 collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/
 Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/
 wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and
 integration with `Deep Learning` frameworks, so that you as a `Data Scientist`
 can maintain your current workflow while using these new `privacy-enhancing
@@ -68,20 +78,20 @@
 |                 [Image]                  |                   [Image]                    |
 |_______ð¨ð»âð¼_Data|_______ð©ð½âð¬_Data_Sci|ntists
 | Provide `datasets` which they would like | Are end `users` who desire to perform        |
 |to make available for `study` by an       |`computations` or `answer` a specific         |
 |`outside party` they may or may not `fully|`question` using one or more data owners'     |
 |trust`_has_good_intentions._______________|`datasets`.___________________________________|
 |                     [Image]              |                        [Image]               |
-|________________ð°_Domain_Server____|__________________ð_Network_Server_____|
+|________________ð°_Domain_Server____|__________________ð_Gateway_Server_____|
 | Manages the `remote study` of the data by| Provides services to a group of `Data Owners`|
 |a `Data Scientist` and allows the `Data   |and `Data Scientists`, such as dataset        |
 |Owner` to manage the `data` and control   |`search` and bulk `project approval` (legal / |
 |the `privacy guarantees` of the subjects  |technical) to participate in a project. A     |
-|under study. It also acts as a            |network server acts as a bridge between it's  |
+|under study. It also acts as a            |gateway server acts as a bridge between it's  |
 |`gatekeeper` for the `Data Scientist's`   |members (`Domains`) and their subscribers     |
 |access to the data to compute and         |(`Data Scientists`) and can provide access to |
 |experiment_with_the_results.______________|a_collection_of_`domains`_at_once.____________|
 # Community
  ______________________________________________________________________________
 |[Image]|                           [Image]                            |[Image]|
 |       |                                                              |       |
@@ -96,22 +106,19 @@
 |_______|ð_A_generic_framework_for_privacy_preserving_deep_...__|_______|
 # Courses
  _______________________
 |[Image]|[Image]|[Image]|
 # Contributors OpenMined and Syft appreciates all contributors, if you would
 like to fix a bug or suggest a new feature, please see our [guidelines](https:/
 /openmined.github.io/PySyft/developer_guide/index.html).
-[Contributors] [Contributors] # Supporters
-                                                                                                      [docs/img/              [docs/img/
-  [docs/img/      [docs/img/     [docs/img/       [docs/img/       [docs/img/     [docs/img/   logo_arkhn_light.png#gh- logo_cape_light.png#gh-   [docs/img/
-logo_sloan.png] logo_meta.png] logo_torch.png] logo_udacity.png] logo_gsoc.png] logo_gsod.png] light-mode-only] [docs/  light-mode-only] [docs/ logo_begin.png]
-                                                                                                img/logo_arkhn.png#gh-   img/logo_cape.png#gh-
-                                                                                                   dark-mode-only]          dark-mode-only]
+  [Contributors]  # Supporters
+  [docs/img/      [docs/img/     [docs/img/       [docs/img/       [docs/img/     [docs/img/         [docs/img/            [docs/img/       [docs/img/
+logo_sloan.png] logo_meta.png] logo_torch.png] logo_udacity.png] logo_gsoc.png] logo_gsod.png] logo_arkhn_light.png] logo_cape_light.png] logo_begin.png]
 # Open Collective `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA.
 We are funded by our generous supporters on Open_Collective.
 
-[Contributors] [Contributors] # Disclaimer Syft is under active development and
-is not yet ready for pilots on private data without our assistance. As early
-access participants, please contact us via [Slack](https://slack.openmined.org/
-) or email if you would like to ask a question or have a use case that you
-would like to discuss. # License [Apache License 2.0](LICENSE)
+  [Contributors]  # Disclaimer Syft is under active development and is not yet
+ready for pilots on private data without our assistance. As early access
+participants, please contact us via [Slack](https://slack.openmined.org/) or
+email if you would like to ask a question or have a use case that you would
+like to discuss. # License [Apache License 2.0](LICENSE)
 Person_icons_created_by_Freepik_-_Flaticon
```

### Comparing `syft-0.8.0b8/setup.cfg` & `syft-0.8.0b9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.0-beta.8"
+version = attr: "0.8.0-beta.9"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -27,32 +27,35 @@
 	bcrypt==4.0.1
 	flax==0.5.3
 	forbiddenfruit==0.1.4
 	gevent==22.10.2
 	gipc==1.5.0
 	jax==0.3.14
 	jaxlib==0.3.14
-	loguru==0.6.0
+	loguru==0.7.0
 	numpy==1.24.2
 	opendp==0.6.2
 	packaging>=21.0
 	pandas==1.5.3
 	pyarrow==11.0.0
 	pycapnp==1.3.0
-	pydantic[email]==1.10.6
+	pydantic[email]==1.10.7
 	pymongo==4.3.3
 	pynacl==1.5.0
-	redis==4.5.1
+	redis==4.5.4
 	requests==2.28.2
 	RestrictedPython==6.0
 	result==0.9.0
 	tqdm==4.65.0
 	typeguard==2.13.3
 	typing_extensions==4.5.0
 	sherlock[redis,filelock]==0.4.1
+	uvicorn[standard]==0.21.1
+	fastapi==0.95.1
+	hagrid>=0.3
 telemetry = 
 	opentelemetry-api==1.14.0
 	opentelemetry-sdk==1.14.0
 	opentelemetry-exporter-jaeger==1.14.0
 	opentelemetry-instrumentation==0.35b0
 	opentelemetry-instrumentation-requests==0.35b0
 install_requires = 
@@ -89,14 +92,18 @@
 	pytest-rerunfailures
 	coverage
 	joblib
 	faker
 oblv = 
 	pyoblv==0.2.0
 
+[options.entry_points]
+console_scripts = 
+	syft=syft.node.run:run
+
 [test]
 addopts = --verbose
 extras = True
 
 [tool:pytest]
 addopts = --verbose
 norecursedirs =
```

### Comparing `syft-0.8.0b8/src/syft/VERSION` & `syft-0.8.0b9/src/syft/VERSION`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.0-beta.8"
+__version__ = "0.8.0-beta.9"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/action_object.py` & `syft-0.8.0b9/src/syft/service/action/action_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 from typing import Union
 
 # third party
 import pydantic
 from typing_extensions import Self
 
 # relative
+from ...client.client import SyftClient
+from ...serde.serializable import serializable
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftBaseObject
+from ...types.syft_object import SyftObject
+from ...types.uid import LineageID
+from ...types.uid import UID
+from ..response import SyftException
 from .action_data_empty import ActionDataEmpty
 from .action_types import action_type_for_type
 from .action_types import action_types
-from .client import SyftClient
-from .response import SyftException
-from .serializable import serializable
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftBaseObject
-from .syft_object import SyftObject
-from .uid import LineageID
-from .uid import UID
 
 
 @serializable()
 class Action(SyftObject):
     __canonical_name__ = "Action"
     __version__ = SYFT_OBJECT_VERSION_1
 
@@ -576,16 +576,16 @@
 
     def syft_execute_action(
         self, action: Action, sync: bool = True
     ) -> ActionObjectPointer:
         if self.syft_node_uid is None:
             raise SyftException("Pointers can't execute without a node_uid.")
         # relative
-        from .api import APIRegistry
-        from .api import SyftAPICall
+        from ...client.api import APIRegistry
+        from ...client.api import SyftAPICall
 
         api = APIRegistry.api_for(node_uid=self.syft_node_uid)
 
         kwargs = {"action": action}
         api_call = SyftAPICall(
             node_uid=self.syft_node_uid, path="action.execute", args=[], kwargs=kwargs
         )
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/action_permissions.py` & `syft-0.8.0b9/src/syft/service/action/action_permissions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # stdlib
 from enum import Enum
 from typing import Optional
 
 # relative
-from .credentials import SyftVerifyKey
-from .serializable import serializable
-from .uid import UID
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...types.uid import UID
 
 
 @serializable()
 class ActionPermission(Enum):
     OWNER = 1
     READ = 2
     ALL_READ = 4
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/action_service.py` & `syft-0.8.0b9/src/syft/service/action/action_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,36 +8,36 @@
 # third party
 import numpy as np
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
+from ...serde.serializable import serializable
+from ...types.twin_object import TwinObject
+from ...types.uid import UID
+from ..code.user_code import UserCode
+from ..code.user_code import execute_byte_code
+from ..context import AuthedServiceContext
+from ..response import SyftError
+from ..response import SyftSuccess
+from ..service import AbstractService
+from ..service import SERVICE_TO_TYPES
+from ..service import TYPE_TO_SERVICE
+from ..service import service_method
+from ..user.user_roles import GUEST_ROLE_LEVEL
 from .action_object import Action
 from .action_object import ActionObject
 from .action_object import ActionObjectPointer
 from .action_object import AnyActionObject
 from .action_store import ActionStore
 from .action_types import action_type_for_type
-from .context import AuthedServiceContext
 from .numpy import NumpyArrayObject
 from .pandas import PandasDataFrameObject  # noqa: F401
 from .pandas import PandasSeriesObject  # noqa: F401
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .service import AbstractService
-from .service import SERVICE_TO_TYPES
-from .service import TYPE_TO_SERVICE
-from .service import service_method
-from .twin_object import TwinObject
-from .uid import UID
-from .user_code import UserCode
-from .user_code import execute_byte_code
-from .user_roles import GUEST_ROLE_LEVEL
 
 
 @serializable()
 class TwinMode(Enum):
     NONE = 0
     PRIVATE = 1
     MOCK = 2
@@ -97,22 +97,19 @@
 
     @service_method(path="action.get", name="get", roles=GUEST_ROLE_LEVEL)
     def get(
         self,
         context: AuthedServiceContext,
         uid: UID,
         twin_mode: TwinMode = TwinMode.PRIVATE,
-        skip_permission: bool = False,
     ) -> Result[ActionObject, str]:
         """Get an object from the action store"""
         # TODO 🟣 Temporarily added skip permission arguments for enclave
         # until permissions are fully integrated
-        result = self.store.get(
-            uid=uid, credentials=context.credentials, skip_permission=skip_permission
-        )
+        result = self.store.get(uid=uid, credentials=context.credentials)
         if result.is_ok():
             obj = result.ok()
             if isinstance(obj, TwinObject):
                 if twin_mode == TwinMode.PRIVATE:
                     obj = obj.private
                     obj.syft_point_to(context.node.id)
                 elif twin_mode == TwinMode.MOCK:
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/action_store.py` & `syft-0.8.0b9/src/syft/service/action/action_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 
 # third party
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
+from ...node.credentials import SyftSigningKey
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...store.dict_document_store import DictStoreConfig
+from ...store.document_store import BasePartitionSettings
+from ...store.document_store import StoreConfig
+from ...types.syft_object import SyftObject
+from ...types.twin_object import TwinObject
+from ...types.uid import UID
+from ..response import SyftSuccess
 from .action_permissions import ActionObjectEXECUTE
 from .action_permissions import ActionObjectOWNER
 from .action_permissions import ActionObjectPermission
 from .action_permissions import ActionObjectREAD
 from .action_permissions import ActionObjectWRITE
 from .action_permissions import ActionPermission
-from .credentials import SyftSigningKey
-from .credentials import SyftVerifyKey
-from .dict_document_store import DictStoreConfig
-from .document_store import BasePartitionSettings
-from .document_store import StoreConfig
-from .response import SyftSuccess
-from .serializable import serializable
-from .syft_object import SyftObject
-from .twin_object import TwinObject
-from .uid import UID
 
 
 class ActionStore:
     pass
 
 
 @serializable()
@@ -55,23 +55,21 @@
         self.permissions = self.store_config.backing_store(
             "permissions", self.settings, self.store_config, ddtype=set
         )
         if root_verify_key is None:
             root_verify_key = SyftSigningKey.generate().verify_key
         self.root_verify_key = root_verify_key
 
-    def get(
-        self, uid: UID, credentials: SyftVerifyKey, skip_permission: bool = False
-    ) -> Result[SyftObject, str]:
+    def get(self, uid: UID, credentials: SyftVerifyKey) -> Result[SyftObject, str]:
         # TODO 🟣 Temporarily added skip permission argument for enclave
         # until permissions are fully integrated
         # if you get something you need READ permission
         read_permission = ActionObjectREAD(uid=uid, credentials=credentials)
         # if True:
-        if skip_permission or self.has_permission(read_permission):
+        if self.has_permission(read_permission):
             syft_object = self.data[uid]
             return Ok(syft_object)
         return Err(f"Permission: {read_permission} denied")
 
     def get_pointer(
         self, uid: UID, credentials: SyftVerifyKey, node_uid: UID
     ) -> Result[SyftObject, str]:
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/action_types.py` & `syft-0.8.0b9/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/core/node/new/api.py` & `syft-0.8.0b9/src/syft/client/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,35 +18,35 @@
 from pydantic import BaseModel
 from pydantic import EmailStr
 from result import OkErr
 from result import Result
 from typeguard import check_type
 
 # relative
-from ....telemetry import instrument
+from ..abstract_node import AbstractNode
+from ..node.credentials import SyftSigningKey
+from ..node.credentials import SyftVerifyKey
+from ..serde.deserialize import _deserialize
+from ..serde.recursive import index_syft_by_module_name
+from ..serde.serializable import serializable
+from ..serde.serialize import _serialize
+from ..serde.signature import Signature
+from ..serde.signature import signature_remove_context
+from ..serde.signature import signature_remove_self
+from ..service.context import AuthedServiceContext
+from ..service.response import SyftAttributeError
+from ..service.response import SyftError
+from ..service.response import SyftSuccess
+from ..service.service import UserServiceConfigRegistry
+from ..types.syft_object import SYFT_OBJECT_VERSION_1
+from ..types.syft_object import SyftBaseObject
+from ..types.syft_object import SyftObject
+from ..types.uid import UID
+from ..util.telemetry import instrument
 from .connection import NodeConnection
-from .context import AuthedServiceContext
-from .credentials import SyftSigningKey
-from .credentials import SyftVerifyKey
-from .deserialize import _deserialize
-from .node import NewNode
-from .recursive import index_syft_by_module_name
-from .response import SyftAttributeError
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .serialize import _serialize
-from .service import UserServiceConfigRegistry
-from .signature import Signature
-from .signature import signature_remove_context
-from .signature import signature_remove_self
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftBaseObject
-from .syft_object import SyftObject
-from .uid import UID
 
 
 class APIRegistry:
     __api_registry__: Dict[str, SyftAPI] = {}
 
     @classmethod
     def set_api_for(cls, node_uid: Union[UID, str], api: SyftAPI) -> None:
@@ -307,19 +307,19 @@
     refresh_api_callback: Optional[Callable] = None
 
     # def __post_init__(self) -> None:
     #     pass
 
     @staticmethod
     def for_user(
-        node: NewNode, user_verify_key: Optional[SyftVerifyKey] = None
+        node: AbstractNode, user_verify_key: Optional[SyftVerifyKey] = None
     ) -> SyftAPI:
         # relative
         # TODO: Maybe there is a possibility of merging ServiceConfig and APIEndpoint
-        from .user_code_service import UserCodeService
+        from ..service.code.user_code_service import UserCodeService
 
         # find user role by verify_key
         # TODO: we should probably not allow empty verify keys but instead make user always register
         role = node.get_role_for_credentials(user_verify_key)
         _user_service_config_registry = UserServiceConfigRegistry.from_role(role)
         endpoints = {}
 
@@ -339,25 +339,26 @@
 
         # 🟡 TODO 35: fix root context
         context = AuthedServiceContext(credentials=user_verify_key)
         method = node.get_method_with_context(UserCodeService.get_all_for_user, context)
         code_items = method()
 
         for code_item in code_items:
-            path = "code.call"
+            api_path = "code.call"
+            unique_path = f"code.call_{code_item.service_func_name}"
             endpoint = APIEndpoint(
-                path=path,
+                path=api_path,
                 name=code_item.service_func_name,
                 description="",
                 doc_string=f"Users custom func {code_item.service_func_name}",
                 signature=code_item.signature,
                 has_self=False,
                 pre_kwargs={"uid": code_item.id},
             )
-            endpoints[path] = endpoint
+            endpoints[unique_path] = endpoint
 
         return SyftAPI(node_name=node.name, node_uid=node.id, endpoints=endpoints)
 
     def make_call(self, api_call: SyftAPICall) -> Result:
         signed_call = api_call.sign(credentials=self.signing_key)
         signed_result = self.connection.make_call(signed_call)
 
@@ -378,16 +379,16 @@
             else:
                 return result.err()
         return result
 
     def update_api(self, api_call_result):
         # TODO: hacky stuff with typing and imports to prevent circular imports
         # relative
-        from .request import Request
-        from .request import UserCodeStatusChange
+        from ..service.request.request import Request
+        from ..service.request.request import UserCodeStatusChange
 
         if isinstance(api_call_result, Request) and any(
             [isinstance(x, UserCodeStatusChange) for x in api_call_result.changes]
         ):
             if self.refresh_api_callback is not None:
                 self.refresh_api_callback()
 
@@ -407,15 +408,15 @@
                 submodule_path = f"{_self.path}.{module}"
                 _self._add_submodule(module, APIModule(path=submodule_path))
             _self = getattr(_self, module)
         _self._add_submodule(_last_module, endpoint_method)
 
     def generate_endpoints(self) -> None:
         api_module = APIModule(path="")
-        for k, v in self.endpoints.items():
+        for _, v in self.endpoints.items():
             signature = v.signature
             if not v.has_self:
                 signature = signature_remove_self(signature)
             signature = signature_remove_context(signature)
             endpoint_function = generate_remote_function(
                 self.node_uid,
                 signature,
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/array.py` & `syft-0.8.0b9/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/core/node/new/arrow.py` & `syft-0.8.0b9/src/syft/serde/arrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import cast
 
 # third party
 import numpy as np
 import pyarrow as pa
 
 # relative
-from ....experimental_flags import ApacheArrowCompression
-from ....experimental_flags import flags
+from ..util.experimental_flags import ApacheArrowCompression
+from ..util.experimental_flags import flags
 from .deserialize import _deserialize
 from .serialize import _serialize
 
 
 def arrow_serialize(obj: np.ndarray) -> bytes:
     original_dtype = obj.dtype
     apache_arrow = pa.Tensor.from_numpy(obj=obj)
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/client.py` & `syft-0.8.0b9/src/syft/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,41 +16,41 @@
 from requests import Session
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from tqdm import tqdm
 from typing_extensions import Self
 
 # relative
-from .... import __version__
-from ....logger import debug
-from ....telemetry import instrument
-from ....util import verify_tls
-from ...node.new.credentials import UserLoginCredentials
-from ...node.new.node_metadata import NodeMetadataJSON
-from ...node.new.user import UserCreate
-from ...node.new.user import UserPrivateKey
+from .. import __version__
+from ..abstract_node import AbstractNode
+from ..node.credentials import SyftSigningKey
+from ..node.credentials import UserLoginCredentials
+from ..serde.deserialize import _deserialize
+from ..serde.serializable import serializable
+from ..serde.serialize import _serialize
+from ..service.context import NodeServiceContext
+from ..service.dataset.dataset import CreateDataset
+from ..service.metadata.node_metadata import NodeMetadataJSON
+from ..service.response import SyftError
+from ..service.response import SyftSuccess
+from ..service.user.user import UserCreate
+from ..service.user.user import UserPrivateKey
+from ..service.user.user_service import UserService
+from ..types.grid_url import GridURL
+from ..types.syft_object import SYFT_OBJECT_VERSION_1
+from ..types.uid import UID
+from ..util.logger import debug
+from ..util.telemetry import instrument
+from ..util.util import verify_tls
 from .api import APIModule
 from .api import APIRegistry
 from .api import SignedSyftAPICall
 from .api import SyftAPI
 from .api import SyftAPICall
 from .connection import NodeConnection
-from .context import NodeServiceContext
-from .credentials import SyftSigningKey
-from .dataset import CreateDataset
-from .deserialize import _deserialize
-from .grid_url import GridURL
-from .node import NewNode
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .serialize import _serialize
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .uid import UID
-from .user_service import UserService
 
 # use to enable mitm proxy
 # from syft.grid.connections.http_connection import HTTPConnection
 # HTTPConnection.proxies = {"http": "http://127.0.0.1:8080"}
 
 
 def upgrade_tls(url: GridURL, response: Response) -> GridURL:
@@ -222,15 +222,15 @@
 
 
 @serializable()
 class PythonConnection(NodeConnection):
     __canonical_name__ = "PythonConnection"
     __version__ = SYFT_OBJECT_VERSION_1
 
-    node: NewNode
+    node: AbstractNode
     proxy_target_uid: Optional[UID]
 
     def with_proxy(self, proxy_target_uid: UID) -> Self:
         return PythonConnection(node=self.node, proxy_target_uid=proxy_target_uid)
 
     def get_node_metadata(self, credentials: SyftSigningKey) -> NodeMetadataJSON:
         if self.proxy_target_uid:
@@ -325,15 +325,15 @@
         return bool(self.credentials)
 
     @staticmethod
     def from_url(url: Union[str, GridURL]) -> Self:
         return SyftClient(connection=HTTPConnection(GridURL.from_url(url)))
 
     @staticmethod
-    def from_node(node: NewNode) -> Self:
+    def from_node(node: AbstractNode) -> Self:
         return SyftClient(connection=PythonConnection(node=node))
 
     @property
     def name(self) -> Optional[str]:
         return self.metadata.name if self.metadata else None
 
     @property
@@ -353,15 +353,15 @@
 
     def guest(self) -> Self:
         self.credentials = SyftSigningKey.generate()
         return self
 
     def upload_dataset(self, dataset: CreateDataset) -> Union[SyftSuccess, SyftError]:
         # relative
-        from .twin_object import TwinObject
+        from ..types.twin_object import TwinObject
 
         for asset in tqdm(dataset.asset_list):
             print(f"Uploading: {asset.name}")
             try:
                 twin = TwinObject(private_obj=asset.data, mock_obj=asset.mock)
             except Exception as e:
                 return SyftError(message=f"Failed to create twin. {e}")
@@ -379,15 +379,15 @@
                 return tuple(valid.err())
             return valid.err()
 
     def exchange_route(self, client: Self) -> None:
         result = self.api.services.network.exchange_credentials_with(client=client)
         if result:
             # relative
-            from .network_service import connection_to_route
+            from ..service.network.network_service import connection_to_route
 
             route = connection_to_route(self.connection)
             result = self.api.services.network.add_route_for(route=route, client=client)
         return result
 
     def apply_to_gateway(self, client: Self) -> None:
         return self.exchange_route(client)
@@ -466,15 +466,15 @@
             self._fetch_api(self.credentials)
             response = response[0]
         return response
 
     @property
     def peer(self) -> Any:
         # relative
-        from .network_service import NodePeer
+        from ..service.network.network_service import NodePeer
 
         return NodePeer.from_client(self)
 
     @property
     def route(self) -> Any:
         return self.connection.route
 
@@ -526,15 +526,15 @@
         APIRegistry.set_api_for(node_uid=self.id, api=_api)
         self._api = _api
 
 
 @instrument
 def connect(
     url: Union[str, GridURL] = DEFAULT_PYGRID_ADDRESS,
-    node: Optional[NewNode] = None,
+    node: Optional[AbstractNode] = None,
     port: Optional[int] = None,
 ) -> SyftClient:
     if node:
         connection = PythonConnection(node=node)
     else:
         url = GridURL.from_url(url)
         if isinstance(port, (int, str)):
@@ -543,15 +543,15 @@
     _client = SyftClient(connection=connection)
     return _client
 
 
 @instrument
 def login(
     url: Union[str, GridURL] = DEFAULT_PYGRID_ADDRESS,
-    node: Optional[NewNode] = None,
+    node: Optional[AbstractNode] = None,
     port: Optional[int] = None,
     email: Optional[str] = None,
     password: Optional[str] = None,
     cache: bool = True,
 ) -> SyftClient:
     _client = connect(url=url, node=node, port=port)
     connection = _client.connection
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/connection.py` & `syft-0.8.0b9/src/syft/client/connection.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # stdlib
 from typing import Any
 
 # relative
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftObject
+from ..types.syft_object import SYFT_OBJECT_VERSION_1
+from ..types.syft_object import SyftObject
 
 
 class NodeConnection(SyftObject):
     __canonical_name__ = "NodeConnection"
     __version__ = SYFT_OBJECT_VERSION_1
 
     def get_cache_key() -> str:
@@ -15,10 +15,10 @@
 
     def __repr__(self) -> str:
         return f"<{type(self).__name__}"
 
     @property
     def route(self) -> Any:
         # relative
-        from .network_service import connection_to_route
+        from ..service.network.network_service import connection_to_route
 
         return connection_to_route(self)
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/context.py` & `syft-0.8.0b9/src/syft/service/context.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 from typing import List
 from typing import Optional
 
 # third party
 from typing_extensions import Self
 
 # relative
-from .credentials import SyftVerifyKey
-from .credentials import UserLoginCredentials
-from .node import NewNode
-from .syft_object import Context
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftBaseObject
-from .syft_object import SyftObject
-from .uid import UID
-from .user_roles import ROLE_TO_CAPABILITIES
-from .user_roles import ServiceRole
-from .user_roles import ServiceRoleCapability
+from ..abstract_node import AbstractNode
+from ..node.credentials import SyftVerifyKey
+from ..node.credentials import UserLoginCredentials
+from ..types.syft_object import Context
+from ..types.syft_object import SYFT_OBJECT_VERSION_1
+from ..types.syft_object import SyftBaseObject
+from ..types.syft_object import SyftObject
+from ..types.uid import UID
+from .user.user_roles import ROLE_TO_CAPABILITIES
+from .user.user_roles import ServiceRole
+from .user.user_roles import ServiceRoleCapability
 
 
 class NodeServiceContext(Context, SyftObject):
     __canonical_name__ = "NodeServiceContext"
     __version__ = SYFT_OBJECT_VERSION_1
     id: Optional[UID]
-    node: Optional[NewNode]
+    node: Optional[AbstractNode]
 
 
 class AuthedServiceContext(NodeServiceContext):
     __canonical_name__ = "AuthedServiceContext"
     __version__ = SYFT_OBJECT_VERSION_1
 
     credentials: SyftVerifyKey
@@ -38,20 +38,20 @@
 
 
 class UnauthedServiceContext(NodeServiceContext):
     __canonical_name__ = "UnauthedServiceContext"
     __version__ = SYFT_OBJECT_VERSION_1
 
     login_credentials: UserLoginCredentials
-    node: Optional[NewNode]
+    node: Optional[AbstractNode]
     role: ServiceRole = ServiceRole.NONE
 
 
 class ChangeContext(SyftBaseObject):
-    node: Optional[NewNode] = None
+    node: Optional[AbstractNode] = None
     approving_user_credentials: Optional[SyftVerifyKey]
     requesting_user_credentials: Optional[SyftVerifyKey]
 
     @staticmethod
     def from_service(context: AuthedServiceContext) -> Self:
         return ChangeContext(
             node=context.node, approving_user_credentials=context.credentials
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/credentials.py` & `syft-0.8.0b9/src/syft/node/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 # third party
 from nacl.encoding import HexEncoder
 from nacl.signing import SigningKey
 from nacl.signing import VerifyKey
 
 # relative
-from .base import SyftBaseModel
-from .serializable import serializable
+from ..serde.serializable import serializable
+from ..types.base import SyftBaseModel
 
 SIGNING_KEY_FOR = "SigningKey for"
 
 
 @serializable()
 class SyftVerifyKey(SyftBaseModel):
     verify_key: VerifyKey
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/data_subject.py` & `syft-0.8.0b9/src/syft/service/data_subject/data_subject.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from typing import Set
 from typing import Tuple
 
 # third party
 from typing_extensions import Self
 
 # relative
-from .document_store import PartitionKey
-from .response import SyftError
-from .serializable import serializable
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftObject
-from .transforms import TransformContext
-from .transforms import add_node_uid_for_key
-from .transforms import generate_id
-from .transforms import transform
-from .uid import UID
+from ...serde.serializable import serializable
+from ...store.document_store import PartitionKey
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftObject
+from ...types.transforms import TransformContext
+from ...types.transforms import add_node_uid_for_key
+from ...types.transforms import generate_id
+from ...types.transforms import transform
+from ...types.uid import UID
+from ..response import SyftError
 
 NamePartitionKey = PartitionKey(key="name", type_=str)
 
 
 @serializable()
 class DataSubject(SyftObject):
     # version
@@ -33,15 +33,15 @@
     name: str
     description: Optional[str]
     aliases: List[str] = []
 
     @property
     def members(self) -> List:
         # relative
-        from .api import APIRegistry
+        from ...client.api import APIRegistry
 
         api = APIRegistry.api_for(self.node_uid)
         if api is None:
             return SyftError(message=f"You must login to {self.node_uid}")
         members = api.services.data_subject.members_for(self.name)
         return members
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/data_subject_member.py` & `syft-0.8.0b9/src/syft/service/data_subject/data_subject_member.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # relative
-from .document_store import PartitionKey
-from .serializable import serializable
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftObject
+from ...serde.serializable import serializable
+from ...store.document_store import PartitionKey
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftObject
 
 ParentPartitionKey = PartitionKey(key="parent", type_=str)
 ChildPartitionKey = PartitionKey(key="child", type_=str)
 
 
 @serializable()
 class DataSubjectMemberRelationship(SyftObject):
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/data_subject_member_service.py` & `syft-0.8.0b9/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from typing import Optional
 from typing import Union
 
 # third party
 from result import Result
 
 # relative
-from ....telemetry import instrument
-from .context import AuthedServiceContext
-from .credentials import SyftVerifyKey
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...store.document_store import BaseUIDStoreStash
+from ...store.document_store import DocumentStore
+from ...store.document_store import PartitionSettings
+from ...store.document_store import QueryKeys
+from ...util.telemetry import instrument
+from ..context import AuthedServiceContext
+from ..response import SyftError
+from ..response import SyftSuccess
+from ..service import AbstractService
+from ..service import SERVICE_TO_TYPES
+from ..service import TYPE_TO_SERVICE
 from .data_subject_member import ChildPartitionKey
 from .data_subject_member import DataSubjectMemberRelationship
 from .data_subject_member import ParentPartitionKey
-from .document_store import BaseUIDStoreStash
-from .document_store import DocumentStore
-from .document_store import PartitionSettings
-from .document_store import QueryKeys
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .service import AbstractService
-from .service import SERVICE_TO_TYPES
-from .service import TYPE_TO_SERVICE
 
 
 @instrument
 @serializable()
 class DataSubjectMemberStash(BaseUIDStoreStash):
     object_type = DataSubjectMemberRelationship
     settings: PartitionSettings = PartitionSettings(
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/data_subject_service.py` & `syft-0.8.0b9/src/syft/service/data_subject/data_subject_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 from typing import Optional
 from typing import Union
 
 # third party
 from result import Result
 
 # relative
-from ....telemetry import instrument
-from .context import AuthedServiceContext
-from .credentials import SyftVerifyKey
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...store.document_store import BaseUIDStoreStash
+from ...store.document_store import DocumentStore
+from ...store.document_store import PartitionSettings
+from ...store.document_store import QueryKeys
+from ...util.telemetry import instrument
+from ..context import AuthedServiceContext
+from ..response import SyftError
+from ..response import SyftSuccess
+from ..service import AbstractService
+from ..service import SERVICE_TO_TYPES
+from ..service import TYPE_TO_SERVICE
+from ..service import service_method
 from .data_subject import DataSubject
 from .data_subject import DataSubjectCreate
 from .data_subject import NamePartitionKey
 from .data_subject_member_service import DataSubjectMemberService
-from .document_store import BaseUIDStoreStash
-from .document_store import DocumentStore
-from .document_store import PartitionSettings
-from .document_store import QueryKeys
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .service import AbstractService
-from .service import SERVICE_TO_TYPES
-from .service import TYPE_TO_SERVICE
-from .service import service_method
 
 
 @instrument
 @serializable()
 class DataSubjectStash(BaseUIDStoreStash):
     object_type = DataSubject
     settings: PartitionSettings = PartitionSettings(
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/dataset.py` & `syft-0.8.0b9/src/syft/service/dataset/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,30 +12,29 @@
 
 # third party
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
-# from .action_object import ActionObjectPointer
-from .data_subject import DataSubject
-from .data_subject import DataSubjectCreate
-from .data_subject_service import DataSubjectService
-from .document_store import PartitionKey
-from .response import SyftError
-from .response import SyftException
-from .response import SyftSuccess
-from .serializable import serializable
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftObject
-from .transforms import TransformContext
-from .transforms import generate_id
-from .transforms import transform
-from .transforms import validate_url
-from .uid import UID
+from ...serde.serializable import serializable
+from ...store.document_store import PartitionKey
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftObject
+from ...types.transforms import TransformContext
+from ...types.transforms import generate_id
+from ...types.transforms import transform
+from ...types.transforms import validate_url
+from ...types.uid import UID
+from ..data_subject.data_subject import DataSubject
+from ..data_subject.data_subject import DataSubjectCreate
+from ..data_subject.data_subject_service import DataSubjectService
+from ..response import SyftError
+from ..response import SyftException
+from ..response import SyftSuccess
 
 
 @serializable()
 class TupleDict(OrderedDict):
     def __getitem__(self, key: Union[str, int]) -> Any:
         if isinstance(key, int):
             return list(self.values())[key]
@@ -90,23 +89,23 @@
         for contributor in self.contributors:
             _repr_str += f"\t{contributor.name}: {contributor.email}\n"
         return "```python\n" + _repr_str + "\n```"
 
     @property
     def mock(self) -> Any:
         # relative
-        from .api import APIRegistry
+        from ...client.api import APIRegistry
 
         api = APIRegistry.api_for(node_uid=self.node_uid)
         return api.services.action.get_pointer(self.action_id)
 
     @property
     def data(self) -> Any:
         # relative
-        from .api import APIRegistry
+        from ...client.api import APIRegistry
 
         api = APIRegistry.api_for(node_uid=self.node_uid)
         return api.services.action.get(self.action_id)
 
 
 @serializable()
 class CreateAsset(SyftObject):
@@ -234,15 +233,15 @@
         if self.description:
             _repr_str += f"Description: {self.description}\n"
         return "```python\n" + _repr_str + "\n```"
 
     @property
     def client(self) -> Optional[Any]:
         # relative
-        from .client import SyftClientSessionCache
+        from ...client.client import SyftClientSessionCache
 
         client = SyftClientSessionCache.get_client_for_node_uid(self.node_uid)
         if client is None:
             return SyftError(
                 message=f"No clients for {self.node_uid} in memory. Please login with sy.login"
             )
         return client
@@ -305,15 +304,15 @@
         return Ok(SyftSuccess(message="Dataset is Valid"))
 
 
 def create_and_store_twin(context: TransformContext) -> TransformContext:
     action_id = context.output["action_id"]
     if action_id is None:
         # relative
-        from .twin_object import TwinObject
+        from ...types.twin_object import TwinObject
 
         private_obj = context.output.pop("data", None)
         mock_obj = context.output.pop("mock", None)
         if private_obj is None and mock_obj is None:
             raise Exception("No data and no action_id means this asset has no data")
 
         twin = TwinObject(
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/dataset_service.py` & `syft-0.8.0b9/src/syft/service/dataset/dataset_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # stdlib
 from typing import List
 from typing import Union
 
 # relative
-from ....telemetry import instrument
-from .action_permissions import ActionObjectPermission
-from .action_permissions import ActionPermission
-from .context import AuthedServiceContext
+from ...serde.serializable import serializable
+from ...store.document_store import DocumentStore
+from ...types.uid import UID
+from ...util.telemetry import instrument
+from ..action.action_permissions import ActionObjectPermission
+from ..action.action_permissions import ActionPermission
+from ..context import AuthedServiceContext
+from ..response import SyftError
+from ..response import SyftSuccess
+from ..service import AbstractService
+from ..service import SERVICE_TO_TYPES
+from ..service import TYPE_TO_SERVICE
+from ..service import service_method
+from ..user.user_roles import DATA_OWNER_ROLE_LEVEL
+from ..user.user_roles import GUEST_ROLE_LEVEL
 from .dataset import Asset
 from .dataset import CreateDataset
 from .dataset import Dataset
 from .dataset_stash import DatasetStash
-from .document_store import DocumentStore
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .service import AbstractService
-from .service import SERVICE_TO_TYPES
-from .service import TYPE_TO_SERVICE
-from .service import service_method
-from .uid import UID
-from .user_roles import DATA_OWNER_ROLE_LEVEL
-from .user_roles import GUEST_ROLE_LEVEL
 
 
 @instrument
 @serializable()
 class DatasetService(AbstractService):
     store: DocumentStore
     stash: DatasetStash
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/dataset_stash.py` & `syft-0.8.0b9/src/syft/service/dataset/dataset_stash.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from typing import List
 from typing import Optional
 
 # third party
 from result import Result
 
 # relative
-from ....telemetry import instrument
-from .credentials import SyftVerifyKey
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...store.document_store import BaseUIDStoreStash
+from ...store.document_store import DocumentStore
+from ...store.document_store import PartitionKey
+from ...store.document_store import PartitionSettings
+from ...store.document_store import QueryKeys
+from ...types.uid import UID
+from ...util.telemetry import instrument
 from .dataset import Dataset
 from .dataset import DatasetUpdate
-from .document_store import BaseUIDStoreStash
-from .document_store import DocumentStore
-from .document_store import PartitionKey
-from .document_store import PartitionSettings
-from .document_store import QueryKeys
-from .serializable import serializable
-from .uid import UID
 
 NamePartitionKey = PartitionKey(key="name", type_=str)
 ActionIDsPartitionKey = PartitionKey(key="action_ids", type_=List[UID])
 
 
 @instrument
 @serializable()
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/datetime.py` & `syft-0.8.0b9/src/syft/types/datetime.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # stdlib
 from datetime import datetime
 
 # third party
 from typing_extensions import Self
 
 # relative
-from .serializable import serializable
+from ..serde.serializable import serializable
 from .syft_object import SYFT_OBJECT_VERSION_1
 from .syft_object import SyftObject
 
 
 @serializable()
 class DateTime(SyftObject):
     __canonical_name__ = "DateTime"
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/decorators.py` & `syft-0.8.0b9/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/core/node/new/deserialize.py` & `syft-0.8.0b9/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/core/node/new/dict_document_store.py` & `syft-0.8.0b9/src/syft/store/dict_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 # stdlib
 from typing import Any
 from typing import Optional
 from typing import Type
 
 # relative
-from .credentials import SyftVerifyKey
+from ..node.credentials import SyftVerifyKey
+from ..serde.serializable import serializable
 from .document_store import DocumentStore
 from .document_store import StoreConfig
 from .kv_document_store import KeyValueBackingStore
 from .kv_document_store import KeyValueStorePartition
 from .locks import LockingConfig
 from .locks import ThreadingLockingConfig
-from .serializable import serializable
 
 
 @serializable()
 class DictBackingStore(dict, KeyValueBackingStore):
     """Dictionary-based Store core logic"""
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/document_store.py` & `syft-0.8.0b9/src/syft/store/document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 from pydantic import BaseModel
 from result import Err
 from result import Ok
 from result import Result
 from typeguard import check_type
 
 # relative
-from ....telemetry import instrument
-from .action_permissions import ActionObjectPermission
-from .base import SyftBaseModel
-from .credentials import SyftSigningKey
-from .credentials import SyftVerifyKey
+from ..node.credentials import SyftSigningKey
+from ..node.credentials import SyftVerifyKey
+from ..serde.serializable import serializable
+from ..service.action.action_permissions import ActionObjectPermission
+from ..service.response import SyftSuccess
+from ..types.base import SyftBaseModel
+from ..types.syft_object import SYFT_OBJECT_VERSION_1
+from ..types.syft_object import SyftBaseObject
+from ..types.syft_object import SyftObject
+from ..types.uid import UID
+from ..util.telemetry import instrument
 from .locks import LockingConfig
 from .locks import NoLockingConfig
 from .locks import SyftLock
-from .response import SyftSuccess
-from .serializable import serializable
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftBaseObject
-from .syft_object import SyftObject
-from .uid import UID
 
 
 @serializable()
 class BasePartitionSettings(SyftBaseModel):
     """Basic Partition Settings
 
     Parameters:
@@ -379,21 +379,19 @@
             ignore_duplicates=ignore_duplicates,
         )
 
     def get(
         self,
         credentials: SyftVerifyKey,
         uid: UID,
-        skip_permissions: bool = False,
     ) -> Result[SyftObject, str]:
         return self._thread_safe_cbk(
             self._get,
             uid=uid,
             credentials=credentials,
-            skip_permissions=skip_permissions,
         )
 
     def find_index_or_search_keys(
         self, credentials: SyftVerifyKey, index_qks: QueryKeys, search_qks: QueryKeys
     ) -> Result[List[SyftObject], str]:
         return self._thread_safe_cbk(
             self._find_index_or_search_keys,
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/grid_url.py` & `syft-0.8.0b9/src/syft/types/grid_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from typing import Union
 from urllib.parse import urlparse
 
 # third party
 import requests
 
 # relative
-from .serializable import serializable
-from .util import verify_tls
+from ..serde.serializable import serializable
+from ..util.util import verify_tls
 
 
 @serializable(attrs=["protocol", "host_or_ip", "port", "path", "query"])
 class GridURL:
     @staticmethod
     def from_url(url: Union[str, GridURL]) -> GridURL:
         if isinstance(url, GridURL):
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/kv_document_store.py` & `syft-0.8.0b9/src/syft/store/kv_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 # third party
 from result import Err
 from result import Ok
 from result import Result
 from typing_extensions import Self
 
 # relative
-from .action_permissions import ActionObjectEXECUTE
-from .action_permissions import ActionObjectOWNER
-from .action_permissions import ActionObjectPermission
-from .action_permissions import ActionObjectREAD
-from .action_permissions import ActionObjectWRITE
-from .action_permissions import ActionPermission
-from .credentials import SyftVerifyKey
+from ..node.credentials import SyftVerifyKey
+from ..serde.serializable import serializable
+from ..service.action.action_permissions import ActionObjectEXECUTE
+from ..service.action.action_permissions import ActionObjectOWNER
+from ..service.action.action_permissions import ActionObjectPermission
+from ..service.action.action_permissions import ActionObjectREAD
+from ..service.action.action_permissions import ActionObjectWRITE
+from ..service.action.action_permissions import ActionPermission
+from ..service.response import SyftSuccess
+from ..types.syft_object import SyftObject
+from ..types.uid import UID
 from .document_store import BaseStash
 from .document_store import PartitionSettings
 from .document_store import QueryKey
 from .document_store import QueryKeys
 from .document_store import StoreConfig
 from .document_store import StorePartition
-from .response import SyftSuccess
-from .serializable import serializable
-from .syft_object import SyftObject
-from .uid import UID
 
 
 @serializable()
 class UniqueKeyCheck(Enum):
     EMPTY = 0
     MATCHES = 1
     ERROR = 2
@@ -138,26 +138,24 @@
             return Err(str(e))
 
         return Ok()
 
     def __len__(self) -> int:
         return len(self.data)
 
-    def _get(
-        self, uid: UID, credentials: SyftVerifyKey, skip_permission: bool = False
-    ) -> Result[SyftObject, str]:
+    def _get(self, uid: UID, credentials: SyftVerifyKey) -> Result[SyftObject, str]:
         # relative
-        from .action_store import ActionObjectREAD
+        from ..service.action.action_store import ActionObjectREAD
 
         # TODO 🟣 Temporarily added skip permission argument for enclave
         # until permissions are fully integrated
         # if you get something you need READ permission
         read_permission = ActionObjectREAD(uid=uid, credentials=credentials)
         # if True:
-        if skip_permission or self.has_permission(read_permission):
+        if self.has_permission(read_permission):
             syft_object = self.data[uid]
             return Ok(syft_object)
         return Err(f"Permission: {read_permission} denied")
 
     # Potentially thread-unsafe methods.
     # CAUTION:
     #       * Don't use self.lock here.
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/linked_obj.py` & `syft-0.8.0b9/src/syft/store/linked_obj.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from typing import Type
 from typing import Union
 
 # third party
 from typing_extensions import Self
 
 # relative
-from .context import AuthedServiceContext
-from .context import ChangeContext
-from .context import NodeServiceContext
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftObject
-from .uid import UID
+from ..serde.serializable import serializable
+from ..service.context import AuthedServiceContext
+from ..service.context import ChangeContext
+from ..service.context import NodeServiceContext
+from ..service.response import SyftError
+from ..service.response import SyftSuccess
+from ..types.syft_object import SYFT_OBJECT_VERSION_1
+from ..types.syft_object import SyftObject
+from ..types.uid import UID
 
 
 @serializable()
 class LinkedObject(SyftObject):
     __canonical_name__ = "LinkedObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
@@ -31,15 +31,15 @@
 
     def __str__(self) -> str:
         return f"<{self.object_type}: {self.object_uid}@<Node: {self.node_uid}>"
 
     @property
     def resolve(self) -> SyftObject:
         # relative
-        from .api import APIRegistry
+        from ..client.api import APIRegistry
 
         api = APIRegistry.api_for(node_uid=self.node_uid)
         return api.services.messages.resolve_object(self)
 
     def resolve_with_context(self, context: NodeServiceContext) -> Any:
         return context.node.get_service(self.service_type).resolve_link(
             context=context, linked_obj=self
@@ -65,17 +65,17 @@
         cls,
         obj: SyftObject,
         service_type: Optional[Type[Any]] = None,
         node_uid: Optional[UID] = None,
     ) -> Self:
         if service_type is None:
             # relative
-            from .action_object import ActionObject
-            from .action_service import ActionService
-            from .service import TYPE_TO_SERVICE
+            from ..service.action.action_object import ActionObject
+            from ..service.action.action_service import ActionService
+            from ..service.service import TYPE_TO_SERVICE
 
             if isinstance(obj, ActionObject):
                 service_type = ActionService
             else:
                 service_type = TYPE_TO_SERVICE[type(obj)]
 
         object_uid = getattr(obj, "id", None)
@@ -100,15 +100,15 @@
         obj: SyftObject,
         context: NodeServiceContext,
         object_uid: Optional[UID] = None,
         service_type: Optional[Type[Any]] = None,
     ) -> Self:
         if service_type is None:
             # relative
-            from .service import TYPE_TO_SERVICE
+            from ..service.service import TYPE_TO_SERVICE
 
             service_type = TYPE_TO_SERVICE[type(obj)]
 
         if object_uid is None and hasattr(obj, "id"):
             object_uid = getattr(obj, "id", None)
         if object_uid is None:
             raise Exception(f"{cls} Requires an object UID")
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/locks.py` & `syft-0.8.0b9/src/syft/store/locks.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from pydantic import BaseModel
 import redis
 from sherlock.lock import BaseLock
 from sherlock.lock import FileLock
 from sherlock.lock import RedisLock
 
 # relative
-from ....logger import debug
-from .serializable import serializable
+from ..serde.serializable import serializable
+from ..util.logger import debug
 
 
 @serializable()
 class LockingConfig(BaseModel):
     """
     Locking config
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/message_service.py` & `syft-0.8.0b9/src/syft/service/message/message_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # stdlib
 from typing import List
 from typing import Union
 
 # relative
-from ....telemetry import instrument
-from .context import AuthedServiceContext
-from .document_store import DocumentStore
+from ...serde.serializable import serializable
+from ...store.document_store import DocumentStore
+from ...types.uid import UID
+from ...util.telemetry import instrument
+from ..context import AuthedServiceContext
+from ..response import SyftError
+from ..response import SyftSuccess
+from ..service import AbstractService
+from ..service import SERVICE_TO_TYPES
+from ..service import TYPE_TO_SERVICE
+from ..service import service_method
 from .message_stash import MessageStash
 from .messages import CreateMessage
 from .messages import LinkedObject
 from .messages import Message
 from .messages import MessageStatus
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .service import AbstractService
-from .service import SERVICE_TO_TYPES
-from .service import TYPE_TO_SERVICE
-from .service import service_method
-from .uid import UID
 
 
 @instrument
 @serializable()
 class MessageService(AbstractService):
     store: DocumentStore
     stash: MessageStash
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/message_stash.py` & `syft-0.8.0b9/src/syft/service/message/message_stash.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 # third party
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
-from ....telemetry import instrument
-from .credentials import SyftVerifyKey
-from .document_store import BaseUIDStoreStash
-from .document_store import PartitionKey
-from .document_store import PartitionSettings
-from .document_store import QueryKeys
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...store.document_store import BaseUIDStoreStash
+from ...store.document_store import PartitionKey
+from ...store.document_store import PartitionSettings
+from ...store.document_store import QueryKeys
+from ...types.uid import UID
+from ...util.telemetry import instrument
 from .messages import Message
 from .messages import MessageStatus
-from .serializable import serializable
-from .uid import UID
 
 FromUserVerifyKeyPartitionKey = PartitionKey(
     key="from_user_verify_key", type_=SyftVerifyKey
 )
 ToUserVerifyKeyPartitionKey = PartitionKey(
     key="to_user_verify_key", type_=SyftVerifyKey
 )
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/messages.py` & `syft-0.8.0b9/src/syft/service/message/messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # stdlib
 from enum import Enum
 from typing import Optional
 
 # relative
-from .credentials import SyftVerifyKey
-from .linked_obj import LinkedObject
-from .request import DateTime
-from .serializable import serializable
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftObject
-from .transforms import TransformContext
-from .transforms import add_credentials_for_key
-from .transforms import add_node_uid_for_key
-from .transforms import generate_id
-from .transforms import transform
-from .uid import UID
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...store.linked_obj import LinkedObject
+from ...types.datetime import DateTime
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftObject
+from ...types.transforms import TransformContext
+from ...types.transforms import add_credentials_for_key
+from ...types.transforms import add_node_uid_for_key
+from ...types.transforms import generate_id
+from ...types.transforms import transform
+from ...types.uid import UID
 
 
 @serializable()
 class MessageStatus(Enum):
     UNDELIVERED = 0
     DELIVERED = 1
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/metadata_service.py` & `syft-0.8.0b9/src/syft/service/metadata/metadata_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,39 @@
 
 # third party
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
-from .context import AuthedServiceContext
-from .document_store import DocumentStore
+from ...serde.serializable import serializable
+from ...store.document_store import DocumentStore
+from ..context import AuthedServiceContext
+from ..context import UnauthedServiceContext
+from ..response import SyftError
+from ..service import AbstractService
+from ..service import service_method
 from .metadata_stash import MetadataStash
 from .node_metadata import NodeMetadata
 from .node_metadata import NodeMetadataUpdate
-from .response import SyftError
-from .serializable import serializable
-from .service import AbstractService
-from .service import service_method
 
 
 @serializable()
 class MetadataService(AbstractService):
     store: DocumentStore
     stash: MetadataStash
 
     def __init__(self, store: DocumentStore) -> None:
         self.store = store
         self.stash = MetadataStash(store=store)
 
     @service_method(path="metadata.get", name="get")
-    def get(self, context: AuthedServiceContext) -> Result[Ok, Err]:
+    def get(self, context: UnauthedServiceContext) -> Result[Ok, Err]:
         """Get Metadata"""
-        result = self.stash.get_all(context.credentials)
+        result = self.stash.get_all(context.node.signing_key.verify_key)
         if result.is_ok():
             metadata = result.ok()
             # check if the metadata list is empty
             if len(metadata) == 0:
                 return SyftError(message="No metadata found")
             result = metadata[0]
             return Ok(result)
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/metadata_stash.py` & `syft-0.8.0b9/src/syft/service/metadata/metadata_stash.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # stdlib
 from typing import List
 
 # third party
 from result import Result
 
 # relative
-from ....telemetry import instrument
-from .credentials import SyftVerifyKey
-from .document_store import BaseUIDStoreStash
-from .document_store import DocumentStore
-from .document_store import PartitionKey
-from .document_store import PartitionSettings
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...store.document_store import BaseUIDStoreStash
+from ...store.document_store import DocumentStore
+from ...store.document_store import PartitionKey
+from ...store.document_store import PartitionSettings
+from ...types.uid import UID
+from ...util.telemetry import instrument
 from .node_metadata import NodeMetadata
-from .serializable import serializable
-from .uid import UID
 
 NamePartitionKey = PartitionKey(key="name", type_=str)
 ActionIDsPartitionKey = PartitionKey(key="action_ids", type_=List[UID])
 
 
 @instrument
 @serializable()
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/mongo_client.py` & `syft-0.8.0b9/src/syft/store/mongo_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from pymongo.errors import ConnectionFailure
 from pymongo.mongo_client import MongoClient as PyMongoClient
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
+from ..serde.serializable import serializable
 from .document_store import PartitionSettings
 from .document_store import StoreClientConfig
 from .document_store import StoreConfig
 from .mongo_codecs import SYFT_CODEC_OPTIONS
-from .serializable import serializable
 
 
 @serializable()
 class MongoStoreClientConfig(StoreClientConfig):
     """
     Paramaters:
         `hostname`: optional string
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/mongo_codecs.py` & `syft-0.8.0b9/src/syft/store/mongo_codecs.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from bson import CodecOptions
 from bson.binary import Binary
 from bson.binary import USER_DEFINED_SUBTYPE
 from bson.codec_options import TypeDecoder
 from bson.codec_options import TypeRegistry
 
 # relative
-from .deserialize import _deserialize
-from .serialize import _serialize
+from ..serde.deserialize import _deserialize
+from ..serde.serialize import _serialize
 
 
 def fallback_syft_encoder(value):
     return Binary(_serialize(value, to_bytes=True), USER_DEFINED_SUBTYPE)
 
 
 class SyftMongoBinaryDecoder(TypeDecoder):
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/mongo_document_store.py` & `syft-0.8.0b9/src/syft/store/mongo_document_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 from pymongo.collection import Collection as MongoCollection
 from pymongo.errors import DuplicateKeyError
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
-from .action_permissions import ActionObjectPermission
-from .action_permissions import ActionObjectREAD
-from .action_permissions import ActionObjectWRITE
-from .credentials import SyftVerifyKey
+from ..node.credentials import SyftVerifyKey
+from ..serde.serializable import serializable
+from ..service.action.action_permissions import ActionObjectPermission
+from ..service.action.action_permissions import ActionObjectREAD
+from ..service.action.action_permissions import ActionObjectWRITE
+from ..service.response import SyftSuccess
+from ..types.syft_object import StorableObjectType
+from ..types.syft_object import SyftObject
+from ..types.syft_object import SyftObjectRegistry
+from ..types.transforms import TransformContext
+from ..types.transforms import transform
+from ..types.transforms import transform_method
 from .document_store import DocumentStore
 from .document_store import QueryKey
 from .document_store import QueryKeys
 from .document_store import StoreConfig
 from .document_store import StorePartition
 from .locks import LockingConfig
 from .locks import NoLockingConfig
 from .mongo_client import MongoClient
 from .mongo_client import MongoStoreClientConfig
-from .response import SyftSuccess
-from .serializable import serializable
-from .syft_object import StorableObjectType
-from .syft_object import SyftObject
-from .syft_object import SyftObjectRegistry
-from .transforms import TransformContext
-from .transforms import transform
-from .transforms import transform_method
 
 
 class MongoBsonObject(StorableObjectType, dict):
     pass
 
 
 def _repr_debug_(value: Any) -> str:
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/network_service.py` & `syft-0.8.0b9/src/syft/service/network/network_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,47 +6,47 @@
 from typing import Union
 
 # third party
 from result import Result
 from typing_extensions import Self
 
 # relative
-from ....telemetry import instrument
-from ...node.new.node_metadata import NodeMetadata
-from .client import HTTPConnection
-from .client import NodeConnection
-from .client import PythonConnection
-from .client import SyftClient
-from .context import AuthedServiceContext
-from .context import NodeServiceContext
-from .credentials import SyftSigningKey
-from .credentials import SyftVerifyKey
-from .data_subject import NamePartitionKey
-from .document_store import BaseUIDStoreStash
-from .document_store import DocumentStore
-from .document_store import PartitionKey
-from .document_store import PartitionSettings
-from .document_store import QueryKeys
-from .grid_url import GridURL
-from .node import NewNode
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .service import AbstractService
-from .service import SERVICE_TO_TYPES
-from .service import TYPE_TO_SERVICE
-from .service import service_method
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftObject
-from .transforms import TransformContext
-from .transforms import keep
-from .transforms import transform
-from .transforms import transform_method
-from .uid import UID
-from .worker_settings import WorkerSettings
+from ...abstract_node import AbstractNode
+from ...client.client import HTTPConnection
+from ...client.client import NodeConnection
+from ...client.client import PythonConnection
+from ...client.client import SyftClient
+from ...node.credentials import SyftSigningKey
+from ...node.credentials import SyftVerifyKey
+from ...node.worker_settings import WorkerSettings
+from ...serde.serializable import serializable
+from ...store.document_store import BaseUIDStoreStash
+from ...store.document_store import DocumentStore
+from ...store.document_store import PartitionKey
+from ...store.document_store import PartitionSettings
+from ...store.document_store import QueryKeys
+from ...types.grid_url import GridURL
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftObject
+from ...types.transforms import TransformContext
+from ...types.transforms import keep
+from ...types.transforms import transform
+from ...types.transforms import transform_method
+from ...types.uid import UID
+from ...util.telemetry import instrument
+from ..context import AuthedServiceContext
+from ..context import NodeServiceContext
+from ..data_subject.data_subject import NamePartitionKey
+from ..metadata.node_metadata import NodeMetadata
+from ..response import SyftError
+from ..response import SyftSuccess
+from ..service import AbstractService
+from ..service import SERVICE_TO_TYPES
+from ..service import TYPE_TO_SERVICE
+from ..service import service_method
 
 VerifyKeyPartitionKey = PartitionKey(key="verify_key", type_=SyftVerifyKey)
 
 
 class NodeRoute:
     def client_with_context(self, context: NodeServiceContext) -> SyftClient:
         connection = route_to_connection(route=self, context=context)
@@ -81,30 +81,30 @@
 class PythonNodeRoute(SyftObject, NodeRoute):
     __canonical_name__ = "PythonNodeRoute"
     __version__ = SYFT_OBJECT_VERSION_1
 
     worker_settings: WorkerSettings
 
     @property
-    def node(self) -> Optional[NewNode]:
+    def node(self) -> Optional[AbstractNode]:
         # relative
-        from ..worker import Worker
+        from ...node.worker import Worker
 
         node = Worker(
             id=self.worker_settings.id,
             name=self.worker_settings.name,
             signing_key=self.worker_settings.signing_key,
             document_store_config=self.worker_settings.document_store_config,
             action_store_config=self.worker_settings.action_store_config,
             processes=1,
         )
         return node
 
     @staticmethod
-    def with_node(self, node: NewNode) -> Self:
+    def with_node(self, node: AbstractNode) -> Self:
         worker_settings = WorkerSettings.from_node(node)
         return PythonNodeRoute(id=worker_settings.id, worker_settings=worker_settings)
 
     def __hash__(self) -> int:
         return (
             hash(self.worker_settings.id)
             + hash(self.worker_settings.name)
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/node.py` & `syft-0.8.0b9/src/syft/abstract_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # stdlib
 from enum import Enum
 from typing import Callable
 from typing import Optional
 from typing import Union
 
 # relative
-from .credentials import SyftSigningKey
-from .serializable import serializable
-from .uid import UID
+from .serde.serializable import serializable
+from .types.uid import UID
 
 
 @serializable()
 class NodeType(Enum):
     DOMAIN = "domain"
     NETWORK = "network"
     ENCLAVE = "enclave"
 
 
-class NewNode:
+class AbstractNode:
     id: Optional[UID]
     name: Optional[str]
-    signing_key: Optional[SyftSigningKey]
     node_type: Optional[NodeType]
 
     def get_service(self, path_or_func: Union[str, Callable]) -> Callable:
         raise NotImplementedError
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/node_metadata.py` & `syft-0.8.0b9/src/syft/service/metadata/node_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from typing import Optional
 
 # third party
 from packaging import version
 from pydantic import BaseModel
 
 # relative
-from ..new.credentials import SyftVerifyKey
-from ..new.transforms import convert_types
-from ..new.transforms import drop
-from ..new.transforms import rename
-from .serializable import serializable
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import StorableObjectType
-from .syft_object import SyftObject
-from .transforms import transform
-from .uid import UID
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import StorableObjectType
+from ...types.syft_object import SyftObject
+from ...types.transforms import convert_types
+from ...types.transforms import drop
+from ...types.transforms import rename
+from ...types.transforms import transform
+from ...types.uid import UID
 
 
 def check_version(
     client_version: str, server_version: str, server_name: str, silent: bool = False
 ) -> bool:
     client_syft_version = version.parse(client_version)
     node_syft_version = version.parse(server_version)
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/numpy.py` & `syft-0.8.0b9/src/syft/service/action/numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from typing import ClassVar
 from typing import Type
 
 # third party
 import numpy as np
 
 # relative
+from ...serde.serializable import serializable
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from .action_object import ActionObject
 from .action_types import action_types
-from .serializable import serializable
-from .syft_object import SYFT_OBJECT_VERSION_1
 
 # @serializable(attrs=["id", "node_uid", "parent_id"])
 # class NumpyArrayObjectPointer(ActionObjectPointer):
 #     _inflix_operations = ["__add__", "__sub__", "__eq__", "__mul__"]
 #     __canonical_name__ = "NumpyArrayObjectPointer"
 #     __version__ = SYFT_OBJECT_VERSION_1
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/pandas.py` & `syft-0.8.0b9/src/syft/service/action/pandas.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from typing import Type
 
 # third party
 from pandas import DataFrame
 from pandas import Series
 
 # relative
+from ...serde.serializable import serializable
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from .action_object import ActionObject
 from .action_types import action_types
-from .serializable import serializable
-from .syft_object import SYFT_OBJECT_VERSION_1
 
 
 @serializable()
 class PandasDataFrameObject(ActionObject):
     __canonical_name__ = "PandasDataframeObject"
     __version__ = SYFT_OBJECT_VERSION_1
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/policy.py` & `syft-0.8.0b9/src/syft/service/policy/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,36 +20,36 @@
 from typing import Union
 
 # third party
 from RestrictedPython import compile_restricted
 from result import Ok
 
 # relative
-from ....util import is_interpreter_jupyter
-from .action_object import ActionObject
-from .api import NodeView
-from .code_parse import GlobalsVisitor
-from .context import AuthedServiceContext
-from .context import NodeServiceContext
-from .credentials import SyftVerifyKey
-from .dataset import Asset
-from .datetime import DateTime
-from .document_store import PartitionKey
-from .node import NodeType
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftObject
-from .transforms import TransformContext
-from .transforms import generate_id
-from .transforms import transform
-from .twin_object import TwinObject
-from .uid import UID
-from .unparse import unparse
+from ...abstract_node import NodeType
+from ...client.api import NodeView
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...store.document_store import PartitionKey
+from ...types.datetime import DateTime
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftObject
+from ...types.transforms import TransformContext
+from ...types.transforms import generate_id
+from ...types.transforms import transform
+from ...types.twin_object import TwinObject
+from ...types.uid import UID
+from ...util.util import is_interpreter_jupyter
+from ..action.action_object import ActionObject
+from ..code.code_parse import GlobalsVisitor
+from ..code.unparse import unparse
+from ..context import AuthedServiceContext
+from ..context import NodeServiceContext
+from ..dataset.dataset import Asset
+from ..response import SyftError
+from ..response import SyftSuccess
 
 PolicyUserVerifyKeyPartitionKey = PartitionKey(
     key="user_verify_key", type_=SyftVerifyKey
 )
 PyCodeObject = Any
 
 
@@ -124,18 +124,18 @@
     SUBMITTED = "submitted"
     DENIED = "denied"
     APPROVED = "approved"
 
 
 def partition_by_node(kwargs: Dict[str, Any]) -> Dict[str, UID]:
     # relative
-    from .action_object import ActionObject
-    from .api import APIRegistry
-    from .api import NodeView
-    from .twin_object import TwinObject
+    from ...client.api import APIRegistry
+    from ...client.api import NodeView
+    from ...types.twin_object import TwinObject
+    from ..action.action_object import ActionObject
 
     # fetches the all the current api's connected
     api_list = APIRegistry.get_all_api()
     output_kwargs = {}
     for k, v in kwargs.items():
         uid = v
         if isinstance(v, ActionObject):
@@ -189,15 +189,15 @@
         return self.init_kwargs
 
 
 def retrieve_from_db(
     code_item_id: UID, allowed_inputs: Dict[str, UID], context: AuthedServiceContext
 ) -> Dict:
     # relative
-    from .action_service import TwinMode
+    from ...service.action.action_service import TwinMode
 
     action_service = context.node.get_service("actionservice")
     code_inputs = {}
 
     if context.node.node_type == NodeType.DOMAIN:
         for var_name, arg_id in allowed_inputs.items():
             kwarg_value = action_service.get(
@@ -206,17 +206,15 @@
             if kwarg_value.is_err():
                 return kwarg_value
             code_inputs[var_name] = kwarg_value.ok()
 
     elif context.node.node_type == NodeType.ENCLAVE:
         # TODO 🟣 Temporarily added skip permission arguments for enclave
         # until permissions are fully integrated
-        dict_object = action_service.get(
-            context=context, uid=code_item_id, skip_permission=True
-        )
+        dict_object = action_service.get(context=context, uid=code_item_id)
         if dict_object.is_err():
             return dict_object
         for value in dict_object.ok().base_dict.values():
             code_inputs.update(value)
 
     else:
         raise Exception(
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/policy_service.py` & `syft-0.8.0b9/src/syft/service/policy/policy_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # stdlib
 from typing import List
 from typing import Union
 
 # relative
-from .context import AuthedServiceContext
-from .document_store import DocumentStore
+from ...serde.serializable import serializable
+from ...store.document_store import DocumentStore
+from ...types.uid import UID
+from ..context import AuthedServiceContext
+from ..response import SyftError
+from ..response import SyftSuccess
+from ..service import AbstractService
+from ..service import TYPE_TO_SERVICE
+from ..service import service_method
 from .policy import SubmitUserPolicy
 from .policy import UserPolicy
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .service import AbstractService
-from .service import TYPE_TO_SERVICE
-from .service import service_method
-from .uid import UID
 from .user_policy_stash import UserPolicyStash
 
 
 @serializable()
 class PolicyService(AbstractService):
     store: DocumentStore
     stash: UserPolicyStash
@@ -26,36 +26,36 @@
         self.store = store
         self.stash = UserPolicyStash(store=store)
 
     @service_method(path="policy.get_all", name="get_all")
     def get_all_user_policy(
         self, context: AuthedServiceContext
     ) -> Union[List[UserPolicy], SyftError]:
-        result = self.stash.get_all()
+        result = self.stash.get_all(context.credentials)
         if result.is_ok():
             return result.ok()
         return SyftError(message=result.err())
 
     @service_method(path="policy.add", name="add")
     def add_user_policy(
         self,
         context: AuthedServiceContext,
         policy_code: Union[SubmitUserPolicy, UserPolicy],
     ) -> Union[SyftSuccess, SyftError]:
         if isinstance(policy_code, SubmitUserPolicy):
             policy_code = policy_code.to(UserPolicy, context=context)
-        result = self.stash.set(policy_code)
+        result = self.stash.set(context.credentials, policy_code)
         if result.is_err():
             return SyftError(message=str(result.err()))
         return SyftSuccess(message="Policy Code Submitted")
 
     @service_method(path="policy.get_by_uid", name="get_by_uid")
     def get_policy_by_uid(
         self, context: AuthedServiceContext, uid: UID
     ) -> Union[SyftSuccess, SyftError]:
-        result = self.stash.get_by_uid(uid=uid)
+        result = self.stash.get_by_uid(context.credentials, uid=uid)
         if result.is_ok():
             return result.ok()
         return SyftError(message=result.err())
 
 
 TYPE_TO_SERVICE[UserPolicy] = UserPolicy
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/project.py` & `syft-0.8.0b9/src/syft/service/project/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 from typing import Optional
 from typing import Type
 
 # third party
 from result import OkErr
 
 # relative
-from .credentials import SyftVerifyKey
-from .linked_obj import LinkedObject
-from .request import EnumMutation
-from .request import Request
-from .request import SubmitRequest
-from .request import UserCodeStatusChange
-from .request_service import RequestService
-from .response import SyftError
-from .serializable import serializable
-from .service import TYPE_TO_SERVICE
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftObject
-from .transforms import TransformContext
-from .transforms import generate_id
-from .transforms import transform
-from .uid import UID
-from .user_code import UserCode
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...store.linked_obj import LinkedObject
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftObject
+from ...types.transforms import TransformContext
+from ...types.transforms import generate_id
+from ...types.transforms import transform
+from ...types.uid import UID
+from ..code.user_code import UserCode
+from ..request.request import EnumMutation
+from ..request.request import Request
+from ..request.request import SubmitRequest
+from ..request.request import UserCodeStatusChange
+from ..request.request_service import RequestService
+from ..response import SyftError
+from ..service import TYPE_TO_SERVICE
 
 
 @serializable()
 class Project(SyftObject):
     __canonical_name__ = "Project"
     __version__ = SYFT_OBJECT_VERSION_1
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/project_service.py` & `syft-0.8.0b9/src/syft/service/project/project_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 from typing import Union
 
 # third party
 from result import Err
 from result import Ok
 
 # relative
-from ....telemetry import instrument
-from .context import AuthedServiceContext
-from .document_store import DocumentStore
-from .linked_obj import LinkedObject
-from .message_service import CreateMessage
-from .message_service import Message
-from .message_service import MessageService
+from ...serde.serializable import serializable
+from ...store.document_store import DocumentStore
+from ...store.linked_obj import LinkedObject
+from ...util.telemetry import instrument
+from ..context import AuthedServiceContext
+from ..message.message_service import CreateMessage
+from ..message.message_service import Message
+from ..message.message_service import MessageService
+from ..response import SyftError
+from ..response import SyftSuccess
+from ..service import AbstractService
+from ..service import SERVICE_TO_TYPES
+from ..service import TYPE_TO_SERVICE
+from ..service import service_method
+from ..user.user_roles import GUEST_ROLE_LEVEL
+from ..user.user_service import UserService
 from .project import Project
 from .project import ProjectSubmit
 from .project_stash import ProjectStash
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .service import AbstractService
-from .service import SERVICE_TO_TYPES
-from .service import TYPE_TO_SERVICE
-from .service import service_method
-from .user_roles import GUEST_ROLE_LEVEL
-from .user_service import UserService
 
 
 @instrument
 @serializable()
 class ProjectService(AbstractService):
     store: DocumentStore
     stash: ProjectStash
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/project_stash.py` & `syft-0.8.0b9/src/syft/service/request/request_stash.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 # stdlib
 from typing import List
 
 # third party
 from result import Result
 
 # relative
-from ....telemetry import instrument
-from .credentials import SyftVerifyKey
-from .document_store import BaseUIDStoreStash
-from .document_store import PartitionKey
-from .document_store import PartitionSettings
-from .document_store import QueryKeys
-from .project import Project
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...store.document_store import BaseUIDStoreStash
+from ...store.document_store import PartitionKey
+from ...store.document_store import PartitionSettings
+from ...store.document_store import QueryKeys
+from ...util.telemetry import instrument
 from .request import Request
-from .response import SyftError
-from .serializable import serializable
+from .request import RequestStatus
 
-ProjectUserVerifyKeyPartitionKey = PartitionKey(
-    key="user_verify_key", type_=SyftVerifyKey
+RequestingUserVerifyKeyPartitionKey = PartitionKey(
+    key="requesting_user_verify_key", type_=SyftVerifyKey
 )
+StatusPartitionKey = PartitionKey(key="status", type_=RequestStatus)
 
 
 @instrument
 @serializable()
-class ProjectStash(BaseUIDStoreStash):
-    object_type = Project
+class RequestStash(BaseUIDStoreStash):
+    object_type = Request
     settings: PartitionSettings = PartitionSettings(
-        name=Project.__canonical_name__, object_type=Project
+        name=Request.__canonical_name__, object_type=Request
     )
 
     def get_all_for_verify_key(
-        self, credentials: SyftVerifyKey, verify_key: ProjectUserVerifyKeyPartitionKey
-    ) -> Result[List[Request], SyftError]:
+        self,
+        credentials: SyftVerifyKey,
+        verify_key: SyftVerifyKey,
+    ) -> Result[List[Request], str]:
         if isinstance(verify_key, str):
             verify_key = SyftVerifyKey.from_string(verify_key)
-        qks = QueryKeys(qks=[ProjectUserVerifyKeyPartitionKey.with_obj(verify_key)])
+        qks = QueryKeys(qks=[RequestingUserVerifyKeyPartitionKey.with_obj(verify_key)])
+        return self.query_all(credentials=credentials, qks=qks)
+
+    def get_all_for_status(
+        self, credentials: SyftVerifyKey, status: RequestStatus
+    ) -> Result[List[Request], str]:
+        qks = QueryKeys(qks=[StatusPartitionKey.with_obj(status)])
         return self.query_all(credentials=credentials, qks=qks)
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/queue_stash.py` & `syft-0.8.0b9/src/syft/service/queue/queue_stash.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 from typing import Union
 
 # third party
 from result import Ok
 from result import Result
 
 # relative
-from ....telemetry import instrument
-from .action_permissions import ActionObjectPermission
-from .api import APIRegistry
-from .api import SyftAPICall
-from .credentials import SyftVerifyKey
-from .document_store import BaseStash
-from .document_store import DocumentStore
-from .document_store import PartitionSettings
-from .document_store import QueryKeys
-from .document_store import UIDPartitionKey
-from .response import SyftError
-from .response import SyftNotReady
-from .response import SyftSuccess
-from .serializable import serializable
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftObject
-from .uid import UID
+from ...client.api import APIRegistry
+from ...client.api import SyftAPICall
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...store.document_store import BaseStash
+from ...store.document_store import DocumentStore
+from ...store.document_store import PartitionSettings
+from ...store.document_store import QueryKeys
+from ...store.document_store import UIDPartitionKey
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftObject
+from ...types.uid import UID
+from ...util.telemetry import instrument
+from ..action.action_permissions import ActionObjectPermission
+from ..response import SyftError
+from ..response import SyftNotReady
+from ..response import SyftSuccess
 
 
 @serializable()
 class QueueItem(SyftObject):
     __canonical_name__ = "QueueItem"
     __version__ = SYFT_OBJECT_VERSION_1
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/recursive.py` & `syft-0.8.0b9/src/syft/serde/recursive.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,50 +3,51 @@
 import sys
 import threading
 import types
 from typing import Any
 from typing import Callable
 from typing import List
 from typing import Optional
+from typing import Set
 from typing import Type
 from typing import Union
 
 # third party
 from capnp.lib.capnp import _DynamicStructBuilder
 from pydantic import BaseModel
 
 # syft absolute
 import syft as sy
 
 # relative
-from ....util import get_fully_qualified_name
-from ....util import index_syft_by_module_name
+from ..util.util import get_fully_qualified_name
+from ..util.util import index_syft_by_module_name
 from .capnp import get_capnp_schema
 
 TYPE_BANK = {}
 
 recursive_scheme = get_capnp_schema("recursive_serde.capnp").RecursiveSerde  # type: ignore
 
 
 def thread_ident() -> int:
-    return threading.current_thread().ident
+    return int(threading.current_thread().ident)
 
 
 def recursive_serde_register(
     cls: Union[object, type],
     serialize: Optional[Callable] = None,
     deserialize: Optional[Callable] = None,
     serialize_attrs: Optional[List] = None,
     exclude_attrs: Optional[List] = None,
     inherit_attrs: Optional[bool] = True,
     inheritable_attrs: Optional[bool] = True,
 ) -> None:
     pydantic_fields = None
     base_attrs = None
-    attribute_list = set()
+    attribute_list: Set[str] = set()
 
     cls = type(cls) if not isinstance(cls, type) else cls
     fqn = f"{cls.__module__}.{cls.__name__}"
 
     nonrecursive = bool(serialize and deserialize)
     _serialize = serialize if nonrecursive else rs_object2proto
     _deserialize = deserialize if nonrecursive else rs_proto2object
@@ -78,23 +79,23 @@
         attribute_list.update(["value"])
 
     if inheritable_attrs and attribute_list and not is_pydantic:
         # only set __syft_serializable__ for non-pydantic classes because
         # pydantic objects inherit by default
         setattr(cls, "__syft_serializable__", attribute_list)
 
-    attribute_list = list(attribute_list) if attribute_list else None
+    attributes = set(list(attribute_list)) if attribute_list else None
     serde_overrides = getattr(cls, "__serde_overrides__", {})
 
     # without fqn duplicate class names overwrite
     TYPE_BANK[fqn] = (
         nonrecursive,
         _serialize,
         _deserialize,
-        attribute_list,
+        attributes,
         serde_overrides,
         cls,
     )
 
 
 def chunk_bytes(
     data: bytes, field_name: Union[str, int], builder: _DynamicStructBuilder
@@ -197,15 +198,15 @@
             class_type = index_syft_by_module_name(proto.fullyQualifiedName)  # type: ignore
         except Exception:  # nosec
             try:
                 class_type = getattr(sys.modules[".".join(module_parts)], klass)
             except Exception:  # nosec
                 if "syft.user" in proto.fullyQualifiedName:
                     # relative
-                    from ..worker import CODE_RELOADER
+                    from ..node.node import CODE_RELOADER
 
                     for _, load_user_code in CODE_RELOADER.items():
                         load_user_code()
                 try:
                     class_type = getattr(sys.modules[".".join(module_parts)], klass)
                 except Exception:  # nosec
                     pass
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/recursive_primitives.py` & `syft-0.8.0b9/src/syft/serde/recursive_primitives.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from enum import Enum
 from enum import EnumMeta
 import functools
 import sys
 from types import MappingProxyType
 from typing import Any
 from typing import Collection
+from typing import Dict
 from typing import List
 from typing import Mapping
 from typing import Optional
 from typing import TypeVar
 from typing import Union
 from typing import _GenericAlias
 from typing import _SpecialForm
@@ -119,15 +120,15 @@
 def deserialize_defaultdict(blob: bytes) -> Mapping:
     # relative
     from .deserialize import _deserialize
 
     df_tuple = _deserialize(blob, from_bytes=True)
     df_type_bytes, df_kv_bytes = df_tuple[0], df_tuple[1]
     df_type = _deserialize(df_type_bytes, from_bytes=True)
-    mapping = defaultdict(df_type)
+    mapping: Dict = defaultdict(df_type)
 
     pairs = get_deserialized_kv_pairs(blob=df_kv_bytes)
     mapping.update(pairs)
 
     return mapping
 
 
@@ -144,15 +145,15 @@
 
     enum_value = _deserialize(enum_buf, from_bytes=True)
     return enum_type(enum_value)
 
 
 def serialize_type(serialized_type: type) -> bytes:
     # relative
-    from .util import full_name_with_qualname
+    from ..util.util import full_name_with_qualname
 
     fqn = full_name_with_qualname(klass=serialized_type)
     module_parts = fqn.split(".")
     return ".".join(module_parts).encode()
 
 
 def deserialize_type(type_blob: bytes) -> type:
@@ -264,16 +265,16 @@
     serialize=serialize_kv,
     deserialize=functools.partial(deserialize_kv, MappingProxyType),
 )
 
 
 def serialize_generic_alias(serialized_type: _GenericAlias) -> bytes:
     # relative
+    from ..util.util import full_name_with_name
     from .serialize import _serialize
-    from .util import full_name_with_name
 
     fqn = full_name_with_name(klass=serialized_type)
     module_parts = fqn.split(".")
 
     obj_dict = {
         "path": ".".join(module_parts),
         "__origin__": serialized_type.__origin__,
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/request.py` & `syft-0.8.0b9/src/syft/service/request/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,38 +12,38 @@
 # third party
 from result import Err
 from result import Ok
 from result import Result
 from typing_extensions import Self
 
 # relative
-from ....external import OBLV
-from .action_object import ActionObject
-from .action_service import ActionService
-from .action_store import ActionObjectPermission
-from .action_store import ActionPermission
-from .api import APIRegistry
-from .context import AuthedServiceContext
-from .context import ChangeContext
-from .credentials import SyftVerifyKey
-from .datetime import DateTime
-from .linked_obj import LinkedObject
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .serialize import _serialize
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftObject
-from .transforms import TransformContext
-from .transforms import add_node_uid_for_key
-from .transforms import generate_id
-from .transforms import transform
-from .uid import UID
-from .user_code import UserCode
-from .user_code import UserCodeStatus
+from ...client.api import APIRegistry
+from ...external import OBLV
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...serde.serialize import _serialize
+from ...store.linked_obj import LinkedObject
+from ...types.datetime import DateTime
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftObject
+from ...types.transforms import TransformContext
+from ...types.transforms import add_node_uid_for_key
+from ...types.transforms import generate_id
+from ...types.transforms import transform
+from ...types.uid import UID
+from ..action.action_object import ActionObject
+from ..action.action_service import ActionService
+from ..action.action_store import ActionObjectPermission
+from ..action.action_store import ActionPermission
+from ..code.user_code import UserCode
+from ..code.user_code import UserCodeStatus
+from ..context import AuthedServiceContext
+from ..context import ChangeContext
+from ..response import SyftError
+from ..response import SyftSuccess
 
 
 @serializable()
 class RequestStatus(Enum):
     PENDING = 0
     REJECTED = 1
     APPROVED = 2
@@ -455,15 +455,15 @@
                 res = self.mutate(obj, context)
 
                 if res.is_err():
                     return res
                 res = res.ok()
                 if OBLV:
                     # relative
-                    from ....external.oblv.oblv_service import check_enclave_transfer
+                    from ...external.oblv.oblv_service import check_enclave_transfer
 
                     enclave_res = check_enclave_transfer(
                         user_code=res, value=self.value, context=context
                     )
                 else:
                     enclave_res = Ok()
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/request_service.py` & `syft-0.8.0b9/src/syft/service/request/request_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 from typing import Union
 
 # third party
 from result import Err
 from result import Ok
 
 # relative
-from ....telemetry import instrument
-from .action_permissions import ActionObjectPermission
-from .action_permissions import ActionPermission
-from .context import AuthedServiceContext
-from .document_store import DocumentStore
-from .linked_obj import LinkedObject
-from .message_service import CreateMessage
-from .message_service import Message
-from .message_service import MessageService
+from ...serde.serializable import serializable
+from ...store.document_store import DocumentStore
+from ...store.linked_obj import LinkedObject
+from ...types.uid import UID
+from ...util.telemetry import instrument
+from ..action.action_permissions import ActionObjectPermission
+from ..action.action_permissions import ActionPermission
+from ..context import AuthedServiceContext
+from ..message.message_service import CreateMessage
+from ..message.message_service import Message
+from ..message.message_service import MessageService
+from ..response import SyftError
+from ..response import SyftSuccess
+from ..service import AbstractService
+from ..service import SERVICE_TO_TYPES
+from ..service import TYPE_TO_SERVICE
+from ..service import service_method
+from ..user.user_service import UserService
 from .request import Request
 from .request import RequestStatus
 from .request import SubmitRequest
 from .request_stash import RequestStash
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .service import AbstractService
-from .service import SERVICE_TO_TYPES
-from .service import TYPE_TO_SERVICE
-from .service import service_method
-from .uid import UID
-from .user_service import UserService
 
 
 @instrument
 @serializable()
 class RequestService(AbstractService):
     store: DocumentStore
     stash: RequestStash
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/request_stash.py` & `syft-0.8.0b9/src/syft/service/code/user_code_stash.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 # stdlib
 from typing import List
+from typing import Optional
 
 # third party
 from result import Result
 
 # relative
-from ....telemetry import instrument
-from .credentials import SyftVerifyKey
-from .document_store import BaseUIDStoreStash
-from .document_store import PartitionKey
-from .document_store import PartitionSettings
-from .document_store import QueryKeys
-from .request import Request
-from .request import RequestStatus
-from .serializable import serializable
-
-RequestingUserVerifyKeyPartitionKey = PartitionKey(
-    key="requesting_user_verify_key", type_=SyftVerifyKey
-)
-StatusPartitionKey = PartitionKey(key="status", type_=RequestStatus)
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...store.document_store import BaseUIDStoreStash
+from ...store.document_store import DocumentStore
+from ...store.document_store import PartitionSettings
+from ...store.document_store import QueryKeys
+from ...util.telemetry import instrument
+from .user_code import CodeHashPartitionKey
+from .user_code import UserCode
+from .user_code import UserVerifyKeyPartitionKey
 
 
 @instrument
 @serializable()
-class RequestStash(BaseUIDStoreStash):
-    object_type = Request
+class UserCodeStash(BaseUIDStoreStash):
+    object_type = UserCode
     settings: PartitionSettings = PartitionSettings(
-        name=Request.__canonical_name__, object_type=Request
+        name=UserCode.__canonical_name__, object_type=UserCode
     )
 
-    def get_all_for_verify_key(
-        self,
-        credentials: SyftVerifyKey,
-        verify_key: SyftVerifyKey,
-    ) -> Result[List[Request], str]:
-        if isinstance(verify_key, str):
-            verify_key = SyftVerifyKey.from_string(verify_key)
-        qks = QueryKeys(qks=[RequestingUserVerifyKeyPartitionKey.with_obj(verify_key)])
-        return self.query_all(credentials=credentials, qks=qks)
-
-    def get_all_for_status(
-        self, credentials: SyftVerifyKey, status: RequestStatus
-    ) -> Result[List[Request], str]:
-        qks = QueryKeys(qks=[StatusPartitionKey.with_obj(status)])
-        return self.query_all(credentials=credentials, qks=qks)
+    def __init__(self, store: DocumentStore) -> None:
+        super().__init__(store=store)
+
+    def get_all_by_user_verify_key(
+        self, credentials: SyftVerifyKey, user_verify_key: SyftVerifyKey
+    ) -> Result[List[UserCode], str]:
+        qks = QueryKeys(qks=[UserVerifyKeyPartitionKey.with_obj(user_verify_key)])
+        return self.query_one(credentials=credentials, qks=qks)
+
+    def get_by_code_hash(
+        self, credentials: SyftVerifyKey, code_hash: int
+    ) -> Result[Optional[UserCode], str]:
+        qks = QueryKeys(qks=[CodeHashPartitionKey.with_obj(code_hash)])
+        return self.query_one(credentials=credentials, qks=qks)
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/response.py` & `syft-0.8.0b9/src/syft/service/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # stdlib
 import sys
 import traceback
 from typing import Any
 
 # relative
-from .base import SyftBaseModel
-from .serializable import serializable
+from ..serde.serializable import serializable
+from ..types.base import SyftBaseModel
 
 
 class SyftResponseMessage(SyftBaseModel):
     message: str
     _bool: bool = True
 
     def __bool__(self) -> bool:
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/serializable.py` & `syft-0.8.0b9/src/syft/serde/serializable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # stdlib
+from typing import Callable
 from typing import List
 from typing import Optional
 from typing import TypeVar
 
 # syft absolute
 import syft
 
@@ -16,15 +17,15 @@
 
 
 def serializable(
     attrs: Optional[List[str]] = None,
     without: Optional[List[str]] = None,
     inherit: Optional[bool] = True,
     inheritable: Optional[bool] = True,
-) -> T:
+) -> Callable:
     """
     Recursively serialize attributes of the class.
 
     Args:
         `attrs`       : List of attributes to serialize
         `without`     : List of attributes to exclude from serialization
         `inherit`     : Whether to inherit serializable attribute list from base class
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/service.py` & `syft-0.8.0b9/src/syft/service/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,36 +13,33 @@
 from typing import Union
 
 # third party
 from result import Ok
 from result import OkErr
 
 # relative
+from ..abstract_node import AbstractNode
+from ..serde.serializable import serializable
+from ..serde.signature import Signature
+from ..serde.signature import signature_remove_context
+from ..serde.signature import signature_remove_self
+from ..store.linked_obj import LinkedObject
+from ..types.syft_object import SyftBaseObject
+from ..types.syft_object import SyftObject
+from ..types.uid import UID
 from .context import AuthedServiceContext
 from .context import ChangeContext
-from .linked_obj import LinkedObject
 from .response import SyftError
-from .serializable import serializable
-from .signature import Signature
-from .signature import signature_remove_context
-from .signature import signature_remove_self
-from .syft_object import SyftBaseObject
-from .syft_object import SyftObject
-from .uid import UID
-from .user_roles import DATA_OWNER_ROLE_LEVEL
-from .user_roles import ServiceRole
+from .user.user_roles import DATA_OWNER_ROLE_LEVEL
+from .user.user_roles import ServiceRole
 
 TYPE_TO_SERVICE = {}
 SERVICE_TO_TYPES = defaultdict(set)
 
 
-class AbstractNode:
-    id: UID
-
-
 class AbstractService:
     node: AbstractNode
     node_uid: UID
 
     def resolve_link(
         self, context: AuthedServiceContext, linked_obj: LinkedObject
     ) -> Union[Any, SyftError]:
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/signature.py` & `syft-0.8.0b9/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/core/node/new/sqlite_document_store.py` & `syft-0.8.0b9/src/syft/store/sqlite_document_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 from typing import Type
 from typing import Union
 
 # third party
 from typing_extensions import Self
 
 # relative
-from .deserialize import _deserialize
+from ..serde.deserialize import _deserialize
+from ..serde.serializable import serializable
+from ..serde.serialize import _serialize
+from ..types.uid import UID
 from .document_store import DocumentStore
 from .document_store import PartitionSettings
 from .document_store import StoreClientConfig
 from .document_store import StoreConfig
 from .kv_document_store import KeyValueBackingStore
 from .kv_document_store import KeyValueStorePartition
 from .locks import FileLockingConfig
 from .locks import LockingConfig
-from .serializable import serializable
-from .serialize import _serialize
-from .uid import UID
 
 
 def _repr_debug_(value: Any) -> str:
     if hasattr(value, "_repr_debug_"):
         return value._repr_debug_()
     return repr(value)
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/syft_metaclass.py` & `syft-0.8.0b9/src/syft/types/syft_metaclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # third party
 from pydantic.fields import UndefinedType
 from pydantic.main import BaseModel
 from pydantic.main import ModelField
 from pydantic.main import ModelMetaclass
 
 # relative
-from .recursive_primitives import recursive_serde_register_type
-from .serializable import serializable
+from ..serde.recursive_primitives import recursive_serde_register_type
+from ..serde.serializable import serializable
 
 TupleGenerator = Generator[Tuple[str, Any], None, None]
 
 
 @serializable()
 class Empty:
     pass
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/syft_object.py` & `syft-0.8.0b9/src/syft/types/syft_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 import pydantic
 from pydantic import BaseModel
 from pydantic import EmailStr
 from pydantic.fields import Undefined
 from typeguard import check_type
 
 # relative
-from ....util import aggressive_set_attr
-from .credentials import SyftVerifyKey
-from .deserialize import _deserialize as deserialize
-from .recursive_primitives import recursive_serde_register_type
-from .serialize import _serialize as serialize
+from ..node.credentials import SyftVerifyKey
+from ..serde.deserialize import _deserialize as deserialize
+from ..serde.recursive_primitives import recursive_serde_register_type
+from ..serde.serialize import _serialize as serialize
+from ..util.util import aggressive_set_attr
+from ..util.util import full_name_with_qualname
+from ..util.util import get_qualname_for
 from .syft_metaclass import Empty
 from .syft_metaclass import PartialModelMetaclass
 from .uid import UID
-from .util import full_name_with_qualname
-from .util import get_qualname_for
 
 SYFT_OBJECT_VERSION_1 = 1
 SYFT_OBJECT_VERSION_2 = 2
 
 supported_object_versions = [SYFT_OBJECT_VERSION_1, SYFT_OBJECT_VERSION_2]
 
 HIGHEST_SYFT_OBJECT_VERSION = max(supported_object_versions)
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/third_party.py` & `syft-0.8.0b9/src/syft/serde/third_party.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # stdlib
-
-# stdlib
 from datetime import date
 from datetime import datetime
 from datetime import time
 from io import BytesIO
 
 # third party
 from dateutil import parser
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/transforms.py` & `syft-0.8.0b9/src/syft/types/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 from typing import Union
 
 # third party
 from pydantic import EmailStr
 from typing_extensions import Self
 
 # relative
-from .context import AuthedServiceContext
-from .context import NodeServiceContext
-from .credentials import SyftVerifyKey
+from ..abstract_node import AbstractNode
+from ..node.credentials import SyftVerifyKey
+from ..service.context import AuthedServiceContext
+from ..service.context import NodeServiceContext
 from .grid_url import GridURL
-from .node import NewNode
 from .syft_object import Context
 from .syft_object import SyftBaseObject
 from .syft_object import SyftObjectRegistry
 from .uid import UID
 
 
 class NotNone:
     pass
 
 
 class TransformContext(Context):
     output: Optional[Dict[str, Any]]
-    node: Optional[NewNode]
+    node: Optional[AbstractNode]
     credentials: Optional[SyftVerifyKey]
     obj: Optional[Any]
 
     @staticmethod
     def from_context(obj: Any, context: Optional[Context] = None) -> Self:
         t_context = TransformContext()
         t_context.obj = obj
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/twin_object.py` & `syft-0.8.0b9/src/syft/types/twin_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from __future__ import annotations
 
 # stdlib
 from typing import Any
 from typing import Optional
 
 # relative
-from .action_object import ActionObject
-from .action_types import action_types
-from .serializable import serializable
+from ..serde.serializable import serializable
+from ..service.action.action_object import ActionObject
+from ..service.action.action_types import action_types
 from .syft_object import SyftObject
 from .uid import UID
 
 
 def to_action_object(obj: Any) -> ActionObject:
     if isinstance(obj, ActionObject):
         return obj
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/uid.py` & `syft-0.8.0b9/src/syft/types/uid.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from typing import Optional
 from typing import Sequence
 from typing import Union
 import uuid
 from uuid import UUID as uuid_type
 
 # relative
-from ....logger import critical
-from ....logger import traceback_and_raise
-from .serializable import serializable
+from ..serde.serializable import serializable
+from ..util.logger import critical
+from ..util.logger import traceback_and_raise
 
 
 @serializable(attrs=["value"])
 class UID:
     """A unique ID for every Syft object.
 
     This object creates a unique ID for every object in the Syft
@@ -52,15 +52,15 @@
                       in here. This is normally only used during deserialization.
         :type value: uuid.uuid4, optional
         :return: returns the initialized object
         :rtype: UID
 
         .. code-block:: python
 
-            from syft.core.common.uid import UID
+            from syft.types.uid import UID
             my_id = UID()
         """
         # checks to make sure you've set a proto_type
         super().__init__()
 
         # if value is not set - create a novel and unique ID.
         if isinstance(value, str):
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/unparse.py` & `syft-0.8.0b9/src/syft/service/code/unparse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/core/node/new/user.py` & `syft-0.8.0b9/src/syft/service/user/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 from bcrypt import checkpw
 from bcrypt import gensalt
 from bcrypt import hashpw
 import pydantic
 from pydantic.networks import EmailStr
 
 # relative
-from .credentials import SyftSigningKey
-from .credentials import SyftVerifyKey
-from .serializable import serializable
-from .syft_object import PartialSyftObject
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftObject
-from .transforms import TransformContext
-from .transforms import drop
-from .transforms import generate_id
-from .transforms import keep
-from .transforms import make_set_default
-from .transforms import transform
-from .transforms import validate_email
-from .uid import UID
+from ...node.credentials import SyftSigningKey
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...types.syft_object import PartialSyftObject
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftObject
+from ...types.transforms import TransformContext
+from ...types.transforms import drop
+from ...types.transforms import generate_id
+from ...types.transforms import keep
+from ...types.transforms import make_set_default
+from ...types.transforms import transform
+from ...types.transforms import validate_email
+from ...types.uid import UID
 from .user_roles import ServiceRole
 
 
 @serializable()
 class User(SyftObject):
     # version
     __canonical_name__ = "User"
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/user_code.py` & `syft-0.8.0b9/src/syft/service/code/user_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,53 +18,53 @@
 
 # third party
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
-from .api import NodeView
+from ...abstract_node import NodeType
+from ...client.api import NodeView
+from ...node.credentials import SyftVerifyKey
+from ...serde.deserialize import _deserialize
+from ...serde.serializable import serializable
+from ...serde.serialize import _serialize
+from ...store.document_store import PartitionKey
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftObject
+from ...types.transforms import TransformContext
+from ...types.transforms import generate_id
+from ...types.transforms import transform
+from ...types.uid import UID
+from ..context import AuthedServiceContext
+from ..dataset.dataset import Asset
+from ..metadata.node_metadata import EnclaveMetadata
+from ..policy.policy import CustomInputPolicy
+from ..policy.policy import CustomOutputPolicy
+from ..policy.policy import InputPolicy
+from ..policy.policy import OutputPolicy
+from ..policy.policy import Policy
+from ..policy.policy import SubmitUserPolicy
+from ..policy.policy import UserPolicy
+from ..policy.policy import init_policy
+from ..policy.policy_service import PolicyService
+from ..response import SyftError
 from .code_parse import GlobalsVisitor
-from .context import AuthedServiceContext
-from .credentials import SyftVerifyKey
-from .dataset import Asset
-from .deserialize import _deserialize
-from .document_store import PartitionKey
-from .node import NodeType
-from .node_metadata import EnclaveMetadata
-from .policy import CustomInputPolicy
-from .policy import CustomOutputPolicy
-from .policy import InputPolicy
-from .policy import OutputPolicy
-from .policy import Policy
-from .policy import SubmitUserPolicy
-from .policy import UserPolicy
-from .policy import init_policy
-from .policy_service import PolicyService
-from .response import SyftError
-from .serializable import serializable
-from .serialize import _serialize
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftObject
-from .transforms import TransformContext
-from .transforms import generate_id
-from .transforms import transform
-from .uid import UID
 from .unparse import unparse
 
 UserVerifyKeyPartitionKey = PartitionKey(key="user_verify_key", type_=SyftVerifyKey)
 CodeHashPartitionKey = PartitionKey(key="code_hash", type_=int)
 
 PyCodeObject = Any
 
 
 def extract_uids(kwargs: Dict[str, Any]) -> Dict[str, UID]:
     # relative
-    from .action_object import ActionObject
-    from .twin_object import TwinObject
+    from ...types.twin_object import TwinObject
+    from ..action.action_object import ActionObject
 
     uid_kwargs = {}
     for k, v in kwargs.items():
         uid = v
         if isinstance(v, ActionObject):
             uid = v.id
         if isinstance(v, TwinObject):
@@ -293,15 +293,15 @@
     @property
     def byte_code(self) -> Optional[PyCodeObject]:
         return compile_byte_code(self.parsed_code)
 
     @property
     def assets(self) -> List[Asset]:
         # relative
-        from .api import APIRegistry
+        from ...client.api import APIRegistry
 
         api = APIRegistry.api_for(self.node_uid)
         if api is None:
             return SyftError(message=f"You must login to {self.node_uid}")
 
         node_view = NodeView(
             node_name=api.node_name, verify_key=api.signing_key.verify_key
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/user_code_parse.py` & `syft-0.8.0b9/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/core/node/new/user_code_service.py` & `syft-0.8.0b9/src/syft/service/code/user_code_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 from typing import List
 from typing import Union
 
 # third party
 from result import OkErr
 
 # relative
-from ....telemetry import instrument
-from .context import AuthedServiceContext
-from .document_store import DocumentStore
-from .linked_obj import LinkedObject
-from .policy import OutputHistory
-from .policy import UserPolicy
-from .policy import load_policy_code
-from .request import SubmitRequest
-from .request import UserCodeStatusChange
-from .request_service import RequestService
-from .response import SyftError
-from .response import SyftNotReady
-from .response import SyftSuccess
-from .serializable import serializable
-from .service import AbstractService
-from .service import SERVICE_TO_TYPES
-from .service import TYPE_TO_SERVICE
-from .service import service_method
-from .twin_object import TwinObject
-from .uid import UID
+from ...serde.serializable import serializable
+from ...store.document_store import DocumentStore
+from ...store.linked_obj import LinkedObject
+from ...types.twin_object import TwinObject
+from ...types.uid import UID
+from ...util.telemetry import instrument
+from ..context import AuthedServiceContext
+from ..policy.policy import OutputHistory
+from ..policy.policy import UserPolicy
+from ..policy.policy import load_policy_code
+from ..request.request import SubmitRequest
+from ..request.request import UserCodeStatusChange
+from ..request.request_service import RequestService
+from ..response import SyftError
+from ..response import SyftNotReady
+from ..response import SyftSuccess
+from ..service import AbstractService
+from ..service import SERVICE_TO_TYPES
+from ..service import TYPE_TO_SERVICE
+from ..service import service_method
+from ..user.user_roles import GUEST_ROLE_LEVEL
 from .user_code import SubmitUserCode
 from .user_code import UserCode
 from .user_code import UserCodeStatus
 from .user_code_stash import UserCodeStash
-from .user_roles import GUEST_ROLE_LEVEL
 
 
 @instrument
 @serializable()
 class UserCodeService(AbstractService):
     store: DocumentStore
     stash: UserCodeStash
@@ -204,15 +204,15 @@
             return final_results
         except Exception as e:
             return SyftError(message=f"Failed to run. {e}")
 
 
 def get_outputs(context: AuthedServiceContext, output_history: OutputHistory) -> Any:
     # relative
-    from .action_service import TwinMode
+    from ...service.action.action_service import TwinMode
 
     if isinstance(output_history.outputs, list):
         if len(output_history.outputs) == 0:
             return None
         outputs = []
         for output_id in output_history.outputs:
             action_service = context.node.get_service("actionservice")
@@ -227,17 +227,17 @@
         return outputs
     else:
         raise NotImplementedError
 
 
 def filter_kwargs(kwargs: Dict[str, Any]) -> Dict[str, Any]:
     # relative
-    from .action_object import ActionObject
-    from .dataset import Asset
-    from .twin_object import TwinObject
+    from ...types.twin_object import TwinObject
+    from ..action.action_object import ActionObject
+    from ..dataset.dataset import Asset
 
     filtered_kwargs = {}
     for k, v in kwargs.items():
         value = v
         if isinstance(v, ActionObject):
             value = v.id
         if isinstance(v, TwinObject):
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/user_code_stash.py` & `syft-0.8.0b9/src/syft/service/policy/user_policy_stash.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,32 @@
 # stdlib
 from typing import List
-from typing import Optional
 
 # third party
 from result import Result
 
 # relative
-from ....telemetry import instrument
-from .credentials import SyftVerifyKey
-from .document_store import BaseUIDStoreStash
-from .document_store import DocumentStore
-from .document_store import PartitionSettings
-from .document_store import QueryKeys
-from .serializable import serializable
-from .user_code import CodeHashPartitionKey
-from .user_code import UserCode
-from .user_code import UserVerifyKeyPartitionKey
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...store.document_store import BaseUIDStoreStash
+from ...store.document_store import DocumentStore
+from ...store.document_store import PartitionSettings
+from ...store.document_store import QueryKeys
+from .policy import PolicyUserVerifyKeyPartitionKey
+from .policy import UserPolicy
 
 
-@instrument
 @serializable()
-class UserCodeStash(BaseUIDStoreStash):
-    object_type = UserCode
+class UserPolicyStash(BaseUIDStoreStash):
+    object_type = UserPolicy
     settings: PartitionSettings = PartitionSettings(
-        name=UserCode.__canonical_name__, object_type=UserCode
+        name=UserPolicy.__canonical_name__, object_type=UserPolicy
     )
 
     def __init__(self, store: DocumentStore) -> None:
         super().__init__(store=store)
 
     def get_all_by_user_verify_key(
         self, credentials: SyftVerifyKey, user_verify_key: SyftVerifyKey
-    ) -> Result[List[UserCode], str]:
-        qks = QueryKeys(qks=[UserVerifyKeyPartitionKey.with_obj(user_verify_key)])
-        return self.query_one(credentials=credentials, qks=qks)
-
-    def get_by_code_hash(
-        self, credentials: SyftVerifyKey, code_hash: int
-    ) -> Result[Optional[UserCode], str]:
-        qks = QueryKeys(qks=[CodeHashPartitionKey.with_obj(code_hash)])
+    ) -> Result[List[UserPolicy], str]:
+        qks = QueryKeys(qks=[PolicyUserVerifyKeyPartitionKey.with_obj(user_verify_key)])
         return self.query_one(credentials=credentials, qks=qks)
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/user_roles.py` & `syft-0.8.0b9/src/syft/service/user/user_roles.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Tuple
 from typing import Union
 
 # third party
 from typing_extensions import Self
 
 # relative
-from .serializable import serializable
+from ...serde.serializable import serializable
 
 
 class ServiceRoleCapability(Enum):
     CAN_MAKE_DATA_REQUESTS = 1
     CAN_TRIAGE_DATA_REQUESTS = 2
     CAN_MANAGE_PRIVACY_BUDGET = 4
     CAN_CREATE_USERS = 8
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/user_service.py` & `syft-0.8.0b9/src/syft/service/user/user_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # stdlib
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 # relative
-from ....telemetry import instrument
-from .action_permissions import ActionObjectPermission
-from .action_permissions import ActionPermission
-from .context import AuthedServiceContext
-from .context import NodeServiceContext
-from .context import UnauthedServiceContext
-from .credentials import SyftVerifyKey
-from .credentials import UserLoginCredentials
-from .document_store import DocumentStore
-from .response import SyftError
-from .response import SyftSuccess
-from .serializable import serializable
-from .service import AbstractService
-from .service import SERVICE_TO_TYPES
-from .service import TYPE_TO_SERVICE
-from .service import service_method
-from .syft_metaclass import Empty
-from .uid import UID
+from ...node.credentials import SyftVerifyKey
+from ...node.credentials import UserLoginCredentials
+from ...serde.serializable import serializable
+from ...store.document_store import DocumentStore
+from ...types.syft_metaclass import Empty
+from ...types.uid import UID
+from ...util.telemetry import instrument
+from ..action.action_permissions import ActionObjectPermission
+from ..action.action_permissions import ActionPermission
+from ..context import AuthedServiceContext
+from ..context import NodeServiceContext
+from ..context import UnauthedServiceContext
+from ..response import SyftError
+from ..response import SyftSuccess
+from ..service import AbstractService
+from ..service import SERVICE_TO_TYPES
+from ..service import TYPE_TO_SERVICE
+from ..service import service_method
 from .user import User
 from .user import UserCreate
 from .user import UserPrivateKey
 from .user import UserSearch
 from .user import UserUpdate
 from .user import UserView
 from .user import check_pwd
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/user_stash.py` & `syft-0.8.0b9/src/syft/service/user/user_stash.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from typing import Optional
 
 # third party
 from result import Ok
 from result import Result
 
 # relative
-from ....telemetry import instrument
-from .action_permissions import ActionObjectPermission
-from .credentials import SyftSigningKey
-from .credentials import SyftVerifyKey
-from .document_store import BaseStash
-from .document_store import DocumentStore
-from .document_store import PartitionKey
-from .document_store import PartitionSettings
-from .document_store import QueryKeys
-from .document_store import UIDPartitionKey
-from .response import SyftSuccess
-from .serializable import serializable
-from .uid import UID
+from ...node.credentials import SyftSigningKey
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...store.document_store import BaseStash
+from ...store.document_store import DocumentStore
+from ...store.document_store import PartitionKey
+from ...store.document_store import PartitionSettings
+from ...store.document_store import QueryKeys
+from ...store.document_store import UIDPartitionKey
+from ...types.uid import UID
+from ...util.telemetry import instrument
+from ..action.action_permissions import ActionObjectPermission
+from ..response import SyftSuccess
 from .user import User
 from .user_roles import ServiceRole
 
 # 🟡 TODO 27: it would be nice if these could be defined closer to the User
 EmailPartitionKey = PartitionKey(key="email", type_=str)
 RolePartitionKey = PartitionKey(key="role", type_=ServiceRole)
 SigningKeyPartitionKey = PartitionKey(key="signing_key", type_=SyftSigningKey)
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/util.py` & `syft-0.8.0b9/src/syft/util/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 # third party
 from forbiddenfruit import curse
 from nacl.signing import SigningKey
 from nacl.signing import VerifyKey
 import requests
 
 # relative
-from ....logger import critical
-from ....logger import debug
-from ....logger import error
-from ....logger import traceback_and_raise
+from .logger import critical
+from .logger import debug
+from .logger import error
+from .logger import traceback_and_raise
 
 
 def full_name_with_qualname(klass: type) -> str:
     """Returns the klass module name + klass qualname."""
     try:
         if not hasattr(klass, "__module__"):
             return f"builtins.{get_qualname_for(klass)}"
@@ -104,27 +104,236 @@
         return _object
 
     traceback_and_raise(
         f"Object {_object} should've been of type {_type}, not {_object}."
     )
 
 
-def get_loaded_syft() -> ModuleType:
-    return sys.modules[__name__.split(".")[0]]
-
-
 def validate_field(_object: object, _field: str) -> Any:
     object = getattr(_object, _field, None)
 
     if object is not None:
         return object
 
     traceback_and_raise(f"Object {_object} has no {_field} field set.")
 
 
+def get_fully_qualified_name(obj: object) -> str:
+    """Return the full path and name of a class
+
+    Sometimes we want to return the entire path and name encoded
+    using periods.
+
+    Args:
+        obj: the object we want to get the name of
+
+    Returns:
+        the full path and name of the object
+
+    """
+
+    fqn = obj.__class__.__module__
+
+    try:
+        fqn += "." + obj.__class__.__name__
+    except Exception as e:
+        error(f"Failed to get FQN: {e}")
+    return fqn
+
+
+def aggressive_set_attr(obj: object, name: str, attr: object) -> None:
+    """Different objects prefer different types of monkeypatching - try them all
+
+    Args:
+        obj: object whose attribute has to be set
+        name: attribute name
+        attr: value given to the attribute
+
+    """
+    try:
+        setattr(obj, name, attr)
+    except Exception:
+        curse(obj, name, attr)
+
+
+def key_emoji(key: object) -> str:
+    try:
+        if isinstance(key, (bytes, SigningKey, VerifyKey)):
+            hex_chars = bytes(key).hex()[-8:]
+            return char_emoji(hex_chars=hex_chars)
+    except Exception as e:
+        error(f"Fail to get key emoji: {e}")
+        pass
+    return "ALL"
+
+
+def char_emoji(hex_chars: str) -> str:
+    base = ord("\U0001F642")
+    hex_base = ord("0")
+    code = 0
+    for char in hex_chars:
+        offset = ord(char)
+        code += offset - hex_base
+    return chr(base + code)
+
+
+def get_root_data_path() -> Path:
+    # get the PySyft / data directory to share datasets between notebooks
+    # on Linux and MacOS the directory is: ~/.syft/data"
+    # on Windows the directory is: C:/Users/$USER/.syft/data
+
+    data_dir = Path.home() / ".syft" / "data"
+
+    os.makedirs(data_dir, exist_ok=True)
+    return data_dir
+
+
+def download_file(url: str, full_path: Union[str, Path]) -> Optional[Path]:
+    if not os.path.exists(full_path):
+        r = requests.get(url, allow_redirects=True, verify=verify_tls())  # nosec
+        if r.status_code < 199 or 299 < r.status_code:
+            print(f"Got {r.status_code} trying to download {url}")
+            return None
+        path = os.path.dirname(full_path)
+        os.makedirs(path, exist_ok=True)
+        with open(full_path, "wb") as f:
+            f.write(r.content)
+    return Path(full_path)
+
+
+def verify_tls() -> bool:
+    return not str_to_bool(str(os.environ.get("IGNORE_TLS_ERRORS", "0")))
+
+
+def ssl_test() -> bool:
+    return len(os.environ.get("REQUESTS_CA_BUNDLE", "")) > 0
+
+
+def initializer(event_loop: Optional[BaseSelectorEventLoop] = None) -> None:
+    """Set the same event loop to other threads/processes.
+    This is needed because there are new threads/processes started with
+    the Executor and they do not have have an event loop set
+    Args:
+        event_loop: The event loop.
+    """
+    if event_loop:
+        asyncio.set_event_loop(event_loop)
+
+
+def split_rows(rows: Sequence, cpu_count: int) -> List:
+    n = len(rows)
+    a, b = divmod(n, cpu_count)
+    start = 0
+    output = []
+    for i in range(cpu_count):
+        end = start + a + (1 if b - i - 1 >= 0 else 0)
+        output.append(rows[start:end])
+        start = end
+    return output
+
+
+def list_sum(*inp_lst: List[Any]) -> Any:
+    s = inp_lst[0]
+    for i in inp_lst[1:]:
+        s = s + i
+    return s
+
+
+@contextmanager
+def concurrency_override(count: int = 1) -> Iterator:
+    # this only effects local code so its best to use in unit tests
+    try:
+        os.environ["FORCE_CONCURRENCY_COUNT"] = f"{count}"
+        yield None
+    finally:
+        os.environ["FORCE_CONCURRENCY_COUNT"] = "0"
+
+
+def print_process(  # type: ignore
+    message: str,
+    finish: EventClass,
+    success: EventClass,
+    lock: LockBase,
+    refresh_rate=0.1,
+) -> None:
+    with lock:
+        while not finish.is_set():  # type: ignore
+            print(f"{bcolors.bold(message)} .", end="\r")
+            time.sleep(refresh_rate)
+            sys.stdout.flush()
+            print(f"{bcolors.bold(message)} ..", end="\r")
+            time.sleep(refresh_rate)
+            sys.stdout.flush()
+            print(f"{bcolors.bold(message)} ...", end="\r")
+            time.sleep(refresh_rate)
+            sys.stdout.flush()
+        if success.is_set():  # type: ignore
+            print(f"{bcolors.success(message)}" + (" " * len(message)), end="\n")
+        else:
+            print(f"{bcolors.failure(message)}" + (" " * len(message)), end="\n")
+        sys.stdout.flush()
+
+
+def print_dynamic_log(
+    message: str,
+) -> Tuple[EventClass, EventClass]:
+    """
+    Prints a dynamic log message that will change its color (to green or red) when some process is done.
+
+    message: str = Message to be printed.
+
+    return: tuple of events that can control the log print from the outside of this method.
+    """
+    finish = multiprocessing.Event()
+    success = multiprocessing.Event()
+    lock = multiprocessing.Lock()
+
+    if os_name() == "macOS":
+        # set start method to fork in case of MacOS
+        set_start_method("fork", force=True)
+
+    multiprocessing.Process(
+        target=print_process, args=(message, finish, success, lock)
+    ).start()
+    return (finish, success)
+
+
+def find_available_port(host: str, port: int, search: bool = False) -> int:
+    port_available = False
+    while not port_available:
+        try:
+            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            result_of_check = sock.connect_ex((host, port))
+
+            if result_of_check != 0:
+                port_available = True
+                break
+            else:
+                if search:
+                    port += 1
+                else:
+                    break
+
+        except Exception as e:
+            print(f"Failed to check port {port}. {e}")
+    sock.close()
+
+    if search is False and port_available is False:
+        error = (
+            f"{port} is in use, either free the port or "
+            + f"try: {port}+ to auto search for a port"
+        )
+        raise Exception(error)
+    return port
+
+
+def get_loaded_syft() -> ModuleType:
+    return sys.modules[__name__.split(".")[0]]
+
+
 def get_subclasses(obj_type: type) -> List[type]:
     """Recursively generate the list of all classes within the sub-tree of an object
 
     As a paradigm in Syft, we often allow for something to be known about by another
     part of the codebase merely because it has subclassed a particular object. While
     this can be a big "magicish" it also can simplify future extensions and reduce
     the likelihood of small mistakes (if done right).
@@ -190,66 +399,20 @@
     if fully_qualified_name == "builtins.NoneType":
         fully_qualified_name = "syft.lib.python._SyNone"
     attr_list = fully_qualified_name.split(".")
 
     if attr_list[0] != "syft":
         raise ReferenceError(f"Reference don't match: {attr_list[0]}")
 
-    if (
-        attr_list[1] != "core"
-        and attr_list[1] != "lib"
-        and attr_list[1] != "grid"
-        and attr_list[1] != "wrappers"
-        and attr_list[1] != "proxy"
-    ):
-        raise ReferenceError(f"Reference don't match: {attr_list[1]}")
+    # if attr_list[1] != "core" and attr_list[1] != "user":
+    #     raise ReferenceError(f"Reference don't match: {attr_list[1]}")
 
     return index_modules(a_dict=get_loaded_syft(), keys=attr_list[1:])
 
 
-def get_fully_qualified_name(obj: object) -> str:
-    """Return the full path and name of a class
-
-    Sometimes we want to return the entire path and name encoded
-    using periods. For example syft.core.common.message.SyftMessage
-    is the current fully qualified path and name for the SyftMessage
-    object.
-
-    Args:
-        obj: the object we want to get the name of
-
-    Returns:
-        the full path and name of the object
-
-    """
-
-    fqn = obj.__class__.__module__
-
-    try:
-        fqn += "." + obj.__class__.__name__
-    except Exception as e:
-        error(f"Failed to get FQN: {e}")
-    return fqn
-
-
-def aggressive_set_attr(obj: object, name: str, attr: object) -> None:
-    """Different objects prefer different types of monkeypatching - try them all
-
-    Args:
-        obj: object whose attribute has to be set
-        name: attribute name
-        attr: value given to the attribute
-
-    """
-    try:
-        setattr(obj, name, attr)
-    except Exception:
-        curse(obj, name, attr)
-
-
 def obj2pointer_type(obj: Optional[object] = None, fqn: Optional[str] = None) -> type:
     if fqn is None:
         try:
             fqn = get_fully_qualified_name(obj=obj)
         except Exception as e:
             # sometimes the object doesn't have a __module__ so you need to use the type
             # like: collections.OrderedDict
@@ -268,35 +431,14 @@
         log = f"Cannot find {type(obj)} {fqn} in lib_ast. {e}"
         critical(log)
         raise Exception(log)
 
     return ref.pointer_type  # type: ignore
 
 
-def key_emoji(key: object) -> str:
-    try:
-        if isinstance(key, (bytes, SigningKey, VerifyKey)):
-            hex_chars = bytes(key).hex()[-8:]
-            return char_emoji(hex_chars=hex_chars)
-    except Exception as e:
-        error(f"Fail to get key emoji: {e}")
-        pass
-    return "ALL"
-
-
-def char_emoji(hex_chars: str) -> str:
-    base = ord("\U0001F642")
-    hex_base = ord("0")
-    code = 0
-    for char in hex_chars:
-        offset = ord(char)
-        code += offset - hex_base
-    return chr(base + code)
-
-
 left_name = [
     "admiring",
     "adoring",
     "affectionate",
     "agitated",
     "amazing",
     "angry",
@@ -498,25 +640,14 @@
 
     # only generate new tags if the result actually inherit some tags.
     if tags:
         tags.append(attr_path_and_name.split(".")[-1])
         result.tags = tags  # type: ignore
 
 
-def get_root_data_path() -> Path:
-    # get the PySyft / data directory to share datasets between notebooks
-    # on Linux and MacOS the directory is: ~/.syft/data"
-    # on Windows the directory is: C:/Users/$USER/.syft/data
-
-    data_dir = Path.home() / ".syft" / "data"
-
-    os.makedirs(data_dir, exist_ok=True)
-    return data_dir
-
-
 def autocache(
     url: str, extension: Optional[str] = None, cache: bool = True
 ) -> Optional[Path]:
     try:
         data_path = get_root_data_path()
         file_hash = hashlib.sha256(url.encode("utf8")).hexdigest()
         filename = file_hash
@@ -526,54 +657,22 @@
         if os.path.exists(file_path) and cache:
             return file_path
         return download_file(url, file_path)
     except Exception as e:
         print(f"Failed to autocache: {url}. {e}")
 
 
-def download_file(url: str, full_path: Union[str, Path]) -> Optional[Path]:
-    if not os.path.exists(full_path):
-        r = requests.get(url, allow_redirects=True, verify=verify_tls())  # nosec
-        if r.status_code < 199 or 299 < r.status_code:
-            print(f"Got {r.status_code} trying to download {url}")
-            return None
-        path = os.path.dirname(full_path)
-        os.makedirs(path, exist_ok=True)
-        with open(full_path, "wb") as f:
-            f.write(r.content)
-    return Path(full_path)
-
-
 def str_to_bool(bool_str: Optional[str]) -> bool:
     result = False
     bool_str = str(bool_str).lower()
     if bool_str == "true" or bool_str == "1":
         result = True
     return result
 
 
-def verify_tls() -> bool:
-    return not str_to_bool(str(os.environ.get("IGNORE_TLS_ERRORS", "0")))
-
-
-def ssl_test() -> bool:
-    return len(os.environ.get("REQUESTS_CA_BUNDLE", "")) > 0
-
-
-def initializer(event_loop: Optional[BaseSelectorEventLoop] = None) -> None:
-    """Set the same event loop to other threads/processes.
-    This is needed because there are new threads/processes started with
-    the Executor and they do not have have an event loop set
-    Args:
-        event_loop: The event loop.
-    """
-    if event_loop:
-        asyncio.set_event_loop(event_loop)
-
-
 # local scope functions cant be pickled so this needs to be global
 def parallel_execution(
     fn: Callable[..., Any],
     parties: Union[None, List[Any]] = None,
     cpu_bound: bool = False,
 ) -> Callable[..., List[Any]]:
     """Wrap a function such that it can be run in parallel at multiple parties.
@@ -641,49 +740,20 @@
         local_shares = [f.result() for f in futures]
 
         return local_shares
 
     return wrapper
 
 
-def split_rows(rows: Sequence, cpu_count: int) -> List:
-    n = len(rows)
-    a, b = divmod(n, cpu_count)
-    start = 0
-    output = []
-    for i in range(cpu_count):
-        end = start + a + (1 if b - i - 1 >= 0 else 0)
-        output.append(rows[start:end])
-        start = end
-    return output
-
-
-def list_sum(*inp_lst: List[Any]) -> Any:
-    s = inp_lst[0]
-    for i in inp_lst[1:]:
-        s = s + i
-    return s
-
-
 def concurrency_count(factor: float = 0.8) -> int:
     force_count = int(os.environ.get("FORCE_CONCURRENCY_COUNT", 0))
     mp_count = force_count if force_count >= 1 else int(mp.cpu_count() * factor)
     return mp_count
 
 
-@contextmanager
-def concurrency_override(count: int = 1) -> Iterator:
-    # this only effects local code so its best to use in unit tests
-    try:
-        os.environ["FORCE_CONCURRENCY_COUNT"] = f"{count}"
-        yield None
-    finally:
-        os.environ["FORCE_CONCURRENCY_COUNT"] = "0"
-
-
 class bcolors:
     HEADER = "\033[95m"
     BLUE = "\033[94m"
     GREEN = "\033[92m"
     YELLOW = "\033[93m"
     RED = "\033[91m"
     ENDC = "\033[0m"
@@ -726,91 +796,34 @@
         return bcolors.green(message)
 
     @staticmethod
     def failure(message: str) -> str:
         return bcolors.red(message)
 
 
-def print_process(  # type: ignore
-    message: str,
-    finish: EventClass,
-    success: EventClass,
-    lock: LockBase,
-    refresh_rate=0.1,
-) -> None:
-    with lock:
-        while not finish.is_set():  # type: ignore
-            print(f"{bcolors.bold(message)} .", end="\r")
-            time.sleep(refresh_rate)
-            sys.stdout.flush()
-            print(f"{bcolors.bold(message)} ..", end="\r")
-            time.sleep(refresh_rate)
-            sys.stdout.flush()
-            print(f"{bcolors.bold(message)} ...", end="\r")
-            time.sleep(refresh_rate)
-            sys.stdout.flush()
-        if success.is_set():  # type: ignore
-            print(f"{bcolors.success(message)}" + (" " * len(message)), end="\n")
-        else:
-            print(f"{bcolors.failure(message)}" + (" " * len(message)), end="\n")
-        sys.stdout.flush()
-
-
 def os_name() -> str:
     os_name = platform.system()
     if os_name.lower() == "darwin":
         return "macOS"
     else:
         return os_name
 
 
-def print_dynamic_log(
-    message: str,
-) -> Tuple[EventClass, EventClass]:
-    """
-    Prints a dynamic log message that will change its color (to green or red) when some process is done.
-
-    message: str = Message to be printed.
-
-    return: tuple of events that can control the log print from the outside of this method.
-    """
-    finish = multiprocessing.Event()
-    success = multiprocessing.Event()
-    lock = multiprocessing.Lock()
+# Note: In the future there might be other interpreters that we want to use
+def is_interpreter_jupyter() -> bool:
+    return get_interpreter_module() == "ipykernel.zmqshell"
 
-    if os_name() == "macOS":
-        # set start method to fork in case of MacOS
-        set_start_method("fork", force=True)
-
-    multiprocessing.Process(
-        target=print_process, args=(message, finish, success, lock)
-    ).start()
-    return (finish, success)
 
+def is_interpreter_colab() -> bool:
+    return get_interpreter_module() == "google.colab._shell"
 
-def find_available_port(host: str, port: int, search: bool = False) -> int:
-    port_available = False
-    while not port_available:
-        try:
-            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            result_of_check = sock.connect_ex((host, port))
 
-            if result_of_check != 0:
-                port_available = True
-                break
-            else:
-                if search:
-                    port += 1
-                else:
-                    break
+def is_interpreter_standard() -> bool:
+    return get_interpreter_module() == "StandardInterpreter"
 
-        except Exception as e:
-            print(f"Failed to check port {port}. {e}")
-    sock.close()
 
-    if search is False and port_available is False:
-        error = (
-            f"{port} is in use, either free the port or "
-            + f"try: {port}+ to auto search for a port"
-        )
-        raise Exception(error)
-    return port
+def get_interpreter_module() -> str:
+    try:
+        shell = get_ipython().__class__.__module__
+        return shell
+    except NameError:
+        return "StandardInterpreter"  # not sure
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/verification.py` & `syft-0.8.0b9/src/syft/service/action/verification.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from typing import Union
 
 # third party
 import numpy as np
 import pandas as pd
 
 # relative
+from ..response import SyftError
+from ..response import SyftResponseMessage
+from ..response import SyftSuccess
 from .action_object import ActionObject
-from .response import SyftError
-from .response import SyftResponseMessage
-from .response import SyftSuccess
 
 
 def verify_result(
     func: Callable,
     private_inputs: Union[ActionObject, List[ActionObject]],
     private_outputs: Union[ActionObject, List[ActionObject]],
 ) -> SyftResponseMessage:
```

### Comparing `syft-0.8.0b8/src/syft/core/node/new/worker_settings.py` & `syft-0.8.0b9/src/syft/node/worker_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # future
 from __future__ import annotations
 
 # third party
 from typing_extensions import Self
 
 # relative
-from ..new.credentials import SyftSigningKey
-from ..new.document_store import StoreConfig
-from ..new.node import NewNode
-from .serializable import serializable
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftObject
-from .uid import UID
+from ..abstract_node import AbstractNode
+from ..node.credentials import SyftSigningKey
+from ..serde.serializable import serializable
+from ..store.document_store import StoreConfig
+from ..types.syft_object import SYFT_OBJECT_VERSION_1
+from ..types.syft_object import SyftObject
+from ..types.uid import UID
 
 
 @serializable()
 class WorkerSettings(SyftObject):
     __canonical_name__ = "WorkerSettings"
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: UID
     name: str
     signing_key: SyftSigningKey
     document_store_config: StoreConfig
     action_store_config: StoreConfig
 
     @staticmethod
-    def from_node(node: NewNode) -> Self:
+    def from_node(node: AbstractNode) -> Self:
         return WorkerSettings(
             id=node.id,
             name=node.name,
             signing_key=node.signing_key,
             document_store_config=node.document_store_config,
             action_store_config=node.action_store_config,
         )
```

### Comparing `syft-0.8.0b8/src/syft/core/node/worker.py` & `syft-0.8.0b9/src/syft/node/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,69 +22,67 @@
 from gipc.gipc import _GIPCDuplexHandle
 from nacl.signing import SigningKey
 from result import Err
 from result import Result
 from typing_extensions import Self
 
 # relative
-from ... import __version__
-from ...external import OBLV
-from ...telemetry import instrument
-from ...util import random_name
-from .new.action_service import ActionService
-from .new.action_store import DictActionStore
-from .new.action_store import SQLiteActionStore
-from .new.api import SignedSyftAPICall
-from .new.api import SyftAPI
-from .new.api import SyftAPICall
-from .new.api import SyftAPIData
-from .new.context import AuthedServiceContext
-from .new.context import NodeServiceContext
-from .new.context import UnauthedServiceContext
-from .new.context import UserLoginCredentials
-from .new.credentials import SyftSigningKey
-from .new.credentials import SyftVerifyKey
-from .new.data_subject_member_service import DataSubjectMemberService
-from .new.data_subject_service import DataSubjectService
-from .new.dataset_service import DatasetService
-from .new.deserialize import _deserialize
-from .new.dict_document_store import DictStoreConfig
-from .new.document_store import StoreConfig
-from .new.message_service import MessageService
-from .new.metadata_service import MetadataService
-from .new.metadata_stash import MetadataStash
-from .new.network_service import NetworkService
-from .new.node import NewNode
-from .new.node import NodeType
-from .new.node_metadata import NodeMetadata
-from .new.policy_service import PolicyService
-from .new.project_service import ProjectService
-from .new.queue_stash import QueueItem
-from .new.queue_stash import QueueStash
-from .new.request_service import RequestService
-from .new.response import SyftError
-from .new.serializable import serializable
-from .new.serialize import _serialize
-from .new.service import AbstractService
-from .new.service import ServiceConfigRegistry
-from .new.service import UserServiceConfigRegistry
-from .new.sqlite_document_store import SQLiteStoreClientConfig
-from .new.sqlite_document_store import SQLiteStoreConfig
-from .new.syft_object import HIGHEST_SYFT_OBJECT_VERSION
-from .new.syft_object import LOWEST_SYFT_OBJECT_VERSION
-from .new.syft_object import SyftObject
-from .new.test_service import TestService
-from .new.uid import UID
-from .new.user import User
-from .new.user import UserCreate
-from .new.user_code_service import UserCodeService
-from .new.user_roles import ServiceRole
-from .new.user_service import UserService
-from .new.user_stash import UserStash
-from .new.worker_settings import WorkerSettings
+from .. import __version__
+from ..abstract_node import AbstractNode
+from ..abstract_node import NodeType
+from ..client.api import SignedSyftAPICall
+from ..client.api import SyftAPI
+from ..client.api import SyftAPICall
+from ..client.api import SyftAPIData
+from ..external import OBLV
+from ..serde.deserialize import _deserialize
+from ..serde.serialize import _serialize
+from ..service.action.action_service import ActionService
+from ..service.action.action_store import DictActionStore
+from ..service.action.action_store import SQLiteActionStore
+from ..service.code.user_code_service import UserCodeService
+from ..service.context import AuthedServiceContext
+from ..service.context import NodeServiceContext
+from ..service.context import UnauthedServiceContext
+from ..service.context import UserLoginCredentials
+from ..service.data_subject.data_subject_member_service import DataSubjectMemberService
+from ..service.data_subject.data_subject_service import DataSubjectService
+from ..service.dataset.dataset_service import DatasetService
+from ..service.message.message_service import MessageService
+from ..service.metadata.metadata_service import MetadataService
+from ..service.metadata.metadata_stash import MetadataStash
+from ..service.metadata.node_metadata import NodeMetadata
+from ..service.network.network_service import NetworkService
+from ..service.policy.policy_service import PolicyService
+from ..service.project.project_service import ProjectService
+from ..service.queue.queue_stash import QueueItem
+from ..service.queue.queue_stash import QueueStash
+from ..service.request.request_service import RequestService
+from ..service.response import SyftError
+from ..service.service import AbstractService
+from ..service.service import ServiceConfigRegistry
+from ..service.service import UserServiceConfigRegistry
+from ..service.user.user import User
+from ..service.user.user import UserCreate
+from ..service.user.user_roles import ServiceRole
+from ..service.user.user_service import UserService
+from ..service.user.user_stash import UserStash
+from ..store.dict_document_store import DictStoreConfig
+from ..store.document_store import StoreConfig
+from ..store.sqlite_document_store import SQLiteStoreClientConfig
+from ..store.sqlite_document_store import SQLiteStoreConfig
+from ..types.syft_object import HIGHEST_SYFT_OBJECT_VERSION
+from ..types.syft_object import LOWEST_SYFT_OBJECT_VERSION
+from ..types.syft_object import SyftObject
+from ..types.uid import UID
+from ..util.telemetry import instrument
+from ..util.util import random_name
+from .credentials import SyftSigningKey
+from .credentials import SyftVerifyKey
+from .worker_settings import WorkerSettings
 
 
 def thread_ident() -> int:
     return threading.current_thread().ident
 
 
 # if user code needs to be serded and its not available we can call this to refresh
@@ -131,16 +129,15 @@
 node_uid_env = get_node_uid_env()
 
 default_root_email = get_default_root_email()
 default_root_password = get_default_root_password()
 
 
 @instrument
-@serializable()
-class Worker(NewNode):
+class Node(AbstractNode):
     signing_key: Optional[SyftSigningKey]
     required_signed_calls: bool = True
 
     def __init__(
         self,
         *,  # Trasterisk
         name: Optional[str] = None,
@@ -183,15 +180,14 @@
             name = random_name()
         self.name = name
         services = (
             [
                 UserService,
                 MetadataService,
                 ActionService,
-                TestService,
                 DatasetService,
                 UserCodeService,
                 RequestService,
                 DataSubjectService,
                 NetworkService,
                 PolicyService,
                 MessageService,
@@ -208,15 +204,15 @@
         self.init_stores(
             action_store_config=action_store_config,
             document_store_config=document_store_config,
         )
 
         if OBLV:
             # relative
-            from ...external.oblv.oblv_service import OblvService
+            from ..external.oblv.oblv_service import OblvService
 
             services += [OblvService]
             create_oblv_key_pair(worker=self)
 
         self.services = services
         self._construct_services()
 
@@ -278,45 +274,49 @@
 
     def is_root(self, credentials: SyftVerifyKey) -> bool:
         return credentials == self.signing_key.verify_key
 
     @property
     def root_client(self):
         # relative
-        from .new.client import PythonConnection
-        from .new.client import SyftClient
+        from ..client.client import PythonConnection
+        from ..client.client import SyftClient
 
         connection = PythonConnection(node=self)
         return SyftClient(connection=connection, credentials=self.signing_key)
 
     @property
     def guest_client(self):
         # relative
-        from .new.client import PythonConnection
-        from .new.client import SyftClient
+        from ..client.client import PythonConnection
+        from ..client.client import SyftClient
 
         connection = PythonConnection(node=self)
         return SyftClient(connection=connection, credentials=SyftSigningKey.generate())
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}: {self.name} - {self.id} - {self.node_type} - {self.services}"
+        services = []
+        for service in self.services:
+            services.append(service.__name__)
+        service_string = "\n".join(sorted(services))
+        return f"{type(self).__name__}: {self.name} - {self.id} - {self.node_type}\n\nServices:\n{service_string}"
 
     def post_init(self) -> None:
         context = AuthedServiceContext(
             node=self, credentials=self.signing_key.verify_key
         )
 
         if UserCodeService in self.services:
             user_code_service = self.get_service(UserCodeService)
             user_code_service.load_user_code(context=context)
         if self.is_subprocess:
             # print(f"> Starting Subprocess {self}")
             pass
         else:
-            print(f"> Starting {self}")
+            print(f"> {self}")
 
         def reload_user_code() -> None:
             user_code_service.load_user_code(context=context)
 
         CODE_RELOADER[thread_ident()] = reload_user_code
         # super().post_init()
 
@@ -391,15 +391,15 @@
                 MessageService,
                 ProjectService,
                 DataSubjectMemberService,
             ]
 
             if OBLV:
                 # relative
-                from ...external.oblv.oblv_service import OblvService
+                from ..external.oblv.oblv_service import OblvService
 
                 store_services += [OblvService]
 
             if service_klass in store_services:
                 kwargs["store"] = self.document_store
             self.service_path_map[service_klass.__name__.lower()] = service_klass(
                 **kwargs
@@ -444,15 +444,15 @@
     def icon(self) -> str:
         return "🦾"
 
     def __hash__(self) -> int:
         return hash(self.id)
 
     def __eq__(self, other: Any) -> bool:
-        if not isinstance(other, Worker):
+        if not isinstance(other, type(self)):
             return False
 
         if self.id != other.id:
             return False
 
         return True
 
@@ -602,40 +602,45 @@
     ) -> NodeServiceContext:
         return UnauthedServiceContext(node=self, login_credentials=login_credentials)
 
 
 def task_producer(
     pipe: _GIPCDuplexHandle, api_call: SyftAPICall, blocking: bool
 ) -> Any:
+    print("task_producer: Start")
+
     try:
         result = None
         with pipe:
             pipe.put(api_call)
             gevent.sleep(0)
             if blocking:
                 try:
                     result = pipe.get()
                 except EOFError:
                     pass
             pipe.close()
         if blocking:
+            print("task_producer: End")
             return result
     except gipc.gipc.GIPCClosed:
         pass
     except Exception as e:
         print("Exception in task_producer", e)
 
 
 def task_runner(
     pipe: _GIPCDuplexHandle,
     worker_settings: WorkerSettings,
     task_uid: UID,
     blocking: bool,
 ) -> None:
-    worker = Worker(
+    print("task_runner: Start")
+
+    worker = Node(
         id=worker_settings.id,
         name=worker_settings.name,
         signing_key=worker_settings.signing_key,
         document_store_config=worker_settings.document_store_config,
         action_store_config=worker_settings.action_store_config,
         is_subprocess=True,
     )
@@ -652,22 +657,25 @@
                 )
                 worker.queue_stash.set_result(item)
                 worker.queue_stash.partition.close()
             pipe.close()
     except Exception as e:
         print("Exception in task_runner", e)
         raise e
+    print("task_runner: End")
 
 
 def queue_task(
     api_call: SyftAPICall,
     worker_settings: WorkerSettings,
     task_uid: UID,
     blocking: bool,
 ) -> Optional[Any]:
+    print("queue_task: Start")
+
     with gipc.pipe(encoder=gipc_encoder, decoder=gipc_decoder, duplex=True) as (
         cend,
         pend,
     ):
         process = gipc.start_process(
             task_runner, args=(cend, worker_settings, task_uid, blocking)
         )
@@ -676,49 +684,53 @@
             process.join()
         except KeyboardInterrupt:
             producer.kill(block=True)
             process.terminate()
         process.join()
 
     if blocking:
+        print("queue_task: End")
         return producer.value
+    print("queue_task: End")
     return None
 
 
 def create_worker_metadata(
-    worker: NewNode,
+    worker: AbstractNode,
 ) -> Optional[NodeMetadata]:
     try:
         metadata_stash = MetadataStash(store=worker.document_store)
-        metadata_exists = metadata_stash.get_all().ok()
+        metadata_exists = metadata_stash.get_all(worker.signing_key.verify_key).ok()
         if metadata_exists:
             return None
         else:
             new_metadata = NodeMetadata(
                 name=worker.name,
                 id=worker.id,
                 verify_key=worker.signing_key.verify_key,
                 highest_object_version=HIGHEST_SYFT_OBJECT_VERSION,
                 lowest_object_version=LOWEST_SYFT_OBJECT_VERSION,
                 syft_version=__version__,
                 deployed_on=datetime.now().date().strftime("%m/%d/%Y"),
             )
-            result = metadata_stash.set(metadata=new_metadata)
+            result = metadata_stash.set(
+                credentials=worker.signing_key.verify_key, metadata=new_metadata
+            )
             if result.is_ok():
                 return result.ok()
             return None
     except Exception as e:
         print("create_worker_metadata failed", e)
 
 
 def create_admin_new(
     name: str,
     email: str,
     password: str,
-    node: NewNode,
+    node: AbstractNode,
 ) -> Optional[User]:
     try:
         user_stash = UserStash(store=node.document_store)
         row_exists = user_stash.get_by_email(
             credentials=node.signing_key.verify_key, email=email
         ).ok()
         if row_exists:
@@ -742,21 +754,21 @@
             else:
                 raise Exception(f"Could not create user: {result}")
     except Exception as e:
         print("Unable to create new admin", e)
 
 
 def create_oblv_key_pair(
-    worker: Worker,
+    worker: Node,
 ) -> Optional[str]:
     try:
         # relative
-        from ...external.oblv.oblv_keys_stash import OblvKeys
-        from ...external.oblv.oblv_keys_stash import OblvKeysStash
-        from ...external.oblv.oblv_service import generate_oblv_key
+        from ..external.oblv.oblv_keys_stash import OblvKeys
+        from ..external.oblv.oblv_keys_stash import OblvKeysStash
+        from ..external.oblv.oblv_service import generate_oblv_key
 
         oblv_keys_stash = OblvKeysStash(store=worker.document_store)
 
         if not len(oblv_keys_stash):
             public_key, private_key = generate_oblv_key(oblv_key_name=worker.name)
             oblv_keys = OblvKeys(public_key=public_key, private_key=private_key)
             res = oblv_keys_stash.set(worker.signing_key.verify_key, oblv_keys)
```

### Comparing `syft-0.8.0b8/src/syft/deploy.py` & `syft-0.8.0b9/src/syft/client/deploy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # stdlib
 from typing import Any
 
 # relative
-from .core.node.new.response import SyftError
+from ..service.response import SyftError
 
 
 class InstallOrchestra:
     def launch(self, *args: Any, **kwargs: Any) -> None:
         return self.error()
 
     def error(self) -> Any:
@@ -22,11 +22,11 @@
         # third party
         from hagrid import Orchestra
 
         return Orchestra
 
     except Exception:  # nosec
         pass
-    return InstallOrchestra
+    return InstallOrchestra()
 
 
 Orchestra = import_orchestra()
```

### Comparing `syft-0.8.0b8/src/syft/experimental_flags.py` & `syft-0.8.0b9/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/external/__init__.py` & `syft-0.8.0b9/src/syft/external/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 # stdlib
 import importlib
 import os
 from typing import Union
 
 # relative
-from ..core.node.new.response import SyftError
-from ..core.node.new.response import SyftSuccess
-from ..util import str_to_bool
+from ..service.response import SyftError
+from ..service.response import SyftSuccess
+from ..util.util import str_to_bool
 
 # Contains all the external libraries that Syft supports.
 # Used to check if a library is supported
 # if the external library is not installed, we prompt the user
 # to install it with the pip package name.
 
 OBLV = str_to_bool(os.getenv("ENABLE_OBLV", "false"))
```

### Comparing `syft-0.8.0b8/src/syft/external/oblv/__init__.py` & `syft-0.8.0b9/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/external/oblv/deployment.py` & `syft-0.8.0b9/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/external/oblv/deployment_client.py` & `syft-0.8.0b9/src/syft/external/oblv/deployment_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,31 +19,31 @@
 # third party
 from oblv import OblvClient
 from pydantic import BaseModel
 from pydantic import validator
 import requests
 
 # relative
-from ...core.node.new.api import SyftAPI
-from ...core.node.new.client import HTTPConnection
-from ...core.node.new.client import Routes
-from ...core.node.new.client import SyftSigningKey
-from ...core.node.new.deserialize import _deserialize as deserialize
-from ...core.node.new.node_metadata import EnclaveMetadata
-from ...core.node.new.serializable import serializable
-from ...core.node.new.uid import UID
-from ...util import bcolors
+from ...client.api import SyftAPI
+from ...client.client import HTTPConnection
+from ...client.client import Routes
+from ...client.client import SyftSigningKey
+from ...serde.deserialize import _deserialize as deserialize
+from ...serde.serializable import serializable
+from ...service.metadata.node_metadata import EnclaveMetadata
+from ...types.uid import UID
+from ...util.util import bcolors
 from .constants import LOCAL_MODE
 from .exceptions import OblvEnclaveError
 from .exceptions import OblvUnAuthorizedError
 from .oblv_proxy import check_oblv_proxy_installation_status
 
 if TYPE_CHECKING:
     # relative
-    from ...core.node.new.user_code import SubmitUserCode
+    from ...service.code.user_code import SubmitUserCode
 
 
 @serializable()
 class OblvMetadata(EnclaveMetadata, BaseModel):
     """Contains Metadata to connect to Oblivious Enclave"""
 
     class Config:
@@ -261,15 +261,15 @@
             raise OblvEnclaveError(
                 f"Failed to perform the operation  with status {req.status_code}, {req.content!r}"
             )
         return "Failed"
 
     def request_code_execution(self, code: SubmitUserCode) -> Any:
         # relative
-        from ...core.node.new.user_code import SubmitUserCode
+        from ...service.code.user_code import SubmitUserCode
 
         if not isinstance(code, SubmitUserCode):
             raise Exception(
                 f"The input code should be of type: {SubmitUserCode} got:{type(code)}"
             )
 
         enclave_metadata = OblvMetadata(
```

### Comparing `syft-0.8.0b8/src/syft/external/oblv/exceptions.py` & `syft-0.8.0b9/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/external/oblv/oblv_keys.py` & `syft-0.8.0b9/src/syft/external/oblv/oblv_keys.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.0b9/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.0b9/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/external/oblv/oblv_service.py` & `syft-0.8.0b9/src/syft/external/oblv/oblv_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/filterwarnings.py` & `syft-0.8.0b9/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/gevent_patch.py` & `syft-0.8.0b9/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/logger.py` & `syft-0.8.0b9/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/registry.py` & `syft-0.8.0b9/src/syft/client/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 from typing import Union
 
 # third party
 import pandas as pd
 import requests
 
 # relative
-from .core.node.new.grid_url import GridURL
-from .core.node.new.network_service import NodePeer
-from .core.node.new.node_metadata import NodeMetadataJSON
-from .logger import error
-from .logger import warning
+from ..service.metadata.node_metadata import NodeMetadataJSON
+from ..service.network.network_service import NodePeer
+from ..types.grid_url import GridURL
+from ..util.logger import error
+from ..util.logger import warning
 
 if TYPE_CHECKING:
     # relative
-    from .core.node.common.client import Client
+    from .client import Client
 
 NETWORK_REGISTRY_URL = (
     "https://raw.githubusercontent.com/OpenMined/NetworkRegistry/main/gateways.json"
 )
 NETWORK_REGISTRY_REPO = "https://github.com/OpenMined/NetworkRegistry"
 
 
@@ -107,15 +107,15 @@
         if len(on) == 0:
             return "(no gateways online - try syft.gateways.all_gateways to see offline gateways)"
         return pd.DataFrame(on).to_string()
 
     @staticmethod
     def create_client(network: Dict[str, Any]) -> Client:  # type: ignore
         # relative
-        from .core.node.new.client import connect
+        from ..client.client import connect
 
         try:
             port = int(network["port"])
             protocol = network["protocol"]
             host_or_ip = network["host_or_ip"]
             grid_url = GridURL(port=port, protocol=protocol, host_or_ip=host_or_ip)
             client = connect(url=str(grid_url))
```

### Comparing `syft-0.8.0b8/src/syft/search.py` & `syft-0.8.0b9/src/syft/client/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # stdlib
 from typing import List
 from typing import Tuple
 from typing import Union
 
 # relative
-from .core.node.new.client import SyftClient
-from .core.node.new.dataset import Dataset
-from .core.node.new.network_service import NodePeer
-from .core.node.new.node_metadata import NodeMetadataJSON
-from .core.node.new.uid import UID
+from ..service.dataset.dataset import Dataset
+from ..service.metadata.node_metadata import NodeMetadataJSON
+from ..service.network.network_service import NodePeer
+from ..types.uid import UID
+from .client import SyftClient
 from .registry import DomainRegistry
 
 
 class SearchResults:
     def __init__(self, results: List[Tuple[SyftClient, List[Dataset]]]) -> None:
         self._dataset_client = {}
         self._datasets = []
```

### Comparing `syft-0.8.0b8/src/syft/telemetry.py` & `syft-0.8.0b9/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/trace_decorator.py` & `syft-0.8.0b9/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft/user_settings.py` & `syft-0.8.0b9/src/syft/client/user_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # future
 from __future__ import annotations
 
 # stdlib
 import os
 
 # relative
-from .core.node.new.decorators import singleton
+from ..util.decorators import singleton
 
 # TODO: Add this to a file in ~/.syft and add some ENV overrides
 tutorial_mode = bool(os.environ.get("SYFT_TUTORIAL_MODE", True))
 
 
 @singleton
 class UserSettings:
```

### Comparing `syft-0.8.0b8/src/syft/version_compare.py` & `syft-0.8.0b9/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b8/src/syft.egg-info/PKG-INFO` & `syft-0.8.0b9/src/syft.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.0b8
+Version: 0.8.0b9
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -17,74 +17,116 @@
 Provides-Extra: test_plugins
 Provides-Extra: oblv
 License-File: LICENSE
 
 <div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://pepy.tech/badge/syft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev" /></a> <a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
 <br /><br /></div>
 
-<img src="docs/img/title_syft_light.png#gh-light-mode-only" alt="Syft Logo" width="200px" />
-<img src="docs/img/title_syft_dark.png#gh-dark-mode-only" alt="Syft Logo" width="200px" />
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/title_syft_dark.png">
+  <img alt="Syft Logo" src="docs/img/title_syft_light.png" width="200px" />
+</picture>
 
 Perform `numpy`-like analysis on `data` that remains in `someone else's` server
 
 <div align="left">
-<img src="docs/img/header.png#gh-light-mode-only" alt="Syft Overview" width="100%" />
-<img src="docs/img/header.png#gh-dark-mode-only" alt="Syft Overview" width="100%" />
+<img alt="Syft Logo" src="docs/img/header.png" alt="Syft Overview" width="100%" />
 </div>
 
 # Quickstart
 
 ✅ `Linux` ✅ `macOS`\* ✅ `Windows`†‡
-<img src="docs/img/terminalizer.gif" width="50%" align="right" />
 
-1. Install our handy 🛵 cli tool which makes deploying a Domain or Network server a one-liner:  
+## Install syft on Python 3.8 - 3.10
+
+```bash
+$ pip install --pre syft -f https://whls.blob.core.windows.net/unstable/index.html
+```
+
+## Launch a python dev Domain
+
+```python
+# from Jupyter / Python
+import syft as sy
+sy.requires(">=0.8-beta")
+node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
+```
+
+```bash
+# or from the command line
+$ syft launch --name=my-domain --port=8080 --reset=True
+
+Starting syft-node server on 0.0.0.0:8080
+```
+
+## Connect with our Python Client
+
+```python
+import syft as sy
+sy.requires(">=0.8-beta")
+domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
+```
+
+## Deploy to a Container Engine or Cloud
+
+1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server a one-liner:  
    `pip install -U hagrid`
 
 2. Then run our interactive jupyter Install 🧙🏽‍♂️ Wizard<sup>BETA</sup>:  
    `hagrid quickstart`
 
-- In the tutorial you will learn how to install and deploy:  
-  `PySyft` = our `numpy`-like 🐍 Python library for computing on `private data` in someone else's `Domain`
+3. In the tutorial you will learn how to install and deploy:  
+   `PySyft` = our `numpy`-like 🐍 Python library for computing on `private data` in someone else's `Domain`
 
-  `PyGrid` = our 🐳 `docker` / `k8s` / 🐧 `vm` `Domain` & `Network` Servers where `private data` lives
+   `PyGrid` = our 🐳 `docker` / 🐧 `vm` `Domain` & `Gateway` Servers where `private data` lives
 
-- During quickstart we will deploy `PyGrid` to localhost with 🐳 `docker`, however 🛵 HAGrid can deploy to `k8s` or a 🐧 `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using 🔨 `ansible`†
+4. During quickstart we will deploy `PyGrid` to localhost with 🐳 `docker`, however 🛵 HAGrid can deploy to `podman` or a 🐧 `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using 🔨 `ansible`†
 
-3. Read our 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
-4. Ask Questions ❔ in `#support` on <a href="https://slack.openmined.org/">Slack</a>
+## Docs and Support
+
+- 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
+- `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
-- HAGrid Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
+- HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`  
   †`Windows` does not support `ansible`, preventing some remote deployment targets
-- PySyft Requires: 🐍 `python 3.8+` - Run: `pip install -U syft`  
-  \*`macOS` Apple Silicon users need cmake: `brew install cmake`  
+- PySyft 0.8 Requires: 🐍 `python 3.8 - 3.10` - Run: `pip install -U syft`  
+  \*`macOS` Apple Silicon users might need cmake: `brew install cmake`  
   ‡`Windows` users must run this first: `pip install jaxlib==0.3.14 -f https://whls.blob.core.windows.net/unstable/index.html`
-- PyGrid Requires: 🐳 `docker` / `k8s` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
+- PyGrid Requires: 🐳 `docker` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
 
 # Versions
 
-`0.8.0 beta` - `dev` branch 👈🏽  
-`0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>  
-`0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>  
-`0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix  
-`0.2.0` - `0.5.0` Deprecated
+`0.8.0` (Beta) - `dev` branch 👈🏽  
+`0.7.0` (Stable) - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
+
+Deprecated:
+
+- `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
+- `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
+- `0.2.0` - `0.5.0`
 
 PySyft and PyGrid use the same `version` and its best to match them up where possible. We release weekly betas which can be used in each context:
-PySyft: `pip install -U syft --pre`
-PyGrid: `hagrid launch ... tag=latest`
+
+PySyft (Stable): `pip install -U syft`  
+PyGrid (Stable) `hagrid launch ... tag=latest`
+
+PySyft (Beta): `pip install -U syft --pre`  
+PyGrid (Beta): `hagrid launch ... tag=beta`
 
 HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually the best.
 
 # What is Syft?
 
-<img align="right" src="docs/img/logo_big.png#gh-light-mode-only" alt="Syft" height="250" style="padding-left:30px;">
-
-<img align="right" src="docs/img/logo_big_dark.png#gh-dark-mode-only" alt="Syft" height="250" style="padding-left:30px;">
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_big_dark.png">
+  <img align="right" src="docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
+</picture>
 
 `Syft` is OpenMined's `open source` stack that provides `secure` and `private` Data Science in Python. Syft decouples `private data` from model training, using techniques like [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and integration with `Deep Learning` frameworks, so that you as a `Data Scientist` can maintain your current workflow while using these new `privacy-enhancing techniques`.
 
 ### Why should I use Syft?
 
 `Syft` allows a `Data Scientist` to ask `questions` about a `dataset` and, within `privacy limits` set by the `data owner`, get `answers` to those `questions`, all without obtaining a `copy` of the data itself. We call this process `Remote Data Science`. It means in a wide variety of `domains` across society, the current `risks` of sharing information (`copying` data) with someone such as, privacy invasion, IP theft and blackmail will no longer prevent the vast `benefits` such as innovation, insights and scientific discovery which secure access will provide.
 
@@ -177,52 +219,59 @@
 <tr>
 <th align="center">
 <img width="441" height="1">
 <p>🏰 Domain Server</p>
 </th>
 <th align="center">
 <img width="441" height="1">
-<p>🔗 Network Server</p>
+<p>🔗 Gateway Server</p>
 </th>
 </tr>
 <tr>
 <td valign="top">
 <!-- REMOVE THE BACKSLASHES -->
 
 Manages the `remote study` of the data by a `Data Scientist` and allows the `Data Owner` to manage the `data` and control the `privacy guarantees` of the subjects under study. It also acts as a `gatekeeper` for the `Data Scientist's` access to the data to compute and experiment with the results.
 
 </td>
 <td valign="top">
 <!-- REMOVE THE BACKSLASHES -->
 
-Provides services to a group of `Data Owners` and `Data Scientists`, such as dataset `search` and bulk `project approval` (legal / technical) to participate in a project. A network server acts as a bridge between it's members (`Domains`) and their subscribers (`Data Scientists`) and can provide access to a collection of `domains` at once.</td>
+Provides services to a group of `Data Owners` and `Data Scientists`, such as dataset `search` and bulk `project approval` (legal / technical) to participate in a project. A gateway server acts as a bridge between it's members (`Domains`) and their subscribers (`Data Scientists`) and can provide access to a collection of `domains` at once.</td>
 
 </tr>
 <tr>
 </table>
 
 # Community
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
-<img src="docs/img/panel_slack_title_light.png#gh-light-mode-only" alt="" width="100%" align="center" />
-<img src="docs/img/panel_slack_title_dark.png#gh-dark-mode-only" alt="" width="100%" align="center" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/panel_slack_title_dark.png">
+  <img src="docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
+</picture>
 
 <a href="https://slack.openmined.org/"><img src="docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
 
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
-<img src="docs/img/panel_title_videos_papers_light.png#gh-light-mode-only" alt="" width="100%" align="center" />
-<img src="docs/img/panel_title_videos_papers.png#gh-dark-mode-only" alt="" width="100%" align="center" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/panel_title_videos_papers.png">
+  <img src="docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
+</picture>
+
 <p align="left"><sub><sup>
 🎥 <a href="https://www.youtube.com/watch?v=qVf0tPBzr2k">PETs: Remote Data Science Unleashed - R gov 2021</a><br />
 🎥 <a href="https://youtu.be/sCoDWKTbh3s?list=PL_lsbAsL_o2BQKXG7mkGFA8LSApCnhljL">Introduction to Remote Data Science - PyTorch 2021</a><br />
 🎥 <a href="https://youtu.be/kzLeTz_vIeQ?list=PL_lsbAsL_o2BtOz6KUfUI_Zla6Rg5dmyc">The Future of AI Tools - PyTorch 2020</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=4zrU54VIK6k&t=1s">Privacy Preserving AI - MIT Deep Learning Series</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=Pr4erdusiW0">Privacy-Preserving Data Science - TWiML Talk #241</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=NJBBE_SN90A">Privacy Preserving AI - PyTorch Devcon 2019</a><br />
@@ -231,16 +280,19 @@
 📖 <a href="https://arxiv.org/pdf/1811.04017.pdf">A generic framework for privacy preserving deep ...</a>
 </sup></sup></p>
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
-<img src="docs/img/panel_padawan_title_light.png#gh-light-mode-only" alt="" width="100%" align="center" />
-<img src="docs/img/panel_padawan_title_dark.png#gh-dark-mode-only" alt="" width="100%" align="center" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/panel_padawan_title_dark.png">
+  <img src="docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
+</picture>
 
 <a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
 
 </div>
 </th>
 </tr>
 </table>
@@ -267,17 +319,20 @@
 </div>
 </th>
 </tr>
 </table>
 
 # Contributors
 
-OpenMined and Syft appreciates all contributors, if you would like to fix a bug or suggest a new feature, please see our [guidelines](https://openmined.github.io/PySyft/developer_guide/index.html).<br />  
-<img src="docs/img/contributors_light.jpg#gh-light-mode-only" alt="Contributors" width="100%" />
-<img src="docs/img/contributors_dark.jpg#gh-dark-mode-only" alt="Contributors" width="100%" />
+OpenMined and Syft appreciates all contributors, if you would like to fix a bug or suggest a new feature, please see our [guidelines](https://openmined.github.io/PySyft/developer_guide/index.html).<br />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/contributors_dark.jpg">
+  <img src="docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
+</picture>
 
 # Supporters
 
 <table border="0">
 <tr>
 <th align="center">
 <a href="https://sloan.org/"><img src="docs/img/logo_sloan.png" /></a>
@@ -294,32 +349,41 @@
 <th align="center">
 <a href="https://summerofcode.withgoogle.com/"><img src="docs/img/logo_gsoc.png" /></a>
 </th>
 <th align="center">
 <a href="https://developers.google.com/season-of-docs"><img src="docs/img/logo_gsod.png" /></a>
 </th>
 <th align="center">
-<img src="docs/img/logo_arkhn_light.png#gh-light-mode-only" />
-<img src="docs/img/logo_arkhn.png#gh-dark-mode-only" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_arkhn.png">
+  <img src="docs/img/logo_arkhn_light.png" />
+</picture>
+
 </th>
 <th align="center">
-<img src="docs/img/logo_cape_light.png#gh-light-mode-only" />
-<img src="docs/img/logo_cape.png#gh-dark-mode-only" />
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_cape.png">
+  <img src="docs/img/logo_cape_light.png" />
+</picture>
 </th>
 <th align="center">
 <a href="https://begin.ai/"><img src="docs/img/logo_begin.png" /></a>
 </th>
 </tr>
 </table>
 
 # Open Collective
 
 `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA. We are funded by our generous supporters on <a href="https://opencollective.com/openmined">Open Collective</a>. <br /><br />
-<img src="docs/img/opencollective_light.png#gh-light-mode-only" alt="Contributors" width="100%" />
-<img src="docs/img/opencollective_dark.png#gh-dark-mode-only" alt="Contributors" width="100%" />
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/opencollective_dark.png">
+  <img src="docs/img/opencollective_light.png" alt="Contributors" width="100%" />
+</picture>
 
 # Disclaimer
 
 Syft is under active development and is not yet ready for pilots on private data without our assistance. As early access participants, please contact us via [Slack](https://slack.openmined.org/) or email if you would like to ask a question or have a use case that you would like to discuss.
 
 # License
```

#### html2text {}

```diff
@@ -1,52 +1,62 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.0b8 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.0b9 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.8 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
 Provides-Extra: oblv License-File: LICENSE
 [https://pepy.tech/badge/syft] [https://badge.fury.io/py/syft.svg] [https://
 img.shields.io/badge/docker-images-blue?logo=docker] [https://github.com/
 OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev] [https:/
 /img.shields.io/badge/chat-on%20slack-purple?logo=slack] [https://
 img.shields.io/badge/read-docs-yellow?logo=mdbook]
 
-[Syft Logo] [Syft Logo] Perform `numpy`-like analysis on `data` that remains in
-`someone else's` server
-[Syft Overview] [Syft Overview]
-# Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ [docs/img/
-terminalizer.gif] 1. Install our handy ðµ cli tool which makes deploying a
-Domain or Network server a one-liner: `pip install -U hagrid` 2. Then run our
-interactive jupyter Install ð§ð½ââï¸ WizardBETA: `hagrid quickstart` -
-In the tutorial you will learn how to install and deploy: `PySyft` = our
-`numpy`-like ð Python library for computing on `private data` in someone
-else's `Domain` `PyGrid` = our ð³ `docker` / `k8s` / ð§ `vm` `Domain` &
-`Network` Servers where `private data` lives - During quickstart we will deploy
-`PyGrid` to localhost with ð³ `docker`, however ðµ HAGrid can deploy to
-`k8s` or a ð§ `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨
-`ansible`â  3. Read our ð Docs 4. Ask Questions â in `#support` on Slack
-# Install Notes - HAGrid Requires: ð `python` ð `git` - Run: `pip install
--U hagrid` - Interactive Install ð§ð½ââï¸ WizardBETA Requires ðµ
-`hagrid`: - Run: `hagrid quickstart` â `Windows` does not support `ansible`,
-preventing some remote deployment targets - PySyft Requires: ð `python 3.8+`
-- Run: `pip install -U syft` \*`macOS` Apple Silicon users need cmake: `brew
-install cmake` â¡`Windows` users must run this first: `pip install
-jaxlib==0.3.14 -f https://whls.blob.core.windows.net/unstable/index.html` -
-PyGrid Requires: ð³ `docker` / `k8s` or ð§ `ubuntu` VM - Run: `hagrid
-launch ...` # Versions `0.8.0 beta` - `dev` branch ðð½ `0.7.0` - Course_3
-Updated `0.6.0` - Course_3 `0.5.1` - Course_2 + M1 Hotfix `0.2.0` - `0.5.0`
-Deprecated PySyft and PyGrid use the same `version` and its best to match them
-up where possible. We release weekly betas which can be used in each context:
-PySyft: `pip install -U syft --pre` PyGrid: `hagrid launch ... tag=latest`
-HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually
-the best. # What is Syft? [Syft] [Syft] `Syft` is OpenMined's `open source`
-stack that provides `secure` and `private` Data Science in Python. Syft
+  [Syft Logo]  Perform `numpy`-like analysis on `data` that remains in `someone
+else's` server
+[Syft Logo]
+# Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ## Install syft on
+Python 3.8 - 3.10 ```bash $ pip install --pre syft -f https://
+whls.blob.core.windows.net/unstable/index.html ``` ## Launch a python dev
+Domain ```python # from Jupyter / Python import syft as sy sy.requires(">=0.8-
+beta") node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True,
+reset=True) ``` ```bash # or from the command line $ syft launch --name=my-
+domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:8080 ```
+## Connect with our Python Client ```python import syft as sy sy.requires
+(">=0.8-beta") domain_client = sy.login(port=8080, email="info@openmined.org",
+password="changethis") ``` ## Deploy to a Container Engine or Cloud 1. Install
+our handy ðµ cli tool which makes deploying a Domain or Gateway server a one-
+liner: `pip install -U hagrid` 2. Then run our interactive jupyter Install
+ð§ð½ââï¸ WizardBETA: `hagrid quickstart` 3. In the tutorial you will
+learn how to install and deploy: `PySyft` = our `numpy`-like ð Python
+library for computing on `private data` in someone else's `Domain` `PyGrid` =
+our ð³ `docker` / ð§ `vm` `Domain` & `Gateway` Servers where `private data`
+lives 4. During quickstart we will deploy `PyGrid` to localhost with ð³
+`docker`, however ðµ HAGrid can deploy to `podman` or a ð§ `ubuntu` VM on
+`azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨ `ansible`â  ## Docs and
+Support - ð Docs - `#support` on Slack # Install Notes - HAGrid 0.3
+Requires: ð `python` ð `git` - Run: `pip install -U hagrid` - Interactive
+Install ð§ð½ââï¸ WizardBETA Requires ðµ `hagrid`: - Run: `hagrid
+quickstart` â `Windows` does not support `ansible`, preventing some remote
+deployment targets - PySyft 0.8 Requires: ð `python 3.8 - 3.10` - Run: `pip
+install -U syft` \*`macOS` Apple Silicon users might need cmake: `brew install
+cmake` â¡`Windows` users must run this first: `pip install jaxlib==0.3.14 -
+f https://whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires:
+ð³ `docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.0`
+(Beta) - `dev` branch ðð½ `0.7.0` (Stable) - Course_3_Updated Deprecated:
+- `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix - `0.2.0` - `0.5.0`
+PySyft and PyGrid use the same `version` and its best to match them up where
+possible. We release weekly betas which can be used in each context: PySyft
+(Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch ... tag=latest`
+PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta): `hagrid launch ...
+tag=beta` HAGrid is a cli / deployment tool so the latest version of `hagrid`
+is usually the best. # What is Syft?   [Syft]  `Syft` is OpenMined's `open
+source` stack that provides `secure` and `private` Data Science in Python. Syft
 decouples `private data` from model training, using techniques like [Federated
 Learning](https://ai.googleblog.com/2017/04/federated-learning-
 collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/
 Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/
 wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and
 integration with `Deep Learning` frameworks, so that you as a `Data Scientist`
 can maintain your current workflow while using these new `privacy-enhancing
@@ -77,20 +87,20 @@
 |                 [Image]                  |                   [Image]                    |
 |_______ð¨ð»âð¼_Data|_______ð©ð½âð¬_Data_Sci|ntists
 | Provide `datasets` which they would like | Are end `users` who desire to perform        |
 |to make available for `study` by an       |`computations` or `answer` a specific         |
 |`outside party` they may or may not `fully|`question` using one or more data owners'     |
 |trust`_has_good_intentions._______________|`datasets`.___________________________________|
 |                     [Image]              |                        [Image]               |
-|________________ð°_Domain_Server____|__________________ð_Network_Server_____|
+|________________ð°_Domain_Server____|__________________ð_Gateway_Server_____|
 | Manages the `remote study` of the data by| Provides services to a group of `Data Owners`|
 |a `Data Scientist` and allows the `Data   |and `Data Scientists`, such as dataset        |
 |Owner` to manage the `data` and control   |`search` and bulk `project approval` (legal / |
 |the `privacy guarantees` of the subjects  |technical) to participate in a project. A     |
-|under study. It also acts as a            |network server acts as a bridge between it's  |
+|under study. It also acts as a            |gateway server acts as a bridge between it's  |
 |`gatekeeper` for the `Data Scientist's`   |members (`Domains`) and their subscribers     |
 |access to the data to compute and         |(`Data Scientists`) and can provide access to |
 |experiment_with_the_results.______________|a_collection_of_`domains`_at_once.____________|
 # Community
  ______________________________________________________________________________
 |[Image]|                           [Image]                            |[Image]|
 |       |                                                              |       |
@@ -105,22 +115,19 @@
 |_______|ð_A_generic_framework_for_privacy_preserving_deep_...__|_______|
 # Courses
  _______________________
 |[Image]|[Image]|[Image]|
 # Contributors OpenMined and Syft appreciates all contributors, if you would
 like to fix a bug or suggest a new feature, please see our [guidelines](https:/
 /openmined.github.io/PySyft/developer_guide/index.html).
-[Contributors] [Contributors] # Supporters
-                                                                                                      [docs/img/              [docs/img/
-  [docs/img/      [docs/img/     [docs/img/       [docs/img/       [docs/img/     [docs/img/   logo_arkhn_light.png#gh- logo_cape_light.png#gh-   [docs/img/
-logo_sloan.png] logo_meta.png] logo_torch.png] logo_udacity.png] logo_gsoc.png] logo_gsod.png] light-mode-only] [docs/  light-mode-only] [docs/ logo_begin.png]
-                                                                                                img/logo_arkhn.png#gh-   img/logo_cape.png#gh-
-                                                                                                   dark-mode-only]          dark-mode-only]
+  [Contributors]  # Supporters
+  [docs/img/      [docs/img/     [docs/img/       [docs/img/       [docs/img/     [docs/img/         [docs/img/            [docs/img/       [docs/img/
+logo_sloan.png] logo_meta.png] logo_torch.png] logo_udacity.png] logo_gsoc.png] logo_gsod.png] logo_arkhn_light.png] logo_cape_light.png] logo_begin.png]
 # Open Collective `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA.
 We are funded by our generous supporters on Open_Collective.
 
-[Contributors] [Contributors] # Disclaimer Syft is under active development and
-is not yet ready for pilots on private data without our assistance. As early
-access participants, please contact us via [Slack](https://slack.openmined.org/
-) or email if you would like to ask a question or have a use case that you
-would like to discuss. # License [Apache License 2.0](LICENSE)
+  [Contributors]  # Disclaimer Syft is under active development and is not yet
+ready for pilots on private data without our assistance. As early access
+participants, please contact us via [Slack](https://slack.openmined.org/) or
+email if you would like to ask a question or have a use case that you would
+like to discuss. # License [Apache License 2.0](LICENSE)
 Person_icons_created_by_Freepik_-_Flaticon
```

### Comparing `syft-0.8.0b8/src/syft.egg-info/requires.txt` & `syft-0.8.0b9/src/syft.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,32 +2,35 @@
 bcrypt==4.0.1
 flax==0.5.3
 forbiddenfruit==0.1.4
 gevent==22.10.2
 gipc==1.5.0
 jax==0.3.14
 jaxlib==0.3.14
-loguru==0.6.0
+loguru==0.7.0
 numpy==1.24.2
 opendp==0.6.2
 packaging>=21.0
 pandas==1.5.3
 pyarrow==11.0.0
 pycapnp==1.3.0
-pydantic[email]==1.10.6
+pydantic[email]==1.10.7
 pymongo==4.3.3
 pynacl==1.5.0
-redis==4.5.1
+redis==4.5.4
 requests==2.28.2
 RestrictedPython==6.0
 result==0.9.0
 tqdm==4.65.0
 typeguard==2.13.3
 typing_extensions==4.5.0
 sherlock[filelock,redis]==0.4.1
+uvicorn[standard]==0.21.1
+fastapi==0.95.1
+hagrid>=0.3
 opentelemetry-api==1.14.0
 opentelemetry-sdk==1.14.0
 opentelemetry-exporter-jaeger==1.14.0
 opentelemetry-instrumentation==0.35b0
 opentelemetry-instrumentation-requests==0.35b0
 
 [dev]
```

