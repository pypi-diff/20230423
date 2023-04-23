# Comparing `tmp/k8s_audit_filter-0.0.2-py3-none-any.whl.zip` & `tmp/k8s_audit_filter-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,10 @@
-Zip file size: 17616 bytes, number of entries: 9
--rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 k8s_audit_filter/__about__.py
--rw-r--r--  2.0 unx       64 b- defN 20-Feb-02 00:00 k8s_audit_filter/__init__.py
+Zip file size: 17419 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       81 b- defN 20-Feb-02 00:00 k8s_audit_filter/__init__.py
 -rw-r--r--  2.0 unx     1580 b- defN 20-Feb-02 00:00 k8s_audit_filter/audit_filter.py
 -rw-r--r--  2.0 unx     1512 b- defN 20-Feb-02 00:00 k8s_audit_filter/fields.py
 -rw-r--r--  2.0 unx     1372 b- defN 20-Feb-02 00:00 k8s_audit_filter/rules.py
-?rw-r--r--  2.0 unx     4878 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      761 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.2.dist-info/RECORD
-9 files, 45425 bytes uncompressed, 16296 bytes compressed:  64.1%
+?rw-r--r--  2.0 unx     4878 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      677 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.3.dist-info/RECORD
+8 files, 45336 bytes uncompressed, 16233 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -1,28 +1,25 @@
-Filename: k8s_audit_filter/__about__.py
-Comment: 
-
 Filename: k8s_audit_filter/__init__.py
 Comment: 
 
 Filename: k8s_audit_filter/audit_filter.py
 Comment: 
 
 Filename: k8s_audit_filter/fields.py
 Comment: 
 
 Filename: k8s_audit_filter/rules.py
 Comment: 
 
-Filename: k8s_audit_filter-0.0.2.dist-info/METADATA
+Filename: k8s_audit_filter-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: k8s_audit_filter-0.0.2.dist-info/WHEEL
+Filename: k8s_audit_filter-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: k8s_audit_filter-0.0.2.dist-info/licenses/LICENSE
+Filename: k8s_audit_filter-0.0.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: k8s_audit_filter-0.0.2.dist-info/RECORD
+Filename: k8s_audit_filter-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## k8s_audit_filter/__init__.py

```diff
@@ -1,3 +1,3 @@
-from audit_filter import AuditFilter
+from k8s_audit_filter.audit_filter import AuditFilter
 
 __all__ = ["AuditFilter"]
```

## Comparing `k8s_audit_filter-0.0.2.dist-info/METADATA` & `k8s_audit_filter-0.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s-audit-filter
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to filter k8s audit logs
 Project-URL: Homepage, https://github.com/petrishutin/k8s-audit-filter
 Project-URL: Tracker, https://github.com/petrishutin/k8s-audit-filter/issues
 Author-email: Petr Ishutinr <ishutinpetrdev@gmail.com>
 License-File: LICENSE
 Keywords: audit,filter,k8s
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

## Comparing `k8s_audit_filter-0.0.2.dist-info/licenses/LICENSE` & `k8s_audit_filter-0.0.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

