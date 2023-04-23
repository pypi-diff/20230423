# Comparing `tmp/dbxconfig-2.1.1.tar.gz` & `tmp/dbxconfig-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-2.1.1.tar", last modified: Sat Apr 22 18:33:24 2023, max compression
+gzip compressed data, was "dbxconfig-2.2.0.tar", last modified: Sun Apr 23 07:03:53 2023, max compression
```

## Comparing `dbxconfig-2.1.1.tar` & `dbxconfig-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 18:33:24.084141 dbxconfig-2.1.1/
--rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-22 18:33:24.084141 dbxconfig-2.1.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2936 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 18:33:24.080141 dbxconfig-2.1.1/dbxconfig/
--rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/dbxconfig/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2848 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/dbxconfig/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/dbxconfig/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1206 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/dbxconfig/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3513 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/dbxconfig/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/dbxconfig/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1979 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/dbxconfig/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 18:33:24.084141 dbxconfig-2.1.1/dbxconfig/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/dbxconfig/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      903 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/dbxconfig/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3314 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/dbxconfig/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3115 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/dbxconfig/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4982 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/dbxconfig/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/dbxconfig/dataset/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 18:33:24.084141 dbxconfig-2.1.1/dbxconfig.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-22 18:33:24.000000 dbxconfig-2.1.1/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      544 2023-04-22 18:33:24.000000 dbxconfig-2.1.1/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-22 18:33:24.000000 dbxconfig-2.1.1/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-22 18:33:24.000000 dbxconfig-2.1.1/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       31 2023-04-22 18:33:24.000000 dbxconfig-2.1.1/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-22 18:33:24.000000 dbxconfig-2.1.1/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-22 18:33:24.084141 dbxconfig-2.1.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1103 2023-04-22 18:32:29.000000 dbxconfig-2.1.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 07:03:53.833813 dbxconfig-2.2.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3710 2023-04-23 07:03:53.833813 dbxconfig-2.2.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     3158 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 07:03:53.833813 dbxconfig-2.2.0/dbxconfig/
+-rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/dbxconfig/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2848 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/dbxconfig/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/dbxconfig/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1204 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/dbxconfig/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3513 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/dbxconfig/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/dbxconfig/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1979 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/dbxconfig/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 07:03:53.833813 dbxconfig-2.2.0/dbxconfig/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/dbxconfig/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      903 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/dbxconfig/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3314 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/dbxconfig/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3115 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/dbxconfig/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4982 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/dbxconfig/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/dbxconfig/dataset/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 07:03:53.833813 dbxconfig-2.2.0/dbxconfig.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3710 2023-04-23 07:03:53.000000 dbxconfig-2.2.0/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      544 2023-04-23 07:03:53.000000 dbxconfig-2.2.0/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-23 07:03:53.000000 dbxconfig-2.2.0/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-23 07:03:53.000000 dbxconfig-2.2.0/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       31 2023-04-23 07:03:53.000000 dbxconfig-2.2.0/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-23 07:03:53.000000 dbxconfig-2.2.0/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-23 07:03:53.833813 dbxconfig-2.2.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1103 2023-04-23 07:02:56.000000 dbxconfig-2.2.0/setup.py
```

### Comparing `dbxconfig-2.1.1/PKG-INFO` & `dbxconfig-2.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 2.1.1
+Version: 2.2.0
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
@@ -29,14 +29,24 @@
 raw:
   raw_dbx_patterns:
     customers:
       ids: id
       depends_on:
         - landing.landing_dbx_patterns.customer_details_1
         - landing.landing_dbx_patterns.customer_details_2
+      warning_thresholds:
+        invalid_ratio: 0.1
+        invalid_rows: 0
+        max_rows: 100
+        min_rows: 5
+      exception_thresholds:
+        invalid_ratio: 0.2
+        invalid_rows: 2
+        max_rows: 1000
+        min_rows: 0
 
 base:
   base_dbx_patterns:
     customer_details_1:
       ids: id
       depends_on:
         - raw.raw_dbx_patterns.customers
@@ -45,32 +55,32 @@
       depends_on:
         - raw.raw_dbx_patterns.customers
 ```
 
 Define you load configuration:
 
 ```yaml
-tables: ./test/Config/tables.yaml
+tables: ./tables.yaml
 
 landing:
   trigger: customerdetailscomplete-{{filename_date_format}}*.flg
   trigger_type: file
   database: landing_dbx_patterns
   table: "{{table}}"
   container: datalake
   root: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
   filename: "{{table}}-{{filename_date_format}}*.csv"
   filename_date_format: "%Y%m%d"
   path_date_format: "%Y%m%d"
   format: cloudFiles
-  spark_schema: ./test/Schema/{{table.lower()}}.yaml
+  spark_schema: ../Schema/{{table.lower()}}.yaml
   options:
     # autoloader
     cloudFiles.format: csv
-    cloudFiles.schemaLocation:  /mnt/{{container}}/checkpoint/{{checkpoint}}
+    cloudFiles.schemaLocation:  "/mnt/{{container}}/checkpoint/{{checkpoint}}"
     cloudFiles.useIncrementalListing: auto
     # schema
     inferSchema: false
     enforceSchema: true
     columnNameOfCorruptRecord: _corrupt_record
     # csv
     header: false
@@ -85,40 +95,42 @@
 
 raw:
   database: raw_dbx_patterns
   table: "{{table}}"
   container: datalake
   root: /mnt/{{container}}/data/raw
   path: "{{database}}/{{table}}"
+  checkpoint_location: /mnt/{{container}}/checkpoint/{{checkpoint}}
   options:
-    checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
     mergeSchema: true
 ```
 
 Import the config objects into you pipeline:
 
 ```python
 from dbxconfig import Config, Timeslice, StageType
 
 # build path to configuration file
 pattern = "auto_load_schema"
-config_path = f"./Config/{pattern}.yaml"
+config_path = f"../Config"
 
 # create a timeslice object for slice loading. Use * for all time (supports hrs, mins, seconds and sub-second).
 timeslice = Timeslice(day="*", month="*", year="*")
 
 # parse and create a config objects
-config = Config(timeslice=timeslice, config_path=config_path)
+config = Config(config_path=config_path, pattern=pattern)
 
 # get the configuration for a table mapping to load.
 table_mapping = config.get_table_mapping(
     timeslice=timeslice, 
     stage=StageType.raw, 
     table="customers"
 )
+
+print(table_mapping)
 ```
 
 ## Development Setup
 
 ```
 pip install -r requirements.txt
 ```
```

### Comparing `dbxconfig-2.1.1/README.md` & `dbxconfig-2.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,24 @@
 raw:
   raw_dbx_patterns:
     customers:
       ids: id
       depends_on:
         - landing.landing_dbx_patterns.customer_details_1
         - landing.landing_dbx_patterns.customer_details_2
+      warning_thresholds:
+        invalid_ratio: 0.1
+        invalid_rows: 0
+        max_rows: 100
+        min_rows: 5
+      exception_thresholds:
+        invalid_ratio: 0.2
+        invalid_rows: 2
+        max_rows: 1000
+        min_rows: 0
 
 base:
   base_dbx_patterns:
     customer_details_1:
       ids: id
       depends_on:
         - raw.raw_dbx_patterns.customers
@@ -30,32 +40,32 @@
       depends_on:
         - raw.raw_dbx_patterns.customers
 ```
 
 Define you load configuration:
 
 ```yaml
-tables: ./test/Config/tables.yaml
+tables: ./tables.yaml
 
 landing:
   trigger: customerdetailscomplete-{{filename_date_format}}*.flg
   trigger_type: file
   database: landing_dbx_patterns
   table: "{{table}}"
   container: datalake
   root: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
   filename: "{{table}}-{{filename_date_format}}*.csv"
   filename_date_format: "%Y%m%d"
   path_date_format: "%Y%m%d"
   format: cloudFiles
-  spark_schema: ./test/Schema/{{table.lower()}}.yaml
+  spark_schema: ../Schema/{{table.lower()}}.yaml
   options:
     # autoloader
     cloudFiles.format: csv
-    cloudFiles.schemaLocation:  /mnt/{{container}}/checkpoint/{{checkpoint}}
+    cloudFiles.schemaLocation:  "/mnt/{{container}}/checkpoint/{{checkpoint}}"
     cloudFiles.useIncrementalListing: auto
     # schema
     inferSchema: false
     enforceSchema: true
     columnNameOfCorruptRecord: _corrupt_record
     # csv
     header: false
@@ -70,40 +80,42 @@
 
 raw:
   database: raw_dbx_patterns
   table: "{{table}}"
   container: datalake
   root: /mnt/{{container}}/data/raw
   path: "{{database}}/{{table}}"
+  checkpoint_location: /mnt/{{container}}/checkpoint/{{checkpoint}}
   options:
-    checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
     mergeSchema: true
 ```
 
 Import the config objects into you pipeline:
 
 ```python
 from dbxconfig import Config, Timeslice, StageType
 
 # build path to configuration file
 pattern = "auto_load_schema"
-config_path = f"./Config/{pattern}.yaml"
+config_path = f"../Config"
 
 # create a timeslice object for slice loading. Use * for all time (supports hrs, mins, seconds and sub-second).
 timeslice = Timeslice(day="*", month="*", year="*")
 
 # parse and create a config objects
-config = Config(timeslice=timeslice, config_path=config_path)
+config = Config(config_path=config_path, pattern=pattern)
 
 # get the configuration for a table mapping to load.
 table_mapping = config.get_table_mapping(
     timeslice=timeslice, 
     stage=StageType.raw, 
     table="customers"
 )
+
+print(table_mapping)
 ```
 
 ## Development Setup
 
 ```
 pip install -r requirements.txt
 ```
```

### Comparing `dbxconfig-2.1.1/dbxconfig/_config.py` & `dbxconfig-2.2.0/dbxconfig/_config.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.1.1/dbxconfig/_table.py` & `dbxconfig-2.2.0/dbxconfig/_table.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class ValidationThreshold(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     invalid_ratio: float = Field(default=None)
-    invalid_rows: float = Field(default=None)
+    invalid_rows: int = Field(default=None)
     max_rows: int = Field(default=None)
     min_rows: int = Field(default=None)
 
 
 class BaseTable(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
```

### Comparing `dbxconfig-2.1.1/dbxconfig/_tables.py` & `dbxconfig-2.2.0/dbxconfig/_tables.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.1.1/dbxconfig/_timeslice.py` & `dbxconfig-2.2.0/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.1.1/dbxconfig/_utils.py` & `dbxconfig-2.2.0/dbxconfig/_utils.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.1.1/dbxconfig/dataset/_dataset.py` & `dbxconfig-2.2.0/dbxconfig/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.1.1/dbxconfig/dataset/_deltalake.py` & `dbxconfig-2.2.0/dbxconfig/dataset/_deltalake.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.1.1/dbxconfig/dataset/_factory.py` & `dbxconfig-2.2.0/dbxconfig/dataset/_factory.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.1.1/dbxconfig/dataset/_read.py` & `dbxconfig-2.2.0/dbxconfig/dataset/_read.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.1.1/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-2.2.0/dbxconfig.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 2.1.1
+Version: 2.2.0
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
@@ -29,14 +29,24 @@
 raw:
   raw_dbx_patterns:
     customers:
       ids: id
       depends_on:
         - landing.landing_dbx_patterns.customer_details_1
         - landing.landing_dbx_patterns.customer_details_2
+      warning_thresholds:
+        invalid_ratio: 0.1
+        invalid_rows: 0
+        max_rows: 100
+        min_rows: 5
+      exception_thresholds:
+        invalid_ratio: 0.2
+        invalid_rows: 2
+        max_rows: 1000
+        min_rows: 0
 
 base:
   base_dbx_patterns:
     customer_details_1:
       ids: id
       depends_on:
         - raw.raw_dbx_patterns.customers
@@ -45,32 +55,32 @@
       depends_on:
         - raw.raw_dbx_patterns.customers
 ```
 
 Define you load configuration:
 
 ```yaml
-tables: ./test/Config/tables.yaml
+tables: ./tables.yaml
 
 landing:
   trigger: customerdetailscomplete-{{filename_date_format}}*.flg
   trigger_type: file
   database: landing_dbx_patterns
   table: "{{table}}"
   container: datalake
   root: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
   filename: "{{table}}-{{filename_date_format}}*.csv"
   filename_date_format: "%Y%m%d"
   path_date_format: "%Y%m%d"
   format: cloudFiles
-  spark_schema: ./test/Schema/{{table.lower()}}.yaml
+  spark_schema: ../Schema/{{table.lower()}}.yaml
   options:
     # autoloader
     cloudFiles.format: csv
-    cloudFiles.schemaLocation:  /mnt/{{container}}/checkpoint/{{checkpoint}}
+    cloudFiles.schemaLocation:  "/mnt/{{container}}/checkpoint/{{checkpoint}}"
     cloudFiles.useIncrementalListing: auto
     # schema
     inferSchema: false
     enforceSchema: true
     columnNameOfCorruptRecord: _corrupt_record
     # csv
     header: false
@@ -85,40 +95,42 @@
 
 raw:
   database: raw_dbx_patterns
   table: "{{table}}"
   container: datalake
   root: /mnt/{{container}}/data/raw
   path: "{{database}}/{{table}}"
+  checkpoint_location: /mnt/{{container}}/checkpoint/{{checkpoint}}
   options:
-    checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
     mergeSchema: true
 ```
 
 Import the config objects into you pipeline:
 
 ```python
 from dbxconfig import Config, Timeslice, StageType
 
 # build path to configuration file
 pattern = "auto_load_schema"
-config_path = f"./Config/{pattern}.yaml"
+config_path = f"../Config"
 
 # create a timeslice object for slice loading. Use * for all time (supports hrs, mins, seconds and sub-second).
 timeslice = Timeslice(day="*", month="*", year="*")
 
 # parse and create a config objects
-config = Config(timeslice=timeslice, config_path=config_path)
+config = Config(config_path=config_path, pattern=pattern)
 
 # get the configuration for a table mapping to load.
 table_mapping = config.get_table_mapping(
     timeslice=timeslice, 
     stage=StageType.raw, 
     table="customers"
 )
+
+print(table_mapping)
 ```
 
 ## Development Setup
 
 ```
 pip install -r requirements.txt
 ```
```

### Comparing `dbxconfig-2.1.1/dbxconfig.egg-info/SOURCES.txt` & `dbxconfig-2.2.0/dbxconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.1.1/setup.py` & `dbxconfig-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="2.1.1",
+    version="2.2.0",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

