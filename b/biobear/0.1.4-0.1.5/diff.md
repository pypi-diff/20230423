# Comparing `tmp/biobear-0.1.4.tar.gz` & `tmp/biobear-0.1.5.tar.gz`

## Comparing `biobear-0.1.4.tar` & `biobear-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,37 @@
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 biobear-0.1.4/Cargo.toml
--rw-r--r--   0     1001      123     2663 2023-04-22 21:44:01.000000 biobear-0.1.4/.github/workflows/build-test-release.yml
--rw-r--r--   0     1001      123     4135 2023-04-22 21:44:01.000000 biobear-0.1.4/.gitignore
--rw-r--r--   0     1001      123       68 2023-04-22 21:44:01.000000 biobear-0.1.4/Makefile
--rw-r--r--   0     1001      123     1490 2023-04-22 21:44:01.000000 biobear-0.1.4/README.md
--rw-r--r--   0     1001      123      167 2023-04-22 21:44:01.000000 biobear-0.1.4/cz.json
--rw-r--r--   0     1001      123      421 2023-04-22 21:44:01.000000 biobear-0.1.4/pyproject.toml
--rw-r--r--   0     1001      123      155 2023-04-22 21:44:01.000000 biobear-0.1.4/python/biobear/__init__.py
--rw-r--r--   0     1001      123      889 2023-04-22 21:44:01.000000 biobear-0.1.4/python/biobear/bam_reader.py
--rw-r--r--   0     1001      123      383 2023-04-22 21:44:01.000000 biobear-0.1.4/python/biobear/fasta_reader.py
--rw-r--r--   0     1001      123      383 2023-04-22 21:44:01.000000 biobear-0.1.4/python/biobear/fastq_reader.py
--rw-r--r--   0     1001      123      857 2023-04-22 21:44:01.000000 biobear-0.1.4/python/biobear/vcf_reader.py
--rw-r--r--   0     1001      123      286 2023-04-22 21:44:01.000000 biobear-0.1.4/python/tests/data/test.fastq
--rw-r--r--   0     1001      123      411 2023-04-22 21:44:01.000000 biobear-0.1.4/python/tests/test_fasta_reader.py
--rw-r--r--   0     1001      123      320 2023-04-22 21:44:01.000000 biobear-0.1.4/python/tests/test_fastq_reader.py
--rw-r--r--   0     1001      123       87 2023-04-22 21:44:01.000000 biobear-0.1.4/python/tests/test_version.py
--rw-r--r--   0     1001      123     7737 2023-04-22 21:44:01.000000 biobear-0.1.4/src/bam_reader.rs
--rw-r--r--   0     1001      123     2989 2023-04-22 21:44:01.000000 biobear-0.1.4/src/fasta_reader.rs
--rw-r--r--   0     1001      123     3505 2023-04-22 21:44:01.000000 biobear-0.1.4/src/fastq_reader.rs
--rw-r--r--   0     1001      123     4643 2023-04-22 21:44:01.000000 biobear-0.1.4/src/gff_reader.rs
--rw-r--r--   0     1001      123      526 2023-04-22 21:44:01.000000 biobear-0.1.4/src/lib.rs
--rw-r--r--   0     1001      123     6420 2023-04-22 21:44:01.000000 biobear-0.1.4/src/vcf_reader.rs
--rw-r--r--   0     1001      123    37517 2023-04-22 21:44:46.000000 biobear-0.1.4/Cargo.lock
--rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 biobear-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 biobear-0.1.5/Cargo.toml
+-rw-r--r--   0     1001      123     2663 2023-04-22 22:41:16.000000 biobear-0.1.5/.github/workflows/build-test-release.yml
+-rw-r--r--   0     1001      123     4135 2023-04-22 22:41:16.000000 biobear-0.1.5/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-04-22 22:41:16.000000 biobear-0.1.5/LICENSE
+-rw-r--r--   0     1001      123       68 2023-04-22 22:41:16.000000 biobear-0.1.5/Makefile
+-rw-r--r--   0     1001      123     1520 2023-04-22 22:41:16.000000 biobear-0.1.5/README.md
+-rw-r--r--   0     1001      123      167 2023-04-22 22:41:16.000000 biobear-0.1.5/cz.json
+-rw-r--r--   0     1001      123      421 2023-04-22 22:41:16.000000 biobear-0.1.5/pyproject.toml
+-rw-r--r--   0     1001      123      401 2023-04-22 22:41:16.000000 biobear-0.1.5/python/biobear/__init__.py
+-rw-r--r--   0     1001      123      895 2023-04-22 22:41:16.000000 biobear-0.1.5/python/biobear/bam_reader.py
+-rw-r--r--   0     1001      123      383 2023-04-22 22:41:16.000000 biobear-0.1.5/python/biobear/fasta_reader.py
+-rw-r--r--   0     1001      123      383 2023-04-22 22:41:16.000000 biobear-0.1.5/python/biobear/fastq_reader.py
+-rw-r--r--   0     1001      123      373 2023-04-22 22:41:16.000000 biobear-0.1.5/python/biobear/gff_reader.py
+-rw-r--r--   0     1001      123      838 2023-04-22 22:41:16.000000 biobear-0.1.5/python/biobear/vcf_reader.py
+-rw-r--r--   0     1001      123     6152 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/bedcov.bam
+-rw-r--r--   0     1001      123     7608 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/bedcov.bam.bai
+-rw-r--r--   0     1001      123     1749 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/file.vcf
+-rw-r--r--   0     1001      123     8296 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/index.vcf.gz
+-rw-r--r--   0     1001      123      212 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/index.vcf.gz.tbi
+-rw-r--r--   0     1001      123      286 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/test.fastq
+-rw-r--r--   0     1001      123      112 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/test.gff
+-rw-r--r--   0     1001      123     4302 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/vcf_file.vcf
+-rw-r--r--   0     1001      123     1669 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/vcf_file.vcf.gz
+-rw-r--r--   0     1001      123      254 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/data/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      123      513 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/test_bam_reader.py
+-rw-r--r--   0     1001      123      411 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/test_fasta_reader.py
+-rw-r--r--   0     1001      123      300 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/test_fastq_reader.py
+-rw-r--r--   0     1001      123      295 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/test_gff_reader.py
+-rw-r--r--   0     1001      123      591 2023-04-22 22:41:16.000000 biobear-0.1.5/python/tests/test_vcf_reader.py
+-rw-r--r--   0     1001      123     7737 2023-04-22 22:41:16.000000 biobear-0.1.5/src/bam_reader.rs
+-rw-r--r--   0     1001      123     2989 2023-04-22 22:41:16.000000 biobear-0.1.5/src/fasta_reader.rs
+-rw-r--r--   0     1001      123     3505 2023-04-22 22:41:16.000000 biobear-0.1.5/src/fastq_reader.rs
+-rw-r--r--   0     1001      123     4645 2023-04-22 22:41:16.000000 biobear-0.1.5/src/gff_reader.rs
+-rw-r--r--   0     1001      123      526 2023-04-22 22:41:16.000000 biobear-0.1.5/src/lib.rs
+-rw-r--r--   0     1001      123     6420 2023-04-22 22:41:16.000000 biobear-0.1.5/src/vcf_reader.rs
+-rw-r--r--   0     1001      123    37517 2023-04-22 22:42:15.000000 biobear-0.1.5/Cargo.lock
+-rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 biobear-0.1.5/PKG-INFO
```

### Comparing `biobear-0.1.4/.github/workflows/build-test-release.yml` & `biobear-0.1.5/.github/workflows/build-test-release.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.1.4/.gitignore` & `biobear-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `biobear-0.1.4/README.md` & `biobear-0.1.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -50,8 +50,8 @@
 import biobear as bb
 reader = bb.BamIndexedReader("test.bam", "test.bam.bai")
 reader.query("chr1", 1, 1000).head()
 ```
 
 ## Limitations
 
-Currently, the library reads the entire file (or query result) into memory. If you are working with large files or queries, this may not be ideal.
+Currently, the library reads the entire file (or query result) into memory. This probably isn't a problem unless you're working with very large sequence files or query results.
```

### Comparing `biobear-0.1.4/python/biobear/bam_reader.py` & `biobear-0.1.5/python/biobear/bam_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from pathlib import Path
 
-from .biobear import _BamReader, _BamIndexReader
+from .biobear import _BamReader, _BamIndexedReader
 
 import polars as pl
 
 class BamReader:
     def __init__(self, path: Path):
         self._bam_reader = _BamReader(str(path))
 
     def read(self) -> pl.DataFrame:
         return self.to_polars()
 
     def to_polars(self) -> pl.DataFrame:
         contents = self._bam_reader.read()
         return pl.read_ipc(contents)
 
-class BamIndexReader:
+class BamIndexedReader:
     def __init__(self, path: Path, index: Path):
-        self._bam_reader = _BamIndexReader(str(path), str(index))
+        self._bam_reader = _BamIndexedReader(str(path), str(index))
 
     def read(self) -> pl.DataFrame:
         return self.to_polars()
 
     def query(self, chrom: str, start: int, end: int) -> pl.DataFrame:
         contents = self._bam_reader.query(chrom, start, end)
         return pl.read_ipc(contents)
```

### Comparing `biobear-0.1.4/python/biobear/vcf_reader.py` & `biobear-0.1.5/python/biobear/vcf_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from pathlib import Path
 
-from .biobear import _VcfReader, _VcfIndexReader
+from .biobear import _VCFReader, _VCFIndexedReader
 
 import polars as pl
 
-class VcfReader:
+class VCFReader:
     def __init__(self, path: Path):
-        self._vcf_reader = _VcfReader(str(path))
+        self._vcf_reader = _VCFReader(str(path))
 
     def read(self) -> pl.DataFrame:
         return self.to_polars()
 
     def to_polars(self) -> pl.DataFrame:
         contents = self._vcf_reader.read()
         return pl.read_ipc(contents)
 
-class BamIndexReader:
-    def __init__(self, path: Path, index: Path):
-        self._vcf_reader = _VcfIndexReader(str(path), str(index))
+class VCFIndexedReader:
+    def __init__(self, path: Path):
+        self._vcf_reader = _VCFIndexedReader(str(path))
 
     def read(self) -> pl.DataFrame:
         return self.to_polars()
 
     def query(self, region: str) -> pl.DataFrame:
         contents = self._vcf_reader.query(region)
         return pl.read_ipc(contents)
```

### Comparing `biobear-0.1.4/src/bam_reader.rs` & `biobear-0.1.5/src/bam_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.4/src/fasta_reader.rs` & `biobear-0.1.5/src/fasta_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.4/src/fastq_reader.rs` & `biobear-0.1.5/src/fastq_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.4/src/gff_reader.rs` & `biobear-0.1.5/src/gff_reader.rs`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     fn new() -> Self {
         let file_schema = Schema::new(vec![
             Field::new("seqname", DataType::Utf8, false),
             Field::new("source", DataType::Utf8, true),
             Field::new("feature", DataType::Utf8, false),
             Field::new("start", DataType::Int64, false),
             Field::new("end", DataType::Int64, false),
-            Field::new("score", DataType::Int64, true),
+            Field::new("score", DataType::Float32, true),
             Field::new("strand", DataType::Utf8, false),
             Field::new("phase", DataType::Utf8, true),
             Field::new("attributes", DataType::Utf8, true),
         ]);
 
         Self {
             seqnames: GenericStringBuilder::<i32>::new(),
```

### Comparing `biobear-0.1.4/src/lib.rs` & `biobear-0.1.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.4/src/vcf_reader.rs` & `biobear-0.1.5/src/vcf_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.1.4/Cargo.lock` & `biobear-0.1.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "biobear"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "arrow",
  "noodles",
  "pyo3",
 ]
 
 [[package]]
```

### Comparing `biobear-0.1.4/PKG-INFO` & `biobear-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: biobear
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars>=0.17.0
+License-File: LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # biobear
 
 [![PyPI version](https://badge.fury.io/py/biobear.svg)](https://badge.fury.io/py/biobear)
 
@@ -60,9 +61,9 @@
 import biobear as bb
 reader = bb.BamIndexedReader("test.bam", "test.bam.bai")
 reader.query("chr1", 1, 1000).head()
 ```
 
 ## Limitations
 
-Currently, the library reads the entire file (or query result) into memory. If you are working with large files or queries, this may not be ideal.
+Currently, the library reads the entire file (or query result) into memory. This probably isn't a problem unless you're working with very large sequence files or query results.
```

