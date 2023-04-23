# Comparing `tmp/mindsdb_text_to_sql-0.1.0.tar.gz` & `tmp/mindsdb_text_to_sql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mindsdb_text_to_sql-0.1.0.tar", last modified: Fri Apr 21 17:55:18 2023, max compression
+gzip compressed data, was "dist\mindsdb_text_to_sql-0.1.1.tar", last modified: Sun Apr 23 16:18:04 2023, max compression
```

## Comparing `mindsdb_text_to_sql-0.1.0.tar` & `mindsdb_text_to_sql-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 17:55:18.000000 mindsdb_text_to_sql-0.1.0/
--rw-rw-rw-   0        0        0     1572 2023-04-21 17:55:18.000000 mindsdb_text_to_sql-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      854 2023-04-21 17:53:35.000000 mindsdb_text_to_sql-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 17:55:18.000000 mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql/
--rw-rw-rw-   0        0        0      431 2023-04-21 17:53:35.000000 mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql/__about__.py
--rw-rw-rw-   0        0        0       41 2023-04-21 17:53:35.000000 mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:55:18.000000 mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql/config/
--rw-rw-rw-   0        0        0     2713 2023-04-21 17:53:35.000000 mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql/config/examples.json
--rw-rw-rw-   0        0        0     5136 2023-04-21 17:53:35.000000 mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql/gpt.py
--rw-rw-rw-   0        0        0      785 2023-04-21 17:53:35.000000 mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql/gpt_text_to_sql.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:55:18.000000 mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql.egg-info/
--rw-rw-rw-   0        0        0     1572 2023-04-21 17:55:18.000000 mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-04-21 17:55:18.000000 mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 17:55:18.000000 mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-21 17:55:18.000000 mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-21 17:55:18.000000 mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 17:55:18.000000 mindsdb_text_to_sql-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1007 2023-04-21 17:53:35.000000 mindsdb_text_to_sql-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:18:04.000000 mindsdb_text_to_sql-0.1.1/
+-rw-rw-rw-   0        0        0     1572 2023-04-23 16:18:04.000000 mindsdb_text_to_sql-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2023-04-23 16:17:45.000000 mindsdb_text_to_sql-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 16:18:04.000000 mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql/
+-rw-rw-rw-   0        0        0      431 2023-04-23 16:17:45.000000 mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql/__about__.py
+-rw-rw-rw-   0        0        0       41 2023-04-23 16:17:45.000000 mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:18:04.000000 mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql/config/
+-rw-rw-rw-   0        0        0     3259 2023-04-23 16:17:45.000000 mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql/config/examples.json
+-rw-rw-rw-   0        0        0     5136 2023-04-23 16:17:45.000000 mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql/gpt.py
+-rw-rw-rw-   0        0        0      785 2023-04-23 16:17:45.000000 mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql/gpt_text_to_sql.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:18:04.000000 mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql.egg-info/
+-rw-rw-rw-   0        0        0     1572 2023-04-23 16:18:04.000000 mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-04-23 16:18:04.000000 mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 16:18:04.000000 mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-23 16:18:04.000000 mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-23 16:18:04.000000 mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 16:18:04.000000 mindsdb_text_to_sql-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1007 2023-04-23 16:17:45.000000 mindsdb_text_to_sql-0.1.1/setup.py
```

### Comparing `mindsdb_text_to_sql-0.1.0/PKG-INFO` & `mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mindsdb_text_to_sql
-Version: 0.1.0
+Name: mindsdb-text-to-sql
+Version: 0.1.1
 Summary: MindsDB Text to SQL, converts natural language to SQL code.
 Home-page: https://github.com/MinuraPunchihewa/mindsdb-text-to-sql
 Author: Minura Punchihewa
 Author-email: minurapunchihewa17@gmail.com
 License: UNKNOWN
 Download-URL: https://pypi.org/project/mindsdb-text-to-sql/
 Description: # MindsDB Text to SQL
```

### Comparing `mindsdb_text_to_sql-0.1.0/README.md` & `mindsdb_text_to_sql-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql/config/examples.json` & `mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql/config/examples.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5625%*

 * *Differences: {"'create_ml_engine'": "{0: {'Create a engine called openai2 using api key abc1234567': 'CREATE "*

 * *                       'ML_ENGINE openai2\\nFROM openai USING\\n  api_key = "abc1234567";\'}}',*

 * * "'create_model'": '{0: {"Create a model called mindsdb.sentiment_classifier using the openai2 '*

 * *                   "engine to predict sentiment using prompt template 'predict the sentiment of "*

 * *                   'the text:{{review}} exactly as either positive or negative or neutral\'": '*

 * *                   '"CREATE […]*

```diff
@@ -10,25 +10,33 @@
         },
         {
             "Create a connection called sqlite_datasource to the sqlite database at example.db": "CREATE DATABASE sqlite_datasource\nWITH ENGINE = 'sqlite',\nPARAMETERS = {\n  \"database\": \"example.db\"\n};"
         }
     ],
     "create_ml_engine": [
         {
-            "Create a engine called openai2 using api key abc1234567": "CREATE ML_ENGINE openai2\nFROM openai USING\n  \"api_key\": \"abc1234567\"\n};"
+            "Create a engine called openai2 using api key abc1234567": "CREATE ML_ENGINE openai2\nFROM openai USING\n  api_key = \"abc1234567\";"
         }
     ],
     "create_model": [
         {
-            "Create a model called mindsdb.sentiment_classifier using the openai2 engine to predict sentiment using prompt template 'predict the sentiment of the text:{{review}} exactly as either positive or negative or neutral'": "CREATE MODEL mindsdb.sentiment_classifier\nPREDICT sentiment\nUSING\n  engine = 'openai2',\n  prompt_template = 'predict the sentiment of the text:{{review}} exactly as either positive or negative or neutral';\n"
+            "Create a model called mindsdb.sentiment_classifier using the openai2 engine to predict sentiment using prompt template 'predict the sentiment of the text:{{review}} exactly as either positive or negative or neutral'": "CREATE MODEL mindsdb.sentiment_classifier\nPREDICT sentiment\nUSING\n  engine = 'openai2',\n  prompt_template = 'predict the sentiment of the text:{{review}} exactly as either positive or negative or neutral';"
         }
     ],
-    "predict": [
+    "predict_bulk": [
         {
-            "Predict the sentiment of the review 'I love this product' using the mindsdb.sentiment_classifier model": "SELECT review, sentiment\nFROM mindsdb.sentiment_classifier\nWHERE review = 'I love this product';\n"
+            "Predict the sentiments of the reviews table of the google_sheets_datasource using the mindsdb.sentiment_classifier model": "SELECT output.*, input.*\nFROM google_sheets_datasource.reviews AS input\nJOIN mindsdb.sentiment_classifier AS output;"
+        },
+        {
+            "Predict if the data in the spam_data table of the sqlite_datasource is spam or not using the mindsdb.spam_classifier model": "SELECT output.*, input.*\nFROM sqlite_datasource.spam_data AS input\nJOIN mindsdb.spam_classifier AS output;"
+        }
+    ],
+    "predict_one": [
+        {
+            "Predict the sentiment of the review 'I love this product' using the mindsdb.sentiment_classifier model": "SELECT review, sentiment\nFROM mindsdb.sentiment_classifier\nWHERE review = 'I love this product';"
         }
     ],
     "select": [
         {
             "Get all rows from the winequality table of the google_sheets_datasource": "SELECT * FROM google_sheets_datasource.winequality"
         },
         {
```

### Comparing `mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql/gpt.py` & `mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql/gpt.py`

 * *Files identical despite different names*

### Comparing `mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql/gpt_text_to_sql.py` & `mindsdb_text_to_sql-0.1.1/mindsdb_text_to_sql/gpt_text_to_sql.py`

 * *Files identical despite different names*

### Comparing `mindsdb_text_to_sql-0.1.0/mindsdb_text_to_sql.egg-info/PKG-INFO` & `mindsdb_text_to_sql-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mindsdb-text-to-sql
-Version: 0.1.0
+Name: mindsdb_text_to_sql
+Version: 0.1.1
 Summary: MindsDB Text to SQL, converts natural language to SQL code.
 Home-page: https://github.com/MinuraPunchihewa/mindsdb-text-to-sql
 Author: Minura Punchihewa
 Author-email: minurapunchihewa17@gmail.com
 License: UNKNOWN
 Download-URL: https://pypi.org/project/mindsdb-text-to-sql/
 Description: # MindsDB Text to SQL
```

### Comparing `mindsdb_text_to_sql-0.1.0/setup.py` & `mindsdb_text_to_sql-0.1.1/setup.py`

 * *Files identical despite different names*

