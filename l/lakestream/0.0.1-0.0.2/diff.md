# Comparing `tmp/lakestream-0.0.1.tar.gz` & `tmp/lakestream-0.0.2.tar.gz`

## Comparing `lakestream-0.0.1.tar` & `lakestream-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,36 @@
--rw-r--r--   0        0        0     1231 1970-01-01 00:00:00.000000 lakestream-0.0.1/local_dependencies/lakestream/Cargo.toml
--rw-r--r--   0      501       20     2010 2023-04-14 06:06:29.000000 lakestream-0.0.1/local_dependencies/lakestream/src/base/cli.rs
--rw-r--r--   0      501       20     6824 2023-04-14 06:06:29.000000 lakestream-0.0.1/local_dependencies/lakestream/src/base/interfaces.rs
--rw-r--r--   0      501       20       33 2023-04-14 06:06:29.000000 lakestream-0.0.1/local_dependencies/lakestream/src/base/mod.rs
--rw-r--r--   0      501       20       50 2023-04-14 06:06:29.000000 lakestream-0.0.1/local_dependencies/lakestream/src/default.rs
--rw-r--r--   0      501       20      115 2023-04-14 06:06:29.000000 lakestream-0.0.1/local_dependencies/lakestream/src/http/mod.rs
--rw-r--r--   0      501       20     1942 2023-04-14 06:06:29.000000 lakestream-0.0.1/local_dependencies/lakestream/src/http/requests.rs
--rw-r--r--   0      501       20      264 2023-04-14 06:06:29.000000 lakestream-0.0.1/local_dependencies/lakestream/src/lib.rs
--rw-r--r--   0      501       20      557 2023-04-14 06:06:29.000000 lakestream-0.0.1/local_dependencies/lakestream/src/main.rs
--rw-r--r--   0      501       20     8412 2023-04-14 06:06:29.000000 lakestream-0.0.1/local_dependencies/lakestream/src/s3/bucket.rs
--rw-r--r--   0      501       20     8855 2023-04-14 06:06:29.000000 lakestream-0.0.1/local_dependencies/lakestream/src/s3/client.rs
--rw-r--r--   0      501       20       28 2023-04-14 06:06:29.000000 lakestream-0.0.1/local_dependencies/lakestream/src/s3/mod.rs
--rw-r--r--   0      501       20     1031 2023-04-14 06:06:29.000000 lakestream-0.0.1/local_dependencies/lakestream/src/utils/formatters.rs
--rw-r--r--   0      501       20      136 2023-04-14 06:06:29.000000 lakestream-0.0.1/local_dependencies/lakestream/src/utils/mod.rs
--rw-r--r--   0      501       20      436 2023-04-14 06:06:29.000000 lakestream-0.0.1/local_dependencies/lakestream/src/utils/timeparse.rs
--rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 lakestream-0.0.1/Cargo.toml
--rw-r--r--   0      501       20      254 2023-04-14 06:06:29.000000 lakestream-0.0.1/Makefile
--rw-r--r--   0      501       20       74 2023-04-14 06:06:29.000000 lakestream-0.0.1/README.md
--rw-r--r--   0      501       20       26 2023-04-14 06:06:29.000000 lakestream-0.0.1/lakestream/__init__.py
--rw-r--r--   0      501       20      163 2023-04-14 06:06:29.000000 lakestream-0.0.1/lakestream/__main__.py
--rw-r--r--   0      501       20      811 2023-04-14 06:06:30.000000 lakestream-0.0.1/pyproject.toml
--rw-r--r--   0      501       20     3677 2023-04-14 06:06:29.000000 lakestream-0.0.1/src/lib.rs
--rw-r--r--   0      501       20    69826 2023-04-14 06:07:39.000000 lakestream-0.0.1/Cargo.lock
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 lakestream-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1541 1970-01-01 00:00:00.000000 lakestream-0.0.2/local_dependencies/lakestream/Cargo.toml
+-rw-r--r--   0      501       20     9549 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/base/filters.rs
+-rw-r--r--   0      501       20     8978 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/base/interfaces.rs
+-rw-r--r--   0      501       20       37 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/base/mod.rs
+-rw-r--r--   0      501       20     2585 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/cli/ls_command.rs
+-rw-r--r--   0      501       20       32 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/cli/mod.rs
+-rw-r--r--   0      501       20     2897 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/cli/parser.rs
+-rw-r--r--   0      501       20       94 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/default.rs
+-rw-r--r--   0      501       20      135 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/http/mod.rs
+-rw-r--r--   0      501       20     2129 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/http/requests.rs
+-rw-r--r--   0      501       20      472 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/http/requests_wasm32.rs
+-rw-r--r--   0      501       20      368 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/lib.rs
+-rw-r--r--   0      501       20     1095 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/localfs/bucket.rs
+-rw-r--r--   0      501       20     2830 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/localfs/list.rs
+-rw-r--r--   0      501       20       26 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/localfs/mod.rs
+-rw-r--r--   0      501       20      125 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/main.rs
+-rw-r--r--   0      501       20     1459 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/s3/bucket.rs
+-rw-r--r--   0      501       20     8602 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/s3/client.rs
+-rw-r--r--   0      501       20     1127 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/s3/config.rs
+-rw-r--r--   0      501       20    13869 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/s3/list.rs
+-rw-r--r--   0      501       20       50 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/s3/mod.rs
+-rw-r--r--   0      501       20     1036 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/utils/formatters.rs
+-rw-r--r--   0      501       20      200 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/utils/mod.rs
+-rw-r--r--   0      501       20     1031 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/utils/time.rs
+-rw-r--r--   0      501       20     1779 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/utils/time_parse.rs
+-rw-r--r--   0      501       20      689 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/utils/time_parse_ext.rs
+-rw-r--r--   0      501       20      370 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/utils/time_parse_ext_wasm32.rs
+-rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 lakestream-0.0.2/Cargo.toml
+-rw-r--r--   0      501       20      300 2023-04-23 21:04:46.000000 lakestream-0.0.2/Makefile
+-rw-r--r--   0      501       20     3393 2023-04-23 21:04:46.000000 lakestream-0.0.2/README.rst
+-rw-r--r--   0      501       20     1794 2023-04-23 21:04:46.000000 lakestream-0.0.2/lakestream/__init__.py
+-rw-r--r--   0      501       20      165 2023-04-23 21:04:46.000000 lakestream-0.0.2/lakestream/__main__.py
+-rw-r--r--   0      501       20      991 2023-04-23 21:04:47.000000 lakestream-0.0.2/pyproject.toml
+-rw-r--r--   0      501       20     4312 2023-04-23 21:04:46.000000 lakestream-0.0.2/src/lib.rs
+-rw-r--r--   0      501       20    68929 2023-04-23 21:05:49.000000 lakestream-0.0.2/Cargo.lock
+-rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 lakestream-0.0.2/PKG-INFO
```

### Comparing `lakestream-0.0.1/local_dependencies/lakestream/Cargo.toml` & `lakestream-0.0.2/local_dependencies/lakestream/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 [package]
 name = "lakestream"
-version = "0.0.1"
+version = "0.0.2"
+authors = ["Anthony Potappel <aprxi@lakestream.dev>"]
 edition = "2021"
+
 description = "Portable file-utility for object-stores"
+documentation = "https://docs.rs/lakestream"
+homepage = "https://lakestream.dev"
+repository = "https://github.com/serverlessnext/lakestream"
+readme = "../README.rst"
 license = "MIT"
 
+
 [lib]
 name = "lakestream"
 path = "src/lib.rs"
 
 [[bin]]
 name = "lakestream"
 path = "src/main.rs"
 
 [dependencies]
 percent-encoding = { version = "2.1", default-features = false, features = ["alloc"] }
 hex = { version = "0.4.3", default-features = false, features = ["alloc"] }
 serde = { version = "1.0", features = ["derive", "alloc"] }
-hmac = { version = "0.11.0", default-features = false }
-sha2 = { version = "0.9.8", default-features = false }
-serde_json = {version = "1.0.95", default-features = false, features = ["alloc"]}
-regex = { version = "1.7", default-features = false}
-itertools = "0.10.1"
-serde-xml-rs = "0.4.1"
-url = "2.2.2"
+hmac = { version = "0.11", default-features = false }
+sha2 = { version = "0.9.9", default-features = false }
+serde_json = {version = "1.0", default-features = false, features = ["alloc"]}
+regex = { version = "1.7", default-features = false, features = ["std", "unicode"] }
+itertools = "0.10"
+serde-xml-rs = "0.6"
+url = "2.3"
+clap = { version = "4.2" , default-features = false, features = ["std", "help"]}
 
 [target.'cfg(not(target_arch = "wasm32"))'.dependencies]
-clap = { version = "4.2" , features = ["derive"] }
-ureq = { version = "2.2", default-features = false, features = ["tls"]}
 time = { version = "0.3", features = ["parsing"]}
+ureq = { version = "2.2", default-features = false, features = ["tls"]}
 
 # [target.'cfg(target_arch = "wasm32")'.dependencies]
 # js-sys = "0.3"
-# web-sys = { version = "0.3", features = ["Request", "RequestInit", "Response", "Window"] }
+# web-sys = { version = "0.3", features = ['Request', 'RequestInit', 'RequestMode', 'Headers', 'Window', 'Response', 'console'] }
 # wasm-bindgen = "0.2.84"
 # wasm-bindgen-futures = "0.4"
```

### Comparing `lakestream-0.0.1/local_dependencies/lakestream/src/base/interfaces.rs` & `lakestream-0.0.2/local_dependencies/lakestream/src/base/interfaces.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 use std::collections::HashMap;
 
 use regex::Regex;
 use serde::Deserialize;
 use serde_json::{Map, Value};
 
+use crate::localfs::bucket::LocalFs;
 use crate::s3::bucket::{list_buckets, S3Bucket};
 use crate::utils::formatters::{bytes_human_readable, time_human_readable};
+use crate::FileObjectFilter;
 
 pub enum ListObjectsResult {
     Buckets(Vec<ObjectStore>),
     FileObjects(Vec<FileObject>),
 }
 
 pub struct ObjectStoreHandler {
@@ -20,35 +22,48 @@
     pub fn new(configs: Vec<HashMap<String, Value>>) -> Self {
         ObjectStoreHandler { configs }
     }
 
     pub fn list_objects(
         uri: String,
         config: HashMap<String, String>,
+        recursive: bool,
         max_files: Option<u32>,
+        filter: &Option<FileObjectFilter>,
     ) -> ListObjectsResult {
         let (scheme, bucket, prefix) = ObjectStoreHandler::parse_uri(uri);
 
         if let Some(bucket) = bucket {
-            let bucket_uri = format!("{}://{}", scheme.unwrap(), bucket);
+            // list files in a bucket
+            let bucket_uri = if let Some(scheme) = scheme {
+                format!("{}://{}", scheme, bucket)
+            } else {
+                format!("localfs://{}", bucket)
+            };
             let object_store = ObjectStore::new(&bucket_uri, config).unwrap();
-            let file_objects =
-                object_store.list_files(prefix.as_deref(), max_files);
+
+            let file_objects = object_store.list_files(
+                prefix.as_deref(),
+                recursive,
+                max_files,
+                filter,
+            );
             ListObjectsResult::FileObjects(file_objects)
         } else {
+            // list buckets
             let mut object_store_configuration = HashMap::new();
             let config_map: Map<String, Value> = config
                 .into_iter()
                 .map(|(k, v)| (k, Value::String(v)))
                 .collect();
             object_store_configuration
                 .insert("config".to_string(), Value::Object(config_map));
             object_store_configuration.insert(
                 "uri".to_string(),
-                Value::String(format!("{}://", scheme.unwrap()).to_string()),
+                Value::String(format!("{}://", scheme.unwrap())),
             );
 
             let configs = vec![object_store_configuration];
             let handler = ObjectStoreHandler::new(configs);
 
             let object_stores = handler.list_object_stores();
             ListObjectsResult::Buckets(object_stores)
@@ -61,42 +76,31 @@
         if uri.is_empty() {
             return (None, None, None);
         }
 
         let re = Regex::new(r"^(?P<scheme>[a-z0-9]+)://").unwrap();
         let scheme_match = re.captures(&uri);
 
-        if let Some(scheme_captures) = scheme_match {
-            let scheme = scheme_captures.name("scheme").unwrap().as_str();
-            let uri_without_scheme = re.replace(&uri, "");
-            if uri_without_scheme.is_empty() {
-                return (Some(scheme.to_string()), None, None);
-            }
-            let mut parts = uri_without_scheme.splitn(2, '/');
-            let bucket = parts.next().map(|s| s.to_string());
-            let prefix = parts
-                .next()
-                .map(|s| {
-                    if s.is_empty() {
-                        None
-                    } else {
-                        if s.ends_with('/') {
-                            Some(s.to_string())
-                        } else {
-                            Some(format!("{}/", s))
-                        }
-                    }
-                })
-                .flatten();
-
-            (Some(scheme.to_string()), bucket, prefix)
-        } else {
-            eprintln!("Error: Invalid URI or missing scheme.");
-            (None, None, None)
-        }
+        scheme_match.map_or_else(
+            || {
+                // uri has no scheme, assume LocalFs
+                let (bucket, prefix) = parse_uri_path(&uri);
+                (None, bucket, prefix)
+            },
+            |scheme_captures| {
+                let scheme = scheme_captures.name("scheme").unwrap().as_str();
+                let uri_without_scheme = re.replace(&uri, "").to_string();
+                if uri_without_scheme.is_empty() {
+                    (Some(scheme.to_string()), None, None)
+                } else {
+                    let (bucket, prefix) = parse_uri_path(&uri_without_scheme);
+                    (Some(scheme.to_string()), bucket, prefix)
+                }
+            },
+        )
     }
 
     pub fn list_object_stores(&self) -> Vec<ObjectStore> {
         let mut object_stores = Vec::new();
 
         for config in &self.configs {
             let default_uri = Value::String("".to_string());
@@ -111,65 +115,90 @@
             // Convert the serde_json::Map<String, Value> back to HashMap<String, String>
             let config_hashmap: HashMap<String, String> = config_config
                 .iter()
                 .map(|(k, v)| (k.clone(), v.as_str().unwrap().to_string()))
                 .collect();
 
             if uri.starts_with("s3://") {
-                object_stores.append(&mut list_buckets(&config_hashmap));
+                match list_buckets(&config_hashmap) {
+                    Ok(mut buckets) => object_stores.append(&mut buckets),
+                    Err(err) => eprintln!("Error listing buckets: {}", err),
+                }
             } else {
                 eprintln!("Unsupported object store type: {}", uri);
             }
         }
         object_stores
     }
 }
 
 pub trait ObjectStoreTrait {
     fn name(&self) -> &str;
+    fn config(&self) -> &HashMap<String, String>;
     fn list_files(
         &self,
         prefix: Option<&str>,
+        recursive: bool,
         max_keys: Option<u32>,
+        filter: &Option<FileObjectFilter>,
     ) -> Vec<FileObject>;
 }
 
 pub enum ObjectStore {
     S3Bucket(S3Bucket),
-    // Add more object store types here later.
+    LocalFs(LocalFs),
 }
 
 impl ObjectStore {
     pub fn new(
         name: &str,
         config: HashMap<String, String>,
     ) -> Result<ObjectStore, String> {
         if name.starts_with("s3://") {
             let name = name.trim_start_matches("s3://");
-            let bucket = S3Bucket::new(name, config);
+            let bucket =
+                S3Bucket::new(name, config).map_err(|err| err.to_string())?;
             Ok(ObjectStore::S3Bucket(bucket))
+        } else if name.starts_with("localfs://") {
+            let name = name.trim_start_matches("localfs://");
+            let local_fs =
+                LocalFs::new(name, config).map_err(|err| err.to_string())?;
+            Ok(ObjectStore::LocalFs(local_fs))
         } else {
             Err("Unsupported object store.".to_string())
         }
     }
 
     pub fn name(&self) -> &str {
         match self {
             ObjectStore::S3Bucket(bucket) => bucket.name(),
+            ObjectStore::LocalFs(local_fs) => local_fs.name(),
+        }
+    }
+
+    pub fn config(&self) -> &HashMap<String, String> {
+        match self {
+            ObjectStore::S3Bucket(bucket) => bucket.config(),
+            ObjectStore::LocalFs(local_fs) => local_fs.config(),
         }
     }
 
     pub fn list_files(
         &self,
         prefix: Option<&str>,
+        recursive: bool,
         max_keys: Option<u32>,
+        filter: &Option<FileObjectFilter>,
     ) -> Vec<FileObject> {
         match self {
             ObjectStore::S3Bucket(bucket) => {
-                bucket.list_files(prefix, max_keys)
+                bucket.list_files(prefix, recursive, max_keys, filter)
+            }
+            ObjectStore::LocalFs(local_fs) => {
+                local_fs.list_files(prefix, recursive, max_keys, filter)
             }
         }
     }
 }
 
 #[derive(Debug, Clone, Deserialize)]
 pub struct FileObject {
@@ -206,30 +235,66 @@
         self.modified
     }
 
     pub fn tags(&self) -> &Option<HashMap<String, String>> {
         &self.tags
     }
 
-    pub fn printable(&self) -> String {
+    pub fn printable(&self, full_path: bool) -> String {
         let name_without_trailing_slash = self.name.trim_end_matches('/');
-        let mut basename = name_without_trailing_slash
-            .split('/')
-            .last()
-            .unwrap_or(name_without_trailing_slash)
-            .to_string();
+        let mut name_to_print = if full_path {
+            name_without_trailing_slash.to_string()
+        } else {
+            name_without_trailing_slash
+                .split('/')
+                .last()
+                .unwrap_or(name_without_trailing_slash)
+                .to_string()
+        };
 
         if self.name.ends_with('/') {
-            basename.push('/');
+            name_to_print.push('/');
         }
+
         format!(
             "{:8} {} {}",
             bytes_human_readable(self.size()),
             if let Some(modified) = self.modified() {
                 time_human_readable(modified)
             } else {
                 "PRE".to_string()
             },
-            basename
+            name_to_print
         )
     }
 }
+
+fn parse_uri_path(uri_path: &str) -> (Option<String>, Option<String>) {
+    let cleaned_uri = uri_path.trim_end_matches('.');
+
+    if cleaned_uri.is_empty() {
+        return (Some(".".to_string()), None);
+    }
+
+    let is_absolute = cleaned_uri.starts_with('/');
+    let mut parts = cleaned_uri.splitn(2, '/');
+    let bucket = parts.next().map(|s| s.to_string());
+    let prefix = parts.next().filter(|s| !s.is_empty()).map(|s| {
+        let cleaned_prefix = s.replace("./", "");
+        if cleaned_prefix.ends_with('/') {
+            cleaned_prefix
+        } else {
+            format!("{}/", cleaned_prefix)
+        }
+    });
+
+    if let Some(bucket) = bucket {
+        let formatted_bucket = if is_absolute {
+            format!("/{}", bucket)
+        } else {
+            bucket
+        };
+        return (Some(formatted_bucket), prefix);
+    }
+
+    (Some(".".to_string()), None)
+}
```

### Comparing `lakestream-0.0.1/local_dependencies/lakestream/src/http/requests.rs` & `lakestream-0.0.2/local_dependencies/lakestream/src/http/requests.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 use std::collections::HashMap;
 use std::error::Error;
 use std::io::Read;
 
 use ureq::{Agent, Response};
 
+type ResponseData = (String, u16, HashMap<String, String>);
+type HttpResult = Result<ResponseData, Box<dyn Error>>;
+type ResponseDataWithoutHeaders = (String, u16);
+type HttpResultWithoutHeaders =
+    Result<ResponseDataWithoutHeaders, Box<dyn Error>>;
+
 pub fn http_get_request(
     url: &str,
     headers: &HashMap<String, String>,
-) -> Result<(String, u16), Box<dyn Error>> {
+) -> HttpResultWithoutHeaders {
     let response = perform_request(url, headers)?;
     let status = response.status();
 
     if !(200..300).contains(&status) {
         return Ok((String::new(), status));
     }
     let mut body = String::new();
     response.into_reader().read_to_string(&mut body)?;
     Ok((body, status))
 }
 
 pub fn http_get_request_with_headers(
     url: &str,
     headers: &HashMap<String, String>,
-) -> Result<(String, u16, HashMap<String, String>), Box<dyn Error>> {
+) -> HttpResult {
     let response = perform_request(url, headers)?;
     let status = response.status();
     let headers_map = parse_response_headers(&response);
 
     if !(200..300).contains(&status) {
         return Ok((String::new(), status, headers_map));
     }
@@ -41,15 +47,15 @@
     headers: &HashMap<String, String>,
 ) -> Result<Response, Box<dyn Error>> {
     let agent = Agent::new();
     let mut request_builder = agent.get(url);
 
     // Add headers to the request
     for (key, value) in headers {
-        request_builder = request_builder.set(&key, &value);
+        request_builder = request_builder.set(key, value);
     }
 
     let response = request_builder.call()?;
     Ok(response)
 }
 
 fn parse_response_headers(
```

### Comparing `lakestream-0.0.1/local_dependencies/lakestream/src/s3/client.rs` & `lakestream-0.0.2/local_dependencies/lakestream/src/s3/client.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 use std::collections::HashMap;
 
 use hmac::{Hmac, Mac, NewMac};
 use itertools::Itertools;
-use percent_encoding::{utf8_percent_encode, AsciiSet, CONTROLS};
+use percent_encoding::{utf8_percent_encode, CONTROLS};
 use sha2::{Digest, Sha256};
-use time::OffsetDateTime;
-use url::Url;
+use url::{form_urlencoded, Url};
 
 use super::bucket::S3Credentials;
-
-const CUSTOM_ENCODE_SET: &AsciiSet = &CONTROLS.add(b'/');
+use crate::utils::time::UtcTimeNow;
+use crate::AWS_MAX_LIST_OBJECTS;
 
 fn sign(key: &[u8], msg: &[u8]) -> Vec<u8> {
     let mut hmac = Hmac::<Sha256>::new_from_slice(key)
         .expect("HMAC can take key of any size");
     hmac.update(msg);
     let result = hmac.finalize();
     result.into_bytes().as_slice().to_vec()
 }
 
 pub struct S3Client {
     resource: String,
     region: String,
     credentials: S3Credentials,
     endpoint_url: String,
-    utc_now: OffsetDateTime,
+    utc_now: UtcTimeNow,
     query_string: Option<String>,
 }
 
 impl S3Client {
     pub fn new(
         endpoint_url: String,
         region: String,
         credentials: S3Credentials,
     ) -> S3Client {
         let resource = "".to_string();
-        let utc_now = OffsetDateTime::now_utc();
+        let utc_now = UtcTimeNow::new();
 
         S3Client {
             resource,
             region,
             credentials,
             endpoint_url,
             utc_now,
@@ -77,24 +76,17 @@
             }
         }
 
         canonical_headers
     }
 
     fn generate_signing_key(&self) -> Vec<u8> {
-        let date_stamp = format!(
-            "{:04}{:02}{:02}",
-            self.utc_now.year(),
-            self.utc_now.month() as u8,
-            self.utc_now.day()
-        );
-
         let k_date = sign(
             format!("AWS4{}", self.credentials.secret_key()).as_bytes(),
-            date_stamp.as_bytes(),
+            self.utc_now.date_stamp().as_bytes(),
         );
         let k_region = sign(&k_date, self.region.as_bytes());
         let k_service = sign(&k_region, b"s3");
         sign(&k_service, b"aws4_request")
     }
 
     fn initiate_headers(
@@ -109,28 +101,28 @@
             "x-amz-content-sha256".to_string(),
             payload_hash.unwrap_or("UNSIGNED-PAYLOAD").to_string(),
         );
         Ok(headers)
     }
 
     fn get_canonical_uri(&self, url: &Url, resource: &str) -> String {
-        let canonical_resource = utf8_percent_encode(
-            resource.trim_end_matches('/'),
-            CUSTOM_ENCODE_SET,
+        let canonical_resource = form_urlencoded::byte_serialize(
+            resource.trim_end_matches('/').as_bytes(),
         )
-        .to_string();
+        .collect::<String>();
         let endpoint_path =
             url.path().trim_start_matches('/').trim_end_matches('/');
 
         if endpoint_path.is_empty() {
             canonical_resource
         } else {
             format!(
                 "{}/{}",
-                utf8_percent_encode(endpoint_path, CUSTOM_ENCODE_SET),
+                form_urlencoded::byte_serialize(endpoint_path.as_bytes())
+                    .collect::<String>(),
                 canonical_resource
             )
         }
     }
 
     fn get_canonical_query_string(
         &self,
@@ -175,59 +167,49 @@
         self.generate_headers(method, None, None)
     }
 
     pub fn generate_list_objects_headers(
         &mut self,
         prefix: Option<&str>,
         max_keys: Option<u32>,
+        continuation_token: Option<&str>,
     ) -> Result<HashMap<String, String>, Box<dyn std::error::Error>> {
         let method = "GET";
 
-        // Generate the query string for listing files
-        let mut query_parts = vec![
-            "list-type=2".to_string(),
-            format!("max-keys={}", max_keys.unwrap_or(1000)),
-            format!(
-                "delimiter={}",
-                utf8_percent_encode("/", &CUSTOM_ENCODE_SET)
-            ),
-            "encoding-type=url".to_string(),
-        ];
+        // Ensure max_keys does not exceed AWS_MAX_LIST_OBJECTS
+        let max_keys = max_keys
+            .map(|keys| std::cmp::min(keys, AWS_MAX_LIST_OBJECTS))
+            .unwrap_or(AWS_MAX_LIST_OBJECTS);
+
+        let mut query_parts = form_urlencoded::Serializer::new(String::new());
+        query_parts.append_pair("list-type", "2");
+        query_parts.append_pair("max-keys", &max_keys.to_string());
+        query_parts.append_pair("delimiter", "/");
+        query_parts.append_pair("encoding-type", "url");
 
         if let Some(p) = prefix {
-            query_parts.push(format!(
-                "prefix={}",
-                utf8_percent_encode(&p, &CUSTOM_ENCODE_SET)
-            ));
+            query_parts.append_pair("prefix", p);
         }
-        self.query_string = Some(query_parts.join("&"));
+        if let Some(token) = continuation_token {
+            query_parts.append_pair("continuation-token", token);
+        }
+
+        self.query_string = Some(query_parts.finish());
 
-        // Call generate_headers with the generated query_string
         self.generate_headers(method, None, None)
     }
 
     fn generate_headers(
         &mut self,
         method: &str,
         headers: Option<HashMap<String, String>>,
         payload_hash: Option<&str>,
     ) -> Result<HashMap<String, String>, Box<dyn std::error::Error>> {
-        let date_stamp = format!(
-            "{:04}{:02}{:02}",
-            self.utc_now.year(),
-            self.utc_now.month() as u8,
-            self.utc_now.day()
-        );
-        let x_amz_date = format!(
-            "{}T{:02}{:02}{:02}Z",
-            &date_stamp,
-            self.utc_now.hour(),
-            self.utc_now.minute(),
-            self.utc_now.second()
-        );
+        let date_stamp = self.utc_now.date_stamp();
+        let x_amz_date = self.utc_now.x_amz_date();
 
         let credential_scope =
             format!("{}/{}/s3/aws4_request", date_stamp, self.region);
         let mut headers =
             self.initiate_headers(headers, &x_amz_date, payload_hash)?;
 
         let url = Url::parse(&self.endpoint_url)?;
@@ -239,15 +221,15 @@
         headers.insert("host".to_string(), host);
 
         let canonical_uri = self.get_canonical_uri(&url, &self.resource);
 
         let canonical_headers = self.get_canonical_headers(&headers);
         let signed_headers = headers
             .keys()
-            .cloned()
+            .map(|key| key.to_lowercase())
             .sorted()
             .collect::<Vec<String>>()
             .join(";");
 
         let canonical_query_string = self.get_canonical_query_string()?;
 
         let canonical_request = format!(
```

### Comparing `lakestream-0.0.1/local_dependencies/lakestream/src/utils/formatters.rs` & `lakestream-0.0.2/local_dependencies/lakestream/src/utils/formatters.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use super::timeparse::epoch_to_rfc3339;
+use super::time_parse_ext::epoch_to_rfc3339;
 
 pub fn time_human_readable(epoch_time: u64) -> String {
     epoch_to_rfc3339(epoch_time).unwrap()
 }
 
 pub fn bytes_human_readable(size: u64) -> String {
     let exponent: u32;
```

### Comparing `lakestream-0.0.1/pyproject.toml` & `lakestream-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "lakestream"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python interface for Lakestream"
-readme = "README.md"
+readme = "README.rst"
 requires-python = ">=3.7"
+url = "https://lakestream.dev"
+documentation = "https://lakestream.dev/python_api"
+repository = "https://github.com/serverlessnext/lakestream"
+keywords = ["serverless", "data", "api"]
+
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
@@ -23,11 +28,11 @@
 [dependencies]
 
 [project.license]
 text = "MIT"
 
 [[project.maintainers]]
 name = "Anthony Potappel"
-email = "anthony.potappel@gmail.com"
+email = "aprxi@lakestream.dev"
 
 [tool.maturin]
 module-name = "lakestream"
```

### Comparing `lakestream-0.0.1/Cargo.lock` & `lakestream-0.0.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "aho-corasick"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "anstream"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e579a7752471abc2a8268df8b20005e3eadd975f585398f17efcfd8d4927371"
 dependencies = [
  "anstyle",
  "anstyle-parse",
@@ -168,17 +177,17 @@
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
@@ -381,28 +390,28 @@
  "termcolor",
  "terminal_size",
  "textwrap 0.16.0",
 ]
 
 [[package]]
 name = "clap"
-version = "4.2.2"
+version = "4.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b802d85aaf3a1cdb02b224ba472ebdea62014fccfcb269b95a4d76443b5ee5a"
+checksum = "956ac1f6381d8d82ab4684768f89c0ea3afe66925ceadb4eeb3fc452ffc55d62"
 dependencies = [
  "clap_builder",
  "clap_derive 4.2.0",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.2.2"
+version = "4.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14a1a858f532119338887a4b8e1af9c60de8249cd7bafd68036a489e261e37b6"
+checksum = "84080e799e54cff944f4b4a4b0e71630b0e0443b25b985175c7dddc1a859b749"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex 0.4.1",
  "strsim",
  "terminal_size",
@@ -510,17 +519,17 @@
  "libc",
  "unicode-width",
  "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "280a9f2d8b3a38871a3c8a46fb80db65e5e5ed97da80c4d08bf27fb63e35e181"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -646,17 +655,17 @@
  "libc",
  "redox_users",
  "winapi",
 ]
 
 [[package]]
 name = "dunce"
-version = "1.0.3"
+version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bd4b30a6560bbd9b4620f4de34c3f14f60848e58a9b7216801afcb4c7b31c3c"
+checksum = "56ce8c6da7551ec6c462cbaf3bfbc75131ebbfa1c944aeaa9dab51ca1c5f0c3b"
 
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
@@ -805,15 +814,15 @@
 
 [[package]]
 name = "globset"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "029d74589adefde59de1a0c4f4732695c32805624aec7b68d91503d4dba79afc"
 dependencies = [
- "aho-corasick",
+ "aho-corasick 0.7.20",
  "bstr",
  "fnv",
  "log",
  "regex",
 ]
 
 [[package]]
@@ -965,34 +974,17 @@
  "number_prefix",
  "portable-atomic",
  "unicode-width",
 ]
 
 [[package]]
 name = "indoc"
-version = "0.3.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "47741a8bc60fb26eb8d6e0238bbb26d8575ff623fdc97b1a2c00c050b9684ed8"
-dependencies = [
- "indoc-impl",
- "proc-macro-hack",
-]
-
-[[package]]
-name = "indoc-impl"
-version = "0.3.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce046d161f000fffde5f432a0d034d0341dc152643b2598ed5bfce44c4f3a8f0"
-dependencies = [
- "proc-macro-hack",
- "proc-macro2",
- "quote",
- "syn 1.0.109",
- "unindent",
-]
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
@@ -1044,17 +1036,17 @@
 checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lakestream"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
- "clap 4.2.2",
+ "clap 4.2.4",
  "hex",
  "hmac",
  "itertools",
  "percent-encoding",
  "regex",
  "serde",
  "serde-xml-rs",
@@ -1063,15 +1055,15 @@
  "time",
  "ureq",
  "url",
 ]
 
 [[package]]
 name = "lakestream_py"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
  "lakestream",
  "maturin",
  "pyo3",
 ]
 
 [[package]]
@@ -1089,23 +1081,23 @@
  "fs-err",
  "glob",
  "goblin 0.5.4",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.1"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d59d8c75012853d2e872fb56bc8a2e53718e2cafe1a4c823143141c6d90c322f"
+checksum = "36eb31c1778188ae1e64398743890d0877fef36d11521ac60406b42016e8c2cf"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -1345,45 +1337,20 @@
 name = "os_str_bytes"
 version = "6.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ceedf44fb00f2d1984b0bc98102627ce622e083e49a5bacdb3e514fa4238e267"
 
 [[package]]
 name = "parking_lot"
-version = "0.11.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
-dependencies = [
- "instant",
- "lock_api",
- "parking_lot_core 0.8.6",
-]
-
-[[package]]
-name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
- "parking_lot_core 0.9.7",
-]
-
-[[package]]
-name = "parking_lot_core"
-version = "0.8.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
-dependencies = [
- "cfg-if",
- "instant",
- "libc",
- "redox_syscall 0.2.16",
- "smallvec",
- "winapi",
+ "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
 version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
@@ -1392,33 +1359,14 @@
  "libc",
  "redox_syscall 0.2.16",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
-name = "paste"
-version = "0.1.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45ca20c77d80be666aef2b45486da86238fabe33e38306bd3118fe4af33fa880"
-dependencies = [
- "paste-impl",
- "proc-macro-hack",
-]
-
-[[package]]
-name = "paste-impl"
-version = "0.1.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d95a7db200b97ef370c8e6de0088252f7e0dfff7d047a28528e47456c0fc98b6"
-dependencies = [
- "proc-macro-hack",
-]
-
-[[package]]
 name = "path-slash"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "498a099351efa4becc6a19c72aa9270598e8fd274ca47052e37455241c88b696"
 
 [[package]]
 name = "percent-encoding"
@@ -1497,20 +1445,14 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
-name = "proc-macro-hack"
-version = "0.5.20+deprecated"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
-
-[[package]]
 name = "proc-macro2"
 version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
@@ -1522,56 +1464,68 @@
 checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.14.5"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "35100f9347670a566a67aa623369293703322bb9db77d99d7df7313b575ae0c8"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "parking_lot 0.11.2",
- "paste",
+ "memoffset",
+ "parking_lot",
  "pyo3-build-config",
+ "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.14.5"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d12961738cacbd7f91b7c43bc25cfeeaa2698ad07a04b3be0aa88b950865738f"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
+ "target-lexicon",
+]
+
+[[package]]
+name = "pyo3-ffi"
+version = "0.18.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+dependencies = [
+ "libc",
+ "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.14.5"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc0bc5215d704824dfddddc03f93cb572e1155c68b6761c37005e1c288808ea8"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
+ "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.14.5"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71623fc593224afaab918aa3afcaf86ed2f43d34f6afde7f3922608f253240df"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
- "pyo3-build-config",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyproject-toml"
 version = "0.3.3"
@@ -1697,39 +1651,45 @@
  "getrandom",
  "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
- "aho-corasick",
+ "aho-corasick 1.0.1",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.7.1",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 dependencies = [
- "regex-syntax",
+ "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
+name = "regex-syntax"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+
+[[package]]
 name = "rfc2047-decoder"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61fc4b4e52897c3e30b12b7e9b04461215b647fbe66f6def60dd8edbce14ec2e"
 dependencies = [
  "base64 0.21.0",
  "charset",
@@ -1764,32 +1724,32 @@
  "serde",
  "serde_json",
  "winapi",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d4a36c42d1873f9a77c53bde094f9664d9891bc604a45b4798fd2c389ed12e5b"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.11"
+version = "0.37.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85597d61f83914ddeba6a47b3b8ffe7365107221c2e557ed94426489fefb5f77"
+checksum = "d9b864d3c18a5785a05953adeed93e2dca37ed30f18e69bba9f30079d51f363f"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
@@ -1874,17 +1834,17 @@
 checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-xml-rs"
-version = "0.4.1"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0bf1ba0696ccf0872866277143ff1fd14d22eec235d2b23702f95e6660f7dfa"
+checksum = "fb3aa78ecda1ebc9ec9847d5d3aba7d618823446a049ba2491940506da6e2782"
 dependencies = [
  "log",
  "serde",
  "thiserror",
  "xml-rs",
 ]
 
@@ -2282,17 +2242,17 @@
 dependencies = [
  "serde",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-subscriber"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6176eae26dd70d0c919749377897b54a9276bd7061339665dd68777926b5a70"
+checksum = "30a651bc37f915e81f087d86e62a18eec5f79550c7faff886f7090b4ea757c77"
 dependencies = [
  "matchers",
  "once_cell",
  "regex",
  "serde",
  "serde_json",
  "sharded-slab",
@@ -2760,20 +2720,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f5f72397389fd26dd36b01f23e19c0608db8e764f7bb65fdc5b1e7e2aa02550"
 dependencies = [
  "anyhow",
  "bytes",
  "cab",
  "camino",
- "clap 4.2.2",
+ "clap 4.2.4",
  "cli-table",
  "flate2",
  "indicatif",
  "msi",
- "parking_lot 0.12.1",
+ "parking_lot",
  "rayon",
  "regex",
  "serde",
  "serde_json",
  "sha2 0.10.6",
  "tempfile",
  "tracing",
```

