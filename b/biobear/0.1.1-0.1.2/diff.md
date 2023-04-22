# Comparing `tmp/biobear-0.1.1.tar.gz` & `tmp/biobear-0.1.2.tar.gz`

## Comparing `biobear-0.1.1.tar` & `biobear-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 biobear-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123     2948 2023-04-22 20:50:36.000000 biobear-0.1.1/.github/workflows/build-test-release.yml
--rw-r--r--   0     1001      123     4135 2023-04-22 20:50:36.000000 biobear-0.1.1/.gitignore
--rw-r--r--   0     1001      123       68 2023-04-22 20:50:36.000000 biobear-0.1.1/Makefile
--rw-r--r--   0     1001      123      167 2023-04-22 20:50:36.000000 biobear-0.1.1/cz.json
--rw-r--r--   0     1001      123      421 2023-04-22 20:50:36.000000 biobear-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123      155 2023-04-22 20:50:36.000000 biobear-0.1.1/python/biobear/__init__.py
--rw-r--r--   0     1001      123      889 2023-04-22 20:50:36.000000 biobear-0.1.1/python/biobear/bam_reader.py
--rw-r--r--   0     1001      123      383 2023-04-22 20:50:36.000000 biobear-0.1.1/python/biobear/fasta_reader.py
--rw-r--r--   0     1001      123      383 2023-04-22 20:50:36.000000 biobear-0.1.1/python/biobear/fastq_reader.py
--rw-r--r--   0     1001      123      857 2023-04-22 20:50:36.000000 biobear-0.1.1/python/biobear/vcf_reader.py
--rw-r--r--   0     1001      123      286 2023-04-22 20:50:36.000000 biobear-0.1.1/python/tests/data/test.fastq
--rw-r--r--   0     1001      123      411 2023-04-22 20:50:36.000000 biobear-0.1.1/python/tests/test_fasta_reader.py
--rw-r--r--   0     1001      123      320 2023-04-22 20:50:36.000000 biobear-0.1.1/python/tests/test_fastq_reader.py
--rw-r--r--   0     1001      123       87 2023-04-22 20:50:36.000000 biobear-0.1.1/python/tests/test_version.py
--rw-r--r--   0     1001      123     7737 2023-04-22 20:50:36.000000 biobear-0.1.1/src/bam_reader.rs
--rw-r--r--   0     1001      123     2989 2023-04-22 20:50:36.000000 biobear-0.1.1/src/fasta_reader.rs
--rw-r--r--   0     1001      123     3505 2023-04-22 20:50:36.000000 biobear-0.1.1/src/fastq_reader.rs
--rw-r--r--   0     1001      123     4643 2023-04-22 20:50:36.000000 biobear-0.1.1/src/gff_reader.rs
--rw-r--r--   0     1001      123      526 2023-04-22 20:50:36.000000 biobear-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123     6420 2023-04-22 20:50:36.000000 biobear-0.1.1/src/vcf_reader.rs
--rw-r--r--   0     1001      123    37517 2023-04-22 20:51:23.000000 biobear-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 biobear-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 biobear-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      123     2921 2023-04-22 20:57:52.000000 biobear-0.1.2/.github/workflows/build-test-release.yml
+-rw-r--r--   0     1001      123     4135 2023-04-22 20:57:52.000000 biobear-0.1.2/.gitignore
+-rw-r--r--   0     1001      123       68 2023-04-22 20:57:52.000000 biobear-0.1.2/Makefile
+-rw-r--r--   0     1001      123      167 2023-04-22 20:57:52.000000 biobear-0.1.2/cz.json
+-rw-r--r--   0     1001      123      421 2023-04-22 20:57:52.000000 biobear-0.1.2/pyproject.toml
+-rw-r--r--   0     1001      123      155 2023-04-22 20:57:52.000000 biobear-0.1.2/python/biobear/__init__.py
+-rw-r--r--   0     1001      123      889 2023-04-22 20:57:52.000000 biobear-0.1.2/python/biobear/bam_reader.py
+-rw-r--r--   0     1001      123      383 2023-04-22 20:57:52.000000 biobear-0.1.2/python/biobear/fasta_reader.py
+-rw-r--r--   0     1001      123      383 2023-04-22 20:57:52.000000 biobear-0.1.2/python/biobear/fastq_reader.py
+-rw-r--r--   0     1001      123      857 2023-04-22 20:57:52.000000 biobear-0.1.2/python/biobear/vcf_reader.py
+-rw-r--r--   0     1001      123      286 2023-04-22 20:57:52.000000 biobear-0.1.2/python/tests/data/test.fastq
+-rw-r--r--   0     1001      123      411 2023-04-22 20:57:52.000000 biobear-0.1.2/python/tests/test_fasta_reader.py
+-rw-r--r--   0     1001      123      320 2023-04-22 20:57:52.000000 biobear-0.1.2/python/tests/test_fastq_reader.py
+-rw-r--r--   0     1001      123       87 2023-04-22 20:57:52.000000 biobear-0.1.2/python/tests/test_version.py
+-rw-r--r--   0     1001      123     7737 2023-04-22 20:57:52.000000 biobear-0.1.2/src/bam_reader.rs
+-rw-r--r--   0     1001      123     2989 2023-04-22 20:57:52.000000 biobear-0.1.2/src/fasta_reader.rs
+-rw-r--r--   0     1001      123     3505 2023-04-22 20:57:52.000000 biobear-0.1.2/src/fastq_reader.rs
+-rw-r--r--   0     1001      123     4643 2023-04-22 20:57:52.000000 biobear-0.1.2/src/gff_reader.rs
+-rw-r--r--   0     1001      123      526 2023-04-22 20:57:52.000000 biobear-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      123     6420 2023-04-22 20:57:52.000000 biobear-0.1.2/src/vcf_reader.rs
+-rw-r--r--   0     1001      123    37517 2023-04-22 20:58:38.000000 biobear-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 biobear-0.1.2/PKG-INFO
```

### Comparing `biobear-0.1.1/.github/workflows/build-test-release.yml` & `biobear-0.1.2/.github/workflows/build-test-release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,15 @@
   contents: read
 
 jobs:
   linux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        # target: [x86_64, x86, aarch64, armv7, s390x, ppc64le]
-        target: [x86_64]
+        target: [x86_64, x86, aarch64, armv7, s390x, ppc64le]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
```

### Comparing `biobear-0.1.1/.gitignore` & `biobear-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `biobear-0.1.1/python/biobear/bam_reader.py` & `biobear-0.1.2/python/biobear/bam_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.1.1/python/biobear/vcf_reader.py` & `biobear-0.1.2/python/biobear/vcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.1.1/src/bam_reader.rs` & `biobear-0.1.2/src/bam_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.1/src/fasta_reader.rs` & `biobear-0.1.2/src/fasta_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.1/src/fastq_reader.rs` & `biobear-0.1.2/src/fastq_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.1/src/gff_reader.rs` & `biobear-0.1.2/src/gff_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.1/src/lib.rs` & `biobear-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.1/src/vcf_reader.rs` & `biobear-0.1.2/src/vcf_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.1/Cargo.lock` & `biobear-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "biobear"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "arrow",
  "noodles",
  "pyo3",
 ]
 
 [[package]]
```

