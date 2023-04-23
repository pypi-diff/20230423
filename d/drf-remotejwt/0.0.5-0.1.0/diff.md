# Comparing `tmp/drf-remotejwt-0.0.5.tar.gz` & `tmp/drf-remotejwt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-remotejwt-0.0.5.tar", last modified: Sat Apr 22 04:55:48 2023, max compression
+gzip compressed data, was "drf-remotejwt-0.1.0.tar", last modified: Sun Apr 23 02:15:22 2023, max compression
```

## Comparing `drf-remotejwt-0.0.5.tar` & `drf-remotejwt-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,38 @@
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-22 04:55:48.531897 drf-remotejwt-0.0.5/
--rw-r--r--   0 garrethcain   (501) staff       (20)    33885 2023-04-21 05:14:06.000000 drf-remotejwt-0.0.5/LICENCE
--rw-r--r--   0 garrethcain   (501) staff       (20)      149 2023-04-21 05:14:06.000000 drf-remotejwt-0.0.5/MANIFEST.in
--rw-r--r--   0 garrethcain   (501) staff       (20)     6219 2023-04-22 04:55:48.532087 drf-remotejwt-0.0.5/PKG-INFO
--rw-r--r--   0 garrethcain   (501) staff       (20)       75 2023-04-21 05:14:06.000000 drf-remotejwt-0.0.5/README.rst
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-22 04:55:48.529143 drf-remotejwt-0.0.5/drf-remotejwt/
--rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-04-21 05:14:06.000000 drf-remotejwt-0.0.5/drf-remotejwt/__init__.py
--rw-r--r--   0 garrethcain   (501) staff       (20)       63 2023-04-21 05:14:06.000000 drf-remotejwt-0.0.5/drf-remotejwt/admin.py
--rw-r--r--   0 garrethcain   (501) staff       (20)      148 2023-04-22 04:54:37.000000 drf-remotejwt-0.0.5/drf-remotejwt/apps.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     7281 2023-04-21 05:14:06.000000 drf-remotejwt-0.0.5/drf-remotejwt/authentication.py
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-22 04:55:48.531775 drf-remotejwt-0.0.5/drf-remotejwt/migrations/
--rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-04-21 05:14:06.000000 drf-remotejwt-0.0.5/drf-remotejwt/migrations/__init__.py
--rw-r--r--   0 garrethcain   (501) staff       (20)       57 2023-04-21 05:14:06.000000 drf-remotejwt-0.0.5/drf-remotejwt/models.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     1587 2023-04-21 22:43:59.000000 drf-remotejwt-0.0.5/drf-remotejwt/serializers.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     1971 2023-04-21 05:14:06.000000 drf-remotejwt-0.0.5/drf-remotejwt/settings.py
--rw-r--r--   0 garrethcain   (501) staff       (20)       60 2023-04-21 05:14:06.000000 drf-remotejwt-0.0.5/drf-remotejwt/tests.py
--rw-r--r--   0 garrethcain   (501) staff       (20)      369 2023-04-21 05:14:06.000000 drf-remotejwt-0.0.5/drf-remotejwt/urls.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     5546 2023-04-21 05:14:06.000000 drf-remotejwt-0.0.5/drf-remotejwt/utils.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     1518 2023-04-21 22:45:07.000000 drf-remotejwt-0.0.5/drf-remotejwt/views.py
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-22 04:55:48.531413 drf-remotejwt-0.0.5/drf-remotejwt.egg-info/
--rw-r--r--   0 garrethcain   (501) staff       (20)     6219 2023-04-22 04:55:48.000000 drf-remotejwt-0.0.5/drf-remotejwt.egg-info/PKG-INFO
--rw-r--r--   0 garrethcain   (501) staff       (20)      558 2023-04-22 04:55:48.000000 drf-remotejwt-0.0.5/drf-remotejwt.egg-info/SOURCES.txt
--rw-r--r--   0 garrethcain   (501) staff       (20)        1 2023-04-22 04:55:48.000000 drf-remotejwt-0.0.5/drf-remotejwt.egg-info/dependency_links.txt
--rw-r--r--   0 garrethcain   (501) staff       (20)       57 2023-04-22 04:55:48.000000 drf-remotejwt-0.0.5/drf-remotejwt.egg-info/requires.txt
--rw-r--r--   0 garrethcain   (501) staff       (20)       14 2023-04-22 04:55:48.000000 drf-remotejwt-0.0.5/drf-remotejwt.egg-info/top_level.txt
--rw-r--r--   0 garrethcain   (501) staff       (20)      104 2023-04-21 05:14:06.000000 drf-remotejwt-0.0.5/pyproject.toml
--rw-r--r--   0 garrethcain   (501) staff       (20)     1221 2023-04-22 04:55:48.533065 drf-remotejwt-0.0.5/setup.cfg
--rw-r--r--   0 garrethcain   (501) staff       (20)       37 2023-04-21 05:14:06.000000 drf-remotejwt-0.0.5/setup.py
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-23 02:15:22.296126 drf-remotejwt-0.1.0/
+-rw-r--r--   0 garrethcain   (501) staff       (20)    33885 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.0/LICENCE
+-rw-r--r--   0 garrethcain   (501) staff       (20)      149 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.0/MANIFEST.in
+-rw-r--r--   0 garrethcain   (501) staff       (20)     7574 2023-04-23 02:15:22.296223 drf-remotejwt-0.1.0/PKG-INFO
+-rw-r--r--   0 garrethcain   (501) staff       (20)       75 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.0/README.rst
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-23 02:15:22.289161 drf-remotejwt-0.1.0/drf-remotejwt.egg-info/
+-rw-r--r--   0 garrethcain   (501) staff       (20)     7574 2023-04-23 02:15:22.000000 drf-remotejwt-0.1.0/drf-remotejwt.egg-info/PKG-INFO
+-rw-r--r--   0 garrethcain   (501) staff       (20)      740 2023-04-23 02:15:22.000000 drf-remotejwt-0.1.0/drf-remotejwt.egg-info/SOURCES.txt
+-rw-r--r--   0 garrethcain   (501) staff       (20)        1 2023-04-23 02:15:22.000000 drf-remotejwt-0.1.0/drf-remotejwt.egg-info/dependency_links.txt
+-rw-r--r--   0 garrethcain   (501) staff       (20)       57 2023-04-23 02:15:22.000000 drf-remotejwt-0.1.0/drf-remotejwt.egg-info/requires.txt
+-rw-r--r--   0 garrethcain   (501) staff       (20)       25 2023-04-23 02:15:22.000000 drf-remotejwt-0.1.0/drf-remotejwt.egg-info/top_level.txt
+-rw-r--r--   0 garrethcain   (501) staff       (20)      104 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.0/pyproject.toml
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-23 02:15:22.291449 drf-remotejwt-0.1.0/remotejwt/
+-rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/__init__.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)       63 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/admin.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)      144 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/apps.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     7281 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/authentication.py
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-23 02:15:22.291623 drf-remotejwt-0.1.0/remotejwt/migrations/
+-rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/migrations/__init__.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)       57 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/models.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     1587 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/serializers.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     1971 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/settings.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)       60 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/tests.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)      370 2023-04-23 01:51:41.000000 drf-remotejwt-0.1.0/remotejwt/urls.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     5546 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/utils.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     1518 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/views.py
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-23 02:15:22.295824 drf-remotejwt-0.1.0/remotejwt_user/
+-rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-04-23 00:46:13.000000 drf-remotejwt-0.1.0/remotejwt_user/__init__.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     3324 2023-04-23 01:20:39.000000 drf-remotejwt-0.1.0/remotejwt_user/admin.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)      159 2023-04-23 01:20:52.000000 drf-remotejwt-0.1.0/remotejwt_user/apps.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     8965 2023-04-23 00:46:13.000000 drf-remotejwt-0.1.0/remotejwt_user/models.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-04-23 00:46:13.000000 drf-remotejwt-0.1.0/remotejwt_user/permissions.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)      587 2023-04-23 00:46:13.000000 drf-remotejwt-0.1.0/remotejwt_user/serializers.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)       60 2023-04-23 00:46:13.000000 drf-remotejwt-0.1.0/remotejwt_user/tests.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)      168 2023-04-23 01:42:04.000000 drf-remotejwt-0.1.0/remotejwt_user/urls.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)      673 2023-04-23 00:48:32.000000 drf-remotejwt-0.1.0/remotejwt_user/views.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     1221 2023-04-23 02:15:22.296691 drf-remotejwt-0.1.0/setup.cfg
+-rw-r--r--   0 garrethcain   (501) staff       (20)       37 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.0/setup.py
```

### Comparing `drf-remotejwt-0.0.5/LICENCE` & `drf-remotejwt-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.0.5/PKG-INFO` & `drf-remotejwt-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-remotejwt
-Version: 0.0.5
+Version: 0.1.0
 Summary: A package to authenticate against a remote Authentication Service that support JWTs, think microservice authentication backend.
 Home-page: https://github.com/garrethcain/drf-remotejwt
 Author: Garreth Cain
 Author-email: garrethccain@gmail.com
 License: AGPL-3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -44,27 +44,27 @@
 * /token/refresh/ to refresh an access token.
 * /token/verify/ to confirm if a token is valid or not.
 
 Which all match the auth service exactly. You can decide on the URLs prefix path
 by modifying the config/urls.py file appropriately. 
 
 For example;
-`path('auth/', include("drf-remotejwt.urls"))` 
+`path('auth/', include("remotejwt.urls"))` 
 
 ... will prefix the `/token/`, `/token/verify/`, and `/token/refresh/` endpoints 
 with `/auth/` which gives some clean seperation.
 
 Eg;
 ```PYTHON
 /auth/token/
 /auth/token/refresh/
 /auth/token/verify/
 ```
 
-All you need to is add the drf-remotejwt URLs to your API service that will be 
+All you need to is add the DRF-RemoteJWT URLs to your API service that will be 
 authing against the remote auth-service.
 
 You can't create users in the local client-service. If you retrieve a different
 user from the auth-service you may get integrity errors in that the DRF-RemoteJWT 
 package will overwrite your local user with data from the auth-service... 
 It will assume your local user was updated in the remote auth-service.
 
@@ -78,38 +78,40 @@
 ## Get Started
 
 Create a basic API Project. 
 Then create your first app to contain a view that returns something indicating a
 success.
 Change DRFs default permission class to IsAuthenticated.
 
-Install package `drf-remotejwt` and add the following to the 
-INSTALLED_APPS;
+Install package `remotejwt` and add the following to the INSTALLED_APPS;
 
 ```PYTHON
-'rest_framework', # because it is an API.
-'drf-remotejwt', # for the auth backend to access the auth-service.
-'custom_user.apps.CustomUserConfig', # so the local user model matches the auth
+INSTALLED_APPS = [
+    ...
+    'rest_framework', # because it is an API.
+    'remotejwt', # for the auth backend to access the auth-service.
+    ...
+]
 ```
 
 Add the following config to your settings.py and modify as appropriate.
 
 Assumptions: The auth-service runs on :8000 and the client-service (your API) 
 runs on `:8001`
 
 
 ## Add this configuration to the client-service `settings.py`;
 
-Instruct `REST_FRAMEWORK` that it must use the `drf-remotejwt` module for
+Instruct `REST_FRAMEWORK` that it must use the `remotejwt` module for
 authentication.
 
 ```PYTHON
 REST_FRAMEWORK = {
     "DEFAULT_AUTHENTICATION_CLASSES": (
-        'drf-remotejwt.authentication.RemoteJWTAuthentication',
+        'remotejwt.authentication.RemoteJWTAuthentication',
     ),
 }
 ```
 
 ```PYTHON
 REMOTE_JWT = {
     # leave these as the default.
@@ -139,27 +141,87 @@
 validate the JWT, then use the local user object, if it exists, otherwise a new
 one will be requested if none exists.
 
 Something to think about is that it's possible for the user to authenticate with
 the auth-service directly, then suddenly turn up at your API service and the
 tokens will be honoured...
 
+A custom user `remotejwt_user` has been include in the model and can be used in
+both the client-service and auth-service for convenience. To use it simply add
+the following config.
+
+```PYTHON
+INSTALLED_APPS = [
+    ...
+    'remotejwt_user.User',
+    ...
+]
+```
+
+```PYTHON
+AUTH_USER_MODEL = "remotejwt_user.User"
+```
+
+And then in your auth-service you can import the end points from the package
+like this;
+
+auth_service.urls.py
+```python
+urlpatterns = [
+    path("admin/", admin.site.urls),
+    path('auth/',
+         include(
+            [
+                path('', include('remotejwt.urls')),
+                path('', include('remotejwt_user.urls')),
+            ]
+        )
+    )
+]
+```
+
+or add them in yourself for a bit more control;
+
+```python
+from remotejwt.views import (
+    TokenObtainPairView,
+    TokenRefreshView,
+    TokenVerifyView,
+)
+from remotejwt_user.views import TokenUserDetailView
+
+
+urlpatterns = [
+    path("admin/", admin.site.urls),
+    path("auth/token/", TokenObtainPairView.as_view(), name="token_obtain_pair"),
+    path("auth/token/refresh/", TokenRefreshView.as_view(), name="token_refresh"),
+    path("auth/token/verify/", TokenVerifyView.as_view(), name="token_verify"),
+    path("auth/users/<int:pk>/", TokenUserDetailView.as_view(), name="user_detail"),
+]
+```
+
 
 If you want your DRF views to authenticate in a browser window, ie. the session
 created when you logged in with either the admin panel or your own login page
 then additionally add `rest_framework.authentication.SessionAuthentication` to
 `DEFAULT_AUTHENTICATION_CLASSES` inside `REST_FRAMEWORK`.
 
 Eg.
 ```PYTHON
 REST_FRAMEWORK = {
     "DEFAULT_AUTHENTICATION_CLASSES": (
-        'drf-remotejwt.authentication.RemoteJWTAuthentication',
+        'remotejwt.authentication.RemoteJWTAuthentication',
         'rest_framework.authentication.SessionAuthentication',
+        ...
     ),
 }
 ```
 
 ## TODO:
-1. I think the wrapper for the auth endpoints could be implemented better. Maybe a tidy class.
-2. There seems to be a bug with Simple-JWT which results in the Authorisation heading not being found.
-3. Write something that lets an admin user bring a user from the auth-service into our local service for when they need conf.
+1. I think the wrapper for the auth endpoints could be implemented better. Maybe
+    a tidy class.
+2. There seems to be a bug with Simple-JWT which results in the Authorisation
+    heading not being found.
+3. Write something that lets an admin user bring a user from the auth-service
+    into our local service for when they need conf.
+4. Implement a custom user model for convenience.
+5. Rename the module itself to remove the hyphen.
```

### Comparing `drf-remotejwt-0.0.5/drf-remotejwt/authentication.py` & `drf-remotejwt-0.1.0/remotejwt/authentication.py`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.0.5/drf-remotejwt/serializers.py` & `drf-remotejwt-0.1.0/remotejwt/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.0.5/drf-remotejwt/settings.py` & `drf-remotejwt-0.1.0/remotejwt/settings.py`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.0.5/drf-remotejwt/utils.py` & `drf-remotejwt-0.1.0/remotejwt/utils.py`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.0.5/drf-remotejwt/views.py` & `drf-remotejwt-0.1.0/remotejwt/views.py`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.0.5/drf-remotejwt.egg-info/PKG-INFO` & `drf-remotejwt-0.1.0/drf-remotejwt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-remotejwt
-Version: 0.0.5
+Version: 0.1.0
 Summary: A package to authenticate against a remote Authentication Service that support JWTs, think microservice authentication backend.
 Home-page: https://github.com/garrethcain/drf-remotejwt
 Author: Garreth Cain
 Author-email: garrethccain@gmail.com
 License: AGPL-3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -44,27 +44,27 @@
 * /token/refresh/ to refresh an access token.
 * /token/verify/ to confirm if a token is valid or not.
 
 Which all match the auth service exactly. You can decide on the URLs prefix path
 by modifying the config/urls.py file appropriately. 
 
 For example;
-`path('auth/', include("drf-remotejwt.urls"))` 
+`path('auth/', include("remotejwt.urls"))` 
 
 ... will prefix the `/token/`, `/token/verify/`, and `/token/refresh/` endpoints 
 with `/auth/` which gives some clean seperation.
 
 Eg;
 ```PYTHON
 /auth/token/
 /auth/token/refresh/
 /auth/token/verify/
 ```
 
-All you need to is add the drf-remotejwt URLs to your API service that will be 
+All you need to is add the DRF-RemoteJWT URLs to your API service that will be 
 authing against the remote auth-service.
 
 You can't create users in the local client-service. If you retrieve a different
 user from the auth-service you may get integrity errors in that the DRF-RemoteJWT 
 package will overwrite your local user with data from the auth-service... 
 It will assume your local user was updated in the remote auth-service.
 
@@ -78,38 +78,40 @@
 ## Get Started
 
 Create a basic API Project. 
 Then create your first app to contain a view that returns something indicating a
 success.
 Change DRFs default permission class to IsAuthenticated.
 
-Install package `drf-remotejwt` and add the following to the 
-INSTALLED_APPS;
+Install package `remotejwt` and add the following to the INSTALLED_APPS;
 
 ```PYTHON
-'rest_framework', # because it is an API.
-'drf-remotejwt', # for the auth backend to access the auth-service.
-'custom_user.apps.CustomUserConfig', # so the local user model matches the auth
+INSTALLED_APPS = [
+    ...
+    'rest_framework', # because it is an API.
+    'remotejwt', # for the auth backend to access the auth-service.
+    ...
+]
 ```
 
 Add the following config to your settings.py and modify as appropriate.
 
 Assumptions: The auth-service runs on :8000 and the client-service (your API) 
 runs on `:8001`
 
 
 ## Add this configuration to the client-service `settings.py`;
 
-Instruct `REST_FRAMEWORK` that it must use the `drf-remotejwt` module for
+Instruct `REST_FRAMEWORK` that it must use the `remotejwt` module for
 authentication.
 
 ```PYTHON
 REST_FRAMEWORK = {
     "DEFAULT_AUTHENTICATION_CLASSES": (
-        'drf-remotejwt.authentication.RemoteJWTAuthentication',
+        'remotejwt.authentication.RemoteJWTAuthentication',
     ),
 }
 ```
 
 ```PYTHON
 REMOTE_JWT = {
     # leave these as the default.
@@ -139,27 +141,87 @@
 validate the JWT, then use the local user object, if it exists, otherwise a new
 one will be requested if none exists.
 
 Something to think about is that it's possible for the user to authenticate with
 the auth-service directly, then suddenly turn up at your API service and the
 tokens will be honoured...
 
+A custom user `remotejwt_user` has been include in the model and can be used in
+both the client-service and auth-service for convenience. To use it simply add
+the following config.
+
+```PYTHON
+INSTALLED_APPS = [
+    ...
+    'remotejwt_user.User',
+    ...
+]
+```
+
+```PYTHON
+AUTH_USER_MODEL = "remotejwt_user.User"
+```
+
+And then in your auth-service you can import the end points from the package
+like this;
+
+auth_service.urls.py
+```python
+urlpatterns = [
+    path("admin/", admin.site.urls),
+    path('auth/',
+         include(
+            [
+                path('', include('remotejwt.urls')),
+                path('', include('remotejwt_user.urls')),
+            ]
+        )
+    )
+]
+```
+
+or add them in yourself for a bit more control;
+
+```python
+from remotejwt.views import (
+    TokenObtainPairView,
+    TokenRefreshView,
+    TokenVerifyView,
+)
+from remotejwt_user.views import TokenUserDetailView
+
+
+urlpatterns = [
+    path("admin/", admin.site.urls),
+    path("auth/token/", TokenObtainPairView.as_view(), name="token_obtain_pair"),
+    path("auth/token/refresh/", TokenRefreshView.as_view(), name="token_refresh"),
+    path("auth/token/verify/", TokenVerifyView.as_view(), name="token_verify"),
+    path("auth/users/<int:pk>/", TokenUserDetailView.as_view(), name="user_detail"),
+]
+```
+
 
 If you want your DRF views to authenticate in a browser window, ie. the session
 created when you logged in with either the admin panel or your own login page
 then additionally add `rest_framework.authentication.SessionAuthentication` to
 `DEFAULT_AUTHENTICATION_CLASSES` inside `REST_FRAMEWORK`.
 
 Eg.
 ```PYTHON
 REST_FRAMEWORK = {
     "DEFAULT_AUTHENTICATION_CLASSES": (
-        'drf-remotejwt.authentication.RemoteJWTAuthentication',
+        'remotejwt.authentication.RemoteJWTAuthentication',
         'rest_framework.authentication.SessionAuthentication',
+        ...
     ),
 }
 ```
 
 ## TODO:
-1. I think the wrapper for the auth endpoints could be implemented better. Maybe a tidy class.
-2. There seems to be a bug with Simple-JWT which results in the Authorisation heading not being found.
-3. Write something that lets an admin user bring a user from the auth-service into our local service for when they need conf.
+1. I think the wrapper for the auth endpoints could be implemented better. Maybe
+    a tidy class.
+2. There seems to be a bug with Simple-JWT which results in the Authorisation
+    heading not being found.
+3. Write something that lets an admin user bring a user from the auth-service
+    into our local service for when they need conf.
+4. Implement a custom user model for convenience.
+5. Rename the module itself to remove the hyphen.
```

### Comparing `drf-remotejwt-0.0.5/drf-remotejwt.egg-info/SOURCES.txt` & `drf-remotejwt-0.1.0/drf-remotejwt.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 LICENCE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
-drf-remotejwt/__init__.py
-drf-remotejwt/admin.py
-drf-remotejwt/apps.py
-drf-remotejwt/authentication.py
-drf-remotejwt/models.py
-drf-remotejwt/serializers.py
-drf-remotejwt/settings.py
-drf-remotejwt/tests.py
-drf-remotejwt/urls.py
-drf-remotejwt/utils.py
-drf-remotejwt/views.py
 drf-remotejwt.egg-info/PKG-INFO
 drf-remotejwt.egg-info/SOURCES.txt
 drf-remotejwt.egg-info/dependency_links.txt
 drf-remotejwt.egg-info/requires.txt
 drf-remotejwt.egg-info/top_level.txt
-drf-remotejwt/migrations/__init__.py
+remotejwt/__init__.py
+remotejwt/admin.py
+remotejwt/apps.py
+remotejwt/authentication.py
+remotejwt/models.py
+remotejwt/serializers.py
+remotejwt/settings.py
+remotejwt/tests.py
+remotejwt/urls.py
+remotejwt/utils.py
+remotejwt/views.py
+remotejwt/migrations/__init__.py
+remotejwt_user/__init__.py
+remotejwt_user/admin.py
+remotejwt_user/apps.py
+remotejwt_user/models.py
+remotejwt_user/permissions.py
+remotejwt_user/serializers.py
+remotejwt_user/tests.py
+remotejwt_user/urls.py
+remotejwt_user/views.py
```

### Comparing `drf-remotejwt-0.0.5/setup.cfg` & `drf-remotejwt-0.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drf-remotejwt
-version = 0.0.5
+version = 0.1.0
 description = A package to authenticate against a remote Authentication Service that support JWTs, think microservice authentication backend.
 long_description = file: README.MD
 long_description_content_type = text/markdown
 readme = "README.MD"
 url = https://github.com/garrethcain/drf-remotejwt
 author = Garreth Cain
 author_email = garrethccain@gmail.com
```

