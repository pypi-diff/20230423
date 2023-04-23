# Comparing `tmp/SalamHunter-0.0.8.tar.gz` & `tmp/SalamHunter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SalamHunter-0.0.8.tar", last modified: Wed Aug 17 23:58:07 2022, max compression
+gzip compressed data, was "SalamHunter-0.0.9.tar", last modified: Mon Aug 22 21:44:13 2022, max compression
```

## Comparing `SalamHunter-0.0.8.tar` & `SalamHunter-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 root         (0)     9997        0 2022-08-17 23:58:07.420285 SalamHunter-0.0.8/
--rw-rw----   0 root         (0)     9997     1068 2022-08-05 16:34:15.000000 SalamHunter-0.0.8/LICENSE
--rw-rw----   0 root         (0)     9997     2508 2022-08-17 23:58:07.400285 SalamHunter-0.0.8/PKG-INFO
--rw-rw----   0 root         (0)     9997     2001 2022-08-06 16:50:48.000000 SalamHunter-0.0.8/README.md
--rw-rw----   0 root         (0)     9997       38 2022-08-17 23:58:07.420285 SalamHunter-0.0.8/setup.cfg
--rw-rw----   0 root         (0)     9997     1110 2022-08-17 23:53:36.000000 SalamHunter-0.0.8/setup.py
-drwxrwx---   0 root         (0)     9997        0 2022-08-17 23:58:07.110285 SalamHunter-0.0.8/src/
-drwxrwx---   0 root         (0)     9997        0 2022-08-17 23:58:07.270285 SalamHunter-0.0.8/src/SalamHunter/
--rw-rw----   0 root         (0)     9997    18937 2022-08-17 23:52:05.000000 SalamHunter-0.0.8/src/SalamHunter/SalamHunter.py
--rw-rw----   0 root         (0)     9997       28 2022-08-05 20:51:19.000000 SalamHunter-0.0.8/src/SalamHunter/__init__.py
-drwxrwx---   0 root         (0)     9997        0 2022-08-17 23:58:07.380285 SalamHunter-0.0.8/src/SalamHunter.egg-info/
--rw-rw----   0 root         (0)     9997     2508 2022-08-17 23:58:06.000000 SalamHunter-0.0.8/src/SalamHunter.egg-info/PKG-INFO
--rw-rw----   0 root         (0)     9997      241 2022-08-17 23:58:07.000000 SalamHunter-0.0.8/src/SalamHunter.egg-info/SOURCES.txt
--rw-rw----   0 root         (0)     9997        1 2022-08-17 23:58:06.000000 SalamHunter-0.0.8/src/SalamHunter.egg-info/dependency_links.txt
--rw-rw----   0 root         (0)     9997       12 2022-08-17 23:58:07.000000 SalamHunter-0.0.8/src/SalamHunter.egg-info/top_level.txt
+drwxrwx---   0 root         (0)     9997        0 2022-08-22 21:44:13.614757 SalamHunter-0.0.9/
+-rw-rw----   0 root         (0)     9997     1068 2022-08-05 16:34:15.000000 SalamHunter-0.0.9/LICENSE
+-rw-rw----   0 root         (0)     9997     2508 2022-08-22 21:44:13.604757 SalamHunter-0.0.9/PKG-INFO
+-rw-rw----   0 root         (0)     9997     2001 2022-08-06 16:50:48.000000 SalamHunter-0.0.9/README.md
+-rw-rw----   0 root         (0)     9997       38 2022-08-22 21:44:13.624757 SalamHunter-0.0.9/setup.cfg
+-rw-rw----   0 root         (0)     9997     1110 2022-08-22 18:31:22.000000 SalamHunter-0.0.9/setup.py
+drwxrwx---   0 root         (0)     9997        0 2022-08-22 21:44:13.294757 SalamHunter-0.0.9/src/
+drwxrwx---   0 root         (0)     9997        0 2022-08-22 21:44:13.474757 SalamHunter-0.0.9/src/SalamHunter/
+-rw-rw----   0 root         (0)     9997    21097 2022-08-22 18:27:41.000000 SalamHunter-0.0.9/src/SalamHunter/SalamHunter.py
+-rw-rw----   0 root         (0)     9997       28 2022-08-05 20:51:19.000000 SalamHunter-0.0.9/src/SalamHunter/__init__.py
+drwxrwx---   0 root         (0)     9997        0 2022-08-22 21:44:13.584757 SalamHunter-0.0.9/src/SalamHunter.egg-info/
+-rw-rw----   0 root         (0)     9997     2508 2022-08-22 21:44:13.000000 SalamHunter-0.0.9/src/SalamHunter.egg-info/PKG-INFO
+-rw-rw----   0 root         (0)     9997      241 2022-08-22 21:44:13.000000 SalamHunter-0.0.9/src/SalamHunter.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0)     9997        1 2022-08-22 21:44:13.000000 SalamHunter-0.0.9/src/SalamHunter.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0)     9997       12 2022-08-22 21:44:13.000000 SalamHunter-0.0.9/src/SalamHunter.egg-info/top_level.txt
```

### Comparing `SalamHunter-0.0.8/LICENSE` & `SalamHunter-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SalamHunter-0.0.8/PKG-INFO` & `SalamHunter-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SalamHunter
-Version: 0.0.8
+Version: 0.0.9
 Summary: • Script Very Nice To Helping Programmer .
 Home-page: https://github.com/salammzere3/SalamHunterr
 Author: salammzere3
 Author-email: salamhunter@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SalamHunter Version: 0.0.8 Summary: â¢ Script Very
+Metadata-Version: 2.1 Name: SalamHunter Version: 0.0.9 Summary: â¢ Script Very
 Nice To Helping Programmer . Home-page: https://github.com/salammzere3/
 SalamHunterr Author: salammzere3 Author-email: salamhunter@gmail.com Project-
 URL: Bug Tracker, https://github.com/pypa/sampleproject/issues Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 2 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3 Description-Content-Type: text/
 markdown License-File: LICENSE
```

### Comparing `SalamHunter-0.0.8/README.md` & `SalamHunter-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `SalamHunter-0.0.8/setup.py` & `SalamHunter-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 f.write('requests\nuser_agent\njson\nsecrets\nnames\nhashlib\nurllib\nuuid\nre\nmechanize\ninstaloader ')
 
 fr = open("requirements.txt",'r')
 requires = fr.read().split('\n')
     
 setuptools.setup(
     name="SalamHunter",
-    version="0.0.8",
+    version="0.0.9",
     author="salammzere3",
     author_email="salamhunter@gmail.com",
     description="• Script Very Nice To Helping Programmer .",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/salammzere3/SalamHunterr",
     project_urls={
```

### Comparing `SalamHunter-0.0.8/src/SalamHunter/SalamHunter.py` & `SalamHunter-0.0.9/src/SalamHunter/SalamHunter.py`

 * *Files 4% similar despite different names*

```diff
@@ -385,7 +385,34 @@
             private = res['user']['is_private']
             following = info_insta.following(username)
             followers = info_insta.followers(username)
             date = info_insta.date(username)
             return {'status':'Success','username':str(username),'id':str(id),'name':str(full_name),'following':str(following),'followers':str(followers),'date':str(date),'private':str(private),'profile':str(profile),'sessionid':str(session)}
 
 
+
+
+class Tiktok:
+    def sendreset(email: str) -> str:
+        url = 'https://api16-va.tiktokv.com/passport/email/send_code/?passport-sdk-version=19&os_api=22&device_type=SM-G975N&ssmix=a&manifest_version_code=2021806060&dpi=240&uoo=0&carrier_region=AR&region=IQ&app_name=musical_ly&version_name=18.6.6&timezone_offset=10800&ts=1660261379&ab_version=18.6.6&residence=AR&cpu_support64=false&current_region=US&ac2=wifi&app_type=normal&ac=wifi&host_abi=armeabi-v7a&update_version_code=2021806060&channel=googleplay&_rticket=1660261381871&device_platform=android&iid=7126814077612115718&build_number=18.6.6&locale=ar&op_region=AR&version_code=180606&timezone_name=Europe%2FMoscow&cdid=86654e69-0edf-405a-a5a1-181f0e7aa14f&openudid=1c8a72b315ac7fbf&sys_region=IQ&device_id=6833300910404519430&app_language=ar&resolution=1280*720&os_version=5.1.1&language=ar&device_brand=samsung&aid=1233&mcc_mnc=310410'
+        
+        headers = {
+        'Host': 'api16-va.tiktokv.com',
+        'x-ss-stub': '04465DFECBF3ED2D56AF61B7DE2921AB',
+        'accept-encoding': 'gzip',
+        'passport-sdk-version': '19',
+        'sdk-version': '2',
+        'x-ss-req-ticket': '1660261382504',
+        'cookie': 'odin_tt=7a321b6667e2ada3027155e053cc1e681ac076f643fbe4861f283fe2ecbc80c1260f1371bb96c8a4812ba32df7d22d4b785a5ba640289e1913e674bd3ffd6b52e8e38d3ade7f3d2d3e41f79931cfb1d4; passport_csrf_token_default=f7bdb605ee9f55f0186b3f0da6cc71e4; store-idc=alisg; store-country-code=cn; install_id=7126814077612115718; ttreq=1$065fc339e22f7da8844faf9adc4f19e5f267c6eb',
+        'x-gorgon': '04048032500189a229bdf66e04feefcf47d5ccc94e336871888b',
+        'x-khronos': '1660261382',
+        'content-type': 'application/x-www-form-urlencoded; charset=UTF-8',
+        'content-length': '131',
+        'user-agent': 'okhttp/3.10.0.1',
+    }
+        data = f'email={email}&account_sdk_source=app&rules_version=v2&mix_mode=1&multi_login=1&type=31'
+        req = requests.post(url, headers=headers, data=data)
+        if req.json()["message"] =="success":
+            return {'status': 'Success', 'email': email}
+            
+        else:
+            return {'status': 'error', 'email': email}
```

### Comparing `SalamHunter-0.0.8/src/SalamHunter.egg-info/PKG-INFO` & `SalamHunter-0.0.9/src/SalamHunter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SalamHunter
-Version: 0.0.8
+Version: 0.0.9
 Summary: • Script Very Nice To Helping Programmer .
 Home-page: https://github.com/salammzere3/SalamHunterr
 Author: salammzere3
 Author-email: salamhunter@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SalamHunter Version: 0.0.8 Summary: â¢ Script Very
+Metadata-Version: 2.1 Name: SalamHunter Version: 0.0.9 Summary: â¢ Script Very
 Nice To Helping Programmer . Home-page: https://github.com/salammzere3/
 SalamHunterr Author: salammzere3 Author-email: salamhunter@gmail.com Project-
 URL: Bug Tracker, https://github.com/pypa/sampleproject/issues Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 2 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3 Description-Content-Type: text/
 markdown License-File: LICENSE
```

