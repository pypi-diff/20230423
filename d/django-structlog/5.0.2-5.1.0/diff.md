# Comparing `tmp/django-structlog-5.0.2.tar.gz` & `tmp/django-structlog-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-structlog-5.0.2.tar", last modified: Mon Apr 17 00:49:30 2023, max compression
+gzip compressed data, was "django-structlog-5.1.0.tar", last modified: Sun Apr 23 02:54:08 2023, max compression
```

## Comparing `django-structlog-5.0.2.tar` & `django-structlog-5.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:30.238410 django-structlog-5.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-17 00:49:20.000000 django-structlog-5.0.2/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 00:49:20.000000 django-structlog-5.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-04-17 00:49:30.238410 django-structlog-5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21911 2023-04-17 00:49:20.000000 django-structlog-5.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:30.234410 django-structlog-5.0.2/django_structlog/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:30.234410 django-structlog-5.0.2/django_structlog/celery/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/celery/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/celery/receivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/celery/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/celery/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:30.238410 django-structlog-5.0.2/django_structlog/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/middlewares/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:30.234410 django-structlog-5.0.2/django_structlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-04-17 00:49:30.000000 django-structlog-5.0.2/django_structlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-17 00:49:30.000000 django-structlog-5.0.2/django_structlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 00:49:30.000000 django-structlog-5.0.2/django_structlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-17 00:49:30.000000 django-structlog-5.0.2/django_structlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 00:49:30.000000 django-structlog-5.0.2/django_structlog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-17 00:49:20.000000 django-structlog-5.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 00:49:30.238410 django-structlog-5.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:54:08.865115 django-structlog-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-23 02:53:57.000000 django-structlog-5.1.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 02:53:57.000000 django-structlog-5.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-04-23 02:54:08.865115 django-structlog-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21911 2023-04-23 02:53:57.000000 django-structlog-5.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:54:08.865115 django-structlog-5.1.0/django_structlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:54:08.865115 django-structlog-5.1.0/django_structlog/celery/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/celery/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/celery/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/celery/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/celery/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:54:08.865115 django-structlog-5.1.0/django_structlog/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/middlewares/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:54:08.865115 django-structlog-5.1.0/django_structlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-04-23 02:54:08.000000 django-structlog-5.1.0/django_structlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-23 02:54:08.000000 django-structlog-5.1.0/django_structlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 02:54:08.000000 django-structlog-5.1.0/django_structlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-23 02:54:08.000000 django-structlog-5.1.0/django_structlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 02:54:08.000000 django-structlog-5.1.0/django_structlog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-23 02:53:57.000000 django-structlog-5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-23 02:54:08.865115 django-structlog-5.1.0/setup.cfg
```

### Comparing `django-structlog-5.0.2/LICENSE.rst` & `django-structlog-5.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `django-structlog-5.0.2/PKG-INFO` & `django-structlog-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-structlog
-Version: 5.0.2
+Version: 5.1.0
 Summary: Structured Logging for Django
 Author-email: Jules Robichaud-Gagnon <j.robichaudg+pypi@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/jrobichaud/django-structlog
 Project-URL: repository, https://github.com/jrobichaud/django-structlog
 Project-URL: documentation, https://django-structlog.readthedocs.io
 Classifier: Framework :: Django
```

### Comparing `django-structlog-5.0.2/README.rst` & `django-structlog-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-structlog-5.0.2/django_structlog/celery/middlewares.py` & `django-structlog-5.1.0/django_structlog/celery/middlewares.py`

 * *Files identical despite different names*

### Comparing `django-structlog-5.0.2/django_structlog/celery/receivers.py` & `django-structlog-5.1.0/django_structlog/celery/receivers.py`

 * *Files identical despite different names*

### Comparing `django-structlog-5.0.2/django_structlog/celery/signals.py` & `django-structlog-5.1.0/django_structlog/celery/signals.py`

 * *Files identical despite different names*

### Comparing `django-structlog-5.0.2/django_structlog/celery/steps.py` & `django-structlog-5.1.0/django_structlog/celery/steps.py`

 * *Files identical despite different names*

### Comparing `django-structlog-5.0.2/django_structlog/middlewares/request.py` & `django-structlog-5.1.0/django_structlog/middlewares/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,23 @@
             )
             logger.info(
                 "request_finished",
                 code=response.status_code,
                 request=self.format_request(request),
             )
         else:
+            exception = getattr(request, "_raised_exception")
             delattr(request, "_raised_exception")
+            signals.update_failure_response.send(
+                sender=self.__class__,
+                request=request,
+                response=response,
+                logger=logger,
+                exception=exception,
+            )
         structlog.contextvars.clear_contextvars()
 
     def prepare(self, request):
         from ipware import get_client_ip
 
         request_id = get_request_header(
             request, "x-request-id", "HTTP_X_REQUEST_ID"
@@ -73,15 +81,15 @@
     def process_exception(self, request, exception):
         if isinstance(exception, (Http404, PermissionDenied)):
             # We don't log an exception here, and we don't set that we handled
             # an error as we want the standard `request_finished` log message
             # to be emitted.
             return
 
-        setattr(request, "_raised_exception", True)
+        setattr(request, "_raised_exception", exception)
         self.bind_user_id(request)
         signals.bind_extra_request_failed_metadata.send(
             sender=self.__class__,
             request=request,
             logger=logger,
             exception=exception,
         )
```

### Comparing `django-structlog-5.0.2/django_structlog/signals.py` & `django-structlog-5.1.0/django_structlog/signals.py`

 * *Files 17% similar despite different names*

```diff
@@ -43,7 +43,26 @@
 >>> import structlog
 >>>
 >>> @receiver(signals.bind_extra_request_failed_metadata)
 ... def bind_user_email(request, logger, exception, **kwargs):
 ...     structlog.contextvars.bind_contextvars(user_email=getattr(request.user, 'email', ''))
 
 """
+
+update_failure_response = django.dispatch.Signal()
+""" Signal to update response failure response before it is returned.
+
+:param request: the request returned by the view
+:param response: the response resulting of the request
+:param logger: the logger
+:param exception: the exception
+
+>>> from django.dispatch import receiver
+>>> from django_structlog import signals
+>>> import structlog
+>>>
+>>> @receiver(signals.update_failure_response)
+... def add_request_id_to_error_response(request, response, logger, exception, **kwargs):
+...     context = structlog.contextvars.get_merged_contextvars(logger)
+...     response['X-Request-ID'] = context["request_id"]
+
+"""
```

### Comparing `django-structlog-5.0.2/django_structlog.egg-info/PKG-INFO` & `django-structlog-5.1.0/django_structlog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-structlog
-Version: 5.0.2
+Version: 5.1.0
 Summary: Structured Logging for Django
 Author-email: Jules Robichaud-Gagnon <j.robichaudg+pypi@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/jrobichaud/django-structlog
 Project-URL: repository, https://github.com/jrobichaud/django-structlog
 Project-URL: documentation, https://django-structlog.readthedocs.io
 Classifier: Framework :: Django
```

### Comparing `django-structlog-5.0.2/django_structlog.egg-info/SOURCES.txt` & `django-structlog-5.1.0/django_structlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-structlog-5.0.2/pyproject.toml` & `django-structlog-5.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -105,12 +105,12 @@
         redis4: redis>=4, <5
         kombu5: kombu<6
         celery51: Celery >=5.1, <5.2
         celery52: Celery >=5.2, <5.3
         django32: Django >=3.2, <4.0
         django40: Django >=4.0, <4.1
         django41: Django >=4.1, <4.2
-        django42: Django ==4.2rc1
+        django42: Django >=4.2, <5.0
         -r{toxinidir}/requirements/ci.txt
 
     commands = pytest --cov=./test_app --cov=./django_structlog --cov-append test_app
     """
```

