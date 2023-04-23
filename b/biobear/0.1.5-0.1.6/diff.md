# Comparing `tmp/biobear-0.1.5.tar.gz` & `tmp/biobear-0.1.6.tar.gz`

## Comparing `biobear-0.1.5.tar` & `biobear-0.1.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 biobear-0.1.5/Cargo.toml
--rw-r--r--   0     1001      123     2663 2023-04-22 22:41:16.000000 biobear-0.1.5/.github/workflows/build-test-release.yml
--rw-r--r--   0     1001      123     4135 2023-04-22 22:41:16.000000 biobear-0.1.5/.gitignore
--rw-r--r--   0     1001      123     1055 2023-04-22 22:41:16.000000 biobear-0.1.5/LICENSE
--rw-r--r--   0     1001      123       68 2023-04-22 22:41:16.000000 biobear-0.1.5/Makefile
--rw-r--r--   0     1001      123     1520 2023-04-22 22:41:16.000000 biobear-0.1.5/README.md
--rw-r--r--   0     1001      123      167 2023-04-22 22:41:16.000000 biobear-0.1.5/cz.json
--rw-r--r--   0     1001      123      421 2023-04-22 22:41:16.000000 biobear-0.1.5/pyproject.toml
--rw-r--r--   0     1001      123      401 2023-04-22 22:41:16.000000 biobear-0.1.5/python/biobear/__init__.py
--rw-r--r--   0     1001      123      895 2023-04-22 22:41:16.000000 biobear-0.1.5/python/biobear/bam_reader.py
--rw-r--r--   0     1001      123      383 2023-04-22 22:41:16.000000 biobear-0.1.5/python/biobear/fasta_reader.py
--rw-r--r--   0     1001      123      383 2023-04-22 22:41:16.000000 biobear-0.1.5/python/biobear/fastq_reader.py
--rw-r--r--   0     1001      123      373 2023-04-22 22:41:16.000000 biobear-0.1.5/python/biobear/gff_reader.py
--rw-r--r--   0     1001      123      838 2023-04-22 22:41:16.000000 biobear-0.1.5/python/biobear/vcf_reader.py
--rw-r--r--   0     1001      123     6152 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/bedcov.bam
--rw-r--r--   0     1001      123     7608 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/bedcov.bam.bai
--rw-r--r--   0     1001      123     1749 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/file.vcf
--rw-r--r--   0     1001      123     8296 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/index.vcf.gz
--rw-r--r--   0     1001      123      212 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/index.vcf.gz.tbi
--rw-r--r--   0     1001      123      286 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/test.fastq
--rw-r--r--   0     1001      123      112 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/test.gff
--rw-r--r--   0     1001      123     4302 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/vcf_file.vcf
--rw-r--r--   0     1001      123     1669 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/vcf_file.vcf.gz
--rw-r--r--   0     1001      123      254 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/vcf_file.vcf.gz.tbi
--rw-r--r--   0     1001      123      513 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/test_bam_reader.py
--rw-r--r--   0     1001      123      411 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/test_fasta_reader.py
--rw-r--r--   0     1001      123      300 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/test_fastq_reader.py
--rw-r--r--   0     1001      123      295 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/test_gff_reader.py
--rw-r--r--   0     1001      123      591 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/test_vcf_reader.py
--rw-r--r--   0     1001      123     7737 2023-04-22 22:41:16.000000 biobear-0.1.5/src/bam_reader.rs
--rw-r--r--   0     1001      123     2989 2023-04-22 22:41:16.000000 biobear-0.1.5/src/fasta_reader.rs
--rw-r--r--   0     1001      123     3505 2023-04-22 22:41:16.000000 biobear-0.1.5/src/fastq_reader.rs
--rw-r--r--   0     1001      123     4645 2023-04-22 22:41:16.000000 biobear-0.1.5/src/gff_reader.rs
--rw-r--r--   0     1001      123      526 2023-04-22 22:41:16.000000 biobear-0.1.5/src/lib.rs
--rw-r--r--   0     1001      123     6420 2023-04-22 22:41:16.000000 biobear-0.1.5/src/vcf_reader.rs
--rw-r--r--   0     1001      123    37517 2023-04-22 22:42:15.000000 biobear-0.1.5/Cargo.lock
--rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 biobear-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 biobear-0.1.6/Cargo.toml
+-rw-r--r--   0     1001      123     2663 2023-04-23 00:24:08.000000 biobear-0.1.6/.github/workflows/build-test-release.yml
+-rw-r--r--   0     1001      123     4135 2023-04-23 00:24:08.000000 biobear-0.1.6/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-04-23 00:24:08.000000 biobear-0.1.6/LICENSE
+-rw-r--r--   0     1001      123       68 2023-04-23 00:24:08.000000 biobear-0.1.6/Makefile
+-rw-r--r--   0     1001      123     6254 2023-04-23 00:24:08.000000 biobear-0.1.6/README.md
+-rw-r--r--   0     1001      123      167 2023-04-23 00:24:08.000000 biobear-0.1.6/cz.json
+-rw-r--r--   0     1001      123      421 2023-04-23 00:24:08.000000 biobear-0.1.6/pyproject.toml
+-rw-r--r--   0     1001      123      401 2023-04-23 00:24:08.000000 biobear-0.1.6/python/biobear/__init__.py
+-rw-r--r--   0     1001      123      895 2023-04-23 00:24:08.000000 biobear-0.1.6/python/biobear/bam_reader.py
+-rw-r--r--   0     1001      123      383 2023-04-23 00:24:08.000000 biobear-0.1.6/python/biobear/fasta_reader.py
+-rw-r--r--   0     1001      123      383 2023-04-23 00:24:08.000000 biobear-0.1.6/python/biobear/fastq_reader.py
+-rw-r--r--   0     1001      123      373 2023-04-23 00:24:08.000000 biobear-0.1.6/python/biobear/gff_reader.py
+-rw-r--r--   0     1001      123      838 2023-04-23 00:24:08.000000 biobear-0.1.6/python/biobear/vcf_reader.py
+-rw-r--r--   0     1001      123     6152 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/bedcov.bam
+-rw-r--r--   0     1001      123     7608 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/bedcov.bam.bai
+-rw-r--r--   0     1001      123     1749 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/file.vcf
+-rw-r--r--   0     1001      123     8296 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/index.vcf.gz
+-rw-r--r--   0     1001      123      212 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/index.vcf.gz.tbi
+-rw-r--r--   0     1001      123      286 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/test.fastq
+-rw-r--r--   0     1001      123      112 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/test.gff
+-rw-r--r--   0     1001      123     4302 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/vcf_file.vcf
+-rw-r--r--   0     1001      123     1669 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/vcf_file.vcf.gz
+-rw-r--r--   0     1001      123      254 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      123      483 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/test_bam_reader.py
+-rw-r--r--   0     1001      123      411 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/test_fasta_reader.py
+-rw-r--r--   0     1001      123      300 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/test_fastq_reader.py
+-rw-r--r--   0     1001      123      280 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/test_gff_reader.py
+-rw-r--r--   0     1001      123      591 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/test_vcf_reader.py
+-rw-r--r--   0     1001      123     7737 2023-04-23 00:24:08.000000 biobear-0.1.6/src/bam_reader.rs
+-rw-r--r--   0     1001      123     2989 2023-04-23 00:24:08.000000 biobear-0.1.6/src/fasta_reader.rs
+-rw-r--r--   0     1001      123     3505 2023-04-23 00:24:08.000000 biobear-0.1.6/src/fastq_reader.rs
+-rw-r--r--   0     1001      123     4645 2023-04-23 00:24:08.000000 biobear-0.1.6/src/gff_reader.rs
+-rw-r--r--   0     1001      123      526 2023-04-23 00:24:08.000000 biobear-0.1.6/src/lib.rs
+-rw-r--r--   0     1001      123     6420 2023-04-23 00:24:08.000000 biobear-0.1.6/src/vcf_reader.rs
+-rw-r--r--   0     1001      123    37517 2023-04-23 00:25:00.000000 biobear-0.1.6/Cargo.lock
+-rw-r--r--   0        0        0     6632 1970-01-01 00:00:00.000000 biobear-0.1.6/PKG-INFO
```

### Comparing `biobear-0.1.5/.github/workflows/build-test-release.yml` & `biobear-0.1.6/.github/workflows/build-test-release.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/.gitignore` & `biobear-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/LICENSE` & `biobear-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/python/biobear/bam_reader.py` & `biobear-0.1.6/python/biobear/bam_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/python/biobear/vcf_reader.py` & `biobear-0.1.6/python/biobear/vcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/python/tests/data/bedcov.bam` & `biobear-0.1.6/python/tests/data/bedcov.bam`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/python/tests/data/bedcov.bam.bai` & `biobear-0.1.6/python/tests/data/bedcov.bam.bai`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/python/tests/data/file.vcf` & `biobear-0.1.6/python/tests/data/file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/python/tests/data/index.vcf.gz` & `biobear-0.1.6/python/tests/data/index.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/python/tests/data/vcf_file.vcf` & `biobear-0.1.6/python/tests/data/vcf_file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/python/tests/data/vcf_file.vcf.gz` & `biobear-0.1.6/python/tests/data/vcf_file.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/python/tests/test_bam_reader.py` & `biobear-0.1.6/python/tests/test_vcf_reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # Test the fasta reader can be converted to a polars dataframe
 
 from pathlib import Path
 
-from biobear import BamReader, BamIndexedReader
+from biobear import VCFReader, VCFIndexedReader
 
 DATA = Path(__file__).parent / "data"
 
 
-def test_bam_reader():
-    reader = BamReader(DATA / "bedcov.bam")
+def test_vcf_reader():
+    reader = VCFReader(DATA / "vcf_file.vcf")
     df = reader.to_polars()
 
-    print(df)
+    assert len(df) == 15
 
-    assert len(df) == 61
+def test_sam_indexed_reader_read():
+    reader = VCFIndexedReader(DATA / "vcf_file.vcf.gz")
+    df = reader.read()
 
-def test_sam_indexed_reader():
-    reader = BamIndexedReader(DATA / "bedcov.bam", DATA / "bedcov.bam.bai")
-    df = reader.query("chr1", 12203700, 12205426)
+    assert len(df) == 15
 
-    print(df)
 
-    assert len(df) == 1
+def test_sam_indexed_reader_quer():
+    reader = VCFIndexedReader(DATA / "vcf_file.vcf.gz")
+    df = reader.query("1")
+
+    assert len(df) == 11
```

### Comparing `biobear-0.1.5/src/bam_reader.rs` & `biobear-0.1.6/src/bam_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/src/fasta_reader.rs` & `biobear-0.1.6/src/fasta_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/src/fastq_reader.rs` & `biobear-0.1.6/src/fastq_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/src/gff_reader.rs` & `biobear-0.1.6/src/gff_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/src/lib.rs` & `biobear-0.1.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/src/vcf_reader.rs` & `biobear-0.1.6/src/vcf_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.5/Cargo.lock` & `biobear-0.1.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "biobear"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "arrow",
  "noodles",
  "pyo3",
 ]
 
 [[package]]
```

