# Comparing `tmp/opendal-0.32.0.tar.gz` & `tmp/opendal-0.33.0.tar.gz`

## Comparing `opendal-0.32.0.tar` & `opendal-0.33.0.tar`

### file list

```diff
@@ -1,249 +1,252 @@
--rw-r--r--   0        0        0     5623 1970-01-01 00:00:00.000000 opendal-0.32.0/local_dependencies/opendal/Cargo.toml
--rw-r--r--   0     1001      123    62800 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/CHANGELOG.md
--rw-r--r--   0     1001      123     1256 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/CONTRIBUTING.md
--rw-r--r--   0     1001      123     6635 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/README.md
--rw-r--r--   0     1001      123      378 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/benches/README.md
--rw-r--r--   0     1001      123      672 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/benches/ops/README.md
--rw-r--r--   0     1001      123      979 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/benches/ops/main.rs
--rw-r--r--   0     1001      123     5574 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/benches/ops/read.rs
--rw-r--r--   0     1001      123     2438 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/benches/ops/utils.rs
--rw-r--r--   0     1001      123     2163 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/benches/ops/write.rs
--rw-r--r--   0     1001      123     1832 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/examples/object.rs
--rw-r--r--   0     1001      123     1290 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/comparisons/mod.rs
--rw-r--r--   0     1001      123     7703 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
--rw-r--r--   0     1001      123     5241 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/concepts.rs
--rw-r--r--   0     1001      123      982 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/features.md
--rw-r--r--   0     1001      123    10798 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/internals/accessor.rs
--rw-r--r--   0     1001      123     1765 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/internals/layer.rs
--rw-r--r--   0     1001      123     3409 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/internals/mod.rs
--rw-r--r--   0     1001      123     1458 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/mod.rs
--rw-r--r--   0     1001      123     3436 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md
--rw-r--r--   0     1001      123     5329 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
--rw-r--r--   0     1001      123     4885 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
--rw-r--r--   0     1001      123     5428 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
--rw-r--r--   0     1001      123     3341 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
--rw-r--r--   0     1001      123     4425 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
--rw-r--r--   0     1001      123     2902 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
--rw-r--r--   0     1001      123    12349 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
--rw-r--r--   0     1001      123     2538 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
--rw-r--r--   0     1001      123     2347 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
--rw-r--r--   0     1001      123     2805 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
--rw-r--r--   0     1001      123     1803 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
--rw-r--r--   0     1001      123     4733 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
--rw-r--r--   0     1001      123     2184 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
--rw-r--r--   0     1001      123     5771 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
--rw-r--r--   0     1001      123     8563 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
--rw-r--r--   0     1001      123     3113 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
--rw-r--r--   0     1001      123     4321 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
--rw-r--r--   0     1001      123     1881 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
--rw-r--r--   0     1001      123     2926 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
--rw-r--r--   0     1001      123     2246 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
--rw-r--r--   0     1001      123     6523 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
--rw-r--r--   0     1001      123     4792 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
--rw-r--r--   0     1001      123    10091 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
--rw-r--r--   0     1001      123     2508 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
--rw-r--r--   0     1001      123     2670 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
--rw-r--r--   0     1001      123     8059 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
--rw-r--r--   0     1001      123     2472 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
--rw-r--r--   0     1001      123     4452 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
--rw-r--r--   0     1001      123     2534 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
--rw-r--r--   0     1001      123     3693 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
--rw-r--r--   0     1001      123     3255 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
--rw-r--r--   0     1001      123     4133 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
--rw-r--r--   0     1001      123     4408 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
--rw-r--r--   0     1001      123     4230 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
--rw-r--r--   0     1001      123     4392 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/mod.rs
--rw-r--r--   0     1001      123    22576 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/upgrade.md
--rw-r--r--   0     1001      123     6746 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/chaos.rs
--rw-r--r--   0     1001      123    17164 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/complete.rs
--rw-r--r--   0     1001      123    10078 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/concurrent_limit.rs
--rw-r--r--   0     1001      123    16344 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/error_context.rs
--rw-r--r--   0     1001      123    13631 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/immutable_index.rs
--rw-r--r--   0     1001      123    53193 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/logging.rs
--rw-r--r--   0     1001      123    12128 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/madsim.rs
--rw-r--r--   0     1001      123    32436 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/metrics.rs
--rw-r--r--   0     1001      123    13351 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/minitrace.rs
--rw-r--r--   0     1001      123     2117 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/mod.rs
--rw-r--r--   0     1001      123    25253 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/prometheus.rs
--rw-r--r--   0     1001      123    37956 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/retry.rs
--rw-r--r--   0     1001      123    12792 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/tracing.rs
--rw-r--r--   0     1001      123     3844 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/type_eraser.rs
--rw-r--r--   0     1001      123     3076 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/lib.rs
--rw-r--r--   0     1001      123    21038 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/accessor.rs
--rw-r--r--   0     1001      123     5164 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs
--rw-r--r--   0     1001      123     9291 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
--rw-r--r--   0     1001      123     1181 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
--rw-r--r--   0     1001      123     1548 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/mod.rs
--rw-r--r--   0     1001      123     1934 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/chrono_util.rs
--rw-r--r--   0     1001      123     6441 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/body.rs
--rw-r--r--   0     1001      123    10135 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
--rw-r--r--   0     1001      123    10534 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
--rw-r--r--   0     1001      123     5404 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/client.rs
--rw-r--r--   0     1001      123     3394 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/error.rs
--rw-r--r--   0     1001      123    10427 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/header.rs
--rw-r--r--   0     1001      123     2025 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/mod.rs
--rw-r--r--   0     1001      123     2962 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/uri.rs
--rw-r--r--   0     1001      123    11983 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/layer.rs
--rw-r--r--   0     1001      123     2020 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/mod.rs
--rw-r--r--   0     1001      123     4439 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/cursor.rs
--rw-r--r--   0     1001      123     2512 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/entry.rs
--rw-r--r--   0     1001      123     3666 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
--rw-r--r--   0     1001      123     1006 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
--rw-r--r--   0     1001      123    15332 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
--rw-r--r--   0     1001      123     4148 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
--rw-r--r--   0     1001      123     1686 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
--rw-r--r--   0     1001      123     4577 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs
--rw-r--r--   0     1001      123     1971 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/mod.rs
--rw-r--r--   0     1001      123     3509 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/page.rs
--rw-r--r--   0     1001      123    10680 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/read.rs
--rw-r--r--   0     1001      123     9260 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
--rw-r--r--   0     1001      123     6861 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
--rw-r--r--   0     1001      123     5968 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/write.rs
--rw-r--r--   0     1001      123     4077 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/operation.rs
--rw-r--r--   0     1001      123    11671 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/path.rs
--rw-r--r--   0     1001      123     6387 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/rps.rs
--rw-r--r--   0     1001      123     1396 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/serde_util.rs
--rw-r--r--   0     1001      123     1077 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/version.rs
--rw-r--r--   0     1001      123    27080 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azblob/backend.rs
--rw-r--r--   0     1001      123    10124 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azblob/batch.rs
--rw-r--r--   0     1001      123     9184 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azblob/core.rs
--rw-r--r--   0     1001      123     5821 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azblob/error.rs
--rw-r--r--   0     1001      123      913 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azblob/mod.rs
--rw-r--r--   0     1001      123    14196 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azblob/pager.rs
--rw-r--r--   0     1001      123     2251 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azblob/writer.rs
--rw-r--r--   0     1001      123    16283 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/backend.rs
--rw-r--r--   0     1001      123     9557 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/core.rs
--rw-r--r--   0     1001      123     3520 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/error.rs
--rw-r--r--   0     1001      123      900 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/mod.rs
--rw-r--r--   0     1001      123     5647 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/pager.rs
--rw-r--r--   0     1001      123     2945 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/writer.rs
--rw-r--r--   0     1001      123     3973 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/dashmap/backend.rs
--rw-r--r--   0     1001      123      859 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/dashmap/mod.rs
--rw-r--r--   0     1001      123    23336 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/fs/backend.rs
--rw-r--r--   0     1001      123     1424 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/fs/error.rs
--rw-r--r--   0     1001      123      884 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/fs/mod.rs
--rw-r--r--   0     1001      123     4430 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/fs/pager.rs
--rw-r--r--   0     1001      123     3744 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/fs/writer.rs
--rw-r--r--   0     1001      123    15980 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ftp/backend.rs
--rw-r--r--   0     1001      123     1808 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ftp/err.rs
--rw-r--r--   0     1001      123      894 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ftp/mod.rs
--rw-r--r--   0     1001      123     2504 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ftp/pager.rs
--rw-r--r--   0     1001      123     4206 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ftp/util.rs
--rw-r--r--   0     1001      123     2109 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ftp/writer.rs
--rw-r--r--   0     1001      123    18489 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/gcs/backend.rs
--rw-r--r--   0     1001      123    11118 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/gcs/core.rs
--rw-r--r--   0     1001      123     3463 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/gcs/error.rs
--rw-r--r--   0     1001      123      905 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/gcs/mod.rs
--rw-r--r--   0     1001      123    10014 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/gcs/pager.rs
--rw-r--r--   0     1001      123     2820 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/gcs/uri.rs
--rw-r--r--   0     1001      123     4503 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/gcs/writer.rs
--rw-r--r--   0     1001      123    20557 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ghac/backend.rs
--rw-r--r--   0     1001      123     1908 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ghac/error.rs
--rw-r--r--   0     1001      123      877 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ghac/mod.rs
--rw-r--r--   0     1001      123     2584 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ghac/writer.rs
--rw-r--r--   0     1001      123    15693 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/backend.rs
--rw-r--r--   0     1001      123     1497 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/error.rs
--rw-r--r--   0     1001      123      888 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/mod.rs
--rw-r--r--   0     1001      123     3315 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/pager.rs
--rw-r--r--   0     1001      123     3256 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/writer.rs
--rw-r--r--   0     1001      123    15552 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/http/backend.rs
--rw-r--r--   0     1001      123     1826 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/http/error.rs
--rw-r--r--   0     1001      123      265 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
--rw-r--r--   0     1001      123      865 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/http/mod.rs
--rw-r--r--   0     1001      123    16810 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/backend.rs
--rw-r--r--   0     1001      123     1871 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/error.rs
--rw-r--r--   0     1001      123     8200 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/ipld.rs
--rw-r--r--   0     1001      123      875 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/mod.rs
--rw-r--r--   0     1001      123     8689 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/backend.rs
--rw-r--r--   0     1001      123     3946 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/builder.rs
--rw-r--r--   0     1001      123     2790 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/error.rs
--rw-r--r--   0     1001      123      903 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/mod.rs
--rw-r--r--   0     1001      123     3819 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/pager.rs
--rw-r--r--   0     1001      123     2043 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/writer.rs
--rw-r--r--   0     1001      123     1074 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt
--rw-r--r--   0     1001      123     4713 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/memcached/ascii.rs
--rw-r--r--   0     1001      123     9954 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/memcached/backend.rs
--rw-r--r--   0     1001      123      875 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/memcached/mod.rs
--rw-r--r--   0     1001      123     4228 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/memory/backend.rs
--rw-r--r--   0     1001      123      857 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/memory/mod.rs
--rw-r--r--   0     1001      123     3459 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/mod.rs
--rw-r--r--   0     1001      123     7949 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/moka/backend.rs
--rw-r--r--   0     1001      123      853 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/moka/mod.rs
--rw-r--r--   0     1001      123    13398 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/obs/backend.rs
--rw-r--r--   0     1001      123     7025 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/obs/core.rs
--rw-r--r--   0     1001      123     3443 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/obs/error.rs
--rw-r--r--   0     1001      123      896 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/obs/mod.rs
--rw-r--r--   0     1001      123     6027 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/obs/pager.rs
--rw-r--r--   0     1001      123     2261 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/obs/writer.rs
--rw-r--r--   0     1001      123    18877 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/oss/backend.rs
--rw-r--r--   0     1001      123    21580 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/oss/core.rs
--rw-r--r--   0     1001      123     3358 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/oss/error.rs
--rw-r--r--   0     1001      123      896 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/oss/mod.rs
--rw-r--r--   0     1001      123     7006 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/oss/pager.rs
--rw-r--r--   0     1001      123     4256 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/oss/writer.rs
--rw-r--r--   0     1001      123    10492 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/redis/backend.rs
--rw-r--r--   0     1001      123      855 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/redis/mod.rs
--rw-r--r--   0     1001      123     5615 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/rocksdb/backend.rs
--rw-r--r--   0     1001      123      859 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/rocksdb/mod.rs
--rw-r--r--   0     1001      123    39372 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/s3/backend.rs
--rw-r--r--   0     1001      123     3395 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/s3/compatible_services.md
--rw-r--r--   0     1001      123    27531 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/s3/core.rs
--rw-r--r--   0     1001      123     3685 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/s3/error.rs
--rw-r--r--   0     1001      123      894 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/s3/mod.rs
--rw-r--r--   0     1001      123     7040 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/s3/pager.rs
--rw-r--r--   0     1001      123     4820 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/s3/writer.rs
--rw-r--r--   0     1001      123     5375 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/sled/backend.rs
--rw-r--r--   0     1001      123      854 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/sled/mod.rs
--rw-r--r--   0     1001      123    38770 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/backend.rs
--rw-r--r--   0     1001      123    29663 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/core.rs
--rw-r--r--   0     1001      123     3712 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/error.rs
--rw-r--r--   0     1001      123      902 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/mod.rs
--rw-r--r--   0     1001      123     7061 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/pager.rs
--rw-r--r--   0     1001      123     2844 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/writer.rs
--rw-r--r--   0     1001      123    20472 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/backend.rs
--rw-r--r--   0     1001      123     1743 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/error.rs
--rw-r--r--   0     1001      123      130 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
--rw-r--r--   0     1001      123      626 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
--rw-r--r--   0     1001      123      531 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
--rw-r--r--   0     1001      123    16965 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/list_response.rs
--rw-r--r--   0     1001      123      911 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/mod.rs
--rw-r--r--   0     1001      123     2532 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/pager.rs
--rw-r--r--   0     1001      123     2275 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/writer.rs
--rw-r--r--   0     1001      123    19320 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/backend.rs
--rw-r--r--   0     1001      123     4085 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/error.rs
--rw-r--r--   0     1001      123     4679 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/message.rs
--rw-r--r--   0     1001      123      907 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/mod.rs
--rw-r--r--   0     1001      123     2452 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/pager.rs
--rw-r--r--   0     1001      123     2285 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/writer.rs
--rw-r--r--   0     1001      123     2333 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/builder.rs
--rw-r--r--   0     1001      123     2494 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/entry.rs
--rw-r--r--   0     1001      123    10799 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/error.rs
--rw-r--r--   0     1001      123     6197 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/list.rs
--rw-r--r--   0     1001      123    15166 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/metadata.rs
--rw-r--r--   0     1001      123     1462 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/mod.rs
--rw-r--r--   0     1001      123     1747 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/mode.rs
--rw-r--r--   0     1001      123    23910 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs
--rw-r--r--   0     1001      123     8731 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/operator/builder.rs
--rw-r--r--   0     1001      123     3235 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/operator/metadata.rs
--rw-r--r--   0     1001      123     1098 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/operator/mod.rs
--rw-r--r--   0     1001      123    40763 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/operator/operator.rs
--rw-r--r--   0     1001      123    10255 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/ops.rs
--rw-r--r--   0     1001      123     9611 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/reader.rs
--rw-r--r--   0     1001      123     5852 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/scheme.rs
--rw-r--r--   0     1001      123     7643 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/writer.rs
--rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 opendal-0.32.0/Cargo.toml
--rw-r--r--   0     1001      123      709 2023-04-18 13:34:01.000000 opendal-0.32.0/.gitignore
--rw-r--r--   0     1001      123      982 2023-04-18 13:34:01.000000 opendal-0.32.0/README.md
--rw-r--r--   0     1001      123      765 2023-04-18 13:34:01.000000 opendal-0.32.0/benchmark/README.md
--rw-r--r--   0     1001      123     2426 2023-04-18 13:34:01.000000 opendal-0.32.0/benchmark/async_opendal_benchmark.py
--rw-r--r--   0     1001      123     2955 2023-04-18 13:34:01.000000 opendal-0.32.0/benchmark/async_origin_s3_benchmark_with_gevent.py
--rw-r--r--   0     1001      123     1665 2023-04-18 13:34:01.000000 opendal-0.32.0/pyproject.toml
--rw-r--r--   0     1001      123      866 2023-04-18 13:34:01.000000 opendal-0.32.0/python/opendal/__init__.py
--rw-r--r--   0     1001      123     2917 2023-04-18 13:34:01.000000 opendal-0.32.0/python/opendal/__init__.pyi
--rw-r--r--   0     1001      123    11963 2023-04-18 13:34:01.000000 opendal-0.32.0/src/asyncio.rs
--rw-r--r--   0     1001      123     3311 2023-04-18 13:34:01.000000 opendal-0.32.0/src/layers.rs
--rw-r--r--   0     1001      123    13929 2023-04-18 13:34:01.000000 opendal-0.32.0/src/lib.rs
--rw-r--r--   0     1001      123     1604 2023-04-18 13:34:01.000000 opendal-0.32.0/tests/binding.feature
--rw-r--r--   0     1001      123     2942 2023-04-18 13:34:01.000000 opendal-0.32.0/tests/steps/binding.py
--rw-r--r--   0     1001      123   117208 2023-04-18 13:34:01.000000 opendal-0.32.0/Cargo.lock
--rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 opendal-0.32.0/PKG-INFO
+-rw-r--r--   0        0        0     5737 1970-01-01 00:00:00.000000 opendal-0.33.0/local_dependencies/opendal/Cargo.toml
+-rw-r--r--   0     1001      123    64485 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/CHANGELOG.md
+-rw-r--r--   0     1001      123     1256 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     6635 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/README.md
+-rw-r--r--   0     1001      123      378 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/benches/README.md
+-rw-r--r--   0     1001      123      672 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/benches/ops/README.md
+-rw-r--r--   0     1001      123      979 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/benches/ops/main.rs
+-rw-r--r--   0     1001      123     5574 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/benches/ops/read.rs
+-rw-r--r--   0     1001      123     2438 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/benches/ops/utils.rs
+-rw-r--r--   0     1001      123     2163 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/benches/ops/write.rs
+-rw-r--r--   0     1001      123     1832 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/examples/object.rs
+-rw-r--r--   0     1001      123     1290 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/comparisons/mod.rs
+-rw-r--r--   0     1001      123     7682 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
+-rw-r--r--   0     1001      123     5241 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/concepts.rs
+-rw-r--r--   0     1001      123      982 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/features.md
+-rw-r--r--   0     1001      123    10880 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/internals/accessor.rs
+-rw-r--r--   0     1001      123     1765 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/internals/layer.rs
+-rw-r--r--   0     1001      123     3409 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/internals/mod.rs
+-rw-r--r--   0     1001      123     1458 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3436 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md
+-rw-r--r--   0     1001      123     5329 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
+-rw-r--r--   0     1001      123     4885 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
+-rw-r--r--   0     1001      123     5428 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
+-rw-r--r--   0     1001      123     3341 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
+-rw-r--r--   0     1001      123     4425 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
+-rw-r--r--   0     1001      123     2902 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
+-rw-r--r--   0     1001      123    12349 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
+-rw-r--r--   0     1001      123     2538 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
+-rw-r--r--   0     1001      123     2347 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
+-rw-r--r--   0     1001      123     2805 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
+-rw-r--r--   0     1001      123     1803 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
+-rw-r--r--   0     1001      123     4733 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
+-rw-r--r--   0     1001      123     2184 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
+-rw-r--r--   0     1001      123     5771 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
+-rw-r--r--   0     1001      123     8563 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
+-rw-r--r--   0     1001      123     3113 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
+-rw-r--r--   0     1001      123     4321 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
+-rw-r--r--   0     1001      123     1881 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
+-rw-r--r--   0     1001      123     2926 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
+-rw-r--r--   0     1001      123     2246 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
+-rw-r--r--   0     1001      123     6523 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
+-rw-r--r--   0     1001      123     4792 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
+-rw-r--r--   0     1001      123    10091 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
+-rw-r--r--   0     1001      123     2508 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
+-rw-r--r--   0     1001      123     2670 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
+-rw-r--r--   0     1001      123     8059 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
+-rw-r--r--   0     1001      123     2472 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
+-rw-r--r--   0     1001      123     4452 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
+-rw-r--r--   0     1001      123     2534 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
+-rw-r--r--   0     1001      123     3693 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
+-rw-r--r--   0     1001      123     3255 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
+-rw-r--r--   0     1001      123     4133 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
+-rw-r--r--   0     1001      123     4408 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
+-rw-r--r--   0     1001      123     4230 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
+-rw-r--r--   0     1001      123     4392 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/mod.rs
+-rw-r--r--   0     1001      123    23435 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/upgrade.md
+-rw-r--r--   0     1001      123     6746 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/chaos.rs
+-rw-r--r--   0     1001      123    19723 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/complete.rs
+-rw-r--r--   0     1001      123     9888 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/concurrent_limit.rs
+-rw-r--r--   0     1001      123    17355 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/error_context.rs
+-rw-r--r--   0     1001      123    13556 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/immutable_index.rs
+-rw-r--r--   0     1001      123    50969 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/logging.rs
+-rw-r--r--   0     1001      123    13497 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/madsim.rs
+-rw-r--r--   0     1001      123    31779 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/metrics.rs
+-rw-r--r--   0     1001      123    12877 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/minitrace.rs
+-rw-r--r--   0     1001      123     2205 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/mod.rs
+-rw-r--r--   0     1001      123    13882 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/oteltrace.rs
+-rw-r--r--   0     1001      123    24230 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/prometheus.rs
+-rw-r--r--   0     1001      123    37745 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/retry.rs
+-rw-r--r--   0     1001      123    12402 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/tracing.rs
+-rw-r--r--   0     1001      123     3844 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/type_eraser.rs
+-rw-r--r--   0     1001      123     3001 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/lib.rs
+-rw-r--r--   0     1001      123    18458 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/accessor.rs
+-rw-r--r--   0     1001      123     5049 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs
+-rw-r--r--   0     1001      123     9348 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
+-rw-r--r--   0     1001      123     1181 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
+-rw-r--r--   0     1001      123     1548 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/mod.rs
+-rw-r--r--   0     1001      123     1934 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/chrono_util.rs
+-rw-r--r--   0     1001      123     6512 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/body.rs
+-rw-r--r--   0     1001      123    10135 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
+-rw-r--r--   0     1001      123    10534 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
+-rw-r--r--   0     1001      123     5578 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/client.rs
+-rw-r--r--   0     1001      123     3394 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/error.rs
+-rw-r--r--   0     1001      123    10427 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/header.rs
+-rw-r--r--   0     1001      123     2025 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/mod.rs
+-rw-r--r--   0     1001      123     2962 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/uri.rs
+-rw-r--r--   0     1001      123    11983 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/layer.rs
+-rw-r--r--   0     1001      123     1950 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/mod.rs
+-rw-r--r--   0     1001      123     8881 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/cursor.rs
+-rw-r--r--   0     1001      123     2512 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/entry.rs
+-rw-r--r--   0     1001      123     3666 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1006 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
+-rw-r--r--   0     1001      123    15397 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
+-rw-r--r--   0     1001      123     4148 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1686 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
+-rw-r--r--   0     1001      123     4577 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs
+-rw-r--r--   0     1001      123     2001 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/mod.rs
+-rw-r--r--   0     1001      123     3509 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/page.rs
+-rw-r--r--   0     1001      123    10680 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/read.rs
+-rw-r--r--   0     1001      123     9182 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
+-rw-r--r--   0     1001      123     6861 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
+-rw-r--r--   0     1001      123     5198 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/write.rs
+-rw-r--r--   0     1001      123     4081 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/operation.rs
+-rw-r--r--   0     1001      123    11671 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/path.rs
+-rw-r--r--   0     1001      123     6387 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/rps.rs
+-rw-r--r--   0     1001      123     1396 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/serde_util.rs
+-rw-r--r--   0     1001      123     1077 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/version.rs
+-rw-r--r--   0     1001      123    27973 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azblob/backend.rs
+-rw-r--r--   0     1001      123    10124 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azblob/batch.rs
+-rw-r--r--   0     1001      123    10574 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azblob/core.rs
+-rw-r--r--   0     1001      123     5821 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azblob/error.rs
+-rw-r--r--   0     1001      123      913 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azblob/mod.rs
+-rw-r--r--   0     1001      123    14196 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azblob/pager.rs
+-rw-r--r--   0     1001      123     2079 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azblob/writer.rs
+-rw-r--r--   0     1001      123    16278 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/backend.rs
+-rw-r--r--   0     1001      123     9557 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/core.rs
+-rw-r--r--   0     1001      123     3520 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/error.rs
+-rw-r--r--   0     1001      123      900 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/mod.rs
+-rw-r--r--   0     1001      123     5647 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/pager.rs
+-rw-r--r--   0     1001      123     2736 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/writer.rs
+-rw-r--r--   0     1001      123     4046 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/dashmap/backend.rs
+-rw-r--r--   0     1001      123      859 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/dashmap/mod.rs
+-rw-r--r--   0     1001      123    23295 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/fs/backend.rs
+-rw-r--r--   0     1001      123     1424 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/fs/error.rs
+-rw-r--r--   0     1001      123      884 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/fs/mod.rs
+-rw-r--r--   0     1001      123     4430 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/fs/pager.rs
+-rw-r--r--   0     1001      123     3092 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/fs/writer.rs
+-rw-r--r--   0     1001      123    16606 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ftp/backend.rs
+-rw-r--r--   0     1001      123     1808 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ftp/err.rs
+-rw-r--r--   0     1001      123      894 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ftp/mod.rs
+-rw-r--r--   0     1001      123     2504 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ftp/pager.rs
+-rw-r--r--   0     1001      123     4206 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ftp/util.rs
+-rw-r--r--   0     1001      123     1900 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ftp/writer.rs
+-rw-r--r--   0     1001      123    17782 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/gcs/backend.rs
+-rw-r--r--   0     1001      123    11557 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/gcs/core.rs
+-rw-r--r--   0     1001      123     3463 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/gcs/error.rs
+-rw-r--r--   0     1001      123      905 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/gcs/mod.rs
+-rw-r--r--   0     1001      123    10014 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/gcs/pager.rs
+-rw-r--r--   0     1001      123     2820 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/gcs/uri.rs
+-rw-r--r--   0     1001      123     6187 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/gcs/writer.rs
+-rw-r--r--   0     1001      123    20642 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ghac/backend.rs
+-rw-r--r--   0     1001      123     1908 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ghac/error.rs
+-rw-r--r--   0     1001      123      877 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ghac/mod.rs
+-rw-r--r--   0     1001      123     2375 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ghac/writer.rs
+-rw-r--r--   0     1001      123    15656 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/backend.rs
+-rw-r--r--   0     1001      123     1497 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/error.rs
+-rw-r--r--   0     1001      123      888 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/mod.rs
+-rw-r--r--   0     1001      123     3315 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/pager.rs
+-rw-r--r--   0     1001      123     2549 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/writer.rs
+-rw-r--r--   0     1001      123    15962 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/http/backend.rs
+-rw-r--r--   0     1001      123     1826 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/http/error.rs
+-rw-r--r--   0     1001      123      265 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
+-rw-r--r--   0     1001      123      865 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/http/mod.rs
+-rw-r--r--   0     1001      123    16861 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/backend.rs
+-rw-r--r--   0     1001      123     1871 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/error.rs
+-rw-r--r--   0     1001      123     8200 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/ipld.rs
+-rw-r--r--   0     1001      123      875 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/mod.rs
+-rw-r--r--   0     1001      123     8716 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/backend.rs
+-rw-r--r--   0     1001      123     3946 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/builder.rs
+-rw-r--r--   0     1001      123     2790 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/error.rs
+-rw-r--r--   0     1001      123      903 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/mod.rs
+-rw-r--r--   0     1001      123     3819 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/pager.rs
+-rw-r--r--   0     1001      123     1834 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/writer.rs
+-rw-r--r--   0     1001      123     1074 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt
+-rw-r--r--   0     1001      123     4713 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/memcached/ascii.rs
+-rw-r--r--   0     1001      123    10057 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/memcached/backend.rs
+-rw-r--r--   0     1001      123      875 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/memcached/mod.rs
+-rw-r--r--   0     1001      123     4336 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/memory/backend.rs
+-rw-r--r--   0     1001      123      857 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/memory/mod.rs
+-rw-r--r--   0     1001      123     3459 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/mod.rs
+-rw-r--r--   0     1001      123     7999 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/moka/backend.rs
+-rw-r--r--   0     1001      123      853 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/moka/mod.rs
+-rw-r--r--   0     1001      123    13534 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/obs/backend.rs
+-rw-r--r--   0     1001      123     7081 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/obs/core.rs
+-rw-r--r--   0     1001      123     3443 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/obs/error.rs
+-rw-r--r--   0     1001      123      896 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/obs/mod.rs
+-rw-r--r--   0     1001      123     6027 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/obs/pager.rs
+-rw-r--r--   0     1001      123     2057 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/obs/writer.rs
+-rw-r--r--   0     1001      123    18746 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/oss/backend.rs
+-rw-r--r--   0     1001      123    22799 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/oss/core.rs
+-rw-r--r--   0     1001      123     3358 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/oss/error.rs
+-rw-r--r--   0     1001      123      896 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/oss/mod.rs
+-rw-r--r--   0     1001      123     7006 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/oss/pager.rs
+-rw-r--r--   0     1001      123     6946 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/oss/writer.rs
+-rw-r--r--   0     1001      123    10637 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/redis/backend.rs
+-rw-r--r--   0     1001      123      855 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/redis/mod.rs
+-rw-r--r--   0     1001      123     5664 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/rocksdb/backend.rs
+-rw-r--r--   0     1001      123      859 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/rocksdb/mod.rs
+-rw-r--r--   0     1001      123    39157 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/s3/backend.rs
+-rw-r--r--   0     1001      123     3395 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/s3/compatible_services.md
+-rw-r--r--   0     1001      123    28151 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/s3/core.rs
+-rw-r--r--   0     1001      123     3685 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/s3/error.rs
+-rw-r--r--   0     1001      123      894 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/s3/mod.rs
+-rw-r--r--   0     1001      123     7040 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/s3/pager.rs
+-rw-r--r--   0     1001      123     7529 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/s3/writer.rs
+-rw-r--r--   0     1001      123     5518 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/sled/backend.rs
+-rw-r--r--   0     1001      123      854 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/sled/mod.rs
+-rw-r--r--   0     1001      123    38885 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/backend.rs
+-rw-r--r--   0     1001      123    29663 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/core.rs
+-rw-r--r--   0     1001      123     3712 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/error.rs
+-rw-r--r--   0     1001      123      902 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/mod.rs
+-rw-r--r--   0     1001      123     7061 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/pager.rs
+-rw-r--r--   0     1001      123     2666 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/writer.rs
+-rw-r--r--   0     1001      123    20511 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/backend.rs
+-rw-r--r--   0     1001      123     1743 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/error.rs
+-rw-r--r--   0     1001      123      130 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
+-rw-r--r--   0     1001      123      626 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
+-rw-r--r--   0     1001      123      531 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
+-rw-r--r--   0     1001      123    16965 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/list_response.rs
+-rw-r--r--   0     1001      123      911 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/mod.rs
+-rw-r--r--   0     1001      123     2560 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/pager.rs
+-rw-r--r--   0     1001      123     2066 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/writer.rs
+-rw-r--r--   0     1001      123    19374 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/backend.rs
+-rw-r--r--   0     1001      123     4085 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/error.rs
+-rw-r--r--   0     1001      123     4679 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/message.rs
+-rw-r--r--   0     1001      123      907 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/mod.rs
+-rw-r--r--   0     1001      123     2452 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/pager.rs
+-rw-r--r--   0     1001      123     2076 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/writer.rs
+-rw-r--r--   0     1001      123     2333 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/builder.rs
+-rw-r--r--   0     1001      123     6381 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/capability.rs
+-rw-r--r--   0     1001      123     2494 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/entry.rs
+-rw-r--r--   0     1001      123    11590 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/error.rs
+-rw-r--r--   0     1001      123     6197 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/list.rs
+-rw-r--r--   0     1001      123    15166 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/metadata.rs
+-rw-r--r--   0     1001      123     1511 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/mod.rs
+-rw-r--r--   0     1001      123     1747 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/mode.rs
+-rw-r--r--   0     1001      123    24145 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs
+-rw-r--r--   0     1001      123     8731 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/operator/builder.rs
+-rw-r--r--   0     1001      123     3067 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/operator/metadata.rs
+-rw-r--r--   0     1001      123     1098 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/operator/mod.rs
+-rw-r--r--   0     1001      123    42195 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/operator/operator.rs
+-rw-r--r--   0     1001      123    10788 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/ops.rs
+-rw-r--r--   0     1001      123     9569 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/reader.rs
+-rw-r--r--   0     1001      123     5852 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/scheme.rs
+-rw-r--r--   0     1001      123    10180 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/writer.rs
+-rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 opendal-0.33.0/Cargo.toml
+-rw-r--r--   0     1001      123      709 2023-04-23 05:13:34.000000 opendal-0.33.0/.gitignore
+-rw-r--r--   0     1001      123      982 2023-04-23 05:13:34.000000 opendal-0.33.0/README.md
+-rw-r--r--   0     1001      123      765 2023-04-23 05:13:34.000000 opendal-0.33.0/benchmark/README.md
+-rw-r--r--   0     1001      123     2426 2023-04-23 05:13:34.000000 opendal-0.33.0/benchmark/async_opendal_benchmark.py
+-rw-r--r--   0     1001      123     2955 2023-04-23 05:13:34.000000 opendal-0.33.0/benchmark/async_origin_s3_benchmark_with_gevent.py
+-rw-r--r--   0     1001      123      917 2023-04-23 05:13:34.000000 opendal-0.33.0/examples/object.ipynb
+-rw-r--r--   0     1001      123     1665 2023-04-23 05:13:34.000000 opendal-0.33.0/pyproject.toml
+-rw-r--r--   0     1001      123      866 2023-04-23 05:13:34.000000 opendal-0.33.0/python/opendal/__init__.py
+-rw-r--r--   0     1001      123     2917 2023-04-23 05:13:34.000000 opendal-0.33.0/python/opendal/__init__.pyi
+-rw-r--r--   0     1001      123    11963 2023-04-23 05:13:34.000000 opendal-0.33.0/src/asyncio.rs
+-rw-r--r--   0     1001      123     3311 2023-04-23 05:13:34.000000 opendal-0.33.0/src/layers.rs
+-rw-r--r--   0     1001      123    13929 2023-04-23 05:13:34.000000 opendal-0.33.0/src/lib.rs
+-rw-r--r--   0     1001      123     1604 2023-04-23 05:13:34.000000 opendal-0.33.0/tests/binding.feature
+-rw-r--r--   0     1001      123     2942 2023-04-23 05:13:34.000000 opendal-0.33.0/tests/steps/binding.py
+-rw-r--r--   0     1001      123   117424 2023-04-23 05:13:34.000000 opendal-0.33.0/Cargo.lock
+-rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 opendal-0.33.0/PKG-INFO
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/Cargo.toml` & `opendal-0.33.0/local_dependencies/opendal/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.64"
-version= "0.32.0"
+version= "0.33.0"
 
 [package.metadata.docs.rs]
 all-features = true
 
 [features]
 default = [
   "rustls",
@@ -70,28 +70,29 @@
 # Enable all layers.
 layers-all = [
   "layers-chaos",
   "layers-metrics",
   "layers-prometheus",
   "layers-tracing",
   "layers-minitrace",
-  "layers-madsim",
 ]
 # Enable layers chaos support
 layers-chaos = ["dep:rand"]
 # Enable layers metrics support
 layers-metrics = ["dep:metrics"]
 # Enable layers prometheus support
 layers-prometheus = ["dep:prometheus"]
 # Enable layers madsim support
 layers-madsim = ["dep:madsim"]
 # Enable layers minitrace support.
 layers-minitrace = ["dep:minitrace"]
 # Enable layers tracing support.
 layers-tracing = ["dep:tracing"]
+# Enable layers oteltrace support.
+layers-otel-trace = ["dep:opentelemetry"]
 
 services-azblob = [
   "dep:reqsign",
   "reqsign?/services-azblob",
   "reqsign?/reqwest_request",
 ]
 services-azdfs = [
@@ -168,14 +169,15 @@
 log = "0.4"
 madsim = { version = "0.2.21", optional = true }
 md-5 = "0.10"
 metrics = { version = "0.20", optional = true }
 minitrace = { version = "0.4.0", optional = true }
 moka = { version = "0.10", optional = true, features = ["future"] }
 once_cell = "1"
+opentelemetry = { version = "0.19.0", optional = true }
 parking_lot = "0.12"
 percent-encoding = "2"
 pin-project = "1"
 prometheus = { version = "0.13", features = ["process"], optional = true }
 prost = { version = "0.11", optional = true }
 quick-xml = { version = "0.27", features = ["serialize", "overlapped-lists"] }
 rand = { version = "0.8", optional = true }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/CHANGELOG.md` & `opendal-0.33.0/local_dependencies/opendal/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,57 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](https://semver.org/).
 
+## [v0.33.0] - 2023-04-23
+
+### Added
+
+- feat: Add OpenTelemetry Trace Layer (#2001)
+- feat: add if_none_match support for azblob (#2035)
+- feat: add if_none_match/if_match for gcs (#2039)
+- feat: Add size check for sized writer (#2038)
+- feat(services/azblob): Add if-match support (#2037)
+- feat(core): add copy&rename to error_context layer (#2040)
+- feat: add if-match support for OSS (#2034)
+- feat: Bootstrap new (old) project oay (#2041)
+- feat(services/OSS): Add override_content_disposition support (#2043)
+- feat: add IF_MATCH for http (#2044)
+- feat: add IF_MATCH for http HEAD request (#2047)
+- feat: add cache control header for azblob and obs (#2049)
+- feat: Add capability for operation's variant and args (#2057)
+- feat(azblob): Add override_content_disposition support (#2065)
+- feat(core): test for read_with_override_content_composition (#2067)
+- feat(core): Add `start-after` support for list (#2071)
+
+### Changed
+
+- refactor: Polish Writer API by merging append and write together (#2036)
+- refactor(raw/http_util): Add url in error context (#2066)
+- refactor: Allow reusing the same operator to speed up tests (#2068)
+
+### Fixed
+
+- fix(bindings/ruby): use rb_sys_env to help find ruby for building (#2051)
+- fix: MadsimLayer should be able to built without cfg (#2059)
+- fix(services/s3): Ignore prefix if it's empty (#2064)
+
+### Docs
+
+- docs(bindings/python): ipynb examples for users (#2061)
+
+### CI
+
+- ci(bindings/nodejs): publish support `--provenance` (#2046)
+- ci: upgrade typos to 1.14.8 (#2055)
+- chore(bindings/C): ignore the formatting of auto-generated opendal.h (#2056)
+
 ## [v0.32.0] - 2023-04-18
 
 ### Added
 
 - feat: Add wasabi service implementation (#2004)
 - feat: improve the readability of oli command line error output (#2016)
 - feat: add If-Match Support for OpRead, OpWrite, OpStat (#2017)
@@ -1911,14 +1954,15 @@
 
 ## v0.0.1 - 2022-02-14
 
 ### Added
 
 Hello, OpenDAL!
 
+[v0.33.0]: https://github.com/apache/incubator-opendal/compare/v0.32.0...v0.33.0
 [v0.32.0]: https://github.com/apache/incubator-opendal/compare/v0.31.1...v0.32.0
 [v0.31.1]: https://github.com/apache/incubator-opendal/compare/v0.31.0...v0.31.1
 [v0.31.0]: https://github.com/apache/incubator-opendal/compare/v0.30.5...v0.31.0
 [v0.30.5]: https://github.com/apache/incubator-opendal/compare/v0.30.4...v0.30.5
 [v0.30.4]: https://github.com/apache/incubator-opendal/compare/v0.30.3...v0.30.4
 [v0.30.3]: https://github.com/apache/incubator-opendal/compare/v0.30.2...v0.30.3
 [v0.30.2]: https://github.com/apache/incubator-opendal/compare/v0.30.1...v0.30.2
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/CONTRIBUTING.md` & `opendal-0.33.0/local_dependencies/opendal/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/README.md` & `opendal-0.33.0/local_dependencies/opendal/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/benches/ops/README.md` & `opendal-0.33.0/local_dependencies/opendal/benches/ops/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/benches/ops/main.rs` & `opendal-0.33.0/local_dependencies/opendal/benches/ops/main.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/benches/ops/read.rs` & `opendal-0.33.0/local_dependencies/opendal/benches/ops/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/benches/ops/utils.rs` & `opendal-0.33.0/local_dependencies/opendal/benches/ops/utils.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/benches/ops/write.rs` & `opendal-0.33.0/local_dependencies/opendal/benches/ops/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/examples/object.rs` & `opendal-0.33.0/local_dependencies/opendal/examples/object.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/comparisons/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/docs/comparisons/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 | http    | Y *(read only)* | N                                       |
 | ipfs    | Y *(read only)* | N                                       |
 | ipmfs   | Y               | N                                       |
 | memory  | Y               | Y                                       |
 | obs     | Y               | N                                       |
 | s3      | Y               | Y                                       |
 
-opendal has an idea called [`AccessorCapability`][crate::raw::AccessorCapability], so it's services may have different capability sets. For example, opendal's `http` and `ipfs` are read only.
+opendal has an idea called [`Capability`][crate::Capability], so it's services may have different capability sets. For example, opendal's `http` and `ipfs` are read only.
 
 ### Features
 
 `opendal` and `object_store` have different visions, so they have different feature sets:
 
 | opendal   | object_store         | notes                                        |
 |-----------|----------------------|----------------------------------------------|
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/concepts.rs` & `opendal-0.33.0/local_dependencies/opendal/src/docs/concepts.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/features.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/features.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/internals/accessor.rs` & `opendal-0.33.0/local_dependencies/opendal/src/docs/internals/accessor.rs`

 * *Files 3% similar despite different names*

```diff
@@ -110,28 +110,31 @@
 //! - OpenDAL will erase those type at the final stage of Operator building. Please don't return dynamic trait object like `oio::Reader`.
 //! - Use `()` as type if the operation is not supported.
 //!
 //! ## API Style
 //!
 //! Every API of [`Accessor`] follows the same style:
 //!
-//! - All APIs have a unique [`Operation`] and [`AccessorCapability`]
+//! - All APIs have a unique [`Operation`] and [`Capability`]
 //! - All APIs are orthogonal and do not overlap with each other
 //! - Most APIs accept `path` and `OpXxx`, and returns `RpXxx`.
 //! - Most APIs have `async` and `blocking` variants, they share the same semantics but may have different underlying implementations.
 //!
-//! [`Accessor`] can declare their capabilities via [`AccessorInfo`]'s `set_capabilities`:
+//! [`Accessor`] can declare their capabilities via [`AccessorInfo`]'s `set_capability`:
 //!
 //! ```ignore
 //! impl Accessor for MyBackend {
 //!     fn metadata(&self) -> AccessorInfo {
-//!        use AccessorCapability::*;
-//!
-//!        let mut am = AccessorInfo::default();
-//!        am.set_capabilities(Read | Write | List | Scan | Presign | Batch);
+//!         let mut am = AccessorInfo::default();
+//!         am.set_capability(
+//!             Capability {
+//!                 read: true,
+//!                 write: true,
+//!                 ..Default::default()
+//!         });
 //!
 //!         am
 //!     }
 //! }
 //! ```
 //!
 //! Now that you have mastered [`Accessor`], let's go and implement our own backend!
@@ -287,21 +290,22 @@
 //!     type BlockingReader = ();
 //!     type Writer = ();
 //!     type BlockingWriter = ();
 //!     type Pager = ();
 //!     type BlockingPager = ();
 //!
 //!     fn metadata(&self) -> AccessorInfo {
-//!         use AccessorCapability::*;
-//!         use AccessorHint::*;
-//!
 //!         let mut am = AccessorInfo::default();
 //!         am.set_scheme(Scheme::Duck)
 //!             .set_root(&self.root)
-//!             .set_capabilities(Read);
+//!             .set_capability(
+//!                 Capability {
+//!                     read: true,
+//!                     ..Default::default()
+//!             });
 //!
 //!         am
 //!     }
 //!
 //!     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
 //!         gagaga!()
 //!     }
@@ -313,11 +317,11 @@
 //!
 //! What!? There are no Super Power Ducks? So sad, but never mind, we have
 //! really powerful storage services [here](https://github.com/apache/incubator-opendal/issues/5). Welcome to pick one to implement. I promise you won't
 //! have to `gagaga!()` this time.
 //!
 //! [`Accessor`]: crate::raw::Accessor
 //! [`Operation`]: crate::raw::Operation
-//! [`AccessorCapability`]: crate::raw::AccessorCapability
+//! [`Capability`]: crate::Capability
 //! [`AccessorInfo`]: crate::raw::AccessorInfo
 //! [`Scheme`]: crate::Scheme
 //! [`Builder`]: crate::Builder
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/internals/layer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/docs/internals/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/internals/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/docs/internals/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/docs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/docs/upgrade.md` & `opendal-0.33.0/local_dependencies/opendal/src/docs/upgrade.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# Upgrade to v0.33
+
+## Public API
+
+OpenDAL 0.33 has redesigned the `Writer` API, replacing all instances of `writer.append()` with `writer.write()`. For more information, please refer to [`Writer`](crate::Writer).
+
+## Raw API
+
+In addition to the redesign of the `Writer` API, we have removed `append` from `oio::Write`. Therefore, users who implement services and layers should also remove it.
+
+After v0.33 landing, services should handle `OpWrite::content_length` correctly by following these guidelines:
+
+- If the writer does not support uploading unsized data, return a response of `NotSupported` if content length is `None`.
+- Otherwise, continue writing data until either `close` or `abort` has been called.
+
+Furthermore, OpenDAL 0.33 introduces a new concept called `Capability` which replaces `AccessorCapability`. Services must adapt to this change.
+
 # Upgrade to v0.32
 
 OpenDAL 0.32 doesn't have much breaking changes.
 
 We changed `Accessor::create` into `Accessor::create_dir`. Only users who implement `Layer` need to change.
 
 # Upgrade to v0.31
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/layers/chaos.rs` & `opendal-0.33.0/local_dependencies/opendal/src/layers/chaos.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/layers/complete.rs` & `opendal-0.33.0/local_dependencies/opendal/src/layers/complete.rs`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 use std::fmt::Formatter;
 use std::io;
 use std::sync::Arc;
 use std::task::Context;
 use std::task::Poll;
 
 use async_trait::async_trait;
+use bytes::Bytes;
 
 use crate::ops::*;
 use crate::raw::oio::into_reader::RangeReader;
 use crate::raw::oio::to_flat_pager;
 use crate::raw::oio::to_hierarchy_pager;
 use crate::raw::oio::Entry;
 use crate::raw::oio::IntoStreamableReader;
@@ -147,18 +148,17 @@
 
 impl<A: Accessor> CompleteReaderAccessor<A> {
     async fn complete_reader(
         &self,
         path: &str,
         args: OpRead,
     ) -> Result<(RpRead, CompleteReader<A, A::Reader>)> {
-        let (seekable, streamable) = (
-            self.meta.hints().contains(AccessorHint::ReadSeekable),
-            self.meta.hints().contains(AccessorHint::ReadStreamable),
-        );
+        let capability = self.meta.capability();
+        let seekable = capability.read_can_seek;
+        let streamable = capability.read_can_next;
 
         let range = args.range();
         let (rp, r) = self.inner.read(path, args).await?;
         let content_length = rp.metadata().content_length();
 
         match (seekable, streamable) {
             (true, true) => Ok((rp, CompleteReader::AlreadyComplete(r))),
@@ -197,18 +197,17 @@
     }
 
     fn complete_blocking_reader(
         &self,
         path: &str,
         args: OpRead,
     ) -> Result<(RpRead, CompleteReader<A, A::BlockingReader>)> {
-        let (seekable, streamable) = (
-            self.meta.hints().contains(AccessorHint::ReadSeekable),
-            self.meta.hints().contains(AccessorHint::ReadStreamable),
-        );
+        let capability = self.meta.capability();
+        let seekable = capability.read_can_seek;
+        let streamable = capability.read_can_next;
 
         let (rp, r) = self.inner.blocking_read(path, args)?;
 
         match (seekable, streamable) {
             (true, true) => Ok((rp, CompleteReader::AlreadyComplete(r))),
             (true, false) => {
                 let r = oio::into_streamable_reader(r, 256 * 1024);
@@ -222,18 +221,16 @@
     }
 
     async fn complete_list(
         &self,
         path: &str,
         args: OpList,
     ) -> Result<(RpList, CompletePager<A, A::Pager>)> {
-        let (can_list, can_scan) = (
-            self.meta.capabilities().contains(AccessorCapability::List),
-            self.meta.capabilities().contains(AccessorCapability::Scan),
-        );
+        let capability = self.meta.capability();
+        let (can_list, can_scan) = (capability.list, capability.scan);
 
         if can_list {
             let (rp, p) = self.inner.list(path, args).await?;
             Ok((rp, CompletePager::AlreadyComplete(p)))
         } else if can_scan {
             let (_, p) = self.inner.scan(path, OpScan::new()).await?;
             let p = to_hierarchy_pager(p, path);
@@ -248,18 +245,16 @@
     }
 
     fn complete_blocking_list(
         &self,
         path: &str,
         args: OpList,
     ) -> Result<(RpList, CompletePager<A, A::BlockingPager>)> {
-        let (can_list, can_scan) = (
-            self.meta.capabilities().contains(AccessorCapability::List),
-            self.meta.capabilities().contains(AccessorCapability::Scan),
-        );
+        let capability = self.meta.capability();
+        let (can_list, can_scan) = (capability.list, capability.scan);
 
         if can_list {
             let (rp, p) = self.inner.blocking_list(path, args)?;
             Ok((rp, CompletePager::AlreadyComplete(p)))
         } else if can_scan {
             let (_, p) = self.inner.blocking_scan(path, OpScan::new())?;
             let p = to_hierarchy_pager(p, path);
@@ -274,18 +269,16 @@
     }
 
     async fn complete_scan(
         &self,
         path: &str,
         args: OpScan,
     ) -> Result<(RpScan, CompletePager<A, A::Pager>)> {
-        let (can_list, can_scan) = (
-            self.meta.capabilities().contains(AccessorCapability::List),
-            self.meta.capabilities().contains(AccessorCapability::Scan),
-        );
+        let capability = self.meta.capability();
+        let (can_list, can_scan) = (capability.list, capability.scan);
 
         if can_scan {
             let (rp, p) = self.inner.scan(path, args).await?;
             Ok((rp, CompletePager::AlreadyComplete(p)))
         } else if can_list {
             let p = to_flat_pager(self.inner.clone(), path, args.limit().unwrap_or(1000));
             Ok((RpScan::default(), CompletePager::NeedFlat(p)))
@@ -299,18 +292,16 @@
     }
 
     fn complete_blocking_scan(
         &self,
         path: &str,
         args: OpScan,
     ) -> Result<(RpScan, CompletePager<A, A::BlockingPager>)> {
-        let (can_list, can_scan) = (
-            self.meta.capabilities().contains(AccessorCapability::List),
-            self.meta.capabilities().contains(AccessorCapability::Scan),
-        );
+        let capability = self.meta.capability();
+        let (can_list, can_scan) = (capability.list, capability.scan);
 
         if can_scan {
             let (rp, p) = self.inner.blocking_scan(path, args)?;
             Ok((rp, CompletePager::AlreadyComplete(p)))
         } else if can_list {
             let p = to_flat_pager(self.inner.clone(), path, args.limit().unwrap_or(1000));
             Ok((RpScan::default(), CompletePager::NeedFlat(p)))
@@ -325,16 +316,16 @@
 }
 
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for CompleteReaderAccessor<A> {
     type Inner = A;
     type Reader = CompleteReader<A, A::Reader>;
     type BlockingReader = CompleteReader<A, A::BlockingReader>;
-    type Writer = A::Writer;
-    type BlockingWriter = A::BlockingWriter;
+    type Writer = CompleteWriter<A::Writer>;
+    type BlockingWriter = CompleteWriter<A::BlockingWriter>;
     type Pager = CompletePager<A, A::Pager>;
     type BlockingPager = CompletePager<A, A::BlockingPager>;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
@@ -361,19 +352,26 @@
                 let bit = m.bit();
                 m.with_bit(bit | Metakey::Complete)
             })
         })
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        self.inner.write(path, args).await
+        let size = args.content_length();
+        self.inner
+            .write(path, args)
+            .await
+            .map(|(rp, w)| (rp, CompleteWriter::new(w, size)))
     }
 
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
-        self.inner.blocking_write(path, args)
+        let size = args.content_length();
+        self.inner
+            .blocking_write(path, args)
+            .map(|(rp, w)| (rp, CompleteWriter::new(w, size)))
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         self.complete_list(path, args).await
     }
 
     fn blocking_list(&self, path: &str, args: OpList) -> Result<(RpList, Self::BlockingPager)> {
@@ -419,15 +417,15 @@
             AlreadyComplete(r) => r.poll_seek(cx, pos),
             NeedSeekable(r) => r.poll_seek(cx, pos),
             NeedStreamable(r) => r.poll_seek(cx, pos),
             NeedBoth(r) => r.poll_seek(cx, pos),
         }
     }
 
-    fn poll_next(&mut self, cx: &mut Context<'_>) -> Poll<Option<Result<bytes::Bytes>>> {
+    fn poll_next(&mut self, cx: &mut Context<'_>) -> Poll<Option<Result<Bytes>>> {
         use CompleteReader::*;
 
         match self {
             AlreadyComplete(r) => r.poll_next(cx),
             NeedSeekable(r) => r.poll_next(cx),
             NeedStreamable(r) => r.poll_next(cx),
             NeedBoth(r) => r.poll_next(cx),
@@ -456,15 +454,15 @@
         match self {
             AlreadyComplete(r) => r.seek(pos),
             NeedStreamable(r) => r.seek(pos),
             _ => unreachable!("not supported types of complete reader"),
         }
     }
 
-    fn next(&mut self) -> Option<Result<bytes::Bytes>> {
+    fn next(&mut self) -> Option<Result<Bytes>> {
         use CompleteReader::*;
 
         match self {
             AlreadyComplete(r) => r.next(),
             NeedStreamable(r) => r.next(),
             _ => unreachable!("not supported types of complete reader"),
         }
@@ -505,7 +503,112 @@
         match self {
             AlreadyComplete(p) => p.next(),
             NeedFlat(p) => p.next(),
             NeedHierarchy(p) => p.next(),
         }
     }
 }
+
+pub struct CompleteWriter<W> {
+    inner: W,
+    size: Option<u64>,
+    written: u64,
+}
+
+impl<W> CompleteWriter<W> {
+    pub fn new(inner: W, size: Option<u64>) -> CompleteWriter<W> {
+        CompleteWriter {
+            inner,
+            size,
+            written: 0,
+        }
+    }
+}
+
+#[async_trait]
+impl<W> oio::Write for CompleteWriter<W>
+where
+    W: oio::Write,
+{
+    async fn write(&mut self, bs: Bytes) -> Result<()> {
+        let n = bs.len();
+
+        if let Some(size) = self.size {
+            if self.written + n as u64 > size {
+                return Err(Error::new(
+                    ErrorKind::ContentTruncated,
+                    &format!(
+                        "writer got too much data, expect: {size}, actual: {}",
+                        self.written + n as u64
+                    ),
+                ));
+            }
+        }
+
+        self.inner.write(bs).await?;
+        self.written += n as u64;
+        Ok(())
+    }
+
+    async fn abort(&mut self) -> Result<()> {
+        self.inner.abort().await
+    }
+
+    async fn close(&mut self) -> Result<()> {
+        if let Some(size) = self.size {
+            if self.written < size {
+                return Err(Error::new(
+                    ErrorKind::ContentIncomplete,
+                    &format!(
+                        "writer got too less data, expect: {size}, actual: {}",
+                        self.written
+                    ),
+                ));
+            }
+        }
+
+        self.inner.close().await?;
+        Ok(())
+    }
+}
+
+impl<W> oio::BlockingWrite for CompleteWriter<W>
+where
+    W: oio::BlockingWrite,
+{
+    fn write(&mut self, bs: Bytes) -> Result<()> {
+        let n = bs.len();
+
+        if let Some(size) = self.size {
+            if self.written + n as u64 > size {
+                return Err(Error::new(
+                    ErrorKind::ContentTruncated,
+                    &format!(
+                        "writer got too much data, expect: {size}, actual: {}",
+                        self.written + n as u64
+                    ),
+                ));
+            }
+        }
+
+        self.inner.write(bs)?;
+        self.written += n as u64;
+        Ok(())
+    }
+
+    fn close(&mut self) -> Result<()> {
+        if let Some(size) = self.size {
+            if self.written < size {
+                return Err(Error::new(
+                    ErrorKind::ContentIncomplete,
+                    &format!(
+                        "writer got too less data, expect: {size}, actual: {}",
+                        self.written
+                    ),
+                ));
+            }
+        }
+
+        self.inner.close()?;
+        Ok(())
+    }
+}
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/layers/concurrent_limit.rs` & `opendal-0.33.0/local_dependencies/opendal/src/layers/concurrent_limit.rs`

 * *Files 2% similar despite different names*

```diff
@@ -312,36 +312,28 @@
 
 #[async_trait]
 impl<R: oio::Write> oio::Write for ConcurrentLimitWrapper<R> {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         self.inner.write(bs).await
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        self.inner.append(bs).await
-    }
-
     async fn abort(&mut self) -> Result<()> {
         self.inner.abort().await
     }
 
     async fn close(&mut self) -> Result<()> {
         self.inner.close().await
     }
 }
 
 impl<R: oio::BlockingWrite> oio::BlockingWrite for ConcurrentLimitWrapper<R> {
     fn write(&mut self, bs: Bytes) -> Result<()> {
         self.inner.write(bs)
     }
 
-    fn append(&mut self, bs: Bytes) -> Result<()> {
-        self.inner.append(bs)
-    }
-
     fn close(&mut self) -> Result<()> {
         self.inner.close()
     }
 }
 
 #[async_trait]
 impl<R: oio::Page> oio::Page for ConcurrentLimitWrapper<R> {
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/layers/error_context.rs` & `opendal-0.33.0/local_dependencies/opendal/src/layers/error_context.rs`

 * *Files 9% similar despite different names*

```diff
@@ -134,14 +134,38 @@
                 err.with_operation(Operation::Write)
                     .with_context("service", self.meta.scheme())
                     .with_context("path", path)
             })
             .await
     }
 
+    async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        self.inner
+            .copy(from, to, args)
+            .map_err(|err| {
+                err.with_operation(Operation::Copy)
+                    .with_context("service", self.meta.scheme())
+                    .with_context("from", from)
+                    .with_context("to", to)
+            })
+            .await
+    }
+
+    async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        self.inner
+            .rename(from, to, args)
+            .map_err(|err| {
+                err.with_operation(Operation::Rename)
+                    .with_context("service", self.meta.scheme())
+                    .with_context("from", from)
+                    .with_context("to", to)
+            })
+            .await
+    }
+
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         self.inner
             .stat(path, args)
             .map_err(|err| {
                 err.with_operation(Operation::Stat)
                     .with_context("service", self.meta.scheme())
                     .with_context("path", path)
@@ -280,14 +304,32 @@
             .map_err(|err| {
                 err.with_operation(Operation::BlockingWrite)
                     .with_context("service", self.meta.scheme())
                     .with_context("path", path)
             })
     }
 
+    fn blocking_copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        self.inner.blocking_copy(from, to, args).map_err(|err| {
+            err.with_operation(Operation::BlockingCopy)
+                .with_context("service", self.meta.scheme())
+                .with_context("from", from)
+                .with_context("to", to)
+        })
+    }
+
+    fn blocking_rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        self.inner.blocking_rename(from, to, args).map_err(|err| {
+            err.with_operation(Operation::BlockingRename)
+                .with_context("service", self.meta.scheme())
+                .with_context("from", from)
+                .with_context("to", to)
+        })
+    }
+
     fn blocking_stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         self.inner.blocking_stat(path, args).map_err(|err| {
             err.with_operation(Operation::BlockingStat)
                 .with_context("service", self.meta.scheme())
                 .with_context("path", path)
         })
     }
@@ -407,25 +449,17 @@
         self.inner.write(bs).await.map_err(|err| {
             err.with_operation(WriteOperation::Write)
                 .with_context("service", self.scheme)
                 .with_context("path", &self.path)
         })
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        self.inner.append(bs).await.map_err(|err| {
-            err.with_operation(WriteOperation::Append)
-                .with_context("service", self.scheme)
-                .with_context("path", &self.path)
-        })
-    }
-
     async fn abort(&mut self) -> Result<()> {
         self.inner.abort().await.map_err(|err| {
-            err.with_operation(WriteOperation::Append)
+            err.with_operation(WriteOperation::Abort)
                 .with_context("service", self.scheme)
                 .with_context("path", &self.path)
         })
     }
 
     async fn close(&mut self) -> Result<()> {
         self.inner.close().await.map_err(|err| {
@@ -441,22 +475,14 @@
         self.inner.write(bs).map_err(|err| {
             err.with_operation(WriteOperation::BlockingWrite)
                 .with_context("service", self.scheme)
                 .with_context("path", &self.path)
         })
     }
 
-    fn append(&mut self, bs: Bytes) -> Result<()> {
-        self.inner.append(bs).map_err(|err| {
-            err.with_operation(WriteOperation::BlockingAppend)
-                .with_context("service", self.scheme)
-                .with_context("path", &self.path)
-        })
-    }
-
     fn close(&mut self) -> Result<()> {
         self.inner.close().map_err(|err| {
             err.with_operation(WriteOperation::BlockingClose)
                 .with_context("service", self.scheme)
                 .with_context("path", &self.path)
         })
     }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/layers/immutable_index.rs` & `opendal-0.33.0/local_dependencies/opendal/src/layers/immutable_index.rs`

 * *Files 2% similar despite different names*

```diff
@@ -145,18 +145,18 @@
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
     /// Add list capabilities for underlying storage services.
     fn metadata(&self) -> AccessorInfo {
         let mut meta = self.inner.info();
-        meta.set_capabilities(
-            meta.capabilities() | AccessorCapability::List | AccessorCapability::Scan,
-        );
-        meta.set_hints(meta.hints());
+
+        let cap = meta.capability_mut();
+        cap.list = true;
+        cap.scan = true;
 
         meta
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         self.inner.read(path, args).await
     }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/layers/logging.rs` & `opendal-0.33.0/local_dependencies/opendal/src/layers/logging.rs`

 * *Files 2% similar despite different names*

```diff
@@ -823,40 +823,40 @@
     }
 
     fn blocking_rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
         debug!(
             target: LOGGING_TARGET,
             "service={} operation={} from={} to={} -> started",
             self.scheme,
-            Operation::BlockingMove,
+            Operation::BlockingRename,
             from,
             to,
         );
 
         self.inner
             .blocking_rename(from, to, args)
             .map(|v| {
                 debug!(
                     target: LOGGING_TARGET,
                     "service={} operation={} from={} to={} -> finished",
                     self.scheme,
-                    Operation::BlockingMove,
+                    Operation::BlockingRename,
                     from,
                     to,
                 );
                 v
             })
             .map_err(|err| {
                 if let Some(lvl) = self.err_level(&err) {
                     log!(
                         target: LOGGING_TARGET,
                         lvl,
                         "service={} operation={} from={} to={} -> {}: {err:?}",
                         self.scheme,
-                        Operation::BlockingMove,
+                        Operation::BlockingRename,
                         from,
                         to,
                         self.err_status(&err)
                     );
                 }
                 err
             })
@@ -1382,47 +1382,14 @@
                     )
                 }
                 Err(err)
             }
         }
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let size = bs.len();
-        match self.inner.append(bs).await {
-            Ok(_) => {
-                self.written += size as u64;
-                trace!(
-                    target: LOGGING_TARGET,
-                    "service={} operation={} path={} written={} -> data write {}B",
-                    self.scheme,
-                    WriteOperation::Append,
-                    self.path,
-                    self.written,
-                    size
-                );
-                Ok(())
-            }
-            Err(err) => {
-                if let Some(lvl) = self.failure_level {
-                    log!(
-                        target: LOGGING_TARGET,
-                        lvl,
-                        "service={} operation={} path={} written={} -> data write failed: {err:?}",
-                        self.scheme,
-                        WriteOperation::Append,
-                        self.path,
-                        self.written,
-                    )
-                }
-                Err(err)
-            }
-        }
-    }
-
     async fn abort(&mut self) -> Result<()> {
         match self.inner.abort().await {
             Ok(_) => {
                 trace!(
                     target: LOGGING_TARGET,
                     "service={} operation={} path={} written={} -> abort writer",
                     self.scheme,
@@ -1498,47 +1465,14 @@
                         self.path,
                         self.written,
                     )
                 }
                 Err(err)
             }
         }
-    }
-
-    fn append(&mut self, bs: Bytes) -> Result<()> {
-        let size = bs.len();
-        match self.inner.append(bs) {
-            Ok(_) => {
-                self.written += size as u64;
-                trace!(
-                    target: LOGGING_TARGET,
-                    "service={} operation={} path={} written={} -> data write {}B",
-                    self.scheme,
-                    WriteOperation::BlockingAppend,
-                    self.path,
-                    self.written,
-                    size
-                );
-                Ok(())
-            }
-            Err(err) => {
-                if let Some(lvl) = self.failure_level {
-                    log!(
-                        target: LOGGING_TARGET,
-                        lvl,
-                        "service={} operation={} path={} written={} -> data write failed: {err:?}",
-                        self.scheme,
-                        WriteOperation::BlockingAppend,
-                        self.path,
-                        self.written,
-                    )
-                }
-                Err(err)
-            }
-        }
     }
 
     fn close(&mut self) -> Result<()> {
         match self.inner.close() {
             Ok(_) => Ok(()),
             Err(err) => {
                 if let Some(lvl) = self.failure_level {
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/layers/madsim.rs` & `opendal-0.33.0/local_dependencies/opendal/src/layers/madsim.rs`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,36 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+// This module requires to be work under `cfg(madsim)` so we will allow
+// dead code and unused variables.
+#![allow(unused_imports)]
+#![allow(unused_variables)]
+#![allow(dead_code)]
+
+use std::any::Any;
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::io::Result;
 use std::io::SeekFrom;
 use std::net::SocketAddr;
 use std::sync::Arc;
 use std::sync::Mutex;
 use std::task::Context;
 use std::task::Poll;
 
 use async_trait::async_trait;
 use bytes::Bytes;
+#[cfg(madsim)]
 use madsim::net::Endpoint;
+#[cfg(madsim)]
 use madsim::net::Payload;
 
 use crate::ops::*;
 use crate::raw::oio;
 use crate::raw::oio::Entry;
 use crate::raw::*;
 use crate::*;
@@ -89,35 +98,52 @@
 /// ```
 /// To enable logging output, please set `RUSTFLAGS="--cfg madsim"`:
 /// ```shell
 /// RUSTFLAGS="--cfg madsim" cargo test
 /// ```
 #[derive(Debug, Copy, Clone)]
 pub struct MadsimLayer {
+    #[cfg(madsim)]
     addr: SocketAddr,
 }
 
 impl MadsimLayer {
+    /// Create new madsim layer
     pub fn new(endpoint: &str) -> Self {
-        Self {
-            addr: endpoint.parse().unwrap(),
+        #[cfg(madsim)]
+        {
+            Self {
+                addr: endpoint.parse().unwrap(),
+            }
+        }
+        #[cfg(not(madsim))]
+        {
+            unreachable!("madsim is not enabled")
         }
     }
 }
 
 impl<A: Accessor> Layer<A> for MadsimLayer {
     type LayeredAccessor = MadsimAccessor;
 
     fn layer(&self, _: A) -> Self::LayeredAccessor {
-        MadsimAccessor { addr: self.addr }
+        #[cfg(madsim)]
+        {
+            MadsimAccessor { addr: self.addr }
+        }
+        #[cfg(not(madsim))]
+        {
+            unreachable!("madsim is not enabled")
+        }
     }
 }
 
 #[derive(Debug)]
 pub struct MadsimAccessor {
+    #[cfg(madsim)]
     addr: SocketAddr,
 }
 
 #[async_trait]
 impl LayeredAccessor for MadsimAccessor {
     type Inner = ();
     type Reader = MadsimReader;
@@ -130,53 +156,73 @@
     fn inner(&self) -> &Self::Inner {
         &()
     }
 
     fn metadata(&self) -> AccessorInfo {
         let mut info = AccessorInfo::default();
         info.set_name("madsim");
-        info.set_capabilities(AccessorCapability::Read | AccessorCapability::Write);
+
+        info.set_capability(Capability {
+            read: true,
+            write: true,
+            ..Default::default()
+        });
+
         info
     }
 
     async fn read(&self, path: &str, args: OpRead) -> crate::Result<(RpRead, Self::Reader)> {
-        let req = Request::Read(path.to_string(), args);
-        let ep = Endpoint::connect(self.addr)
-            .await
-            .expect("fail to connect to sim server");
-        let (tx, mut rx) = ep
-            .connect1(self.addr)
-            .await
-            .expect("fail to connect1 to sim server");
-        tx.send(Box::new(req))
-            .await
-            .expect("fail to send request to sim server");
-        let resp = rx
-            .recv()
-            .await
-            .expect("fail to recv response from sim server");
-        let resp = resp
-            .downcast::<ReadResponse>()
-            .expect("fail to downcast response to ReadResponse");
-        let content_length = resp.data.as_ref().map(|b| b.len()).unwrap_or(0);
-        Ok((
-            RpRead::new(content_length as u64),
-            MadsimReader { data: resp.data },
-        ))
+        #[cfg(madsim)]
+        {
+            let req = Request::Read(path.to_string(), args);
+            let ep = Endpoint::connect(self.addr)
+                .await
+                .expect("fail to connect to sim server");
+            let (tx, mut rx) = ep
+                .connect1(self.addr)
+                .await
+                .expect("fail to connect1 to sim server");
+            tx.send(Box::new(req))
+                .await
+                .expect("fail to send request to sim server");
+            let resp = rx
+                .recv()
+                .await
+                .expect("fail to recv response from sim server");
+            let resp = resp
+                .downcast::<ReadResponse>()
+                .expect("fail to downcast response to ReadResponse");
+            let content_length = resp.data.as_ref().map(|b| b.len()).unwrap_or(0);
+            Ok((
+                RpRead::new(content_length as u64),
+                MadsimReader { data: resp.data },
+            ))
+        }
+        #[cfg(not(madsim))]
+        {
+            unreachable!("madsim is not enabled")
+        }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> crate::Result<(RpWrite, Self::Writer)> {
-        Ok((
-            RpWrite::default(),
-            MadsimWriter {
-                path: path.to_string(),
-                args,
-                addr: self.addr,
-            },
-        ))
+        #[cfg(madsim)]
+        {
+            Ok((
+                RpWrite::default(),
+                MadsimWriter {
+                    path: path.to_string(),
+                    args,
+                    addr: self.addr,
+                },
+            ))
+        }
+        #[cfg(not(madsim))]
+        {
+            unreachable!("madsim is not enabled")
+        }
     }
 
     async fn list(&self, path: &str, args: OpList) -> crate::Result<(RpList, Self::Pager)> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "will be supported in the future",
         ))
@@ -235,61 +281,64 @@
 }
 
 pub struct MadsimReader {
     data: Option<Bytes>,
 }
 
 impl oio::Read for MadsimReader {
-    fn poll_read(&mut self, _cx: &mut Context<'_>, buf: &mut [u8]) -> Poll<crate::Result<usize>> {
+    fn poll_read(&mut self, _: &mut Context<'_>, buf: &mut [u8]) -> Poll<crate::Result<usize>> {
         if let Some(ref data) = self.data {
             let len = data.len();
             buf[..len].copy_from_slice(data);
             Poll::Ready(Ok(len))
         } else {
             Poll::Ready(Ok(0))
         }
     }
 
-    fn poll_seek(&mut self, cx: &mut Context<'_>, pos: SeekFrom) -> Poll<crate::Result<u64>> {
+    fn poll_seek(&mut self, _: &mut Context<'_>, _: SeekFrom) -> Poll<crate::Result<u64>> {
         Poll::Ready(Err(Error::new(
             ErrorKind::Unsupported,
             "will be supported in the future",
         )))
     }
 
-    fn poll_next(&mut self, cx: &mut Context<'_>) -> Poll<Option<crate::Result<Bytes>>> {
+    fn poll_next(&mut self, _: &mut Context<'_>) -> Poll<Option<crate::Result<Bytes>>> {
         Poll::Ready(Some(Err(Error::new(
             ErrorKind::Unsupported,
             "will be supported in the future",
         ))))
     }
 }
 
 pub struct MadsimWriter {
+    #[cfg(madsim)]
     path: String,
+    #[cfg(madsim)]
     args: OpWrite,
+    #[cfg(madsim)]
     addr: SocketAddr,
 }
 
 #[async_trait]
 impl oio::Write for MadsimWriter {
     async fn write(&mut self, bs: Bytes) -> crate::Result<()> {
-        let req = Request::Write(self.path.to_string(), bs);
-        let ep = Endpoint::connect(self.addr).await?;
-        let (tx, mut rx) = ep.connect1(self.addr).await?;
-        tx.send(Box::new(req)).await?;
-        rx.recv().await?;
-        Ok(())
-    }
-
-    async fn append(&mut self, bs: Bytes) -> crate::Result<()> {
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "will be supported in the future",
-        ))
+        #[cfg(madsim)]
+        {
+            let req = Request::Write(self.path.to_string(), bs);
+            let ep = Endpoint::bind(self.addr).await?;
+            let (tx, mut rx) = ep.connect1(self.addr).await?;
+            tx.send(Box::new(req)).await?;
+            rx.recv().await?;
+            Ok(())
+        }
+        #[cfg(not(madsim))]
+        {
+            unreachable!("madsim is not enabled")
+        }
     }
 
     async fn abort(&mut self) -> crate::Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "will be supported in the future",
         ))
@@ -319,37 +368,45 @@
 }
 
 /// A simulated server.This an experimental feature, docs are not ready yet.
 #[derive(Default, Clone)]
 pub struct MadsimServer;
 
 impl MadsimServer {
+    /// Start serving as madsim server.
     pub async fn serve(addr: SocketAddr) -> Result<()> {
-        let ep = Endpoint::bind(addr).await?;
-        let service = Arc::new(SimService::default());
-        loop {
-            let (tx, mut rx, _) = ep.accept1().await?;
-            let service = service.clone();
-            madsim::task::spawn(async move {
-                let request = *rx
-                    .recv()
-                    .await?
-                    .downcast::<Request>()
-                    .expect("invalid request");
-                let response = match request {
-                    Request::Read(path, args) => {
-                        Box::new(service.read(&path, args).await) as Payload
-                    }
-                    Request::Write(path, args) => {
-                        Box::new(service.write(&path, args).await) as Payload
-                    }
-                };
-                tx.send(response).await?;
-                Ok(()) as Result<()>
-            });
+        #[cfg(madsim)]
+        {
+            let ep = Endpoint::bind(addr).await?;
+            let service = Arc::new(SimService::default());
+            loop {
+                let (tx, mut rx, _) = ep.accept1().await?;
+                let service = service.clone();
+                madsim::task::spawn(async move {
+                    let request = *rx
+                        .recv()
+                        .await?
+                        .downcast::<Request>()
+                        .expect("invalid request");
+                    let response = match request {
+                        Request::Read(path, args) => {
+                            Box::new(service.read(&path, args).await) as Payload
+                        }
+                        Request::Write(path, args) => {
+                            Box::new(service.write(&path, args).await) as Payload
+                        }
+                    };
+                    tx.send(response).await?;
+                    Ok(()) as Result<()>
+                });
+            }
+        }
+        #[cfg(not(madsim))]
+        {
+            unreachable!("madsim is not enabled")
         }
     }
 }
 
 enum Request {
     Read(String, OpRead),
     Write(String, Bytes),
@@ -379,14 +436,15 @@
 struct ReadResponse {
     data: Option<Bytes>,
 }
 
 struct WriteResponse {}
 
 #[cfg(test)]
+#[cfg(madsim)]
 mod test {
     use std::time::Duration;
 
     use madsim::runtime::Handle;
     use madsim::time::sleep;
 
     use super::*;
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/layers/metrics.rs` & `opendal-0.33.0/local_dependencies/opendal/src/layers/metrics.rs`

 * *Files 0% similar despite different names*

```diff
@@ -921,26 +921,14 @@
             .map(|_| self.bytes += size as u64)
             .map_err(|err| {
                 self.handle.increment_errors_total(self.op, err.kind());
                 err
             })
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let size = bs.len();
-        self.inner
-            .append(bs)
-            .await
-            .map(|_| self.bytes += size as u64)
-            .map_err(|err| {
-                self.handle.increment_errors_total(self.op, err.kind());
-                err
-            })
-    }
-
     async fn abort(&mut self) -> Result<()> {
         self.inner.abort().await.map_err(|err| {
             self.handle.increment_errors_total(self.op, err.kind());
             err
         })
     }
 
@@ -960,25 +948,14 @@
             .map(|_| self.bytes += size as u64)
             .map_err(|err| {
                 self.handle.increment_errors_total(self.op, err.kind());
                 err
             })
     }
 
-    fn append(&mut self, bs: Bytes) -> Result<()> {
-        let size = bs.len();
-        self.inner
-            .append(bs)
-            .map(|_| self.bytes += size as u64)
-            .map_err(|err| {
-                self.handle.increment_errors_total(self.op, err.kind());
-                err
-            })
-    }
-
     fn close(&mut self) -> Result<()> {
         self.inner.close().map_err(|err| {
             self.handle.increment_errors_total(self.op, err.kind());
             err
         })
     }
 }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/layers/minitrace.rs` & `opendal-0.33.0/local_dependencies/opendal/src/layers/minitrace.rs`

 * *Files 4% similar despite different names*

```diff
@@ -333,24 +333,14 @@
             .in_span(Span::enter_with_parent(
                 WriteOperation::Write.into_static(),
                 &self.span,
             ))
             .await
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        self.inner
-            .append(bs)
-            .in_span(Span::enter_with_parent(
-                WriteOperation::Append.into_static(),
-                &self.span,
-            ))
-            .await
-    }
-
     async fn abort(&mut self) -> Result<()> {
         self.inner
             .abort()
             .in_span(Span::enter_with_parent(
                 WriteOperation::Abort.into_static(),
                 &self.span,
             ))
@@ -371,20 +361,14 @@
 impl<R: oio::BlockingWrite> oio::BlockingWrite for MinitraceWrapper<R> {
     fn write(&mut self, bs: Bytes) -> Result<()> {
         let _span =
             Span::enter_with_parent(WriteOperation::BlockingWrite.into_static(), &self.span);
         self.inner.write(bs)
     }
 
-    fn append(&mut self, bs: Bytes) -> Result<()> {
-        let _span =
-            Span::enter_with_parent(WriteOperation::BlockingAppend.into_static(), &self.span);
-        self.inner.append(bs)
-    }
-
     fn close(&mut self) -> Result<()> {
         let _span =
             Span::enter_with_parent(WriteOperation::BlockingClose.into_static(), &self.span);
         self.inner.close()
     }
 }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/layers/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/layers/mod.rs`

 * *Files 5% similar despite different names*

```diff
@@ -60,16 +60,18 @@
 mod error_context;
 pub(crate) use error_context::ErrorContextLayer;
 
 mod complete;
 pub(crate) use complete::CompleteLayer;
 
 #[cfg(feature = "layers-madsim")]
-#[cfg(madsim)]
 mod madsim;
 
 #[cfg(feature = "layers-madsim")]
-#[cfg(madsim)]
 pub use self::madsim::MadsimLayer;
 #[cfg(feature = "layers-madsim")]
-#[cfg(madsim)]
 pub use self::madsim::MadsimServer;
+
+#[cfg(feature = "layers-otel-trace")]
+mod oteltrace;
+#[cfg(feature = "layers-otel-trace")]
+pub use self::oteltrace::OtelTraceLayer;
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/layers/prometheus.rs` & `opendal-0.33.0/local_dependencies/opendal/src/layers/prometheus.rs`

 * *Files 2% similar despite different names*

```diff
@@ -716,31 +716,14 @@
             })
             .map_err(|err| {
                 self.stats.increment_errors_total(self.op, err.kind());
                 err
             })
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let size = bs.len();
-        self.inner
-            .append(bs)
-            .await
-            .map(|_| {
-                self.stats
-                    .bytes_total
-                    .with_label_values(&[&self.scheme, Operation::Write.into_static()])
-                    .observe(size as f64)
-            })
-            .map_err(|err| {
-                self.stats.increment_errors_total(self.op, err.kind());
-                err
-            })
-    }
-
     async fn abort(&mut self) -> Result<()> {
         self.inner.abort().await.map_err(|err| {
             self.stats.increment_errors_total(self.op, err.kind());
             err
         })
     }
 
@@ -760,30 +743,14 @@
             .map(|_| {
                 self.stats
                     .bytes_total
                     .with_label_values(&[&self.scheme, Operation::BlockingWrite.into_static()])
                     .observe(size as f64)
             })
             .map_err(|err| {
-                self.stats.increment_errors_total(self.op, err.kind());
-                err
-            })
-    }
-
-    fn append(&mut self, bs: Bytes) -> Result<()> {
-        let size = bs.len();
-        self.inner
-            .append(bs)
-            .map(|_| {
-                self.stats
-                    .bytes_total
-                    .with_label_values(&[&self.scheme, Operation::BlockingWrite.into_static()])
-                    .observe(size as f64)
-            })
-            .map_err(|err| {
                 self.stats.increment_errors_total(self.op, err.kind());
                 err
             })
     }
 
     fn close(&mut self) -> Result<()> {
         self.inner.close().map_err(|err| {
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/layers/retry.rs` & `opendal-0.33.0/local_dependencies/opendal/src/layers/retry.rs`

 * *Files 1% similar despite different names*

```diff
@@ -243,14 +243,42 @@
                     "operation={} -> retry after {}s: error={:?}",
                     Operation::Delete, dur.as_secs_f64(), err)
             })
             .map(|v| v.map_err(|e| e.set_persistent()))
             .await
     }
 
+    async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        { || self.inner.copy(from, to, args.clone()) }
+            .retry(&self.builder)
+            .when(|e| e.is_temporary())
+            .notify(|err, dur| {
+                warn!(
+                    target: "opendal::service",
+                    "operation={} -> retry after {}s: error={:?}",
+                    Operation::Copy, dur.as_secs_f64(), err)
+            })
+            .map(|v| v.map_err(|e| e.set_persistent()))
+            .await
+    }
+
+    async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        { || self.inner.rename(from, to, args.clone()) }
+            .retry(&self.builder)
+            .when(|e| e.is_temporary())
+            .notify(|err, dur| {
+                warn!(
+                    target: "opendal::service",
+                    "operation={} -> retry after {}s: error={:?}",
+                    Operation::Rename, dur.as_secs_f64(), err)
+            })
+            .map(|v| v.map_err(|e| e.set_persistent()))
+            .await
+    }
+
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         { || self.inner.list(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
                 warn!(
                     target: "opendal::service",
@@ -647,48 +675,27 @@
                         continue;
                     }
                 },
             }
         }
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let mut backoff = self.builder.build();
-
-        loop {
-            match self.inner.append(bs.clone()).await {
-                Ok(v) => return Ok(v),
-                Err(e) if !e.is_temporary() => return Err(e),
-                Err(e) => match backoff.next() {
-                    None => return Err(e),
-                    Some(dur) => {
-                        warn!(target: "opendal::service",
-                              "operation={} path={} -> pager retry after {}s: error={:?}",
-                              WriteOperation::Append, self.path, dur.as_secs_f64(), e);
-                        tokio::time::sleep(dur).await;
-                        continue;
-                    }
-                },
-            }
-        }
-    }
-
     async fn abort(&mut self) -> Result<()> {
         let mut backoff = self.builder.build();
 
         loop {
             match self.inner.abort().await {
                 Ok(v) => return Ok(v),
                 Err(e) if !e.is_temporary() => return Err(e),
                 Err(e) => match backoff.next() {
                     None => return Err(e),
                     Some(dur) => {
                         warn!(target: "opendal::service",
                               "operation={} path={} -> pager retry after {}s: error={:?}",
-                              WriteOperation::Append, self.path, dur.as_secs_f64(), e);
+                              WriteOperation::Abort, self.path, dur.as_secs_f64(), e);
                         tokio::time::sleep(dur).await;
                         continue;
                     }
                 },
             }
         }
     }
@@ -726,28 +733,14 @@
                 "operation={} -> pager retry after {}s: error={:?}",
                 WriteOperation::BlockingWrite, dur.as_secs_f64(), err)
             })
             .call()
             .map_err(|e| e.set_persistent())
     }
 
-    fn append(&mut self, bs: Bytes) -> Result<()> {
-        { || self.inner.append(bs.clone()) }
-            .retry(&self.builder)
-            .when(|e| e.is_temporary())
-            .notify(move |err, dur| {
-                warn!(
-                target: "opendal::service",
-                "operation={} -> pager retry after {}s: error={:?}",
-                WriteOperation::BlockingAppend, dur.as_secs_f64(), err)
-            })
-            .call()
-            .map_err(|e| e.set_persistent())
-    }
-
     fn close(&mut self) -> Result<()> {
         { || self.inner.close() }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(move |err, dur| {
                 warn!(
                 target: "opendal::service",
@@ -847,16 +840,19 @@
         type Writer = ();
         type BlockingWriter = ();
         type Pager = MockPager;
         type BlockingPager = ();
 
         fn info(&self) -> AccessorInfo {
             let mut am = AccessorInfo::default();
-            am.set_capabilities(AccessorCapability::List | AccessorCapability::Batch);
-            am.set_hints(AccessorHint::ReadStreamable);
+            am.set_capability(Capability {
+                list: true,
+                batch: true,
+                ..Default::default()
+            });
 
             am
         }
 
         async fn read(&self, _: &str, _: OpRead) -> Result<(RpRead, Self::Reader)> {
             Ok((
                 RpRead::new(13),
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/layers/tracing.rs` & `opendal-0.33.0/local_dependencies/opendal/src/layers/tracing.rs`

 * *Files 3% similar despite different names*

```diff
@@ -344,22 +344,14 @@
         self.inner.write(bs).await
     }
 
     #[tracing::instrument(
         parent = &self.span,
         level = "trace",
         skip_all)]
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        self.inner.append(bs).await
-    }
-
-    #[tracing::instrument(
-        parent = &self.span,
-        level = "trace",
-        skip_all)]
     async fn abort(&mut self) -> Result<()> {
         self.inner.abort().await
     }
 
     #[tracing::instrument(
         parent = &self.span,
         level = "trace",
@@ -378,22 +370,14 @@
         self.inner.write(bs)
     }
 
     #[tracing::instrument(
         parent = &self.span,
         level = "trace",
         skip_all)]
-    fn append(&mut self, bs: Bytes) -> Result<()> {
-        self.inner.append(bs)
-    }
-
-    #[tracing::instrument(
-        parent = &self.span,
-        level = "trace",
-        skip_all)]
     fn close(&mut self) -> Result<()> {
         self.inner.close()
     }
 }
 
 #[async_trait]
 impl<R: oio::Page> oio::Page for TracingWrapper<R> {
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/layers/type_eraser.rs` & `opendal-0.33.0/local_dependencies/opendal/src/layers/type_eraser.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/lib.rs` & `opendal-0.33.0/local_dependencies/opendal/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -77,23 +77,21 @@
 pub mod services;
 
 #[cfg(test)]
 mod tests {
     use std::mem::size_of;
 
     use super::*;
-    use crate::raw::*;
 
     /// This is not a real test case.
     ///
     /// We assert our public structs here to make sure we don't introduce
     /// unexpected struct/enum size change.
     #[test]
     fn assert_size() {
-        assert_eq!(104, size_of::<AccessorInfo>());
         assert_eq!(24, size_of::<Operator>());
         assert_eq!(216, size_of::<Entry>());
         assert_eq!(192, size_of::<Metadata>());
         assert_eq!(1, size_of::<EntryMode>());
         assert_eq!(24, size_of::<Scheme>());
     }
 }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/accessor.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/accessor.rs`

 * *Files 16% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::Debug;
 use std::sync::Arc;
 
 use async_trait::async_trait;
-use flagset::flags;
-use flagset::FlagSet;
 
 use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Underlying trait of all backends for implementors.
 ///
@@ -76,15 +74,15 @@
     /// - scheme: declare the scheme of backend.
     /// - capabilities: declare the capabilities of current backend.
     /// - hints: declare the hints of current backend
     fn info(&self) -> AccessorInfo;
 
     /// Invoke the `create` operation on the specified path
     ///
-    /// Require [`AccessorCapability::Write`]
+    /// Require [`Capability::create_dir`]
     ///
     /// # Behavior
     ///
     /// - Input path MUST match with EntryMode, DON'T NEED to check mode.
     /// - Create on existing dir SHOULD succeed.
     async fn create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         let (_, _) = (path, args);
@@ -94,15 +92,15 @@
             "operation is not supported",
         ))
     }
 
     /// Invoke the `read` operation on the specified path, returns a
     /// [`Reader`][crate::Reader] if operate successful.
     ///
-    /// Require [`AccessorCapability::Read`]
+    /// Require [`Capability::read`]
     ///
     /// # Behavior
     ///
     /// - Input path MUST be file path, DON'T NEED to check mode.
     /// - The returning content length may be smaller than the range specified.
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let (_, _) = (path, args);
@@ -112,15 +110,15 @@
             "operation is not supported",
         ))
     }
 
     /// Invoke the `write` operation on the specified path, returns a
     /// written size if operate successful.
     ///
-    /// Require [`AccessorCapability::Write`]
+    /// Require [`Capability::write`]
     ///
     /// # Behavior
     ///
     /// - Input path MUST be file path, DON'T NEED to check mode.
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         let (_, _) = (path, args);
 
@@ -128,15 +126,15 @@
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `copy` operation on the specified `from` path and `to` path.
     ///
-    /// Require [AccessorCapability::Copy]
+    /// Require [Capability::copy]
     ///
     /// # Behaviour
     ///
     /// - `from` and `to` MUST be file path, DON'T NEED to check mode.
     /// - Copy on existing file SHOULD succeed.
     /// - Copy on existing file SHOULD overwrite and truncate.
     async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
@@ -146,27 +144,27 @@
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `rename` operation on the specified `from` path and `to` path.
     ///
-    /// Require [AccessorCapability::Rename]
+    /// Require [Capability::rename]
     async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
         let (_, _, _) = (from, to, args);
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `stat` operation on the specified path.
     ///
-    /// Require [`AccessorCapability::Read`]
+    /// Require [`Capability::stat`]
     ///
     /// # Behavior
     ///
     /// - `stat` empty path means stat backend's root path.
     /// - `stat` a path endswith "/" means stating a dir.
     /// - `mode` and `content_length` must be set.
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
@@ -176,15 +174,15 @@
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `delete` operation on the specified path.
     ///
-    /// Require [`AccessorCapability::Write`]
+    /// Require [`Capability::delete`]
     ///
     /// # Behavior
     ///
     /// - `delete` is an idempotent operation, it's safe to call `Delete` on the same path multiple times.
     /// - `delete` SHOULD return `Ok(())` if the path is deleted successfully or not exist.
     async fn delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
         let (_, _) = (path, args);
@@ -193,15 +191,15 @@
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `list` operation on the specified path.
     ///
-    /// Require [`AccessorCapability::List`]
+    /// Require [`Capability::list`]
     ///
     /// # Behavior
     ///
     /// - Input path MUST be dir path, DON'T NEED to check mode.
     /// - List non-exist dir should return Empty.
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         let (_, _) = (path, args);
@@ -210,153 +208,155 @@
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `scan` operation on the specified path.
     ///
-    /// Require [`AccessorCapability::Scan`]
+    /// Require [`Capability::scan`]
     async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)> {
         let (_, _) = (path, args);
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `presign` operation on the specified path.
     ///
-    /// Require [`AccessorCapability::Presign`]
+    /// Require [`Capability::presign`]
     ///
     /// # Behavior
     ///
     /// - This API is optional, return [`std::io::ErrorKind::Unsupported`] if not supported.
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         let (_, _) = (path, args);
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `batch` operations.
+    ///
+    /// Require [`Capability::batch`]
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
         let _ = args;
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `blocking_create` operation on the specified path.
     ///
-    /// This operation is the blocking version of [`Accessor::create`]
+    /// This operation is the blocking version of [`Accessor::create_dir`]
     ///
-    /// Require [`AccessorCapability::Write`] and [`AccessorCapability::Blocking`]
+    /// Require [`Capability::create_dir`] and [`Capability::blocking`]
     fn blocking_create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         let (_, _) = (path, args);
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `blocking_read` operation on the specified path.
     ///
     /// This operation is the blocking version of [`Accessor::read`]
     ///
-    /// Require [`AccessorCapability::Read`] and [`AccessorCapability::Blocking`]
+    /// Require [`Capability::read`] and [`Capability::blocking`]
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         let (_, _) = (path, args);
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `blocking_write` operation on the specified path.
     ///
     /// This operation is the blocking version of [`Accessor::write`]
     ///
-    /// Require [`AccessorCapability::Write`] and [`AccessorCapability::Blocking`]
+    /// Require [`Capability::write`] and [`Capability::blocking`]
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
         let (_, _) = (path, args);
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `blocking_copy` operation on the specified `from` path and `to` path.
     ///
     /// This operation is the blocking version of [`Accessor::copy`]
     ///
-    /// Require [`AccessorCapability::Copy`] and [`AccessorCapability::Blocking`]
+    /// Require [`Capability::copy`] and [`Capability::blocking`]
     fn blocking_copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
         let (_, _, _) = (from, to, args);
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `blocking_rename` operation on the specified `from` path and `to` path.
     ///
     /// This operation is the blocking version of [`Accessor::rename`]
     ///
-    /// Require [`AccessorCapability::Rename`] and [`AccessorCapability::Blocking`]
+    /// Require [`Capability::rename`] and [`Capability::blocking`]
     fn blocking_rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
         let (_, _, _) = (from, to, args);
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `blocking_stat` operation on the specified path.
     ///
     /// This operation is the blocking version of [`Accessor::stat`]
     ///
-    /// Require [`AccessorCapability::Read`] and [`AccessorCapability::Blocking`]
+    /// Require [`Capability::stat`] and [`Capability::blocking`]
     fn blocking_stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         let (_, _) = (path, args);
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `blocking_delete` operation on the specified path.
     ///
     /// This operation is the blocking version of [`Accessor::delete`]
     ///
-    /// Require [`AccessorCapability::Write`] and [`AccessorCapability::Blocking`]
+    /// Require [`Capability::write`] and [`Capability::blocking`]
     fn blocking_delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
         let (_, _) = (path, args);
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `blocking_list` operation on the specified path.
     ///
     /// This operation is the blocking version of [`Accessor::list`]
     ///
-    /// Require [`AccessorCapability::List`] and [`AccessorCapability::Blocking`]
+    /// Require [`Capability::list`] and [`Capability::blocking`]
     ///
     /// # Behavior
     ///
     /// - List non-exist dir should return Empty.
     fn blocking_list(&self, path: &str, args: OpList) -> Result<(RpList, Self::BlockingPager)> {
         let (_, _) = (path, args);
 
@@ -364,15 +364,15 @@
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
     /// Invoke the `blocking_scan` operation on the specified path.
     ///
-    /// Require [`AccessorCapability::Scan`] and [`AccessorCapability::Blocking`]
+    /// Require [`Capability::scan`] and [`Capability::blocking`]
     fn blocking_scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::BlockingPager)> {
         let (_, _) = (path, args);
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
@@ -390,17 +390,15 @@
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         AccessorInfo {
             scheme: Scheme::Custom("dummy"),
             root: "".to_string(),
             name: "dummy".to_string(),
-            max_batch_operations: None,
-            capabilities: None.into(),
-            hints: None.into(),
+            capability: Capability::default(),
         }
     }
 }
 
 /// All functions in `Accessor` only requires `&self`, so it's safe to implement
 /// `Accessor` for `Arc<dyn Accessor>`.
 #[async_trait]
@@ -503,19 +501,16 @@
 
 /// Metadata for accessor, users can use this metadata to get information of underlying backend.
 #[derive(Clone, Debug, Default)]
 pub struct AccessorInfo {
     scheme: Scheme,
     root: String,
     name: String,
-    /// limit of batch operation
-    /// only meaningful when accessor supports batch operation
-    max_batch_operations: Option<usize>,
-    capabilities: FlagSet<AccessorCapability>,
-    hints: FlagSet<AccessorHint>,
+
+    capability: Capability,
 }
 
 impl AccessorInfo {
     /// [`Scheme`] of backend.
     pub fn scheme(&self) -> Scheme {
         self.scheme
     }
@@ -551,89 +546,23 @@
 
     /// Set name of this backend.
     pub fn set_name(&mut self, name: &str) -> &mut Self {
         self.name = name.to_string();
         self
     }
 
-    /// backend's number limitation of operations in a single batch.
-    ///
-    /// # Note
-    /// - Got Some(x): limitation is x
-    /// - Got None: no limitation
-    pub(crate) fn max_batch_operations(&self) -> Option<usize> {
-        self.max_batch_operations
-    }
-
-    /// Set batch size limit for backend.
-    pub(crate) fn set_max_batch_operations(&mut self, limit: usize) -> &mut Self {
-        self.max_batch_operations = Some(limit);
-        self
+    /// Get backend's capabilities.
+    pub fn capability(&self) -> Capability {
+        self.capability
     }
 
     /// Get backend's capabilities.
-    pub fn capabilities(&self) -> FlagSet<AccessorCapability> {
-        self.capabilities
+    pub fn capability_mut(&mut self) -> &mut Capability {
+        &mut self.capability
     }
 
     /// Set capabilities for backend.
-    pub fn set_capabilities(
-        &mut self,
-        capabilities: impl Into<FlagSet<AccessorCapability>>,
-    ) -> &mut Self {
-        self.capabilities = capabilities.into();
-        self
-    }
-
-    /// Get backend's hints.
-    pub fn hints(&self) -> FlagSet<AccessorHint> {
-        self.hints
-    }
-
-    /// Set hints for backend.
-    pub fn set_hints(&mut self, hints: impl Into<FlagSet<AccessorHint>>) -> &mut Self {
-        self.hints = hints.into();
+    pub fn set_capability(&mut self, capability: Capability) -> &mut Self {
+        self.capability = capability;
         self
     }
 }
-
-flags! {
-    /// AccessorCapability describes accessor's advanced capability.
-    pub enum AccessorCapability: u32 {
-        /// Add this capability if service supports `read` and `stat`
-        Read,
-        /// Add this capability if service supports `write` and `delete`
-        Write,
-        /// Add this capability if service supports `copy`
-        Copy,
-        /// Add this capability if service supports `rename`
-        Rename,
-        /// Add this capability if service supports `list`
-        List,
-        /// Add this capability if service supports `scan`
-        Scan,
-        /// Add this capability if service supports `presign`
-        Presign,
-        /// Add this capability if service supports `blocking`
-        Blocking,
-        /// Add this capability if service supports `batch`
-        Batch,
-    }
-}
-
-flags! {
-    /// AccessorHint describes accessor's hint.
-    ///
-    /// Hint means developers can do optimize for this accessor.
-    ///
-    /// All hints are internal used only and will not be exposed to users.
-    pub enum AccessorHint: u64 {
-        /// Read seekable means the underlying read is seekable.
-        ///
-        /// We can reuse the same reader instead of always creating new one.
-        ReadSeekable,
-        /// Read streamable means the underlying read is streamable.
-        ///
-        /// It's better to use stream to reading data.
-        ReadStreamable,
-    }
-}
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::Debug;
 
 use async_trait::async_trait;
-use flagset::FlagSet;
 
 use crate::raw::*;
+use crate::Capability;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Result;
 use crate::Scheme;
 
 /// KvAdapter is the adapter to underlying kv services.
 ///
@@ -131,50 +131,46 @@
     }
 }
 
 /// Metadata for this key value accessor.
 pub struct Metadata {
     scheme: Scheme,
     name: String,
-    capabilities: FlagSet<AccessorCapability>,
+    capabilities: Capability,
 }
 
 impl Metadata {
     /// Create a new KeyValueAccessorInfo.
-    pub fn new(
-        scheme: Scheme,
-        name: &str,
-        capabilities: impl Into<FlagSet<AccessorCapability>>,
-    ) -> Self {
+    pub fn new(scheme: Scheme, name: &str, capabilities: Capability) -> Self {
         Self {
             scheme,
             name: name.to_string(),
-            capabilities: capabilities.into(),
+            capabilities,
         }
     }
 
     /// Get the scheme.
     pub fn scheme(&self) -> Scheme {
         self.scheme
     }
 
     /// Get the name.
     pub fn name(&self) -> &str {
         &self.name
     }
 
     /// Get the capabilities.
-    pub fn capabilities(&self) -> FlagSet<AccessorCapability> {
+    pub fn capabilities(&self) -> Capability {
         self.capabilities
     }
 }
 
 impl From<Metadata> for AccessorInfo {
     fn from(m: Metadata) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_name(m.name());
         am.set_scheme(m.scheme());
-        am.set_capabilities(m.capabilities());
+        am.set_capability(m.capabilities());
 
         am
     }
 }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs`

 * *Files 7% similar despite different names*

```diff
@@ -58,16 +58,27 @@
     type Writer = KvWriter<S>;
     type BlockingWriter = KvWriter<S>;
     type Pager = KvPager;
     type BlockingPager = KvPager;
 
     fn info(&self) -> AccessorInfo {
         let mut am: AccessorInfo = self.kv.metadata().into();
-        am.set_root(&self.root)
-            .set_hints(AccessorHint::ReadStreamable | AccessorHint::ReadSeekable);
+        am.set_root(&self.root);
+
+        let cap = am.capability_mut();
+        if cap.read {
+            cap.read_can_seek = true;
+            cap.read_can_next = true;
+            cap.stat = true;
+        }
+
+        if cap.write {
+            cap.create_dir = true;
+            cap.delete = true;
+        }
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let p = build_abs_path(&self.root, path);
         self.kv.set(&p, &[]).await?;
@@ -103,21 +114,35 @@
             None => return Err(Error::new(ErrorKind::NotFound, "kv doesn't have this path")),
         };
 
         let bs = self.apply_range(bs, args.range());
         Ok((RpRead::new(bs.len() as u64), oio::Cursor::from(bs)))
     }
 
-    async fn write(&self, path: &str, _: OpWrite) -> Result<(RpWrite, Self::Writer)> {
+    async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
+        if args.content_length().is_none() {
+            return Err(Error::new(
+                ErrorKind::Unsupported,
+                "write without content length is not supported",
+            ));
+        }
+
         let p = build_abs_path(&self.root, path);
 
         Ok((RpWrite::new(), KvWriter::new(self.kv.clone(), p)))
     }
 
-    fn blocking_write(&self, path: &str, _: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
+    fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
+        if args.content_length().is_none() {
+            return Err(Error::new(
+                ErrorKind::Unsupported,
+                "write without content length is not supported",
+            ));
+        }
+
         let p = build_abs_path(&self.root, path);
 
         Ok((RpWrite::new(), KvWriter::new(self.kv.clone(), p)))
     }
 
     async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
         let p = build_abs_path(&self.root, path);
@@ -260,43 +285,25 @@
     fn new(kv: Arc<S>, path: String) -> Self {
         KvWriter {
             kv,
             path,
             buf: None,
         }
     }
-
-    fn extend_buf(&mut self, bs: Bytes) {
-        if let Some(buf) = self.buf.as_mut() {
-            buf.extend(bs);
-        } else {
-            self.buf = Some(bs.into())
-        }
-    }
 }
 
 #[async_trait]
 impl<S: Adapter> oio::Write for KvWriter<S> {
+    // TODO: we need to support append in the future.
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         self.buf = Some(bs.into());
 
         Ok(())
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        if let Err(e) = self.kv.append(&self.path, bs.to_vec().as_slice()).await {
-            if e.kind() == ErrorKind::Unsupported {
-                self.extend_buf(bs);
-            } else {
-                return Err(e);
-            }
-        }
-        Ok(())
-    }
-
     async fn abort(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support abort",
         ))
     }
 
@@ -312,20 +319,14 @@
 impl<S: Adapter> oio::BlockingWrite for KvWriter<S> {
     fn write(&mut self, bs: Bytes) -> Result<()> {
         self.buf = Some(bs.into());
 
         Ok(())
     }
 
-    fn append(&mut self, bs: Bytes) -> Result<()> {
-        self.extend_buf(bs);
-
-        Ok(())
-    }
-
     fn close(&mut self) -> Result<()> {
         if let Some(buf) = self.buf.as_deref() {
             self.kv.blocking_set(&self.path, buf)?;
         }
 
         Ok(())
     }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/chrono_util.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/chrono_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/body.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/body.rs`

 * *Files 6% similar despite different names*

```diff
@@ -140,21 +140,23 @@
     }
 
     #[inline]
     fn check(expect: u64, actual: u64) -> Result<()> {
         match actual.cmp(&expect) {
             Ordering::Equal => Ok(()),
             Ordering::Less => Err(Error::new(
-                ErrorKind::Unexpected,
+                ErrorKind::ContentIncomplete,
                 &format!("reader got too less data, expect: {expect}, actual: {actual}"),
-            )),
+            )
+            .set_temporary()),
             Ordering::Greater => Err(Error::new(
-                ErrorKind::Unexpected,
+                ErrorKind::ContentTruncated,
                 &format!("reader got too much data, expect: {expect}, actual: {actual}"),
-            )),
+            )
+            .set_temporary()),
         }
     }
 }
 
 impl oio::Read for IncomingAsyncBody {
     fn poll_read(&mut self, cx: &mut Context<'_>, mut buf: &mut [u8]) -> Poll<Result<usize>> {
         if buf.is_empty() {
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/client.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/client.rs`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::Debug;
 use std::fmt::Formatter;
+use std::mem;
 use std::str::FromStr;
 
 use futures::TryStreamExt;
 use http::Request;
 use http::Response;
 use reqwest::redirect::Policy;
 use reqwest::Url;
@@ -75,37 +76,39 @@
     /// Get the async client from http client.
     pub fn client(&self) -> reqwest::Client {
         self.client.clone()
     }
 
     /// Send a request in async way.
     pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
+        let url = req.uri().to_string();
         let is_head = req.method() == http::Method::HEAD;
+
         let (parts, body) = req.into_parts();
 
         let mut req_builder = self
             .client
             .request(
                 parts.method,
-                Url::from_str(&parts.uri.to_string()).expect("input request url must be valid"),
+                Url::from_str(&url).expect("input request url must be valid"),
             )
             .version(parts.version)
             .headers(parts.headers);
 
         req_builder = if let AsyncBody::Multipart(field, r) = body {
             let mut form = reqwest::multipart::Form::new();
             let part = reqwest::multipart::Part::stream(AsyncBody::Bytes(r));
             form = form.part(field, part);
 
             req_builder.multipart(form)
         } else {
             req_builder.body(body)
         };
 
-        let resp = req_builder.send().await.map_err(|err| {
+        let mut resp = req_builder.send().await.map_err(|err| {
             let is_temporary = !(
                 // Builder related error should not be retried.
                 err.is_builder() ||
                 // Error returned by RedirectPolicy.
                 //
                 // We don't set this by hand, just don't allow retry.
                 err.is_redirect() ||
@@ -113,14 +116,15 @@
                 //
                 // Status should be checked by our services.
                 err.is_status()
             );
 
             let mut oerr = Error::new(ErrorKind::Unexpected, "send async request")
                 .with_operation("http_util::Client::send_async")
+                .with_context("url", &url)
                 .set_source(err);
             if is_temporary {
                 oerr = oerr.set_temporary();
             }
 
             oerr
         })?;
@@ -132,23 +136,23 @@
         } else {
             parse_content_length(resp.headers()).expect("response content length must be valid")
         };
 
         let mut hr = Response::builder()
             .version(resp.version())
             .status(resp.status());
-        for (k, v) in resp.headers().iter() {
-            hr = hr.header(k, v);
-        }
+        // Swap headers directly instead of copy the entire map.
+        mem::swap(hr.headers_mut().unwrap(), resp.headers_mut());
 
-        let stream = resp.bytes_stream().map_err(|err| {
+        let stream = resp.bytes_stream().map_err(move |err| {
             // If stream returns a body related error, we can convert
             // it to interrupt so we can retry it.
             Error::new(ErrorKind::Unexpected, "read data from http stream")
                 .map(|v| if err.is_body() { v.set_temporary() } else { v })
+                .with_context("url", &url)
                 .set_source(err)
         });
 
         let body = IncomingAsyncBody::new(Box::new(stream), content_length);
 
         let resp = hr.body(body).expect("response must build succeed");
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/header.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/header.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/uri.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/layer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,14 @@
 //! - Raw APIs should only be accessed via `opendal::raw::Xxxx`, any public
 //!   API should never expose raw API directly.
 //! - Raw APIs are far more less stable than public API, please don't rely on
 //!   them whenever possible.
 
 mod accessor;
 pub use accessor::Accessor;
-pub use accessor::AccessorCapability;
-pub use accessor::AccessorHint;
 pub use accessor::AccessorInfo;
 pub use accessor::FusedAccessor;
 
 mod layer;
 pub use layer::Layer;
 pub use layer::LayeredAccessor;
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/cursor.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ftp/util.rs`

 * *Files 20% similar despite different names*

```diff
@@ -11,130 +11,113 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::io::Read;
-use std::io::SeekFrom;
+use std::io;
+use std::pin::Pin;
 use std::task::Context;
 use std::task::Poll;
 
-use bytes::Bytes;
+use bb8::PooledConnection;
+use futures::future::BoxFuture;
+use futures::ready;
+use futures::AsyncRead;
+use futures::FutureExt;
+use suppaftp::Status;
 
+use super::backend::Manager;
 use crate::raw::*;
 use crate::*;
 
-/// Cursor is the cursor for [`Bytes`] that implements [`oio::Read`]
-pub struct Cursor {
-    inner: Bytes,
-    pos: u64,
+/// Wrapper for ftp data stream and command stream.
+pub struct FtpReader {
+    reader: Box<dyn AsyncRead + Send + Unpin>,
+    state: State,
 }
 
-impl Cursor {
-    /// Returns `true` if the remaining slice is empty.
-    pub fn is_empty(&self) -> bool {
-        self.pos as usize >= self.inner.len()
-    }
+unsafe impl Sync for FtpReader {}
 
-    /// Returns the remaining slice.
-    pub fn remaining_slice(&self) -> &[u8] {
-        let len = self.pos.min(self.inner.len() as u64) as usize;
-        &self.inner.as_ref()[len..]
-    }
+pub enum State {
+    Reading(Option<PooledConnection<'static, Manager>>),
+    Finalize(BoxFuture<'static, Result<()>>),
 }
 
-impl From<Vec<u8>> for Cursor {
-    fn from(v: Vec<u8>) -> Self {
-        Cursor {
-            inner: Bytes::from(v),
-            pos: 0,
+impl FtpReader {
+    /// Create an instance of FtpReader.
+    pub fn new(
+        r: Box<dyn AsyncRead + Send + Unpin>,
+        c: PooledConnection<'static, Manager>,
+    ) -> Self {
+        Self {
+            reader: r,
+            state: State::Reading(Some(c)),
         }
     }
 }
 
-impl oio::Read for Cursor {
-    fn poll_read(&mut self, _: &mut Context<'_>, buf: &mut [u8]) -> Poll<Result<usize>> {
-        let n = Read::read(&mut self.remaining_slice(), buf).map_err(|err| {
-            Error::new(ErrorKind::Unexpected, "read data from Cursor")
-                .with_context("source", "Cursor")
-                .set_source(err)
-        })?;
-        self.pos += n as u64;
-        Poll::Ready(Ok(n))
-    }
-
-    fn poll_seek(&mut self, _: &mut Context<'_>, pos: SeekFrom) -> Poll<Result<u64>> {
-        let (base, amt) = match pos {
-            SeekFrom::Start(n) => (0, n as i64),
-            SeekFrom::End(n) => (self.inner.len() as i64, n),
-            SeekFrom::Current(n) => (self.pos as i64, n),
-        };
-
-        let n = match base.checked_add(amt) {
-            Some(n) if n >= 0 => n as u64,
-            _ => {
-                return Poll::Ready(Err(Error::new(
-                    ErrorKind::Unexpected,
-                    "invalid seek to a negative or overflowing position",
-                )))
+impl oio::Read for FtpReader {
+    fn poll_read(&mut self, cx: &mut Context<'_>, buf: &mut [u8]) -> Poll<Result<usize>> {
+        let data = Pin::new(&mut self.reader).poll_read(cx, buf);
+
+        match &mut self.state {
+            // Reading state, try to poll some data.
+            State::Reading(stream) => {
+                match stream {
+                    Some(_) => {
+                        // when hit Err or EOF, consume ftpstream, change state to Finalize and send fut.
+                        if let Poll::Ready(Err(_)) | Poll::Ready(Ok(0)) = data {
+                            let mut ft = stream.take().unwrap();
+
+                            let fut = async move {
+                                ft.read_response_in(&[
+                                    Status::ClosingDataConnection,
+                                    Status::RequestedFileActionOk,
+                                ])
+                                .await?;
+
+                                Ok(())
+                            };
+                            self.state = State::Finalize(Box::pin(fut));
+                        } else {
+                            // Otherwise, exit and return data.
+                            return data.map_err(|err| {
+                                Error::new(ErrorKind::Unexpected, "read data from ftp data stream")
+                                    .set_source(err)
+                            });
+                        }
+
+                        self.poll_read(cx, buf)
+                    }
+                    // We could never reach this branch because we will change to Finalize state once we consume ftp stream.
+                    None => unreachable!(),
+                }
             }
-        };
-        self.pos = n;
-        Poll::Ready(Ok(n))
-    }
 
-    fn poll_next(&mut self, _: &mut Context<'_>) -> Poll<Option<Result<Bytes>>> {
-        if self.is_empty() {
-            Poll::Ready(None)
-        } else {
-            // The clone here is required as we don't want to change it.
-            let bs = self.inner.clone().split_off(self.pos as usize);
-            self.pos += bs.len() as u64;
-            Poll::Ready(Some(Ok(bs)))
+            // Finalize state, wait for finalization of stream.
+            State::Finalize(fut) => match ready!(Pin::new(fut).poll_unpin(cx)) {
+                Ok(_) => Poll::Ready(Ok(0)),
+                Err(e) => Poll::Ready(Err(e)),
+            },
         }
     }
-}
 
-impl oio::BlockingRead for Cursor {
-    fn read(&mut self, buf: &mut [u8]) -> Result<usize> {
-        let n = Read::read(&mut self.remaining_slice(), buf).map_err(|err| {
-            Error::new(ErrorKind::Unexpected, "read data from Cursor")
-                .with_context("source", "Cursor")
-                .set_source(err)
-        })?;
-        self.pos += n as u64;
-        Ok(n)
-    }
+    fn poll_seek(&mut self, cx: &mut Context<'_>, pos: io::SeekFrom) -> Poll<Result<u64>> {
+        let (_, _) = (cx, pos);
 
-    fn seek(&mut self, pos: SeekFrom) -> Result<u64> {
-        let (base, amt) = match pos {
-            SeekFrom::Start(n) => (0, n as i64),
-            SeekFrom::End(n) => (self.inner.len() as i64, n),
-            SeekFrom::Current(n) => (self.pos as i64, n),
-        };
-
-        let n = match base.checked_add(amt) {
-            Some(n) if n >= 0 => n as u64,
-            _ => {
-                return Err(Error::new(
-                    ErrorKind::Unexpected,
-                    "invalid seek to a negative or overflowing position",
-                ))
-            }
-        };
-        self.pos = n;
-        Ok(n)
-    }
-
-    fn next(&mut self) -> Option<Result<Bytes>> {
-        if self.is_empty() {
-            None
-        } else {
-            // The clone here is required as we don't want to change it.
-            let bs = self.inner.clone().split_off(self.pos as usize);
-            self.pos += bs.len() as u64;
-            Some(Ok(bs))
-        }
+        Poll::Ready(Err(Error::new(
+            ErrorKind::Unsupported,
+            "output reader doesn't support seeking",
+        )))
+    }
+
+    fn poll_next(&mut self, cx: &mut Context<'_>) -> Poll<Option<Result<bytes::Bytes>>> {
+        let _ = cx;
+
+        Poll::Ready(Some(Err(Error::new(
+            ErrorKind::Unsupported,
+            "output reader doesn't support seeking",
+        ))))
     }
 }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/entry.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,18 @@
         type Writer = ();
         type BlockingWriter = ();
         type Pager = ();
         type BlockingPager = ();
 
         fn info(&self) -> AccessorInfo {
             let mut am = AccessorInfo::default();
-            am.set_capabilities(AccessorCapability::Read);
+            am.set_capability(Capability {
+                read: true,
+                ..Default::default()
+            });
 
             am
         }
 
         async fn read(&self, _: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
             let bs = args.range().apply_on_bytes(self.data.clone());
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 pub use write::BlockingWriter;
 pub use write::Write;
 pub use write::WriteOperation;
 pub use write::Writer;
 
 mod cursor;
 pub use cursor::Cursor;
+pub use cursor::VectorCursor;
 
 mod into_streamable;
 pub use into_streamable::into_streamable_reader;
 pub use into_streamable::IntoStreamableReader;
 
 mod entry;
 pub use entry::Entry;
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/page.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/page.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/read.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 
 /// to_flat_pager is used to make a hierarchy pager flat.
 pub fn to_flat_pager<A: Accessor, P>(acc: A, path: &str, size: usize) -> ToFlatPager<A, P> {
     #[cfg(debug_assertions)]
     {
         let meta = acc.info();
         debug_assert!(
-            !meta.capabilities().contains(AccessorCapability::Scan),
+            !meta.capability().scan,
             "service already supports scan, call to_flat_pager must be a mistake"
         );
         debug_assert!(
-            meta.capabilities().contains(AccessorCapability::List),
+            meta.capability().list,
             "service doesn't support list hierarchy, it must be a bug"
         );
     }
 
     ToFlatPager {
         acc,
         size,
@@ -254,15 +254,15 @@
         type Writer = ();
         type BlockingWriter = ();
         type Pager = ();
         type BlockingPager = MockPager;
 
         fn info(&self) -> AccessorInfo {
             let mut am = AccessorInfo::default();
-            am.set_capabilities(AccessorCapability::List);
+            am.capability_mut().list = true;
 
             am
         }
 
         fn blocking_list(&self, path: &str, _: OpList) -> Result<(RpList, Self::BlockingPager)> {
             debug!("visit path: {path}");
             Ok((RpList::default(), self.get(path)))
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/write.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/write.rs`

 * *Files 13% similar despite different names*

```diff
@@ -25,24 +25,20 @@
 
 /// WriteOperation is the name for APIs of Writer.
 #[derive(Debug, Copy, Clone, Hash, Eq, PartialEq)]
 #[non_exhaustive]
 pub enum WriteOperation {
     /// Operation for [`Write::write`]
     Write,
-    /// Operation for [`Write::append`]
-    Append,
     /// Operation for [`Write::abort`]
     Abort,
     /// Operation for [`Write::close`]
     Close,
     /// Operation for [`BlockingWrite::write`]
     BlockingWrite,
-    /// Operation for [`BlockingWrite::append`]
-    BlockingAppend,
     /// Operation for [`BlockingWrite::close`]
     BlockingClose,
 }
 
 impl WriteOperation {
     /// Convert self into static str.
     pub fn into_static(self) -> &'static str {
@@ -58,68 +54,64 @@
 
 impl From<WriteOperation> for &'static str {
     fn from(v: WriteOperation) -> &'static str {
         use WriteOperation::*;
 
         match v {
             Write => "Writer::write",
-            Append => "Writer::append",
             Abort => "Writer::abort",
             Close => "Writer::close",
             BlockingWrite => "BlockingWriter::write",
-            BlockingAppend => "BlockingWriter::append",
             BlockingClose => "BlockingWriter::close",
         }
     }
 }
 
 /// Writer is a type erased [`Write`]
 pub type Writer = Box<dyn Write>;
 
 /// Write is the trait that OpenDAL returns to callers.
+///
+/// # Notes
+///
+/// There are two possible two cases:
+///
+/// - Sized: The total size of the object is known in advance.
+/// - Unsized: The total size of the object is unknown in advance.
+///
+/// And it's possible that the given bs length is less than the total
+/// content length. Users will call write multiple times to write
+/// the whole data.
 #[async_trait]
 pub trait Write: Unpin + Send + Sync {
-    /// Write whole content at once.
+    /// Write given into writer.
+    ///
+    /// # Notes
+    ///
+    /// It's possible that the given bs length is less than the total
+    /// content length. And users will call write multiple times.
     ///
-    /// To append multiple bytes together, use `append` instead.
+    /// Please make sure `write` is safe to re-enter.
     async fn write(&mut self, bs: Bytes) -> Result<()>;
 
-    /// Append bytes to the writer.
-    ///
-    /// It is highly recommended to align the length of the input bytes
-    /// into blocks of 4MiB (except the last block) for better performance
-    /// and compatibility.
-    async fn append(&mut self, bs: Bytes) -> Result<()>;
-
-    /// Abort the pending appendable writer.
-    /// #note
-    /// This method is only applicable to writers opened in append mode.
+    /// Abort the pending writer.
     async fn abort(&mut self) -> Result<()>;
 
     /// Close the writer and make sure all data has been flushed.
     async fn close(&mut self) -> Result<()>;
 }
 
 #[async_trait]
 impl Write for () {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let _ = bs;
 
         unimplemented!("write is required to be implemented for oio::Write")
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let _ = bs;
-
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "output writer doesn't support append",
-        ))
-    }
-
     async fn abort(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support abort",
         ))
     }
 
@@ -135,18 +127,14 @@
 /// work as expected, we must add this impl.
 #[async_trait]
 impl<T: Write + ?Sized> Write for Box<T> {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         (**self).write(bs).await
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        (**self).append(bs).await
-    }
-
     async fn abort(&mut self) -> Result<()> {
         (**self).abort().await
     }
 
     async fn close(&mut self) -> Result<()> {
         (**self).close().await
     }
@@ -156,37 +144,25 @@
 pub type BlockingWriter = Box<dyn BlockingWrite>;
 
 /// BlockingWrite is the trait that OpenDAL returns to callers.
 pub trait BlockingWrite: Send + Sync + 'static {
     /// Write whole content at once.
     fn write(&mut self, bs: Bytes) -> Result<()>;
 
-    /// Append content at tailing.
-    fn append(&mut self, bs: Bytes) -> Result<()>;
-
     /// Close the writer and make sure all data has been flushed.
     fn close(&mut self) -> Result<()>;
 }
 
 impl BlockingWrite for () {
     fn write(&mut self, bs: Bytes) -> Result<()> {
         let _ = bs;
 
         unimplemented!("write is required to be implemented for oio::BlockingWrite")
     }
 
-    fn append(&mut self, bs: Bytes) -> Result<()> {
-        let _ = bs;
-
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "output writer doesn't support append",
-        ))
-    }
-
     fn close(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support close",
         ))
     }
 }
@@ -194,15 +170,11 @@
 /// `Box<dyn BlockingWrite>` won't implement `BlockingWrite` automatically.
 /// To make BlockingWriter work as expected, we must add this impl.
 impl<T: BlockingWrite + ?Sized> BlockingWrite for Box<T> {
     fn write(&mut self, bs: Bytes) -> Result<()> {
         (**self).write(bs)
     }
 
-    fn append(&mut self, bs: Bytes) -> Result<()> {
-        (**self).append(bs)
-    }
-
     fn close(&mut self) -> Result<()> {
         (**self).close()
     }
 }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/operation.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/operation.rs`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     /// Operation for [`crate::raw::Accessor::blocking_read`]
     BlockingRead,
     /// Operation for [`crate::raw::Accessor::blocking_write`]
     BlockingWrite,
     /// Operation for [`crate::raw::Accessor::blocking_copy`]
     BlockingCopy,
     /// Operation for [`crate::raw::Accessor::blocking_rename`]
-    BlockingMove,
+    BlockingRename,
     /// Operation for [`crate::raw::Accessor::blocking_stat`]
     BlockingStat,
     /// Operation for [`crate::raw::Accessor::blocking_delete`]
     BlockingDelete,
     /// Operation for [`crate::raw::Accessor::blocking_list`]
     BlockingList,
     /// Operation for [`crate::raw::Accessor::blocking_scan`]
@@ -95,15 +95,15 @@
             Operation::Scan => "scan",
             Operation::Presign => "presign",
             Operation::Batch => "batch",
             Operation::BlockingCreateDir => "blocking_create_dir",
             Operation::BlockingRead => "blocking_read",
             Operation::BlockingWrite => "blocking_write",
             Operation::BlockingCopy => "blocking_copy",
-            Operation::BlockingMove => "blocking_rename",
+            Operation::BlockingRename => "blocking_rename",
             Operation::BlockingStat => "blocking_stat",
             Operation::BlockingDelete => "blocking_delete",
             Operation::BlockingList => "blocking_list",
             Operation::BlockingScan => "blocking_scan",
         }
     }
 }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/path.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/path.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/rps.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/rps.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/serde_util.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/serde_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/raw/version.rs` & `opendal-0.33.0/local_dependencies/opendal/src/raw/version.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/azblob/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/azblob/backend.rs`

 * *Files 3% similar despite different names*

```diff
@@ -443,32 +443,50 @@
     type BlockingReader = ();
     type Writer = AzblobWriter;
     type BlockingWriter = ();
     type Pager = AzblobPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
-        use AccessorCapability::*;
-        use AccessorHint::*;
-
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Azblob)
             .set_root(&self.core.root)
             .set_name(&self.core.container)
-            .set_max_batch_operations(AZBLOB_BATCH_LIMIT)
-            .set_capabilities(Read | Write | List | Scan | Batch | Copy)
-            .set_hints(ReadStreamable);
+            .set_capability(Capability {
+                stat: true,
+                stat_with_if_match: true,
+                stat_with_if_none_match: true,
+
+                read: true,
+                read_can_next: true,
+                read_with_if_match: true,
+                read_with_if_none_match: true,
+                read_with_override_content_disposition: true,
+
+                write: true,
+                write_with_content_type: true,
+                write_with_cache_control: true,
+
+                delete: true,
+                create_dir: true,
+                list: true,
+                scan: true,
+                copy: true,
+                batch: true,
+                batch_max_operations: Some(AZBLOB_BATCH_LIMIT),
+                ..Default::default()
+            });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
-        let mut req = self
-            .core
-            .azblob_put_blob_request(path, Some(0), None, AsyncBody::Empty)?;
+        let mut req =
+            self.core
+                .azblob_put_blob_request(path, Some(0), None, None, AsyncBody::Empty)?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
         let status = resp.status();
 
@@ -478,33 +496,42 @@
                 Ok(RpCreate::default())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self.core.azblob_get_blob(path, args.range()).await?;
+        let resp = self
+            .core
+            .azblob_get_blob(
+                path,
+                args.range(),
+                args.if_none_match(),
+                args.if_match(),
+                args.override_content_disposition(),
+            )
+            .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
 
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.append() {
+        if args.content_length().is_none() {
             return Err(Error::new(
                 ErrorKind::Unsupported,
-                "append write is not supported",
+                "write without content length is not supported",
             ));
         }
 
         Ok((
             RpWrite::default(),
             AzblobWriter::new(self.core.clone(), args, path.to_string()),
         ))
@@ -520,21 +547,24 @@
                 resp.into_body().consume().await?;
                 Ok(RpCopy::default())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
-    async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
+    async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
-        let resp = self.core.azblob_get_blob_properties(path).await?;
+        let resp = self
+            .core
+            .azblob_get_blob_properties(path, args.if_none_match(), args.if_match())
+            .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
             StatusCode::NOT_FOUND if path.ends_with('/') => {
                 Ok(RpStat::new(Metadata::new(EntryMode::DIR)))
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/azblob/batch.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/azblob/batch.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/azblob/core.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/azblob/core.rs`

 * *Files 8% similar despite different names*

```diff
@@ -18,29 +18,34 @@
 use std::fmt;
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::fmt::Write;
 use std::str::FromStr;
 
 use http::header::HeaderName;
+use http::header::CACHE_CONTROL;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
+use http::header::IF_MATCH;
+use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
 use http::Uri;
 use reqsign::AzureStorageCredential;
 use reqsign::AzureStorageLoader;
 use reqsign::AzureStorageSigner;
 
 use super::batch::BatchDeleteRequestBuilder;
 use crate::raw::*;
 use crate::*;
 
-const X_MS_BLOB_TYPE: &str = "x-ms-blob-type";
-const X_MS_COPY_SOURCE: &str = "x-ms-copy-source";
+mod constants {
+    pub const X_MS_BLOB_TYPE: &str = "x-ms-blob-type";
+    pub const X_MS_COPY_SOURCE: &str = "x-ms-copy-source";
+}
 
 pub struct AzblobCore {
     pub container: String,
     pub root: String,
     pub endpoint: String,
 
     pub client: HttpClient,
@@ -96,24 +101,39 @@
 }
 
 impl AzblobCore {
     pub async fn azblob_get_blob(
         &self,
         path: &str,
         range: BytesRange,
+        if_none_match: Option<&str>,
+        if_match: Option<&str>,
+        override_content_disposition: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
-        let url = format!(
+        let mut url = format!(
             "{}/{}/{}",
             self.endpoint,
             self.container,
             percent_encode_path(&p)
         );
 
+        let mut query_args = Vec::new();
+        if let Some(override_content_disposition) = override_content_disposition {
+            query_args.push(format!(
+                "rscd={}",
+                percent_encode_path(override_content_disposition)
+            ))
+        }
+
+        if !query_args.is_empty() {
+            url.push_str(&format!("?{}", query_args.join("&")));
+        }
+
         let mut req = Request::get(&url);
 
         if !range.is_full() {
             // azblob doesn't support read with suffix range.
             //
             // ref: https://learn.microsoft.com/en-us/rest/api/storageservices/specifying-the-range-header-for-blob-service-operations
             if range.offset().is_none() && range.size().is_some() {
@@ -122,71 +142,95 @@
                     "azblob doesn't support read with suffix range",
                 ));
             }
 
             req = req.header(http::header::RANGE, range.to_header());
         }
 
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
+
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
+
         let mut req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
     pub fn azblob_put_blob_request(
         &self,
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
+        cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
             "{}/{}/{}",
             self.endpoint,
             self.container,
             percent_encode_path(&p)
         );
 
         let mut req = Request::put(&url);
-
+        if let Some(cache_control) = cache_control {
+            req = req.header(CACHE_CONTROL, cache_control);
+        }
         if let Some(size) = size {
             req = req.header(CONTENT_LENGTH, size)
         }
 
         if let Some(ty) = content_type {
             req = req.header(CONTENT_TYPE, ty)
         }
 
-        req = req.header(HeaderName::from_static(X_MS_BLOB_TYPE), "BlockBlob");
+        req = req.header(
+            HeaderName::from_static(constants::X_MS_BLOB_TYPE),
+            "BlockBlob",
+        );
 
         // Set body
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
     pub async fn azblob_get_blob_properties(
         &self,
         path: &str,
+        if_none_match: Option<&str>,
+        if_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
             "{}/{}/{}",
             self.endpoint,
             self.container,
             percent_encode_path(&p)
         );
 
-        let req = Request::head(&url);
+        let mut req = Request::head(&url);
+
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
+
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
 
         let mut req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
@@ -230,15 +274,15 @@
             "{}/{}/{}",
             self.endpoint,
             self.container,
             percent_encode_path(&target)
         );
 
         let mut req = Request::put(&target)
-            .header(X_MS_COPY_SOURCE, source)
+            .header(constants::X_MS_COPY_SOURCE, source)
             .header(CONTENT_LENGTH, 0)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/azblob/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/azblob/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/azblob/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/azblob/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/azblob/pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/azblob/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/azblob/writer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/azblob/writer.rs`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 #[async_trait]
 impl oio::Write for AzblobWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let mut req = self.core.azblob_put_blob_request(
             &self.path,
             Some(bs.len()),
             self.op.content_type(),
+            self.op.cache_control(),
             AsyncBody::Bytes(bs),
         )?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
@@ -61,23 +62,14 @@
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let _ = bs;
-
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "output writer doesn't support append",
-        ))
-    }
-
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -304,21 +304,22 @@
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Azdfs)
             .set_root(&self.core.root)
             .set_name(&self.core.filesystem)
-            .set_capabilities(
-                AccessorCapability::Read
-                    | AccessorCapability::Write
-                    | AccessorCapability::Rename
-                    | AccessorCapability::List,
-            )
-            .set_hints(AccessorHint::ReadStreamable);
+            .set_capability(Capability {
+                read: true,
+                read_can_next: true,
+                write: true,
+                rename: true,
+                list: true,
+                ..Default::default()
+            });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let mut req =
             self.core
@@ -350,18 +351,18 @@
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.append() {
+        if args.content_length().is_none() {
             return Err(Error::new(
                 ErrorKind::Unsupported,
-                "append write is not supported",
+                "write without content length is not supported",
             ));
         }
 
         Ok((
             RpWrite::default(),
             AzdfsWriter::new(self.core.clone(), args, path.to_string()),
         ))
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/core.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/writer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/writer.rs`

 * *Files 7% similar despite different names*

```diff
@@ -83,23 +83,14 @@
             }
             _ => Err(parse_error(resp)
                 .await?
                 .with_operation("Backend::azdfs_update_request")),
         }
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let _ = bs;
-
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "output writer doesn't support append",
-        ))
-    }
-
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/dashmap/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/dashmap/backend.rs`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 use std::collections::HashMap;
 use std::fmt::Debug;
 
 use async_trait::async_trait;
 use dashmap::DashMap;
 
 use crate::raw::adapters::kv;
-use crate::raw::*;
 use crate::*;
 
 /// [dashmap](https://github.com/xacrimon/dashmap) backend support.
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
@@ -80,15 +79,20 @@
 
 #[async_trait]
 impl kv::Adapter for Adapter {
     fn metadata(&self) -> kv::Metadata {
         kv::Metadata::new(
             Scheme::Dashmap,
             &format!("{:?}", &self.inner as *const _),
-            AccessorCapability::Read | AccessorCapability::Write | AccessorCapability::Scan,
+            Capability {
+                read: true,
+                write: true,
+                scan: true,
+                ..Default::default()
+            },
         )
     }
 
     async fn get(&self, path: &str) -> Result<Option<Vec<u8>>> {
         self.blocking_get(path)
     }
 
@@ -132,14 +136,15 @@
         }
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
+    use crate::raw::*;
 
     #[test]
     fn test_accessor_metadata_name() {
         let b1 = DashmapBuilder::default().build().unwrap();
         assert_eq!(b1.info().name(), b1.info().name());
 
         let b2 = DashmapBuilder::default().build().unwrap();
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/dashmap/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/dashmap/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/fs/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/fs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -296,23 +296,25 @@
     type Pager = Option<FsPager<tokio::fs::ReadDir>>;
     type BlockingPager = Option<FsPager<std::fs::ReadDir>>;
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Fs)
             .set_root(&self.root.to_string_lossy())
-            .set_capabilities(
-                AccessorCapability::Read
-                    | AccessorCapability::Write
-                    | AccessorCapability::Copy
-                    | AccessorCapability::Rename
-                    | AccessorCapability::List
-                    | AccessorCapability::Blocking,
-            )
-            .set_hints(AccessorHint::ReadSeekable);
+            .set_capability(Capability {
+                read: true,
+                read_can_seek: true,
+                write: true,
+                create_dir: true,
+                list: true,
+                copy: true,
+                rename: true,
+                blocking: true,
+                ..Default::default()
+            });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let p = self.root.join(path.trim_end_matches('/'));
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/fs/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/fs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/fs/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/fs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/fs/pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/fs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/fs/writer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/fs/writer.rs`

 * *Files 14% similar despite different names*

```diff
@@ -50,25 +50,14 @@
 #[async_trait]
 impl oio::Write for FsWriter<tokio::fs::File> {
     /// # Notes
     ///
     /// File could be partial written, so we will seek to start to make sure
     /// we write the same content.
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        self.f.rewind().await.map_err(parse_io_error)?;
-        self.f.write_all(&bs).await.map_err(parse_io_error)?;
-
-        Ok(())
-    }
-
-    /// # Notes
-    ///
-    /// File could be partial written, so we will seek to start to make sure
-    /// we write the same content.
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
         self.f
             .seek(SeekFrom::Start(self.pos))
             .await
             .map_err(parse_io_error)?;
         self.f.write_all(&bs).await.map_err(parse_io_error)?;
         self.pos += bs.len() as u64;
 
@@ -97,25 +86,14 @@
 
 impl oio::BlockingWrite for FsWriter<std::fs::File> {
     /// # Notes
     ///
     /// File could be partial written, so we will seek to start to make sure
     /// we write the same content.
     fn write(&mut self, bs: Bytes) -> Result<()> {
-        self.f.rewind().map_err(parse_io_error)?;
-        self.f.write_all(&bs).map_err(parse_io_error)?;
-
-        Ok(())
-    }
-
-    /// # Notes
-    ///
-    /// File could be partial written, so we will seek to start to make sure
-    /// we write the same content.
-    fn append(&mut self, bs: Bytes) -> Result<()> {
         self.f
             .seek(SeekFrom::Start(self.pos))
             .map_err(parse_io_error)?;
         self.f.write_all(&bs).map_err(parse_io_error)?;
         self.pos += bs.len() as u64;
 
         Ok(())
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ftp/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ftp/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -312,46 +312,43 @@
     type Pager = FtpPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Ftp)
             .set_root(&self.root)
-            .set_capabilities(
-                AccessorCapability::Read | AccessorCapability::Write | AccessorCapability::List,
-            );
+            .set_capability(Capability {
+                read: true,
+                write: true,
+                list: true,
+                ..Default::default()
+            });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let mut ftp_stream = self.ftp_connect(Operation::CreateDir).await?;
 
         let paths: Vec<&str> = path.split_inclusive('/').collect();
 
         let mut curr_path = String::new();
 
         for path in paths {
             curr_path.push_str(path);
-            // try to create directory
-            if curr_path.ends_with('/') {
-                match ftp_stream.mkdir(&curr_path).await {
-                    // Do nothing if status is FileUnavailable or OK(()) is return.
-                    Err(FtpError::UnexpectedResponse(Response {
-                        status: Status::FileUnavailable,
-                        ..
-                    }))
-                    | Ok(()) => (),
-                    Err(e) => {
-                        return Err(e.into());
-                    }
+            match ftp_stream.mkdir(&curr_path).await {
+                // Do nothing if status is FileUnavailable or OK(()) is return.
+                Err(FtpError::UnexpectedResponse(Response {
+                    status: Status::FileUnavailable,
+                    ..
+                }))
+                | Ok(()) => (),
+                Err(e) => {
+                    return Err(e.into());
                 }
-            } else {
-                // else, create file
-                ftp_stream.put_file(&curr_path, &mut "".as_bytes()).await?;
             }
         }
 
         return Ok(RpCreate::default());
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
@@ -384,21 +381,43 @@
             }
         };
 
         Ok((RpRead::new(size), FtpReader::new(r, ftp_stream)))
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.append() {
+        if args.content_length().is_none() {
             return Err(Error::new(
                 ErrorKind::Unsupported,
-                "append write is not supported",
+                "write without content length is not supported",
             ));
         }
 
+        // Ensure the parent dir exists.
+        let parent = get_parent(path);
+        let paths: Vec<&str> = parent.split('/').collect();
+
+        // TODO: we can optimize this by checking dir existence first.
+        let mut ftp_stream = self.ftp_connect(Operation::Write).await?;
+        let mut curr_path = String::new();
+        for path in paths {
+            curr_path.push_str(path);
+            match ftp_stream.mkdir(&curr_path).await {
+                // Do nothing if status is FileUnavailable or OK(()) is return.
+                Err(FtpError::UnexpectedResponse(Response {
+                    status: Status::FileUnavailable,
+                    ..
+                }))
+                | Ok(()) => (),
+                Err(e) => {
+                    return Err(e.into());
+                }
+            }
+        }
+
         Ok((
             RpWrite::new(),
             FtpWriter::new(self.clone(), path.to_string()),
         ))
     }
 
     async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ftp/err.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ftp/err.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ftp/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ftp/pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ftp/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ftp/writer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ftp/writer.rs`

 * *Files 8% similar despite different names*

```diff
@@ -49,23 +49,14 @@
         })?;
 
         ftp_stream.finalize_put_stream(data_stream).await?;
 
         Ok(())
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let _ = bs;
-
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "output writer doesn't support append",
-        ))
-    }
-
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/gcs/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/gcs/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -365,23 +365,27 @@
     type BlockingReader = ();
     type Writer = GcsWriter;
     type BlockingWriter = ();
     type Pager = GcsPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
-        use AccessorCapability::*;
-        use AccessorHint::*;
-
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Gcs)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
-            .set_capabilities(Read | Write | List | Scan | Copy)
-            .set_hints(ReadStreamable);
+            .set_capability(Capability {
+                read: true,
+                read_can_next: true,
+                write: true,
+                list: true,
+                scan: true,
+                copy: true,
+                ..Default::default()
+            });
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let mut req = self
             .core
             .gcs_insert_object_request(path, Some(0), None, AsyncBody::Empty)?;
@@ -395,51 +399,31 @@
             Ok(RpCreate::default())
         } else {
             Err(parse_error(resp).await?)
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self.core.gcs_get_object(path, args.range()).await?;
+        let resp = self
+            .core
+            .gcs_get_object(path, args.range(), args.if_match(), args.if_none_match())
+            .await?;
 
         if resp.status().is_success() {
             let meta = parse_into_metadata(path, resp.headers())?;
             Ok((RpRead::with_metadata(meta), resp.into_body()))
         } else {
             Err(parse_error(resp).await?)
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        let upload_location = if args.append() {
-            let resp = self.core.gcs_initiate_resumable_upload(path).await?;
-            let status = resp.status();
-
-            match status {
-                StatusCode::OK => {
-                    let bs = parse_location(resp.headers())
-                        .expect("Failed to retrieve location of resumable upload");
-                    if let Some(location) = bs {
-                        Some(String::from(location))
-                    } else {
-                        return Err(Error::new(
-                            ErrorKind::NotFound,
-                            "location is not in the response header",
-                        ));
-                    }
-                }
-                _ => return Err(parse_error(resp).await?),
-            }
-        } else {
-            None
-        };
-
         Ok((
             RpWrite::default(),
-            GcsWriter::new(self.core.clone(), args, path.to_string(), upload_location),
+            GcsWriter::new(self.core.clone(), path, args),
         ))
     }
 
     async fn copy(&self, from: &str, to: &str, _: OpCopy) -> Result<RpCopy> {
         let resp = self.core.gcs_copy_object(from, to).await?;
 
         if resp.status().is_success() {
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/gcs/core.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/gcs/core.rs`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,21 @@
 
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::fmt::Write;
 
 use backon::ExponentialBuilder;
 use backon::Retryable;
-use bytes::{Bytes, BytesMut};
+use bytes::Bytes;
+use bytes::BytesMut;
+use http::header::CONTENT_LENGTH;
+use http::header::CONTENT_RANGE;
 use http::header::CONTENT_TYPE;
-use http::header::{CONTENT_LENGTH, CONTENT_RANGE};
+use http::header::IF_MATCH;
+use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
 use once_cell::sync::Lazy;
 use reqsign::GoogleCredentialLoader;
 use reqsign::GoogleSigner;
 use reqsign::GoogleToken;
 use reqsign::GoogleTokenLoader;
@@ -93,26 +97,34 @@
 }
 
 impl GcsCore {
     pub fn gcs_get_object_request(
         &self,
         path: &str,
         range: BytesRange,
+        if_match: Option<&str>,
+        if_none_match: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
             "{}/storage/v1/b/{}/o/{}?alt=media",
             self.endpoint,
             self.bucket,
             percent_encode_path(&p)
         );
 
         let mut req = Request::get(&url);
 
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
         if !range.is_full() {
             req = req.header(http::header::RANGE, range.to_header());
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
@@ -120,16 +132,18 @@
         Ok(req)
     }
 
     pub async fn gcs_get_object(
         &self,
         path: &str,
         range: BytesRange,
+        if_match: Option<&str>,
+        if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.gcs_get_object_request(path, range)?;
+        let mut req = self.gcs_get_object_request(path, range, if_match, if_none_match)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
     pub fn gcs_insert_object_request(
         &self,
@@ -318,29 +332,29 @@
         self.send(req).await
     }
 
     pub fn gcs_upload_in_resumable_upload(
         &self,
         location: &str,
         size: u64,
-        written_bytes: u64,
+        written: u64,
         is_last_part: bool,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let mut req = Request::put(location);
 
         let range_header = if is_last_part {
             format!(
                 "bytes {}-{}/{}",
-                written_bytes,
-                written_bytes + size - 1,
-                written_bytes + size
+                written,
+                written + size - 1,
+                written + size
             )
         } else {
-            format!("bytes {}-{}/*", written_bytes, written_bytes + size - 1)
+            format!("bytes {}-{}/*", written, written + size - 1)
         };
 
         req = req
             .header(CONTENT_LENGTH, size)
             .header(CONTENT_RANGE, range_header);
 
         // Set body
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/gcs/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/gcs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/gcs/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/gcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/gcs/pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/gcs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/gcs/uri.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/gcs/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ghac/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ghac/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -296,16 +296,21 @@
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Ghac)
             .set_root(&self.root)
             .set_name(&self.version)
-            .set_capabilities(AccessorCapability::Read | AccessorCapability::Write)
-            .set_hints(AccessorHint::ReadStreamable);
+            .set_capability(Capability {
+                read: true,
+                read_can_next: true,
+                write: true,
+
+                ..Default::default()
+            });
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         // ignore creation of dir.
         if path.ends_with('/') {
             return Ok(RpCreate::default());
@@ -387,18 +392,18 @@
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.append() {
+        if args.content_length().is_none() {
             return Err(Error::new(
                 ErrorKind::Unsupported,
-                "append write is not supported",
+                "write without content length is not supported",
             ));
         }
 
         let req = self.ghac_reserve(path).await?;
 
         let resp = self.client.send(req).await?;
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ghac/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ghac/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ghac/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ghac/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ghac/writer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ghac/writer.rs`

 * *Files 3% similar despite different names*

```diff
@@ -58,23 +58,14 @@
         } else {
             Err(parse_error(resp)
                 .await
                 .map(|err| err.with_operation("Backend::ghac_upload"))?)
         }
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let _ = bs;
-
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "output writer doesn't support append",
-        ))
-    }
-
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         let req = self.backend.ghac_commit(self.cache_id, self.size).await?;
         let resp = self.backend.client.send(req).await?;
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -228,21 +228,22 @@
     type Pager = Option<HdfsPager>;
     type BlockingPager = Option<HdfsPager>;
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Hdfs)
             .set_root(&self.root)
-            .set_capabilities(
-                AccessorCapability::Read
-                    | AccessorCapability::Write
-                    | AccessorCapability::List
-                    | AccessorCapability::Blocking,
-            )
-            .set_hints(AccessorHint::ReadSeekable);
+            .set_capability(Capability {
+                read: true,
+                read_can_seek: true,
+                write: true,
+                list: true,
+                blocking: true,
+                ..Default::default()
+            });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let p = build_rooted_abs_path(&self.root, path);
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/writer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/writer.rs`

 * *Files 6% similar despite different names*

```diff
@@ -43,28 +43,14 @@
 impl oio::Write for HdfsWriter<hdrs::AsyncFile> {
     /// # Notes
     ///
     /// File could be partial written, so we will seek to start to make sure
     /// we write the same content.
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         self.f
-            .seek(SeekFrom::Start(0))
-            .await
-            .map_err(parse_io_error)?;
-        self.f.write_all(&bs).await.map_err(parse_io_error)?;
-
-        Ok(())
-    }
-
-    /// # Notes
-    ///
-    /// File could be partial written, so we will seek to start to make sure
-    /// we write the same content.
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        self.f
             .seek(SeekFrom::Start(self.pos))
             .await
             .map_err(parse_io_error)?;
         self.f.write_all(&bs).await.map_err(parse_io_error)?;
         self.pos += bs.len() as u64;
 
         Ok(())
@@ -86,25 +72,14 @@
 
 impl oio::BlockingWrite for HdfsWriter<hdrs::File> {
     /// # Notes
     ///
     /// File could be partial written, so we will seek to start to make sure
     /// we write the same content.
     fn write(&mut self, bs: Bytes) -> Result<()> {
-        self.f.rewind().map_err(parse_io_error)?;
-        self.f.write_all(&bs).map_err(parse_io_error)?;
-
-        Ok(())
-    }
-
-    /// # Notes
-    ///
-    /// File could be partial written, so we will seek to start to make sure
-    /// we write the same content.
-    fn append(&mut self, bs: Bytes) -> Result<()> {
         self.f
             .seek(SeekFrom::Start(self.pos))
             .map_err(parse_io_error)?;
         self.f.write_all(&bs).map_err(parse_io_error)?;
         self.pos += bs.len() as u64;
 
         Ok(())
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/http/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/http/backend.rs`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::fmt::Formatter;
 
 use async_trait::async_trait;
 use http::header;
+use http::header::IF_MATCH;
 use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
 use http::StatusCode;
 use log::debug;
 
 use super::error::parse_error;
@@ -253,23 +254,27 @@
     type Pager = ();
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
         ma.set_scheme(Scheme::Http)
             .set_root(&self.root)
-            .set_capabilities(AccessorCapability::Read)
-            .set_hints(AccessorHint::ReadStreamable);
+            .set_capability(Capability {
+                read: true,
+                read_can_next: true,
+
+                ..Default::default()
+            });
 
         ma
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let resp = self
-            .http_get(path, args.range(), args.if_none_match())
+            .http_get(path, args.range(), args.if_match(), args.if_none_match())
             .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
@@ -281,15 +286,17 @@
 
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
-        let resp = self.http_head(path, args.if_none_match()).await?;
+        let resp = self
+            .http_head(path, args.if_match(), args.if_none_match())
+            .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
             // HTTP Server like nginx could return FORBIDDEN if auto-index
             // is not enabled, we should ignore them.
@@ -302,22 +309,27 @@
 }
 
 impl HttpBackend {
     async fn http_get(
         &self,
         path: &str,
         range: BytesRange,
+        if_match: Option<&str>,
         if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_rooted_abs_path(&self.root, path);
 
         let url = format!("{}{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::get(&url);
 
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
+
         if let Some(if_none_match) = if_none_match {
             req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
         if let Some(auth) = &self.authorization {
             req = req.header(header::AUTHORIZATION, auth.clone())
         }
@@ -332,22 +344,27 @@
 
         self.client.send(req).await
     }
 
     async fn http_head(
         &self,
         path: &str,
+        if_match: Option<&str>,
         if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_rooted_abs_path(&self.root, path);
 
         let url = format!("{}{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::head(&url);
 
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
+
         if let Some(if_none_match) = if_none_match {
             req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
         if let Some(auth) = &self.authorization {
             req = req.header(header::AUTHORIZATION, auth.clone())
         }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/http/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/http/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/http/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/http/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -215,16 +215,21 @@
     type Pager = DirStream;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
         ma.set_scheme(Scheme::Ipfs)
             .set_root(&self.root)
-            .set_capabilities(AccessorCapability::Read | AccessorCapability::List)
-            .set_hints(AccessorHint::ReadStreamable);
+            .set_capability(Capability {
+                read: true,
+                read_can_next: true,
+                list: true,
+
+                ..Default::default()
+            });
 
         ma
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let resp = self.ipfs_get(path, args.range()).await?;
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/ipld.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/ipld.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -69,18 +69,21 @@
     type Pager = IpmfsPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Ipmfs)
             .set_root(&self.root)
-            .set_capabilities(
-                AccessorCapability::Read | AccessorCapability::Write | AccessorCapability::List,
-            )
-            .set_hints(AccessorHint::ReadStreamable);
+            .set_capability(Capability {
+                read: true,
+                read_can_next: true,
+                write: true,
+
+                ..Default::default()
+            });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let resp = self.ipmfs_mkdir(path).await?;
 
@@ -106,18 +109,18 @@
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.append() {
+        if args.content_length().is_none() {
             return Err(Error::new(
                 ErrorKind::Unsupported,
-                "append write is not supported",
+                "write without content length is not supported",
             ));
         }
 
         Ok((
             RpWrite::default(),
             IpmfsWriter::new(self.clone(), path.to_string()),
         ))
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/builder.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/writer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/writer.rs`

 * *Files 11% similar despite different names*

```diff
@@ -51,23 +51,14 @@
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let _ = bs;
-
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "output writer doesn't support append",
-        ))
-    }
-
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt` & `opendal-0.33.0/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/memcached/ascii.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/memcached/ascii.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/memcached/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/memcached/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,21 @@
 
 #[async_trait]
 impl kv::Adapter for Adapter {
     fn metadata(&self) -> kv::Metadata {
         kv::Metadata::new(
             Scheme::Memcached,
             "memcached",
-            AccessorCapability::Read | AccessorCapability::Write,
+            Capability {
+                read: true,
+                write: true,
+                create_dir: true,
+
+                ..Default::default()
+            },
         )
     }
 
     async fn get(&self, key: &str) -> Result<Option<Vec<u8>>> {
         let mut conn = self.conn().await?;
         // TODO: memcache-async have `Sized` limit on key, can we remove it?
         match conn.get(&percent_encode_path(key)).await {
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/memcached/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/memcached/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/memory/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/memory/backend.rs`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 use std::collections::HashMap;
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use parking_lot::Mutex;
 
 use crate::raw::adapters::kv;
-use crate::raw::*;
 use crate::*;
 
 /// In memory service support. (BTreeMap Based)
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
@@ -82,15 +81,22 @@
 
 #[async_trait]
 impl kv::Adapter for Adapter {
     fn metadata(&self) -> kv::Metadata {
         kv::Metadata::new(
             Scheme::Memory,
             &format!("{:?}", &self.inner as *const _),
-            AccessorCapability::Read | AccessorCapability::Write | AccessorCapability::Scan,
+            Capability {
+                read: true,
+                write: true,
+                create_dir: true,
+                scan: true,
+
+                ..Default::default()
+            },
         )
     }
 
     async fn get(&self, path: &str) -> Result<Option<Vec<u8>>> {
         self.blocking_get(path)
     }
 
@@ -140,14 +146,15 @@
         Ok(keys)
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
+    use crate::raw::*;
 
     #[test]
     fn test_accessor_metadata_name() {
         let b1 = MemoryBuilder::default().build().unwrap();
         assert_eq!(b1.info().name(), b1.info().name());
 
         let b2 = MemoryBuilder::default().build().unwrap();
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/memory/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/memory/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/moka/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/moka/backend.rs`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 use async_trait::async_trait;
 use log::debug;
 use moka::sync::CacheBuilder;
 use moka::sync::SegmentedCache;
 
 use crate::raw::adapters::kv;
-use crate::raw::*;
 use crate::*;
 
 /// [moka](https://github.com/moka-rs/moka) backend support.
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
@@ -196,15 +195,20 @@
 
 #[async_trait]
 impl kv::Adapter for Adapter {
     fn metadata(&self) -> kv::Metadata {
         kv::Metadata::new(
             Scheme::Moka,
             self.inner.name().unwrap_or("moka"),
-            AccessorCapability::Read | AccessorCapability::Write,
+            Capability {
+                read: true,
+                write: true,
+
+                ..Default::default()
+            },
         )
     }
 
     async fn get(&self, path: &str) -> Result<Option<Vec<u8>>> {
         self.blocking_get(path)
     }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/moka/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/moka/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/obs/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/obs/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -297,23 +297,27 @@
     type BlockingReader = ();
     type Writer = ObsWriter;
     type BlockingWriter = ();
     type Pager = ObsPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
-        use AccessorCapability::*;
-        use AccessorHint::*;
-
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Obs)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
-            .set_capabilities(Read | Write | Copy | List | Scan)
-            .set_hints(ReadStreamable);
+            .set_capability(Capability {
+                read: true,
+                read_can_next: true,
+                write: true,
+                list: true,
+                scan: true,
+                copy: true,
+                ..Default::default()
+            });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let mut req =
             self.core
@@ -348,18 +352,18 @@
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.append() {
+        if args.content_length().is_none() {
             return Err(Error::new(
                 ErrorKind::Unsupported,
-                "append write is not supported",
+                "write without content length is not supported",
             ));
         }
 
         Ok((
             RpWrite::default(),
             ObsWriter::new(self.core.clone(), args, path.to_string()),
         ))
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/obs/core.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/obs/core.rs`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::Debug;
 use std::fmt::Formatter;
 
+use http::header::CACHE_CONTROL;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
 use http::header::IF_MATCH;
 use http::Request;
 use http::Response;
 use reqsign::HuaweicloudObsCredential;
 use reqsign::HuaweicloudObsCredentialLoader;
@@ -112,30 +113,29 @@
     }
 
     pub fn obs_put_object_request(
         &self,
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
-        if_match: Option<&str>,
+        cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::put(&url);
 
-        if let Some(if_match) = if_match {
-            req = req.header(IF_MATCH, if_match);
-        }
-
         if let Some(size) = size {
             req = req.header(CONTENT_LENGTH, size)
         }
+        if let Some(cache_control) = cache_control {
+            req = req.header(CACHE_CONTROL, cache_control)
+        }
 
         if let Some(mime) = content_type {
             req = req.header(CONTENT_TYPE, mime)
         }
 
         let req = req.body(body).map_err(new_request_build_error)?;
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/obs/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/obs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/obs/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/obs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/obs/pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/obs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/obs/writer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/obs/writer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 #[async_trait]
 impl oio::Write for ObsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let mut req = self.core.obs_put_object_request(
             &self.path,
             Some(bs.len()),
             self.op.content_type(),
-            self.op.if_match(),
+            self.op.cache_control(),
             AsyncBody::Bytes(bs),
         )?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
@@ -62,23 +62,14 @@
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let _ = bs;
-
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "output writer doesn't support append",
-        ))
-    }
-
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/oss/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/oss/backend.rs`

 * *Files 6% similar despite different names*

```diff
@@ -355,24 +355,30 @@
     type BlockingReader = ();
     type Writer = OssWriter;
     type BlockingWriter = ();
     type Pager = OssPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
-        use AccessorCapability::*;
-        use AccessorHint::*;
-
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Oss)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
-            .set_max_batch_operations(1000)
-            .set_capabilities(Read | Write | Copy | List | Scan | Presign | Batch)
-            .set_hints(ReadStreamable);
+            .set_capability(Capability {
+                read: true,
+                read_can_next: true,
+                write: true,
+                list: true,
+                scan: true,
+                copy: true,
+                presign: true,
+                batch: true,
+                batch_max_operations: Some(1000),
+                ..Default::default()
+            });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let resp = self
             .core
@@ -388,48 +394,38 @@
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let resp = self
             .core
-            .oss_get_object(path, args.range(), args.if_none_match())
+            .oss_get_object(
+                path,
+                args.range(),
+                args.if_match(),
+                args.if_none_match(),
+                args.override_content_disposition(),
+            )
             .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        let upload_id = if args.append() {
-            let resp = self.core.oss_initiate_upload(path, &args).await?;
-            match resp.status() {
-                StatusCode::OK => {
-                    let bs = resp.into_body().bytes().await?;
-                    let result: InitiateMultipartUploadResult =
-                        quick_xml::de::from_reader(bs.reader())
-                            .map_err(new_xml_deserialize_error)?;
-                    Some(result.upload_id)
-                }
-                _ => return Err(parse_error(resp).await?),
-            }
-        } else {
-            None
-        };
-
         Ok((
             RpWrite::default(),
-            OssWriter::new(self.core.clone(), args, path.to_string(), upload_id),
+            OssWriter::new(self.core.clone(), path, args),
         ))
     }
 
     async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
         let resp = self.core.oss_copy_object(from, to).await?;
         let status = resp.status();
 
@@ -446,15 +442,15 @@
         if path == "/" {
             let m = Metadata::new(EntryMode::DIR);
             return Ok(RpStat::new(m));
         }
 
         let resp = self
             .core
-            .oss_head_object(path, args.if_none_match())
+            .oss_head_object(path, args.if_match(), args.if_none_match())
             .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
             StatusCode::NOT_FOUND if path.ends_with('/') => {
@@ -491,19 +487,26 @@
             OssPager::new(self.core.clone(), path, "", args.limit()),
         ))
     }
 
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         // We will not send this request out, just for signing.
         let mut req = match args.operation() {
-            PresignOperation::Stat(_) => self.core.oss_head_object_request(path, true, None)?,
-            PresignOperation::Read(v) => {
+            PresignOperation::Stat(v) => {
                 self.core
-                    .oss_get_object_request(path, v.range(), true, None)?
+                    .oss_head_object_request(path, true, v.if_match(), v.if_none_match())?
             }
+            PresignOperation::Read(v) => self.core.oss_get_object_request(
+                path,
+                v.range(),
+                true,
+                v.if_match(),
+                v.if_none_match(),
+                v.override_content_disposition(),
+            )?,
             PresignOperation::Write(v) => self.core.oss_put_object_request(
                 path,
                 None,
                 v.content_type(),
                 v.content_disposition(),
                 v.cache_control(),
                 AsyncBody::Empty,
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/oss/core.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/oss/core.rs`

 * *Files 6% similar despite different names*

```diff
@@ -20,28 +20,33 @@
 use std::time::Duration;
 
 use bytes::Bytes;
 use http::header::CACHE_CONTROL;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
+use http::header::IF_MATCH;
 use http::header::IF_NONE_MATCH;
 use http::header::RANGE;
 use http::Request;
 use http::Response;
 use reqsign::AliyunCredential;
 use reqsign::AliyunLoader;
 use reqsign::AliyunOssSigner;
 use serde::Deserialize;
 use serde::Serialize;
 
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
+mod constants {
+    pub const RESPONSE_CONTENT_DISPOSITION: &str = "response-content-disposition";
+}
+
 pub struct OssCore {
     pub root: String,
     pub bucket: String,
     /// buffered host string
     ///
     /// format: <bucket-name>.<endpoint-domain-name>
     pub host: String,
@@ -144,30 +149,49 @@
     }
 
     pub fn oss_get_object_request(
         &self,
         path: &str,
         range: BytesRange,
         is_presign: bool,
+        if_match: Option<&str>,
         if_none_match: Option<&str>,
+        override_content_disposition: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
         let endpoint = self.get_endpoint(is_presign);
-        let url = format!("{}/{}", endpoint, percent_encode_path(&p));
+        let mut url = format!("{}/{}", endpoint, percent_encode_path(&p));
+
+        // Add query arguments to the URL based on response overrides
+        let mut query_args = Vec::new();
+        if let Some(override_content_disposition) = override_content_disposition {
+            query_args.push(format!(
+                "{}={}",
+                constants::RESPONSE_CONTENT_DISPOSITION,
+                percent_encode_path(override_content_disposition)
+            ))
+        }
+
+        if !query_args.is_empty() {
+            url.push_str(&format!("?{}", query_args.join("&")));
+        }
 
         let mut req = Request::get(&url);
         req = req.header(CONTENT_TYPE, "application/octet-stream");
 
         if !range.is_full() {
             req = req.header(RANGE, range.to_header());
             // Adding `x-oss-range-behavior` header to use standard behavior.
             // ref: https://help.aliyun.com/document_detail/39571.html
             req = req.header("x-oss-range-behavior", "standard");
         }
 
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match)
+        }
         if let Some(if_none_match) = if_none_match {
             req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
@@ -188,21 +212,25 @@
         Ok(req)
     }
 
     pub fn oss_head_object_request(
         &self,
         path: &str,
         is_presign: bool,
+        if_match: Option<&str>,
         if_none_match: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
         let endpoint = self.get_endpoint(is_presign);
         let url = format!("{}/{}", endpoint, percent_encode_path(&p));
 
         let mut req = Request::head(&url);
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match)
+        }
         if let Some(if_none_match) = if_none_match {
             req = req.header(IF_NONE_MATCH, if_none_match);
         }
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
@@ -235,28 +263,37 @@
         Ok(req)
     }
 
     pub async fn oss_get_object(
         &self,
         path: &str,
         range: BytesRange,
+        if_match: Option<&str>,
         if_none_match: Option<&str>,
+        override_content_disposition: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.oss_get_object_request(path, range, false, if_none_match)?;
-
+        let mut req = self.oss_get_object_request(
+            path,
+            range,
+            false,
+            if_match,
+            if_none_match,
+            override_content_disposition,
+        )?;
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
     pub async fn oss_head_object(
         &self,
         path: &str,
+        if_match: Option<&str>,
         if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.oss_head_object_request(path, false, if_none_match)?;
+        let mut req = self.oss_head_object_request(path, false, if_match, if_none_match)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
     pub async fn oss_put_object(
         &self,
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/oss/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/oss/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/oss/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/oss/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/oss/pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/oss/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/oss/writer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/writer.rs`

 * *Files 26% similar despite different names*

```diff
@@ -23,123 +23,67 @@
 
 use super::core::*;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct OssWriter {
-    core: Arc<OssCore>,
+pub struct WasabiWriter {
+    core: Arc<WasabiCore>,
 
     op: OpWrite,
     path: String,
-    upload_id: Option<String>,
-    parts: Vec<MultipartUploadPart>,
 }
 
-impl OssWriter {
-    pub fn new(core: Arc<OssCore>, op: OpWrite, path: String, upload_id: Option<String>) -> Self {
-        OssWriter {
-            core,
-            op,
-            path,
-            upload_id,
-            parts: vec![],
-        }
+impl WasabiWriter {
+    pub fn new(core: Arc<WasabiCore>, op: OpWrite, path: String) -> Self {
+        WasabiWriter { core, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for OssWriter {
+impl oio::Write for WasabiWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut req = self.core.oss_put_object_request(
-            &self.path,
-            Some(bs.len()),
-            self.op.content_type(),
-            self.op.content_disposition(),
-            self.op.cache_control(),
-            AsyncBody::Bytes(bs),
-            false,
-        )?;
-
-        self.core.sign(&mut req).await?;
-
-        let resp = self.core.send(req).await?;
-
-        let status = resp.status();
-
-        match status {
-            StatusCode::CREATED | StatusCode::OK => {
-                resp.into_body().consume().await?;
-                Ok(())
+        if self.op.content_length().unwrap_or_default() == bs.len() as u64 {
+            let resp = self
+                .core
+                .put_object(
+                    &self.path,
+                    Some(bs.len()),
+                    self.op.content_type(),
+                    self.op.content_disposition(),
+                    self.op.cache_control(),
+                    AsyncBody::Bytes(bs),
+                )
+                .await?;
+
+            match resp.status() {
+                StatusCode::CREATED | StatusCode::OK => {
+                    resp.into_body().consume().await?;
+                    Ok(())
+                }
+                _ => Err(parse_error(resp).await?),
             }
-            _ => Err(parse_error(resp).await?),
-        }
-    }
-
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let upload_id = self.upload_id.as_ref().expect(
-            "Writer doesn't have upload id, but users trying to call append, must be buggy",
-        );
-        // Aliyun OSS requires part number must between [1..=10000]
-        let part_number = self.parts.len() + 1;
-        let mut req = self
-            .core
-            .oss_upload_part_request(
-                &self.path,
-                upload_id,
-                part_number,
-                false,
-                Some(bs.len() as u64),
-                AsyncBody::Bytes(bs),
-            )
-            .await?;
-
-        self.core.sign(&mut req).await?;
-
-        let resp = self.core.send(req).await?;
-        match resp.status() {
-            StatusCode::OK => {
-                let etag = parse_etag(resp.headers())?
-                    .ok_or_else(|| {
-                        Error::new(
-                            ErrorKind::Unexpected,
-                            "ETag not present in returning response",
-                        )
-                    })?
-                    .to_string();
-                resp.into_body().consume().await?;
-                self.parts.push(MultipartUploadPart { part_number, etag });
-                Ok(())
+        } else {
+            let resp = self
+                .core
+                .append_object(&self.path, Some(bs.len()), AsyncBody::Bytes(bs))
+                .await?;
+
+            match resp.status() {
+                StatusCode::CREATED | StatusCode::OK | StatusCode::NO_CONTENT => {
+                    resp.into_body().consume().await?;
+                    Ok(())
+                }
+                _ => Err(parse_error(resp).await?),
             }
-            _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn abort(&mut self) -> Result<()> {
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "output writer doesn't support abort",
-        ))
+        Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
-        let upload_id = if let Some(upload_id) = &self.upload_id {
-            upload_id
-        } else {
-            return Ok(());
-        };
-
-        let resp = self
-            .core
-            .oss_complete_multipart_upload_request(&self.path, upload_id, false, &self.parts)
-            .await?;
-        match resp.status() {
-            StatusCode::OK => {
-                resp.into_body().consume().await?;
-
-                Ok(())
-            }
-            _ => Err(parse_error(resp).await?),
-        }
+        Ok(())
     }
 }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/redis/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/redis/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -312,15 +312,21 @@
 
 #[async_trait]
 impl kv::Adapter for Adapter {
     fn metadata(&self) -> kv::Metadata {
         kv::Metadata::new(
             Scheme::Redis,
             &self.client.get_connection_info().addr.to_string(),
-            AccessorCapability::Read | AccessorCapability::Write,
+            Capability {
+                read: true,
+                write: true,
+                create_dir: true,
+
+                ..Default::default()
+            },
         )
     }
 
     async fn get(&self, key: &str) -> Result<Option<Vec<u8>>> {
         let mut conn = self.conn().await?;
         let bs: Option<Vec<u8>> = conn.get(key).await?;
         Ok(bs)
@@ -346,10 +352,12 @@
         conn.append(key, value).await?;
         Ok(())
     }
 }
 
 impl From<RedisError> for Error {
     fn from(e: RedisError) -> Self {
-        Error::new(ErrorKind::Unexpected, e.category()).set_source(e)
+        Error::new(ErrorKind::Unexpected, e.category())
+            .set_source(e)
+            .set_temporary()
     }
 }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/redis/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/redis/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/rocksdb/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/rocksdb/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 use std::fmt::Formatter;
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use rocksdb::DB;
 
 use crate::raw::adapters::kv;
-use crate::raw::*;
 use crate::Result;
 use crate::*;
 
 /// Rocksdb service support.
 ///
 /// # Capabilities
 ///
@@ -156,15 +155,19 @@
 
 #[async_trait]
 impl kv::Adapter for Adapter {
     fn metadata(&self) -> kv::Metadata {
         kv::Metadata::new(
             Scheme::Rocksdb,
             &self.db.path().to_string_lossy(),
-            AccessorCapability::Read | AccessorCapability::Write,
+            Capability {
+                read: true,
+                write: true,
+                ..Default::default()
+            },
         )
     }
 
     async fn get(&self, path: &str) -> Result<Option<Vec<u8>>> {
         self.blocking_get(path)
     }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/rocksdb/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/rocksdb/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/s3/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/s3/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -903,24 +903,39 @@
     type BlockingReader = ();
     type Writer = S3Writer;
     type BlockingWriter = ();
     type Pager = S3Pager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
-        use AccessorCapability::*;
-        use AccessorHint::*;
-
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::S3)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
-            .set_max_batch_operations(1000)
-            .set_capabilities(Read | Write | List | Scan | Presign | Batch | Copy)
-            .set_hints(ReadStreamable);
+            .set_capability(Capability {
+                stat: true,
+                stat_with_if_match: true,
+                stat_with_if_none_match: true,
+
+                read: true,
+                read_can_next: true,
+                read_with_if_match: true,
+                read_with_if_none_match: true,
+                read_with_override_content_disposition: true,
+
+                write: true,
+                list: true,
+                scan: true,
+                copy: true,
+                presign: true,
+                batch: true,
+                batch_max_operations: Some(1000),
+
+                ..Default::default()
+            });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let mut req =
             self.core
@@ -940,61 +955,38 @@
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let resp = self
             .core
-            .s3_get_object(path, args.range(), args.if_none_match())
+            .s3_get_object(
+                path,
+                args.range(),
+                args.if_none_match(),
+                args.if_match(),
+                args.override_content_disposition(),
+            )
             .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        let upload_id = if args.append() {
-            let resp = self
-                .core
-                .s3_initiate_multipart_upload(
-                    path,
-                    args.content_type(),
-                    args.content_disposition(),
-                    args.cache_control(),
-                )
-                .await?;
-
-            let status = resp.status();
-
-            match status {
-                StatusCode::OK => {
-                    let bs = resp.into_body().bytes().await?;
-
-                    let result: InitiateMultipartUploadResult =
-                        quick_xml::de::from_reader(bs.reader())
-                            .map_err(new_xml_deserialize_error)?;
-
-                    Some(result.upload_id)
-                }
-                _ => return Err(parse_error(resp).await?),
-            }
-        } else {
-            None
-        };
-
         Ok((
             RpWrite::default(),
-            S3Writer::new(self.core.clone(), args, path.to_string(), upload_id),
+            S3Writer::new(self.core.clone(), path, args),
         ))
     }
 
     async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
         let resp = self.core.s3_copy_object(from, to).await?;
 
         let status = resp.status();
@@ -1013,15 +1005,18 @@
 
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
-        let resp = self.core.s3_head_object(path, args.if_none_match()).await?;
+        let resp = self
+            .core
+            .s3_head_object(path, args.if_none_match(), args.if_match())
+            .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
             StatusCode::NOT_FOUND if path.ends_with('/') => {
                 Ok(RpStat::new(Metadata::new(EntryMode::DIR)))
@@ -1055,22 +1050,24 @@
         ))
     }
 
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         // We will not send this request out, just for signing.
         let mut req = match args.operation() {
             PresignOperation::Stat(v) => {
-                self.core.s3_head_object_request(path, v.if_none_match())?
+                self.core
+                    .s3_head_object_request(path, v.if_none_match(), v.if_match())?
             }
             PresignOperation::Read(v) => self.core.s3_get_object_request(
                 path,
                 v.range(),
                 v.override_content_disposition(),
                 v.override_cache_control(),
                 v.if_none_match(),
+                v.if_match(),
             )?,
             PresignOperation::Write(_) => {
                 self.core
                     .s3_put_object_request(path, None, None, None, None, AsyncBody::Empty)?
             }
         };
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/s3/compatible_services.md` & `opendal-0.33.0/local_dependencies/opendal/src/services/s3/compatible_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/s3/core.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 use backon::Retryable;
 use bytes::Bytes;
 use http::header::HeaderName;
 use http::header::CACHE_CONTROL;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
-use http::header::IF_NONE_MATCH;
 use http::HeaderValue;
 use http::Request;
 use http::Response;
 use once_cell::sync::Lazy;
 use reqsign::AwsCredential;
 use reqsign::AwsLoader;
 use reqsign::AwsV4Signer;
@@ -53,29 +52,35 @@
         "x-amz-server-side-encryption-customer-key";
     pub const X_AMZ_SERVER_SIDE_ENCRYPTION_CUSTOMER_KEY_MD5: &str =
         "x-amz-server-side-encryption-customer-key-md5";
     pub const X_AMZ_SERVER_SIDE_ENCRYPTION_AWS_KMS_KEY_ID: &str =
         "x-amz-server-side-encryption-aws-kms-key-id";
     pub const X_AMZ_STORAGE_CLASS: &str = "x-amz-storage-class";
 
+    #[allow(dead_code)]
     pub const X_AMZ_COPY_SOURCE_SERVER_SIDE_ENCRYPTION_CUSTOMER_ALGORITHM: &str =
         "x-amz-copy-source-server-side-encryption-customer-algorithm";
+    #[allow(dead_code)]
     pub const X_AMZ_COPY_SOURCE_SERVER_SIDE_ENCRYPTION_CUSTOMER_KEY: &str =
         "x-amz-copy-source-server-side-encryption-customer-key";
+    #[allow(dead_code)]
     pub const X_AMZ_COPY_SOURCE_SERVER_SIDE_ENCRYPTION_CUSTOMER_KEY_MD5: &str =
         "x-amz-copy-source-server-side-encryption-customer-key-md5";
 
     pub const RESPONSE_CONTENT_DISPOSITION: &str = "response-content-disposition";
     pub const RESPONSE_CACHE_CONTROL: &str = "response-cache-control";
+
+    pub const DESTINATION: &str = "Destination";
+    pub const OVERWRITE: &str = "Overwrite";
 }
 
 static BACKOFF: Lazy<ExponentialBuilder> =
     Lazy::new(|| ExponentialBuilder::default().with_jitter());
 
-pub struct S3Core {
+pub struct WasabiCore {
     pub bucket: String,
     pub endpoint: String,
     pub root: String,
     pub server_side_encryption: Option<HeaderValue>,
     pub server_side_encryption_aws_kms_key_id: Option<HeaderValue>,
     pub server_side_encryption_customer_algorithm: Option<HeaderValue>,
     pub server_side_encryption_customer_key: Option<HeaderValue>,
@@ -83,25 +88,25 @@
     pub default_storage_class: Option<HeaderValue>,
 
     pub signer: AwsV4Signer,
     pub loader: AwsLoader,
     pub client: HttpClient,
 }
 
-impl Debug for S3Core {
+impl Debug for WasabiCore {
     fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
-        f.debug_struct("S3Core")
+        f.debug_struct("WasabiCore")
             .field("bucket", &self.bucket)
             .field("endpoint", &self.endpoint)
             .field("root", &self.root)
             .finish_non_exhaustive()
     }
 }
 
-impl S3Core {
+impl WasabiCore {
     /// If credential is not found, we will not sign the request.
     async fn load_credential(&self) -> Result<Option<AwsCredential>> {
         let cred = { || self.loader.load() }
             .retry(&*BACKOFF)
             .await
             .map_err(new_request_credential_error)?;
 
@@ -138,15 +143,15 @@
     pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
         self.client.send(req).await
     }
 
     /// # Note
     ///
     /// header like X_AMZ_SERVER_SIDE_ENCRYPTION doesn't need to set while
-    //  get or stat.
+    /// get or stat.
     pub fn insert_sse_headers(
         &self,
         mut req: http::request::Builder,
         is_write: bool,
     ) -> http::request::Builder {
         if is_write {
             if let Some(v) = &self.server_side_encryption {
@@ -197,40 +202,40 @@
             )
         }
 
         req
     }
 }
 
-impl S3Core {
-    pub fn s3_head_object_request(
+impl WasabiCore {
+    pub fn head_object_request(
         &self,
         path: &str,
         if_none_match: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::head(&url);
 
         req = self.insert_sse_headers(req, false);
 
         if let Some(if_none_match) = if_none_match {
-            req = req.header(IF_NONE_MATCH, if_none_match);
+            req = req.header(http::header::IF_NONE_MATCH, if_none_match);
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub fn s3_get_object_request(
+    pub fn get_object_request(
         &self,
         path: &str,
         range: BytesRange,
         override_content_disposition: Option<&str>,
         override_cache_control: Option<&str>,
         if_none_match: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
@@ -262,42 +267,42 @@
         let mut req = Request::get(&url);
 
         if !range.is_full() {
             req = req.header(http::header::RANGE, range.to_header());
         }
 
         if let Some(if_none_match) = if_none_match {
-            req = req.header(IF_NONE_MATCH, if_none_match);
+            req = req.header(http::header::IF_NONE_MATCH, if_none_match);
         }
 
         // Set SSE headers.
         // TODO: how will this work with presign?
         req = self.insert_sse_headers(req, false);
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn s3_get_object(
+    pub async fn get_object(
         &self,
         path: &str,
         range: BytesRange,
         if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.s3_get_object_request(path, range, None, None, if_none_match)?;
+        let mut req = self.get_object_request(path, range, None, None, if_none_match)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub fn s3_put_object_request(
+    pub fn put_object_request(
         &self,
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
         cache_control: Option<&str>,
         body: AsyncBody,
@@ -334,45 +339,41 @@
 
         // Set body
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn s3_head_object(
+    pub async fn head_object(
         &self,
         path: &str,
         if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.s3_head_object_request(path, if_none_match)?;
+        let mut req = self.head_object_request(path, if_none_match)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn s3_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::delete(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn s3_copy_object(
-        &self,
-        from: &str,
-        to: &str,
-    ) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn copy_object(&self, from: &str, to: &str) -> Result<Response<IncomingAsyncBody>> {
         let from = build_abs_path(&self.root, from);
         let to = build_abs_path(&self.root, to);
 
         let source = format!("{}/{}", self.bucket, percent_encode_path(&from));
         let target = format!("{}/{}", self.endpoint, percent_encode_path(&to));
 
         let mut req = Request::put(&target);
@@ -424,31 +425,28 @@
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
     /// Make this functions as `pub(suber)` because `DirStream` depends
     /// on this.
-    pub async fn s3_list_objects(
+    pub async fn list_objects(
         &self,
         path: &str,
         continuation_token: &str,
         delimiter: &str,
         limit: Option<usize>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let mut url = format!(
-            "{}?list-type=2&prefix={}",
+            "{}?list-type=2&delimiter={delimiter}&prefix={}",
             self.endpoint,
             percent_encode_path(&p)
         );
-        if !delimiter.is_empty() {
-            write!(url, "&delimiter={delimiter}").expect("write into string must succeed");
-        }
         if let Some(limit) = limit {
             write!(url, "&max-keys={limit}").expect("write into string must succeed");
         }
         if !continuation_token.is_empty() {
             // AWS S3 could return continuation-token that contains `=`
             // which could lead `reqsign` parse query wrongly.
             // URL encode continuation-token before starting signing so that
@@ -466,15 +464,15 @@
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn s3_initiate_multipart_upload(
+    pub async fn initiate_multipart_upload(
         &self,
         path: &str,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
         cache_control: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
@@ -508,15 +506,15 @@
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub fn s3_upload_part_request(
+    pub fn upload_part_request(
         &self,
         path: &str,
         upload_id: &str,
         part_number: usize,
         size: Option<u64>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
@@ -541,15 +539,15 @@
 
         // Set body
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn s3_complete_multipart_upload(
+    pub async fn complete_multipart_upload(
         &self,
         path: &str,
         upload_id: &str,
         parts: &[CompleteMultipartUploadRequestPart],
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
@@ -580,15 +578,15 @@
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
     /// Abort an on-going multipart upload.
-    pub async fn s3_abort_multipart_upload(
+    pub async fn abort_multipart_upload(
         &self,
         path: &str,
         upload_id: &str,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
@@ -601,18 +599,15 @@
         let mut req = Request::delete(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
-    pub async fn s3_delete_objects(
-        &self,
-        paths: Vec<String>,
-    ) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn delete_objects(&self, paths: Vec<String>) -> Result<Response<IncomingAsyncBody>> {
         let url = format!("{}/?delete", self.endpoint);
 
         let req = Request::post(&url);
 
         let content = quick_xml::se::to_string(&DeleteObjectsRequest {
             object: paths
                 .into_iter()
@@ -634,14 +629,90 @@
             .body(AsyncBody::Bytes(Bytes::from(content)))
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
+
+    pub async fn put_object(
+        &self,
+        path: &str,
+        size: Option<usize>,
+        content_type: Option<&str>,
+        content_disposition: Option<&str>,
+        cache_control: Option<&str>,
+        body: AsyncBody,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = self.put_object_request(
+            path,
+            size,
+            content_type,
+            content_disposition,
+            cache_control,
+            body,
+        )?;
+
+        self.sign(&mut req).await?;
+
+        self.send(req).await
+    }
+
+    pub async fn rename_object(&self, from: &str, to: &str) -> Result<Response<IncomingAsyncBody>> {
+        let from = percent_encode_path(build_abs_path(&self.root, from).as_str());
+        let to = percent_encode_path(build_abs_path(&self.root, to).as_str());
+
+        let url = format!("{}/{}", self.endpoint, from);
+
+        let mut req = Request::builder().method("MOVE").uri(url);
+
+        // Set SSE headers.
+        req = self.insert_sse_headers(req, true);
+
+        let mut req = req
+            .header(constants::DESTINATION, to)
+            .header(constants::OVERWRITE, "true")
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        self.sign(&mut req).await?;
+
+        self.send(req).await
+    }
+
+    pub async fn append_object(
+        &self,
+        path: &str,
+        size: Option<usize>,
+        body: AsyncBody,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        let url = format!("{}/{}?append", self.endpoint, percent_encode_path(&p));
+
+        let mut req = Request::put(&url);
+
+        if let Some(size) = size {
+            req = req.header(CONTENT_LENGTH, size)
+        }
+
+        // Set storage class header
+        if let Some(v) = &self.default_storage_class {
+            req = req.header(HeaderName::from_static(constants::X_AMZ_STORAGE_CLASS), v);
+        }
+
+        // Set SSE headers.
+        req = self.insert_sse_headers(req, true);
+
+        let mut req = req.body(body).map_err(new_request_build_error)?;
+
+        self.sign(&mut req).await?;
+
+        self.send(req).await
+    }
 }
 
 /// Result of CreateMultipartUpload
 #[derive(Default, Debug, Deserialize)]
 #[serde(default, rename_all = "PascalCase")]
 pub struct InitiateMultipartUploadResult {
     pub upload_id: String,
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/s3/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/s3/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/s3/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/s3/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/s3/pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/s3/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/s3/writer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/s3/writer.rs`

 * *Files 25% similar despite different names*

```diff
@@ -14,54 +14,57 @@
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::sync::Arc;
 
 use async_trait::async_trait;
+use bytes::Buf;
 use bytes::Bytes;
 use http::StatusCode;
 
 use super::core::*;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct S3Writer {
     core: Arc<S3Core>,
 
     op: OpWrite,
     path: String,
-
     upload_id: Option<String>,
+
     parts: Vec<CompleteMultipartUploadRequestPart>,
+    buffer: oio::VectorCursor,
+    buffer_size: usize,
 }
 
 impl S3Writer {
-    pub fn new(core: Arc<S3Core>, op: OpWrite, path: String, upload_id: Option<String>) -> Self {
+    pub fn new(core: Arc<S3Core>, path: &str, op: OpWrite) -> Self {
         S3Writer {
             core,
-
+            path: path.to_string(),
             op,
-            path,
-            upload_id,
+
+            upload_id: None,
             parts: vec![],
+            buffer: oio::VectorCursor::new(),
+            // The part size must be 5 MiB to 5 GiB. There is no minimum
+            // size limit on the last part of your multipart upload.
+            //
+            // We pick the default value as 8 MiB for better thoughput.
+            //
+            // TODO: allow this value to be configured.
+            buffer_size: 8 * 1024 * 1024,
         }
     }
-}
-
-#[async_trait]
-impl oio::Write for S3Writer {
-    async fn write(&mut self, bs: Bytes) -> Result<()> {
-        debug_assert!(
-            self.upload_id.is_none(),
-            "Writer initiated with upload id, but users trying to call write, must be buggy"
-        );
 
+    async fn write_oneshot(&self, bs: Bytes) -> Result<()> {
         let mut req = self.core.s3_put_object_request(
             &self.path,
             Some(bs.len()),
             self.op.content_type(),
             self.op.content_disposition(),
             self.op.cache_control(),
             AsyncBody::Bytes(bs),
@@ -78,18 +81,45 @@
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let upload_id = self.upload_id.as_ref().expect(
-            "Writer doesn't have upload id, but users trying to call append, must be buggy",
-        );
+    async fn initiate_upload(&self) -> Result<String> {
+        let resp = self
+            .core
+            .s3_initiate_multipart_upload(
+                &self.path,
+                self.op.content_type(),
+                self.op.content_disposition(),
+                self.op.cache_control(),
+            )
+            .await?;
+
+        let status = resp.status();
+
+        match status {
+            StatusCode::OK => {
+                let bs = resp.into_body().bytes().await?;
+
+                let result: InitiateMultipartUploadResult =
+                    quick_xml::de::from_reader(bs.reader()).map_err(new_xml_deserialize_error)?;
+
+                Ok(result.upload_id)
+            }
+            _ => Err(parse_error(resp).await?),
+        }
+    }
+
+    async fn write_part(
+        &self,
+        upload_id: &str,
+        bs: Bytes,
+    ) -> Result<CompleteMultipartUploadRequestPart> {
         // AWS S3 requires part number must between [1..=10000]
         let part_number = self.parts.len() + 1;
 
         let mut req = self.core.s3_upload_part_request(
             &self.path,
             upload_id,
             part_number,
@@ -112,20 +142,63 @@
                             "ETag not present in returning response",
                         )
                     })?
                     .to_string();
 
                 resp.into_body().consume().await?;
 
-                self.parts
-                    .push(CompleteMultipartUploadRequestPart { part_number, etag });
+                Ok(CompleteMultipartUploadRequestPart { part_number, etag })
+            }
+            _ => Err(parse_error(resp).await?),
+        }
+    }
+}
+
+#[async_trait]
+impl oio::Write for S3Writer {
+    async fn write(&mut self, bs: Bytes) -> Result<()> {
+        let upload_id = match &self.upload_id {
+            Some(upload_id) => upload_id,
+            None => {
+                if self.op.content_length().unwrap_or_default() == bs.len() as u64 {
+                    return self.write_oneshot(bs).await;
+                } else {
+                    let upload_id = self.initiate_upload().await?;
+                    self.upload_id = Some(upload_id);
+                    self.upload_id.as_deref().unwrap()
+                }
+            }
+        };
+
+        // Ignore empty bytes
+        if bs.is_empty() {
+            return Ok(());
+        }
+
+        self.buffer.push(bs);
+        // Return directly if the buffer is not full
+        if self.buffer.len() <= self.buffer_size {
+            return Ok(());
+        }
+
+        let bs = self.buffer.peak_at_least(self.buffer_size);
+        let size = bs.len();
 
+        match self.write_part(upload_id, bs).await {
+            Ok(part) => {
+                self.buffer.take(size);
+                self.parts.push(part);
                 Ok(())
             }
-            _ => Err(parse_error(resp).await?),
+            Err(e) => {
+                // If the upload fails, we should pop the given bs to make sure
+                // write is re-enter safe.
+                self.buffer.pop();
+                Err(e)
+            }
         }
     }
 
     async fn abort(&mut self) -> Result<()> {
         let upload_id = if let Some(upload_id) = &self.upload_id {
             upload_id
         } else {
@@ -149,14 +222,29 @@
     async fn close(&mut self) -> Result<()> {
         let upload_id = if let Some(upload_id) = &self.upload_id {
             upload_id
         } else {
             return Ok(());
         };
 
+        // Make sure internal buffer has been flushed.
+        if !self.buffer.is_empty() {
+            let bs = self.buffer.peak_exact(self.buffer.len());
+
+            match self.write_part(upload_id, bs).await {
+                Ok(part) => {
+                    self.buffer.clear();
+                    self.parts.push(part);
+                }
+                Err(e) => {
+                    return Err(e);
+                }
+            }
+        }
+
         let resp = self
             .core
             .s3_complete_multipart_upload(&self.path, upload_id, &self.parts)
             .await?;
 
         let status = resp.status();
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/sled/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/sled/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::fmt::Formatter;
 
 use async_trait::async_trait;
 
 use crate::raw::adapters::kv;
-use crate::raw::*;
 use crate::Builder;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Scheme;
 use crate::*;
 
 /// Sled service support.
@@ -137,16 +136,25 @@
         ds.finish()
     }
 }
 
 #[async_trait]
 impl kv::Adapter for Adapter {
     fn metadata(&self) -> kv::Metadata {
-        use AccessorCapability::*;
-        kv::Metadata::new(Scheme::Sled, &self.datadir, Read | Write | Scan | Blocking)
+        kv::Metadata::new(
+            Scheme::Sled,
+            &self.datadir,
+            Capability {
+                read: true,
+                write: true,
+                scan: true,
+                blocking: true,
+                ..Default::default()
+            },
+        )
     }
 
     async fn get(&self, path: &str) -> Result<Option<Vec<u8>>> {
         self.blocking_get(path)
     }
 
     fn blocking_get(&self, path: &str) -> Result<Option<Vec<u8>>> {
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/sled/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/sled/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -893,24 +893,30 @@
     type BlockingReader = ();
     type Writer = WasabiWriter;
     type BlockingWriter = ();
     type Pager = WasabiPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
-        use AccessorCapability::*;
-        use AccessorHint::*;
-
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Wasabi)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
-            .set_max_batch_operations(1000)
-            .set_capabilities(Read | Write | List | Scan | Presign | Batch | Copy | Rename)
-            .set_hints(ReadStreamable);
+            .set_capability(Capability {
+                read: true,
+                read_can_next: true,
+                write: true,
+                list: true,
+                scan: true,
+                copy: true,
+                presign: true,
+                batch: true,
+                rename: true,
+                ..Default::default()
+            });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let mut req =
             self.core
@@ -947,15 +953,15 @@
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         Ok((
             RpWrite::default(),
-            WasabiWriter::new(self.core.clone(), args, path.to_string(), None),
+            WasabiWriter::new(self.core.clone(), args, path.to_string()),
         ))
     }
 
     async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
         let resp = self.core.copy_object(from, to).await?;
 
         let status = resp.status();
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/core.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/s3/core.rs`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 use backon::Retryable;
 use bytes::Bytes;
 use http::header::HeaderName;
 use http::header::CACHE_CONTROL;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
+use http::header::IF_MATCH;
+use http::header::IF_NONE_MATCH;
 use http::HeaderValue;
 use http::Request;
 use http::Response;
 use once_cell::sync::Lazy;
 use reqsign::AwsCredential;
 use reqsign::AwsLoader;
 use reqsign::AwsV4Signer;
@@ -52,35 +54,29 @@
         "x-amz-server-side-encryption-customer-key";
     pub const X_AMZ_SERVER_SIDE_ENCRYPTION_CUSTOMER_KEY_MD5: &str =
         "x-amz-server-side-encryption-customer-key-md5";
     pub const X_AMZ_SERVER_SIDE_ENCRYPTION_AWS_KMS_KEY_ID: &str =
         "x-amz-server-side-encryption-aws-kms-key-id";
     pub const X_AMZ_STORAGE_CLASS: &str = "x-amz-storage-class";
 
-    #[allow(dead_code)]
     pub const X_AMZ_COPY_SOURCE_SERVER_SIDE_ENCRYPTION_CUSTOMER_ALGORITHM: &str =
         "x-amz-copy-source-server-side-encryption-customer-algorithm";
-    #[allow(dead_code)]
     pub const X_AMZ_COPY_SOURCE_SERVER_SIDE_ENCRYPTION_CUSTOMER_KEY: &str =
         "x-amz-copy-source-server-side-encryption-customer-key";
-    #[allow(dead_code)]
     pub const X_AMZ_COPY_SOURCE_SERVER_SIDE_ENCRYPTION_CUSTOMER_KEY_MD5: &str =
         "x-amz-copy-source-server-side-encryption-customer-key-md5";
 
     pub const RESPONSE_CONTENT_DISPOSITION: &str = "response-content-disposition";
     pub const RESPONSE_CACHE_CONTROL: &str = "response-cache-control";
-
-    pub const DESTINATION: &str = "Destination";
-    pub const OVERWRITE: &str = "Overwrite";
 }
 
 static BACKOFF: Lazy<ExponentialBuilder> =
     Lazy::new(|| ExponentialBuilder::default().with_jitter());
 
-pub struct WasabiCore {
+pub struct S3Core {
     pub bucket: String,
     pub endpoint: String,
     pub root: String,
     pub server_side_encryption: Option<HeaderValue>,
     pub server_side_encryption_aws_kms_key_id: Option<HeaderValue>,
     pub server_side_encryption_customer_algorithm: Option<HeaderValue>,
     pub server_side_encryption_customer_key: Option<HeaderValue>,
@@ -88,25 +84,25 @@
     pub default_storage_class: Option<HeaderValue>,
 
     pub signer: AwsV4Signer,
     pub loader: AwsLoader,
     pub client: HttpClient,
 }
 
-impl Debug for WasabiCore {
+impl Debug for S3Core {
     fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
-        f.debug_struct("WasabiCore")
+        f.debug_struct("S3Core")
             .field("bucket", &self.bucket)
             .field("endpoint", &self.endpoint)
             .field("root", &self.root)
             .finish_non_exhaustive()
     }
 }
 
-impl WasabiCore {
+impl S3Core {
     /// If credential is not found, we will not sign the request.
     async fn load_credential(&self) -> Result<Option<AwsCredential>> {
         let cred = { || self.loader.load() }
             .retry(&*BACKOFF)
             .await
             .map_err(new_request_credential_error)?;
 
@@ -143,15 +139,15 @@
     pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
         self.client.send(req).await
     }
 
     /// # Note
     ///
     /// header like X_AMZ_SERVER_SIDE_ENCRYPTION doesn't need to set while
-    /// get or stat.
+    //  get or stat.
     pub fn insert_sse_headers(
         &self,
         mut req: http::request::Builder,
         is_write: bool,
     ) -> http::request::Builder {
         if is_write {
             if let Some(v) = &self.server_side_encryption {
@@ -202,46 +198,52 @@
             )
         }
 
         req
     }
 }
 
-impl WasabiCore {
-    pub fn head_object_request(
+impl S3Core {
+    pub fn s3_head_object_request(
         &self,
         path: &str,
         if_none_match: Option<&str>,
+        if_match: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::head(&url);
 
         req = self.insert_sse_headers(req, false);
 
         if let Some(if_none_match) = if_none_match {
-            req = req.header(http::header::IF_NONE_MATCH, if_none_match);
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
+
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub fn get_object_request(
+    pub fn s3_get_object_request(
         &self,
         path: &str,
         range: BytesRange,
         override_content_disposition: Option<&str>,
         override_cache_control: Option<&str>,
         if_none_match: Option<&str>,
+        if_match: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         // Construct headers to add to the request
         let mut url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         // Add query arguments to the URL based on response overrides
@@ -267,42 +269,54 @@
         let mut req = Request::get(&url);
 
         if !range.is_full() {
             req = req.header(http::header::RANGE, range.to_header());
         }
 
         if let Some(if_none_match) = if_none_match {
-            req = req.header(http::header::IF_NONE_MATCH, if_none_match);
+            req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
         // Set SSE headers.
         // TODO: how will this work with presign?
         req = self.insert_sse_headers(req, false);
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn get_object(
+    pub async fn s3_get_object(
         &self,
         path: &str,
         range: BytesRange,
         if_none_match: Option<&str>,
+        if_match: Option<&str>,
+        override_content_disposition: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.get_object_request(path, range, None, None, if_none_match)?;
+        let mut req = self.s3_get_object_request(
+            path,
+            range,
+            override_content_disposition,
+            None,
+            if_none_match,
+            if_match,
+        )?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub fn put_object_request(
+    pub fn s3_put_object_request(
         &self,
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
         cache_control: Option<&str>,
         body: AsyncBody,
@@ -339,41 +353,46 @@
 
         // Set body
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn head_object(
+    pub async fn s3_head_object(
         &self,
         path: &str,
         if_none_match: Option<&str>,
+        if_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.head_object_request(path, if_none_match)?;
+        let mut req = self.s3_head_object_request(path, if_none_match, if_match)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn s3_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::delete(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn copy_object(&self, from: &str, to: &str) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn s3_copy_object(
+        &self,
+        from: &str,
+        to: &str,
+    ) -> Result<Response<IncomingAsyncBody>> {
         let from = build_abs_path(&self.root, from);
         let to = build_abs_path(&self.root, to);
 
         let source = format!("{}/{}", self.bucket, percent_encode_path(&from));
         let target = format!("{}/{}", self.endpoint, percent_encode_path(&to));
 
         let mut req = Request::put(&target);
@@ -425,28 +444,31 @@
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
     /// Make this functions as `pub(suber)` because `DirStream` depends
     /// on this.
-    pub async fn list_objects(
+    pub async fn s3_list_objects(
         &self,
         path: &str,
         continuation_token: &str,
         delimiter: &str,
         limit: Option<usize>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
-        let mut url = format!(
-            "{}?list-type=2&delimiter={delimiter}&prefix={}",
-            self.endpoint,
-            percent_encode_path(&p)
-        );
+        let mut url = format!("{}?list-type=2", self.endpoint);
+        if !p.is_empty() {
+            write!(url, "&prefix={}", percent_encode_path(&p))
+                .expect("write into string must succeed");
+        }
+        if !delimiter.is_empty() {
+            write!(url, "&delimiter={delimiter}").expect("write into string must succeed");
+        }
         if let Some(limit) = limit {
             write!(url, "&max-keys={limit}").expect("write into string must succeed");
         }
         if !continuation_token.is_empty() {
             // AWS S3 could return continuation-token that contains `=`
             // which could lead `reqsign` parse query wrongly.
             // URL encode continuation-token before starting signing so that
@@ -464,15 +486,15 @@
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn initiate_multipart_upload(
+    pub async fn s3_initiate_multipart_upload(
         &self,
         path: &str,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
         cache_control: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
@@ -506,15 +528,15 @@
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub fn upload_part_request(
+    pub fn s3_upload_part_request(
         &self,
         path: &str,
         upload_id: &str,
         part_number: usize,
         size: Option<u64>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
@@ -539,15 +561,15 @@
 
         // Set body
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn complete_multipart_upload(
+    pub async fn s3_complete_multipart_upload(
         &self,
         path: &str,
         upload_id: &str,
         parts: &[CompleteMultipartUploadRequestPart],
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
@@ -578,15 +600,15 @@
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
     /// Abort an on-going multipart upload.
-    pub async fn abort_multipart_upload(
+    pub async fn s3_abort_multipart_upload(
         &self,
         path: &str,
         upload_id: &str,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
@@ -599,15 +621,18 @@
         let mut req = Request::delete(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
-    pub async fn delete_objects(&self, paths: Vec<String>) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn s3_delete_objects(
+        &self,
+        paths: Vec<String>,
+    ) -> Result<Response<IncomingAsyncBody>> {
         let url = format!("{}/?delete", self.endpoint);
 
         let req = Request::post(&url);
 
         let content = quick_xml::se::to_string(&DeleteObjectsRequest {
             object: paths
                 .into_iter()
@@ -629,90 +654,14 @@
             .body(AsyncBody::Bytes(Bytes::from(content)))
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
-
-    pub async fn put_object(
-        &self,
-        path: &str,
-        size: Option<usize>,
-        content_type: Option<&str>,
-        content_disposition: Option<&str>,
-        cache_control: Option<&str>,
-        body: AsyncBody,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.put_object_request(
-            path,
-            size,
-            content_type,
-            content_disposition,
-            cache_control,
-            body,
-        )?;
-
-        self.sign(&mut req).await?;
-
-        self.send(req).await
-    }
-
-    pub async fn rename_object(&self, from: &str, to: &str) -> Result<Response<IncomingAsyncBody>> {
-        let from = percent_encode_path(build_abs_path(&self.root, from).as_str());
-        let to = percent_encode_path(build_abs_path(&self.root, to).as_str());
-
-        let url = format!("{}/{}", self.endpoint, from);
-
-        let mut req = Request::builder().method("MOVE").uri(url);
-
-        // Set SSE headers.
-        req = self.insert_sse_headers(req, true);
-
-        let mut req = req
-            .header(constants::DESTINATION, to)
-            .header(constants::OVERWRITE, "true")
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.sign(&mut req).await?;
-
-        self.send(req).await
-    }
-
-    pub async fn append_object(
-        &self,
-        path: &str,
-        size: Option<usize>,
-        body: AsyncBody,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!("{}/{}?append", self.endpoint, percent_encode_path(&p));
-
-        let mut req = Request::put(&url);
-
-        if let Some(size) = size {
-            req = req.header(CONTENT_LENGTH, size)
-        }
-
-        // Set storage class header
-        if let Some(v) = &self.default_storage_class {
-            req = req.header(HeaderName::from_static(constants::X_AMZ_STORAGE_CLASS), v);
-        }
-
-        // Set SSE headers.
-        req = self.insert_sse_headers(req, true);
-
-        let mut req = req.body(body).map_err(new_request_build_error)?;
-
-        self.sign(&mut req).await?;
-
-        self.send(req).await
-    }
 }
 
 /// Result of CreateMultipartUpload
 #[derive(Default, Debug, Deserialize)]
 #[serde(default, rename_all = "PascalCase")]
 pub struct InitiateMultipartUploadResult {
     pub upload_id: String,
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/writer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/writer.rs`

 * *Files 19% similar despite different names*

```diff
@@ -11,88 +11,54 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::sync::Arc;
-
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::core::*;
+use super::backend::WebdavBackend;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct WasabiWriter {
-    core: Arc<WasabiCore>,
+pub struct WebdavWriter {
+    backend: WebdavBackend,
 
     op: OpWrite,
     path: String,
-
-    upload_id: Option<String>,
 }
 
-impl WasabiWriter {
-    pub fn new(
-        core: Arc<WasabiCore>,
-        op: OpWrite,
-        path: String,
-        upload_id: Option<String>,
-    ) -> Self {
-        WasabiWriter {
-            core,
-
-            op,
-            path,
-            upload_id,
-        }
+impl WebdavWriter {
+    pub fn new(backend: WebdavBackend, op: OpWrite, path: String) -> Self {
+        WebdavWriter { backend, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for WasabiWriter {
+impl oio::Write for WebdavWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        debug_assert!(
-            self.upload_id.is_none(),
-            "Writer initiated with upload id, but users trying to call write, must be buggy"
-        );
-
         let resp = self
-            .core
-            .put_object(
+            .backend
+            .webdav_put(
                 &self.path,
                 Some(bs.len()),
                 self.op.content_type(),
                 self.op.content_disposition(),
-                self.op.cache_control(),
                 AsyncBody::Bytes(bs),
             )
             .await?;
 
-        match resp.status() {
-            StatusCode::CREATED | StatusCode::OK => {
-                resp.into_body().consume().await?;
-                Ok(())
-            }
-            _ => Err(parse_error(resp).await?),
-        }
-    }
-
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let resp = self
-            .core
-            .append_object(&self.path, Some(bs.len()), AsyncBody::Bytes(bs))
-            .await?;
+        let status = resp.status();
 
-        match resp.status() {
+        match status {
             StatusCode::CREATED | StatusCode::OK | StatusCode::NO_CONTENT => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -262,22 +262,23 @@
     type Pager = WebdavPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
         ma.set_scheme(Scheme::Webdav)
             .set_root(&self.root)
-            .set_capabilities(
-                AccessorCapability::Read
-                    | AccessorCapability::Write
-                    | AccessorCapability::Copy
-                    | AccessorCapability::Rename
-                    | AccessorCapability::List,
-            )
-            .set_hints(AccessorHint::ReadStreamable);
+            .set_capability(Capability {
+                read: true,
+                read_can_next: true,
+                write: true,
+                list: true,
+                copy: true,
+                rename: true,
+                ..Default::default()
+            });
 
         ma
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         self.ensure_parent_path(path).await?;
 
@@ -296,18 +297,18 @@
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.append() {
+        if args.content_length().is_none() {
             return Err(Error::new(
                 ErrorKind::Unsupported,
-                "append write is not supported",
+                "write without content length is not supported",
             ));
         }
 
         let p = build_abs_path(&self.root, path);
 
         Ok((RpWrite::default(), WebdavWriter::new(self.clone(), args, p)))
     }
@@ -643,14 +644,18 @@
                 Ok(RpCreate::default())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn ensure_parent_path(&self, path: &str) -> Result<()> {
+        if path == "/" {
+            return Ok(());
+        }
+
         // create dir recursively, split path by `/` and create each dir except the last one
         let abs_path = build_abs_path(&self.root, path);
         let abs_path = abs_path.as_str();
         let mut parts: Vec<&str> = abs_path.split('/').filter(|x| !x.is_empty()).collect();
         if !parts.is_empty() {
             parts.pop();
         }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf` & `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf` & `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/list_response.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/list_response.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/pager.rs`

 * *Files 6% similar despite different names*

```diff
@@ -50,20 +50,21 @@
         };
         let oes = mem::take(&mut self.multistates.response);
 
         let oes = oes
             .into_iter()
             .filter_map(|de| {
                 let path = de.href;
-                let normalized_path = if self.root != path {
-                    build_rel_path(&self.root, &path)
-                } else {
-                    path
-                };
 
+                // Ignore the root path itself.
+                if self.root == path {
+                    return None;
+                }
+
+                let normalized_path = build_rel_path(&self.root, &path);
                 if normalized_path == self.path {
                     // WebDav server may return the current path as an entry.
                     return None;
                 }
 
                 let entry = if de.propstat.prop.resourcetype.value
                     == Some(super::list_response::ResourceType::Collection)
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/backend.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -461,18 +461,21 @@
     type Pager = WebhdfsPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Webhdfs)
             .set_root(&self.root)
-            .set_capabilities(
-                AccessorCapability::Read | AccessorCapability::Write | AccessorCapability::List,
-            )
-            .set_hints(AccessorHint::ReadStreamable);
+            .set_capability(Capability {
+                read: true,
+                read_can_next: true,
+                write: true,
+                list: true,
+                ..Default::default()
+            });
         am
     }
 
     /// Create a file or directory
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let req = self
             .webhdfs_create_object_request(path, Some(0), None, AsyncBody::Empty)
@@ -515,18 +518,18 @@
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.append() {
+        if args.content_length().is_none() {
             return Err(Error::new(
                 ErrorKind::Unsupported,
-                "append write is not supported",
+                "write without content length is not supported",
             ));
         }
 
         Ok((
             RpWrite::default(),
             WebhdfsWriter::new(self.clone(), args, path.to_string()),
         ))
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/message.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/message.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/pager.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/writer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/writer.rs`

 * *Files 8% similar despite different names*

```diff
@@ -59,23 +59,14 @@
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
-    async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let _ = bs;
-
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "output writer doesn't support append",
-        ))
-    }
-
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/builder.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/entry.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/error.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/error.rs`

 * *Files 8% similar despite different names*

```diff
@@ -71,14 +71,32 @@
     /// The given file paths are same.
     IsSameFile,
     /// The preconfition of this operation is not met.
     ///
     /// For example, reading a file with If-Match header but the file's ETag
     /// is not match.
     PreconditionFailed,
+    /// The content is truncated.
+    ///
+    /// This error kind means there are more content to come but been truncated.
+    ///
+    /// For examples:
+    ///
+    /// - Users expected to read 1024 bytes, but service returned more bytes.
+    /// - Service expected to write 1024 bytes, but users write more bytes.
+    ContentTruncated,
+    /// The content is incomplete.
+    ///
+    /// This error kind means expect content length is not reached.
+    ///
+    /// For examples:
+    ///
+    /// - Users expected to read 1024 bytes, but service returned less bytes.
+    /// - Service expected to write 1024 bytes, but users write less bytes.
+    ContentIncomplete,
 }
 
 impl ErrorKind {
     /// Convert self into static str.
     pub fn into_static(self) -> &'static str {
         self.into()
     }
@@ -100,14 +118,16 @@
             ErrorKind::PermissionDenied => "PermissionDenied",
             ErrorKind::IsADirectory => "IsADirectory",
             ErrorKind::NotADirectory => "NotADirectory",
             ErrorKind::AlreadyExists => "AlreadyExists",
             ErrorKind::RateLimited => "RateLimited",
             ErrorKind::IsSameFile => "IsSameFile",
             ErrorKind::PreconditionFailed => "PreconditionFailed",
+            ErrorKind::ContentTruncated => "ContentTruncated",
+            ErrorKind::ContentIncomplete => "ContentIncomplete",
         }
     }
 }
 
 #[derive(Clone, Copy, Debug, PartialEq, Eq)]
 enum ErrorStatus {
     /// Permanent means without external changes, the error never changes.
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/list.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/list.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/metadata.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/mod.rs`

 * *Files 21% similar despite different names*

```diff
@@ -50,8 +50,11 @@
 pub use error::Error;
 pub use error::ErrorKind;
 pub use error::Result;
 
 mod scheme;
 pub use scheme::Scheme;
 
+mod capability;
+pub use capability::Capability;
+
 pub mod ops;
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/mode.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/mode.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,19 @@
     }
 
     /// create a new blocking operator from inner accessor.
     ///
     /// # Note
     /// default batch limit is 1000.
     pub(crate) fn from_inner(accessor: FusedAccessor) -> Self {
-        let limit = accessor.info().max_batch_operations().unwrap_or(1000);
+        let limit = accessor
+            .info()
+            .capability()
+            .batch_max_operations
+            .unwrap_or(1000);
         Self { accessor, limit }
     }
 
     /// Get current operator's limit
     pub fn limit(&self) -> usize {
         self.limit
     }
@@ -415,15 +419,15 @@
                     .with_context("service", self.info().scheme().into_static())
                     .with_context("path", &path),
             );
         }
 
         let op = OpRead::new().with_range(range.into());
 
-        BlockingReader::create_dir(self.inner().clone(), &path, op)
+        BlockingReader::create(self.inner().clone(), &path, op)
     }
 
     /// Write bytes into given path.
     ///
     /// # Notes
     ///
     /// - Write will make sure all bytes has been written, or an error will be returned.
@@ -439,15 +443,20 @@
     ///
     /// # fn test(op: BlockingOperator) -> Result<()> {
     /// op.write("path/to/file", vec![0; 4096])?;
     /// # Ok(())
     /// # }
     /// ```
     pub fn write(&self, path: &str, bs: impl Into<Bytes>) -> Result<()> {
-        self.write_with(path, OpWrite::new(), bs)
+        let bs = bs.into();
+        self.write_with(
+            path,
+            OpWrite::new().with_content_length(bs.len() as u64),
+            bs,
+        )
     }
 
     /// Copy a file from `from` to `to`.
     ///
     /// # Notes
     ///
     /// - `from` and `to` must be a file.
@@ -590,16 +599,19 @@
                 Error::new(ErrorKind::IsADirectory, "write path is a directory")
                     .with_operation("BlockingOperator::write_with")
                     .with_context("service", self.info().scheme().into_static())
                     .with_context("path", &path),
             );
         }
 
-        let (_, mut w) = self.inner().blocking_write(&path, args)?;
-        w.write(bs.into())?;
+        let bs = bs.into();
+        let (_, mut w) = self
+            .inner()
+            .blocking_write(&path, args.with_content_length(bs.len() as u64))?;
+        w.write(bs)?;
         w.close()?;
 
         Ok(())
     }
 
     /// Write multiple bytes into given path.
     ///
@@ -614,16 +626,16 @@
     /// # use opendal::BlockingOperator;
     /// # use futures::StreamExt;
     /// # use futures::SinkExt;
     /// use bytes::Bytes;
     ///
     /// # fn test(op: BlockingOperator) -> Result<()> {
     /// let mut w = op.writer("path/to/file")?;
-    /// w.append(vec![0; 4096])?;
-    /// w.append(vec![1; 4096])?;
+    /// w.write(vec![0; 4096])?;
+    /// w.write(vec![1; 4096])?;
     /// w.close()?;
     /// # Ok(())
     /// # }
     /// ```
     pub fn writer(&self, path: &str) -> Result<BlockingWriter> {
         let path = normalize_path(path);
 
@@ -632,16 +644,16 @@
                 Error::new(ErrorKind::IsADirectory, "write path is a directory")
                     .with_operation("BlockingOperator::writer")
                     .with_context("service", self.info().scheme().into_static())
                     .with_context("path", &path),
             );
         }
 
-        let op = OpWrite::default().with_append();
-        BlockingWriter::create_dir(self.inner().clone(), &path, op)
+        let op = OpWrite::default();
+        BlockingWriter::create(self.inner().clone(), &path, op)
     }
 
     /// Delete given path.
     ///
     /// # Notes
     ///
     /// - Delete not existing error won't return errors.
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/operator/builder.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/operator/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/operator/metadata.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/operator/metadata.rs`

 * *Files 14% similar despite different names*

```diff
@@ -43,52 +43,57 @@
     ///
     /// - name for `s3` => bucket name
     /// - name for `azblob` => container name
     pub fn name(&self) -> &str {
         self.0.name()
     }
 
+    /// Get [`Capability`] of operator.
+    pub fn capability(&self) -> Capability {
+        self.0.capability()
+    }
+
     /// Check if current backend supports [`Accessor::read`] or not.
     pub fn can_read(&self) -> bool {
-        self.0.capabilities().contains(AccessorCapability::Read)
+        self.0.capability().read
     }
 
     /// Check if current backend supports [`Accessor::write`] or not.
     pub fn can_write(&self) -> bool {
-        self.0.capabilities().contains(AccessorCapability::Write)
+        self.0.capability().write
     }
 
     /// Check if current backend supports [`Accessor::copy`] or not.
     pub fn can_copy(&self) -> bool {
-        self.0.capabilities().contains(AccessorCapability::Copy)
+        self.0.capability().copy
     }
 
     /// Check if current backend supports [`Accessor::rename`] or not.
     pub fn can_rename(&self) -> bool {
-        self.0.capabilities().contains(AccessorCapability::Rename)
+        self.0.capability().rename
     }
 
     /// Check if current backend supports [`Accessor::list`] or not.
     pub fn can_list(&self) -> bool {
-        self.0.capabilities().contains(AccessorCapability::List)
+        self.0.capability().list
     }
 
     /// Check if current backend supports [`Accessor::scan`] or not.
     pub fn can_scan(&self) -> bool {
-        self.0.capabilities().contains(AccessorCapability::Scan)
+        self.0.capability().scan
     }
 
     /// Check if current backend supports [`Accessor::presign`] or not.
     pub fn can_presign(&self) -> bool {
-        self.0.capabilities().contains(AccessorCapability::Presign)
+        self.0.capability().presign
     }
 
     /// Check if current backend supports batch operations or not.
     pub fn can_batch(&self) -> bool {
-        self.0.capabilities().contains(AccessorCapability::Batch)
+        self.0.capability().batch
     }
 
     /// Check if current backend supports blocking operations or not.
     pub fn can_blocking(&self) -> bool {
-        self.0.capabilities().contains(AccessorCapability::Blocking)
+        self.0.capability().blocking
     }
 }
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/operator/mod.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/operator/operator.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/operator/operator.rs`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,19 @@
 /// # Operator basic API.
 impl Operator {
     pub(super) fn inner(&self) -> &FusedAccessor {
         &self.accessor
     }
 
     pub(crate) fn from_inner(accessor: FusedAccessor) -> Self {
-        let limit = accessor.info().max_batch_operations().unwrap_or(1000);
+        let limit = accessor
+            .info()
+            .capability()
+            .batch_max_operations
+            .unwrap_or(1000);
         Self { accessor, limit }
     }
 
     pub(super) fn into_inner(self) -> FusedAccessor {
         self.accessor
     }
 
@@ -627,15 +631,21 @@
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
     /// op.write("path/to/file", vec![0; 4096]).await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn write(&self, path: &str, bs: impl Into<Bytes>) -> Result<()> {
-        self.write_with(path, OpWrite::new(), bs).await
+        let bs = bs.into();
+        self.write_with(
+            path,
+            OpWrite::new().with_content_length(bs.len() as u64),
+            bs,
+        )
+        .await
     }
 
     /// Copy a file from `from` to `to`.
     ///
     /// # Notes
     ///
     /// - `from` and `to` must be a file.
@@ -749,45 +759,41 @@
         self.inner().rename(&from, &to, OpRename::new()).await?;
 
         Ok(())
     }
 
     /// Write multiple bytes into path.
     ///
-    /// # Notes
-    ///
-    /// - Write will make sure all bytes has been written, or an error will be returned.
+    /// Refer to [`Writer`] for more details.
     ///
     /// # Examples
     ///
     /// ```
     /// # use std::io::Result;
     /// # use opendal::Operator;
     /// # use futures::StreamExt;
     /// # use futures::SinkExt;
     /// use bytes::Bytes;
     ///
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
     /// let mut w = op.writer("path/to/file").await?;
-    /// w.append(vec![0; 4096]).await?;
-    /// w.append(vec![1; 4096]).await?;
+    /// w.write(vec![0; 4096]).await?;
+    /// w.write(vec![1; 4096]).await?;
     /// w.close().await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn writer(&self, path: &str) -> Result<Writer> {
         self.writer_with(path, OpWrite::default()).await
     }
 
     /// Write multiple bytes into path with extra options.
     ///
-    /// # Notes
-    ///
-    /// - Write will make sure all bytes has been written, or an error will be returned.
+    /// Refer to [`Writer`] for more details.
     ///
     /// # Examples
     ///
     /// ```
     /// # use std::io::Result;
     /// # use opendal::Operator;
     /// # use futures::StreamExt;
@@ -795,16 +801,16 @@
     /// use bytes::Bytes;
     /// use opendal::ops::OpWrite;
     ///
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
     /// let args = OpWrite::new().with_content_type("application/octet-stream");
     /// let mut w = op.writer_with("path/to/file", args).await?;
-    /// w.append(vec![0; 4096]).await?;
-    /// w.append(vec![1; 4096]).await?;
+    /// w.write(vec![0; 4096]).await?;
+    /// w.write(vec![1; 4096]).await?;
     /// w.close().await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn writer_with(&self, path: &str, args: OpWrite) -> Result<Writer> {
         let path = normalize_path(path);
 
@@ -813,15 +819,15 @@
                 Error::new(ErrorKind::IsADirectory, "write path is a directory")
                     .with_operation("Operator::writer")
                     .with_context("service", self.inner().info().scheme().into_static())
                     .with_context("path", &path),
             );
         }
 
-        Writer::create_dir(self.inner().clone(), &path, args.with_append()).await
+        Writer::create(self.inner().clone(), &path, args).await
     }
 
     /// Write data with extra options.
     ///
     /// # Notes
     ///
     /// - Write will make sure all bytes has been written, or an error will be returned.
@@ -850,16 +856,20 @@
                 Error::new(ErrorKind::IsADirectory, "write path is a directory")
                     .with_operation("Operator::write_with")
                     .with_context("service", self.info().scheme().into_static())
                     .with_context("path", &path),
             );
         }
 
-        let (_, mut w) = self.inner().write(&path, args).await?;
-        w.write(bs.into()).await?;
+        let bs = bs.into();
+        let (_, mut w) = self
+            .inner()
+            .write(&path, args.with_content_length(bs.len() as u64))
+            .await?;
+        w.write(bs).await?;
         w.close().await?;
 
         Ok(())
     }
 
     /// Delete the given path.
     ///
@@ -1068,27 +1078,66 @@
     ///         EntryMode::Unknown => continue,
     ///     }
     /// }
     /// # Ok(())
     /// # }
     /// ```
     pub async fn list(&self, path: &str) -> Result<Lister> {
+        self.list_with(path, OpList::new()).await
+    }
+
+    /// List given path with OpList.
+    ///
+    /// This function will create a new handle to list entries.
+    ///
+    /// An error will be returned if given path doesn't end with `/`.
+    ///
+    /// # Examples
+    ///
+    /// ```no_run
+    /// # use anyhow::Result;
+    /// # use futures::io;
+    /// use futures::TryStreamExt;
+    /// use opendal::EntryMode;
+    /// use opendal::Metakey;
+    /// use opendal::Operator;
+    /// use opendal::ops::OpList;
+    /// # #[tokio::main]
+    /// # async fn test(op: Operator) -> Result<()> {
+    /// let option = OpList::new().with_limit(10).with_start_after("start");
+    /// let mut ds = op.list_with("path/to/dir/", option).await?;
+    /// while let Some(mut de) = ds.try_next().await? {
+    ///     let meta = op.metadata(&de, Metakey::Mode).await?;
+    ///     match meta.mode() {
+    ///         EntryMode::FILE => {
+    ///             println!("Handling file")
+    ///         }
+    ///         EntryMode::DIR => {
+    ///             println!("Handling dir like start a new list via meta.path()")
+    ///         }
+    ///         EntryMode::Unknown => continue,
+    ///     }
+    /// }
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub async fn list_with(&self, path: &str, op: OpList) -> Result<Lister> {
         let path = normalize_path(path);
 
         if !validate_path(&path, EntryMode::DIR) {
             return Err(Error::new(
                 ErrorKind::NotADirectory,
                 "the path trying to list should end with `/`",
             )
             .with_operation("Operator::list")
             .with_context("service", self.info().scheme().into_static())
             .with_context("path", &path));
         }
 
-        let (_, pager) = self.inner().list(&path, OpList::new()).await?;
+        let (_, pager) = self.inner().list(&path, op).await?;
 
         Ok(Lister::new(pager))
     }
 
     /// List dir in flat way.
     ///
     /// Also, this function can be used to list a prefix.
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/ops.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/ops.rs`

 * *Files 9% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 
 /// Args for `list` operation.
 #[derive(Debug, Clone, Default)]
 pub struct OpList {
     /// The limit passed to underlying service to specify the max results
     /// that could return.
     limit: Option<usize>,
+
+    /// The start_after passes to underlying service to specify the specified key
+    /// to start listing from.
+    start_after: Option<String>,
 }
 
 impl OpList {
     /// Create a new `OpList`.
     pub fn new() -> Self {
         Self::default()
     }
@@ -69,14 +73,25 @@
         self
     }
 
     /// Get the limit of list operation.
     pub fn limit(&self) -> Option<usize> {
         self.limit
     }
+
+    /// Change the start_after of this list operation.
+    pub fn with_start_after(mut self, start_after: &str) -> Self {
+        self.start_after = Some(start_after.into());
+        self
+    }
+
+    /// Get the start_after of list operation.
+    pub fn start_after(&self) -> Option<&str> {
+        self.start_after.as_deref()
+    }
 }
 
 /// Args for `scan` operation.
 #[derive(Debug, Default, Clone)]
 pub struct OpScan {
     /// The limit passed to underlying service to specify the max results
     /// that could return.
@@ -208,18 +223,18 @@
     }
 }
 
 /// Args for `read` operation.
 #[derive(Debug, Clone, Default)]
 pub struct OpRead {
     br: BytesRange,
-    override_content_disposition: Option<String>,
-    override_cache_control: Option<String>,
     if_match: Option<String>,
     if_none_match: Option<String>,
+    override_cache_control: Option<String>,
+    override_content_disposition: Option<String>,
 }
 
 impl OpRead {
     /// Create a default `OpRead` which will read whole content of path.
     pub fn new() -> Self {
         Self::default()
     }
@@ -316,37 +331,42 @@
         self.if_none_match.as_deref()
     }
 }
 
 /// Args for `write` operation.
 #[derive(Debug, Clone, Default)]
 pub struct OpWrite {
-    append: bool,
-
+    content_length: Option<u64>,
     content_type: Option<String>,
     content_disposition: Option<String>,
     cache_control: Option<String>,
-    if_match: Option<String>,
 }
 
 impl OpWrite {
     /// Create a new `OpWrite`.
     ///
     /// If input path is not a file path, an error will be returned.
     pub fn new() -> Self {
         Self::default()
     }
 
-    pub(crate) fn with_append(mut self) -> Self {
-        self.append = true;
-        self
+    /// Get the content length from op.
+    ///
+    /// The content length is the total length of the data to be written.
+    pub fn content_length(&self) -> Option<u64> {
+        self.content_length
     }
 
-    pub(crate) fn append(&self) -> bool {
-        self.append
+    /// Set the content length of op.
+    ///
+    /// If the content length is not set, the content length will be
+    /// calculated automatically by buffering part of data.
+    pub fn with_content_length(mut self, content_length: u64) -> Self {
+        self.content_length = Some(content_length);
+        self
     }
 
     /// Get the content type from option
     pub fn content_type(&self) -> Option<&str> {
         self.content_type.as_deref()
     }
 
@@ -373,25 +393,14 @@
     }
 
     /// Set the content type of option
     pub fn with_cache_control(mut self, cache_control: &str) -> Self {
         self.cache_control = Some(cache_control.to_string());
         self
     }
-
-    /// Set the If-Match of the option
-    pub fn with_if_match(mut self, if_match: &str) -> Self {
-        self.if_match = Some(if_match.to_string());
-        self
-    }
-
-    /// Get If-Match from option
-    pub fn if_match(&self) -> Option<&str> {
-        self.if_match.as_deref()
-    }
 }
 
 /// Args for `copy` operation.
 #[derive(Debug, Clone, Default)]
 pub struct OpCopy {}
 
 impl OpCopy {
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/reader.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/reader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -188,28 +188,28 @@
     /// Create a new blocking reader.
     ///
     /// Create will use internal information to decide the most suitable
     /// implementation for users.
     ///
     /// We don't want to expose those details to users so keep this function
     /// in crate only.
-    pub(crate) fn create_dir(acc: FusedAccessor, path: &str, op: OpRead) -> Result<Self> {
+    pub(crate) fn create(acc: FusedAccessor, path: &str, op: OpRead) -> Result<Self> {
         let acc_meta = acc.info();
 
-        let r = if acc_meta.hints().contains(AccessorHint::ReadSeekable) {
+        let r = if acc_meta.capability().read_can_seek {
             let (_, r) = acc.blocking_read(path, op)?;
             r
         } else {
             return Err(Error::new(
                 ErrorKind::Unsupported,
                 "non seekable blocking reader is not supported",
             ));
         };
 
-        let r = if acc_meta.hints().contains(AccessorHint::ReadStreamable) {
+        let r = if acc_meta.capability().read_can_next {
             r
         } else {
             // Make this capacity configurable.
             Box::new(oio::into_streamable_reader(r, 256 * 1024))
         };
 
         Ok(BlockingReader { inner: r })
```

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/scheme.rs` & `opendal-0.33.0/local_dependencies/opendal/src/types/scheme.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/local_dependencies/opendal/src/types/writer.rs` & `opendal-0.33.0/local_dependencies/opendal/src/services/oss/writer.rs`

 * *Files 22% similar despite different names*

```diff
@@ -11,223 +11,216 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::fmt::Display;
-use std::io;
-use std::pin::Pin;
-use std::task::Context;
-use std::task::Poll;
+use std::sync::Arc;
 
+use async_trait::async_trait;
+use bytes::Buf;
 use bytes::Bytes;
-use futures::future::BoxFuture;
-use futures::ready;
-use futures::AsyncWrite;
-use futures::FutureExt;
+use http::StatusCode;
 
+use super::core::*;
+use super::error::parse_error;
 use crate::ops::OpWrite;
-use crate::raw::oio::Write;
 use crate::raw::*;
 use crate::*;
 
-/// Writer is designed to write data into given path in an asynchronous
-/// manner.
-///
-/// # Notes
-///
-/// Writer is designed for appending multiple blocks which could
-/// lead to much requests. If only want to send all data in single chunk,
-/// please use [`Operator::write`] instead.
-pub struct Writer {
-    state: State,
-}
+pub struct OssWriter {
+    core: Arc<OssCore>,
 
-impl Writer {
-    /// Create a new writer.
-    ///
-    /// Create will use internal information to decide the most suitable
-    /// implementation for users.
-    ///
-    /// We don't want to expose those details to users so keep this function
-    /// in crate only.
-    pub(crate) async fn create_dir(acc: FusedAccessor, path: &str, op: OpWrite) -> Result<Self> {
-        let (_, w) = acc.write(path, op).await?;
-
-        Ok(Writer {
-            state: State::Idle(Some(w)),
-        })
-    }
-
-    /// Append data into writer.
-    ///
-    /// It is highly recommended to align the length of the input bytes
-    /// into blocks of 4MiB (except the last block) for better performance
-    /// and compatibility.
-    pub async fn append(&mut self, bs: impl Into<Bytes>) -> Result<()> {
-        if let State::Idle(Some(w)) = &mut self.state {
-            w.append(bs.into()).await
-        } else {
-            unreachable!(
-                "writer state invalid while append, expect Idle, actual {}",
-                self.state
-            );
+    op: OpWrite,
+    path: String,
+    upload_id: Option<String>,
+
+    parts: Vec<MultipartUploadPart>,
+    buffer: oio::VectorCursor,
+    buffer_size: usize,
+}
+
+impl OssWriter {
+    pub fn new(core: Arc<OssCore>, path: &str, op: OpWrite) -> Self {
+        OssWriter {
+            core,
+            path: path.to_string(),
+            op,
+
+            upload_id: None,
+            parts: vec![],
+            buffer: oio::VectorCursor::new(),
+            // The part size must be 5 MiB to 5 GiB. There is no minimum
+            // size limit on the last part of your multipart upload.
+            //
+            // We pick the default value as 8 MiB for better thoughput.
+            //
+            // TODO: allow this value to be configured.
+            buffer_size: 8 * 1024 * 1024,
         }
     }
 
-    /// Abort inner writer.
-    pub async fn abort(&mut self) -> Result<()> {
-        if let State::Idle(Some(w)) = &mut self.state {
-            w.abort().await
-        } else {
-            unreachable!(
-                "writer state invalid while abort, expect Idle, actual {}",
-                self.state
-            );
+    async fn write_oneshot(&self, bs: Bytes) -> Result<()> {
+        let mut req = self.core.oss_put_object_request(
+            &self.path,
+            Some(bs.len()),
+            self.op.content_type(),
+            self.op.content_disposition(),
+            self.op.cache_control(),
+            AsyncBody::Bytes(bs),
+            false,
+        )?;
+
+        self.core.sign(&mut req).await?;
+
+        let resp = self.core.send(req).await?;
+
+        let status = resp.status();
+
+        match status {
+            StatusCode::CREATED | StatusCode::OK => {
+                resp.into_body().consume().await?;
+                Ok(())
+            }
+            _ => Err(parse_error(resp).await?),
         }
     }
 
-    /// Close the writer and make sure all data have been stored.
-    pub async fn close(&mut self) -> Result<()> {
-        if let State::Idle(Some(w)) = &mut self.state {
-            w.close().await
-        } else {
-            unreachable!(
-                "writer state invalid while close, expect Idle, actual {}",
-                self.state
-            );
+    async fn initiate_upload(&self) -> Result<String> {
+        let resp = self.core.oss_initiate_upload(&self.path, &self.op).await?;
+        match resp.status() {
+            StatusCode::OK => {
+                let bs = resp.into_body().bytes().await?;
+                let result: InitiateMultipartUploadResult =
+                    quick_xml::de::from_reader(bs.reader()).map_err(new_xml_deserialize_error)?;
+                Ok(result.upload_id)
+            }
+            _ => Err(parse_error(resp).await?),
         }
     }
-}
-
-enum State {
-    Idle(Option<oio::Writer>),
-    Write(BoxFuture<'static, Result<(usize, oio::Writer)>>),
-    Close(BoxFuture<'static, Result<oio::Writer>>),
-}
 
-impl Display for State {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        match self {
-            State::Idle(_) => write!(f, "Idle"),
-            State::Write(_) => write!(f, "Write"),
-            State::Close(_) => write!(f, "Close"),
+    async fn write_part(&self, upload_id: &str, bs: Bytes) -> Result<MultipartUploadPart> {
+        // Aliyun OSS requires part number must between [1..=10000]
+        let part_number = self.parts.len() + 1;
+        let mut req = self
+            .core
+            .oss_upload_part_request(
+                &self.path,
+                upload_id,
+                part_number,
+                false,
+                Some(bs.len() as u64),
+                AsyncBody::Bytes(bs),
+            )
+            .await?;
+
+        self.core.sign(&mut req).await?;
+
+        let resp = self.core.send(req).await?;
+        match resp.status() {
+            StatusCode::OK => {
+                let etag = parse_etag(resp.headers())?
+                    .ok_or_else(|| {
+                        Error::new(
+                            ErrorKind::Unexpected,
+                            "ETag not present in returning response",
+                        )
+                    })?
+                    .to_string();
+                resp.into_body().consume().await?;
+                Ok(MultipartUploadPart { part_number, etag })
+            }
+            _ => Err(parse_error(resp).await?),
         }
     }
 }
 
-impl AsyncWrite for Writer {
-    fn poll_write(
-        mut self: Pin<&mut Self>,
-        cx: &mut Context<'_>,
-        buf: &[u8],
-    ) -> Poll<io::Result<usize>> {
-        loop {
-            match &mut self.state {
-                State::Idle(w) => {
-                    let mut w = w
-                        .take()
-                        .expect("invalid state of writer: Idle state with empty write");
-                    let bs = Bytes::from(buf.to_vec());
-                    let size = bs.len();
-                    let fut = async move {
-                        w.append(bs).await?;
-                        Ok((size, w))
-                    };
-                    self.state = State::Write(Box::pin(fut));
-                }
-                State::Write(fut) => match ready!(fut.poll_unpin(cx)) {
-                    Ok((size, w)) => {
-                        self.state = State::Idle(Some(w));
-                        return Poll::Ready(Ok(size));
-                    }
-                    Err(err) => return Poll::Ready(Err(io::Error::new(io::ErrorKind::Other, err))),
-                },
-                State::Close(_) => {
-                    unreachable!("invalid state of writer: poll_write with State::Close")
+#[async_trait]
+impl oio::Write for OssWriter {
+    async fn write(&mut self, bs: Bytes) -> Result<()> {
+        let upload_id = match &self.upload_id {
+            Some(upload_id) => upload_id,
+            None => {
+                if self.op.content_length().unwrap_or_default() == bs.len() as u64 {
+                    return self.write_oneshot(bs).await;
+                } else {
+                    let upload_id = self.initiate_upload().await?;
+                    self.upload_id = Some(upload_id);
+                    self.upload_id.as_deref().unwrap()
                 }
-            };
+            }
+        };
+
+        // Ignore empty bytes
+        if bs.is_empty() {
+            return Ok(());
         }
-    }
 
-    /// Writer makes sure that every write is flushed.
-    fn poll_flush(self: Pin<&mut Self>, _: &mut Context<'_>) -> Poll<io::Result<()>> {
-        Poll::Ready(Ok(()))
-    }
-
-    fn poll_close(mut self: Pin<&mut Self>, cx: &mut Context<'_>) -> Poll<io::Result<()>> {
-        loop {
-            match &mut self.state {
-                State::Idle(w) => {
-                    let mut w = w
-                        .take()
-                        .expect("invalid state of writer: Idle state with empty write");
-                    let fut = async move {
-                        w.close().await?;
-                        Ok(w)
-                    };
-                    self.state = State::Close(Box::pin(fut));
-                }
-                State::Write(_) => {
-                    unreachable!("invalid state of writer: poll_close with State::Write")
-                }
-                State::Close(fut) => match ready!(fut.poll_unpin(cx)) {
-                    Ok(w) => {
-                        self.state = State::Idle(Some(w));
-                        return Poll::Ready(Ok(()));
-                    }
-                    Err(err) => return Poll::Ready(Err(io::Error::new(io::ErrorKind::Other, err))),
-                },
-            }
+        self.buffer.push(bs);
+        // Return directly if the buffer is not full
+        if self.buffer.len() <= self.buffer_size {
+            return Ok(());
         }
-    }
-}
 
-/// BlockingWriter is designed to write data into given path in an blocking
-/// manner.
-pub struct BlockingWriter {
-    pub(crate) inner: oio::BlockingWriter,
-}
+        let bs = self.buffer.peak_at_least(self.buffer_size);
+        let size = bs.len();
 
-impl BlockingWriter {
-    /// Create a new writer.
-    ///
-    /// Create will use internal information to decide the most suitable
-    /// implementation for users.
-    ///
-    /// We don't want to expose those details to users so keep this function
-    /// in crate only.
-    pub(crate) fn create_dir(acc: FusedAccessor, path: &str, op: OpWrite) -> Result<Self> {
-        let (_, w) = acc.blocking_write(path, op)?;
-
-        Ok(BlockingWriter { inner: w })
-    }
-
-    /// Append data into writer.
-    ///
-    /// It is highly recommended to align the length of the input bytes
-    /// into blocks of 4MiB (except the last block) for better performance
-    /// and compatibility.
-    pub fn append(&mut self, bs: impl Into<Bytes>) -> Result<()> {
-        self.inner.append(bs.into())
-    }
-
-    /// Close the writer and make sure all data have been stored.
-    pub fn close(&mut self) -> Result<()> {
-        self.inner.close()
+        match self.write_part(upload_id, bs).await {
+            Ok(part) => {
+                self.buffer.take(size);
+                self.parts.push(part);
+                Ok(())
+            }
+            Err(e) => {
+                // If the upload fails, we should pop the given bs to make sure
+                // write is re-enter safe.
+                self.buffer.pop();
+                Err(e)
+            }
+        }
     }
-}
 
-impl io::Write for BlockingWriter {
-    fn write(&mut self, buf: &[u8]) -> io::Result<usize> {
-        let size = buf.len();
-        self.append(Bytes::from(buf.to_vec()))
-            .map(|_| size)
-            .map_err(|err| io::Error::new(io::ErrorKind::Other, err))
+    // TODO: we can cancel the upload by sending an abort request.
+    async fn abort(&mut self) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "output writer doesn't support abort",
+        ))
     }
 
-    fn flush(&mut self) -> io::Result<()> {
-        Ok(())
+    async fn close(&mut self) -> Result<()> {
+        let upload_id = if let Some(upload_id) = &self.upload_id {
+            upload_id
+        } else {
+            return Ok(());
+        };
+
+        // Make sure internal buffer has been flushed.
+        if !self.buffer.is_empty() {
+            let bs = self.buffer.peak_exact(self.buffer.len());
+
+            match self.write_part(upload_id, bs).await {
+                Ok(part) => {
+                    self.buffer.clear();
+                    self.parts.push(part);
+                }
+                Err(e) => {
+                    return Err(e);
+                }
+            }
+        }
+
+        let resp = self
+            .core
+            .oss_complete_multipart_upload_request(&self.path, upload_id, false, &self.parts)
+            .await?;
+        match resp.status() {
+            StatusCode::OK => {
+                resp.into_body().consume().await?;
+
+                Ok(())
+            }
+            _ => Err(parse_error(resp).await?),
+        }
     }
 }
```

### Comparing `opendal-0.32.0/Cargo.toml` & `opendal-0.33.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.64"
-version= "0.32.0"
+version= "0.33.0"
 
 [lib]
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 chrono = { version = "0.4.24", default-features = false, features = ["std"] }
```

### Comparing `opendal-0.32.0/.gitignore` & `opendal-0.33.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/README.md` & `opendal-0.33.0/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/benchmark/README.md` & `opendal-0.33.0/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/benchmark/async_opendal_benchmark.py` & `opendal-0.33.0/benchmark/async_opendal_benchmark.py`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/benchmark/async_origin_s3_benchmark_with_gevent.py` & `opendal-0.33.0/benchmark/async_origin_s3_benchmark_with_gevent.py`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/pyproject.toml` & `opendal-0.33.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/python/opendal/__init__.py` & `opendal-0.33.0/python/opendal/__init__.py`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/python/opendal/__init__.pyi` & `opendal-0.33.0/python/opendal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/src/asyncio.rs` & `opendal-0.33.0/src/asyncio.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/src/layers.rs` & `opendal-0.33.0/src/layers.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/src/lib.rs` & `opendal-0.33.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/tests/binding.feature` & `opendal-0.33.0/tests/binding.feature`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/tests/steps/binding.py` & `opendal-0.33.0/tests/steps/binding.py`

 * *Files identical despite different names*

### Comparing `opendal-0.32.0/Cargo.lock` & `opendal-0.33.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2288,14 +2288,31 @@
 checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
+name = "oay"
+version = "0.33.0"
+dependencies = [
+ "anyhow",
+ "clap 4.1.11",
+ "dirs",
+ "env_logger",
+ "futures",
+ "log",
+ "opendal",
+ "serde",
+ "tokio",
+ "toml 0.7.3",
+ "url",
+]
+
+[[package]]
 name = "object_store"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1ea8f683b4f89a64181393742c041520a1a87e9775e6b4c0dd5a3281af05fc6"
 dependencies = [
  "async-trait",
  "bytes",
@@ -2309,27 +2326,27 @@
  "tracing",
  "url",
  "walkdir",
 ]
 
 [[package]]
 name = "object_store_opendal"
-version = "0.32.0"
+version = "0.33.0"
 dependencies = [
  "async-trait",
  "bytes",
  "futures",
  "object_store",
  "opendal",
  "tokio",
 ]
 
 [[package]]
 name = "oli"
-version = "0.32.0"
+version = "0.33.0"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "clap 4.1.11",
  "dirs",
  "env_logger",
  "futures",
@@ -2352,15 +2369,15 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opendal"
-version = "0.32.0"
+version = "0.33.0"
 dependencies = [
  "anyhow",
  "async-compat",
  "async-tls",
  "async-trait",
  "backon",
  "base64 0.21.0",
@@ -2429,26 +2446,26 @@
 dependencies = [
  "jni",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-nodejs"
-version = "0.32.0"
+version = "0.33.0"
 dependencies = [
  "futures",
  "napi",
  "napi-build",
  "napi-derive",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-python"
-version = "0.32.0"
+version = "0.33.0"
 dependencies = [
  "chrono",
  "futures",
  "opendal",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
@@ -2456,14 +2473,16 @@
 
 [[package]]
 name = "opendal-ruby"
 version = "0.1.0"
 dependencies = [
  "magnus",
  "opendal",
+ "rb-sys",
+ "rb-sys-env",
 ]
 
 [[package]]
 name = "openssl"
 version = "0.10.47"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d8b277f87dacc05a6b709965d1cbafac4649d6ce9f3ce9ceb88508b5666dfec9"
@@ -3241,26 +3260,26 @@
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
 name = "rb-sys"
-version = "0.9.69"
+version = "0.9.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74a18381b4e31d2c3d0f7bdbcce22d53f6ff18131842d1fec1adcef6527ff573"
+checksum = "3e36bdb8be5f395264fb4345a5f6c13dac307ed3be3bccf6305b57835981c605"
 dependencies = [
  "rb-sys-build",
 ]
 
 [[package]]
 name = "rb-sys-build"
-version = "0.9.69"
+version = "0.9.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9e211890b3bd43f4d90111b7bfd863b519e3c62a5118f1bf620a0ffb43ec7f3"
+checksum = "b56f8993adac385ed6208f0dc62f99181eb0676dea50bac7bc3d36a86bb9429b"
 dependencies = [
  "bindgen 0.60.1",
  "lazy_static",
  "proc-macro2",
  "quote",
  "regex",
  "shell-words",
```

### Comparing `opendal-0.32.0/PKG-INFO` & `opendal-0.33.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendal
-Version: 0.32.0
+Version: 0.33.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pdoc; extra == 'docs'
 Requires-Dist: gevent; extra == 'benchmark'
 Requires-Dist: greenify; extra == 'benchmark'
 Requires-Dist: greenlet; extra == 'benchmark'
@@ -18,17 +18,17 @@
 Summary: OpenDAL Python Binding
 Home-Page: https://opendal.apache.org/
 Author: OpenDAL Contributors <dev@opendal.apache.org>
 Author-email: OpenDAL Contributors <dev@opendal.apache.org>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Repository, https://github.com/apache/incubator-opendal
 Project-URL: Documentation, https://opendal.apache.org/docs/python/opendal.html
 Project-URL: Homepage, https://opendal.apache.org/
+Project-URL: Repository, https://github.com/apache/incubator-opendal
 
 # OpenDAL Python Binding
 
 Documentation: [main](https://opendal.apache.org/docs/python/)
 
 This crate intends to build a native python binding.
```

