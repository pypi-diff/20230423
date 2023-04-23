# Comparing `tmp/dss-python-sdk-0.0.9.tar.gz` & `tmp/dss-python-sdk-0.10.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dss-python-sdk-0.0.9.tar", last modified: Tue Nov 10 08:49:21 2020, max compression
+gzip compressed data, was "dss-python-sdk-0.10.0.tar", last modified: Sun Apr 23 08:08:16 2023, max compression
```

## Comparing `dss-python-sdk-0.0.9.tar` & `dss-python-sdk-0.10.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 vivian    (1000) vivian    (1000)        0 2020-11-10 08:49:21.000000 dss-python-sdk-0.0.9/
-drwxr-xr-x   0 vivian    (1000) vivian    (1000)        0 2020-11-10 08:49:21.000000 dss-python-sdk-0.0.9/dss_python_sdk/
--rw-r--r--   0 vivian    (1000) vivian    (1000)        0 2020-07-30 08:51:11.000000 dss-python-sdk-0.0.9/dss_python_sdk/__init__.py
--rw-r--r--   0 vivian    (1000) vivian    (1000)     1150 2020-08-13 07:42:22.000000 dss-python-sdk-0.0.9/dss_python_sdk/db_utils.py
--rw-r--r--   0 vivian    (1000) vivian    (1000)      828 2020-08-13 07:40:51.000000 dss-python-sdk-0.0.9/dss_python_sdk/dss_utils.py
--rw-r--r--   0 vivian    (1000) vivian    (1000)     1035 2020-10-12 09:20:37.000000 dss-python-sdk-0.0.9/dss_python_sdk/http_utils.py
--rw-r--r--   0 vivian    (1000) vivian    (1000)     1153 2020-11-10 06:54:29.000000 dss-python-sdk-0.0.9/dss_python_sdk/memory_utils.py
--rw-r--r--   0 vivian    (1000) vivian    (1000)     1150 2020-08-13 08:12:59.000000 dss-python-sdk-0.0.9/dss_python_sdk/misc_utils.py
--rw-r--r--   0 vivian    (1000) vivian    (1000)     1153 2020-08-13 08:12:59.000000 dss-python-sdk-0.0.9/dss_python_sdk/queue_utils.py
--rw-r--r--   0 vivian    (1000) vivian    (1000)      633 2020-08-13 07:48:55.000000 dss-python-sdk-0.0.9/dss_python_sdk/test_db_utils.py
--rw-r--r--   0 vivian    (1000) vivian    (1000)      595 2020-11-10 08:10:44.000000 dss-python-sdk-0.0.9/dss_python_sdk/test_memory_utils.py
--rw-r--r--   0 vivian    (1000) vivian    (1000)      589 2020-08-13 08:01:58.000000 dss-python-sdk-0.0.9/dss_python_sdk/test_misc_utils.py
--rw-r--r--   0 vivian    (1000) vivian    (1000)      645 2020-10-12 09:19:58.000000 dss-python-sdk-0.0.9/dss_python_sdk/test_queue_utils.py
-drwxr-xr-x   0 vivian    (1000) vivian    (1000)        0 2020-11-10 08:49:21.000000 dss-python-sdk-0.0.9/dss_python_sdk.egg-info/
--rw-rw-r--   0 vivian    (1000) vivian    (1000)        1 2020-11-10 08:49:21.000000 dss-python-sdk-0.0.9/dss_python_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vivian    (1000) vivian    (1000)      221 2020-11-10 08:49:21.000000 dss-python-sdk-0.0.9/dss_python_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vivian    (1000) vivian    (1000)       14 2020-11-10 08:49:21.000000 dss-python-sdk-0.0.9/dss_python_sdk.egg-info/requires.txt
--rw-rw-r--   0 vivian    (1000) vivian    (1000)      545 2020-11-10 08:49:21.000000 dss-python-sdk-0.0.9/dss_python_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vivian    (1000) vivian    (1000)       15 2020-11-10 08:49:21.000000 dss-python-sdk-0.0.9/dss_python_sdk.egg-info/top_level.txt
--rw-rw-r--   0 vivian    (1000) vivian    (1000)      221 2020-11-10 08:49:21.000000 dss-python-sdk-0.0.9/PKG-INFO
--rw-r--r--   0 vivian    (1000) vivian    (1000)     1408 2020-08-13 08:02:24.000000 dss-python-sdk-0.0.9/README.md
--rw-rw-r--   0 vivian    (1000) vivian    (1000)       38 2020-11-10 08:49:21.000000 dss-python-sdk-0.0.9/setup.cfg
--rw-r--r--   0 vivian    (1000) vivian    (1000)      334 2020-11-10 08:47:22.000000 dss-python-sdk-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:08:16.860492 dss-python-sdk-0.10.0/
+-rw-rw-rw-   0        0        0      159 2023-04-23 08:08:16.860492 dss-python-sdk-0.10.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1505 2023-04-23 07:18:15.000000 dss-python-sdk-0.10.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 08:08:16.853515 dss-python-sdk-0.10.0/dss_python_sdk/
+-rw-rw-rw-   0        0        0        0 2023-04-23 07:18:15.000000 dss-python-sdk-0.10.0/dss_python_sdk/__init__.py
+-rw-rw-rw-   0        0        0     1183 2023-04-23 07:18:15.000000 dss-python-sdk-0.10.0/dss_python_sdk/db_utils.py
+-rw-rw-rw-   0        0        0      850 2023-04-23 07:18:15.000000 dss-python-sdk-0.10.0/dss_python_sdk/dss_utils.py
+-rw-rw-rw-   0        0        0     1071 2023-04-23 07:18:15.000000 dss-python-sdk-0.10.0/dss_python_sdk/http_utils.py
+-rw-rw-rw-   0        0        0     1186 2023-04-23 07:18:15.000000 dss-python-sdk-0.10.0/dss_python_sdk/memory_utils.py
+-rw-rw-rw-   0        0        0     1183 2023-04-23 07:18:15.000000 dss-python-sdk-0.10.0/dss_python_sdk/misc_utils.py
+-rw-rw-rw-   0        0        0     1186 2023-04-23 07:18:15.000000 dss-python-sdk-0.10.0/dss_python_sdk/queue_utils.py
+-rw-rw-rw-   0        0        0      651 2023-04-23 07:18:15.000000 dss-python-sdk-0.10.0/dss_python_sdk/test_db_utils.py
+-rw-rw-rw-   0        0        0      613 2023-04-23 07:18:15.000000 dss-python-sdk-0.10.0/dss_python_sdk/test_memory_utils.py
+-rw-rw-rw-   0        0        0      607 2023-04-23 07:18:15.000000 dss-python-sdk-0.10.0/dss_python_sdk/test_misc_utils.py
+-rw-rw-rw-   0        0        0      711 2023-04-23 07:18:15.000000 dss-python-sdk-0.10.0/dss_python_sdk/test_queue_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:08:16.859500 dss-python-sdk-0.10.0/dss_python_sdk.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-04-23 08:08:16.000000 dss-python-sdk-0.10.0/dss_python_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2023-04-23 08:08:16.000000 dss-python-sdk-0.10.0/dss_python_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 08:08:16.000000 dss-python-sdk-0.10.0/dss_python_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-23 08:08:16.000000 dss-python-sdk-0.10.0/dss_python_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-23 08:08:16.000000 dss-python-sdk-0.10.0/dss_python_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 08:08:16.861488 dss-python-sdk-0.10.0/setup.cfg
+-rw-rw-rw-   0        0        0      350 2023-04-23 07:53:18.000000 dss-python-sdk-0.10.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dss-python-sdk-0.0.9/dss_python_sdk/db_utils.py` & `dss-python-sdk-0.10.0/dss_python_sdk/db_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# -*- coding: utf-8 -*-
-__author__ = 'vivian'
-
-import yaml
-from dss_python_sdk.http_utils import http_get
-from dss_python_sdk.dss_utils import check_param
-from dss_python_sdk.dss_utils import TIMEOUT
-
-
-def get_db_properties(url, plat_key, svc_code, profile, user_agent):
-    """
-    Get database connection parameters
-    :param url:
-    :param plat_key:
-    :param svc_code:
-    :param profile:
-    :param user_agent:
-    :return:
-    """
-    check_param(url, plat_key, svc_code, profile, user_agent)
-    prams = {"platkey": plat_key, "svccode": svc_code, "profile": profile}
-    if user_agent.strip() == "":
-        user_agent = svc_code
-    res_bytes = http_get(url, user_agent, prams, TIMEOUT)
-    d = yaml.load(res_bytes, Loader=yaml.FullLoader)
-    try:
-        ret_dict = d["database"]
-        return ret_dict
-    except TypeError:
-        # It indicates that the server does not return db.yml file normally, either the PLATKEY is wrong,
-        # or the SVCCODE is wrong, or the PROFILE is wrong.
-        # If there is no problem in self-examination, contact the data source management system administrator
-        raise Exception(res_bytes)
+# -*- coding: utf-8 -*-
+__author__ = 'vivian'
+
+import yaml
+from dss_python_sdk.http_utils import http_get
+from dss_python_sdk.dss_utils import check_param
+from dss_python_sdk.dss_utils import TIMEOUT
+
+
+def get_db_properties(url, plat_key, svc_code, profile, user_agent):
+    """
+    Get database connection parameters
+    :param url:
+    :param plat_key:
+    :param svc_code:
+    :param profile:
+    :param user_agent:
+    :return:
+    """
+    check_param(url, plat_key, svc_code, profile, user_agent)
+    prams = {"platkey": plat_key, "svccode": svc_code, "profile": profile}
+    if user_agent.strip() == "":
+        user_agent = svc_code
+    res_bytes = http_get(url, user_agent, prams, TIMEOUT)
+    d = yaml.load(res_bytes, Loader=yaml.FullLoader)
+    try:
+        ret_dict = d["database"]
+        return ret_dict
+    except TypeError:
+        # It indicates that the server does not return db.yml file normally, either the PLATKEY is wrong,
+        # or the SVCCODE is wrong, or the PROFILE is wrong.
+        # If there is no problem in self-examination, contact the data source management system administrator
+        raise Exception(res_bytes)
```

### Comparing `dss-python-sdk-0.0.9/dss_python_sdk/dss_utils.py` & `dss-python-sdk-0.10.0/dss_python_sdk/dss_utils.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# -*- coding: utf-8 -*-
-__author__ = 'vivian'
-
-TIMEOUT = 3
-PROFILE_RC1 = "rc1"
-PROFILE_RC2 = "rc2"
-PROFILE_PROD = "prod"
-
-
-def check_param(url, plat_key, svc_code, profile, user_agent):
-    if url is None or url.strip() == "":
-        raise Exception("URL can't be empty string")
-    if not url.startswith("https"):
-        raise Exception("Only https protocol is supported ")
-    if plat_key is None or plat_key.strip() == "":
-        raise Exception("plat_key can't be empty string")
-    if svc_code is None or svc_code.strip() == "":
-        raise Exception("svc_code can't be empty string")
-    if profile is None or profile.strip() == "":
-        raise Exception("profile can't be empty string")
-    if profile != PROFILE_RC1 and profile != PROFILE_RC2 and profile != PROFILE_PROD:
-        raise Exception("profile error")
+# -*- coding: utf-8 -*-
+__author__ = 'vivian'
+
+TIMEOUT = 3
+PROFILE_RC1 = "rc1"
+PROFILE_RC2 = "rc2"
+PROFILE_PROD = "prod"
+
+
+def check_param(url, plat_key, svc_code, profile, user_agent):
+    if url is None or url.strip() == "":
+        raise Exception("URL can't be empty string")
+    if not url.startswith("https"):
+        raise Exception("Only https protocol is supported ")
+    if plat_key is None or plat_key.strip() == "":
+        raise Exception("plat_key can't be empty string")
+    if svc_code is None or svc_code.strip() == "":
+        raise Exception("svc_code can't be empty string")
+    if profile is None or profile.strip() == "":
+        raise Exception("profile can't be empty string")
+    if profile != PROFILE_RC1 and profile != PROFILE_RC2 and profile != PROFILE_PROD:
+        raise Exception("profile error")
```

### Comparing `dss-python-sdk-0.0.9/dss_python_sdk/http_utils.py` & `dss-python-sdk-0.10.0/dss_python_sdk/http_utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# -*- coding: utf-8 -*-
-__author__ = 'vivian'
-import sys
-
-
-def http_get(url, user_agent, prams, time_out):
-    """
-    http get request,
-    :param url:
-    :param user_agent:
-    :param prams:
-    :param time_out:
-    :return:
-    """
-    if sys.version > '3':
-        import urllib3
-        import urllib
-        data = urllib.parse.urlencode(prams)
-        url = url + "?" + data
-        http = urllib3.PoolManager(timeout=time_out, cert_reqs='CERT_NONE')
-        f = http.request(method='GET', url=url, headers={"User-Agent": user_agent})
-        res_bytes = f.data
-        msg = res_bytes.decode("utf-8")
-        f.close()
-        return msg
-    else:
-        import urllib2
-        import ssl
-        import urllib
-        data = urllib.urlencode(prams)
-        url = url + "?" + data
-        request = urllib2.Request(url, headers={"User-Agent": user_agent})
-        f = urllib2.urlopen(request, timeout=time_out, context=ssl._create_unverified_context())
-        res_bytes = f.read()
-        f.close()
-        return res_bytes
+# -*- coding: utf-8 -*-
+__author__ = 'vivian'
+import sys
+
+
+def http_get(url, user_agent, prams, time_out):
+    """
+    http get request,
+    :param url:
+    :param user_agent:
+    :param prams:
+    :param time_out:
+    :return:
+    """
+    if sys.version > '3':
+        import urllib3
+        import urllib
+        data = urllib.parse.urlencode(prams)
+        url = url + "?" + data
+        http = urllib3.PoolManager(timeout=time_out, cert_reqs='CERT_NONE')
+        f = http.request(method='GET', url=url, headers={"User-Agent": user_agent})
+        res_bytes = f.data
+        msg = res_bytes.decode("utf-8")
+        f.close()
+        return msg
+    else:
+        import urllib2
+        import ssl
+        import urllib
+        data = urllib.urlencode(prams)
+        url = url + "?" + data
+        request = urllib2.Request(url, headers={"User-Agent": user_agent})
+        f = urllib2.urlopen(request, timeout=time_out, context=ssl._create_unverified_context())
+        res_bytes = f.read()
+        f.close()
+        return res_bytes
```

### Comparing `dss-python-sdk-0.0.9/dss_python_sdk/memory_utils.py` & `dss-python-sdk-0.10.0/dss_python_sdk/misc_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# -*- coding: utf-8 -*-
-__author__ = 'vivian'
-
-import yaml
-from dss_python_sdk.http_utils import http_get
-from dss_python_sdk.dss_utils import check_param
-from dss_python_sdk.dss_utils import TIMEOUT
-
-
-def get_mem_properties(url, plat_key, svc_code, profile, user_agent):
-    """
-    Get database connection parameters
-    :param url:
-    :param plat_key:
-    :param svc_code:
-    :param profile:
-    :param user_agent:
-    :return:
-    """
-    check_param(url, plat_key, svc_code, profile, user_agent)
-    prams = {"platkey": plat_key, "svccode": svc_code, "profile": profile}
-    if user_agent.strip() == "":
-        user_agent = svc_code
-    res_bytes = http_get(url, user_agent, prams, TIMEOUT)
-    d = yaml.load(res_bytes, Loader=yaml.FullLoader)
-    try:
-        ret_dict = d["memory"]
-        return ret_dict
-    except TypeError:
-        # It indicates that the server does not return memory.yml file normally, either the PLATKEY is wrong,
-        # or the SVCCODE is wrong, or the PROFILE is wrong.
-        # If there is no problem in self-examination, contact the data source management system administrator
-        raise Exception(res_bytes)
+# -*- coding: utf-8 -*-
+__author__ = 'vivian'
+
+import yaml
+from dss_python_sdk.http_utils import http_get
+from dss_python_sdk.dss_utils import check_param
+from dss_python_sdk.dss_utils import TIMEOUT
+
+
+def get_misc_properties(url, plat_key, svc_code, profile, user_agent):
+    """
+    Get database connection parameters
+    :param url:
+    :param plat_key:
+    :param svc_code:
+    :param profile:
+    :param user_agent:
+    :return:
+    """
+    check_param(url, plat_key, svc_code, profile, user_agent)
+    prams = {"platkey": plat_key, "svccode": svc_code, "profile": profile}
+    if user_agent.strip() == "":
+        user_agent = svc_code
+    res_bytes = http_get(url, user_agent, prams, TIMEOUT)
+    d = yaml.load(res_bytes, Loader=yaml.FullLoader)
+    try:
+        ret_dict = d["misc"]
+        return ret_dict
+    except TypeError:
+        # It indicates that the server does not return misc.yml file normally, either the PLATKEY is wrong,
+        # or the SVCCODE is wrong, or the PROFILE is wrong.
+        # If there is no problem in self-examination, contact the data source management system administrator
+        raise Exception(res_bytes)
```

### Comparing `dss-python-sdk-0.0.9/dss_python_sdk/misc_utils.py` & `dss-python-sdk-0.10.0/dss_python_sdk/memory_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# -*- coding: utf-8 -*-
-__author__ = 'vivian'
-
-import yaml
-from dss_python_sdk.http_utils import http_get
-from dss_python_sdk.dss_utils import check_param
-from dss_python_sdk.dss_utils import TIMEOUT
-
-
-def get_misc_properties(url, plat_key, svc_code, profile, user_agent):
-    """
-    Get database connection parameters
-    :param url:
-    :param plat_key:
-    :param svc_code:
-    :param profile:
-    :param user_agent:
-    :return:
-    """
-    check_param(url, plat_key, svc_code, profile, user_agent)
-    prams = {"platkey": plat_key, "svccode": svc_code, "profile": profile}
-    if user_agent.strip() == "":
-        user_agent = svc_code
-    res_bytes = http_get(url, user_agent, prams, TIMEOUT)
-    d = yaml.load(res_bytes, Loader=yaml.FullLoader)
-    try:
-        ret_dict = d["misc"]
-        return ret_dict
-    except TypeError:
-        # It indicates that the server does not return misc.yml file normally, either the PLATKEY is wrong,
-        # or the SVCCODE is wrong, or the PROFILE is wrong.
-        # If there is no problem in self-examination, contact the data source management system administrator
-        raise Exception(res_bytes)
+# -*- coding: utf-8 -*-
+__author__ = 'vivian'
+
+import yaml
+from dss_python_sdk.http_utils import http_get
+from dss_python_sdk.dss_utils import check_param
+from dss_python_sdk.dss_utils import TIMEOUT
+
+
+def get_mem_properties(url, plat_key, svc_code, profile, user_agent):
+    """
+    Get database connection parameters
+    :param url:
+    :param plat_key:
+    :param svc_code:
+    :param profile:
+    :param user_agent:
+    :return:
+    """
+    check_param(url, plat_key, svc_code, profile, user_agent)
+    prams = {"platkey": plat_key, "svccode": svc_code, "profile": profile}
+    if user_agent.strip() == "":
+        user_agent = svc_code
+    res_bytes = http_get(url, user_agent, prams, TIMEOUT)
+    d = yaml.load(res_bytes, Loader=yaml.FullLoader)
+    try:
+        ret_dict = d["memory"]
+        return ret_dict
+    except TypeError:
+        # It indicates that the server does not return memory.yml file normally, either the PLATKEY is wrong,
+        # or the SVCCODE is wrong, or the PROFILE is wrong.
+        # If there is no problem in self-examination, contact the data source management system administrator
+        raise Exception(res_bytes)
```

### Comparing `dss-python-sdk-0.0.9/dss_python_sdk/queue_utils.py` & `dss-python-sdk-0.10.0/dss_python_sdk/queue_utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# -*- coding: utf-8 -*-
-__author__ = 'vivian'
-
-import yaml
-from dss_python_sdk.http_utils import http_get
-from dss_python_sdk.dss_utils import check_param
-from dss_python_sdk.dss_utils import TIMEOUT
-
-
-def get_queue_properties(url, plat_key, svc_code, profile, user_agent):
-    """
-    Get database connection parameters
-    :param url:
-    :param plat_key:
-    :param svc_code:
-    :param profile:
-    :param user_agent:
-    :return:
-    """
-    check_param(url, plat_key, svc_code, profile, user_agent)
-    prams = {"platkey": plat_key, "svccode": svc_code, "profile": profile}
-    if user_agent.strip() == "":
-        user_agent = svc_code
-    res_bytes = http_get(url, user_agent, prams, TIMEOUT)
-    d = yaml.load(res_bytes, Loader=yaml.FullLoader)
-    try:
-        ret_dict = d["queue"]
-        return ret_dict
-    except TypeError:
-        # It indicates that the server does not return queue.yml file normally, either the PLATKEY is wrong,
-        # or the SVCCODE is wrong, or the PROFILE is wrong.
-        # If there is no problem in self-examination, contact the data source management system administrator
-        raise Exception(res_bytes)
+# -*- coding: utf-8 -*-
+__author__ = 'vivian'
+
+import yaml
+from dss_python_sdk.http_utils import http_get
+from dss_python_sdk.dss_utils import check_param
+from dss_python_sdk.dss_utils import TIMEOUT
+
+
+def get_queue_properties(url, plat_key, svc_code, profile, user_agent):
+    """
+    Get database connection parameters
+    :param url:
+    :param plat_key:
+    :param svc_code:
+    :param profile:
+    :param user_agent:
+    :return:
+    """
+    check_param(url, plat_key, svc_code, profile, user_agent)
+    prams = {"platkey": plat_key, "svccode": svc_code, "profile": profile}
+    if user_agent.strip() == "":
+        user_agent = svc_code
+    res_bytes = http_get(url, user_agent, prams, TIMEOUT)
+    d = yaml.load(res_bytes, Loader=yaml.FullLoader)
+    try:
+        ret_dict = d["queue"]
+        return ret_dict
+    except TypeError:
+        # It indicates that the server does not return queue.yml file normally, either the PLATKEY is wrong,
+        # or the SVCCODE is wrong, or the PROFILE is wrong.
+        # If there is no problem in self-examination, contact the data source management system administrator
+        raise Exception(res_bytes)
```

### Comparing `dss-python-sdk-0.0.9/dss_python_sdk/test_db_utils.py` & `dss-python-sdk-0.10.0/dss_python_sdk/test_db_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# -*- coding: utf-8 -*-
-__author__ = 'vivian'
-
-import unittest
-from dss_python_sdk.db_utils import get_db_properties
-
-
-class TestDBUtils(unittest.TestCase):
-    def test_get_db_properties(self):
-        url = "https://test.example.com/dss/db"
-        plat_key = "xx"
-        svc_code = "xx"
-        profile = "xx"
-        user_agent = svc_code
-        databases = get_db_properties(url, plat_key, svc_code, profile, user_agent)
-        for (k, v) in databases.items():
-            print("dsn-n:%s, ip:%s, port:%d, sid:%s, username:%s, password:%s" %
-                  (k, v["ip"], v["port"], v["sid"], v["username"], v["password"]))
+# -*- coding: utf-8 -*-
+__author__ = 'vivian'
+
+import unittest
+from dss_python_sdk.db_utils import get_db_properties
+
+
+class TestDBUtils(unittest.TestCase):
+    def test_get_db_properties(self):
+        url = "https://test.example.com/dss/db"
+        plat_key = "xx"
+        svc_code = "xx"
+        profile = "xx"
+        user_agent = svc_code
+        databases = get_db_properties(url, plat_key, svc_code, profile, user_agent)
+        for (k, v) in databases.items():
+            print("dsn-n:%s, ip:%s, port:%d, sid:%s, username:%s, password:%s" %
+                  (k, v["ip"], v["port"], v["sid"], v["username"], v["password"]))
```

### Comparing `dss-python-sdk-0.0.9/dss_python_sdk/test_memory_utils.py` & `dss-python-sdk-0.10.0/dss_python_sdk/test_memory_utils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# -*- coding: utf-8 -*-
-__author__ = 'vivian'
-
-import unittest
-from dss_python_sdk.memory_utils import get_mem_properties
-
-
-class TestDBUtils(unittest.TestCase):
-    def test_get_queue_properties(self):
-        url = "https://test.example.com/dss/mem"
-        plat_key = "xxx"
-        svc_code = "xxx"
-        profile = "xxx"
-        user_agent = svc_code
-        miscs = get_mem_properties(url, plat_key, svc_code, profile, user_agent)
-        for (k, v) in miscs.items():
-            print("mem-n:%s, server_path:%s, mount_path:%s " %
-                  (k, v["server_path"], v["mount_path"]))
+# -*- coding: utf-8 -*-
+__author__ = 'vivian'
+
+import unittest
+from dss_python_sdk.memory_utils import get_mem_properties
+
+
+class TestDBUtils(unittest.TestCase):
+    def test_get_queue_properties(self):
+        url = "https://test.example.com/dss/mem"
+        plat_key = "xxx"
+        svc_code = "xxx"
+        profile = "xxx"
+        user_agent = svc_code
+        miscs = get_mem_properties(url, plat_key, svc_code, profile, user_agent)
+        for (k, v) in miscs.items():
+            print("mem-n:%s, server_path:%s, mount_path:%s " %
+                  (k, v["server_path"], v["mount_path"]))
```

### Comparing `dss-python-sdk-0.0.9/dss_python_sdk/test_queue_utils.py` & `dss-python-sdk-0.10.0/dss_python_sdk/test_queue_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# -*- coding: utf-8 -*-
-__author__ = 'vivian'
-
-import unittest
-from dss_python_sdk.queue_utils import get_queue_properties
-
-
-class TestDBUtils(unittest.TestCase):
-    def test_get_queue_properties(self):
-        url = "https://test.example.com/dss/queue"
-        plat_key = "xx"
-        svc_code = "xx"
-        profile = "xx"
-        user_agent = svc_code
-        queues = get_queue_properties(url, plat_key, svc_code, profile, user_agent)
-        for (k, v) in queues.items():
-            print("mq-n:%s, ip:%s, port:%d, vhost:%s, username:%s, password:%s" %
-                  (k, v["ip"], v["port"], v["vhost"], v["username"], v["password"]))
+# -*- coding: utf-8 -*-
+__author__ = 'vivian'
+
+import unittest
+from dss_python_sdk.queue_utils import get_queue_properties
+
+
+class TestDBUtils(unittest.TestCase):
+    def test_get_queue_properties(self):
+        url = "https://test.example.com/dss/queue"
+        plat_key = "xx"
+        svc_code = "xx"
+        profile = "xx"
+        user_agent = svc_code
+        queues = get_queue_properties(url, plat_key, svc_code, profile, user_agent)
+        for (k, v) in queues.items():
+            print("mq-n:%s, ip:%s, port:%d, vhost:%s, username:%s, password:%s, cluster:%s, topic:%s" %
+                  (k, v["ip"], v["port"], v["vhost"], v["username"], v["password"], v["cluster"], v["topic"]))
```

### Comparing `dss-python-sdk-0.0.9/dss_python_sdk.egg-info/SOURCES.txt` & `dss-python-sdk-0.10.0/dss_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

