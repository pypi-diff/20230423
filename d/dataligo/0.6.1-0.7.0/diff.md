# Comparing `tmp/dataligo-0.6.1.tar.gz` & `tmp/dataligo-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/alchemist/Desktop/OpenSource/dataligo/dist/.tmp-u1pfyily/dataligo-0.6.1.tar", last modified: Sat Apr 15 19:35:56 2023, max compression
+gzip compressed data, was "/home/alchemist/Desktop/OpenSource/dataligo/dist/.tmp-gjxd9htl/dataligo-0.7.0.tar", last modified: Sun Apr 23 15:51:45 2023, max compression
```

## Comparing `dataligo-0.6.1.tar` & `dataligo-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-15 19:35:56.000000 dataligo-0.6.1/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11338 2023-04-15 19:19:37.000000 dataligo-0.6.1/LICENSE
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    18882 2023-04-15 19:35:56.000000 dataligo-0.6.1/PKG-INFO
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     5330 2023-04-15 19:19:37.000000 dataligo-0.6.1/README.md
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-15 19:35:56.000000 dataligo-0.6.1/dataligo.egg-info/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    18882 2023-04-15 19:35:56.000000 dataligo-0.6.1/dataligo.egg-info/PKG-INFO
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      191 2023-04-15 19:35:56.000000 dataligo-0.6.1/dataligo.egg-info/SOURCES.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        1 2023-04-15 19:35:56.000000 dataligo-0.6.1/dataligo.egg-info/dependency_links.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      334 2023-04-15 19:35:56.000000 dataligo-0.6.1/dataligo.egg-info/requires.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        9 2023-04-15 19:35:56.000000 dataligo-0.6.1/dataligo.egg-info/top_level.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1687 2023-04-15 19:34:51.000000 dataligo-0.6.1/pyproject.toml
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       38 2023-04-15 19:35:56.000000 dataligo-0.6.1/setup.cfg
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-23 15:51:45.000000 dataligo-0.7.0/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11338 2023-04-15 19:19:37.000000 dataligo-0.7.0/LICENSE
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    19511 2023-04-23 15:51:45.000000 dataligo-0.7.0/PKG-INFO
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     5936 2023-04-23 15:20:00.000000 dataligo-0.7.0/README.md
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-23 15:51:45.000000 dataligo-0.7.0/dataligo.egg-info/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    19511 2023-04-23 15:51:45.000000 dataligo-0.7.0/dataligo.egg-info/PKG-INFO
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      191 2023-04-23 15:51:45.000000 dataligo-0.7.0/dataligo.egg-info/SOURCES.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        1 2023-04-23 15:51:45.000000 dataligo-0.7.0/dataligo.egg-info/dependency_links.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      358 2023-04-23 15:51:45.000000 dataligo-0.7.0/dataligo.egg-info/requires.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        9 2023-04-23 15:51:45.000000 dataligo-0.7.0/dataligo.egg-info/top_level.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1714 2023-04-23 15:51:16.000000 dataligo-0.7.0/pyproject.toml
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       38 2023-04-23 15:51:45.000000 dataligo-0.7.0/setup.cfg
```

### Comparing `dataligo-0.6.1/LICENSE` & `dataligo-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataligo-0.6.1/PKG-INFO` & `dataligo-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataligo
-Version: 0.6.1
+Version: 0.7.0
 Summary: A library to accelerate ML and ETL pipeline by connecting all data sources
 Author-email: Vinish M <vinishuchiha@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -208,14 +208,15 @@
 Project-URL: Homepage, https://github.com/VinishUchiha/dataligo
 Keywords: connectors,datalake reader,datawarehouse reader,dataconnector,nosql connector
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: polars
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # DataLigo
 
@@ -238,18 +239,34 @@
 ## Quick tour
 ```python
 >>> from dataligo import Ligo
 >>> from transformers import pipeline
 
 >>> ligo = Ligo('./ligo_config.yaml') # Check the sample_ligo_config.yaml for reference
 >>> print(ligo.get_supported_data_sources_list())
-['s3', 'gcs', 'azureblob', 'bigquery', 'snowflake', 'redshift', 'starrocks', 'postgresql', 'mysql', 'oracle', 'mssql', 'mariadb', 'sqlite', 'elasticsearch', 'mongodb']
+['s3',
+ 'gcs',
+ 'azureblob',
+ 'bigquery',
+ 'snowflake',
+ 'redshift',
+ 'starrocks',
+ 'postgresql',
+ 'mysql',
+ 'oracle',
+ 'mssql',
+ 'mariadb',
+ 'sqlite',
+ 'elasticsearch',
+ 'mongodb',
+ 'dynamodb',
+ 'redis']
 
 >>> mongodb = ligo.connect('mongodb')
->>> df = mongodb.read_as_dataframe(database='reviewdb',collection='reviews')
+>>> df = mongodb.read_as_dataframe(database='reviewdb',collection='reviews',return_type='pandas') # Default return_type is pandas
 >>> df.head()
         _id	                        Review
 0	64272bb06a14f52787e0a09e	good and interesting
 1	64272bb06a14f52787e0a09f	This class is very helpful to me. Currently, I...
 2	64272bb06a14f52787e0a0a0	like!Prof and TAs are helpful and the discussi...
 3	64272bb06a14f52787e0a0a1	Easy to follow and includes a lot basic and im...
 4	64272bb06a14f52787e0a0a2	Really nice teacher!I could got the point eazl...
@@ -267,39 +284,52 @@
 
 >>> df['predicted_label'] = [result['label'] for result in results]
 >>> df['predicted_score'] = [round(result['score'], 4) for result in results]
 
 # Write the results to the MongoDB
 >>> mongodb.write_dataframe(df,'reviewdb','review_sentiments')
 ```
+
+## Example DataLigo Pipeline
+
+## ETL Pipeline
+<p align="center"><img alt="dataligo ETL pipeline diagram" src="https://github.com/VinishUchiha/dataligo/blob/main/docs/images/DataLigo_ETL_pipeline.jpg"/></p>
+
+## ML Pipeline
+<p align="center"><img alt="dataligo ML pipeline diagram" src="https://github.com/VinishUchiha/dataligo/blob/main/docs/images/DataLigo_ML_pipeline.jpg"/></p>
+
 ## Supported Connectors
 
         
  |Data Sources| Type | pandas | polars | dask |
 |------------|------| ----  | -----| ----- |
-|S3|datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|GCS|datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|Azure Blob Stoarge| datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|Snowflake| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|BigQuery| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|StarRocks| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|Redshift| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|PostgreSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|MySQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|MariaDB| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|MsSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|Oracle| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|SQLite| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|MongoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|ElasticSearch| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|DynamoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|Redis| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|S3|datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|GCS|datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|Azure Blob Storage| datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|Snowflake| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|BigQuery| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|StarRocks| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|Redshift| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|PostgreSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|MySQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|MariaDB| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|MsSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|Oracle| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|SQLite| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|MongoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|ElasticSearch| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|DynamoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|Redis| nosql | <ul><li>[x] read</li><li>[ ] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
 
 
 ## Acknowledgement
 
 Some functionalities of DataLigo are inspired by the following packages.
 
 - [ConnectorX](https://github.com/sfu-db/connector-x)
   
   DataLigo used Connectorx to read data from most of the RDBMS databases to utilize the performance benefits and inspired the return_type parameter from it
   
+- [dynamo-pandas](https://github.com/DrGFreeman/dynamo-pandas)
+
+  DataLigo used dynamo-pandas to read and write data from DynamoDB
+
```

### Comparing `dataligo-0.6.1/README.md` & `dataligo-0.7.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -21,18 +21,34 @@
 ## Quick tour
 ```python
 >>> from dataligo import Ligo
 >>> from transformers import pipeline
 
 >>> ligo = Ligo('./ligo_config.yaml') # Check the sample_ligo_config.yaml for reference
 >>> print(ligo.get_supported_data_sources_list())
-['s3', 'gcs', 'azureblob', 'bigquery', 'snowflake', 'redshift', 'starrocks', 'postgresql', 'mysql', 'oracle', 'mssql', 'mariadb', 'sqlite', 'elasticsearch', 'mongodb']
+['s3',
+ 'gcs',
+ 'azureblob',
+ 'bigquery',
+ 'snowflake',
+ 'redshift',
+ 'starrocks',
+ 'postgresql',
+ 'mysql',
+ 'oracle',
+ 'mssql',
+ 'mariadb',
+ 'sqlite',
+ 'elasticsearch',
+ 'mongodb',
+ 'dynamodb',
+ 'redis']
 
 >>> mongodb = ligo.connect('mongodb')
->>> df = mongodb.read_as_dataframe(database='reviewdb',collection='reviews')
+>>> df = mongodb.read_as_dataframe(database='reviewdb',collection='reviews',return_type='pandas') # Default return_type is pandas
 >>> df.head()
         _id	                        Review
 0	64272bb06a14f52787e0a09e	good and interesting
 1	64272bb06a14f52787e0a09f	This class is very helpful to me. Currently, I...
 2	64272bb06a14f52787e0a0a0	like!Prof and TAs are helpful and the discussi...
 3	64272bb06a14f52787e0a0a1	Easy to follow and includes a lot basic and im...
 4	64272bb06a14f52787e0a0a2	Really nice teacher!I could got the point eazl...
@@ -50,39 +66,52 @@
 
 >>> df['predicted_label'] = [result['label'] for result in results]
 >>> df['predicted_score'] = [round(result['score'], 4) for result in results]
 
 # Write the results to the MongoDB
 >>> mongodb.write_dataframe(df,'reviewdb','review_sentiments')
 ```
+
+## Example DataLigo Pipeline
+
+## ETL Pipeline
+<p align="center"><img alt="dataligo ETL pipeline diagram" src="https://github.com/VinishUchiha/dataligo/blob/main/docs/images/DataLigo_ETL_pipeline.jpg"/></p>
+
+## ML Pipeline
+<p align="center"><img alt="dataligo ML pipeline diagram" src="https://github.com/VinishUchiha/dataligo/blob/main/docs/images/DataLigo_ML_pipeline.jpg"/></p>
+
 ## Supported Connectors
 
         
  |Data Sources| Type | pandas | polars | dask |
 |------------|------| ----  | -----| ----- |
-|S3|datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|GCS|datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|Azure Blob Stoarge| datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|Snowflake| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|BigQuery| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|StarRocks| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|Redshift| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|PostgreSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|MySQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|MariaDB| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|MsSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|Oracle| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|SQLite| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|MongoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|ElasticSearch| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|DynamoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|Redis| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|S3|datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|GCS|datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|Azure Blob Storage| datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|Snowflake| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|BigQuery| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|StarRocks| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|Redshift| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|PostgreSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|MySQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|MariaDB| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|MsSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|Oracle| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|SQLite| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|MongoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|ElasticSearch| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|DynamoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|Redis| nosql | <ul><li>[x] read</li><li>[ ] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
 
 
 ## Acknowledgement
 
 Some functionalities of DataLigo are inspired by the following packages.
 
 - [ConnectorX](https://github.com/sfu-db/connector-x)
   
   DataLigo used Connectorx to read data from most of the RDBMS databases to utilize the performance benefits and inspired the return_type parameter from it
   
+- [dynamo-pandas](https://github.com/DrGFreeman/dynamo-pandas)
+
+  DataLigo used dynamo-pandas to read and write data from DynamoDB
+
```

### Comparing `dataligo-0.6.1/dataligo.egg-info/PKG-INFO` & `dataligo-0.7.0/dataligo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataligo
-Version: 0.6.1
+Version: 0.7.0
 Summary: A library to accelerate ML and ETL pipeline by connecting all data sources
 Author-email: Vinish M <vinishuchiha@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -208,14 +208,15 @@
 Project-URL: Homepage, https://github.com/VinishUchiha/dataligo
 Keywords: connectors,datalake reader,datawarehouse reader,dataconnector,nosql connector
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: polars
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # DataLigo
 
@@ -238,18 +239,34 @@
 ## Quick tour
 ```python
 >>> from dataligo import Ligo
 >>> from transformers import pipeline
 
 >>> ligo = Ligo('./ligo_config.yaml') # Check the sample_ligo_config.yaml for reference
 >>> print(ligo.get_supported_data_sources_list())
-['s3', 'gcs', 'azureblob', 'bigquery', 'snowflake', 'redshift', 'starrocks', 'postgresql', 'mysql', 'oracle', 'mssql', 'mariadb', 'sqlite', 'elasticsearch', 'mongodb']
+['s3',
+ 'gcs',
+ 'azureblob',
+ 'bigquery',
+ 'snowflake',
+ 'redshift',
+ 'starrocks',
+ 'postgresql',
+ 'mysql',
+ 'oracle',
+ 'mssql',
+ 'mariadb',
+ 'sqlite',
+ 'elasticsearch',
+ 'mongodb',
+ 'dynamodb',
+ 'redis']
 
 >>> mongodb = ligo.connect('mongodb')
->>> df = mongodb.read_as_dataframe(database='reviewdb',collection='reviews')
+>>> df = mongodb.read_as_dataframe(database='reviewdb',collection='reviews',return_type='pandas') # Default return_type is pandas
 >>> df.head()
         _id	                        Review
 0	64272bb06a14f52787e0a09e	good and interesting
 1	64272bb06a14f52787e0a09f	This class is very helpful to me. Currently, I...
 2	64272bb06a14f52787e0a0a0	like!Prof and TAs are helpful and the discussi...
 3	64272bb06a14f52787e0a0a1	Easy to follow and includes a lot basic and im...
 4	64272bb06a14f52787e0a0a2	Really nice teacher!I could got the point eazl...
@@ -267,39 +284,52 @@
 
 >>> df['predicted_label'] = [result['label'] for result in results]
 >>> df['predicted_score'] = [round(result['score'], 4) for result in results]
 
 # Write the results to the MongoDB
 >>> mongodb.write_dataframe(df,'reviewdb','review_sentiments')
 ```
+
+## Example DataLigo Pipeline
+
+## ETL Pipeline
+<p align="center"><img alt="dataligo ETL pipeline diagram" src="https://github.com/VinishUchiha/dataligo/blob/main/docs/images/DataLigo_ETL_pipeline.jpg"/></p>
+
+## ML Pipeline
+<p align="center"><img alt="dataligo ML pipeline diagram" src="https://github.com/VinishUchiha/dataligo/blob/main/docs/images/DataLigo_ML_pipeline.jpg"/></p>
+
 ## Supported Connectors
 
         
  |Data Sources| Type | pandas | polars | dask |
 |------------|------| ----  | -----| ----- |
-|S3|datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|GCS|datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|Azure Blob Stoarge| datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|Snowflake| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|BigQuery| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|StarRocks| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|Redshift| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|PostgreSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|MySQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|MariaDB| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|MsSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|Oracle| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|SQLite| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[ ] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
-|MongoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|ElasticSearch| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|DynamoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|Redis| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|S3|datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|GCS|datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|Azure Blob Storage| datalake| <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|Snowflake| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|BigQuery| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|StarRocks| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|Redshift| datawarehouse | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|PostgreSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|MySQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|MariaDB| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|MsSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|Oracle| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|SQLite| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
+|MongoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|ElasticSearch| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|DynamoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|Redis| nosql | <ul><li>[x] read</li><li>[ ] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
 
 
 ## Acknowledgement
 
 Some functionalities of DataLigo are inspired by the following packages.
 
 - [ConnectorX](https://github.com/sfu-db/connector-x)
   
   DataLigo used Connectorx to read data from most of the RDBMS databases to utilize the performance benefits and inspired the return_type parameter from it
   
+- [dynamo-pandas](https://github.com/DrGFreeman/dynamo-pandas)
+
+  DataLigo used dynamo-pandas to read and write data from DynamoDB
+
```

### Comparing `dataligo-0.6.1/pyproject.toml` & `dataligo-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataligo"
-version = "0.6.1"
+version = "0.7.0"
 description = "A library to accelerate ML and ETL pipeline by connecting all data sources"
 readme = "README.md"
 authors = [{ name = "Vinish M", email = "vinishuchiha@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -18,39 +18,40 @@
 dependencies = [
     "boto3 >= 1.26.93",
     "google-cloud-storage >= 2.7.0",
     "azure-storage-blob >= 12.15.0",
     "pandas >= 1.0.0",
     "PyYAML",
     "connectorx",
-    "snowflake-connector-python[pandas]",
+    "snowflake-connector-python[pandas]==3.0.2",
     "mysql-connector-python-rf",
     "elasticsearch > 8.0.0",
     "sqlalchemy==1.4.46",
     "pymongo",
     "dynamo_pandas",
     "fastparquet",
     "openpyxl",
     "xlrd",
     "xlwt",
     'tomli; python_version < "3.11"',
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
+polars = ["polars"]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/VinishUchiha/dataligo"
 
 [tool.setuptools]
 py-modules = ["dataligo"]
 
 [tool.bumpver]
-current_version = "0.6.1"
+current_version = "0.7.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

