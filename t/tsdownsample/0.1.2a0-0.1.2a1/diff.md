# Comparing `tmp/tsdownsample-0.1.2a0.tar.gz` & `tmp/tsdownsample-0.1.2a1.tar.gz`

## Comparing `tsdownsample-0.1.2a0.tar` & `tsdownsample-0.1.2a1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/Cargo.toml
--rw-r--r--   0     1001      123     1078 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/LICENSE
--rw-r--r--   0     1001      123       82 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/README.md
--rw-r--r--   0     1001      123     1736 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_lttb.rs
--rw-r--r--   0     1001      123     4043 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_m4.rs
--rw-r--r--   0     1001      123     5795 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_minmax.rs
--rw-r--r--   0     1001      123     5517 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_minmaxlttb.rs
--rw-r--r--   0     1001      123     6060 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/results
--rw-r--r--   0     1001      123     1886 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/helpers.rs
--rw-r--r--   0     1001      123      211 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/lib.rs
--rw-r--r--   0     1001      123       31 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/lttb/mod.rs
--rw-r--r--   0     1001      123     8462 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/lttb/scalar.rs
--rw-r--r--   0     1001      123     7630 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/m4/generic.rs
--rw-r--r--   0     1001      123       97 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/m4/mod.rs
--rw-r--r--   0     1001      123     8766 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/m4/scalar.rs
--rw-r--r--   0     1001      123     8728 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/m4/simd.rs
--rw-r--r--   0     1001      123     6691 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmax/generic.rs
--rw-r--r--   0     1001      123       97 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmax/mod.rs
--rw-r--r--   0     1001      123     8824 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmax/scalar.rs
--rw-r--r--   0     1001      123     8852 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmax/simd.rs
--rw-r--r--   0     1001      123     2775 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmaxlttb/generic.rs
--rw-r--r--   0     1001      123       97 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmaxlttb/mod.rs
--rw-r--r--   0     1001      123     4220 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmaxlttb/scalar.rs
--rw-r--r--   0     1001      123     4214 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmaxlttb/simd.rs
--rw-r--r--   0     1001      123    11715 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/searchsorted.rs
--rw-r--r--   0     1001      123      375 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/types.rs
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 tsdownsample-0.1.2a0/Cargo.toml
--rw-r--r--   0     1001      123     4159 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/.github/workflows/ci-downsample_rs.yml
--rw-r--r--   0     1001      123     5514 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/.github/workflows/ci-tsdownsample.yml
--rw-r--r--   0     1001      123     1195 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/.github/workflows/codspeed.yml
--rw-r--r--   0     1001      123     2302 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/.gitignore
--rw-r--r--   0     1001      123     3004 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1078 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/LICENSE
--rw-r--r--   0     1001      123     1336 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/Makefile
--rw-r--r--   0     1001      123     5931 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/README.md
--rw-r--r--   0     1001      123     1616 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/pyproject.toml
--rw-r--r--   0     1001      123    13461 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/benchmarks/__init__.py
--rw-r--r--   0     1001      123     6594 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/benchmarks/test_downsamplers.py
--rw-r--r--   0     1001      123       16 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/requirements-linting.txt
--rw-r--r--   0     1001      123       35 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/requirements.txt
--rw-r--r--   0     1001      123     1026 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/test_algos_python_compliance.py
--rw-r--r--   0     1001      123      599 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/test_config.py
--rw-r--r--   0     1001      123     1489 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/test_rust_mods.py
--rw-r--r--   0     1001      123    10222 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/test_tsdownsample.py
--rw-r--r--   0     1001      123      437 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tsdownsample/__init__.py
--rw-r--r--   0     1001      123        0 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tsdownsample/_python/__init__.py
--rw-r--r--   0     1001      123     6358 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tsdownsample/_python/downsamplers.py
--rw-r--r--   0     1001      123       58 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tsdownsample/_rust/__init__.py
--rw-r--r--   0     1001      123     2107 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tsdownsample/downsamplers.py
--rw-r--r--   0     1001      123    12370 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tsdownsample/downsampling_interface.py
--rw-r--r--   0     1001      123    13037 2023-04-12 17:22:03.000000 tsdownsample-0.1.2a0/Cargo.lock
--rw-r--r--   0        0        0     6952 1970-01-01 00:00:00.000000 tsdownsample-0.1.2a0/PKG-INFO
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/Cargo.toml
+-rw-r--r--   0     1001      123     1078 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/LICENSE
+-rw-r--r--   0     1001      123       82 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/README.md
+-rw-r--r--   0     1001      123     1736 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/benches/bench_lttb.rs
+-rw-r--r--   0     1001      123     4043 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/benches/bench_m4.rs
+-rw-r--r--   0     1001      123     5795 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/benches/bench_minmax.rs
+-rw-r--r--   0     1001      123     5517 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/benches/bench_minmaxlttb.rs
+-rw-r--r--   0     1001      123     6060 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/benches/results
+-rw-r--r--   0     1001      123     1886 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/helpers.rs
+-rw-r--r--   0     1001      123      211 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/lib.rs
+-rw-r--r--   0     1001      123       31 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/lttb/mod.rs
+-rw-r--r--   0     1001      123     8462 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/lttb/scalar.rs
+-rw-r--r--   0     1001      123     7630 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/m4/generic.rs
+-rw-r--r--   0     1001      123       97 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/m4/mod.rs
+-rw-r--r--   0     1001      123     8766 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/m4/scalar.rs
+-rw-r--r--   0     1001      123     8728 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/m4/simd.rs
+-rw-r--r--   0     1001      123     6691 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/minmax/generic.rs
+-rw-r--r--   0     1001      123       97 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/minmax/mod.rs
+-rw-r--r--   0     1001      123     8824 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/minmax/scalar.rs
+-rw-r--r--   0     1001      123     8852 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/minmax/simd.rs
+-rw-r--r--   0     1001      123     2775 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/minmaxlttb/generic.rs
+-rw-r--r--   0     1001      123       97 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/minmaxlttb/mod.rs
+-rw-r--r--   0     1001      123     4220 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/minmaxlttb/scalar.rs
+-rw-r--r--   0     1001      123     4214 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/minmaxlttb/simd.rs
+-rw-r--r--   0     1001      123    11715 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/searchsorted.rs
+-rw-r--r--   0     1001      123      375 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/types.rs
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 tsdownsample-0.1.2a1/Cargo.toml
+-rw-r--r--   0     1001      123     4159 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/.github/workflows/ci-downsample_rs.yml
+-rw-r--r--   0     1001      123     5514 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/.github/workflows/ci-tsdownsample.yml
+-rw-r--r--   0     1001      123     1195 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/.github/workflows/codspeed.yml
+-rw-r--r--   0     1001      123     2302 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/.gitignore
+-rw-r--r--   0     1001      123     3004 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1078 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/LICENSE
+-rw-r--r--   0     1001      123     1336 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/Makefile
+-rw-r--r--   0     1001      123     5931 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/README.md
+-rw-r--r--   0     1001      123     1616 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/pyproject.toml
+-rw-r--r--   0     1001      123    13461 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/tests/benchmarks/__init__.py
+-rw-r--r--   0     1001      123     6594 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/tests/benchmarks/test_downsamplers.py
+-rw-r--r--   0     1001      123       16 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/tests/requirements-linting.txt
+-rw-r--r--   0     1001      123       35 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/tests/requirements.txt
+-rw-r--r--   0     1001      123     1026 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/tests/test_algos_python_compliance.py
+-rw-r--r--   0     1001      123      599 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/tests/test_config.py
+-rw-r--r--   0     1001      123     1489 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/tests/test_rust_mods.py
+-rw-r--r--   0     1001      123    10657 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/tests/test_tsdownsample.py
+-rw-r--r--   0     1001      123      437 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/tsdownsample/__init__.py
+-rw-r--r--   0     1001      123        0 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/tsdownsample/_python/__init__.py
+-rw-r--r--   0     1001      123     6358 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/tsdownsample/_python/downsamplers.py
+-rw-r--r--   0     1001      123       58 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/tsdownsample/_rust/__init__.py
+-rw-r--r--   0     1001      123     2117 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/tsdownsample/downsamplers.py
+-rw-r--r--   0     1001      123    12998 2023-04-14 16:05:55.000000 tsdownsample-0.1.2a1/tsdownsample/downsampling_interface.py
+-rw-r--r--   0     1001      123    13037 2023-04-14 16:06:38.000000 tsdownsample-0.1.2a1/Cargo.lock
+-rw-r--r--   0        0        0     6952 1970-01-01 00:00:00.000000 tsdownsample-0.1.2a1/PKG-INFO
```

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/Cargo.toml` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/LICENSE` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/LICENSE`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_lttb.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/benches/bench_lttb.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_m4.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/benches/bench_m4.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_minmax.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/benches/bench_minmax.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_minmaxlttb.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/benches/bench_minmaxlttb.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/results` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/benches/results`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/helpers.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/lttb/scalar.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/lttb/scalar.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/m4/generic.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/m4/generic.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/m4/scalar.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/m4/scalar.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/m4/simd.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/m4/simd.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmax/generic.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/minmax/generic.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmax/scalar.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/minmax/scalar.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmax/simd.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/minmax/simd.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmaxlttb/generic.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/minmaxlttb/generic.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmaxlttb/scalar.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/minmaxlttb/scalar.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmaxlttb/simd.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/minmaxlttb/simd.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/searchsorted.rs` & `tsdownsample-0.1.2a1/local_dependencies/downsample_rs/src/searchsorted.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/Cargo.toml` & `tsdownsample-0.1.2a1/Cargo.toml`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/.github/workflows/ci-downsample_rs.yml` & `tsdownsample-0.1.2a1/.github/workflows/ci-downsample_rs.yml`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/.github/workflows/ci-tsdownsample.yml` & `tsdownsample-0.1.2a1/.github/workflows/ci-tsdownsample.yml`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/.github/workflows/codspeed.yml` & `tsdownsample-0.1.2a1/.github/workflows/codspeed.yml`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/.gitignore` & `tsdownsample-0.1.2a1/.gitignore`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/CONTRIBUTING.md` & `tsdownsample-0.1.2a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/LICENSE` & `tsdownsample-0.1.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/Makefile` & `tsdownsample-0.1.2a1/Makefile`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/README.md` & `tsdownsample-0.1.2a1/README.md`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/pyproject.toml` & `tsdownsample-0.1.2a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "tsdownsample"
 description = "Time series downsampling in rust"
-version = "0.1.2a0"
+version = "0.1.2a1"
 requires-python = ">=3.7"
 dependencies = ["numpy"]
 authors = [{name = "Jeroen Van Der Donckt"}]
 readme = "README.md"
 license = {text = "MIT"}
 keywords = ["time series", "downsampling", "rust", "data science", "visualization"]
 classifiers = [
```

### Comparing `tsdownsample-0.1.2a0/src/lib.rs` & `tsdownsample-0.1.2a1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/tests/benchmarks/test_downsamplers.py` & `tsdownsample-0.1.2a1/tests/benchmarks/test_downsamplers.py`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/tests/test_algos_python_compliance.py` & `tsdownsample-0.1.2a1/tests/test_algos_python_compliance.py`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/tests/test_config.py` & `tsdownsample-0.1.2a1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/tests/test_rust_mods.py` & `tsdownsample-0.1.2a1/tests/test_rust_mods.py`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/tests/test_tsdownsample.py` & `tsdownsample-0.1.2a1/tests/test_tsdownsample.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,29 +34,42 @@
 
 def generate_all_downsamplers() -> Iterable[AbstractDownsampler]:
     for downsampler in RUST_DOWNSAMPLERS + OTHER_DOWNSAMPLERS:
         yield downsampler
 
 
 @pytest.mark.parametrize("downsampler", generate_all_downsamplers())
-def test_serialization(downsampler: AbstractDownsampler):
+def test_serialization_copy(downsampler: AbstractDownsampler):
     """Test serialization."""
     from copy import copy, deepcopy
 
     dc = copy(downsampler)
     ddc = deepcopy(downsampler)
 
     arr = np.arange(10_000)
     orig_downsampled = downsampler.downsample(arr, n_out=100)
     dc_downsampled = dc.downsample(arr, n_out=100)
     ddc_downsampled = ddc.downsample(arr, n_out=100)
     assert np.all(orig_downsampled == dc_downsampled)
     assert np.all(orig_downsampled == ddc_downsampled)
 
 
+@pytest.mark.parametrize("downsampler", generate_all_downsamplers())
+def test_serialization_pickle(downsampler: AbstractDownsampler):
+    """Test serialization."""
+    import pickle
+
+    dc = pickle.loads(pickle.dumps(downsampler))
+
+    arr = np.arange(10_000)
+    orig_downsampled = downsampler.downsample(arr, n_out=100)
+    dc_downsampled = dc.downsample(arr, n_out=100)
+    assert np.all(orig_downsampled == dc_downsampled)
+
+
 @pytest.mark.parametrize("downsampler", generate_rust_downsamplers())
 def test_rust_downsampler(downsampler: AbstractDownsampler):
     """Test the Rust downsamplers."""
     arr = np.arange(10_000)
     s_downsampled = downsampler.downsample(arr, n_out=100)
     assert s_downsampled[0] == 0
     assert s_downsampled[-1] == len(arr) - 1
```

### Comparing `tsdownsample-0.1.2a0/tsdownsample/_python/downsamplers.py` & `tsdownsample-0.1.2a1/tsdownsample/_python/downsamplers.py`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.2a0/tsdownsample/downsamplers.py` & `tsdownsample-0.1.2a1/tsdownsample/downsamplers.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,43 +6,47 @@
 # ------------------ Rust Downsamplers ------------------
 from tsdownsample._rust import _tsdownsample_rs  # type: ignore[attr-defined]
 
 from .downsampling_interface import AbstractDownsampler, AbstractRustDownsampler
 
 
 class MinMaxDownsampler(AbstractRustDownsampler):
-    def __init__(self) -> None:
-        super().__init__(_tsdownsample_rs.minmax)
+    @property
+    def rust_mod(self):
+        return _tsdownsample_rs.minmax
 
     @staticmethod
     def _check_valid_n_out(n_out: int):
         AbstractRustDownsampler._check_valid_n_out(n_out)
         if n_out % 2 != 0:
             raise ValueError("n_out must be even")
 
 
 class M4Downsampler(AbstractRustDownsampler):
-    def __init__(self):
-        super().__init__(_tsdownsample_rs.m4)
+    @property
+    def rust_mod(self):
+        return _tsdownsample_rs.m4
 
     @staticmethod
     def _check_valid_n_out(n_out: int):
         AbstractRustDownsampler._check_valid_n_out(n_out)
         if n_out % 4 != 0:
             raise ValueError("n_out must be a multiple of 4")
 
 
 class LTTBDownsampler(AbstractRustDownsampler):
-    def __init__(self):
-        super().__init__(_tsdownsample_rs.lttb)
+    @property
+    def rust_mod(self):
+        return _tsdownsample_rs.lttb
 
 
 class MinMaxLTTBDownsampler(AbstractRustDownsampler):
-    def __init__(self):
-        super().__init__(_tsdownsample_rs.minmaxlttb)
+    @property
+    def rust_mod(self):
+        return _tsdownsample_rs.minmaxlttb
 
     def downsample(
         self, *args, n_out: int, minmax_ratio: int = 30, parallel: bool = False, **_
     ):
         assert minmax_ratio > 0, "minmax_ratio must be greater than 0"
         return super().downsample(
             *args, n_out=n_out, parallel=parallel, ratio=minmax_ratio
@@ -59,8 +63,8 @@
         if x is not None:
             name = self.__class__.__name__
             warnings.warn(
                 f"x is passed to downsample method of {name}, but is not taken "
                 "into account by the current implementation of the EveryNth algorithm."
             )
         step = max(1, len(y) / n_out)
-        return np.arange(start=0, stop=len(y), step=step).astype(np.uint)
+        return np.arange(start=0, stop=len(y) - 0.1, step=step).astype(np.uint)
```

### Comparing `tsdownsample-0.1.2a0/tsdownsample/downsampling_interface.py` & `tsdownsample-0.1.2a1/tsdownsample/downsampling_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,32 +139,55 @@
 # downsampling
 _y_rust_dtypes = _rust_dtypes + ["float16", "int8", "uint8", "bool"]
 
 
 class AbstractRustDownsampler(AbstractDownsampler, ABC):
     """RustDownsampler interface-class, subclassed by concrete downsamplers."""
 
-    def __init__(self, resampling_mod: ModuleType):
+    def __init__(self):
         super().__init__(_rust_dtypes, _y_rust_dtypes)  # same for x and y
-        self.rust_mod = resampling_mod
 
-        # Store the single core sub module
-        self.mod_single_core = self.rust_mod.scalar
+    @property
+    def rust_mod(self) -> ModuleType:
+        """The compiled Rust module for the current downsampler."""
+        raise NotImplementedError
+
+    @property
+    def mod_single_core(self) -> ModuleType:
+        """Get the single-core Rust module.
+
+        Returns
+        -------
+        ModuleType
+            If SIMD compiled module is available, that one is returned. Otherwise, the
+            scalar compiled module is returned.
+        """
         if hasattr(self.rust_mod, "simd"):
             # use SIMD implementation if available
-            self.mod_single_core = self.rust_mod.simd
+            return self.rust_mod.simd
+        return self.rust_mod.scalar
 
-        # Store the multi-core sub module (if present)
-        self.mod_multi_core = None  # no multi-core implementation (default)
+    @property
+    def mod_multi_core(self) -> Union[ModuleType, None]:
+        """Get the multi-core Rust module.
+
+        Returns
+        -------
+        ModuleType or None
+            If SIMD parallel compiled module is available, that one is returned.
+            Otherwise, the scalar parallel compiled module is returned.
+            If no parallel compiled module is available, None is returned.
+        """
         if hasattr(self.rust_mod, "simd_parallel"):
             # use SIMD implementation if available
-            self.mod_multi_core = self.rust_mod.simd_parallel
+            return self.rust_mod.simd_parallel
         elif hasattr(self.rust_mod, "scalar_parallel"):
             # use scalar implementation if available (when no SIMD available)
-            self.mod_multi_core = self.rust_mod.scalar_parallel
+            return self.rust_mod.scalar_parallel
+        return None  # no parallel compiled module available
 
     @staticmethod
     def _switch_mod_with_y(
         y_dtype: np.dtype, mod: ModuleType, downsample_func: str = DOWNSAMPLE_F
     ) -> Callable:
         """The x-data is not considered in the downsampling
```

### Comparing `tsdownsample-0.1.2a0/Cargo.lock` & `tsdownsample-0.1.2a1/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -273,66 +273,66 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
```

### Comparing `tsdownsample-0.1.2a0/PKG-INFO` & `tsdownsample-0.1.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsdownsample
-Version: 0.1.2a0
+Version: 0.1.2a1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,16 +16,16 @@
 License-File: LICENSE
 Summary: Time series downsampling in rust
 Keywords: time series,downsampling,rust,data science,visualization
 Author: Jeroen Van Der Donckt
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Homepage, https://github.com/predict-idlab/tsdownsample
 Project-URL: Repository, https://github.com/predict-idlab/tsdownsample
+Project-URL: Homepage, https://github.com/predict-idlab/tsdownsample
 
 # tsdownsample
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/tsdownsample.svg)](https://pypi.org/project/tsdownsample/)
 [![support-version](https://img.shields.io/pypi/pyversions/tsdownsample)](https://img.shields.io/pypi/pyversions/tsdownsample)
 [![Downloads](https://pepy.tech/badge/tsdownsample)](https://pepy.tech/project/tsdownsample)
 [![Testing](https://github.com/predict-idlab/tsdownsample/actions/workflows/ci-downsample_rs.yml/badge.svg)](https://github.com/predict-idlab/tsdownsample/actions/workflows/ci-downsample_rs.yml)
```

#### html2text {}

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1 Name: tsdownsample Version: 0.1.2a0 Classifier: Intended
+Metadata-Version: 2.1 Name: tsdownsample Version: 0.1.2a1 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Requires-Dist:
 numpy License-File: LICENSE Summary: Time series downsampling in rust Keywords:
 time series,downsampling,rust,data science,visualization Author: Jeroen Van Der
 Donckt License: MIT Requires-Python: >=3.7 Description-Content-Type: text/
-markdown; charset=UTF-8; variant=GFM Project-URL: Homepage, https://github.com/
-predict-idlab/tsdownsample Project-URL: Repository, https://github.com/predict-
-idlab/tsdownsample # tsdownsample [![PyPI Latest Release](https://
-img.shields.io/pypi/v/tsdownsample.svg)](https://pypi.org/project/tsdownsample/
-) [![support-version](https://img.shields.io/pypi/pyversions/tsdownsample)]
-(https://img.shields.io/pypi/pyversions/tsdownsample) [![Downloads](https://
-pepy.tech/badge/tsdownsample)](https://pepy.tech/project/tsdownsample) [!
-[Testing](https://github.com/predict-idlab/tsdownsample/actions/workflows/ci-
-downsample_rs.yml/badge.svg)](https://github.com/predict-idlab/tsdownsample/
-actions/workflows/ci-downsample_rs.yml) [![Testing](https://github.com/predict-
-idlab/tsdownsample/actions/workflows/ci-tsdownsample.yml/badge.svg)](https://
-github.com/predict-idlab/tsdownsample/actions/workflows/ci-tsdownsample.yml)
-Extremely fast **time series downsampling ð** for visualization, written in
-Rust. ## Features â¨ * **Fast**: written in rust with PyO3 bindings -
-leverages optimized [argminmax](https://github.com/jvdd/argminmax) - which is
-SIMD accelerated with runtime feature detection - scales linearly with the
-number of data points  - multithreaded with Rayon (in Rust)  Why we do not use
-Python multiprocessing Citing the PyO3_docs_on_parallelism:
+markdown; charset=UTF-8; variant=GFM Project-URL: Repository, https://
+github.com/predict-idlab/tsdownsample Project-URL: Homepage, https://
+github.com/predict-idlab/tsdownsample # tsdownsample [![PyPI Latest Release]
+(https://img.shields.io/pypi/v/tsdownsample.svg)](https://pypi.org/project/
+tsdownsample/) [![support-version](https://img.shields.io/pypi/pyversions/
+tsdownsample)](https://img.shields.io/pypi/pyversions/tsdownsample) [!
+[Downloads](https://pepy.tech/badge/tsdownsample)](https://pepy.tech/project/
+tsdownsample) [![Testing](https://github.com/predict-idlab/tsdownsample/
+actions/workflows/ci-downsample_rs.yml/badge.svg)](https://github.com/predict-
+idlab/tsdownsample/actions/workflows/ci-downsample_rs.yml) [![Testing](https://
+github.com/predict-idlab/tsdownsample/actions/workflows/ci-tsdownsample.yml/
+badge.svg)](https://github.com/predict-idlab/tsdownsample/actions/workflows/ci-
+tsdownsample.yml)  Extremely fast **time series downsampling ð** for
+visualization, written in Rust. ## Features â¨ * **Fast**: written in rust
+with PyO3 bindings - leverages optimized [argminmax](https://github.com/jvdd/
+argminmax) - which is SIMD accelerated with runtime feature detection - scales
+linearly with the number of data points  - multithreaded with Rayon (in Rust)
+Why we do not use Python multiprocessing Citing the PyO3_docs_on_parallelism:
      CPython has the infamous Global Interpreter Lock, which prevents
      several threads from executing Python bytecode in parallel. This
      makes threading in Python a bad fit for CPU-bound tasks and often
      forces developers to accept the overhead of multiprocessing.
 In Rust - which is a compiled language - there is no GIL, so CPU-bound tasks
 can be parallelized (with Rayon) with little to no overhead.  * **Efficient**:
 memory efficient - works on views of the data (no copies) - no intermediate
```

