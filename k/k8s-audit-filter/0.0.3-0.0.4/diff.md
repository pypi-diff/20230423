# Comparing `tmp/k8s_audit_filter-0.0.3-py3-none-any.whl.zip` & `tmp/k8s_audit_filter-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 17419 bytes, number of entries: 8
+Zip file size: 17401 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       81 b- defN 20-Feb-02 00:00 k8s_audit_filter/__init__.py
--rw-r--r--  2.0 unx     1580 b- defN 20-Feb-02 00:00 k8s_audit_filter/audit_filter.py
+-rw-r--r--  2.0 unx     1564 b- defN 20-Feb-02 00:00 k8s_audit_filter/audit_filter.py
 -rw-r--r--  2.0 unx     1512 b- defN 20-Feb-02 00:00 k8s_audit_filter/fields.py
--rw-r--r--  2.0 unx     1372 b- defN 20-Feb-02 00:00 k8s_audit_filter/rules.py
-?rw-r--r--  2.0 unx     4878 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.3.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.3.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      677 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.3.dist-info/RECORD
-8 files, 45336 bytes uncompressed, 16233 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx     1356 b- defN 20-Feb-02 00:00 k8s_audit_filter/rules.py
+?rw-r--r--  2.0 unx     4878 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.4.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.4.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      677 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.4.dist-info/RECORD
+8 files, 45304 bytes uncompressed, 16215 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: k8s_audit_filter/fields.py
 Comment: 
 
 Filename: k8s_audit_filter/rules.py
 Comment: 
 
-Filename: k8s_audit_filter-0.0.3.dist-info/METADATA
+Filename: k8s_audit_filter-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: k8s_audit_filter-0.0.3.dist-info/WHEEL
+Filename: k8s_audit_filter-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: k8s_audit_filter-0.0.3.dist-info/licenses/LICENSE
+Filename: k8s_audit_filter-0.0.4.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: k8s_audit_filter-0.0.3.dist-info/RECORD
+Filename: k8s_audit_filter-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## k8s_audit_filter/audit_filter.py

```diff
@@ -1,12 +1,12 @@
 from typing import Union
 
 import yaml
 
-from k8s_audit_filter.rules import RuleFactory
+from .rules import RuleFactory
 
 
 class AuditFilterException(Exception):
     pass
 
 
 class AuditFilter:
```

## k8s_audit_filter/rules.py

```diff
@@ -1,10 +1,10 @@
 from abc import ABC
 
-from k8s_audit_filter.fields import FieldFactory
+from .fields import FieldFactory
 
 
 class Rule(ABC):
     def __init__(self, fields: dict):
         self.as_dict = fields
         self.fields = FieldFactory.create(fields)
```

## Comparing `k8s_audit_filter-0.0.3.dist-info/METADATA` & `k8s_audit_filter-0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s-audit-filter
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tool to filter k8s audit logs
 Project-URL: Homepage, https://github.com/petrishutin/k8s-audit-filter
 Project-URL: Tracker, https://github.com/petrishutin/k8s-audit-filter/issues
 Author-email: Petr Ishutinr <ishutinpetrdev@gmail.com>
 License-File: LICENSE
 Keywords: audit,filter,k8s
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

## Comparing `k8s_audit_filter-0.0.3.dist-info/licenses/LICENSE` & `k8s_audit_filter-0.0.4.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `k8s_audit_filter-0.0.3.dist-info/RECORD` & `k8s_audit_filter-0.0.4.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 k8s_audit_filter/__init__.py,sha256=Ygyj50ubIBSq7rPmZA5toFWotAC4D3Mc6DzCq_07s2k,81
-k8s_audit_filter/audit_filter.py,sha256=T3sJ0sF2yQV902ZLWdo94fFechLYj061x7paNyM-u7Q,1580
+k8s_audit_filter/audit_filter.py,sha256=Fmq9JLln-LpQ-deHajwYSKB-v0RCOuPgKIBiwEX1scM,1564
 k8s_audit_filter/fields.py,sha256=Lgfj4NJZuqRRfgefu99JNtbmCuDIEN5sw-PBfT80C-I,1512
-k8s_audit_filter/rules.py,sha256=TI-SNBaQS3cvCcgHdzDYVy9gcusrBzHXUJkaPWv4iyQ,1372
-k8s_audit_filter-0.0.3.dist-info/METADATA,sha256=gEmvmlqErjoXNVrDhg3EVnME891eaWQPx98hsg1qFTM,4878
-k8s_audit_filter-0.0.3.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-k8s_audit_filter-0.0.3.dist-info/licenses/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-k8s_audit_filter-0.0.3.dist-info/RECORD,,
+k8s_audit_filter/rules.py,sha256=RpURuZqj0rdEkBj70eNjAKoQxrXeqMHv4IfvlpxyI1s,1356
+k8s_audit_filter-0.0.4.dist-info/METADATA,sha256=tXXKAuS7L5pPHzvmIQnj5bPcb5DYxtde3M64DYMvu8A,4878
+k8s_audit_filter-0.0.4.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+k8s_audit_filter-0.0.4.dist-info/licenses/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+k8s_audit_filter-0.0.4.dist-info/RECORD,,
```

